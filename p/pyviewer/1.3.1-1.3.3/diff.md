# Comparing `tmp/pyviewer-1.3.1.tar.gz` & `tmp/pyviewer-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyviewer-1.3.1.tar", last modified: Wed Feb  1 06:24:04 2023, max compression
+gzip compressed data, was "pyviewer-1.3.3.tar", last modified: Tue Apr 25 04:55:05 2023, max compression
```

## Comparing `pyviewer-1.3.1.tar` & `pyviewer-1.3.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 06:24:04.298176 pyviewer-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-02-01 06:23:52.000000 pyviewer-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-02-01 06:24:04.298176 pyviewer-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-02-01 06:23:52.000000 pyviewer-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 06:24:04.294175 pyviewer-1.3.1/pyviewer/
--rw-r--r--   0 runner    (1001) docker     (123)  3423528 2023-02-01 06:23:52.000000 pyviewer-1.3.1/pyviewer/MPLUSRounded1c-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-02-01 06:23:52.000000 pyviewer-1.3.1/pyviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-01 06:23:52.000000 pyviewer-1.3.1/pyviewer/easy_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    24774 2023-02-01 06:23:52.000000 pyviewer-1.3.1/pyviewer/gl_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24300 2023-02-01 06:23:52.000000 pyviewer-1.3.1/pyviewer/imgui_themes.py
--rw-r--r--   0 runner    (1001) docker     (123)    71936 2023-02-01 06:23:52.000000 pyviewer-1.3.1/pyviewer/roboto_mono.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-02-01 06:23:52.000000 pyviewer-1.3.1/pyviewer/single_image_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-02-01 06:23:52.000000 pyviewer-1.3.1/pyviewer/toolbar_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-02-01 06:23:52.000000 pyviewer-1.3.1/pyviewer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 06:24:04.298176 pyviewer-1.3.1/pyviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-02-01 06:24:04.000000 pyviewer-1.3.1/pyviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-02-01 06:24:04.000000 pyviewer-1.3.1/pyviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 06:24:04.000000 pyviewer-1.3.1/pyviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-01 06:24:04.000000 pyviewer-1.3.1/pyviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-01 06:24:04.000000 pyviewer-1.3.1/pyviewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-01 06:24:04.298176 pyviewer-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-02-01 06:23:52.000000 pyviewer-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:55:05.646079 pyviewer-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-04-25 04:54:54.000000 pyviewer-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-25 04:55:05.646079 pyviewer-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-25 04:54:54.000000 pyviewer-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:55:05.646079 pyviewer-1.3.3/pyviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)  3423528 2023-04-25 04:54:54.000000 pyviewer-1.3.3/pyviewer/MPLUSRounded1c-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-25 04:54:54.000000 pyviewer-1.3.3/pyviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-25 04:54:54.000000 pyviewer-1.3.3/pyviewer/easy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24774 2023-04-25 04:54:54.000000 pyviewer-1.3.3/pyviewer/gl_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24300 2023-04-25 04:54:54.000000 pyviewer-1.3.3/pyviewer/imgui_themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-25 04:54:54.000000 pyviewer-1.3.3/pyviewer/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71936 2023-04-25 04:54:54.000000 pyviewer-1.3.3/pyviewer/roboto_mono.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-04-25 04:54:54.000000 pyviewer-1.3.3/pyviewer/single_image_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-04-25 04:54:54.000000 pyviewer-1.3.3/pyviewer/toolbar_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19702 2023-04-25 04:54:54.000000 pyviewer-1.3.3/pyviewer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:55:05.646079 pyviewer-1.3.3/pyviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-25 04:55:05.000000 pyviewer-1.3.3/pyviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-25 04:55:05.000000 pyviewer-1.3.3/pyviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 04:55:05.000000 pyviewer-1.3.3/pyviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-25 04:55:05.000000 pyviewer-1.3.3/pyviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 04:55:05.000000 pyviewer-1.3.3/pyviewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 04:55:05.646079 pyviewer-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-25 04:54:54.000000 pyviewer-1.3.3/setup.py
```

### Comparing `pyviewer-1.3.1/LICENSE` & `pyviewer-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.1/PKG-INFO` & `pyviewer-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviewer
-Version: 1.3.1
+Version: 1.3.3
 Summary: Interactyive python viewers
 Home-page: https://github.com/harskish/pyviewer
 Author: Erik Härkönen
 Author-email: erik.harkonen@hotmail.com
 License: CC BY-NC-SA 4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyviewer-1.3.1/README.md` & `pyviewer-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.1/pyviewer/MPLUSRounded1c-Medium.ttf` & `pyviewer-1.3.3/pyviewer/MPLUSRounded1c-Medium.ttf`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.1/pyviewer/gl_viewer.py` & `pyviewer-1.3.3/pyviewer/gl_viewer.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.1/pyviewer/imgui_themes.py` & `pyviewer-1.3.3/pyviewer/imgui_themes.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.1/pyviewer/roboto_mono.ttf` & `pyviewer-1.3.3/pyviewer/roboto_mono.ttf`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.1/pyviewer/single_image_viewer.py` & `pyviewer-1.3.3/pyviewer/single_image_viewer.py`

 * *Files 5% similar despite different names*

```diff
@@ -198,20 +198,20 @@
         begin_inline('Output')
         
         # Draw provided image
         if self.pan_enabled.value:
             tex_in = v._images.get(self.key)
             if tex_in:
                 tex_H, tex_W, _ = tex_in.shape
-                cW, cH = [r-l for l,r in zip(
+                cW, cH = [int(r-l) for l,r in zip(
                     imgui.get_window_content_region_min(), imgui.get_window_content_region_max())]
                 scale = min(cW / tex_W, cH / tex_H)
                 out_res = (int(tex_W*scale), int(tex_H*scale))
-                tex = v.pan_handler.draw_to_canvas(tex_in.tex, *out_res)
-                imgui.image(tex, *out_res)
+                tex = v.pan_handler.draw_to_canvas(tex_in.tex, *out_res, cW, cH)
+                imgui.image(tex, cW, cH)
         else:
             v.draw_image(self.key, width='fit')
 
         if self.paused.value:
             imgui.push_font(v._imgui_fonts[30])
             dl = imgui.get_window_draw_list()
             dl.add_rect_filled(5, 8, 115, 43, imgui.get_color_u32_rgba(0,0,0,1))
@@ -249,16 +249,17 @@
         message="'pyviewer.single_image_viewer' found in sys.modules.*")
 
 # Single global instance
 # Removes need to pass variable around in code
 # Just call draw() (optionally call init first)
 inst: SingleImageViewer = None
 
-def init(*args, **kwargs):
+def init(*args, sync=True, **kwargs):
     global inst
     if inst is None:
         inst = SingleImageViewer(*args, **kwargs)
-        inst.wait_for_startup()
+        if sync:
+            inst.wait_for_startup() # if calling from debugger: need to give process time to start
 
 def draw(*, img_hwc=None, img_chw=None, ignore_pause=False):
     init('SIV') # no-op if init already performed
     inst.draw(img_hwc, img_chw, ignore_pause)
```

### Comparing `pyviewer-1.3.1/pyviewer/toolbar_viewer.py` & `pyviewer-1.3.3/pyviewer/toolbar_viewer.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,36 +5,43 @@
 import string
 import numpy as np
 import time
 
 from . import gl_viewer
 from .utils import imgui_item_width, begin_inline, PannableArea
 from .easy_dict import EasyDict
+from .params import ParamContainer, Param
 
 #----------------------------------------------------------------------------
 # Helper class for UIs with toolbar on the left and output image on the right
 
 class ToolbarViewer:
     def __init__(self, name, pad_bottom=0, hidden=False, batch_mode=False):
         self.output_key = ''.join(random.choices(string.ascii_letters, k=20))
         self.pad_bottom = pad_bottom
         self.v = gl_viewer.viewer(name, hidden=hidden or batch_mode, swap_interval=1)
         self.menu_bar_height = 0
         self.toolbar_width = 300
+        # Size of latest image data in texels, (C, H, W)
         self.img_shape = [3, 4, 4]
+        # Position of drawn imgui.image element,
+        # relative to glfw window top-left
         self.output_pos_tl = np.zeros(2, dtype=np.float32)
         self.output_pos_br = np.zeros(2, dtype=np.float32)
+        # Size in pixels of drawn imgui.image, (W, H)
+        self.content_size_px = (1, 1)
+        # Size of available canvas
         self.output_area_tl = np.zeros(2, dtype=np.float32)
         self.output_area_br = np.zeros(2, dtype=np.float32)
-        self.content_size_px = (1, 1) # actual current content size
         self.ui_locked = True
         self.state = EasyDict()
 
         # Support image zoom and pan
         self.pan_handler = PannableArea()
+        self.pan_handler.clear_color = (0.101, 0.101, 0.101, 1.00) # match theme_deep_dark
         self.pan_enabled = True
         
         # User-provided
         self.setup_state()
 
         # User nearest interpolation for sharpness by default
         self.v.set_interp_nearest()
@@ -99,32 +106,41 @@
         imgui.set_next_window_size(W - self.toolbar_width, H - self.menu_bar_height)
         imgui.set_next_window_position(self.toolbar_width, self.menu_bar_height)
 
         s = v.ui_scale
 
         begin_inline('Output')
         BOTTOM_PAD = max(self.pad_bottom, int(round(20 * s)) + 6) # extra user content below image
+        
+        # Calculate size of current (virtual) imgui.window
         rmin, rmax = imgui.get_window_content_region_min(), imgui.get_window_content_region_max()
         cW, cH = [int(r-l) for l,r in zip(rmin, rmax)]
+        
+        # Compute size of image that fills smaller dimension
+        # Bottom area for integer scaling buttons taken into account
         aspect = self.img_shape[2] / self.img_shape[1]
-        out_size = min(cW, aspect*(cH - BOTTOM_PAD))
-        self.content_size_px = (int(out_size), int(out_size / aspect))
+        out_width = min(cW, aspect*(cH - BOTTOM_PAD))
+        self.content_size_px = (int(out_width), int(out_width / aspect))
         
-        # Draw provided image
+        # Create imgui.image from provided data
         if self.pan_enabled:
             tex_in = v._images.get(self.output_key)
             if tex_in:
-                tex = self.pan_handler.draw_to_canvas(tex_in.tex, *self.content_size_px)
-                imgui.image(tex, *self.content_size_px)
+                canvas_size = (cW, cH - BOTTOM_PAD)
+                tex = self.pan_handler.draw_to_canvas(tex_in.tex, *self.content_size_px, *canvas_size)
+                imgui.image(tex, *canvas_size)
         else:
-            v.draw_image(self.output_key, width=out_size)
+            v.draw_image(self.output_key, width=out_width)
 
-        # Potential space for content
+        # Imgui.image drawn above
+        # => get position where it was drawn
         self.output_pos_tl[:] = imgui.get_item_rect_min()
         self.output_pos_br[:] = imgui.get_item_rect_max()
+        
+        # Record maximum available canvas size
         self.output_area_tl[:] = self.output_pos_tl
         self.output_area_br[:] = np.array(rmax) - np.array([0, BOTTOM_PAD])
 
         # Equal spacing
         imgui.columns(2, 'outputBottom', border=False)
 
         # Extra UI elements below output
@@ -187,17 +203,22 @@
         _, H = glfw.get_window_size(v._window)
         self.toolbar_width = 350 * v.ui_scale
         imgui.set_next_window_size(self.toolbar_width, H - self.menu_bar_height)
         imgui.set_next_window_position(0, self.menu_bar_height)
 
         # User callback
         begin_inline('toolbar')
+        self.draw_toolbar_autoUI()
         self.draw_toolbar()
         imgui.end()
 
+    # Only used by AutoUIViewer
+    def draw_toolbar_autoUI(self):
+        pass
+
     def mouse_over_image(self):
         x, y = self.mouse_pos_img_norm
         return (0 <= x <= 1) and (0 <= y <= 1)
 
     def mouse_over_content(self):
         x, y = self.mouse_pos_content_norm
         return (0 <= x <= 1) and (0 <= y <= 1)
@@ -206,15 +227,15 @@
     # (e.g. in callbacks or from UI thread)
     def update_image(self, img_hwc):
         H, W = img_hwc.shape[0:2]
         C = 1 if img_hwc.ndim == 2 else img_hwc.shape[-1]
         self.img_shape = [C, H, W]
         self.v.upload_image(self.output_key, img_hwc)
     
-    #-----------------------------------------------------------------------------------
+    #------------------------
     # User-provided functions
 
     # Draw toolbar, must be implemented
     def draw_toolbar(self):
         pass
 
     # Draw extra UI elements below output image
@@ -235,15 +256,33 @@
         pass
 
     # GLFW callbacks
     def setup_callbacks(self, window):
         pass
 
 
-#-----------------------------------------------------------------------------
+#----------------------------------------------
+# Version that creates UI widgets automatically
+
+class AutoUIViewer(ToolbarViewer):
+    def draw_toolbar_autoUI(self):
+        if not isinstance(self.state, ParamContainer):
+            return
+
+        for _, p in self.state:
+            if isinstance(p, Param):
+                p.draw()
+        
+        # Draw below widgets
+        if imgui.button('Reset'):
+            for _, p in self.state:
+                if isinstance(p, Param):
+                    p.reset()
+
+#--------------
 # Example usage
 
 def main():
     import numpy as np
     
     class Test(ToolbarViewer):
         def setup_state(self):
```

### Comparing `pyviewer-1.3.1/pyviewer/utils.py` & `pyviewer-1.3.3/pyviewer/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         self.output_pos_tl = np.zeros(2, dtype=np.float32)
         self.id = ''.join(random.choices(string.ascii_letters, k=20))
         self.is_panning = False
         self.pan = (0, 0)
         self.pan_start = (0, 0)
         self.pan_delta = (0, 0)
         self.zoom: float = 1.0
+        self.clear_color = (0, 0, 0, 1) # in [0, 1]
 
         # Canvas onto which resmapled image is drawn
         self.canvas_tex = None
         self.canvas_fb = None
         self.canvas_w = 0
         self.canvas_h = 0
 
@@ -153,44 +154,53 @@
             +1, +1, 1, 0,      #  | /  |        | SPACE |           |    |
             +1, -1, 1, 1,      #  2----4        +-------+           +----+
         ], dtype=np.float32)   #           (-1, -1)   (+1, -1)   (0,1)  (1,1)
 
         gl.glBindBuffer(gl.GL_ARRAY_BUFFER, self._vbo_handle)
         gl.glBufferData(gl.GL_ARRAY_BUFFER, 4 * vertex_size, vertices, gl.GL_STATIC_DRAW)
 
-    def draw_to_canvas(self, texture_in, W, H):
+    # iW, iH = image size
+    # cW, cH = canvas size
+    def draw_to_canvas(self, texture_in, iW, iH, cW, cH):
         last_texture = gl.glGetIntegerv(gl.GL_TEXTURE_BINDING_2D)
         last_array_buffer = gl.glGetIntegerv(gl.GL_ARRAY_BUFFER_BINDING)
         last_vertex_array = gl.glGetIntegerv(gl.GL_VERTEX_ARRAY_BINDING)
         last_framebuffer = gl.glGetInteger(gl.GL_FRAMEBUFFER_BINDING)
         last_clear_color = gl.glGetFloatv(gl.GL_COLOR_CLEAR_VALUE)
         last_viewport = gl.glGetIntegerv(gl.GL_VIEWPORT)
 
         if self.canvas_fb is None:
-            self.init_gl(W, H)
+            self.init_gl(cW, cH)
 
         # Reallocate if window size has changed
-        self.resize_canvas(W, H)
+        self.resize_canvas(cW, cH)
 
         # Keep track of content position
         self.output_pos_tl[:] = imgui.get_item_rect_min()
 
         # Update pan & zoom state
         self.handle_pan()
 
         #gl.glDisable(gl.GL_BLEND)
         gl.glDisable(gl.GL_CULL_FACE)
         gl.glDisable(gl.GL_DEPTH_TEST)
         gl.glDisable(gl.GL_SCISSOR_TEST)
         gl.glActiveTexture(gl.GL_TEXTURE0)
-        gl.glClearColor(0, 0, 0, 1)
+        gl.glClearColor(*self.clear_color)
 
-        xform = self.get_transform(1, 1)
+        # Get current pan/zoom xform
+        xform = self.get_transform_ndc()
         xform[1, 1] *= -1  # flip y
-        xform[0:2, 2] *= 2 # adapt to larger [-1, 1] NDC range
+
+        # Image size is computed to fill smaller canvas dimension
+        # Account for this scaling to prevent image stretching
+        scale = np.diag([iW/cW, iH/cH, 1])
+        xform = xform @ scale
+        
+        # GL expects [..., tX, tY, 1]
         xform = np.transpose(xform)
 
         gl.glUseProgram(self._shader_handle)
         gl.glUniform1i(self._attrib_location_tex, 0) # slot 0
         gl.glUniformMatrix3fv(self._attrib_location_xform, 1, gl.GL_FALSE, xform)
         gl.glBindVertexArray(self._vao_handle)
         gl.glBindFramebuffer(gl.GL_FRAMEBUFFER, self.canvas_fb)
@@ -209,32 +219,71 @@
         gl.glClearColor(*last_clear_color)
         gl.glViewport(*last_viewport)
 
         return self.canvas_tex
 
     def set_callbacks(self, glfw_window):
         self.prev_cbk = glfw.set_scroll_callback(glfw_window, self.mouse_wheel_callback)
-
-    def get_transform(self, W, H):        
+    
+    def get_transform_ndc(self):
+        """
+        Get current image transform.
+        Should be applied to coordinates in [-1, 1] (NDC space)
+        """
         M = np.eye(3, dtype=np.float32)
-        M[0, 2] += (self.pan[0]+self.pan_delta[0])*W
-        M[1, 2] += (self.pan[1]+self.pan_delta[1])*H
+        M[0, 2] += (self.pan[0]+self.pan_delta[0])*2
+        M[1, 2] += (self.pan[1]+self.pan_delta[1])*2
         M = np.diag((self.zoom, self.zoom, 1)) @ M
         return M
+    
+    def get_transform_scaled(self, W, H):
+        """
+        Get current image transform.
+        Should be applied to coordinates in [0, W]x[0, H]
+        """
+        M = self.get_transform_ndc()
+
+        # NDC to absolute (inputs in [O,W]x[0,H])
+        S = np.array([
+            W/2,   0, W/2,
+              0, H/2, H/2,
+              0,   0,   1,
+        ]).astype(np.float32).reshape(3, 3)
+        M = S @ M @ np.linalg.inv(S)
+
+        return M
+    
+    def get_transform(self):
+        """
+        Get current image transform.
+        Should be applied to coordinates in [0, 1]
+        """
+        return self.get_transform_scaled(1, 1)
+    
+    # Set transform state from np matrix
+    # Assuming M contains only zoom & translation
+    def set_transform(self, M, W=1, H=1):
+        #assert not self.is_panning
+        assert M.shape == (3, 3)
+        self.zoom = np.sqrt(M[0, 0] * M[1, 1])
+        self.pan = (
+            M[0, 2] / W / self.zoom,
+            M[1, 2] / H / self.zoom,
+        )
 
     # Handle pan action
     def handle_pan(self):
         xy = np.array(self.mouse_pos_img_norm)
         
         # Figure out what part of image is currently visible
         box = np.array([
             0.0, 0.0, 1.0,
             1.0, 1.0, 1.0,
         ]).reshape(1, 2, 3)
-        M = np.linalg.inv(self.get_transform(1, 1))
+        M = np.linalg.inv(self.get_transform())
         box = (box @ M)[0, 0:2, 0:2]
         a, b = (box[0] * (1 - xy) + box[1] * xy).tolist()
 
         if imgui.is_mouse_clicked(0) and self.mouse_hovers_content():
             self.is_panning = True
             self.pan_start = (a, b)
         if self.is_panning and imgui.is_mouse_down(0):
@@ -317,39 +366,47 @@
     head = obj
     while '.' in key:
         bot, key = key.split('.', maxsplit=1)
         head = getattr(head, bot, {})
     return getattr(head, key, default)
 
 # Combo box that returns value, not index
-def combo_box_vals(title, values, current, height_in_items=-1, to_str=str):
+def combo_box_vals(title, values, current, height_in_items=-1, to_str: callable = str):
     values = list(values)
     curr_idx = 0 if current not in values else values.index(current)
     changed, ind = imgui.combo(title, curr_idx, [to_str(v) for v in values], height_in_items)
     return changed, values[ind]
 
+# Slider that cycles through predefined values
+# Abusing format to draw current enum value onto slider
+def enum_slider(title, values, current, to_str: callable = str):
+    values = list(values)
+    curr_idx = 0 if current not in values else values.index(current)
+    changed, idx = imgui.slider_int(title, curr_idx, 0, len(values)-1, format=to_str(current))
+    return changed, values[idx]
+
 # Imgui slider that can switch between int and float formatting at runtime
 def slider_dynamic(title, v, min, max, width=0.0):
     scale_fmt = '%.2f' if np.modf(v)[0] > 0 else '%.0f' # dynamically change from ints to floats
     with imgui_item_width(width):
         return imgui.slider_float(title, v, min, max, format=scale_fmt)
 
 # Int2 slider that prevents overlap
-def slider_range(v1, v2, vmin, vmax, push=False, title='', width=0.0):
+def slider_range_int(v1, v2, vmin, vmax, push=False, title='', width=0.0):
     with imgui_item_width(width):
-        s, e = imgui.slider_int2(title, v1, v2, vmin, vmax)[1]
+        ch, (s, e) = imgui.slider_int2(title, v1, v2, vmin, vmax)
 
     if push:
-        return (min(s, e), max(s, e))
+        return ch, (min(s, e), max(s, e))
     elif s != v1:
-        return (min(s, e), e)
+        return ch, (min(s, e), e)
     elif e != v2:
-        return (s, max(s, e))
+        return ch, (s, max(s, e))
     else:
-        return (s, e)
+        return ch, (s, e)
 
 # Shape batch as square if possible
 def get_grid_dims(B):
     if B == 0:
         return (0, 0)
     
     S = int(B**0.5 + 0.5)
```

### Comparing `pyviewer-1.3.1/pyviewer.egg-info/PKG-INFO` & `pyviewer-1.3.3/pyviewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviewer
-Version: 1.3.1
+Version: 1.3.3
 Summary: Interactyive python viewers
 Home-page: https://github.com/harskish/pyviewer
 Author: Erik Härkönen
 Author-email: erik.harkonen@hotmail.com
 License: CC BY-NC-SA 4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyviewer-1.3.1/setup.py` & `pyviewer-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import sys
 if 'develop' in sys.argv:
     print("WARNING: 'python setup.py develop' won't install \
         dependencies correctly, please use 'pip install -e .' instead.")
 
 setup(name='pyviewer',
-    version='1.3.1',
+    version='1.3.3',
     description='Interactyive python viewers',
     author='Erik Härkönen',
     author_email='erik.harkonen@hotmail.com',
     url='https://github.com/harskish/pyviewer',
     packages=['pyviewer'], # name of importable thing
     setup_requires=['wheel'],
     install_requires=[
```

