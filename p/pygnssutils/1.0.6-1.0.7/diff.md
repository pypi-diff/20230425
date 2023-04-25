# Comparing `tmp/pygnssutils-1.0.6.tar.gz` & `tmp/pygnssutils-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygnssutils-1.0.6.tar", last modified: Tue Apr  4 09:48:23 2023, max compression
+gzip compressed data, was "pygnssutils-1.0.7.tar", last modified: Tue Apr 25 08:37:22 2023, max compression
```

## Comparing `pygnssutils-1.0.6.tar` & `pygnssutils-1.0.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-04 09:48:23.358410 pygnssutils-1.0.6/
--rw-r--r--   0 steve      (501) staff       (20)     1613 2022-05-26 12:22:57.000000 pygnssutils-1.0.6/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)       64 2022-05-26 12:22:57.000000 pygnssutils-1.0.6/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)    24090 2023-04-04 09:48:23.358248 pygnssutils-1.0.6/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)    21117 2023-03-23 11:19:25.000000 pygnssutils-1.0.6/README.md
--rw-r--r--   0 steve      (501) staff       (20)     2578 2023-04-04 09:44:36.000000 pygnssutils-1.0.6/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-04-04 09:48:23.358453 pygnssutils-1.0.6/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-04 09:48:23.354316 pygnssutils-1.0.6/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-04 09:48:23.356634 pygnssutils-1.0.6/src/pygnssutils/
--rw-r--r--   0 steve      (501) staff       (20)      720 2023-03-23 22:14:27.000000 pygnssutils-1.0.6/src/pygnssutils/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      161 2023-04-04 09:44:36.000000 pygnssutils-1.0.6/src/pygnssutils/_version.py
--rw-r--r--   0 steve      (501) staff       (20)      297 2023-03-23 22:14:27.000000 pygnssutils-1.0.6/src/pygnssutils/exceptions.py
--rw-r--r--   0 steve      (501) staff       (20)     1712 2023-03-23 22:14:27.000000 pygnssutils-1.0.6/src/pygnssutils/globals.py
--rw-r--r--   0 steve      (501) staff       (20)    25291 2023-03-23 22:14:27.000000 pygnssutils-1.0.6/src/pygnssutils/gnssdump.py
--rw-r--r--   0 steve      (501) staff       (20)    17488 2023-03-23 22:14:27.000000 pygnssutils-1.0.6/src/pygnssutils/gnssmqttclient.py
--rw-r--r--   0 steve      (501) staff       (20)    24039 2023-03-23 22:14:27.000000 pygnssutils-1.0.6/src/pygnssutils/gnssntripclient.py
--rw-r--r--   0 steve      (501) staff       (20)    13830 2023-03-23 22:14:27.000000 pygnssutils-1.0.6/src/pygnssutils/gnssserver.py
--rw-r--r--   0 steve      (501) staff       (20)     4030 2023-04-04 09:44:36.000000 pygnssutils-1.0.6/src/pygnssutils/helpers.py
--rw-r--r--   0 steve      (501) staff       (20)    12995 2023-03-23 22:14:27.000000 pygnssutils-1.0.6/src/pygnssutils/socket_server.py
--rw-r--r--   0 steve      (501) staff       (20)     8922 2023-03-23 22:14:27.000000 pygnssutils-1.0.6/src/pygnssutils/ubxload.py
--rw-r--r--   0 steve      (501) staff       (20)    10941 2023-03-23 22:14:27.000000 pygnssutils-1.0.6/src/pygnssutils/ubxsave.py
--rw-r--r--   0 steve      (501) staff       (20)     7027 2023-03-23 22:14:27.000000 pygnssutils-1.0.6/src/pygnssutils/ubxsetrate.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-04 09:48:23.357459 pygnssutils-1.0.6/src/pygnssutils.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    24090 2023-04-04 09:48:23.000000 pygnssutils-1.0.6/src/pygnssutils.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      755 2023-04-04 09:48:23.000000 pygnssutils-1.0.6/src/pygnssutils.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-04-04 09:48:23.000000 pygnssutils-1.0.6/src/pygnssutils.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)      307 2023-04-04 09:48:23.000000 pygnssutils-1.0.6/src/pygnssutils.egg-info/entry_points.txt
--rw-r--r--   0 steve      (501) staff       (20)      161 2023-04-04 09:48:23.000000 pygnssutils-1.0.6/src/pygnssutils.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)       12 2023-04-04 09:48:23.000000 pygnssutils-1.0.6/src/pygnssutils.egg-info/top_level.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-04 09:48:23.357983 pygnssutils-1.0.6/tests/
--rw-r--r--   0 steve      (501) staff       (20)     9077 2023-03-28 06:51:04.000000 pygnssutils-1.0.6/tests/test_gnssdump.py
--rw-r--r--   0 steve      (501) staff       (20)    27168 2023-03-28 06:51:04.000000 pygnssutils-1.0.6/tests/test_sourcetable.py
--rw-r--r--   0 steve      (501) staff       (20)     4034 2023-03-28 06:51:04.000000 pygnssutils-1.0.6/tests/test_static.py
--rw-r--r--   0 steve      (501) staff       (20)     3492 2023-03-28 06:51:04.000000 pygnssutils-1.0.6/tests/test_stream.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-25 08:37:22.495053 pygnssutils-1.0.7/
+-rw-r--r--   0 steve      (501) staff       (20)     1613 2022-05-26 12:22:57.000000 pygnssutils-1.0.7/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)       64 2022-05-26 12:22:57.000000 pygnssutils-1.0.7/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)    24113 2023-04-25 08:37:22.494872 pygnssutils-1.0.7/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)    21117 2023-03-23 11:19:25.000000 pygnssutils-1.0.7/README.md
+-rw-r--r--   0 steve      (501) staff       (20)     2934 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-04-25 08:37:22.495106 pygnssutils-1.0.7/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-25 08:37:22.490402 pygnssutils-1.0.7/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-25 08:37:22.493075 pygnssutils-1.0.7/src/pygnssutils/
+-rw-r--r--   0 steve      (501) staff       (20)      704 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      161 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)      297 2023-03-23 22:14:27.000000 pygnssutils-1.0.7/src/pygnssutils/exceptions.py
+-rw-r--r--   0 steve      (501) staff       (20)     1712 2023-03-23 22:14:27.000000 pygnssutils-1.0.7/src/pygnssutils/globals.py
+-rw-r--r--   0 steve      (501) staff       (20)    25351 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/gnssdump.py
+-rw-r--r--   0 steve      (501) staff       (20)    17471 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/gnssmqttclient.py
+-rw-r--r--   0 steve      (501) staff       (20)    24022 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/gnssntripclient.py
+-rw-r--r--   0 steve      (501) staff       (20)    13831 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/gnssserver.py
+-rw-r--r--   0 steve      (501) staff       (20)     4030 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/helpers.py
+-rw-r--r--   0 steve      (501) staff       (20)    12997 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/socket_server.py
+-rw-r--r--   0 steve      (501) staff       (20)     8924 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/ubxload.py
+-rw-r--r--   0 steve      (501) staff       (20)    10943 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/ubxsave.py
+-rw-r--r--   0 steve      (501) staff       (20)     7008 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/src/pygnssutils/ubxsetrate.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-25 08:37:22.493904 pygnssutils-1.0.7/src/pygnssutils.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    24113 2023-04-25 08:37:22.000000 pygnssutils-1.0.7/src/pygnssutils.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      755 2023-04-25 08:37:22.000000 pygnssutils-1.0.7/src/pygnssutils.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-04-25 08:37:22.000000 pygnssutils-1.0.7/src/pygnssutils.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)      307 2023-04-25 08:37:22.000000 pygnssutils-1.0.7/src/pygnssutils.egg-info/entry_points.txt
+-rw-r--r--   0 steve      (501) staff       (20)      232 2023-04-25 08:37:22.000000 pygnssutils-1.0.7/src/pygnssutils.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       12 2023-04-25 08:37:22.000000 pygnssutils-1.0.7/src/pygnssutils.egg-info/top_level.txt
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-25 08:37:22.494570 pygnssutils-1.0.7/tests/
+-rw-r--r--   0 steve      (501) staff       (20)     9075 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/tests/test_gnssdump.py
+-rw-r--r--   0 steve      (501) staff       (20)    27167 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/tests/test_sourcetable.py
+-rw-r--r--   0 steve      (501) staff       (20)     4003 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/tests/test_static.py
+-rw-r--r--   0 steve      (501) staff       (20)     3492 2023-04-25 08:36:15.000000 pygnssutils-1.0.7/tests/test_stream.py
```

### Comparing `pygnssutils-1.0.6/LICENSE` & `pygnssutils-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.6/PKG-INFO` & `pygnssutils-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygnssutils
-Version: 1.0.6
+Version: 1.0.7
 Summary: GNSS Command Line Utilities
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2020, SEMU Consulting
         All rights reserved.
@@ -52,14 +52,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: deploy
 Provides-Extra: test
 License-File: LICENSE
 
 pygnssutils
 =======
 
 [Current Status](#currentstatus) |
```

### Comparing `pygnssutils-1.0.6/README.md` & `pygnssutils-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.6/pyproject.toml` & `pygnssutils-1.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
-requires = ["setuptools>=40.8.0", "wheel"]
+requires = ["setuptools>=66.0.0", "wheel"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "pygnssutils"
 authors = [
     {name = "semuadmin", email = "semuadmin@semuconsulting.com"},
 ]
 maintainers = [
   {name = "semuadmin", email = "semuadmin@semuconsulting.com"}
 ]
 description = "GNSS Command Line Utilities"
-version = "1.0.6"
+version = "1.0.7"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Operating System :: OS Independent",
     "Development Status :: 5 - Production/Stable",
     "Environment :: MacOS X",
@@ -34,18 +34,18 @@
     "License :: OSI Approved :: BSD License",
     "Topic :: Utilities",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Scientific/Engineering :: GIS",
     ]
 
 dependencies = [
-    "pyubx2>=1.2.23",
-    "pyspartn>=0.1.4",
-    "pyserial>=3.5",
     "paho-mqtt>=1.6.1",
+    "pyserial>=3.5",
+    "pyspartn>=0.1.6",
+    "pyubx2>=1.2.24",
 ]
 
 [project.scripts]
 gnssdump = "pygnssutils.gnssdump:main"
 gnssserver = "pygnssutils.gnssserver:main"
 gnssntripclient = "pygnssutils.gnssntripclient:main"
 gnssmqttclient = "pygnssutils.gnssmqttclient:main"
@@ -56,36 +56,53 @@
 [project.urls]
 homepage = "https://github.com/semuconsulting/pygnssutils"
 documentation = "https://www.semuconsulting.com/pygnssutils/"
 repository = "https://github.com/semuconsulting/pygnssutils"
 changelog = "https://github.com/semuconsulting/pygnssutils/blob/master/RELEASE_NOTES.md"
 
 [project.optional-dependencies]
+deploy = [
+    "build >= 0.10",
+    "pip >= 23.0",
+    "setuptools >= 66.0",
+    "wheel >= 0.40"
+] 
 test = [
+    "bandit >= 1.7",
     "black >= 23.1",
     "pylint >= 2.17",
     "pytest >= 7.2",
     "pytest-cov >= 4.0",
-    "Sphinx >= 6.1.3",
-    "sphinx-rtd-theme >= 1.2.0",
+    "Sphinx >= 5.3",
+    "sphinx-rtd-theme >= 1.2.0"
 ]
 
+[tool.bandit]
+exclude_dirs = ["docs", "examples", "tests"]
+skips = ["B104","B307"] # bind 0.0.0.0; use of eval
+
 [tool.pylint]
-exit-zero = ""
+jobs = 0
+reports = "y"
+py-version = "3.7"
+#exit-zero = "y"
+fail-under = "9.8"
+fail-on = "E,F"
+clear-cache-post-run = "y"
 disable = """
     raw-checker-failed,
     bad-inline-option,
     locally-disabled,
     file-ignored,
     suppressed-message,
     useless-suppression,
     deprecated-pragma,
     use-symbolic-message-instead,
 """
 
 [tool.pytest.ini_options]
 minversion = "7.0"
-addopts = "--cov --cov-report term-missing"
+addopts = "--cov --cov-report term-missing --cov-fail-under 35"
 pythonpath = ["src"]
 
 [tool.coverage.run]
 source = ["src"]
```

### Comparing `pygnssutils-1.0.6/src/pygnssutils/__init__.py` & `pygnssutils-1.0.7/src/pygnssutils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,22 +3,19 @@
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
 
 from pygnssutils._version import __version__
-from pygnssutils.exceptions import (
-    ParameterError,
-    GNSSStreamError,
-)
+from pygnssutils.exceptions import GNSSStreamError, ParameterError
+from pygnssutils.globals import *
 from pygnssutils.gnssdump import GNSSStreamer
-from pygnssutils.gnssserver import GNSSSocketServer
-from pygnssutils.gnssntripclient import GNSSNTRIPClient
 from pygnssutils.gnssmqttclient import GNSSMQTTClient
-from pygnssutils.ubxsetrate import UBXSetRate
+from pygnssutils.gnssntripclient import GNSSNTRIPClient
+from pygnssutils.gnssserver import GNSSSocketServer
+from pygnssutils.helpers import *
 from pygnssutils.ubxload import UBXLoader
 from pygnssutils.ubxsave import UBXSaver
-from pygnssutils.helpers import *
-from pygnssutils.globals import *
+from pygnssutils.ubxsetrate import UBXSetRate
 
 version = __version__  # pylint: disable=invalid-name
```

### Comparing `pygnssutils-1.0.6/src/pygnssutils/globals.py` & `pygnssutils-1.0.7/src/pygnssutils/globals.py`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.6/src/pygnssutils/gnssdump.py` & `pygnssutils-1.0.7/src/pygnssutils/gnssdump.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,53 +10,55 @@
 :author: semuadmin
 :copyright: SEMU Consulting © 2022
 :license: BSD 3-Clause
 """
 # pylint: disable=line-too-long eval-used
 
 import os
+from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser
 from collections import defaultdict
-from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
-from socket import socket
+from datetime import datetime
+from io import BufferedWriter, TextIOWrapper
 from queue import Queue
+from socket import socket
 from time import time
-from datetime import datetime
-from io import TextIOWrapper, BufferedWriter
-from serial import Serial
+
+import pynmeagps.exceptions as nme
+import pyrtcm.exceptions as rte
+import pyubx2.exceptions as ube
+from pynmeagps import NMEAMessage
+from pyrtcm import RTCMMessage
 from pyubx2 import (
-    UBXReader,
-    UBXMessage,
-    VALCKSUM,
+    ERR_LOG,
+    ERR_RAISE,
     GET,
-    UBX_PROTOCOL,
     NMEA_PROTOCOL,
     RTCM3_PROTOCOL,
-    ERR_LOG,
-    ERR_RAISE,
+    UBX_PROTOCOL,
+    VALCKSUM,
+    UBXMessage,
+    UBXReader,
     hextable,
 )
-from pynmeagps import NMEAMessage
-import pynmeagps.exceptions as nme
-import pyubx2.exceptions as ube
-from pyrtcm import RTCMMessage
-import pyrtcm.exceptions as rte
+from serial import Serial
+
 from pygnssutils._version import __version__ as VERSION
 from pygnssutils.exceptions import ParameterError
 from pygnssutils.globals import (
-    FORMAT_PARSED,
+    EPILOG,
     FORMAT_BINARY,
     FORMAT_HEX,
     FORMAT_HEXTABLE,
-    FORMAT_PARSEDSTRING,
     FORMAT_JSON,
-    VERBOSITY_MEDIUM,
-    VERBOSITY_HIGH,
-    VERBOSITY_DEBUG,
+    FORMAT_PARSED,
+    FORMAT_PARSEDSTRING,
     LOGLIMIT,
-    EPILOG,
+    VERBOSITY_DEBUG,
+    VERBOSITY_HIGH,
+    VERBOSITY_MEDIUM,
 )
 from pygnssutils.helpers import format_json
 
 
 class GNSSStreamer:
     """
     GNSS Streamer Class.
@@ -189,14 +191,16 @@
     def _setup_output_handlers(self, **kwargs):
         """
         Set up output handlers.
 
         Output handlers can either be writeable output media
         (Serial, File, socket or Queue) or an evaluable expression.
 
+        (Note: ast.literal_eval can't replace eval here)
+
         'allhandler' applies to all protocols and overrides
         individual output handlers.
         """
 
         htypes = (Serial, TextIOWrapper, BufferedWriter, Queue, socket)
 
         erh = kwargs.get("errorhandler", None)
```

### Comparing `pygnssutils-1.0.6/src/pygnssutils/gnssmqttclient.py` & `pygnssutils-1.0.7/src/pygnssutils/gnssmqttclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,50 +17,48 @@
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2023
 :license: BSD 3-Clause
 """
 # pylint: disable=invalid-name
 
-from os import path, getenv
+import socket
+from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser
+from datetime import datetime
+from io import BufferedWriter, BytesIO, TextIOWrapper
+from os import getenv, path
 from pathlib import Path
-from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
 from queue import Queue
-from datetime import datetime
-from io import BytesIO, TextIOWrapper, BufferedWriter
+from threading import Event, Thread
 from time import sleep
-from threading import Thread, Event
-import socket
-from serial import Serial
+
 import paho.mqtt.client as mqtt
-from pyubx2 import (
-    UBXReader,
-    UBXParseError,
-    SET,
-)
 from pyspartn import (
-    SPARTNReader,
-    SPARTNParseError,
     SPARTNMessageError,
+    SPARTNParseError,
+    SPARTNReader,
     SPARTNStreamError,
 )
+from pyubx2 import SET, UBXParseError, UBXReader
+from serial import Serial
+
+from pygnssutils._version import __version__ as VERSION
+from pygnssutils.exceptions import ParameterError
 from pygnssutils.globals import (
-    VERBOSITY_LOW,
-    VERBOSITY_MEDIUM,
+    EPILOG,
     LOGLIMIT,
     OUTPORT_SPARTN,
-    EPILOG,
+    SPARTN_EVENT,
+    SPARTN_PPSERVER,
     TOPIC_IP,
     TOPIC_MGA,
     TOPIC_RXM,
-    SPARTN_PPSERVER,
-    SPARTN_EVENT,
+    VERBOSITY_LOW,
+    VERBOSITY_MEDIUM,
 )
-from pygnssutils.exceptions import ParameterError
-from pygnssutils._version import __version__ as VERSION
 
 TIMEOUT = 8
 
 
 class GNSSMQTTClient:
     """
     SPARTN MQTT client class.
```

### Comparing `pygnssutils-1.0.6/src/pygnssutils/gnssntripclient.py` & `pygnssutils-1.0.7/src/pygnssutils/gnssntripclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,43 +19,41 @@
 :author: semuadmin
 :copyright: SEMU Consulting © 2022
 :license: BSD 3-Clause
 """
 # pylint: disable=invalid-name
 
 import os
-from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
-from time import sleep
-from threading import Thread, Event
-from queue import Queue
 import socket
-from datetime import datetime, timedelta
+from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser
 from base64 import b64encode
-from io import TextIOWrapper, BufferedWriter
+from datetime import datetime, timedelta
+from io import BufferedWriter, TextIOWrapper
+from queue import Queue
+from threading import Event, Thread
+from time import sleep
+
+from pynmeagps import GET, NMEAMessage
+from pyrtcm import RTCMMessageError, RTCMParseError, RTCMTypeError
+from pyubx2 import ERR_IGNORE, RTCM3_PROTOCOL, UBXReader
 from serial import Serial
-from pyubx2 import UBXReader, RTCM3_PROTOCOL, ERR_IGNORE
-from pyrtcm import (
-    RTCMParseError,
-    RTCMMessageError,
-    RTCMTypeError,
-)
-from pynmeagps import NMEAMessage, GET
+
+from pygnssutils._version import __version__ as VERSION
+from pygnssutils.exceptions import ParameterError
 from pygnssutils.globals import (
-    VERBOSITY_LOW,
-    VERBOSITY_MEDIUM,
     DEFAULT_BUFSIZE,
+    EPILOG,
+    HTTPERR,
     LOGLIMIT,
     MAXPORT,
     NOGGA,
     OUTPORT_NTRIP,
-    HTTPERR,
-    EPILOG,
+    VERBOSITY_LOW,
+    VERBOSITY_MEDIUM,
 )
-from pygnssutils.exceptions import ParameterError
-from pygnssutils._version import __version__ as VERSION
 from pygnssutils.helpers import find_mp_distance
 
 TIMEOUT = 10
 GGALIVE = 0
 GGAFIXED = 1
```

### Comparing `pygnssutils-1.0.6/src/pygnssutils/gnssserver.py` & `pygnssutils-1.0.7/src/pygnssutils/gnssserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,32 +12,33 @@
 :author: semuadmin
 :copyright: SEMU Consulting © 2022
 :license: BSD 3-Clause
 """
 # pylint: disable=too-many-arguments
 
 import os
-from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
-from time import sleep
+from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser
 from datetime import datetime
 from queue import Queue
 from threading import Thread
+from time import sleep
+
 from pygnssutils._version import __version__ as VERSION
 from pygnssutils.globals import (
-    FORMAT_BINARY,
-    VERBOSITY_LOW,
-    VERBOSITY_MEDIUM,
     CONNECTED,
+    EPILOG,
+    FORMAT_BINARY,
     LOGLIMIT,
     OUTPORT,
     OUTPORT_NTRIP,
-    EPILOG,
+    VERBOSITY_LOW,
+    VERBOSITY_MEDIUM,
 )
 from pygnssutils.gnssdump import GNSSStreamer
-from pygnssutils.socket_server import SocketServer, ClientHandler
+from pygnssutils.socket_server import ClientHandler, SocketServer
 
 
 class GNSSSocketServer:
     """
     GNSS Socket Server Class.
     """
```

### Comparing `pygnssutils-1.0.6/src/pygnssutils/helpers.py` & `pygnssutils-1.0.7/src/pygnssutils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2020
 :license: BSD 3-Clause
 """
 # pylint: disable=invalid-name
 
-from math import sin, cos, radians
-from pyubx2 import itow2utc
+from math import cos, radians, sin
 
 from pynmeagps import haversine
+from pyubx2 import itow2utc
 
 
 def get_mp_distance(lat: float, lon: float, mp: list) -> float:
     """
     Get distance to mountpoint from current location (if known).
 
     Predicated on the sourcetable being formatted as a
```

### Comparing `pygnssutils-1.0.6/src/pygnssutils/socket_server.py` & `pygnssutils-1.0.7/src/pygnssutils/socket_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,22 +23,23 @@
 Created on 16 May 2022
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2022
 :license: BSD 3-Clause
 """
 
-from os import getenv
-from socketserver import ThreadingTCPServer, StreamRequestHandler
-from threading import Thread, Event
-from queue import Queue
 from base64 import b64encode
 from datetime import datetime, timezone
+from os import getenv
+from queue import Queue
+from socketserver import StreamRequestHandler, ThreadingTCPServer
+from threading import Event, Thread
+
 from pygnssutils._version import __version__ as VERSION
-from pygnssutils.globals import DISCONNECTED, CONNECTED
+from pygnssutils.globals import CONNECTED, DISCONNECTED
 
 # from pygpsclient import version as PYGPSVERSION
 
 RTCM = b"rtcm"
 BUFSIZE = 1024
 PYGPSMP = "pygnssutils"
```

### Comparing `pygnssutils-1.0.6/src/pygnssutils/ubxload.py` & `pygnssutils-1.0.7/src/pygnssutils/ubxload.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,21 +20,23 @@
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2023
 :license: BSD 3-Clause
 """
 # pylint: disable=invalid-name
 
-from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
-from math import ceil
+from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser
 from datetime import datetime, timedelta
-from threading import Thread, Event, Lock
+from math import ceil
 from queue import Queue
+from threading import Event, Lock, Thread
+
+from pyubx2 import SET, UBX_PROTOCOL, UBXMessageError, UBXParseError, UBXReader
 from serial import Serial
-from pyubx2 import UBXReader, UBX_PROTOCOL, SET, UBXMessageError, UBXParseError
+
 from pygnssutils._version import __version__ as VERSION
 from pygnssutils.globals import EPILOG
 
 ACK = "ACK-ACK"
 NAK = "ACK-NAK"
 # try increasing these values if device response is too slow:
 DELAY = 0.05  # delay between sends
```

### Comparing `pygnssutils-1.0.6/src/pygnssutils/ubxsave.py` & `pygnssutils-1.0.7/src/pygnssutils/ubxsave.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,31 +25,33 @@
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2023
 :license: BSD 3-Clause
 """
 # pylint: disable=invalid-name
 
-from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
-from threading import Thread, Event, Lock
+from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser
 from math import ceil
 from queue import Queue
+from threading import Event, Lock, Thread
 from time import sleep, strftime
-from serial import Serial
+
 from pyubx2 import (
-    UBXReader,
-    UBXMessage,
-    UBX_PROTOCOL,
-    UBX_CONFIG_DATABASE,
     POLL_LAYER_RAM,
     SET_LAYER_RAM,
-    TXN_START,
-    TXN_ONGOING,
     TXN_COMMIT,
+    TXN_ONGOING,
+    TXN_START,
+    UBX_CONFIG_DATABASE,
+    UBX_PROTOCOL,
+    UBXMessage,
+    UBXReader,
 )
+from serial import Serial
+
 from pygnssutils._version import __version__ as VERSION
 from pygnssutils.globals import EPILOG
 
 # try increasing these values if device response is too slow:
 DELAY = 0.02  # delay between polls
 WRAPUP = 5  # delay for final responses
```

### Comparing `pygnssutils-1.0.6/src/pygnssutils/ubxsetrate.py` & `pygnssutils-1.0.7/src/pygnssutils/ubxsetrate.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,35 +17,32 @@
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2022
 :license: BSD 3-Clause
 """
 # pylint: disable=invalid-name
 
-from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
+from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser
+
+from pyubx2 import SET, UBX_CLASSES, UBX_MSGIDS, UBXMessage
 from serial import Serial
-from pyubx2 import (
-    UBXMessage,
-    SET,
-    UBX_CLASSES,
-    UBX_MSGIDS,
-)
+
+from pygnssutils._version import __version__ as VERSION
+from pygnssutils.exceptions import ParameterError
 from pygnssutils.globals import (
     ALLNMEA,
+    ALLNMEA_CLS,
     ALLUBX,
+    ALLUBX_CLS,
+    EPILOG,
+    MINMMEA_ID,
     MINNMEA,
     MINUBX,
-    ALLNMEA_CLS,
-    MINMMEA_ID,
-    ALLUBX_CLS,
     MINUBX_ID,
-    EPILOG,
 )
-from pygnssutils._version import __version__ as VERSION
-from pygnssutils.exceptions import ParameterError
 
 
 class UBXSetRate:
     """
     UBX Set Rate Class.
 
      Supports basic enable/disable message configuration for UBX GNSS devices
```

### Comparing `pygnssutils-1.0.6/src/pygnssutils.egg-info/PKG-INFO` & `pygnssutils-1.0.7/src/pygnssutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygnssutils
-Version: 1.0.6
+Version: 1.0.7
 Summary: GNSS Command Line Utilities
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2020, SEMU Consulting
         All rights reserved.
@@ -52,14 +52,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: deploy
 Provides-Extra: test
 License-File: LICENSE
 
 pygnssutils
 =======
 
 [Current Status](#currentstatus) |
```

### Comparing `pygnssutils-1.0.6/src/pygnssutils.egg-info/SOURCES.txt` & `pygnssutils-1.0.7/src/pygnssutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.6/tests/test_gnssdump.py` & `pygnssutils-1.0.7/tests/test_gnssdump.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,26 +6,25 @@
 @author: semuadmin
 """
 # pylint: disable=line-too-long, invalid-name, missing-docstring, no-member
 
 import os
 import sys
 import unittest
-
 from io import StringIO
 
 from pygnssutils import exceptions as pge
 from pygnssutils.gnssdump import (
-    GNSSStreamer,
-    FORMAT_PARSED,
     FORMAT_BINARY,
     FORMAT_HEX,
     FORMAT_HEXTABLE,
     FORMAT_JSON,
+    FORMAT_PARSED,
     FORMAT_PARSEDSTRING,
+    GNSSStreamer,
 )
 
 
 class GNSSDumpTest(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
         self.mixedfile = os.path.join(os.path.dirname(__file__), "pygpsdata-MIXED3.log")
```

### Comparing `pygnssutils-1.0.6/tests/test_sourcetable.py` & `pygnssutils-1.0.7/tests/test_sourcetable.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Test NTRIP sourcetable
 """
 
 import os
 import sys
 import unittest
 
-
 TESTSRT = [
     [
         "AGSSIAAP",
         "Acheres",
         "RTCM 3.0",
         "1004(1),1006(13),1012(1),1033(31)",
         "2",
```

### Comparing `pygnssutils-1.0.6/tests/test_static.py` & `pygnssutils-1.0.7/tests/test_static.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,24 +7,17 @@
 
 @author: semuadmin
 """
 # pylint: disable=line-too-long, invalid-name, missing-docstring, no-member
 
 import unittest
 
-from pyubx2 import (
-    UBXReader,
-    itow2utc,
-)
-from pygnssutils.helpers import (
-    cel2cart,
-    format_json,
-    get_mp_distance,
-    find_mp_distance,
-)
+from pyubx2 import UBXReader, itow2utc
+
+from pygnssutils.helpers import cel2cart, find_mp_distance, format_json, get_mp_distance
 from tests.test_sourcetable import TESTSRT
 
 
 class StaticTest(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
         # dirname = os.path.dirname(__file__)
@@ -107,15 +100,15 @@
         self.assertEqual(res, (None, 9999999))
 
     def testgetmpdist1(self):  # valid
         mp = TESTSRT[12]
         lat = 54.8
         lon = -7.4
         res = get_mp_distance(lat, lon, mp)
-        self.assertAlmostEqual(res, 6221.201, 4)
+        self.assertAlmostEqual(res, 6221.200922509212, 4)
 
     def testgetmpdist2(self):  # mp has no coords
         mp = TESTSRT[27]
         lat = 53
         lon = -2.24
         res = get_mp_distance(lat, lon, mp)
         self.assertEqual(res, None)
```

### Comparing `pygnssutils-1.0.6/tests/test_stream.py` & `pygnssutils-1.0.7/tests/test_stream.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 @author: semuadmin
 """
 # pylint: disable=line-too-long, invalid-name, missing-docstring, no-member
 
 import os
 import sys
 import unittest
-
 from io import StringIO
+
 from pygnssutils import GNSSStreamer
 
 
 class StreamTest(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
```

