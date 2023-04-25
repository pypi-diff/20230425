# Comparing `tmp/kivy_widgets-0.1.5.tar.gz` & `tmp/kivy_widgets-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivy_widgets-0.1.5.tar", max compression
+gzip compressed data, was "kivy_widgets-0.1.6.tar", max compression
```

## Comparing `kivy_widgets-0.1.5.tar` & `kivy_widgets-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1068 2023-03-22 04:32:53.454823 kivy_widgets-0.1.5/LICENSE
--rw-r--r--   0        0        0     1098 2023-03-29 09:24:10.945782 kivy_widgets-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-03-24 03:41:57.270003 kivy_widgets-0.1.5/kivy_widgets/__init__.py
--rw-r--r--   0        0        0      382 2023-03-29 08:42:31.130706 kivy_widgets-0.1.5/kivy_widgets/buttons.py
--rw-r--r--   0        0        0     7716 2023-03-29 09:08:00.598752 kivy_widgets-0.1.5/kivy_widgets/color_definitions.py
--rw-r--r--   0        0        0  1261792 2023-03-29 09:08:00.604752 kivy_widgets-0.1.5/kivy_widgets/fonts/materialdesignicons-webfont.ttf
--rw-r--r--   0        0        0   266864 2023-03-29 09:08:00.605752 kivy_widgets-0.1.5/kivy_widgets/icon_definitions.py
--rw-r--r--   0        0        0     6812 2023-03-29 20:57:19.236051 kivy_widgets-0.1.5/kivy_widgets/icons.py
--rw-r--r--   0        0        0       61 2023-03-24 03:42:53.850005 kivy_widgets-0.1.5/kivy_widgets/test.py
--rw-r--r--   0        0        0      994 2023-03-29 21:03:40.714063 kivy_widgets-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 kivy_widgets-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-22 04:32:53.454823 kivy_widgets-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1098 2023-03-29 09:24:10.945782 kivy_widgets-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-03-24 03:41:57.270003 kivy_widgets-0.1.6/kivy_widgets/__init__.py
+-rw-r--r--   0        0        0     2723 2023-04-25 01:47:03.092367 kivy_widgets-0.1.6/kivy_widgets/buttons.py
+-rw-r--r--   0        0        0     7716 2023-03-29 09:08:00.598752 kivy_widgets-0.1.6/kivy_widgets/color_definitions.py
+-rw-r--r--   0        0        0  1261792 2023-03-29 09:08:00.604752 kivy_widgets-0.1.6/kivy_widgets/fonts/materialdesignicons-webfont.ttf
+-rw-r--r--   0        0        0   266864 2023-03-29 09:08:00.605752 kivy_widgets-0.1.6/kivy_widgets/icon_definitions.py
+-rw-r--r--   0        0        0     6794 2023-04-05 03:45:49.650130 kivy_widgets-0.1.6/kivy_widgets/icons.py
+-rw-r--r--   0        0        0        0 2023-04-01 03:59:53.455098 kivy_widgets-0.1.6/kivy_widgets/inspector.py
+-rw-r--r--   0        0        0       61 2023-03-24 03:42:53.850005 kivy_widgets-0.1.6/kivy_widgets/test.py
+-rw-r--r--   0        0        0      994 2023-04-25 01:50:50.658374 kivy_widgets-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 kivy_widgets-0.1.6/PKG-INFO
```

### Comparing `kivy_widgets-0.1.5/LICENSE` & `kivy_widgets-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.5/README.md` & `kivy_widgets-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.5/kivy_widgets/color_definitions.py` & `kivy_widgets-0.1.6/kivy_widgets/color_definitions.py`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.5/kivy_widgets/fonts/materialdesignicons-webfont.ttf` & `kivy_widgets-0.1.6/kivy_widgets/fonts/materialdesignicons-webfont.ttf`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.5/kivy_widgets/icon_definitions.py` & `kivy_widgets-0.1.6/kivy_widgets/icon_definitions.py`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.5/kivy_widgets/icons.py` & `kivy_widgets-0.1.6/kivy_widgets/icons.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,22 +21,23 @@
 
 __file__ = os.path.abspath(__file__)
 font_path = os.path.join(
     os.path.dirname(__file__), "fonts", "materialdesignicons-webfont.ttf"
 )
 
 global_idmap["unicode"] = icon_unicodes
+global_idmap["icon_font"] = font_path
 
 
 class Icon(Label):
     icon = StringProperty("android")
     font_name = StringProperty(font_path)
     icon_color = ColorProperty([0, 0, 0, 0.1])
     icon_size = NumericProperty(dp(21))
-    background_color = ColorProperty([0, 0, 0, 0])
+    bg_color = ColorProperty([0, 0, 0, 0])
     mode = OptionProperty(
         "default", options=["default", "stretch-background", "stretch-icon"]
     )
 
 
 class IconViewer(RelativeLayout):
     icons = ListProperty()
@@ -62,43 +63,43 @@
             self.icons = [
                 {"icon": name_icon, "viewer": self}
                 for name_icon in icon_unicodes.keys()
             ]
 
 
 class IconViewerItem(ButtonBehavior, BoxLayout):
-    background_color = ListProperty([0, 0, 0, 0.2])
+    bg_color = ListProperty([0, 0, 0, 0.2])
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         Window.bind(mouse_pos=self.check_collision)
 
     def check_collision(self, _, pos):
         """
         Checks if mouse is over icon,
         updates icon background color
         and tipbox position/opacity.
         """
         if self.collide_point(*self.to_widget(*pos)):
-            self.background_color = [0, 0, 0, 0.4]
+            self.bg_color = [0, 0, 0, 0.4]
 
             self.viewer.tipbox.pos = (
                 self.to_window(*self.pos)[0] - self.width / 2,
                 self.to_window(*self.pos)[1] + self.height,
             )
 
             def update_opacity(*args):
                 self.viewer.tipbox.opacity = 1
 
             if self.viewer.selected_icon == self.icon:
                 Clock.schedule_once(update_opacity)
 
             self.viewer.selected_icon = self.icon
         else:
-            self.background_color = [0, 0, 0, 0.2]
+            self.bg_color = [0, 0, 0, 0.2]
             self.viewer.tipbox.opacity = 0
 
     def on_release(self):
         """
         Copy icon name to clipboard
         and update tipbox text
         """
@@ -114,15 +115,15 @@
     size: (root.icon_size, root.icon_size) if root.mode == "default" else (self.texture_size[0], self.texture_size[1]) # this is the background size
     font_size: root.icon_size if root.mode in ["default", "stretch-background"] else (root.size[0] if root.size[0] < root.size[1] else root.size[1]) # this is the icon size
     pos_hint: {"center_x": .5, "center_y": .5}
     color: root.icon_color
     
     canvas.before:
         Color:
-            rgba: root.background_color or (0, 0, 0, 0)
+            rgba: root.bg_color or (0, 0, 0, 0)
         Rectangle:
             pos: self.pos
             size: self.size
 
 <IconViewer>:
     available_space: self.width - dp(30)
     number_of_spacings: int((root.available_space - 2*dp(20)) / dp(150)) - 1
@@ -204,24 +205,24 @@
             rgba: gray_300
         Line:
             rectangle: self.x, self.y, self.width, self.height
             width: dp(1)
 
     canvas.after:
         Color:
-            rgba: root.background_color
+            rgba: root.bg_color
         Rectangle:
             pos: self.pos
             size: self.size
 
     Icon:
         mode: "stretch-icon"
         icon: root.icon
         icon_color: rgba("#5F6368")
-        background_color: slate_200
+        bg_color: slate_200
     Label:
         text: root.icon
         font_size: dp(16)
         size_hint_y: None
         height: dp(20)
         color: black
         shorten: True
```

### Comparing `kivy_widgets-0.1.5/pyproject.toml` & `kivy_widgets-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kivy-widgets"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["filipemarch <filipe.marchesini@gmail.com>", "ShootingStarDragon <rppapamaths@gmail.com>"]
 readme = "README.md"
 packages = [{include = "kivy_widgets"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `kivy_widgets-0.1.5/PKG-INFO` & `kivy_widgets-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivy-widgets
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: filipemarch
 Author-email: filipe.marchesini@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

