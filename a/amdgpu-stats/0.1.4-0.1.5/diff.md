# Comparing `tmp/amdgpu_stats-0.1.4.tar.gz` & `tmp/amdgpu_stats-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amdgpu_stats-0.1.4.tar", max compression
+gzip compressed data, was "amdgpu_stats-0.1.5.tar", max compression
```

## Comparing `amdgpu_stats-0.1.4.tar` & `amdgpu_stats-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2023-04-23 18:43:59.684481 amdgpu_stats-0.1.4/LICENSE.md
--rw-r--r--   0        0        0     2168 2023-04-25 03:23:00.570448 amdgpu_stats-0.1.4/README.md
--rw-r--r--   0        0        0      499 2023-04-25 03:23:00.570448 amdgpu_stats-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-23 21:03:33.649030 amdgpu_stats-0.1.4/src/amdgpu_stats/__init__.py
--rw-r--r--   0        0        0      393 2023-04-23 21:06:47.224510 amdgpu_stats-0.1.4/src/amdgpu_stats/amdgpu_stats.css
--rwxr-xr-x   0        0        0      343 2023-04-25 03:15:22.090179 amdgpu_stats-0.1.4/src/amdgpu_stats/amdgpu_stats.py
--rw-r--r--   0        0        0    11987 2023-04-25 03:15:22.090179 amdgpu_stats-0.1.4/src/amdgpu_stats/interface.py
--rw-r--r--   0        0        0     3665 2023-04-25 03:15:22.090179 amdgpu_stats-0.1.4/src/amdgpu_stats/utils.py
--rw-r--r--   0        0        0     3119 1970-01-01 00:00:00.000000 amdgpu_stats-0.1.4/setup.py
--rw-r--r--   0        0        0     2856 1970-01-01 00:00:00.000000 amdgpu_stats-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-23 18:43:59.684481 amdgpu_stats-0.1.5/LICENSE.md
+-rw-r--r--   0        0        0     1913 2023-04-25 06:19:53.715921 amdgpu_stats-0.1.5/README.md
+-rw-r--r--   0        0        0      499 2023-04-25 04:26:10.596531 amdgpu_stats-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-23 21:03:33.649030 amdgpu_stats-0.1.5/src/amdgpu_stats/__init__.py
+-rw-r--r--   0        0        0      393 2023-04-23 21:06:47.224510 amdgpu_stats-0.1.5/src/amdgpu_stats/amdgpu_stats.css
+-rwxr-xr-x   0        0        0      343 2023-04-25 03:15:22.090179 amdgpu_stats-0.1.5/src/amdgpu_stats/amdgpu_stats.py
+-rw-r--r--   0        0        0    10756 2023-04-25 06:24:41.875920 amdgpu_stats-0.1.5/src/amdgpu_stats/interface.py
+-rw-r--r--   0        0        0     6032 2023-04-25 06:14:10.223234 amdgpu_stats-0.1.5/src/amdgpu_stats/utils.py
+-rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 amdgpu_stats-0.1.5/setup.py
+-rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 amdgpu_stats-0.1.5/PKG-INFO
```

### Comparing `amdgpu_stats-0.1.4/LICENSE.md` & `amdgpu_stats-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `amdgpu_stats-0.1.4/README.md` & `amdgpu_stats-0.1.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: amdgpu-stats
+Version: 0.1.5
+Summary: A simple TUI (using Textual) that shows AMD GPU statistics
+Home-page: https://github.com/joshlay/amdgpu_stats
+License: MIT
+Author: Josh Lay
+Author-email: pypi@jlay.io
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: humanfriendly (>=10.0)
+Requires-Dist: textual (>=0.10)
+Project-URL: Repository, https://github.com/joshlay/amdgpu_stats
+Description-Content-Type: text/markdown
+
 # amdgpu_stats
 
 Simple TUI _(using [Textual](https://textual.textualize.io/))_ that shows AMD GPU statistics
 
 ![Screenshot of main screen](https://raw.githubusercontent.com/joshlay/amdgpu_stats/master/screens/main.png "Main screen")
 
 ![Screenshot of log screen](https://raw.githubusercontent.com/joshlay/amdgpu_stats/master/screens/logging.png "Logging screen")
@@ -27,26 +46,25 @@
 ```
 Once installed, run `amdgpu-stats` in your terminal of choice
 
 ## Module
 
 *Rudimentary* support as a module exists; functions / variables offered can be found in `amdgpu_stats.utils`
 
-Of most interest:
- - The function `find_card` which returns a tuple; the discovered card and hwmon directory
- - The variables `SRC_FILES` and `TEMP_FILES`, dictionaries of hwmon-driven statistics
-
-Example usage:
+Demonstration:
 ```
-In [1]: from amdgpu_stats.utils import find_card, SRC_FILES, TEMP_FILES
+In [1]: import amdgpu_stats.utils
 
-In [2]: print(find_card())
-('card0', '/sys/class/drm/card0/device/hwmon/hwmon9')
+In [2]: print(amdgpu_stats.utils.get_core_stats())
+{'sclk': 0, 'mclk': 1000000000, 'voltage': 0.01, 'util_pct': 0}
 
-In [3]: print(SRC_FILES)
-{'pwr_limit': '/sys/class/drm/card0/device/hwmon/hwmon9/power1_cap', 'pwr_average': '/sys/class/drm/card0/device/hwmon/hwmon9/power1_average',
-[...]
+In [3]: print(amdgpu_stats.utils.get_power_stats())
+{'limit': 281, 'average': 35, 'capability': 323, 'default': 281}
 
-In [4]: print(TEMP_FILES)
-{'edge': '/sys/class/drm/card0/device/hwmon/hwmon9/temp1_input', 'junction': '/sys/class/drm/card0/device/hwmon/hwmon9/temp2_input', 'mem': '/sys/class/drm/card0/device/hwmon/hwmon9/temp3_input'}
+In [4]: print(amdgpu_stats.utils.get_temp_stats())
+{'edge': 33, 'junction': 36, 'mem': 42}
+
+In [5]: print(amdgpu_stats.utils.get_fan_stats())
+{'fan_rpm': 0, 'fan_rpm_target': 0}
 ```
-_Latest_ [Source file](https://github.com/joshlay/amdgpu_stats/blob/master/src/amdgpu_stats/utils.py)
+See `help('amdgpu_stats.utils')` or [the module source](https://github.com/joshlay/amdgpu_stats/blob/master/src/amdgpu_stats/utils.py) for more info
+
```

### Comparing `amdgpu_stats-0.1.4/src/amdgpu_stats/interface.py` & `amdgpu_stats-0.1.5/src/amdgpu_stats/interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from textual.binding import Binding
 from textual.app import App, ComposeResult
 from textual.containers import Container, Horizontal
 from textual.reactive import reactive
 from textual.screen import Screen
 from textual.widgets import Header, Footer, Static, TextLog, Label
 
-from .utils import CARD, SRC_FILES, TEMP_FILES, format_frequency, read_stat
+from .utils import CARD, SRC_FILES, TEMP_FILES, format_frequency, get_core_stats, get_fan_stats, get_power_stats, get_temp_stats  # pylint: disable=line-too-long
 
 
 class LogScreen(Screen):
     """Creates a screen for the logging widget"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -116,16 +116,15 @@
     # used to make a 'reactive' object
     fan_stats = reactive({"fan_rpm": 0,
                           "fan_rpm_target": 0})
     temp_stats = reactive({})
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.timer_fan = None
-        self.timer_temp = None
+        self.timer_misc = None
 
     def compose(self) -> ComposeResult:
         yield Horizontal(Label("[underline]Temperatures"),
                          Label("", classes="statvalue"))
         for temp_node in TEMP_FILES:
             # capitalize the first letter for display
             caption = temp_node[0].upper() + temp_node[1:]
@@ -136,38 +135,22 @@
         yield Horizontal(Label("  Current:",),
                          Label("", id="fan_rpm", classes="statvalue"))
         yield Horizontal(Label("  Target:",),
                          Label("", id="fan_rpm_target", classes="statvalue"))
 
     def on_mount(self) -> None:
         """Event handler called when widget is added to the app."""
-        self.timer_fan = self.set_interval(1, self.update_fan_stats)
-        self.timer_temp = self.set_interval(1, self.update_temp_stats)
+        self.timer_misc = self.set_interval(1, self.update_misc_stats)
 
-    def update_fan_stats(self) -> None:
-        """Method to update the 'fan' values to current measurements.
+    def update_misc_stats(self) -> None:
+        """Method to update the temp/fan values to current measurements.
 
         Run by a timer created 'on_mount'"""
-        val_update = {
-                "fan_rpm": read_stat(SRC_FILES['fan_rpm']),
-                "fan_rpm_target": read_stat(SRC_FILES['fan_rpm_target'])
-        }
-        self.fan_stats = val_update
-
-    def update_temp_stats(self) -> None:
-        """Method to update the 'temperature' values to current measurements.
-
-        Run by a timer created 'on_mount'"""
-        val_update = {}
-        for temp_node, temp_file in TEMP_FILES.items():
-            # iterate through the discovered temperature nodes
-            # ... updating the dictionary with new stats
-            _content = f'{int(read_stat(temp_file)) / 1000:.0f}C'
-            val_update[temp_node] = _content
-        self.temp_stats = val_update
+        self.fan_stats = get_fan_stats()
+        self.temp_stats = get_temp_stats()
 
     def watch_fan_stats(self, fan_stats: dict) -> None:
         """Called when the 'fan_stats' reactive attr changes.
 
          - Updates label values
          - Casting inputs to string to avoid type problems w/ int/None"""
         self.query_one("#fan_rpm", Static).update(f"{fan_stats['fan_rpm']}")
@@ -175,15 +158,15 @@
 
     def watch_temp_stats(self, temp_stats: dict) -> None:
         """Called when the temp_stats reactive attr changes, updates labels"""
         for temp_node in TEMP_FILES:
             # check first if the reactive object has been updated with keys
             if temp_node in temp_stats:
                 stat_dict_item = temp_stats[temp_node]
-                self.query_one("#temp_" + temp_node, Static).update(stat_dict_item)
+                self.query_one("#temp_" + temp_node, Static).update(f'{stat_dict_item}C')
 
 
 class ClockDisplay(Static):
     """A widget to display GPU power stats."""
     core_vals = reactive({"sclk": 0, "mclk": 0, "voltage": 0, "util_pct": 0})
 
     def __init__(self, *args, **kwargs):
@@ -208,36 +191,28 @@
     def on_mount(self) -> None:
         """Event handler called when widget is added to the app."""
         self.timer_clocks = self.set_interval(1, self.update_core_vals)
 
     def update_core_vals(self) -> None:
         """Method to update GPU clock values to the current measurements.
         Run by a timer created 'on_mount'"""
-
-        self.core_vals = {
-            "sclk": format_frequency(read_stat(SRC_FILES['core_clock'])),
-            "mclk": format_frequency(read_stat(SRC_FILES['memory_clock'])),
-            "voltage": float(
-                f"{int(read_stat(SRC_FILES['core_voltage'])) / 1000:.2f}"
-            ),
-            "util_pct": read_stat(SRC_FILES['busy_pct']),
-        }
+        self.core_vals = get_core_stats()
 
     def watch_core_vals(self, core_vals: dict) -> None:
         """Called when the clocks attribute changes
          - Updates label values
          - Casting inputs to string to avoid type problems w/ int/None"""
         self.query_one("#clk_core_val",
-                       Static).update(f"{core_vals['sclk']}")
+                       Static).update(f"{format_frequency(core_vals['sclk'])}")
         self.query_one("#util_pct",
                        Static).update(f"{core_vals['util_pct']}%")
         self.query_one("#clk_voltage_val",
                        Static).update(f"{core_vals['voltage']}V")
         self.query_one("#clk_memory_val",
-                       Static).update(f"{core_vals['mclk']}")
+                       Static).update(f"{format_frequency(core_vals['mclk'])}")
 
 
 class PowerDisplay(Static):
     """A widget to display GPU power stats."""
 
     micro_watts = reactive({"limit": 0,
                             "average": 0,
@@ -267,20 +242,15 @@
         """Event handler called when widget is added to the app."""
         self.timer_micro_watts = self.set_interval(1, self.update_micro_watts)
 
     def update_micro_watts(self) -> None:
         """Method to update GPU power values to current measurements.
 
         Run by a timer created 'on_mount'"""
-        self.micro_watts = {
-            "limit": int(int(read_stat(SRC_FILES['pwr_limit'])) / 1000000),
-            "average": int(int(read_stat(SRC_FILES['pwr_average'])) / 1000000),
-            "capability": int(int(read_stat(SRC_FILES['pwr_cap'])) / 1000000),
-            "default": int(int(read_stat(SRC_FILES['pwr_default'])) / 1000000),
-        }
+        self.micro_watts = get_power_stats()
 
     def watch_micro_watts(self, micro_watts: dict) -> None:
         """Called when the micro_watts attributes change.
          - Updates label values
          - Casting inputs to string to avoid type problems w/ int/None"""
         self.query_one("#pwr_avg_val",
                        Static).update(f"{micro_watts['average']}W")
```

