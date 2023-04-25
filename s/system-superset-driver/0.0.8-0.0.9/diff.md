# Comparing `tmp/system_superset_driver-0.0.8.tar.gz` & `tmp/system_superset_driver-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "system_superset_driver-0.0.8.tar", last modified: Mon Apr 24 08:01:34 2023, max compression
+gzip compressed data, was "system_superset_driver-0.0.9.tar", last modified: Mon Apr 24 08:06:35 2023, max compression
```

## Comparing `system_superset_driver-0.0.8.tar` & `system_superset_driver-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 08:01:34.186977 system_superset_driver-0.0.8/
--rw-rw-rw-   0        0        0      157 2023-04-24 08:01:34.186977 system_superset_driver-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 08:01:34.171019 system_superset_driver-0.0.8/apm_system/
--rw-rw-rw-   0        0        0        0 2023-04-24 07:32:21.000000 system_superset_driver-0.0.8/apm_system/__init__.py
--rw-rw-rw-   0        0        0     3146 2023-04-24 06:56:16.000000 system_superset_driver-0.0.8/apm_system/apm_adapter.py
--rw-rw-rw-   0        0        0     1032 2023-04-24 07:58:06.000000 system_superset_driver-0.0.8/apm_system/apm_dialect.py
--rw-rw-rw-   0        0        0      590 2023-04-24 07:31:18.000000 system_superset_driver-0.0.8/apm_system/db_engine_specs.py
--rw-rw-rw-   0        0        0       42 2023-04-24 08:01:34.186977 system_superset_driver-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      559 2023-04-24 08:01:33.000000 system_superset_driver-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:01:34.185979 system_superset_driver-0.0.8/system_superset_driver.egg-info/
--rw-rw-rw-   0        0        0      157 2023-04-24 08:01:34.000000 system_superset_driver-0.0.8/system_superset_driver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2023-04-24 08:01:34.000000 system_superset_driver-0.0.8/system_superset_driver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 08:01:34.000000 system_superset_driver-0.0.8/system_superset_driver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2023-04-24 08:01:34.000000 system_superset_driver-0.0.8/system_superset_driver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       71 2023-04-24 08:01:34.000000 system_superset_driver-0.0.8/system_superset_driver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-24 08:01:34.000000 system_superset_driver-0.0.8/system_superset_driver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-24 08:06:35.496055 system_superset_driver-0.0.9/
+-rw-rw-rw-   0        0        0      157 2023-04-24 08:06:35.496055 system_superset_driver-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 08:06:35.479099 system_superset_driver-0.0.9/apm_system/
+-rw-rw-rw-   0        0        0        0 2023-04-24 07:32:21.000000 system_superset_driver-0.0.9/apm_system/__init__.py
+-rw-rw-rw-   0        0        0     3146 2023-04-24 06:56:16.000000 system_superset_driver-0.0.9/apm_system/apm_adapter.py
+-rw-rw-rw-   0        0        0     1082 2023-04-24 08:06:34.000000 system_superset_driver-0.0.9/apm_system/apm_dialect.py
+-rw-rw-rw-   0        0        0      590 2023-04-24 07:31:18.000000 system_superset_driver-0.0.9/apm_system/db_engine_specs.py
+-rw-rw-rw-   0        0        0       42 2023-04-24 08:06:35.496055 system_superset_driver-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      559 2023-04-24 08:06:35.000000 system_superset_driver-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 08:06:35.495057 system_superset_driver-0.0.9/system_superset_driver.egg-info/
+-rw-rw-rw-   0        0        0      157 2023-04-24 08:06:35.000000 system_superset_driver-0.0.9/system_superset_driver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2023-04-24 08:06:35.000000 system_superset_driver-0.0.9/system_superset_driver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 08:06:35.000000 system_superset_driver-0.0.9/system_superset_driver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2023-04-24 08:06:35.000000 system_superset_driver-0.0.9/system_superset_driver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       71 2023-04-24 08:06:35.000000 system_superset_driver-0.0.9/system_superset_driver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-24 08:06:35.000000 system_superset_driver-0.0.9/system_superset_driver.egg-info/top_level.txt
```

### Comparing `system_superset_driver-0.0.8/apm_system/apm_adapter.py` & `system_superset_driver-0.0.9/apm_system/apm_adapter.py`

 * *Files identical despite different names*

### Comparing `system_superset_driver-0.0.8/apm_system/apm_dialect.py` & `system_superset_driver-0.0.9/apm_system/apm_dialect.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,8 +28,8 @@
         return "test"
 
     def create_connect_args(
             self,
             url: URL,
     ) -> Tuple[Tuple[()], Dict[str, Any]]:
         args, kwargs = super().create_connect_args(url)
-        return args, {}
+        return args, {**kwargs, "path": ":memory:", "adapter_kwargs": {}}
```

### Comparing `system_superset_driver-0.0.8/apm_system/db_engine_specs.py` & `system_superset_driver-0.0.9/apm_system/db_engine_specs.py`

 * *Files identical despite different names*

### Comparing `system_superset_driver-0.0.8/setup.py` & `system_superset_driver-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-setup(name="system_superset_driver",version="0.0.8",packages=find_packages(),
+setup(name="system_superset_driver",version="0.0.9",packages=find_packages(),
       entry_points={
           "shillelagh.adapter": [
               "system = apm_system.apm_adapter:SystemAPI",
           ],
           "sqlalchemy.dialects": [
               "system = apm_system.apm_dialect:SystemDialect",
           ],
```

