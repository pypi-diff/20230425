# Comparing `tmp/hydrogibs-0.0.9.tar.gz` & `tmp/hydrogibs-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrogibs-0.0.9.tar", last modified: Tue Apr 25 11:11:36 2023, max compression
+gzip compressed data, was "hydrogibs-0.1.4.tar", last modified: Tue Apr 25 12:17:59 2023, max compression
```

## Comparing `hydrogibs-0.0.9.tar` & `hydrogibs-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 11:11:36.575677 hydrogibs-0.0.9/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.0.9/LICENSE
--rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-25 11:11:36.571677 hydrogibs-0.0.9/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.0.9/README.md
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 11:11:36.571677 hydrogibs-0.0.9/hydrogibs/
--rw-rw-r--   0 axel      (1000) axel      (1000)    21448 2023-04-25 11:06:59.000000 hydrogibs-0.0.9/hydrogibs/GR4.py
--rw-rw-r--   0 axel      (1000) axel      (1000)      120 2023-04-25 01:47:38.000000 hydrogibs-0.0.9/hydrogibs/__init_.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     9213 2023-04-24 14:45:59.000000 hydrogibs-0.0.9/hydrogibs/misc.py
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 11:11:36.571677 hydrogibs-0.0.9/hydrogibs.egg-info/
--rw-rw-r--   0 axel      (1000) axel      (1000)      541 2023-04-25 11:11:36.000000 hydrogibs-0.0.9/hydrogibs.egg-info/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)      220 2023-04-25 11:11:36.000000 hydrogibs-0.0.9/hydrogibs.egg-info/SOURCES.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-04-25 11:11:36.000000 hydrogibs-0.0.9/hydrogibs.egg-info/dependency_links.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-04-25 11:11:36.000000 hydrogibs-0.0.9/hydrogibs.egg-info/top_level.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)      489 2023-04-25 11:10:05.000000 hydrogibs-0.0.9/pyproject.toml
--rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-04-25 11:11:36.575677 hydrogibs-0.0.9/setup.cfg
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 12:17:59.855650 hydrogibs-0.1.4/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.1.4/LICENSE
+-rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-04-25 12:17:59.855650 hydrogibs-0.1.4/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.1.4/README.md
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 12:17:59.851649 hydrogibs-0.1.4/hydrogibs/
+-rw-rw-r--   0 axel      (1000) axel      (1000)    21681 2023-04-25 11:42:18.000000 hydrogibs-0.1.4/hydrogibs/GR4.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     2926 2023-04-25 12:03:41.000000 hydrogibs-0.1.4/hydrogibs/QDF.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      982 2023-04-25 11:49:20.000000 hydrogibs-0.1.4/hydrogibs/RationalMethod.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-04-25 11:52:06.000000 hydrogibs-0.1.4/hydrogibs/SoCoSe.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)       61 2023-04-25 12:03:58.000000 hydrogibs-0.1.4/hydrogibs/__init__.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)        0 2023-04-25 12:12:22.000000 hydrogibs-0.1.4/hydrogibs/__main__.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     4748 2023-04-25 11:52:25.000000 hydrogibs-0.1.4/hydrogibs/misc.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 12:17:59.855650 hydrogibs-0.1.4/hydrogibs.egg-info/
+-rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-04-25 12:17:59.000000 hydrogibs-0.1.4/hydrogibs.egg-info/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)      308 2023-04-25 12:17:59.000000 hydrogibs-0.1.4/hydrogibs.egg-info/SOURCES.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-04-25 12:17:59.000000 hydrogibs-0.1.4/hydrogibs.egg-info/dependency_links.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-04-25 12:17:59.000000 hydrogibs-0.1.4/hydrogibs.egg-info/top_level.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)      485 2023-04-25 12:17:09.000000 hydrogibs-0.1.4/pyproject.toml
+-rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-04-25 12:17:59.855650 hydrogibs-0.1.4/setup.cfg
```

### Comparing `hydrogibs-0.0.9/LICENSE` & `hydrogibs-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.0.9/PKG-INFO` & `hydrogibs-0.1.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.0.9
+Version: 0.1.4
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://github.com/giboul/hydrogibs
+Project-URL: Bug Tracker, https://github.com/giboul/hydrogibs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hydrogibs-0.0.9/hydrogibs/GR4.py` & `hydrogibs-0.1.4/hydrogibs/GR4.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,17 +19,25 @@
         return 3/(2*X4) * n**2
     if n < 2:
         return 3/(2*X4) * (2-n)**2
     return 0
 
 
 class Rain:
-
     """
-    Rain object to apply to a catchment
+    Rain object to apply to a Catchment object.
+
+    Args:
+        - time        (np.ndarray)       [h]
+        - rain_func   (callable)   -> [mm/h]
+
+    Creates a GR4h object when called with a Catchment object:
+    >>> gr4h = GR4h(catchment, rain)
+    Creates an Event object when applied to a catchment
+    >>> event = rain @ catchment
     """
 
     def __init__(self, time: np.ndarray, rain_func: Callable) -> None:
 
         self.time = time
         self.rain_func = rain_func
         self.rainfall = np.array([rain_func(t) for t in time])
@@ -45,17 +53,18 @@
 
     Args:
         - intensity        (floaat)[mm/h]
         - duration         (float) [h]
         - timestep         (float) [h]: directly linked to precision
         - observation_span (float) [h]: the duration of the experiment
 
-    Can create a GR4h object when calles with a Catchment object:
-    >>> gr4h = rain @ catchment
+    Creates a GR4h object when called with a Catchment object:
     >>> gr4h = GR4h(catchment, rain)
+    Creates an Event object when applied to a catchment
+    >>> event = rain @ catchment
     """
 
     def __init__(self,
                  intensity: float,
                  duration: float = 1.0,
                  timestep: float = None,
                  observation_span: float = None) -> None:
@@ -81,19 +90,18 @@
         assert 0 <= observation_span > duration
 
 
 class Catchment:
     """
     Stores GR4h catchment parameters.
 
-    Returns a GR4h object when called with a Rain object:
-        >>> catchment = Catchment(X1=8/100, X2=40, X3=0.1, X4=1)
-        >>> rain = BlockRain(intensity=50)
-        >>> gr4: GR4h = catchment @ rain  # first syntax
-        >>> gr4: GR4h = GR4h(catchment, rain)  # second syntax
+    Creates a GR4h object when called with a Rain object:
+    >>> gr4h = GR4h(catchment, rain)
+    Creates an Event object when applied to a Rain object
+    >>> event = rain @ catchment
 
     Args:
         X1 (float)  [-] : dQ = X1 * dPrecipitations
         X2 (float)  [mm]: Initial abstraction (vegetation interception)
         X3 (float) [1/h]: Sub-surface water volume emptying rate dQs = X3*V*dt
         X4 (float)  [h] : the hydrogram's raising time
     """
@@ -324,17 +332,16 @@
     """
     Object storing a Catchment object, a Rain object, and Event object
     and eventually attributes relative to a diagram
 
     A GR4h object is obtained when called with a Rain and a Catchment objects:
         >>> catchment = Catchment(X1=8/100, X2=40, X3=0.1, X4=1)
         >>> rain = BlockRain(intensity=50)
-        >>> gr4: GR4h = catchment @ rain  # first syntax
-        >>> gr4: GR4h = GR4h(catchment, rain)  # second syntax
-        >>> gr4.App()  # opens an interactive diagram in a tkinter window
+        >>> gr4h: GR4h = GR4h(catchment, rain)  # second syntax
+        >>> gr4h.App()  # opens an interactive diagram in a tkinter window
 
     Args:
         catchment (Catchment): contains essential parameters
         rain      (Rain): contains the rainfall event details
 
     Returns:
         gr4h (GR4h): Object contaning an Event object (discharges, water flow)
@@ -357,21 +364,21 @@
 
         self.apply()
 
     def apply_block_rain(self):
 
         self.event = gr4_block_rain(self.catchment, self.rain)
 
-        return self
+        return self.event
 
     def apply_rain(self):
 
         self.event = gr4_diff(self.catchment, self.rain)
 
-        return self
+        return self.event
 
     def create_diagram(self, *args, **kwargs):
 
         self.diagram = GR4diagram(self.event, *args, **kwargs)
 
     def App(self):
         GR4App(self)
@@ -677,20 +684,21 @@
     def update(self):
 
         self.gr4.apply()
         self.diagram.update(self.gr4.event, self.gr4.rain)
         self.canvas.draw()
 
 
-def GR4_demo():
-    # time = np.linspace(0, 10, 1000)
-    # gr4 = Catchment(8/100, 40, 0.1, 1, initial_volume=30) @ Rain(
-    #     time,
-    #     rain_func=lambda t: 50 if t < 2 else 0
-    # )
-    gr4 = Catchment(8/100, 40, 0.1, 1) @ BlockRain(50, duration=1.8)
-    gr4 = gr4.apply()
+def GR4_demo(kind="block"):
+
+    if kind == "block":
+        gr4 = Catchment(8/100, 40, 0.1, 1) @ BlockRain(50, duration=1.8)
+    else:
+        gr4 = Catchment(8/100, 40, 0.1, 1, initial_volume=30) @ Rain(
+            time=np.linspace(0, 10, 1000),
+            rain_func=lambda t: 50 if t < 2 else 0
+        )
     gr4.App()
 
 
 if __name__ == "__main__":
     GR4_demo()
```

### Comparing `hydrogibs-0.0.9/hydrogibs.egg-info/PKG-INFO` & `hydrogibs-0.1.4/hydrogibs.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.0.9
+Version: 0.1.4
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://github.com/giboul/hydrogibs
+Project-URL: Bug Tracker, https://github.com/giboul/hydrogibs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

