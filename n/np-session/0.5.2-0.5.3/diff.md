# Comparing `tmp/np-session-0.5.2.tar.gz` & `tmp/np-session-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np-session-0.5.2.tar", last modified: Thu Apr 20 17:28:18 2023, max compression
+gzip compressed data, was "np-session-0.5.3.tar", last modified: Tue Apr 25 05:42:53 2023, max compression
```

## Comparing `np-session-0.5.2.tar` & `np-session-0.5.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2113 2023-04-20 17:28:10.838237 np-session-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1373 2023-02-14 03:16:07.068541 np-session-0.5.2/README.md
--rw-r--r--   0        0        0      170 2023-03-17 05:14:59.145709 np-session-0.5.2/src/np_session/__init__.py
--rw-r--r--   0        0        0      186 2023-03-17 05:14:59.145709 np-session-0.5.2/src/np_session/components/__init__.py
--rw-r--r--   0        0        0     7972 2023-04-13 01:45:59.657072 np-session-0.5.2/src/np_session/components/info.py
--rw-r--r--   0        0        0     7708 2023-03-23 23:41:50.844242 np-session-0.5.2/src/np_session/components/lims_manifests.py
--rw-r--r--   0        0        0     1390 2023-04-04 00:25:44.745816 np-session-0.5.2/src/np_session/components/paths.py
--rw-r--r--   0        0        0    10785 2023-03-17 05:14:59.154649 np-session-0.5.2/src/np_session/components/platform_json.py
--rw-r--r--   0        0        0     5019 2023-03-17 05:14:59.155648 np-session-0.5.2/src/np_session/components/settings_xml.py
--rw-r--r--   0        0        0      189 2023-03-19 18:40:51.970936 np-session-0.5.2/src/np_session/databases/__init__.py
--rw-r--r--   0        0        0    21233 2023-03-21 02:25:36.728269 np-session-0.5.2/src/np_session/databases/data_getters.py
--rw-r--r--   0        0        0     2716 2023-03-19 17:40:22.225142 np-session-0.5.2/src/np_session/databases/firebase_state.py
--rw-r--r--   0        0        0    12022 2023-03-17 05:14:59.159645 np-session-0.5.2/src/np_session/databases/lims2.py
--rw-r--r--   0        0        0    12644 2023-03-17 05:14:59.161647 np-session-0.5.2/src/np_session/databases/mtrain.py
--rw-r--r--   0        0        0     3687 2023-03-19 17:40:06.274698 np-session-0.5.2/src/np_session/databases/redis_state.py
--rw-r--r--   0        0        0     9863 2023-03-17 05:16:43.438094 np-session-0.5.2/src/np_session/databases/sql_alchemy.py
--rw-r--r--   0        0        0       83 2023-03-17 05:16:43.454095 np-session-0.5.2/src/np_session/jobs/__init__.py
--rw-r--r--   0        0        0      423 2023-03-19 18:45:17.801626 np-session-0.5.2/src/np_session/jobs/find_missing_files.py
--rw-r--r--   0        0        0        0 2023-03-19 18:03:04.930628 np-session-0.5.2/src/np_session/jobs/generate_session_summaries.py
--rw-r--r--   0        0        0     4123 2023-03-19 01:12:39.701848 np-session-0.5.2/src/np_session/jobs/lims_upload.py
--rw-r--r--   0        0        0     5710 2023-03-17 05:16:43.439093 np-session-0.5.2/src/np_session/jobs/probes.py
--rw-r--r--   0        0        0   296297 2023-03-17 05:16:43.442095 np-session-0.5.2/src/np_session/jobs/sessions.json
--rw-r--r--   0        0        0      551 2023-03-19 18:00:31.176404 np-session-0.5.2/src/np_session/jobs/sync_states.py
--rw-r--r--   0        0        0    25576 2023-03-29 21:44:41.257200 np-session-0.5.2/src/np_session/session.py
--rw-r--r--   0        0        0     8357 2023-04-20 17:27:28.627831 np-session-0.5.2/src/np_session/utils.py
--rw-r--r--   0        0        0        0 2023-01-01 18:45:33.027289 np-session-0.5.2/tests/__init__.py
--rw-r--r--   0        0        0      406 2023-03-17 05:16:43.457095 np-session-0.5.2/tests/test_np_session.py
--rw-r--r--   0        0        0     1082 2023-03-17 05:14:59.169233 np-session-0.5.2/tests/test_platform_json.py
--rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 np-session-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     2194 2023-04-25 05:42:45.850824 np-session-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1373 2023-02-14 03:16:07.068541 np-session-0.5.3/README.md
+-rw-r--r--   0        0        0      170 2023-03-17 05:14:59.145709 np-session-0.5.3/src/np_session/__init__.py
+-rw-r--r--   0        0        0      186 2023-03-17 05:14:59.145709 np-session-0.5.3/src/np_session/components/__init__.py
+-rw-r--r--   0        0        0     8087 2023-04-25 01:32:31.553377 np-session-0.5.3/src/np_session/components/info.py
+-rw-r--r--   0        0        0     7708 2023-03-23 23:41:50.844242 np-session-0.5.3/src/np_session/components/lims_manifests.py
+-rw-r--r--   0        0        0     1390 2023-04-04 00:25:44.745816 np-session-0.5.3/src/np_session/components/paths.py
+-rw-r--r--   0        0        0    10785 2023-03-17 05:14:59.154649 np-session-0.5.3/src/np_session/components/platform_json.py
+-rw-r--r--   0        0        0     5019 2023-03-17 05:14:59.155648 np-session-0.5.3/src/np_session/components/settings_xml.py
+-rw-r--r--   0        0        0      189 2023-03-19 18:40:51.970936 np-session-0.5.3/src/np_session/databases/__init__.py
+-rw-r--r--   0        0        0    21233 2023-03-21 02:25:36.728269 np-session-0.5.3/src/np_session/databases/data_getters.py
+-rw-r--r--   0        0        0     2716 2023-03-19 17:40:22.225142 np-session-0.5.3/src/np_session/databases/firebase_state.py
+-rw-r--r--   0        0        0    12022 2023-03-17 05:14:59.159645 np-session-0.5.3/src/np_session/databases/lims2.py
+-rw-r--r--   0        0        0    12644 2023-03-17 05:14:59.161647 np-session-0.5.3/src/np_session/databases/mtrain.py
+-rw-r--r--   0        0        0     3687 2023-03-19 17:40:06.274698 np-session-0.5.3/src/np_session/databases/redis_state.py
+-rw-r--r--   0        0        0     9863 2023-03-17 05:16:43.438094 np-session-0.5.3/src/np_session/databases/sql_alchemy.py
+-rw-r--r--   0        0        0       83 2023-03-17 05:16:43.454095 np-session-0.5.3/src/np_session/jobs/__init__.py
+-rw-r--r--   0        0        0      423 2023-03-19 18:45:17.801626 np-session-0.5.3/src/np_session/jobs/find_missing_files.py
+-rw-r--r--   0        0        0        0 2023-03-19 18:03:04.930628 np-session-0.5.3/src/np_session/jobs/generate_session_summaries.py
+-rw-r--r--   0        0        0     4123 2023-03-19 01:12:39.701848 np-session-0.5.3/src/np_session/jobs/lims_upload.py
+-rw-r--r--   0        0        0     5710 2023-03-17 05:16:43.439093 np-session-0.5.3/src/np_session/jobs/probes.py
+-rw-r--r--   0        0        0   296297 2023-03-17 05:16:43.442095 np-session-0.5.3/src/np_session/jobs/sessions.json
+-rw-r--r--   0        0        0      551 2023-03-19 18:00:31.176404 np-session-0.5.3/src/np_session/jobs/sync_states.py
+-rw-r--r--   0        0        0    26133 2023-04-20 20:34:24.850399 np-session-0.5.3/src/np_session/session.py
+-rw-r--r--   0        0        0     8357 2023-04-20 17:27:28.627831 np-session-0.5.3/src/np_session/utils.py
+-rw-r--r--   0        0        0        0 2023-01-01 18:45:33.027289 np-session-0.5.3/tests/__init__.py
+-rw-r--r--   0        0        0      406 2023-03-17 05:16:43.457095 np-session-0.5.3/tests/test_np_session.py
+-rw-r--r--   0        0        0     1082 2023-03-17 05:14:59.169233 np-session-0.5.3/tests/test_platform_json.py
+-rw-r--r--   0        0        0     1949 1970-01-01 00:00:00.000000 np-session-0.5.3/PKG-INFO
```

### Comparing `np-session-0.5.2/pyproject.toml` & `np-session-0.5.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "np-session"
-version = "0.5.2"
+version = "0.5.3"
 description = "Tools for accessing data, metadata, and jobs related to ecephys and behavior sessions for the Mindscope Neuropixels team."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -64,14 +64,20 @@
 [tool.pdm.scripts.dry-run]
 composite = [
     "prebuild",
     "pdm build",
     "pdm publish --no-build --repository https://test.pypi.org/simple",
 ]
 
+[tool.pdm.scripts.pub]
+composite = [
+    "pdm bump patch",
+    "pdm publish",
+]
+
 [tool.pdm.scripts.publish]
 composite = [
     "pdm build",
     "pdm publish --no-build",
 ]
 
 [tool.pytest.ini_options]
```

### Comparing `np-session-0.5.2/README.md` & `np-session-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `np-session-0.5.2/src/np_session/components/info.py` & `np-session-0.5.3/src/np_session/components/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,19 +102,22 @@
 
     VAR = (
         "VariabilitySpontaneous",
         "VariabilityAim1",
     )
     GLO = ("OpenScopeGlobalLocalOddball",)
     ILLUSION = ("OpenScopeIllusion",)
-    DR = (
+    DRDG = (
         "DynamicRoutingSurgicalDevelopment",
         "DynamicRoutingDynamicGating",
         "DynamicRoutingTask1Production",
     )
+    """Dynamic Gating subset of DR."""
+    DR = DRDG
+    """All Dynamic Routing, including Dynamic Gating."""
     VB = ("NeuropixelVisualBehavior",)
     TTN = ('TaskTrainedNetworksNeuropixel',)
     NP = ('NeuropixelPlatformDevelopment',)
     
     def get_latest_session(self, session_type: Literal['ephys', 'hab', 'behavior'] = 'ephys') -> int | None:
         "Lims session id for latest session for all child projects."
         for _ in self.value:
```

### Comparing `np-session-0.5.2/src/np_session/components/lims_manifests.py` & `np-session-0.5.3/src/np_session/components/lims_manifests.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.2/src/np_session/components/paths.py` & `np-session-0.5.3/src/np_session/components/paths.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.2/src/np_session/components/platform_json.py` & `np-session-0.5.3/src/np_session/components/platform_json.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.2/src/np_session/components/settings_xml.py` & `np-session-0.5.3/src/np_session/components/settings_xml.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.2/src/np_session/databases/data_getters.py` & `np-session-0.5.3/src/np_session/databases/data_getters.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.2/src/np_session/databases/firebase_state.py` & `np-session-0.5.3/src/np_session/databases/firebase_state.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.2/src/np_session/databases/lims2.py` & `np-session-0.5.3/src/np_session/databases/lims2.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.2/src/np_session/databases/mtrain.py` & `np-session-0.5.3/src/np_session/databases/mtrain.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.2/src/np_session/databases/redis_state.py` & `np-session-0.5.3/src/np_session/databases/redis_state.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.2/src/np_session/databases/sql_alchemy.py` & `np-session-0.5.3/src/np_session/databases/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.2/src/np_session/jobs/lims_upload.py` & `np-session-0.5.3/src/np_session/jobs/lims_upload.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.2/src/np_session/jobs/probes.py` & `np-session-0.5.3/src/np_session/jobs/probes.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.2/src/np_session/jobs/sessions.json` & `np-session-0.5.3/src/np_session/jobs/sessions.json`

 * *Files identical despite different names*

### Comparing `np-session-0.5.2/src/np_session/jobs/sync_states.py` & `np-session-0.5.3/src/np_session/jobs/sync_states.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.2/src/np_session/session.py` & `np-session-0.5.3/src/np_session/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import copy
 import datetime
 import doctest
 import functools
 import itertools
 import os
 import pathlib
+import shutil
 from typing import Any, Callable, Generator, Iterable, MutableMapping, Optional, Union
 
 import np_config
 import np_logging
 from backports.cached_property import cached_property
 from typing_extensions import Literal
 
@@ -599,21 +600,33 @@
         if session.is_hab is None:
             logger.debug("Unsure if %s is a hab or ephys session, but it's included in results", session)
             
         yield session
 
 def cleanup_npexp():
     """Remove empty dirs, 366122 dirs, move habs"""
+    def remove_non_empty_dir(path: pathlib.Path):
+        shutil.rmtree(path, ignore_errors=True)
+        if not path.exists():
+            logger.info("Removed %s", path.name)
+        
     for _ in itertools.chain(NPEXP_ROOT.iterdir(), (NPEXP_ROOT / "habituation").iterdir()):
         if not _.is_dir():
             continue
-        if not any(_.iterdir()):
+        with contextlib.suppress(Exception):
             _.rmdir()
             logger.info("Removed empty dir %s", _.name)
             continue
+        if '_366122_' in _.name:
+            remove_non_empty_dir(_)
+            continue
+        contents = tuple(_.iterdir())
+        if len(contents) == 1 and contents[0].suffix == ".json" and "platform" in contents[0].name:
+            remove_non_empty_dir(_)
+            continue
         try:
             session = Session(_)
         except SessionError:
             continue
         if session.is_hab and _.parent == NPEXP_ROOT:
             try:
                 _.replace(NPEXP_ROOT / "habituation" / "backup" / _.name)
@@ -640,14 +653,15 @@
     if session is None:
         logger.info("No latest session found for %s", project)
         return None
     
     return Session(session)
 
 if __name__ == "__main__":
-
+    np_logging.getLogger()
+    cleanup_npexp()
     if is_connected("lims2"):
         doctest.testmod(verbose=True)
         # optionflags=(doctest.ELLIPSIS, doctest.NORMALIZE_WHITESPACE,
         # doctest.IGNORE_EXCEPTION_DETAIL)
     else:
         print("LIMS not connected - skipping doctests")
```

### Comparing `np-session-0.5.2/src/np_session/utils.py` & `np-session-0.5.3/src/np_session/utils.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.2/tests/test_platform_json.py` & `np-session-0.5.3/tests/test_platform_json.py`

 * *Files identical despite different names*

### Comparing `np-session-0.5.2/PKG-INFO` & `np-session-0.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-session
-Version: 0.5.2
+Version: 0.5.3
 Summary: Tools for accessing data, metadata, and jobs related to ecephys and behavior sessions for the Mindscope Neuropixels team.
 Author-email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: dev
```

