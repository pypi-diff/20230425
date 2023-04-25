# Comparing `tmp/pts_fault_injection-0.0.4.tar.gz` & `tmp/pts_fault_injection-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pts_fault_injection-0.0.4.tar", last modified: Mon Apr 24 18:33:37 2023, max compression
+gzip compressed data, was "dist/pts_fault_injection-0.0.5.tar", last modified: Tue Apr 25 13:18:11 2023, max compression
```

## Comparing `pts_fault_injection-0.0.4.tar` & `pts_fault_injection-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:33:37.000000 pts_fault_injection-0.0.4/
--rw-r--r--   0 root         (0) root         (0)     4002 2023-04-24 18:33:37.000000 pts_fault_injection-0.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-24 18:33:25.000000 pts_fault_injection-0.0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:33:37.000000 pts_fault_injection-0.0.4/pts_fault_injection.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4002 2023-04-24 18:33:37.000000 pts_fault_injection-0.0.4/pts_fault_injection.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2023-04-24 18:33:37.000000 pts_fault_injection-0.0.4/pts_fault_injection.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 18:33:37.000000 pts_fault_injection-0.0.4/pts_fault_injection.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-24 18:33:37.000000 pts_fault_injection-0.0.4/pts_fault_injection.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       92 2023-04-24 18:33:37.000000 pts_fault_injection-0.0.4/pts_fault_injection.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-24 18:33:25.000000 pts_fault_injection-0.0.4/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     3470 2023-04-24 18:33:25.000000 pts_fault_injection-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 18:33:37.000000 pts_fault_injection-0.0.4/pts_fault_injection/
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-24 18:33:25.000000 pts_fault_injection-0.0.4/pts_fault_injection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3083 2023-04-24 18:33:25.000000 pts_fault_injection-0.0.4/pts_fault_injection/fault_injection_box.py
--rw-rw-rw-   0 root         (0) root         (0)     8204 2023-04-24 18:33:25.000000 pts_fault_injection-0.0.4/pts_fault_injection/signal_card_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     7764 2023-04-24 18:33:25.000000 pts_fault_injection-0.0.4/pts_fault_injection/CANFWupdate.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-24 18:33:37.000000 pts_fault_injection-0.0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 13:18:11.000000 pts_fault_injection-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-04-25 13:18:11.000000 pts_fault_injection-0.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-25 13:18:00.000000 pts_fault_injection-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 13:18:11.000000 pts_fault_injection-0.0.5/pts_fault_injection.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-04-25 13:18:11.000000 pts_fault_injection-0.0.5/pts_fault_injection.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2023-04-25 13:18:11.000000 pts_fault_injection-0.0.5/pts_fault_injection.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 13:18:11.000000 pts_fault_injection-0.0.5/pts_fault_injection.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-25 13:18:11.000000 pts_fault_injection-0.0.5/pts_fault_injection.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2023-04-25 13:18:11.000000 pts_fault_injection-0.0.5/pts_fault_injection.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-25 13:18:00.000000 pts_fault_injection-0.0.5/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3470 2023-04-25 13:18:00.000000 pts_fault_injection-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 13:18:11.000000 pts_fault_injection-0.0.5/pts_fault_injection/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-25 13:18:00.000000 pts_fault_injection-0.0.5/pts_fault_injection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3083 2023-04-25 13:18:00.000000 pts_fault_injection-0.0.5/pts_fault_injection/fault_injection_box.py
+-rw-rw-rw-   0 root         (0) root         (0)     8385 2023-04-25 13:18:00.000000 pts_fault_injection-0.0.5/pts_fault_injection/signal_card_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     7764 2023-04-25 13:18:00.000000 pts_fault_injection-0.0.5/pts_fault_injection/CANFWupdate.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 13:18:11.000000 pts_fault_injection-0.0.5/setup.cfg
```

### Comparing `pts_fault_injection-0.0.4/PKG-INFO` & `pts_fault_injection-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts_fault_injection
-Version: 0.0.4
+Version: 0.0.5
 Summary: Fault Injection box Diagnostics package Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/pts-fault-injection-box
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_fault_injection-0.0.4/setup.py` & `pts_fault_injection-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="pts_fault_injection",
-    version="0.0.4",
+    version="0.0.5",
     author="Pass testing Solutions GmbH",
     description="Fault Injection box Diagnostics package Diagnostic Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="shuparna@pass-testing.de",
     url="https://gitlab.com/pass-testing-solutions/pts-fault-injection-box",
     license="MIT",
```

### Comparing `pts_fault_injection-0.0.4/pts_fault_injection.egg-info/PKG-INFO` & `pts_fault_injection-0.0.5/pts_fault_injection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pts-fault-injection
-Version: 0.0.4
+Version: 0.0.5
 Summary: Fault Injection box Diagnostics package Diagnostic Package
 Home-page: https://gitlab.com/pass-testing-solutions/pts-fault-injection-box
 Author: Pass testing Solutions GmbH
 Author-email: shuparna@pass-testing.de
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pts_fault_injection-0.0.4/LICENSE.txt` & `pts_fault_injection-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pts_fault_injection-0.0.4/README.md` & `pts_fault_injection-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pts_fault_injection-0.0.4/pts_fault_injection/fault_injection_box.py` & `pts_fault_injection-0.0.5/pts_fault_injection/fault_injection_box.py`

 * *Files identical despite different names*

### Comparing `pts_fault_injection-0.0.4/pts_fault_injection/signal_card_controller.py` & `pts_fault_injection-0.0.5/pts_fault_injection/signal_card_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import sys
 from cantools.database.can.signal import NamedSignalValue
 
 '''
 Please Define Board to test here !!!!
 '''
-dac_setpoints = dac_setpoints = [-1, -1, -1, -1, -1, -1, -1, -1]  # 8 DAC Channels
+dac_setpoints = [-1, -1, -1, -1, -1, -1, -1, -1]  # 8 DAC Channels
 
 dac_mapping = {0: 9,
                1: 1,
                2: 5,
                3: 3,
                4: 4,
                5: 5,
@@ -163,14 +163,18 @@
         used_ports = list(range(32)) + list(range(32, 39)) + list(range(40, 48))  # zero based
         self.check_card(4, used_ports)
 
     def test_bus_signal_card(self):
         used_ports = list(range(3 * 16))  # zero based
         self.check_card(5, used_ports)
 
+    def test_hv_signal_card(self):
+        used_ports = list(range(4)) + list(range(16, 32))  # zero based
+        self.check_card(6, used_ports)
+
     def test_lb_contactor_card(self):
         used_ports = list(range(21))  # zero based
         self.check_card(9, used_ports)
 
     def test_cell_fault_board(self):
         for cell in range(18):
             print(f"Testing Open Circuit on cell {cell}")
@@ -190,14 +194,15 @@
         funcs = {
             "AnalogSignal": self.test_analog_signal_card,
             "StandardSignal1": self.test_standard_signal_card1,
             "StandardSignal2": self.test_standard_signal_card2,
             "StandardSignal3": self.test_standard_signal_card3,
             "StandardSignal4": self.test_standard_signal_card4,
             "BusSignal": self.test_bus_signal_card,
+            "HVSignal": self.test_hv_signal_card,
             "CellFault": self.test_cell_fault_board,
             "LoadboxContactorCard": self.test_lb_contactor_card
         }
         if card in funcs:
             print(f"TESTING BOARD {card}")
             funcs[card]()
         else:
```

### Comparing `pts_fault_injection-0.0.4/pts_fault_injection/CANFWupdate.py` & `pts_fault_injection-0.0.5/pts_fault_injection/CANFWupdate.py`

 * *Files identical despite different names*

