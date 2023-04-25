# Comparing `tmp/amdgpu_stats-0.1.2.tar.gz` & `tmp/amdgpu_stats-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amdgpu_stats-0.1.2.tar", max compression
+gzip compressed data, was "amdgpu_stats-0.1.3.tar", max compression
```

## Comparing `amdgpu_stats-0.1.2.tar` & `amdgpu_stats-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1065 2023-04-23 18:43:59.684481 amdgpu_stats-0.1.2/LICENSE.md
--rw-r--r--   0        0        0     1360 2023-04-23 22:42:12.010831 amdgpu_stats-0.1.2/README.md
--rw-r--r--   0        0        0      503 2023-04-23 22:39:45.000000 amdgpu_stats-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-23 21:03:33.649030 amdgpu_stats-0.1.2/src/amdgpu_stats/__init__.py
--rw-r--r--   0        0        0      393 2023-04-23 21:06:47.224510 amdgpu_stats-0.1.2/src/amdgpu_stats/amdgpu_stats.css
--rwxr-xr-x   0        0        0    14918 2023-04-23 21:43:40.480892 amdgpu_stats-0.1.2/src/amdgpu_stats/amdgpu_stats.py
--rw-r--r--   0        0        0     2283 1970-01-01 00:00:00.000000 amdgpu_stats-0.1.2/setup.py
--rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 amdgpu_stats-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-23 18:43:59.684481 amdgpu_stats-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0     2085 2023-04-25 02:36:00.275489 amdgpu_stats-0.1.3/README.md
+-rw-r--r--   0        0        0      499 2023-04-25 02:24:07.844893 amdgpu_stats-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-23 21:03:33.649030 amdgpu_stats-0.1.3/src/amdgpu_stats/__init__.py
+-rw-r--r--   0        0        0      393 2023-04-23 21:06:47.224510 amdgpu_stats-0.1.3/src/amdgpu_stats/amdgpu_stats.css
+-rwxr-xr-x   0        0        0      343 2023-04-25 02:22:05.604957 amdgpu_stats-0.1.3/src/amdgpu_stats/amdgpu_stats.py
+-rw-r--r--   0        0        0    11987 2023-04-25 02:57:45.178855 amdgpu_stats-0.1.3/src/amdgpu_stats/interface.py
+-rw-r--r--   0        0        0     3665 2023-04-25 03:04:43.241156 amdgpu_stats-0.1.3/src/amdgpu_stats/utils.py
+-rw-r--r--   0        0        0     3035 1970-01-01 00:00:00.000000 amdgpu_stats-0.1.3/setup.py
+-rw-r--r--   0        0        0     2773 1970-01-01 00:00:00.000000 amdgpu_stats-0.1.3/PKG-INFO
```

### Comparing `amdgpu_stats-0.1.2/LICENSE.md` & `amdgpu_stats-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `amdgpu_stats-0.1.2/src/amdgpu_stats/amdgpu_stats.py` & `amdgpu_stats-0.1.3/src/amdgpu_stats/interface.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,33 @@
-#!/usr/bin/python3
-"""Pretty Textual-based stats for AMD GPUs
+"""
+interface.py
+
+This module provides the TUI aspect of 'amdgpu-stats'
 
-TODO: restore argparse / --card, in case detection fails.
-      will require separating the hwmon finding tasks from 'find_card'
+Classes:
+    - GPUStats: the object for the _Application_, instantiated at runtime
+    - GPUStatsWidget: the primary container for the three stat widgets:
+        - MiscDisplay
+        - ClockDisplay
+        - PowerDisplay
+    - LogScreen: Second screen with the logging widget, header, and footer
 
-rich markup reference:
-    https://rich.readthedocs.io/en/stable/markup.html
+Functions:
+    - tui: Renders the TUI using the classes above
 """
-from os import path
-import glob
 import sys
-from typing import Tuple, Optional
 
 from textual.binding import Binding
 from textual.app import App, ComposeResult
 from textual.containers import Container, Horizontal
 from textual.reactive import reactive
 from textual.screen import Screen
 from textual.widgets import Header, Footer, Static, TextLog, Label
-from humanfriendly import format_size
-
 
-# function to find the card / hwmon_dir -- assigned to vars, informs consts
-def find_card() -> Optional[Tuple[Optional[str], Optional[str]]]:
-    """searches contents of /sys/class/drm/card*/device/hwmon/hwmon*/name
-
-    looking for 'amdgpu' to find a card to monitor
-
-    returns the cardN name and hwmon directory for stats"""
-    _card = None
-    _hwmon_dir = None
-    hwmon_names_glob = '/sys/class/drm/card*/device/hwmon/hwmon*/name'
-    hwmon_names = glob.glob(hwmon_names_glob)
-    for hwmon_name_file in hwmon_names:
-        with open(hwmon_name_file, "r", encoding="utf-8") as _f:
-            if _f.read().strip() == 'amdgpu':
-                # found an amdgpu
-                # note: if multiple are found, last will be used/watched
-                # will be configurable in the future, may prompt
-                _card = hwmon_name_file.split('/')[4]
-                _hwmon_dir = path.dirname(hwmon_name_file)
-    return _card, _hwmon_dir
-
-
-# globals - card, hwmon directory, and statistic file paths derived from these
-CARD, hwmon_dir = find_card()
-card_dir = path.join("/sys/class/drm/", CARD)  # eg: /sys/class/drm/card0/
-# ref: https://docs.kernel.org/gpu/amdgpu/thermal.html
-SRC_FILES = {'pwr_limit': path.join(hwmon_dir, "power1_cap"),
-             'pwr_average': path.join(hwmon_dir, "power1_average"),
-             'pwr_cap': path.join(hwmon_dir, "power1_cap_max"),
-             'pwr_default': path.join(hwmon_dir, "power1_cap_default"),
-             'core_clock': path.join(hwmon_dir, "freq1_input"),
-             'core_voltage': path.join(hwmon_dir, "in0_input"),
-             'memory_clock': path.join(hwmon_dir, "freq2_input"),
-             'busy_pct': path.join(card_dir, "device/gpu_busy_percent"),
-             'temp_c': path.join(hwmon_dir, "temp1_input"),
-             'fan_rpm': path.join(hwmon_dir, "fan1_input"),
-             'fan_rpm_target': path.join(hwmon_dir, "fan1_target"),
-             }
-TEMP_FILES = {}
-# determine temperature nodes, construct an empty dict to store them
-temp_node_labels = glob.glob(path.join(hwmon_dir, "temp*_label"))
-for temp_node_label_file in temp_node_labels:
-    # determine the base node id, eg: temp1
-    # construct the path to the file that will label it. ie: edge/junction
-    temp_node_id = path.basename(temp_node_label_file).split('_')[0]
-    temp_node_value_file = path.join(hwmon_dir, f"{temp_node_id}_input")
-    with open(temp_node_label_file, 'r', encoding='utf-8') as _node:
-        temp_node_name = _node.read().strip()
-    # add the node name/type and the corresponding temp file to the dict
-    TEMP_FILES[temp_node_name] = temp_node_value_file
-
-
-def read_stat(file: str) -> str:
-    """given `file`, return the contents"""
-    with open(file, "r", encoding="utf-8") as _fh:
-        data = _fh.read().strip()
-        return data
-
-
-def format_frequency(frequency_hz) -> str:
-    """takes a frequency and formats it with an appropriate Hz suffix"""
-    return (
-        format_size(int(frequency_hz), binary=False)
-        .replace("B", "Hz")
-        .replace("bytes", "Hz")
-    )
+from .utils import CARD, SRC_FILES, TEMP_FILES, format_frequency, read_stat
 
 
 class LogScreen(Screen):
     """Creates a screen for the logging widget"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -285,18 +222,22 @@
             "util_pct": read_stat(SRC_FILES['busy_pct']),
         }
 
     def watch_core_vals(self, core_vals: dict) -> None:
         """Called when the clocks attribute changes
          - Updates label values
          - Casting inputs to string to avoid type problems w/ int/None"""
-        self.query_one("#clk_core_val", Static).update(f"{core_vals['sclk']}")
-        self.query_one("#util_pct", Static).update(f"{core_vals['util_pct']}%")
-        self.query_one("#clk_voltage_val", Static).update(f"{core_vals['voltage']}V")
-        self.query_one("#clk_memory_val", Static).update(f"{core_vals['mclk']}")
+        self.query_one("#clk_core_val",
+                       Static).update(f"{core_vals['sclk']}")
+        self.query_one("#util_pct",
+                       Static).update(f"{core_vals['util_pct']}%")
+        self.query_one("#clk_voltage_val",
+                       Static).update(f"{core_vals['voltage']}V")
+        self.query_one("#clk_memory_val",
+                       Static).update(f"{core_vals['mclk']}")
 
 
 class PowerDisplay(Static):
     """A widget to display GPU power stats."""
 
     micro_watts = reactive({"limit": 0,
                             "average": 0,
@@ -337,29 +278,23 @@
             "default": int(int(read_stat(SRC_FILES['pwr_default'])) / 1000000),
         }
 
     def watch_micro_watts(self, micro_watts: dict) -> None:
         """Called when the micro_watts attributes change.
          - Updates label values
          - Casting inputs to string to avoid type problems w/ int/None"""
-        self.query_one("#pwr_avg_val", Static).update(f"{micro_watts['average']}W")
-        self.query_one("#pwr_lim_val", Static).update(f"{micro_watts['limit']}W")
-        self.query_one("#pwr_def_val", Static).update(f"{micro_watts['default']}W")
-        self.query_one("#pwr_cap_val", Static).update(f"{micro_watts['capability']}W")
+        self.query_one("#pwr_avg_val",
+                       Static).update(f"{micro_watts['average']}W")
+        self.query_one("#pwr_lim_val",
+                       Static).update(f"{micro_watts['limit']}W")
+        self.query_one("#pwr_def_val",
+                       Static).update(f"{micro_watts['default']}W")
+        self.query_one("#pwr_cap_val",
+                       Static).update(f"{micro_watts['capability']}W")
 
 
 def tui() -> None:
     '''Spawns the textual UI only during CLI invocation / after argparse'''
-    app = GPUStats()
-    app.run()
-
-
-def main():
-    '''Main function, entrypoint for packaging'''
-    # exit if AMDGPU not found, otherwise - proceed, assigning stat files
     if CARD is None:
         sys.exit('Could not find an AMD GPU, exiting.')
-    tui()
-
-
-if __name__ == "__main__":
-    main()
+    app = GPUStats()
+    app.run()
```

