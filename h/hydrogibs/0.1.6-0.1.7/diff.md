# Comparing `tmp/hydrogibs-0.1.6.tar.gz` & `tmp/hydrogibs-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrogibs-0.1.6.tar", last modified: Tue Apr 25 12:40:01 2023, max compression
+gzip compressed data, was "hydrogibs-0.1.7.tar", last modified: Tue Apr 25 12:47:06 2023, max compression
```

## Comparing `hydrogibs-0.1.6.tar` & `hydrogibs-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 12:40:01.752954 hydrogibs-0.1.6/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.1.6/LICENSE
--rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-04-25 12:40:01.752954 hydrogibs-0.1.6/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.1.6/README.md
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 12:40:01.748953 hydrogibs-0.1.6/hydrogibs/
--rw-rw-r--   0 axel      (1000) axel      (1000)    21610 2023-04-25 12:37:53.000000 hydrogibs-0.1.6/hydrogibs/GR4.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     2926 2023-04-25 12:03:41.000000 hydrogibs-0.1.6/hydrogibs/QDF.py
--rw-rw-r--   0 axel      (1000) axel      (1000)      982 2023-04-25 11:49:20.000000 hydrogibs-0.1.6/hydrogibs/RationalMethod.py
--rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-04-25 11:52:06.000000 hydrogibs-0.1.6/hydrogibs/SoCoSe.py
--rw-rw-r--   0 axel      (1000) axel      (1000)       61 2023-04-25 12:03:58.000000 hydrogibs-0.1.6/hydrogibs/__init__.py
--rw-rw-r--   0 axel      (1000) axel      (1000)        0 2023-04-25 12:12:22.000000 hydrogibs-0.1.6/hydrogibs/__main__.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     4748 2023-04-25 11:52:25.000000 hydrogibs-0.1.6/hydrogibs/misc.py
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 12:40:01.752954 hydrogibs-0.1.6/hydrogibs.egg-info/
--rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-04-25 12:40:01.000000 hydrogibs-0.1.6/hydrogibs.egg-info/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)      308 2023-04-25 12:40:01.000000 hydrogibs-0.1.6/hydrogibs.egg-info/SOURCES.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-04-25 12:40:01.000000 hydrogibs-0.1.6/hydrogibs.egg-info/dependency_links.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-04-25 12:40:01.000000 hydrogibs-0.1.6/hydrogibs.egg-info/top_level.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)      485 2023-04-25 12:39:14.000000 hydrogibs-0.1.6/pyproject.toml
--rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-04-25 12:40:01.752954 hydrogibs-0.1.6/setup.cfg
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 12:47:06.710797 hydrogibs-0.1.7/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.1.7/LICENSE
+-rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-04-25 12:47:06.710797 hydrogibs-0.1.7/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.1.7/README.md
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 12:47:06.706797 hydrogibs-0.1.7/hydrogibs/
+-rw-rw-r--   0 axel      (1000) axel      (1000)    21642 2023-04-25 12:43:27.000000 hydrogibs-0.1.7/hydrogibs/GR4.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     2926 2023-04-25 12:03:41.000000 hydrogibs-0.1.7/hydrogibs/QDF.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      982 2023-04-25 11:49:20.000000 hydrogibs-0.1.7/hydrogibs/RationalMethod.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-04-25 11:52:06.000000 hydrogibs-0.1.7/hydrogibs/SoCoSe.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)       61 2023-04-25 12:03:58.000000 hydrogibs-0.1.7/hydrogibs/__init__.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)        0 2023-04-25 12:12:22.000000 hydrogibs-0.1.7/hydrogibs/__main__.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     4748 2023-04-25 11:52:25.000000 hydrogibs-0.1.7/hydrogibs/misc.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 12:47:06.710797 hydrogibs-0.1.7/hydrogibs.egg-info/
+-rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-04-25 12:47:06.000000 hydrogibs-0.1.7/hydrogibs.egg-info/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)      308 2023-04-25 12:47:06.000000 hydrogibs-0.1.7/hydrogibs.egg-info/SOURCES.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-04-25 12:47:06.000000 hydrogibs-0.1.7/hydrogibs.egg-info/dependency_links.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-04-25 12:47:06.000000 hydrogibs-0.1.7/hydrogibs.egg-info/top_level.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)      485 2023-04-25 12:46:55.000000 hydrogibs-0.1.7/pyproject.toml
+-rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-04-25 12:47:06.710797 hydrogibs-0.1.7/setup.cfg
```

### Comparing `hydrogibs-0.1.6/LICENSE` & `hydrogibs-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.1.6/PKG-INFO` & `hydrogibs-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.1.6
+Version: 0.1.7
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/giboul/hydrogibs
 Project-URL: Bug Tracker, https://github.com/giboul/hydrogibs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hydrogibs-0.1.6/hydrogibs/GR4.py` & `hydrogibs-0.1.7/hydrogibs/GR4.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,16 +141,16 @@
     water_flow_rain: np.ndarray
     water_flow_volume: np.ndarray
     water_flow: np.ndarray
     discharge_rain: np.ndarray
     discharge_volume: np.ndarray
     discharge: np.ndarray
 
-    def diagram(self):
-        return GR4diagram(self)
+    def diagram(self, *args, **kwargs):
+        return GR4diagram(self, *args, **kwargs)
 
 
 class GR4diagram:
 
     def __init__(self,
                  event: Event,
                  style: str = "ggplot",
@@ -697,12 +697,12 @@
     if kind == "block":
         rain = BlockRain(50, duration=1.8)
     else:
         rain = Rain(
             time=np.linspace(0, 10, 1000),
             rain_func=lambda t: 50 if t < 2 else 0
         )
-    GR4App(GR4h(Catchment(8/100, 40, 0.1, 1), rain))
+    GR4h(Catchment(8/100, 40, 0.1, 1), rain).App()
 
 
 if __name__ == "__main__":
     GR4_demo()
```

### Comparing `hydrogibs-0.1.6/hydrogibs/QDF.py` & `hydrogibs-0.1.7/hydrogibs/QDF.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.1.6/hydrogibs/RationalMethod.py` & `hydrogibs-0.1.7/hydrogibs/RationalMethod.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.1.6/hydrogibs/SoCoSe.py` & `hydrogibs-0.1.7/hydrogibs/SoCoSe.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.1.6/hydrogibs/misc.py` & `hydrogibs-0.1.7/hydrogibs/misc.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.1.6/hydrogibs.egg-info/PKG-INFO` & `hydrogibs-0.1.7/hydrogibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.1.6
+Version: 0.1.7
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/giboul/hydrogibs
 Project-URL: Bug Tracker, https://github.com/giboul/hydrogibs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

