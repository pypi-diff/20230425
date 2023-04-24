# Comparing `tmp/odb-plotter-0.4.5.tar.gz` & `tmp/odb-plotter-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odb-plotter-0.4.5.tar", last modified: Fri Mar 31 17:27:18 2023, max compression
+gzip compressed data, was "odb-plotter-0.4.6.tar", last modified: Mon Apr 24 22:21:45 2023, max compression
```

## Comparing `odb-plotter-0.4.5.tar` & `odb-plotter-0.4.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-03-31 17:27:18.371646 odb-plotter-0.4.5/
--rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-02-07 20:18:25.000000 odb-plotter-0.4.5/LICENSE
--rw-r--r--   0 clark     (1000) clark     (1000)     2569 2023-03-31 17:27:18.371646 odb-plotter-0.4.5/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)      694 2023-02-20 19:23:31.000000 odb-plotter-0.4.5/README.md
--rw-r--r--   0 clark     (1000) clark     (1000)     1271 2023-03-20 21:18:42.000000 odb-plotter-0.4.5/pyproject.toml
--rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-03-31 17:27:18.371646 odb-plotter-0.4.5/setup.cfg
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-03-31 17:27:18.368313 odb-plotter-0.4.5/src/
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-03-31 17:27:18.371646 odb-plotter-0.4.5/src/odb_plotter.egg-info/
--rw-r--r--   0 clark     (1000) clark     (1000)     2569 2023-03-31 17:27:18.000000 odb-plotter-0.4.5/src/odb_plotter.egg-info/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)      525 2023-03-31 17:27:18.000000 odb-plotter-0.4.5/src/odb_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-03-31 17:27:18.000000 odb-plotter-0.4.5/src/odb_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 clark     (1000) clark     (1000)      195 2023-03-31 17:27:18.000000 odb-plotter-0.4.5/src/odb_plotter.egg-info/requires.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-03-31 17:27:18.000000 odb-plotter-0.4.5/src/odb_plotter.egg-info/top_level.txt
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-03-31 17:27:18.371646 odb-plotter-0.4.5/src/odbp/
--rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-03-31 02:50:10.000000 odb-plotter-0.4.5/src/odbp/__init__.py
--rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-02-08 21:45:04.000000 odb-plotter-0.4.5/src/odbp/__main__.py
--rw-r--r--   0 clark     (1000) clark     (1000)    26212 2023-03-27 21:54:24.000000 odb-plotter-0.4.5/src/odbp/cli.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-03-31 17:27:18.371646 odb-plotter-0.4.5/src/odbp/data/
--rw-r--r--   0 clark     (1000) clark     (1000)     5191 2023-03-01 19:01:13.000000 odb-plotter-0.4.5/src/odbp/data/config.toml
--rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-03-01 19:01:13.000000 odb-plotter-0.4.5/src/odbp/data/views.toml
--rw-r--r--   0 clark     (1000) clark     (1000)     1366 2023-03-20 21:18:42.000000 odb-plotter-0.4.5/src/odbp/npz_to_hdf.py
--rw-r--r--   0 clark     (1000) clark     (1000)    10839 2023-03-31 01:27:50.000000 odb-plotter-0.4.5/src/odbp/odb.py
--rw-r--r--   0 clark     (1000) clark     (1000)     4443 2023-03-20 21:18:42.000000 odb-plotter-0.4.5/src/odbp/odb_visualizer.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-03-31 17:27:18.371646 odb-plotter-0.4.5/src/odbp/py2_scripts/
--rw-r--r--   0 clark     (1000) clark     (1000)     6349 2023-03-27 18:20:55.000000 odb-plotter-0.4.5/src/odbp/py2_scripts/extract.py
--rw-r--r--   0 clark     (1000) clark     (1000)     8976 2023-03-27 21:54:24.000000 odb-plotter-0.4.5/src/odbp/py2_scripts/odb_to_npz.py
--rw-r--r--   0 clark     (1000) clark     (1000)     2023 2023-03-20 21:18:42.000000 odb-plotter-0.4.5/src/odbp/read_hdf5.py
--rw-r--r--   0 clark     (1000) clark     (1000)    29923 2023-03-31 02:50:56.000000 odb-plotter-0.4.5/src/odbp/state.py
--rw-r--r--   0 clark     (1000) clark     (1000)      914 2023-03-20 21:18:42.000000 odb-plotter-0.4.5/src/odbp/util.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-04-24 22:21:45.655544 odb-plotter-0.4.6/
+-rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-02-07 20:18:25.000000 odb-plotter-0.4.6/LICENSE
+-rw-r--r--   0 clark     (1000) clark     (1000)     2569 2023-04-24 22:21:45.655544 odb-plotter-0.4.6/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)      694 2023-02-20 19:23:31.000000 odb-plotter-0.4.6/README.md
+-rw-r--r--   0 clark     (1000) clark     (1000)     1271 2023-03-20 21:18:42.000000 odb-plotter-0.4.6/pyproject.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-04-24 22:21:45.655544 odb-plotter-0.4.6/setup.cfg
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-04-24 22:21:45.652210 odb-plotter-0.4.6/src/
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-04-24 22:21:45.652210 odb-plotter-0.4.6/src/odb_plotter.egg-info/
+-rw-r--r--   0 clark     (1000) clark     (1000)     2569 2023-04-24 22:21:45.000000 odb-plotter-0.4.6/src/odb_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)      525 2023-04-24 22:21:45.000000 odb-plotter-0.4.6/src/odb_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-04-24 22:21:45.000000 odb-plotter-0.4.6/src/odb_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)      195 2023-04-24 22:21:45.000000 odb-plotter-0.4.6/src/odb_plotter.egg-info/requires.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-04-24 22:21:45.000000 odb-plotter-0.4.6/src/odb_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-04-24 22:21:45.655544 odb-plotter-0.4.6/src/odbp/
+-rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-04-24 22:21:35.000000 odb-plotter-0.4.6/src/odbp/__init__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-02-08 21:45:04.000000 odb-plotter-0.4.6/src/odbp/__main__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    26212 2023-03-27 21:54:24.000000 odb-plotter-0.4.6/src/odbp/cli.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-04-24 22:21:45.655544 odb-plotter-0.4.6/src/odbp/data/
+-rw-r--r--   0 clark     (1000) clark     (1000)     5191 2023-03-01 19:01:13.000000 odb-plotter-0.4.6/src/odbp/data/config.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-03-01 19:01:13.000000 odb-plotter-0.4.6/src/odbp/data/views.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)     1366 2023-03-20 21:18:42.000000 odb-plotter-0.4.6/src/odbp/npz_to_hdf.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    10839 2023-04-24 22:17:15.000000 odb-plotter-0.4.6/src/odbp/odb.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     5111 2023-04-24 22:18:56.000000 odb-plotter-0.4.6/src/odbp/odb_visualizer.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-04-24 22:21:45.655544 odb-plotter-0.4.6/src/odbp/py2_scripts/
+-rw-r--r--   0 clark     (1000) clark     (1000)     6349 2023-03-27 18:20:55.000000 odb-plotter-0.4.6/src/odbp/py2_scripts/extract.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     8976 2023-03-27 21:54:24.000000 odb-plotter-0.4.6/src/odbp/py2_scripts/odb_to_npz.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     2023 2023-03-20 21:18:42.000000 odb-plotter-0.4.6/src/odbp/read_hdf5.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    29923 2023-04-24 22:17:15.000000 odb-plotter-0.4.6/src/odbp/state.py
+-rw-r--r--   0 clark     (1000) clark     (1000)      914 2023-03-20 21:18:42.000000 odb-plotter-0.4.6/src/odbp/util.py
```

### Comparing `odb-plotter-0.4.5/LICENSE` & `odb-plotter-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.4.5/PKG-INFO` & `odb-plotter-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.4.5
+Version: 0.4.6
 Summary: Python3 API for Abaqus FEA .odb Files and related Command Line Visualization Tool, with an Additive Manufacturing Focus
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
```

### Comparing `odb-plotter-0.4.5/README.md` & `odb-plotter-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.4.5/pyproject.toml` & `odb-plotter-0.4.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.4.5/src/odb_plotter.egg-info/PKG-INFO` & `odb-plotter-0.4.6/src/odb_plotter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.4.5
+Version: 0.4.6
 Summary: Python3 API for Abaqus FEA .odb Files and related Command Line Visualization Tool, with an Additive Manufacturing Focus
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
```

### Comparing `odb-plotter-0.4.5/src/odb_plotter.egg-info/SOURCES.txt` & `odb-plotter-0.4.6/src/odb_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.4.5/src/odbp/cli.py` & `odb-plotter-0.4.6/src/odbp/cli.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.4.5/src/odbp/data/config.toml` & `odb-plotter-0.4.6/src/odbp/data/config.toml`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.4.5/src/odbp/npz_to_hdf.py` & `odb-plotter-0.4.6/src/odbp/npz_to_hdf.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.4.5/src/odbp/odb.py` & `odb-plotter-0.4.6/src/odbp/odb.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.4.5/src/odbp/odb_visualizer.py` & `odb-plotter-0.4.6/src/odbp/odb_visualizer.py`

 * *Files 20% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 
     def select_colormap(self) -> None:
         if not (hasattr(self, "meltpoint") or hasattr(self, "colormap_name")):
             raise MeltpointNotSetError
 
         # TODO different melt color? Don't plot from as low as 0?
-        self.colormap = pv.LookupTable(cmap=self.colormap_name, scalar_range=(self.low_temp, self.meltpoint), above_range_color=(0.25, 0.25, 0.25, 1.0))
+        self.colormap = pv.LookupTable(cmap=self.colormap_name, scalar_range=(self.low_temp, self.meltpoint), above_range_color=(0.75, 0.75, 0.75, 1.0))
 
 
     # Overload parent's set_meltpoint method to always select colormap
     def set_meltpoint(self, meltpoint: float) -> None:
         if not isinstance(meltpoint, float):
             meltpoint = float(meltpoint)
         self.meltpoint = meltpoint
@@ -64,16 +64,16 @@
     def plot_time_3d(self, time: float, label: str, interactive: bool)-> Any:
         curr_nodes: Any = self.out_nodes[self.out_nodes["Time"] == time]
 
         formatted_time: str = format(round(time, 2), ".2f")
         combined_label = f"{label}-{formatted_time}"
 
         off_screen: bool = not interactive
-        plotter = pv.Plotter(off_screen=off_screen, window_size=[1920, 1080])
-        plotter.add_text(combined_label, position="upper_edge", color="white", font="courier", )
+        plotter = pv.Plotter(off_screen=off_screen, window_size=[1920, 1080], lighting="three lights")
+        plotter.add_text(combined_label, position="upper_edge", color="#000000", font="courier", )
         faces: list[str] = ["x_low", "x_high", "y_low", "y_high", "z_low", "z_high"]
         face: str
         for face in faces:
             selected_nodes: Any
 
             # TODO This whole idea could be parameterized, but it might be less readable
             if "x" in face:
@@ -98,19 +98,28 @@
             points: Any = pv.PolyData(selected_nodes.drop(columns=list(set(selected_nodes.columns.values.tolist()) - dims_columns)).to_numpy())
             points["Temp"] = selected_nodes["Temp"].to_numpy()
             surface: Any = points.delaunay_2d()
 
             # For whatever reason, the input data is rotated 180 degrees about the y axis. This fixes that.
             #surface = surface.rotate_z(180)
 
-            plotter.add_mesh(surface, scalars="Temp", cmap=self.colormap, scalar_bar_args={"title": "Nodal Temperature (Kelvins)"})
+            plotter.add_mesh(surface, scalars="Temp", cmap=self.colormap, scalar_bar_args={"title": "Nodal Temperature (kelvins)", "font_family": "courier", "color": "#000000", "fmt": "%.2f", "position_y": 0})
+            dims_columns: set[str] = set(["X", "Y", "Z"])
+            points: Any = pv.PolyData(selected_nodes.drop(columns=list(set(selected_nodes.columns.values.tolist()) - dims_columns)).to_numpy())
+            points["Temp"] = selected_nodes["Temp"].to_numpy()
+            surface: Any = points.delaunay_2d()
+
+            # For whatever reason, the input data is rotated 180 degrees about the y axis. This fixes that.
+            #surface = surface.rotate_z(180)
 
-        plotter.show_bounds(location="outer", ticks="both", font_size=14.0, font_family="courier", color="#FFFFFF", axes_ranges=[self.x.low, self.x.high, self.y.low, self.y.high, self.z.low, self.z.high])
-        plotter.set_background(color="#000000")
+        plotter.show_bounds(location="outer", ticks="both", font_size=14.0, font_family="courier", color="#000000", axes_ranges=[self.x.low, self.x.high, self.y.low, self.y.high, self.z.low, self.z.high])
+        plotter.set_background(color="#FFFFFF")
 
         #plotter.camera.focal_point = ((self.x.high + self.x.low)/2, (self.y.high + self.y.low)/2, (self.z.high + self.z.low)/2)
         plotter.camera.elevation = 0
         plotter.camera.azimuth = 270
         plotter.camera.roll = 300
         plotter.camera_set = True
+        #plotter.disable_shadows()
+        #plotter.add_light(pv.Light(light_type="headlight"))
 
         return plotter
```

### Comparing `odb-plotter-0.4.5/src/odbp/py2_scripts/extract.py` & `odb-plotter-0.4.6/src/odbp/py2_scripts/extract.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.4.5/src/odbp/py2_scripts/odb_to_npz.py` & `odb-plotter-0.4.6/src/odbp/py2_scripts/odb_to_npz.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.4.5/src/odbp/read_hdf5.py` & `odb-plotter-0.4.6/src/odbp/read_hdf5.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.4.5/src/odbp/state.py` & `odb-plotter-0.4.6/src/odbp/state.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.4.5/src/odbp/util.py` & `odb-plotter-0.4.6/src/odbp/util.py`

 * *Files identical despite different names*

