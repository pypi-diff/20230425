# Comparing `tmp/pyecotrend-ista-2.0.5.tar.gz` & `tmp/pyecotrend-ista-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyecotrend-ista-2.0.5.tar", last modified: Mon Apr 24 09:36:22 2023, max compression
+gzip compressed data, was "pyecotrend-ista-2.0.6.tar", last modified: Tue Apr 25 07:34:14 2023, max compression
```

## Comparing `pyecotrend-ista-2.0.5.tar` & `pyecotrend-ista-2.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:36:22.558672 pyecotrend-ista-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-24 09:36:06.000000 pyecotrend-ista-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-24 09:36:22.558672 pyecotrend-ista-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-24 09:36:06.000000 pyecotrend-ista-2.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 09:36:22.558672 pyecotrend-ista-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-24 09:36:06.000000 pyecotrend-ista-2.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:36:22.554672 pyecotrend-ista-2.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:36:22.558672 pyecotrend-ista-2.0.5/src/pyecotrend_ista/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 09:36:06.000000 pyecotrend-ista-2.0.5/src/pyecotrend_ista/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-24 09:36:06.000000 pyecotrend-ista-2.0.5/src/pyecotrend_ista/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-24 09:36:06.000000 pyecotrend-ista-2.0.5/src/pyecotrend_ista/exception_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-24 09:36:06.000000 pyecotrend-ista-2.0.5/src/pyecotrend_ista/helper_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-04-24 09:36:06.000000 pyecotrend-ista-2.0.5/src/pyecotrend_ista/ista_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    23322 2023-04-24 09:36:06.000000 pyecotrend-ista-2.0.5/src/pyecotrend_ista/pyecotrend_ista.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 09:36:22.558672 pyecotrend-ista-2.0.5/src/pyecotrend_ista.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-24 09:36:22.000000 pyecotrend-ista-2.0.5/src/pyecotrend_ista.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-24 09:36:22.000000 pyecotrend-ista-2.0.5/src/pyecotrend_ista.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 09:36:22.000000 pyecotrend-ista-2.0.5/src/pyecotrend_ista.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 09:36:22.000000 pyecotrend-ista-2.0.5/src/pyecotrend_ista.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 09:36:22.000000 pyecotrend-ista-2.0.5/src/pyecotrend_ista.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:34:14.703504 pyecotrend-ista-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-25 07:33:57.000000 pyecotrend-ista-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-25 07:34:14.699504 pyecotrend-ista-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-25 07:33:57.000000 pyecotrend-ista-2.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 07:34:14.703504 pyecotrend-ista-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-25 07:33:57.000000 pyecotrend-ista-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:34:14.699504 pyecotrend-ista-2.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:34:14.699504 pyecotrend-ista-2.0.6/src/pyecotrend_ista/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 07:33:57.000000 pyecotrend-ista-2.0.6/src/pyecotrend_ista/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-25 07:33:57.000000 pyecotrend-ista-2.0.6/src/pyecotrend_ista/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-25 07:33:57.000000 pyecotrend-ista-2.0.6/src/pyecotrend_ista/exception_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-25 07:33:57.000000 pyecotrend-ista-2.0.6/src/pyecotrend_ista/helper_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-25 07:33:57.000000 pyecotrend-ista-2.0.6/src/pyecotrend_ista/ista_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23317 2023-04-25 07:33:57.000000 pyecotrend-ista-2.0.6/src/pyecotrend_ista/pyecotrend_ista.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 07:34:14.699504 pyecotrend-ista-2.0.6/src/pyecotrend_ista.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-25 07:34:14.000000 pyecotrend-ista-2.0.6/src/pyecotrend_ista.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-25 07:34:14.000000 pyecotrend-ista-2.0.6/src/pyecotrend_ista.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 07:34:14.000000 pyecotrend-ista-2.0.6/src/pyecotrend_ista.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-25 07:34:14.000000 pyecotrend-ista-2.0.6/src/pyecotrend_ista.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 07:34:14.000000 pyecotrend-ista-2.0.6/src/pyecotrend_ista.egg-info/top_level.txt
```

### Comparing `pyecotrend-ista-2.0.5/LICENSE` & `pyecotrend-ista-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-2.0.5/PKG-INFO` & `pyecotrend-ista-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecotrend-ista
-Version: 2.0.5
+Version: 2.0.6
 Summary: Python ecotrend-ista Api
 Home-page: https://github.com/Ludy87/pyecotrend-ista
 Author: Ludy87
 Author-email: android@astra-g.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Ludy87/pyecotrend-ista/issues
 Keywords: python api ecotrend ista
```

### Comparing `pyecotrend-ista-2.0.5/README.md` & `pyecotrend-ista-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-2.0.5/setup.py` & `pyecotrend-ista-2.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,10 +34,10 @@
         "Intended Audience :: Developers",
         "Topic :: Software Development",
         "Topic :: Utilities",
         "Topic :: Home Automation",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     keywords="python api ecotrend ista",
-    install_requires=["aiohttp==3.8.1"],
+    install_requires=["aiohttp>=3.8.1", "dataclasses-json==0.5.7"],
     python_requires=">=3.6",
 )
```

### Comparing `pyecotrend-ista-2.0.5/src/pyecotrend_ista/helper_object.py` & `pyecotrend-ista-2.0.6/src/pyecotrend_ista/helper_object.py`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-2.0.5/src/pyecotrend_ista/ista_object.py` & `pyecotrend-ista-2.0.6/src/pyecotrend_ista/ista_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Optional
+from typing import Any, List, Optional
 
 from dataclasses_json import DataClassJsonMixin, dataclass_json
 
 
 @dataclass_json
 @dataclass
 class Resident(DataClassJsonMixin):
```

### Comparing `pyecotrend-ista-2.0.5/src/pyecotrend_ista/pyecotrend_ista.py` & `pyecotrend-ista-2.0.6/src/pyecotrend_ista/pyecotrend_ista.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     def _logoff(self) -> None:
         self._accessToken = None
 
     async def __login(self) -> str | None:
         if self._email == "demo@ista.de" and self._password == "Ausprobieren!" and self._hass_dir:
             self._LOGGER.debug("DEMO")
-            with open(self._hass_dir + "/account.json") as f:
+            with open(self._hass_dir + "/account.json"):
                 self._accessToken = "Demo"
             return self._accessToken
         payload = {
             "email": self._email,
             "password": self._password,
             "fromMobileApp": "false",
         }
```

### Comparing `pyecotrend-ista-2.0.5/src/pyecotrend_ista.egg-info/PKG-INFO` & `pyecotrend-ista-2.0.6/src/pyecotrend_ista.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecotrend-ista
-Version: 2.0.5
+Version: 2.0.6
 Summary: Python ecotrend-ista Api
 Home-page: https://github.com/Ludy87/pyecotrend-ista
 Author: Ludy87
 Author-email: android@astra-g.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Ludy87/pyecotrend-ista/issues
 Keywords: python api ecotrend ista
```

