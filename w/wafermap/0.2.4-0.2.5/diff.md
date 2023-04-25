# Comparing `tmp/wafermap-0.2.4.tar.gz` & `tmp/wafermap-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wafermap-0.2.4.tar", max compression
+gzip compressed data, was "wafermap-0.2.5.tar", max compression
```

## Comparing `wafermap-0.2.4.tar` & `wafermap-0.2.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2021-10-23 17:45:58.152508 wafermap-0.2.4/LICENSE
--rw-r--r--   0        0        0      901 2023-04-23 08:42:29.378279 wafermap-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     8086 2023-04-23 08:34:39.102338 wafermap-0.2.4/README.md
--rw-r--r--   0        0        0      171 2023-04-21 18:46:19.843838 wafermap-0.2.4/wafermap/__init__.py
--rw-r--r--   0        0        0     3134 2023-04-21 18:46:19.843838 wafermap-0.2.4/wafermap/utils.py
--rw-r--r--   0        0        0    26854 2023-04-23 08:43:21.523769 wafermap-0.2.4/wafermap/wafermap.py
--rw-r--r--   0        0        0     8689 1970-01-01 00:00:00.000000 wafermap-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-15 15:10:24.839496 wafermap-0.2.5/LICENSE
+-rw-r--r--   0        0        0      901 2023-04-25 11:34:05.171966 wafermap-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     8271 2023-04-25 11:25:04.467073 wafermap-0.2.5/README.md
+-rw-r--r--   0        0        0      171 2023-04-19 10:42:08.837188 wafermap-0.2.5/wafermap/__init__.py
+-rw-r--r--   0        0        0     3222 2023-04-25 11:13:48.075515 wafermap-0.2.5/wafermap/utils.py
+-rw-r--r--   0        0        0    27775 2023-04-25 11:27:19.164070 wafermap-0.2.5/wafermap/wafermap.py
+-rw-r--r--   0        0        0     8872 1970-01-01 00:00:00.000000 wafermap-0.2.5/PKG-INFO
```

### Comparing `wafermap-0.2.4/LICENSE` & `wafermap-0.2.5/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021, Sotiris Thomas
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021, Sotiris Thomas
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `wafermap-0.2.4/pyproject.toml` & `wafermap-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wafermap"
-version = "0.2.4"
+version = "0.2.5"
 description = "A python package to plot maps of semiconductor wafers."
 authors = ["cap1tan"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/cap1tan/wafermap"
 keywords = ["semiconductor", "wafer", "layout", "plot"]
 include = [
```

### Comparing `wafermap-0.2.4/README.md` & `wafermap-0.2.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 A python package to plot maps of semiconductor wafers.
 
 Free software: MIT license
 
 
 ## Features
 
-* Circular wafers with arbitrary notch orientations.
-* Edge-exclusion and grids with optional margin.
+* Circular wafers with arbitrary notch orientations and full or inner layouts.
+* Grid with adjustable offset and origin, cells with adjustable size and margin.
+* Edge-exclusion.
 * Hover-able points, vectors and images.
 * Tooltips with embeddable images.
 * Individual labels and colors for each die.
 * Toggle layers on/off individually.
 * Export zoom-able maps to HTML.
 * Export PNG images (needs Chromium)
 
@@ -79,14 +80,15 @@
 ```
 
 First let's define a Wafermap:
 ```python
 wm = wafermap.WaferMap(wafer_radius=100,                # all length dimensions in mm
                        cell_size=(10, 20),              # (sizeX, sizeY)
                        cell_margin=(8, 15),             # distance between cell borders (x, y)
+                       cell_origin=(0, 0),              # which cell to select as origin (0, 0), in (x, y)
                        grid_offset=(-2.05, -4.1),       # grid offset in (x, y)
                        edge_exclusion=2.2,              # margin from the wafer edge where a red edge exclusion ring is drawn
                        coverage='full',                 # 'full': will cover wafer with cells, partial cells allowed
                                                         # 'inner': only full cells allowed
                        notch_orientation=270)           # angle of notch in degrees. 270 corresponds to a notch at the bottom
 ```
```

### Comparing `wafermap-0.2.4/wafermap/utils.py` & `wafermap-0.2.5/wafermap/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,108 @@
-"""Utility functions"""
-
-import colorsys
-import math
-
-import numpy
-
-# Color functions
-
-
-def rgb_to_html(red: float, green: float, blue: float) -> str:
-    """Convert given rgb color to an HTML code"""
-    return "#%02X%02X%02X" % (red, green, blue)
-
-
-def complementary(red: int, green: int, blue: int) -> (int, int, int):
-    """returns RGB components of complementary color"""
-    hsv = colorsys.rgb_to_hsv(red, green, blue)
-    return colorsys.hsv_to_rgb((hsv[0] + 0.5) % 1, hsv[1], hsv[2])
-
-
-# Utility functions
-
-
-def euclidean_distance(point: (float, float), origin: (float, float) = None) -> float:
-    """Calculate euclidean distance from the origin"""
-    if origin is None:
-        return math.sqrt(sum((p**2 for p in point)))
-    assert len(origin) == len(point)
-    return math.sqrt(sum(((p - o) ** 2 for p, o in zip(point, origin))))
-
-
-def bounded_rectangle(
-    rect: [(float, float)], bounds: [(float, float)]
-) -> [(float, float)]:
-    """
-    Resize rectangle given by points into a rectangle that fits within bounds,
-    preserving the aspect ratio.
-    :param rect: Input rectangle [ll, ur], where each point is (y, x)
-    :param bounds: Input bounding rectangle [ll, ur]
-    :return: Bounded rectangle with same aspect ratio
-    """
-    assert len(rect) == len(bounds) == 2
-    assert rect[0][0] <= rect[1][0] and rect[0][1] <= rect[1][1]
-    assert bounds[0][0] <= bounds[1][0] and bounds[0][1] <= bounds[1][1]
-
-    width_input = rect[1][1] - rect[0][1]
-    height_input = rect[1][0] - rect[0][0]
-    width_bound = bounds[1][1] - bounds[0][1]
-    height_bound = bounds[1][0] - bounds[0][0]
-
-    width = width_input
-    height = height_input
-
-    # find new rect points
-    while width > width_bound or height > height_bound:
-        if width > width_bound:
-            # need to bound w
-            a_w = width_bound / width
-            width = width_bound
-            height = height * a_w
-
-        if height > height_bound:
-            # need to bound w
-            a_h = height_bound / height
-            height = height_bound
-            width = width * a_h
-
-    rect_out = [rect[0], (rect[0][0] + height, rect[0][1] + width)]
-
-    return rect_out
-
-
-def rotate(
-    points: [(float, float)], anchor: (float, float), angle: float = 90.0
-) -> [(float, float)]:
-    """Rotates points (nx2) about anchor (x, y) by angle in degrees"""
-    points = numpy.array(points)
-    anchor = numpy.array(anchor)
-    angle = math.radians(-angle)
-    return (
-        numpy.dot(
-            points - anchor,
-            [[math.cos(angle), math.sin(angle)], [-math.sin(angle), math.cos(angle)]],
-        )
-        + anchor
-    )
-
-
-def cart2pol(x: float, y: float) -> (float, float):
-    """Convert cartesian coordinates x, y into polar rho, phi"""
-    rho = numpy.sqrt(x**2 + y**2)
-    phi = numpy.arctan2(y, x)
-    return rho, phi
-
-
-def pol2cart(rho: float, phi: float) -> (float, float):
-    """Convert polar coordinates rho, phi into cartesian x, y"""
-    x = rho * numpy.cos(phi)
-    y = rho * numpy.sin(phi)
-    return x, y
+"""Utility functions"""
+
+import math
+
+import numpy
+
+# Color functions
+
+
+def rgb_to_html(red: float, green: float, blue: float) -> str:
+    """Convert given rgb 0-1 color to an HTML code"""
+    r, g, b = to255(red, green, blue)
+    return "#%02X%02X%02X" % (r, g, b)
+
+
+def invert(red: float, green: float, blue: float) -> (float, float, float):
+    """returns RGB components of inverted color"""
+    return 1.0 - red, 1.0 - green, 1.0 - blue
+
+
+def to255(red: float, green: float, blue: float) -> (int, int, int):
+    """returns RGB color to 0-255 scale"""
+    r = min(round(red * 255), 255)
+    g = min(round(green * 255), 255)
+    b = min(round(blue * 255), 255)
+    return r, g, b
+
+
+# Utility functions
+
+
+def euclidean_distance(point: (float, float), origin: (float, float) = None) -> float:
+    """Calculate euclidean distance from the origin"""
+    if origin is None:
+        return math.sqrt(sum((p**2 for p in point)))
+    assert len(origin) == len(point)
+    return math.sqrt(sum(((p - o) ** 2 for p, o in zip(point, origin))))
+
+
+def bounded_rectangle(
+    rect: [(float, float)], bounds: [(float, float)]
+) -> [(float, float)]:
+    """
+    Resize rectangle given by points into a rectangle that fits within bounds,
+    preserving the aspect ratio.
+    :param rect: Input rectangle [ll, ur], where each point is (y, x)
+    :param bounds: Input bounding rectangle [ll, ur]
+    :return: Bounded rectangle with same aspect ratio
+    """
+    assert len(rect) == len(bounds) == 2
+    assert rect[0][0] <= rect[1][0] and rect[0][1] <= rect[1][1]
+    assert bounds[0][0] <= bounds[1][0] and bounds[0][1] <= bounds[1][1]
+
+    width_input = rect[1][1] - rect[0][1]
+    height_input = rect[1][0] - rect[0][0]
+    width_bound = bounds[1][1] - bounds[0][1]
+    height_bound = bounds[1][0] - bounds[0][0]
+
+    width = width_input
+    height = height_input
+
+    # find new rect points
+    while width > width_bound or height > height_bound:
+        if width > width_bound:
+            # need to bound w
+            a_w = width_bound / width
+            width = width_bound
+            height = height * a_w
+
+        if height > height_bound:
+            # need to bound w
+            a_h = height_bound / height
+            height = height_bound
+            width = width * a_h
+
+    rect_out = [rect[0], (rect[0][0] + height, rect[0][1] + width)]
+
+    return rect_out
+
+
+def rotate(
+    points: [(float, float)], anchor: (float, float), angle: float = 90.0
+) -> [(float, float)]:
+    """Rotates points (nx2) about anchor (x, y) by angle in degrees"""
+    points = numpy.array(points)
+    anchor = numpy.array(anchor)
+    angle = math.radians(-angle)
+    return (
+        numpy.dot(
+            points - anchor,
+            [[math.cos(angle), math.sin(angle)], [-math.sin(angle), math.cos(angle)]],
+        )
+        + anchor
+    )
+
+
+def cart2pol(x: float, y: float) -> (float, float):
+    """Convert cartesian coordinates x, y into polar rho, phi"""
+    rho = numpy.sqrt(x**2 + y**2)
+    phi = numpy.arctan2(y, x)
+    return rho, phi
+
+
+def pol2cart(rho: float, phi: float) -> (float, float):
+    """Convert polar coordinates rho, phi into cartesian x, y"""
+    x = rho * numpy.cos(phi)
+    y = rho * numpy.sin(phi)
+    return x, y
```

### Comparing `wafermap-0.2.4/wafermap/wafermap.py` & `wafermap-0.2.5/wafermap/wafermap.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,59 +32,72 @@
     DEFAULT_VECTOR_STYLE = {"color": "#009900", "weight": 1}
     DEFAULT_POINT_STYLE = {"radius": 0.5, "fill": True}
     DEFAULT_LABEL_FONT_SIZE = 8
     DEFAULT_LABEL_HTML_STYLE = (
         f"font-size: {DEFAULT_LABEL_FONT_SIZE}pt; color: black; text-align: center;"
     )
     IMAGE_SIZE_IN_POPUP = (400, 400)
-    MAP_PADDING = (110, 0)  # in pixels (x, y)
+    MAP_PADDING = (110, 20)  # in pixels (x, y)
 
     def __init__(
         self,
         wafer_radius: float,
         cell_size: Tuple[float, float],
-        cell_margin=(0.0, 0.0),
-        grid_offset=(0.0, 0.0),
-        edge_exclusion=3,
+        cell_margin: tuple[float, float] = (0.0, 0.0),
+        cell_origin: tuple[int, int] = (0, 0),
+        grid_offset: tuple[float, float] = (0.0, 0.0),
+        edge_exclusion: float = 3.0,
         coverage="full",
-        notch_orientation=270,
-        bg_color=(1, 1, 1),
-        conversion_factor=1,
+        notch_orientation: float = 270.0,
+        wafer_edge_color: tuple[float, float, float] = (0.0, 0.0, 0.0),
+        map_bg_color: Union[None, tuple[float, float, float]] = None,
+        conversion_factor: float = 1.0,
     ):
         """
         The wafermap origin is always the central die.
         :param wafer_radius: Wafer diameter in mm
         :param cell_size: Cell size in mm, (x, y)
         :param cell_margin: Distance between cells in mm, (x, y)
+        :param cell_origin: The cell index that is the origin (0, 0) of the map, (x, y)
         :param grid_offset: Grid offset in mm, (x, y)
         :param edge_exclusion: Margin from the wafer edge where a red edge exclusion
         ring is drawn in mm.
         :param coverage: Options of 'full', 'inner'. Option 'full' will cover wafer with
          cells, partial cells allowed, 'inner' will only allow full cells
-        :param bg_color: Tuple of (r, g, b), 0-255.
+        :param wafer_edge_color: Tuple of (r, g, b), 0-1 for the wafer edge color.
+        :param map_bg_color: Tuple of (r, g, b), 0-1 for the map background color. If
+        None, the inverted wafer_edge_color will be selected
         :param conversion_factor: Factor to multiply input dimensions with.
         """
 
         assert cell_size[0] > 0
         assert cell_size[1] > 0
         assert coverage.lower() in ["full", "inner"]
+        assert len(wafer_edge_color) == 3
+        assert all([x >= 0 for x in wafer_edge_color])
 
         self.coverage = coverage.lower()
         self.cell_size_x = conversion_factor * cell_size[0]
         self.cell_size_y = conversion_factor * cell_size[1]
         self.cell_margin_x = conversion_factor * cell_margin[0]
         self.cell_margin_y = conversion_factor * cell_margin[1]
+        self.cell_origin_x = int(cell_origin[0])
+        self.cell_origin_y = int(cell_origin[1])
         self.wafer_radius = conversion_factor * wafer_radius
         self.edge_exclusion = conversion_factor * edge_exclusion
         self.grid_offset_x = conversion_factor * grid_offset[0]
         self.grid_offset_y = conversion_factor * grid_offset[1]
         self._num_of_cells_x = math.ceil(2 * self.wafer_radius / self.cell_size_x)
         self._num_of_cells_y = math.ceil(2 * self.wafer_radius / self.cell_size_y)
         self.notch_orientation = notch_orientation
-        wafer_edge_color = utils.rgb_to_html(*utils.complementary(*bg_color))
+        if map_bg_color is None:
+            map_bg_color = utils.to255(*utils.invert(*wafer_edge_color))
+        else:
+            map_bg_color = utils.to255(*map_bg_color)
+        wafer_edge_color = utils.rgb_to_html(*wafer_edge_color)
 
         # init the _cell_map
         # the cell map is a dict that corresponds the pixel coordinates of the bounding
         # box of each cell to the cell index:
         # {(cell_y, cell_x): ((y_lower_left, x_lower_left),
         #                     (y_lower_right, x_lower_right),
         #                     (y_upper_left, x_upper_left),
@@ -109,20 +122,22 @@
             zoomSnap=0,
             zoomDelta=0.1,
             png_enabled=True,
         )
 
         # Add the base layer
         # Create a white image of 4 pixels, and embed it in an url.
-        white_tile = branca.utilities.image_to_url([[bg_color] * 2, [bg_color] * 2])
-        # create base TileLayer (white background)
+        bg_tile = branca.utilities.image_to_url(
+            [[map_bg_color] * 2, [map_bg_color] * 2]
+        )
+        # create base TileLayer
         self._tile_layer = folium.raster_layers.TileLayer(
-            tiles=white_tile,
+            tiles=bg_tile,
             name="base",
-            attr="white tile",
+            attr="bg tile",
         )
         self._tile_layer.add_to(folium_map)
 
         # Init rest of layers
         self._grid_layer = folium.map.FeatureGroup(name="grid")
         self._cell_labels_layer = folium.map.FeatureGroup(
             name="cell labels", show=False
@@ -170,15 +185,15 @@
         # Add grid
         min_index_x = -math.ceil(self._num_of_cells_x / 2) - 1
         max_index_x = math.ceil(self._num_of_cells_x / 2) + 1
         min_index_y = -math.ceil(self._num_of_cells_y / 2) - 1
         max_index_y = math.ceil(self._num_of_cells_y / 2) + 1
         for i_x in range(min_index_x, max_index_x):
             for i_y in range(min_index_y, max_index_y):
-                cell_label = (i_y, i_x)
+                cell_label = (i_y - self.cell_origin_y, i_x - self.cell_origin_x)
                 # print a box
                 lower_bound = (
                     (i_y - 0.5) * (self.cell_size_y + self.cell_margin_y)
                     + self.grid_offset_y,
                     (i_x - 0.5) * (self.cell_size_x + self.cell_margin_x)
                     + self.grid_offset_x,
                 )
```

### Comparing `wafermap-0.2.4/PKG-INFO` & `wafermap-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wafermap
-Version: 0.2.4
+Version: 0.2.5
 Summary: A python package to plot maps of semiconductor wafers.
 Home-page: https://github.com/cap1tan/wafermap
 License: MIT
 Keywords: semiconductor,wafer,layout,plot
 Author: cap1tan
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -39,16 +39,17 @@
 A python package to plot maps of semiconductor wafers.
 
 Free software: MIT license
 
 
 ## Features
 
-* Circular wafers with arbitrary notch orientations.
-* Edge-exclusion and grids with optional margin.
+* Circular wafers with arbitrary notch orientations and full or inner layouts.
+* Grid with adjustable offset and origin, cells with adjustable size and margin.
+* Edge-exclusion.
 * Hover-able points, vectors and images.
 * Tooltips with embeddable images.
 * Individual labels and colors for each die.
 * Toggle layers on/off individually.
 * Export zoom-able maps to HTML.
 * Export PNG images (needs Chromium)
 
@@ -102,14 +103,15 @@
 ```
 
 First let's define a Wafermap:
 ```python
 wm = wafermap.WaferMap(wafer_radius=100,                # all length dimensions in mm
                        cell_size=(10, 20),              # (sizeX, sizeY)
                        cell_margin=(8, 15),             # distance between cell borders (x, y)
+                       cell_origin=(0, 0),              # which cell to select as origin (0, 0), in (x, y)
                        grid_offset=(-2.05, -4.1),       # grid offset in (x, y)
                        edge_exclusion=2.2,              # margin from the wafer edge where a red edge exclusion ring is drawn
                        coverage='full',                 # 'full': will cover wafer with cells, partial cells allowed
                                                         # 'inner': only full cells allowed
                        notch_orientation=270)           # angle of notch in degrees. 270 corresponds to a notch at the bottom
 ```
```

