# Comparing `tmp/blender_plots-1.0.1-py3-none-any.whl.zip` & `tmp/blender_plots-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 21386 bytes, number of entries: 10
--rw-rw-r--  2.0 unx       78 b- defN 23-Apr-24 13:30 blender_plots/__init__.py
--rw-rw-r--  2.0 unx     6142 b- defN 23-Apr-24 13:34 blender_plots/blender_utils.py
--rw-rw-r--  2.0 unx     3354 b- defN 23-Apr-24 13:44 blender_plots/plots_base.py
--rw-rw-r--  2.0 unx    11103 b- defN 23-Apr-24 13:33 blender_plots/scatter.py
--rw-rw-r--  2.0 unx     1507 b- defN 23-Apr-24 09:32 blender_plots/surface.py
--rw-rw-r--  2.0 unx    35149 b- defN 23-Apr-24 13:52 blender_plots-1.0.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx      224 b- defN 23-Apr-24 13:52 blender_plots-1.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-24 13:52 blender_plots-1.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Apr-24 13:52 blender_plots-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      830 b- defN 23-Apr-24 13:52 blender_plots-1.0.1.dist-info/RECORD
-10 files, 58493 bytes uncompressed, 19966 bytes compressed:  65.9%
+Zip file size: 22057 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx      210 b- defN 23-Apr-24 21:48 blender_plots/__init__.py
+-rw-rw-r--  2.0 unx     7273 b- defN 23-Apr-24 19:26 blender_plots/blender_utils.py
+-rw-rw-r--  2.0 unx     5492 b- defN 23-Apr-24 20:40 blender_plots/plots_base.py
+-rw-rw-r--  2.0 unx     8594 b- defN 23-Apr-24 21:48 blender_plots/scatter.py
+-rw-rw-r--  2.0 unx     3255 b- defN 23-Apr-24 20:45 blender_plots/surface.py
+-rw-rw-r--  2.0 unx    35149 b- defN 23-Apr-25 10:43 blender_plots-1.0.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      224 b- defN 23-Apr-25 10:43 blender_plots-1.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-25 10:43 blender_plots-1.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-Apr-25 10:43 blender_plots-1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      830 b- defN 23-Apr-25 10:43 blender_plots-1.0.2.dist-info/RECORD
+10 files, 61133 bytes uncompressed, 20637 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: blender_plots/scatter.py
 Comment: 
 
 Filename: blender_plots/surface.py
 Comment: 
 
-Filename: blender_plots-1.0.1.dist-info/LICENSE
+Filename: blender_plots-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: blender_plots-1.0.1.dist-info/METADATA
+Filename: blender_plots-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: blender_plots-1.0.1.dist-info/WHEEL
+Filename: blender_plots-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: blender_plots-1.0.1.dist-info/top_level.txt
+Filename: blender_plots-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: blender_plots-1.0.1.dist-info/RECORD
+Filename: blender_plots-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## blender_plots/__init__.py

```diff
@@ -1,2 +1,7 @@
-from blender_plots.scatter import *
-from blender_plots.blender_utils import *
+import blender_plots.blender_utils
+import blender_plots.plots_base
+import blender_plots.scatter
+import blender_plots.surface
+
+from blender_plots.scatter import Scatter
+from blender_plots.surface import Surface
```

## blender_plots/blender_utils.py

```diff
@@ -1,12 +1,18 @@
+from dataclasses import dataclass
 import numpy as np
 
 import bpy
 
-MARKER_COLOR = "marker_color"
+
+@dataclass
+class Constants:
+    MARKER_COLOR = "marker_color"
+    FRAME_INDEX = "frame_index"
+
 
 class NodeLinker:
     """Wrapper for bpy.types.GeometryNodeTree which simplifies creating large node trees."""
 
     def __init__(self, node_group):
         self.node_group = node_group
 
@@ -34,15 +40,15 @@
                 match key.split("_"):
                     case ["input", i] if i.isdigit():
                         blender_key = int(i)
                     case _:
                         blender_key = python_arg_to_blender_key(key)
                 if isinstance(value, bpy.types.NodeSocket):
                     self.link(value, node.inputs[blender_key])
-                elif isinstance(blender_key, int) or blender_key in node.inputs:
+                elif (isinstance(blender_key, int) or blender_key in node.inputs) and hasattr(node.inputs[blender_key], "default_value"):
                     node.inputs[blender_key].default_value = value
                 elif hasattr(node, key):
                     setattr(node, key, value)
                 else:
                     raise ValueError(f"Node {node} has no attribute {key} or input {blender_key}.")
         return node
 
@@ -124,22 +130,48 @@
     if color.shape[1] == 3:
         color = np.hstack([color, np.ones((len(color), 1))])
     elif not color.shape[1] == 4:
         raise ValueError(f"Invalid color array shape {color.shape}, expected Nx3 or Nx4")
     if len(mesh.vertices) != len(color):
         raise ValueError(f"Got {len(mesh.vertices)} vertices and {len(color)} color values")
 
-    if MARKER_COLOR not in mesh.attributes:
-        mesh.attributes.new(name=MARKER_COLOR, type="FLOAT_COLOR", domain="POINT")
-    mesh.attributes[MARKER_COLOR].data.foreach_set("color", color.reshape(-1))
+    if Constants.MARKER_COLOR not in mesh.attributes:
+        mesh.attributes.new(name=Constants.MARKER_COLOR, type="FLOAT_COLOR", domain="POINT")
+    mesh.attributes[Constants.MARKER_COLOR].data.foreach_set("color", color.reshape(-1))
 
 
 def get_vertex_color_material():
     """Create a material that obtains its color from the marker_color attribute"""
     material = bpy.data.materials.new("color")
     material.use_nodes = True
     color_node = material.node_tree.nodes.new("ShaderNodeAttribute")
-    color_node.attribute_name = MARKER_COLOR
+    color_node.attribute_name = Constants.MARKER_COLOR
 
     material.node_tree.links.new(color_node.outputs["Color"],
                                  material.node_tree.nodes["Principled BSDF"].inputs["Base Color"])
     return material
+
+def get_frame_selection_node(modifier, n_frames):
+    """Add node that filters points based on the Frame Index property."""
+    node_linker = NodeLinker(modifier.node_group)
+    frame_index = node_linker.new_node(
+        "GeometryNodeInputNamedAttribute",
+        data_type="FLOAT",
+        name=Constants.FRAME_INDEX,
+    )
+    frame_selection_node = node_linker.new_node(
+        "ShaderNodeMath",
+        operation="COMPARE",
+        input_1=frame_index.outputs[1],
+        input_2=0.5
+    )
+
+    action = bpy.data.actions.new("AnimationAction")
+    fcurve = action.fcurves.new(data_path='nodes["Math"].inputs[0].default_value', index=0)
+    fcurve.keyframe_points.add(2)
+    fcurve.keyframe_points.foreach_set("co", [0, 0, n_frames, n_frames])
+    bpy.context.scene.frame_end = n_frames - 1
+
+    modifier.node_group.animation_data_create()
+    modifier.node_group.animation_data.action = action
+
+    return frame_selection_node
```

## blender_plots/plots_base.py

```diff
@@ -8,32 +8,60 @@
     def __init__(self, x, y, z, color=None, name="plot", n_dims=1):
         self.name = name
         self.mesh = bpy.data.meshes.new(self.name)
         self.base_object = bu.new_empty(self.name, self.mesh)
         self.color_material = None
         self.color_material = None
         self._points = None
+        self.modifier = self.base_object.modifiers.new(type="NODES", name=name)
 
         points, self.n_frames, *self.dims = get_points_array(x, y, z, n_dims)
         self.points = points
         self.color = color
 
     @property
+    def n_points(self):
+        return np.prod(self.dims)
+
+    @property
+    def n_vertices(self):
+        return self.n_points * (1 if self.n_frames is None else self.n_frames)
+
+    @property
     def points(self):
         return self._points
 
+    def get_geometry(self):
+        raise NotImplementedError
+
     @points.setter
     def points(self, points):
         if self._points is not None and points.shape != self._points.shape:
             raise ValueError(f"Can't change number of points: was {self._points.shape=}, got {self.points.shape=}")
         self._points = points
         self.update_points()
 
     def update_points(self):
-        raise NotImplementedError
+        if len(self.mesh.vertices) == 0:
+            vertices, edges, faces = self.get_geometry()
+            self.mesh.from_pydata(vertices, edges, faces)
+        elif len(self.mesh.vertices) == len(self._points.reshape(-1, 3)):
+            self.mesh.vertices.foreach_set("co", self._points.reshape(-1))
+        else:
+            raise ValueError(f"Can't change number of vertices,"
+                             f"was {len(self.mesh.vertices)=}, got {self._point.shape=}.")
+
+        if self.n_frames is not None:
+            bu.set_vertex_attribute(
+                self.mesh, bu.Constants.FRAME_INDEX,
+                np.arange(0, self.n_frames)[None].repeat(self.n_points, axis=1).reshape(-1)
+            )
+
+        self.base_object.data = self.mesh
+        self.mesh.update()
 
     @property
     def color(self):
         return self._color
 
     @color.setter
     def color(self, color):
@@ -43,14 +71,34 @@
     def update_color(self):
         if self._color is not None:
             color, _ = self.tile_data(self._color, [[3], [4]], "color")
             bu.set_vertex_colors(self.mesh, color)
             self.color_material = bu.get_vertex_color_material()
             self.mesh.materials.append(self.color_material)
 
+    def tile_data(self, data_array, valid_dims, name=""):
+        """Tile or reshape data_array with shape TxNx(dims), Nx(dims) or (dims) to shape (T*N)x(dims)."""
+        if len(self.dims) != 1:
+            raise NotImplementedError("Only 1D data can be tiled with base class.")
+
+        match data_array.shape:
+            case (self.n_frames, self.n_points, *dims) if dims in valid_dims:
+                out_array = data_array.reshape(self.n_vertices, *dims)
+            case (self.n_points, *dims) if dims in valid_dims:
+                if self.n_frames is not None:
+                    out_array = np.tile(data_array, (self.n_frames, *([1] * len(dims))))
+                else:
+                    out_array = data_array
+            case (*dims, ) if dims in valid_dims:
+                out_array = np.tile(data_array, (self.n_vertices, *([1]*len(dims))))
+            case _:
+                raise ValueError(
+                    f"Invalid {name} data shape: {data_array.shape} with {self.n_frames=}, {self.n_points=}")
+        return out_array, dims
+
 
 def get_points_array(x, y, z, n_dims=1):
     """Parses x,y,z to a N1xN2x...xN{n_dims}x3 or TxN1xN2x...xN{n_dims}x3 array of points."""
     if (y is None) and (z is None):
         # only x provided, parse it as Nx3 or TxNx3
         x = np.array(x)
         match x.shape:
```

## blender_plots/scatter.py

```diff
@@ -1,27 +1,31 @@
+from dataclasses import dataclass
 import numpy as np
 import numbers
 
 import bpy
 import mathutils as mu
 import blender_plots.blender_utils as bu
 from blender_plots import plots_base
 
-FRAME_INDEX = "frame_index"
-MARKER_ROTATION = "marker_rotation"
-MARKER_TYPES = {
-    "cones": "GeometryNodeMeshCone",
-    "cubes": "GeometryNodeMeshCube",
-    "cylinders": "GeometryNodeMeshCylinder",
-    "grids": "GeometryNodeMeshGrid",
-    "ico_spheres": "GeometryNodeMeshIcoSphere",
-    "circles": "GeometryNodeMeshCircle",
-    "lines": "GeometryNodeMeshLine",
-    "uv_spheres": "GeometryNodeMeshUVSphere",
-}
+
+
+@dataclass
+class Constants:
+    MARKER_ROTATION = "marker_rotation"
+    MARKER_TYPES = {
+        "cones": "GeometryNodeMeshCone",
+        "cubes": "GeometryNodeMeshCube",
+        "cylinders": "GeometryNodeMeshCylinder",
+        "grids": "GeometryNodeMeshGrid",
+        "ico_spheres": "GeometryNodeMeshIcoSphere",
+        "circles": "GeometryNodeMeshCircle",
+        "lines": "GeometryNodeMeshLine",
+        "uv_spheres": "GeometryNodeMeshUVSphere",
+    }
 
 
 class Scatter(plots_base.Plot):
     """Create a scatterplot.
 
     Args:
         x,y,z:
@@ -39,47 +43,30 @@
         marker_kwargs: additional arguments for configuring markers
     """
 
     def __init__(self, x, y=None, z=None, color=None, name="scatter", marker_type="cubes", marker_scale=None,
                  marker_rotation=None, randomize_rotation=False, **marker_kwargs):
         super(Scatter, self).__init__(x, y, z, color=color, name=name, n_dims=1)
 
-        self.marker_modifier = self.base_object.modifiers.new(type="NODES", name="spheres")
         if marker_type == "spheres":
-            add_sphere_markers(self.marker_modifier, n_frames=self.n_frames, **marker_kwargs)
+            add_sphere_markers(self.modifier, n_frames=self.n_frames, **marker_kwargs)
         elif marker_type is not None:
             add_mesh_markers(
-                self.marker_modifier,
+                self.modifier,
                 randomize_rotation=randomize_rotation,
                 marker_type=marker_type,
                 marker_scale=marker_scale,
                 n_frames=self.n_frames,
                 **marker_kwargs
             )
-        self.marker_modifier["Input_2"] = self.color_material
+        self.modifier["Input_2"] = self.color_material
         self.marker_rotation = marker_rotation
 
-    @property
-    def n_points(self):
-        return self.dims[0]
-
-    def update_points(self):
-        if len(self.mesh.vertices) == 0:
-            self.mesh.from_pydata(self._points.reshape(-1, 3), [], [])
-        elif len(self.mesh.vertices) == len(self._points):
-            self.mesh.vertices.foreach_set("co", self._points.reshape(-1))
-
-        if self.n_frames is not None:
-            bu.set_vertex_attribute(
-                self.mesh, FRAME_INDEX,
-                np.arange(0, self.n_frames)[None].repeat(self.n_points, axis=1).reshape(-1)
-            )
-
-        self.base_object.data = self.mesh
-        self.mesh.update()
+    def get_geometry(self):
+        return self._points.reshape(-1, 3), [], []
 
     @property
     def marker_rotation(self):
         return self._marker_rotation
 
     @marker_rotation.setter
     def marker_rotation(self, marker_rotation):
@@ -87,33 +74,15 @@
         self.update_marker_rotation()
 
     def update_marker_rotation(self):
         if self._marker_rotation is not None:
             marker_rotation, rotation_dims = self.tile_data(self._marker_rotation, [[3], [3, 3]], "marker rotation")
             if rotation_dims == [3, 3]:
                 marker_rotation = np.stack([np.array(mu.Matrix(r).to_euler()) for r in marker_rotation])
-            bu.set_vertex_attribute(self.mesh, MARKER_ROTATION, marker_rotation, "FLOAT_VECTOR")
-
-    def tile_data(self, data_array, valid_dims, name=""):
-        """Tile or reshape data_array with shape NxTx(dims), Nx(dims) or (dims) to shape (N*T)x(dims)."""
-        match data_array.shape:
-            case (self.n_frames, self.n_points, *dims) if dims in valid_dims:
-                out_array = data_array.reshape(self.n_frames * self.n_points, *dims)
-            case (self.n_points, *dims) if dims in valid_dims:
-                if self.n_frames is not None:
-                    out_array = np.tile(data_array, (self.n_frames, *([1] * len(dims))))
-                else:
-                    out_array = data_array
-            case (*dims, ) if dims in valid_dims:
-                n_points_total = self.n_points * (1 if self.n_frames is None else self.n_frames)
-                out_array = np.tile(data_array, (n_points_total, *([1]*len(dims))))
-            case _:
-                raise ValueError(
-                    f"Invalid {name} data shape: {data_array.shape} with {self.n_frames=}, {self.n_points=}")
-        return out_array, dims
+            bu.set_vertex_attribute(self.mesh, Constants.MARKER_ROTATION, marker_rotation, "FLOAT_VECTOR")
 
 
 def add_mesh_markers(base_modifier, marker_type, randomize_rotation=False, marker_scale=None,
                      n_frames=0, **marker_kwargs):
     """Create a geometry node modifier that instances a mesh on each vertex.
     Args:
         base_modifier: modifier to add markers to.
@@ -133,49 +102,49 @@
     base_modifier.node_group.inputs.new("NodeSocketObject", "Point Instance")  # Input_3
 
     points_socket = node_linker.new_node(
         "GeometryNodeMeshToPoints",
         mesh=node_linker.group_input.outputs["Geometry"]
     ).outputs["Points"]
 
-    if marker_type in MARKER_TYPES:
-        mesh_socket = node_linker.new_node(node_type=MARKER_TYPES[marker_type], **marker_kwargs).outputs["Mesh"]
+    if marker_type in Constants.MARKER_TYPES:
+        mesh_socket = node_linker.new_node(node_type=Constants.MARKER_TYPES[marker_type], **marker_kwargs).outputs["Mesh"]
     elif isinstance(marker_type, bpy.types.Mesh) or isinstance(marker_type, bpy.types.Object):
         # use the supplied mesh by adding it as an input socket to the base_modifier
         base_modifier["Input_3"] = marker_type
         base_modifier.show_viewport = False
         base_modifier.show_viewport = True
         mesh_socket = node_linker.new_node(
             "GeometryNodeObjectInfo",
             Object=node_linker.group_input.outputs["Point Instance"]
         ).outputs["Geometry"]
         marker_type.hide_viewport = True
         marker_type.hide_render = True
     else:
         raise TypeError(f"Invalid marker type: {marker_type}, expected bpy.types.Mesh, bpy.Types.Object, "
-                        f"or one of: {', '.join(MARKER_TYPES)}")
+                        f"or one of: {', '.join(Constants.MARKER_TYPES)}")
 
     colored_mesh = node_linker.new_node(
         "GeometryNodeSetMaterial",
         geometry=mesh_socket,
         material=node_linker.group_input.outputs["Point Color"]
     ).outputs["Geometry"]
 
     if marker_scale is not None and np.array(marker_scale).shape == ():
         marker_scale = [marker_scale] * 3
 
     marker_rotation = node_linker.new_node(
         "GeometryNodeInputNamedAttribute",
         data_type="FLOAT_VECTOR",
-        name=MARKER_ROTATION,
+        name=Constants.MARKER_ROTATION,
     )
     instance_on_points_node = node_linker.new_node(
         "GeometryNodeInstanceOnPoints",
         points=points_socket,
-        selection=None if n_frames is None else get_frame_selection_node(base_modifier, n_frames).outputs["Value"],
+        selection=None if n_frames is None else bu.get_frame_selection_node(base_modifier, n_frames).outputs["Value"],
         instance=colored_mesh,
         rotation=marker_rotation.outputs["Attribute"],
         scale=marker_scale,
     )
     if randomize_rotation:
         # these rotation are not uniform (some orientations will be more likely than others)
         # but it usually looks decent
@@ -203,43 +172,16 @@
     node_linker = bu.NodeLinker(base_modifier.node_group)
 
     base_modifier.node_group.inputs.new("NodeSocketMaterial", "Point Color")  # Input_2
 
     points = node_linker.new_node(
         "GeometryNodeMeshToPoints",
         mesh=node_linker.group_input.outputs["Geometry"],
-        selection=None if n_frames is None else get_frame_selection_node(base_modifier, n_frames).outputs["Value"],
+        selection=None if n_frames is None else bu.get_frame_selection_node(base_modifier, n_frames).outputs["Value"],
         **marker_kwargs,
     ).outputs["Points"]
     node = node_linker.new_node(
         "GeometryNodeSetMaterial",
         geometry=points,
         material=node_linker.group_input.outputs["Point Color"]
     )
     node_linker.new_node("NodeGroupOutput", geometry=node.outputs["Geometry"])
-
-
-def get_frame_selection_node(modifier, n_frames):
-    """Add node that filters points based on the Frame Index property."""
-    node_linker = bu.NodeLinker(modifier.node_group)
-    frame_index = node_linker.new_node(
-        "GeometryNodeInputNamedAttribute",
-        data_type="FLOAT",
-        name=FRAME_INDEX,
-    )
-    frame_selection_node = node_linker.new_node(
-        "ShaderNodeMath",
-        operation="COMPARE",
-        input_1=frame_index.outputs[1],
-        input_2=0.5
-    )
-
-    action = bpy.data.actions.new("AnimationAction")
-    fcurve = action.fcurves.new(data_path='nodes["Math"].inputs[0].default_value', index=0)
-    fcurve.keyframe_points.add(2)
-    fcurve.keyframe_points.foreach_set("co", [0, 0, n_frames, n_frames])
-    bpy.context.scene.frame_end = n_frames - 1
-
-    modifier.node_group.animation_data_create()
-    modifier.node_group.animation_data.action = action
-
-    return frame_selection_node
```

## blender_plots/surface.py

```diff
@@ -1,47 +1,74 @@
 import numpy as np
 
 import bpy
+from blender_plots import plots_base
+from blender_plots import blender_utils as bu
 
 
-"""Create a scatterplot.
-
-Args:
-    x,y,z:
-        If y and z are not provided: expects x to be a Nx3 array with xyz positions for points to scatter, or TxNx3
-            for sequence of scatter plots to animate
-        if y and z are provided: expects x,y,z to be length N or TxN arrays for xyz coordinates respectively.
-    color: Nx3 or Nx4 array or with RGB or RGBA values for each point, or a single RGB/RGBA-value
-        (e.g. (1, 0, 0) for red) to apply to every point.
-    name: name to use for blender object. Will delete any previous plot with the same name.
-    marker_type: select appearance of points. Either MARKER_TYPE, "spheres", bpy_types.Mesh or bpy_types.Object
-    marker_scale: xyz scale for markers
-    marker_rotation: Nx3 (euler angles in radians) or Nx3x3 (rotation matrices) array specifying the rotation for
-        each marker. Or "random" for applying a random rotation to each marker.
-    randomize_rotation: If set to True randomize the rotation of each marker. Overrides marker_rotation.
-    marker_kwargs: additional arguments for configuring markers
-"""
-
-class Surface:
+class Surface(plots_base.Plot):
     """Create a surface plot.
-    Args:
-        x, y, z:
 
+    Args:
+        x,y,z:
+            If y and z are not provided: expects x to be a MxNx3 array with xyz positions for points to plot as a surface, or TxMxNx3 for sequence of to animate
+            if y and z are provided: expects x,y,z to have shapes MxN or TxMxN arrays for xyz coordinates respectively.
+        color: MxNx3 or MxNx4 array or with RGB or RGBA values for each point, or a single RGB/RGBA-value (e.g. (1, 0, 0) for red) to apply to every point.
+        name: name to use for blender object. Will delete any previous plot with the same name.
     """
 
-    def __init__(self, x, y, z, color=None, name="surface"):
-        pass
+    def __init__(self, x, y=None, z=None, color=None, name="surface"):
+        super(Surface, self).__init__(x, y, z, color=color, name=name, n_dims=2)
+        if self.n_frames is not None:
+            animate(self.modifier, self.n_frames)
 
     @property
-    def points(self):
-        return self._points
-    
-    @points.setter
-    def points(self, points):
-        self._points = points
-        self.update_points()
-
-    def update_points(self):
-        pass
-
+    def n_points_x(self):
+        return self.dims[0]
     
+    @property
+    def n_points_y(self):
+        return self.dims[1]
 
+    def get_geometry(self):
+        faces = get_faces(self.n_points_x, self.n_points_y, 1 if self.n_frames is None else self.n_frames)
+        return self._points.reshape(-1, 3), [], faces.reshape(-1, 4)
+
+    def tile_data(self, data_array, valid_dims, name=""):
+        """Tile or reshape data_array with shape TxMxNx(dims), MxNx(dims) or (dims) to shape (T*M*N)x(dims)."""
+        match data_array.shape:
+            case (self.n_frames, self.n_points_x, self.n_points_y, *dims) if dims in valid_dims:
+                out_array = data_array.reshape(self.n_frames * self.n_points, *dims)
+            case (self.n_points_x, self.n_points_y, *dims) if dims in valid_dims:
+                if self.n_frames is not None:
+                    out_array = np.tile(data_array.reshape(-1, *dims), (self.n_frames, *([1] * len(dims))))
+                else:
+                    out_array = data_array.reshape(self.n_vertices, *dims)
+            case (*dims, ) if dims in valid_dims:
+                out_array = np.tile(data_array, (self.n_vertices, *([1]*len(dims))))
+            case _:
+                raise ValueError(
+                    f"Invalid {name} data shape: {data_array.shape} with {self.n_frames=}, {self.n_points=}")
+        return out_array, dims
+
+
+def get_faces(n_points_x, n_points_y, n_frames):
+    return np.array([
+        [
+            j * n_points_x * n_points_y +  np.array([i, i + 1, i + n_points_x + 1, i + n_points_x])
+            for i in range(n_points_x * (n_points_y - 1))
+            if (i + 1) % n_points_x != 0
+        ]
+        for j in range(n_frames)
+    ])
+
+def animate(base_modifier, n_frames):
+    if base_modifier.node_group is None:
+        base_modifier.node_group = bu.geometry_node_group_empty_new()
+    node_linker = bu.NodeLinker(base_modifier.node_group)
+
+    visible_geometry = node_linker.new_node(
+        "GeometryNodeSeparateGeometry",
+        geometry=node_linker.group_input.outputs["Geometry"],
+        selection=bu.get_frame_selection_node(base_modifier, n_frames).outputs["Value"]
+    ).outputs["Selection"]
+    node_linker.new_node("NodeGroupOutput", geometry=visible_geometry)
```

## Comparing `blender_plots-1.0.1.dist-info/LICENSE` & `blender_plots-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `blender_plots-1.0.1.dist-info/RECORD` & `blender_plots-1.0.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-blender_plots/__init__.py,sha256=ikNhgX5Qc3Ytskl_aaEXRbfzeKp7d8GzQ-qhKzuRKdg,78
-blender_plots/blender_utils.py,sha256=_w5ZG3_YGiu5tiKliamBFJ_qK-zhW2ef1c-wQzEdt2g,6142
-blender_plots/plots_base.py,sha256=p4kUCxxChNWrGBLxagq77ZsqCKOxKbM8W2fv5aFmHtQ,3354
-blender_plots/scatter.py,sha256=s1jGQItjAHfDx4iu0oWW3lBPuiZNwPKTPO5KzUWH4N0,11103
-blender_plots/surface.py,sha256=-4906S46IBSBinUxdQ_jkEhGqmsirgZEIf1r3Ty4OaM,1507
-blender_plots-1.0.1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-blender_plots-1.0.1.dist-info/METADATA,sha256=O87953_1StsXE8AAqCqQk4zQUDRYkYsMA3ZRZlklcLI,224
-blender_plots-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-blender_plots-1.0.1.dist-info/top_level.txt,sha256=oowZPkZ4AWwTOxmOvDkA6f6em7A3oc50eUX-4_vOgWo,14
-blender_plots-1.0.1.dist-info/RECORD,,
+blender_plots/__init__.py,sha256=cMFUzb9dxJW8lUYzSfZS2a4-p0ObB4KgKXWeAddA0iU,210
+blender_plots/blender_utils.py,sha256=V_75qWo953IooS_MBAGqInOCNcJziMNpuq77lnvSQFc,7273
+blender_plots/plots_base.py,sha256=JNURhUGWZ7NCLiymWbQ9ioboPX8OKSS4_0wStsizDfM,5492
+blender_plots/scatter.py,sha256=M6Jk03KkPPo9tEWFqvphjBZDeibPOV3aJr78LzuFMCw,8594
+blender_plots/surface.py,sha256=YKziR0VPPEr4Z22zYjTzbeM8I4IWmY9QEhuBswRS_no,3255
+blender_plots-1.0.2.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+blender_plots-1.0.2.dist-info/METADATA,sha256=8DZ_IfLITFg40HkFrJsVXjK00iyQuVEngDXJKTiA8Qw,224
+blender_plots-1.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+blender_plots-1.0.2.dist-info/top_level.txt,sha256=oowZPkZ4AWwTOxmOvDkA6f6em7A3oc50eUX-4_vOgWo,14
+blender_plots-1.0.2.dist-info/RECORD,,
```

