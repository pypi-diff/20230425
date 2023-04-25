# Comparing `tmp/wiliot-tools-4.0.2.tar.gz` & `tmp/wiliot-tools-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-tools-4.0.2.tar", last modified: Mon Mar  6 13:32:18 2023, max compression
+gzip compressed data, was "wiliot-tools-4.0.4.tar", last modified: Tue Apr 25 08:36:10 2023, max compression
```

## Comparing `wiliot-tools-4.0.2.tar` & `wiliot-tools-4.0.4.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-06 13:32:18.908659 wiliot-tools-4.0.2/
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     2316 2023-03-06 13:32:18.908659 wiliot-tools-4.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1812 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)     7205 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      330 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-03-06 13:32:18.908659 wiliot-tools-4.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1821 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-06 13:32:18.900659 wiliot-tools-4.0.2/wiliot_tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/wiliot_tools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-06 13:32:18.900659 wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/
--rw-rw-rw-   0 root         (0) root         (0)     4010 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/feature_flags.py
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/local_gateway_gui.bat
--rw-rw-rw-   0 root         (0) root         (0)    83963 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/local_gateway_gui.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-06 13:32:18.908659 wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/utils/
--rw-rw-rw-   0 root         (0) root         (0)      639 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/utils/.gwCommands.json
--rw-rw-rw-   0 root         (0) root         (0)     4010 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17562 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/utils/custom_ep.ui
--rw-rw-rw-   0 root         (0) root         (0)    10355 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/utils/custom_plots.ui
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/utils/folder.png
--rw-rw-rw-   0 root         (0) root         (0)    26549 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/utils/gw_debugger.ui
--rw-rw-rw-   0 root         (0) root         (0)     4628 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/utils/gw_macros.py
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/wiliot_tools/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-06 13:32:18.908659 wiliot-tools-4.0.2/wiliot_tools/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/wiliot_tools/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6046 2023-03-06 13:32:09.000000 wiliot-tools-4.0.2/wiliot_tools/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-03-06 13:32:18.000000 wiliot-tools-4.0.2/wiliot_tools/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-06 13:32:18.900659 wiliot-tools-4.0.2/wiliot_tools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     2316 2023-03-06 13:32:18.000000 wiliot-tools-4.0.2/wiliot_tools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-03-06 13:32:18.000000 wiliot-tools-4.0.2/wiliot_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-06 13:32:18.000000 wiliot-tools-4.0.2/wiliot_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-06 13:32:18.000000 wiliot-tools-4.0.2/wiliot_tools.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-03-06 13:32:18.000000 wiliot-tools-4.0.2/wiliot_tools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       13 2023-03-06 13:32:18.000000 wiliot-tools-4.0.2/wiliot_tools.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:36:10.613059 wiliot-tools-4.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     2575 2023-04-25 08:36:10.613059 wiliot-tools-4.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     7205 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      330 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-25 08:36:10.613059 wiliot-tools-4.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:36:10.609059 wiliot-tools-4.0.4/wiliot_tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:36:10.609059 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/
+-rw-rw-rw-   0 root         (0) root         (0)     4010 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/feature_flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/local_gateway_gui.bat
+-rw-rw-rw-   0 root         (0) root         (0)    86343 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/local_gateway_gui.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:36:10.613059 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      639 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/.gwCommands.json
+-rw-rw-rw-   0 root         (0) root         (0)     4010 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/configs.gif
+-rw-rw-rw-   0 root         (0) root         (0)    17562 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/custom_ep.ui
+-rw-rw-rw-   0 root         (0) root         (0)    10355 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/custom_plots.ui
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/debug_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/folder.png
+-rw-rw-rw-   0 root         (0) root         (0)    28161 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/gw_debugger.ui
+-rw-rw-rw-   0 root         (0) root         (0)     4628 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/gw_macros.py
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:36:10.613059 wiliot-tools-4.0.4/wiliot_tools/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6046 2023-04-25 08:36:00.000000 wiliot-tools-4.0.4/wiliot_tools/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-25 08:36:10.000000 wiliot-tools-4.0.4/wiliot_tools/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:36:10.609059 wiliot-tools-4.0.4/wiliot_tools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     2575 2023-04-25 08:36:10.000000 wiliot-tools-4.0.4/wiliot_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2023-04-25 08:36:10.000000 wiliot-tools-4.0.4/wiliot_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-25 08:36:10.000000 wiliot-tools-4.0.4/wiliot_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-25 08:36:10.000000 wiliot-tools-4.0.4/wiliot_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-25 08:36:10.000000 wiliot-tools-4.0.4/wiliot_tools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-04-25 08:36:10.000000 wiliot-tools-4.0.4/wiliot_tools.egg-info/top_level.txt
```

### Comparing `wiliot-tools-4.0.2/LICENSE` & `wiliot-tools-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.0.2/PKG-INFO` & `wiliot-tools-4.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-tools
-Version: 4.0.2
+Version: 4.0.4
 Summary: A library for interacting with Wiliot's private tools
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -55,14 +55,22 @@
 * [Local Gateway GUI](wiliot_tools/local_gateway_gui/local_gateway_gui.py)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.0.4:
+-----------------
+* Gateway GUI
+    * add mode for printing full UID, advertising address
+    * show only Silicon Lab port as options for the gw GUI
+    * add button to print the macro file to create new macros.
+    * update GUI visualization
+
 Version 4.0.2:
 -----------------
 * First version
 
 
 The package previous content was published under the name 'wiliot' package.
 for more information please read 'wiliot' package's release notes
```

### Comparing `wiliot-tools-4.0.2/README.md` & `wiliot-tools-4.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -38,14 +38,22 @@
 * [Local Gateway GUI](wiliot_tools/local_gateway_gui/local_gateway_gui.py)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.0.4:
+-----------------
+* Gateway GUI
+    * add mode for printing full UID, advertising address
+    * show only Silicon Lab port as options for the gw GUI
+    * add button to print the macro file to create new macros.
+    * update GUI visualization
+
 Version 4.0.2:
 -----------------
 * First version
 
 
 The package previous content was published under the name 'wiliot' package.
 for more information please read 'wiliot' package's release notes
```

### Comparing `wiliot-tools-4.0.2/bitbucket-pipelines.yml` & `wiliot-tools-4.0.4/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.0.2/setup.py` & `wiliot-tools-4.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,13 +31,14 @@
                  install_requires=[
                      'setuptools_scm',
                      'pyserial',
                      'pandas',
                      'pygubu==0.16',
                      'bokeh==2.4.1',
                      'MarkupSafe==2.0.1',  # for bokeh
-                     'wiliot-core'
+                     'wiliot-api==4.1.0',
+                     'wiliot-core==4.0.8'
                  ],
                  zip_safe=False,
                  python_requires='>=3.6',
                  include_package_data=True,
                  )
```

### Comparing `wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/__init__.py` & `wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/local_gateway_gui.py` & `wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/local_gateway_gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,51 +53,67 @@
 #     FOR ANY LOSS OF USE OR DATA OR BUSINESS INTERRUPTION, AND/OR FOR ANY ECONOMIC LOSS
 #     (SUCH AS LOST PROFITS, REVENUE, ANTICIPATED SAVINGS). THE FOREGOING SHALL APPLY:
 #     (A) HOWEVER CAUSED AND REGARDLESS OF THE THEORY OR BASIS LIABILITY, WHETHER IN
 #     CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE);
 #     (B) EVEN IF ANYONE IS ADVISED OF THE POSSIBILITY OF ANY DAMAGES, LOSSES, OR COSTS; AND
 #     (C) EVEN IF ANY REMEDY FAILS OF ITS ESSENTIAL PURPOSE.
 #  """
-
+import signal
+import socket
+import subprocess
 from os.path import isfile, isdir
 from tkinter import Tk, INSERT, END, filedialog, Toplevel
 from tkinter.font import Font
 import serial.tools.list_ports
 import pygubu
 import json
 import os
+import sys
 import multiprocessing
 import logging
 import datetime
 import time
 import threading
 import pandas as pd
 import numpy as np
 import csv
 import re
 
 from wiliot_core import WiliotGateway, StatType, ActionType, DataType, valid_output_power_vals, valid_bb, \
-                        valid_sub1g_output_power
-from wiliot_core import TagCollection
+    valid_sub1g_output_power
+from wiliot_core import TagCollection, PacketList, Packet
 from wiliot_core import WiliotDir
-from wiliot_core import PacketList
-from wiliot_core import Packet
-from wiliot_tools.utils.get_version import get_version
 from wiliot_tools.local_gateway_gui.utils.gw_macros import macros
+from wiliot_tools.local_gateway_gui.utils.debug_mode import debug_flag
+
+from wiliot_tools.utils.get_version import get_version
 
 DECRYPTION_MODE = False
+
+
+def print_exceptions():
+    package_dir = os.path.dirname(os.path.dirname(__file__))
+    path = os.path.join(package_dir, "extended")
+
+    if (os.path.isfile(path) and os.path.getsize(path) > 0) or debug_flag['debug_bool']:
+        return True
+    return False
+
+
 try:
     from wiliot_core import DecryptedTagCollection
     from wiliot_tools.extended.pixie_analyzer.config_files.plot_config import plot_config
     from wiliot_tools.extended.pixie_analyzer.pixie_analyzer import PixieAnalyzer
+
     DECRYPTION_MODE = True
     print('Working on decrypted mode')
 except Exception as e:
-    # print('Working on encrypted mode') # SHOULD NOT BE PRINTED FOR PUBLIC USER!
-    # print(e) # SHOULD NOT BE PRINTED FOR PUBLIC USER!
+    if print_exceptions():
+        print('Working on encrypted mode')  # SHOULD NOT BE PRINTED FOR PUBLIC USER!
+        print(e)  # SHOULD NOT BE PRINTED FOR PUBLIC USER!
     pass
 
 try:  # live plots
     from wiliot_tools.local_gateway_gui.feature_flags import *
     from collections import deque
     import random
     import dash
@@ -120,15 +136,15 @@
 EPs_DEFAULT = (1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28,
                50, 51, 52)  # All Energizing pattern
 TP_O_DEFAULT = 5  # timing profile on
 TP_P_DEFAULT = 15  # timing profile period
 PI_DEFAULT = 0  # pace interval
 RC_DEFAULT = 37
 RCs_DEFAULT = (37, 38, 39)
-DATA_TYPES = ('raw', 'processed', 'statistics', 'decoded_packet')
+DATA_TYPES = ('raw', 'processed', 'statistics', 'full_UID_mode', 'decoded_packet')
 CONFIG_SUM = "EP:{EP}\nTP_ON:{TP_ON}\nTP_P:{TP_P}\nRC:{RC}\nPI:{PI}\nF:{F}"
 baud_rates = ["921600"]
 energy_pattern_dict = {18: 'Energizing on channel 39 only',
                        20: '20% channel 37 , 80% channel 39',
                        50: 'Energizing in 915Mhz',
                        51: 'Energizing on both channel 39 and 915Mhz',
                        }
@@ -158,24 +174,25 @@
         self.close_requested = False
         # check which mode we are:
         self.decryption_mode = DECRYPTION_MODE
         # 1: Create a builder
         self.builder = builder = pygubu.Builder()
         self.multi_tag = TagCollection()
         self.user_events = pd.DataFrame(columns=['user_event_time', 'user_event_data'])
-        self.filter_tag = ['']
+        self.filter_tag = [re.compile('')]
         self.data_handler_listener = None
-
+        self.UID_mode = False
         if self.decryption_mode:
             try:
                 self.myPixieAnalyzer = PixieAnalyzer()
                 self.packet_decoder = self.myPixieAnalyzer.PacketDecoder()
             except Exception as e:
                 self.myPixieAnalyzer = None
-                print('problem during loading PixieAnalyzer: {}'.format(e))
+                if print_exceptions():
+                    print('problem during loading PixieAnalyzer: {}'.format(e))
 
         self.env_dir = WiliotDir()
         self.logs_dir = os.path.join(self.env_dir.get_tester_dir("local_gateway_gui"), "logs")
         if not isdir(self.logs_dir):
             self.env_dir.create_dir(self.logs_dir)
 
         if LIVE_PLOTS_ENABLE:
@@ -232,15 +249,15 @@
         else:
             self.data_out = array_out
 
         self.ttk.lift()
         self.ttk.attributes("-topmost", True)
         self.ttk.attributes("-topmost", False)
 
-        self.ObjGW = WiliotGateway(logger_name='root', is_multi_processes=False)
+        self.ObjGW = WiliotGateway(logger_name='root')
         self.config_param = {}
         self.formatter = logging.Formatter('%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s', '%H:%M:%S')
         self.logger_num = 1
 
         # update ui
         if self.decryption_mode:
             self.decrypted_multi_tag = DecryptedTagCollection()
@@ -263,15 +280,20 @@
         self.ttk.protocol("WM_DELETE_WINDOW", self.close_window)
 
         self.ttk.after_idle(self.periodic_call)
         self.ttk.mainloop()
 
     @staticmethod
     def get_encrypted_ui(ui_path):
-        decrypted_guis = ['save_to_file', 'plot_log', 'load_log', 'custom_plots']
+        decrypted_guis = ['save_to_file', 'plot_log', 'load_log', 'custom_plots', 'packet_show_button',
+                          'analysis_plot_label', 'live_plot_label']
+        enc_ui_path = ui_path.replace('.ui', '_encrypted.ui')
+        if os.path.isfile(enc_ui_path):
+            return enc_ui_path
+
         with open(ui_path, 'r') as f:
             lines = f.readlines()
             new_lines = []
             need_to_del_section = False
             n_child = 0
             for line in lines:
                 if not need_to_del_section:
@@ -283,18 +305,18 @@
                     if 'child' in line:
                         n_child += 1
                     if n_child == 2:
                         need_to_del_section = False
                         n_child = 0
                 else:
                     new_lines.append(line)
-        new_ui_path = ui_path.replace('.ui', '_encrypted.ui')
-        with open(new_ui_path, 'w') as new_f:
+
+        with open(enc_ui_path, 'w') as new_f:
             new_f.writelines(new_lines)
-        return new_ui_path
+        return enc_ui_path
 
     def get_log_file_name(self, filename=None):
         if filename is None:
             filename = self.builder.get_object('log_path').get()
         if filename:
             filename = filename.strip("\u202a")  # strip left-to-right unicode if exists
             if os.path.isfile(filename):
@@ -303,22 +325,26 @@
         else:
             return None
 
     def get_filter_text(self, text=''):
         if len(text) > 0:
             text = text.replace(' ', '')
             self.filter_tag = text.split(',')
-            self.filter_tag = [f.lower() for f in self.filter_tag]
+            self.filter_tag = [re.compile(f.lower()) for f in self.filter_tag]
         else:
-            self.filter_tag = ['']
+            self.filter_tag = [re.compile('')]
 
     def is_filtered(self, packet):
         for f in self.filter_tag:
-            if f in packet.decoded_data['tag_id'].lower():
-                return True
+            if f.pattern.startswith('^'):
+                if f.search(packet.decoded_data['tag_id'][-4:].lower()):
+                    return True
+            else:
+                if f.search(packet.decoded_data['tag_id'].lower()):
+                    return True
         return False
 
     def close_window(self):
         self.close_requested = True
         print("User requested close at:", time.time(), "Was busy processing:", self.busy_processing)
 
     def periodic_call(self):
@@ -333,14 +359,15 @@
                 self.ObjGW.exit_gw_api()
                 if self.data_handler_listener is not None and self.data_handler_listener.is_alive():
                     self.data_handler_listener.join()
                 if LIVE_PLOTS_ENABLE:
                     self.live_plots_event.set()
                 if self.log_state:
                     logging.FileHandler(self.get_log_file_name()).close()
+                self.exit_packet_show()
                 self.ttk.destroy()
                 exit(0)
             except Exception as e:
                 print('problem during periodic call: {}'.format(e))
                 exit(1)
 
     def on_connect(self):
@@ -363,15 +390,15 @@
                     if 'command complete event' in rsp['raw'].lower():
                         self.config_param['pacer_val'] = '0'
                         self.config_param['filter'] = 'N'
                     # update UI:
                     self.ui_update('connect')
                     self.start_listening()
                     # update config:
-                    rsp = self.ObjGW.write('!pce', with_ack=True)
+                    rsp = self.ObjGW.write('!print_config_extended', with_ack=True)
                     if rsp['raw'] and 'unsupported' not in rsp['raw'].lower():
                         self.print_function(rsp['raw'])
                         self.from_gw_msg_to_config_param(rsp['raw'])
 
                 else:
                     self.print_function(str_in="> Can't open Port - check connection parameters and try again")
                     self.portActive = False
@@ -408,17 +435,19 @@
         # start listening:
         self.ObjGW.start_continuous_listener()
         if self.data_handler_listener is None or not self.data_handler_listener.is_alive():
             self.data_handler_listener = threading.Thread(target=self.recv_data_handler, args=())
             self.data_handler_listener.start()
 
     def on_search_ports(self):
-        self.ObjGW.available_ports = [s.device for s in serial.tools.list_ports.comports()]
+        self.ObjGW.available_ports = [s.device for s in serial.tools.list_ports.comports() if
+                                      'Silicon Labs' in s.description or 'CP210' in s.description]
         if len(self.ObjGW.available_ports) == 0:
-            self.ObjGW.available_ports = [s.name for s in serial.tools.list_ports.comports()]
+            self.ObjGW.available_ports = [s.name for s in serial.tools.list_ports.comports()
+                                          if 'Silicon Labs' in s.description or 'CP210' in s.description]
         # update ui:
         self.ui_update('available_ports')
 
     def on_send_to_additional_app(self):
         self.send_data_to_another_app = self.builder.get_variable('send_data_state').get()
         if self.send_data_to_another_app:
             self.print_function(str_in="> Send data to additional app via tcp/ip communication ({}:{})".format(
@@ -435,44 +464,56 @@
             try:
                 if self.close_requested or not self.portActive:
                     print("DataHandlerProcess Stop")
                     return
 
                 # check if there is data to read
                 if self.ObjGW.is_data_available():
-
+                    self.UID_mode = False
                     action_type = ActionType.ALL_SAMPLE
                     # get data
                     data_type = DataType.RAW
                     if self.builder.get_object('data_type').get() == 'raw':
                         data_type = DataType.RAW
                     elif self.builder.get_object('data_type').get() == 'processed':
                         data_type = DataType.PROCESSED
                     elif self.builder.get_object('data_type').get() == 'statistics':
                         data_type = DataType.PACKET_LIST
+                    elif self.builder.get_object('data_type').get() == 'full_UID_mode':
+                        self.UID_mode = True
+                        if self.decryption_mode:
+                            data_type = DataType.DECODED
+                        else:
+                            data_type = DataType.PACKET_LIST
                     elif self.builder.get_object('data_type').get() == 'decoded_packet' and self.decryption_mode:
                         data_type = DataType.DECODED
                     else:
                         data_type = DataType.PROCESSED
 
                     data_in = self.ObjGW.get_packets(action_type=action_type, num_of_packets=None,
                                                      data_type=data_type,
                                                      send_to_additional_app=self.send_data_to_another_app)
+
                     if data_type == DataType.PACKET_LIST:
+
                         for packet in data_in.packet_list:
-                            if any([f.lower() in packet.packet_data['adv_address'].lower() for f in self.filter_tag]):
-                                self.multi_tag.append(packet)
-                            else:
-                                continue
-                            # self.print_function(str_in=str(d))
+                            for f in self.filter_tag:
+                                if f.search(packet.packet_data['adv_address'].lower()):
+                                    self.multi_tag.append(packet)
+                                    if self.UID_mode:
+                                        self.print_function(str_in='AdvA: ' + str(packet.packet_data['adv_address']))
+                                else:
+                                    continue
+                                # self.print_function(str_in=str(d))
 
-                        if int((time.time() % 5)) == 0:
+                        if int((time.time() % 5)) == 0 and not self.UID_mode:
                             # self.on_clear(restart=False)
                             statistics_df = self.multi_tag.get_statistics_list()
                             all_data_str = statistics_df
+
                             self.print_function(str_in='---------------------- '
                                                        '{}: Tags Statistics '
                                                        '----------------------'.format(datetime.datetime.now()))
                             for d in all_data_str:
                                 self.print_function(str_in=str(d))
 
                     elif data_type == DataType.DECODED:
@@ -482,73 +523,88 @@
                             if self.is_filtered(packet):
                                 self.decrypted_multi_tag.append(packet)
 
                                 self.update_tags_count_label(self.decrypted_multi_tag.get_tags_count())
 
                                 if LIVE_PLOTS_ENABLE:
                                     if self.prev_packet_cntr != packet.decoded_data['packet_cntr']:
-                                        # if self.filter_tag[0] == packet.decoded_data[
-                                        #     'tag_id'].lower():  # self.filter_tag[0]
+
                                         try:
                                             for live_plots_attribute in LIVE_PLOTS_ATTRIBUTES:
                                                 if live_plots_attribute.lower() in packet.decoded_data.keys():
                                                     self.live_plots_data[live_plots_attribute]['X'].append(
                                                         packet.gw_data['time_from_start'].item(0))
                                                     self.live_plots_data[live_plots_attribute]['Y'].append(
                                                         packet.decoded_data[live_plots_attribute.lower()])
                                                     # self.Y.append(packet.decoded_data['packet_cntr'])
                                         except Exception as e:
                                             print(e)
                                     self.prev_packet_cntr = packet.decoded_data['packet_cntr']
                             else:
                                 continue
                             decrypted_packet = self.decrypted_multi_tag.get_last_added_packet()
-                            log_text = decrypted_packet.to_oneline_log()
+                            if self.UID_mode:
+                                try:
+                                    decrypted_packet_id = decrypted_packet.decoded_data['tag_id']
+                                    log_text = 'TagID: ' + decrypted_packet_id
+                                except Exception as e:
+                                    print("Couldn't decrypt packet")
+                            else:
+                                log_text = decrypted_packet.to_oneline_log()
                             if log_text is None:
                                 continue
 
                             self.print_function(log_text)
 
                             if self.send_data_to_another_app:
                                 packet_dict_to_main = {'time': decrypted_packet.gw_data['time_from_start'],
                                                        'raw': decrypted_packet.get_packet_string()}
                                 self.data_out.put(packet_dict_to_main)
 
                     else:
                         if data_type == DataType.PROCESSED:
                             for pkt in data_in:
-                                if any([f.lower() in pkt['adv_address'].lower() for f in self.filter_tag]):
-                                    data_str = []
-                                    for key, value in pkt.items():
-                                        data_str.append("{}:{}".format(key, value))
-                                    all_data_str = ','.join(data_str)
-                                    self.print_function(str_in=all_data_str)
-                                    # add it to the JTAG GUI if needed:
-                                    if self.send_data_to_another_app:
-                                        self.data_out.put(pkt)
-                                else:
-                                    continue
+                                for f in self.filter_tag:
+                                    if f.search(pkt['adv_address'].lower()):
+                                        data_str = []
+                                        for key, value in pkt.items():
+                                            data_str.append("{}:{}".format(key, value))
+                                        all_data_str = ','.join(data_str)
+                                        self.print_function(str_in=all_data_str)
+                                        # add it to the JTAG GUI if needed:
+                                        if self.send_data_to_another_app:
+                                            self.data_out.put(pkt)
+                                    else:
+                                        continue
                         if data_type == DataType.RAW:
                             for pkt in data_in:
                                 data_str = []
                                 for key, value in pkt.items():
+                                    # The 4 next rows are just to make 'time' with the same number of
+                                    # digits for all packets
+                                    if key == 'time':
+                                        value = '{:.6f}'.format(value)
                                     data_str.append("{}:{}".format(key, value))
                                 all_data_str = ','.join(data_str)
                                 self.print_function(str_in=all_data_str)
                                 # add it to the JTAG GUI if needed:
                                 if self.send_data_to_another_app:
                                     self.data_out.put(pkt)
                     consecutive_exception_counter = 0
             except Exception as e:
                 print("DataHandlerProcess Exception: {}".format(e))
                 consecutive_exception_counter = consecutive_exception_counter + 1
                 if consecutive_exception_counter > 10:
                     print("Abort DataHandlerProcess")
                     return
 
+    def on_macro_folder(self):
+        macro_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'utils', 'gw_macros.py')
+        self.print_function(str_in=f"> Go to {macro_path} to edit macros")
+
     def on_update_gw_version(self):
         self.print_function(str_in="> Updating GW version, please wait...")
         version_path_entry = self.builder.get_object('version_path').get()
         if version_path_entry:
             version_path_entry = version_path_entry.strip("\u202a")  # strip left-to-right unicode if exists
             if not os.path.isfile(version_path_entry):
                 self.print_function(str_in="> cannot find the entered gw version file:")
@@ -564,21 +620,62 @@
 
     def on_reset(self):
         self.ObjGW.reset_gw()
         time.sleep(1)
         self.ObjGW.write('!set_tester_mode 1', with_ack=True)
         self.ObjGW.reset_listener()
 
+    def exit_packet_show(self):
+        try:
+            # Check if the Bokeh server is already running on port 5006 and kill it
+            sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            result = sock.connect_ex(('localhost', 5006))  # bokeh port
+            if result == 0:
+                # Server is already running on port 5006, kill it and start a new server
+                if sys.platform == "darwin" or sys.platform == 'linux':
+                    p = subprocess.Popen(['lsof', '-i', ':5006'], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+                    out, err = p.communicate()
+                    pid = out.decode('utf-8').split('\n')[1].split()[1]
+                else:
+                    # windows
+                    p = os.popen('netstat -ano | findstr :5006')
+                    out = p.read()
+                    pid_list = list(set([pid.split(' ')[-1] for pid in out.split('\n') if '0.0.0.0:5006' in pid]))
+                    if len(pid_list) != 1:
+                        self.print_function("Could not decide which process to kill: {}".format(pid_list))
+                        return
+                    pid = pid_list[0]
+                os.kill(int(pid), signal.SIGILL)
+            # kill packet show if running:
+            os.kill(int(self.ObjGW.socket_port), signal.SIGILL)
+
+        except Exception as e:
+            self.print_function(f"Error during exit_packet_show: {e}")
+
+    def on_packet_show(self):
+        self.send_data_to_another_app = True
+        try:
+            # Check if the Bokeh server is already running on port 5006 and kill it
+            self.exit_packet_show()
+
+            # Server is not running on port 5006, start a new server and show the app
+            package_dir = os.path.dirname(os.path.abspath(os.path.dirname(__file__)))
+            path = os.path.join(package_dir, "extended", "packet_show", "packet_show.py")
+            subprocess.Popen(['bokeh', 'serve', '--port', '5006', '--show', path])
+
+        except Exception as e:
+            self.print_function(f"Error during on_packet_show: {e}")
+
     def on_enter_write(self, args):
         if args.char == '\r':
             self.on_write()
 
     def on_write(self):
         cmd_value = self.builder.get_object('write_box').get()
-        rsp_val = self.ObjGW.write(cmd_value, with_ack=True)
+        rsp_val = self.ObjGW.write(cmd_value, with_ack=True, max_time=0.100)
         self.on_user_event(user_event_text=cmd_value)
         self.print_function(', '.join(['{}: {}'.format(k, v) for k, v in rsp_val.items()]))
 
         if cmd_value.strip() not in list(self.builder.get_object('write_box')['values']):
             temp = list(self.builder.get_object('write_box')['values'])
 
             # keep only latest instances
@@ -591,14 +688,15 @@
             self.builder.get_object('write_box')['values'] = tuple(temp)
             with open(self.gwUserCommandsPath, 'w+') as f:
                 json.dump(self.gwUserCommands, f)
 
         self.ui_update(state='config')
 
     def on_run_macro(self):
+        from wiliot_tools.local_gateway_gui.utils.gw_macros import macros  # import again to check changes during run
         selected_macro = self.builder.get_object('macros_ddl').get()
         if selected_macro in macros.keys():
             data_handler_listener = threading.Thread(target=self.run_macro, args=())
             data_handler_listener.start()
         else:
             self.print_function("Please select a valid macro")
 
@@ -658,15 +756,16 @@
         self.config_param["filter"] = str(config_param_set.filter)[0]
 
         self.ui_update(state='config')
 
     def on_clear(self, restart=True):
         self.builder.get_object('recv_box').delete('1.0', END)
         self.builder.get_object('recv_box').see(END)
-        self.update_tags_count_label(0)
+        if self.decryption_mode:
+            self.update_tags_count_label(0)
         if restart:
             self.multi_tag = TagCollection()
             if self.decryption_mode:
                 self.decrypted_multi_tag = DecryptedTagCollection()
                 self.user_events = pd.DataFrame(columns=['user_event_time', 'user_event_data'])
                 if LIVE_PLOTS_ENABLE:
                     self.reset_live_plot()
@@ -722,23 +821,23 @@
             self.builder.get_object('log_path').insert(END, self.log_path)
             self.user_events = pd.DataFrame(columns=['user_event_time', 'user_event_data'])
 
     def on_autoscroll(self):
         self.autoscroll_state = self.builder.get_variable('autoscroll_state').get()
 
     def on_data_type_change(self, selected):
-        if selected.widget.get() == 'decoded_packet':
+        if selected.widget.get() == 'decoded_packet' or selected.widget.get() == 'full_UID_mode':
             self.builder.get_object('filter_id')['state'] = 'enabled'
+            self.builder.get_object('filter_id').delete(0, 'end')
             self.builder.get_object('filter_id').insert(0, 'filter ids')
             if self.decryption_mode:
                 self.builder.get_object('save_to_file')['state'] = 'enabled'
                 self.builder.get_object('plot_log')['state'] = 'enabled'
             self.on_clear()
 
-            self.update_tags_count_label(0)
         else:
             self.builder.get_object('filter_id').delete(0, 'end')
             self.builder.get_object('filter_id')['state'] = 'disabled'
             if self.decryption_mode:
                 self.builder.get_object('save_to_file')['state'] = 'disabled'
                 self.builder.get_object('plot_log')['state'] = 'disabled'
             self.update_tags_count_label(clear=True)
@@ -920,15 +1019,16 @@
     def return_time_str():
         now = datetime.datetime.now()
         # dd/mm/YY H:M:S
         dt_string = now.strftime("%d_%m_%Y__%H_%M_%S")
         return dt_string
 
     def on_processed_data(self, output_path=None):
-        if self.decryption_mode and self.builder.get_object('data_type').get() == 'decoded_packet':
+        if self.decryption_mode and (self.builder.get_object('data_type').get() == 'decoded_packet' or
+                                     self.builder.get_object('data_type').get() == 'full_UID_mode'):
             if len(self.decrypted_multi_tag) > 0:
                 if output_path is None:
                     csv_location = filedialog.asksaveasfilename(
                         filetypes=[("txt file", ".csv")], defaultextension=".csv", title='Choose location to save csv',
                         initialfile='{current_date}.csv'.format(current_date=self.return_time_str()))
                 else:
                     csv_location = output_path
@@ -956,39 +1056,32 @@
                 log_path = self.get_log_file_name()
             if '.log' in log_path:
                 user_event_location = log_path.replace('.log', '_user_event.csv')
             else:
                 user_event_location = log_path.replace('.csv', '_user_event.csv')
             self.user_events.to_csv(user_event_location, index=False)
             try:
-                if self.decryption_mode and self.builder.get_object('data_type').get() == 'decoded_packet':
-                    self.decrypted_multi_tag.to_csv(log_path.replace('.log', '_plot.csv'))
-                    self.print_function(
-                        str_in='export multi-tag csv - {path}'.format(
-                            path=log_path.replace('.log', '_plot.csv')))
-                    print(log_path.replace('.log', '_plot.csv'))
+                processed_log_path = log_path.replace('.log', '_packet_process.csv')
+                packet_list = self.extract_packet_list_from_log(log_path=log_path)
+                packet_list.to_csv(processed_log_path)
+                mt_processed_log_path = log_path.replace('.log', '_statistics_process.csv')
+                mt = TagCollection()
+                for packet in packet_list:
+                    mt.append(packet)
+                stat_df = mt.get_statistics()
+                stat_df.to_csv(path_or_buf=mt_processed_log_path)
+                # check if csv file was created
+                if isfile(processed_log_path):
+                    self.print_function('processed csv file was created: {}'.format(processed_log_path))
                 else:
-                    processed_log_path = log_path.replace('.log', '_packet_process.csv')
-                    packet_list = self.extract_packet_list_from_log(log_path=log_path)
-                    packet_list.to_csv(processed_log_path)
-                    mt_processed_log_path = log_path.replace('.log', '_statistics_process.csv')
-                    mt = TagCollection()
-                    for packet in packet_list:
-                        mt.append(packet)
-                    stat_df = mt.get_statistics()
-                    stat_df.to_csv(path_or_buf=mt_processed_log_path)
-                    # check if csv file was created
-                    if isfile(processed_log_path):
-                        self.print_function('processed csv file was created: {}'.format(processed_log_path))
-                    else:
-                        self.print_function('processed csv file was not created')
-                    if isfile(mt_processed_log_path):
-                        self.print_function('multi tag csv file was created: {}'.format(mt_processed_log_path))
-                    else:
-                        self.print_function('multi tag csv file was not created')
+                    self.print_function('processed csv file was not created')
+                if isfile(mt_processed_log_path):
+                    self.print_function('multi tag csv file was created: {}'.format(mt_processed_log_path))
+                else:
+                    self.print_function('multi tag csv file was not created')
             except Exception as e:
                 self.print_function('processed csv file was failed due to: {}'.format(e))
                 return
 
     def on_custom_ep(self):
         # open a new gui:
         tk_frame = Toplevel(self.ttk)
@@ -1116,17 +1209,19 @@
         path_loc = filedialog.askopenfilename(
             filetypes=[("txt file", ".zip")], defaultextension=".zip", title='Choose version file location')
         self.builder.get_object('version_path').delete(0, 'end')
         self.builder.get_object('version_path').insert(END, path_loc)
 
     def print_function(self, str_in):
         try:
-            self.builder.get_object('recv_box').insert(END, str_in + '\n')
+            recv_box = self.builder.get_object('recv_box')
+            recv_box.insert(END, str_in + '\n')
+            recv_box.config()
             if self.autoscroll_state:
-                self.builder.get_object('recv_box').see(END)
+                recv_box.see(END)
             if self.log_state:
                 self.logger.info(str_in)
         except Exception as e:
             print('print function failed due to: {}'.format(e))
 
     def init_live_plot(self):
         self.live_plots_event = threading.Event()
@@ -1244,19 +1339,14 @@
                 x=list(self.live_plots_data[LIVE_PLOTS_ATTRIBUTES[0]]['X']),
                 y=list(self.live_plots_data[LIVE_PLOTS_ATTRIBUTES[0]]['Y']),
                 name='lo_max_prox'.format(idx=0),
                 mode='lines+markers',
                 line={"color": "#f74242", },
             ))
 
-            # )
-            # takeClosest = lambda num, collection: min(collection, key=lambda x: abs(x - num))
-            # closest_x=takeClosest(max(self.live_plots_data[LIVE_PLOTS_ATTRIBUTES[0]]['X']) - LIVE_PLOTS_HISTORY,self.live_plots_data[LIVE_PLOTS_ATTRIBUTES[0]]['X'])
-            # closest_x_idx=self.live_plots_data['filter']['Y'].index(closest_x)
-            # closest_y=self.live_plots_data['filter']['Y'][closest_x_idx]
             try:
                 if len(self.live_plots_data['filter']['Y']) > LIVE_PLOTS_HISTORY:
                     y_range = [
                         min(list(self.live_plots_data['filter']['Y'])[-LIVE_PLOTS_HISTORY:]) - 2,
                         max(list(self.live_plots_data['filter']['Y'])[-LIVE_PLOTS_HISTORY:]) + 2]
                 else:
                     y_range = [
@@ -1282,51 +1372,14 @@
         @self.dash_app.callback(
             Output('live-graph-scatter-{idx}'.format(idx=1), 'figure'),
             [Input('graph-update', 'n_intervals')],
         )
         def update_graph_scatter(n):
             traces = []
 
-            # num_of_samples = 10
-            # threshold_mhz = 2480
-            # average_remaining = 0
-            #
-            # x_total = []
-            # y_total = []
-            #
-            # prox_x=list(self.live_plots_data[LIVE_PLOTS_ATTRIBUTES[0]]['X'])
-            # if len(list(self.live_plots_data[LIVE_PLOTS_ATTRIBUTES[0]]['X'])) > num_of_samples:
-            #     for i in range(0, len(prox_x), n):
-            #         chunk_x = prox_x[i:i + num_of_samples]
-            #         chunk_y = list(self.live_plots_data[LIVE_PLOTS_ATTRIBUTES[0]]['L'])[i:i + num_of_samples]
-            #
-            #         x_list = []
-            #         y_list = []
-            #         for y,y_idx in enumerate(chunk_y):
-            #             if y <= 2480:
-            #                 continue
-            #             y_list.append(y)
-            #             x_list.append(chunk_x[y_idx])
-            #
-            #             index_min = np.argmin(y_list)
-            #             index_max = np.argmin(y_list)
-            #             x_list.pop(index_min)
-            #             y_list.pop(index_min)
-            #             x_list.pop(index_max)
-            #             y_list.pop(index_max)
-            #
-            #             if len(y_list)>0:
-            #                 x_total.append(x_list[-1])
-            #                 y_total.append(np.average(y_list))
-            #
-            #
-
-            # y_total = list(self.live_plots_data[LIVE_PLOTS_ATTRIBUTES[0]]['Y'])
-            # x_total = list(self.live_plots_data[LIVE_PLOTS_ATTRIBUTES[0]]['X'])
-
             traces.append(plotly.graph_objs.Scatter(
                 x=list(self.live_plots_data[LIVE_PLOTS_ATTRIBUTES[1]]['X']),
                 y=list(self.live_plots_data[LIVE_PLOTS_ATTRIBUTES[1]]['Y']),
                 name='Scatter {idx}'.format(idx=1),
                 mode='lines+markers',
             ))
             try:
@@ -1430,15 +1483,15 @@
     def reset_live_plot(self):
         self.live_plots_data = {}
         self.print_function('Live plotting avaialbe in http://127.0.0.1:8050/')
         for live_plots_attribute in LIVE_PLOTS_ATTRIBUTES:
             self.live_plots_data[live_plots_attribute] = {'X': deque().copy(),
                                                           'Y': deque().copy()}
             self.live_plots_data['filter'] = {'X': deque().copy(),
-                                            'Y': deque().copy()}
+                                              'Y': deque().copy()}
             # self.live_plots_data[live_plots_attribute]['X'].append(0)
             # self.live_plots_data[live_plots_attribute]['Y'].append(0)
 
     def live_plot_task(self):
         self.dash_app.run_server(dev_tools_hot_reload=False, debug=False)
         while True:
             time.sleep(1)
```

### Comparing `wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/utils/.gwCommands.json` & `wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/.gwCommands.json`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/utils/__init__.py` & `wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/utils/custom_ep.ui` & `wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/custom_ep.ui`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/utils/custom_plots.ui` & `wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/custom_plots.ui`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/utils/gw_debugger.ui` & `wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/gw_debugger.ui`

 * *Files 5% similar despite different names*

#### Comparing `wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/utils/gw_debugger.ui` & `wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/gw_debugger.ui`

```diff
@@ -13,14 +13,15 @@
       <object class="ttk.Combobox" id="baud_rate_box">
         <property name="exportselection">true</property>
         <property name="state">disabled</property>
         <property name="width">10</property>
         <layout manager="grid">
           <property name="column">1</property>
           <property name="row">3</property>
+          <property name="sticky">w</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Label" id="baud_rate_name">
         <property name="text" translatable="yes">Baud Rate:</property>
         <layout manager="grid">
@@ -56,15 +57,15 @@
       <object class="ttk.Button" id="connect_button">
         <property cbtype="simple" name="command" type="command">on_connect</property>
         <property name="default">normal</property>
         <property name="text" translatable="yes">Connect</property>
         <property name="width">10</property>
         <layout manager="grid">
           <property name="column">0</property>
-          <property name="columnspan">4</property>
+          <property name="columnspan">3</property>
           <property name="row">0</property>
           <property name="sticky">ew</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="reset_button">
@@ -80,37 +81,37 @@
         </layout>
       </object>
     </child>
     <child>
       <object class="tk.Text" id="recv_box">
         <property name="autoseparators">true</property>
         <property name="blockcursor">false</property>
-        <property name="font">{San Francisco} 10 {}</property>
+        <property name="font">{Courier New} 9 {bold}</property>
         <property name="height">13</property>
         <property name="relief">flat</property>
         <property name="setgrid">false</property>
         <property name="takefocus">false</property>
         <property name="undo">false</property>
         <property name="width">120</property>
         <property name="wrap">char</property>
         <layout manager="grid">
           <property name="column">0</property>
-          <property name="columnspan">12</property>
+          <property name="columnspan">13</property>
           <property name="ipady">2</property>
           <property name="pady">10</property>
           <property name="row">9</property>
           <property name="sticky">nsew</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Scrollbar" id="scrollbar">
         <property name="orient">vertical</property>
         <layout manager="grid">
-          <property name="column">12</property>
+          <property name="column">13</property>
           <property name="row">9</property>
           <property name="sticky">nse</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Combobox" id="write_box">
@@ -139,15 +140,15 @@
     <child>
       <object class="ttk.Label" id="label1">
         <property name="font">{Segoe UI} 12 {bold}</property>
         <property name="text" translatable="yes">Wiliot's Local Gateway App</property>
         <layout manager="grid">
           <property name="column">3</property>
           <property name="columnspan">7</property>
-          <property name="row">11</property>
+          <property name="row">12</property>
           <property name="sticky">s</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Spinbox" id="timing_profile_on">
         <property name="from_">0</property>
@@ -191,14 +192,26 @@
           <property name="pady">5</property>
           <property name="row">6</property>
           <property name="sticky">ew</property>
         </layout>
       </object>
     </child>
     <child>
+      <object class="ttk.Button" id="packet_show_button">
+        <property cbtype="simple" name="command" type="command">on_packet_show</property>
+        <property name="text" translatable="yes">Live Packets Plot</property>
+        <property name="width">13</property>
+        <layout manager="grid">
+          <property name="column">9</property>
+          <property name="row">6</property>
+          <property name="sticky">ew</property>
+        </layout>
+      </object>
+    </child>
+    <child>
       <object class="ttk.Spinbox" id="pace_inter">
         <property name="from_">0</property>
         <property name="increment">1</property>
         <property name="state">disabled</property>
         <property name="to">1000</property>
         <property name="width">4</property>
         <layout manager="grid">
@@ -318,30 +331,28 @@
           <property name="sticky">ew</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Combobox" id="data_type">
         <property name="state">disabled</property>
-        <property name="width">10</property>
         <bind add="True" handler="on_data_type_change" sequence="&lt;&lt;ComboboxSelected&gt;&gt;"/>
         <layout manager="grid">
           <property name="column">10</property>
           <property name="row">2</property>
           <property name="sticky">ew</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Label" id="label9">
-        <property name="text" translatable="yes">data type</property>
+        <property name="text" translatable="yes">Data Type:</property>
         <layout manager="grid">
           <property name="column">9</property>
           <property name="row">2</property>
-          <property name="sticky">e</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="update_button">
         <property cbtype="simple" name="command" type="command">on_update_gw_version</property>
         <property name="state">disabled</property>
@@ -355,15 +366,15 @@
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="clear_button">
         <property cbtype="simple" name="command" type="command">on_clear</property>
         <property name="text" translatable="yes">Clear</property>
         <layout manager="grid">
-          <property name="column">11</property>
+          <property name="column">10</property>
           <property name="ipadx">5</property>
           <property name="row">10</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="search_ports_button">
@@ -382,15 +393,14 @@
       <object class="ttk.Entry" id="version_path">
         <property name="state">disabled</property>
         <layout manager="grid">
           <property name="column">0</property>
           <property name="columnspan">2</property>
           <property name="row">8</property>
           <property name="sticky">new</property>
-          <property id="8" name="pad" type="row">0</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="tk.Text" id="version_num">
         <property name="background">#f2f2f2</property>
         <property name="height">1</property>
@@ -438,20 +448,19 @@
       </object>
     </child>
     <child>
       <object class="ttk.Checkbutton" id="send_data">
         <property cbtype="simple" name="command" type="command">on_send_to_additional_app</property>
         <property name="offvalue">0</property>
         <property name="onvalue">1</property>
-        <property name="text" translatable="yes">Send data to additional app</property>
+        <property name="text" translatable="yes">TCP/IP</property>
         <property name="variable">boolean:send_data_state</property>
         <layout manager="grid">
           <property name="column">9</property>
-          <property name="columnspan">2</property>
-          <property name="row">3</property>
+          <property name="row">4</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Separator" id="separator2">
         <property name="orient">vertical</property>
         <layout manager="grid">
@@ -489,15 +498,16 @@
         <property name="offvalue">0</property>
         <property name="onvalue">1</property>
         <property name="text" translatable="yes">auto-scroll</property>
         <property name="variable">boolean:autoscroll_state</property>
         <layout manager="grid">
           <property name="column">11</property>
           <property name="columnspan">2</property>
-          <property name="row">11</property>
+          <property name="row">10</property>
+          <property name="sticky">ew</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="tk.Text" id="version_num_cur">
         <property name="background">#f2f2f2</property>
         <property name="height">1</property>
@@ -511,171 +521,208 @@
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="save_to_file">
         <property cbtype="simple" name="command" type="command">on_processed_data</property>
         <property name="text" translatable="yes">Save to File</property>
+        <property name="width">13</property>
         <layout manager="grid">
-          <property name="column">9</property>
-          <property name="columnspan">2</property>
-          <property name="row">4</property>
-          <property name="sticky">nsew</property>
+          <property name="column">10</property>
+          <property name="row">6</property>
+          <property name="sticky">ew</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Entry" id="filter_id">
         <property name="text" translatable="yes">filter ids</property>
         <bind add="True" handler="on_filter_id" sequence="&lt;Key&gt;"/>
         <layout manager="grid">
           <property name="column">9</property>
           <property name="row">10</property>
-          <property name="sticky">w</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="plot_log">
         <property cbtype="simple" name="command" type="command">on_plot_log</property>
         <property name="state">disabled</property>
         <property name="text" translatable="yes">Plot Current Data</property>
+        <property name="width">13</property>
         <layout manager="grid">
-          <property name="column">9</property>
-          <property name="columnspan">2</property>
-          <property name="row">6</property>
-          <property name="sticky">nsew</property>
+          <property name="column">10</property>
+          <property name="row">7</property>
+          <property name="sticky">ew</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="load_log">
         <property cbtype="simple" name="command" type="command">on_load_log</property>
         <property name="text" translatable="yes">Load and Plot Data</property>
+        <property name="width">13</property>
         <layout manager="grid">
-          <property name="column">9</property>
-          <property name="columnspan">2</property>
-          <property name="row">7</property>
-          <property name="sticky">nsew</property>
+          <property name="column">10</property>
+          <property name="row">8</property>
+          <property name="sticky">ew</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="tk.Text" id="tags_count">
         <property name="background">#f2f2f2</property>
         <property name="blockcursor">false</property>
         <property name="height">1</property>
         <property name="relief">flat</property>
         <property name="setgrid">false</property>
         <property name="width">16</property>
         <layout manager="grid">
-          <property name="column">10</property>
-          <property name="row">10</property>
-          <property name="sticky">e</property>
+          <property name="column">9</property>
+          <property name="row">11</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Combobox" id="macros_ddl">
         <property name="state">disabled</property>
         <property name="takefocus">false</property>
         <property name="width">40</property>
         <layout manager="grid">
           <property name="column">4</property>
           <property name="columnspan">3</property>
           <property name="row">8</property>
           <property name="sticky">new</property>
-          <property id="8" name="pad" type="row">0</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="run_macro">
         <property cbtype="simple" name="command" type="command">on_run_macro</property>
         <property name="state">disabled</property>
         <property name="text" translatable="yes">run</property>
         <layout manager="grid">
           <property name="column">7</property>
           <property name="row">8</property>
           <property name="sticky">new</property>
-          <property id="8" name="pad" type="row">0</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Label" id="label6">
         <property name="font">{San Francisco} 11 {bold}</property>
         <property name="text" translatable="yes">Macro</property>
         <layout manager="grid">
           <property name="column">4</property>
           <property name="row">7</property>
+          <property name="sticky">w</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="custom_plots">
         <property cbtype="simple" name="command" type="command">on_custom_plots</property>
-        <property name="text" translatable="yes">Plot Selection</property>
+        <property name="image">configs.gif</property>
+        <property name="style">Toolbutton</property>
+        <property name="text" translatable="yes">Plot Configuration</property>
+        <property name="width">13</property>
         <layout manager="grid">
-          <property name="column">9</property>
-          <property name="columnspan">2</property>
-          <property name="propagate">True</property>
+          <property name="column">11</property>
           <property name="row">5</property>
-          <property name="sticky">nsew</property>
+          <property name="sticky">w</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="user_event">
         <property cbtype="simple" name="command" type="command">on_user_event</property>
         <property name="state">normal</property>
         <property name="text" translatable="yes">User event</property>
         <layout manager="grid">
           <property name="column">9</property>
-          <property name="propagate">True</property>
-          <property name="row">8</property>
+          <property name="row">3</property>
           <property name="sticky">nsew</property>
-          <property id="8" name="pad" type="row">0</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Entry" id="user_event_text">
         <property name="text" translatable="yes">User Event Text</property>
         <layout manager="grid">
           <property name="column">10</property>
-          <property name="propagate">True</property>
-          <property name="row">8</property>
+          <property name="row">3</property>
           <property name="sticky">nsew</property>
-          <property id="8" name="pad" type="row">0</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="log_browser">
         <property cbtype="simple" name="command" type="command">on_log_browser</property>
         <property name="image">folder.png</property>
+        <property name="style">Toolbutton</property>
         <property name="width">1</property>
         <layout manager="grid">
           <property name="column">11</property>
-          <property name="ipadx">5</property>
-          <property name="propagate">True</property>
+          <property name="columnspan">2</property>
           <property name="row">1</property>
           <property name="sticky">w</property>
         </layout>
       </object>
     </child>
     <child>
       <object class="ttk.Button" id="version_browser">
         <property cbtype="simple" name="command" type="command">on_version_browser</property>
         <property name="image">folder.png</property>
+        <property name="style">Toolbutton</property>
         <layout manager="grid">
           <property name="column">2</property>
-          <property name="propagate">True</property>
           <property name="row">8</property>
           <property name="sticky">nw</property>
-          <property id="8" name="pad" type="row">0</property>
+        </layout>
+      </object>
+    </child>
+    <child>
+      <object class="ttk.Label" id="live_plot_label">
+        <property name="font">{San Francisco} 11 {bold}</property>
+        <property name="text" translatable="yes">Live Plot</property>
+        <layout manager="grid">
+          <property name="column">9</property>
+          <property name="row">5</property>
+        </layout>
+      </object>
+    </child>
+    <child>
+      <object class="ttk.Label" id="analysis_plot_label">
+        <property name="font">{San Francisco} 11 {bold}</property>
+        <property name="text" translatable="yes">Analysis Plot</property>
+        <layout manager="grid">
+          <property name="column">10</property>
+          <property name="row">5</property>
+        </layout>
+      </object>
+    </child>
+    <child>
+      <object class="ttk.Button" id="macro_button">
+        <property cbtype="simple" name="command" type="command">on_macro_folder</property>
+        <property name="image">folder.png</property>
+        <property name="style">Toolbutton</property>
+        <layout manager="grid">
+          <property name="column">6</property>
+          <property name="row">7</property>
+          <property name="sticky">e</property>
+        </layout>
+      </object>
+    </child>
+    <child>
+      <object class="ttk.Separator" id="separator1">
+        <property name="orient">vertical</property>
+        <layout manager="grid">
+          <property name="column">13</property>
+          <property name="propagate">True</property>
+          <property name="row">0</property>
+          <property name="rowspan">9</property>
+          <property name="sticky">ns</property>
         </layout>
       </object>
     </child>
   </object>
 </interface>
```

### Comparing `wiliot-tools-4.0.2/wiliot_tools/local_gateway_gui/utils/gw_macros.py` & `wiliot-tools-4.0.4/wiliot_tools/local_gateway_gui/utils/gw_macros.py`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.0.2/wiliot_tools/utils/get_version.py` & `wiliot-tools-4.0.4/wiliot_tools/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-tools-4.0.2/wiliot_tools.egg-info/PKG-INFO` & `wiliot-tools-4.0.4/wiliot_tools.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-tools
-Version: 4.0.2
+Version: 4.0.4
 Summary: A library for interacting with Wiliot's private tools
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -55,14 +55,22 @@
 * [Local Gateway GUI](wiliot_tools/local_gateway_gui/local_gateway_gui.py)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.0.4:
+-----------------
+* Gateway GUI
+    * add mode for printing full UID, advertising address
+    * show only Silicon Lab port as options for the gw GUI
+    * add button to print the macro file to create new macros.
+    * update GUI visualization
+
 Version 4.0.2:
 -----------------
 * First version
 
 
 The package previous content was published under the name 'wiliot' package.
 for more information please read 'wiliot' package's release notes
```

### Comparing `wiliot-tools-4.0.2/wiliot_tools.egg-info/SOURCES.txt` & `wiliot-tools-4.0.4/wiliot_tools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 wiliot_tools.egg-info/top_level.txt
 wiliot_tools/local_gateway_gui/__init__.py
 wiliot_tools/local_gateway_gui/feature_flags.py
 wiliot_tools/local_gateway_gui/local_gateway_gui.bat
 wiliot_tools/local_gateway_gui/local_gateway_gui.py
 wiliot_tools/local_gateway_gui/utils/.gwCommands.json
 wiliot_tools/local_gateway_gui/utils/__init__.py
+wiliot_tools/local_gateway_gui/utils/configs.gif
 wiliot_tools/local_gateway_gui/utils/custom_ep.ui
 wiliot_tools/local_gateway_gui/utils/custom_plots.ui
+wiliot_tools/local_gateway_gui/utils/debug_mode.py
 wiliot_tools/local_gateway_gui/utils/folder.png
 wiliot_tools/local_gateway_gui/utils/gw_debugger.ui
 wiliot_tools/local_gateway_gui/utils/gw_macros.py
 wiliot_tools/utils/__init__.py
 wiliot_tools/utils/get_version.py
```

