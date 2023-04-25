# Comparing `tmp/clera-0.0.6.tar.gz` & `tmp/clera-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clera-0.0.6.tar", last modified: Tue Apr 11 13:25:32 2023, max compression
+gzip compressed data, was "clera-0.0.7.tar", last modified: Tue Apr 25 05:45:24 2023, max compression
```

## Comparing `clera-0.0.6.tar` & `clera-0.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 13:25:32.174507 clera-0.0.6/
--rw-rw-rw-   0        0        0      306 2023-04-11 12:10:43.000000 clera-0.0.6/CHANGELOG.md
--rw-rw-rw-   0        0        0     1058 2023-04-01 11:32:04.000000 clera-0.0.6/LICENCE.txt
--rw-rw-rw-   0        0        0       42 2023-04-01 11:31:56.000000 clera-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0    17705 2023-04-11 13:25:32.141435 clera-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    16175 2023-04-11 12:09:09.000000 clera-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 13:25:31.781499 clera-0.0.6/clera/
--rw-rw-rw-   0        0        0       44 2023-01-04 21:56:46.000000 clera-0.0.6/clera/__init__.py
--rw-rw-rw-   0        0        0    45872 2023-04-01 23:28:48.000000 clera-0.0.6/clera/core.py
-drwxrwxrwx   0        0        0        0 2023-04-11 13:25:31.749584 clera-0.0.6/clera/docs/
-drwxrwxrwx   0        0        0        0 2023-04-11 13:25:31.867273 clera-0.0.6/clera/docs/images/
--rw-rw-rw-   0        0        0     7524 2023-04-04 11:32:50.000000 clera-0.0.6/clera/docs/images/empty_window.png
-drwxrwxrwx   0        0        0        0 2023-04-11 13:25:31.878240 clera-0.0.6/clera/icons/
--rw-rw-rw-   0        0        0   290225 2023-02-13 13:07:36.000000 clera-0.0.6/clera/icons/hand-drawn-icon.png
--rw-rw-rw-   0        0        0    87456 2023-02-13 13:46:44.000000 clera-0.0.6/clera/icons/toon-icon.ico
-drwxrwxrwx   0        0        0        0 2023-04-11 13:25:31.926622 clera-0.0.6/clera/utils/
--rw-rw-rw-   0        0        0      121 2023-03-19 13:16:12.000000 clera-0.0.6/clera/utils/__init__.py
--rw-rw-rw-   0        0        0      129 2023-03-24 12:03:54.000000 clera-0.0.6/clera/utils/exceptions.py
--rw-rw-rw-   0        0        0    15007 2023-04-01 23:18:54.000000 clera-0.0.6/clera/utils/handlers.py
--rw-rw-rw-   0        0        0     1071 2023-03-19 13:17:06.000000 clera-0.0.6/clera/utils/keys.py
--rw-rw-rw-   0        0        0     6196 2023-03-24 12:02:34.000000 clera-0.0.6/clera/utils/procr.py
--rw-rw-rw-   0        0        0     3328 2023-03-24 12:03:42.000000 clera-0.0.6/clera/utils/style.py
--rw-rw-rw-   0        0        0    27094 2023-04-11 10:49:46.000000 clera-0.0.6/clera/widgets.py
-drwxrwxrwx   0        0        0        0 2023-04-11 13:25:31.863283 clera-0.0.6/clera.egg-info/
--rw-rw-rw-   0        0        0    17705 2023-04-11 13:25:31.000000 clera-0.0.6/clera.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-04-11 13:25:31.000000 clera-0.0.6/clera.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 13:25:31.000000 clera-0.0.6/clera.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 13:25:31.000000 clera-0.0.6/clera.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-11 13:25:31.000000 clera-0.0.6/clera.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 13:25:32.175345 clera-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1286 2023-04-11 13:25:08.000000 clera-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 05:45:24.204774 clera-0.0.7/
+-rw-rw-rw-   0        0        0      654 2023-04-25 04:51:01.000000 clera-0.0.7/CHANGELOG.md
+-rw-rw-rw-   0        0        0     7651 2023-04-23 00:22:43.000000 clera-0.0.7/LICENCE.txt
+-rw-rw-rw-   0        0        0       42 2023-04-01 11:31:56.000000 clera-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2503 2023-04-25 05:45:24.198527 clera-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1135 2023-04-25 05:28:48.000000 clera-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 05:45:24.009375 clera-0.0.7/clera/
+-rw-rw-rw-   0        0        0      140 2023-04-24 21:56:58.000000 clera-0.0.7/clera/__init__.py
+-rw-rw-rw-   0        0        0    51545 2023-04-24 20:28:34.000000 clera-0.0.7/clera/core.py
+drwxrwxrwx   0        0        0        0 2023-04-25 05:45:24.090233 clera-0.0.7/clera/icons/
+-rw-rw-rw-   0        0        0   290225 2023-02-13 13:07:36.000000 clera-0.0.7/clera/icons/hand-drawn-icon.png
+-rw-rw-rw-   0        0        0    41561 2023-04-25 04:20:56.000000 clera-0.0.7/clera/icons/toon-icon.ico
+drwxrwxrwx   0        0        0        0 2023-04-25 05:45:24.173017 clera-0.0.7/clera/utils/
+-rw-rw-rw-   0        0        0      121 2023-03-19 13:16:12.000000 clera-0.0.7/clera/utils/__init__.py
+-rw-rw-rw-   0        0        0      129 2023-03-24 12:03:54.000000 clera-0.0.7/clera/utils/exceptions.py
+-rw-rw-rw-   0        0        0    16214 2023-04-24 20:53:36.000000 clera-0.0.7/clera/utils/handlers.py
+-rw-rw-rw-   0        0        0     1071 2023-03-19 13:17:06.000000 clera-0.0.7/clera/utils/keys.py
+-rw-rw-rw-   0        0        0     6196 2023-03-24 12:02:34.000000 clera-0.0.7/clera/utils/procr.py
+-rw-rw-rw-   0        0        0     4238 2023-04-25 04:56:14.000000 clera-0.0.7/clera/utils/style.py
+-rw-rw-rw-   0        0        0    27118 2023-04-24 20:54:33.000000 clera-0.0.7/clera/widgets.py
+drwxrwxrwx   0        0        0        0 2023-04-25 05:45:24.074920 clera-0.0.7/clera.egg-info/
+-rw-rw-rw-   0        0        0     2503 2023-04-25 05:45:23.000000 clera-0.0.7/clera.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      476 2023-04-25 05:45:23.000000 clera-0.0.7/clera.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 05:45:23.000000 clera-0.0.7/clera.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-25 05:45:23.000000 clera-0.0.7/clera.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-25 05:45:23.000000 clera-0.0.7/clera.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 05:45:24.189582 clera-0.0.7/images/
+-rw-rw-rw-   0        0        0   290225 2023-02-13 13:07:36.000000 clera-0.0.7/images/icon.png
+-rw-rw-rw-   0        0        0     7524 2023-04-04 11:32:50.000000 clera-0.0.7/images/window.png
+-rw-rw-rw-   0        0        0       42 2023-04-25 05:45:24.207492 clera-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1238 2023-04-25 05:45:20.000000 clera-0.0.7/setup.py
```

### Comparing `clera-0.0.6/clera/core.py` & `clera-0.0.7/clera/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from PySide6.QtCore import QSize, QPoint, QEvent
-from PySide6.QtGui import QIcon, Qt, QMouseEvent
+from PySide6.QtGui import QIcon, Qt, QMouseEvent, QScreen
 from PySide6.QtWidgets import QMainWindow, QToolBar, QStatusBar, QGroupBox, QButtonGroup
 from PySide6.QtWidgets import QWidget,  QHBoxLayout, QVBoxLayout,  QGridLayout, QTabWidget, QMenu
-from PySide6.QtWidgets import QDialog, QFileDialog
+from PySide6.QtWidgets import QDialog, QFileDialog, QStyleFactory
 
 from .utils import *
 from .widgets import *
 
 __all__ = [
     'Window', 'Box', 'Grid', 'fieldset', 'Column', 'column', 'Group', 'group', 'Toolbar', 'toolbar',
     'Menubar', 'menubar', 'Statusbar', 'statusbar', 'GET', 'get', 'Button', 'button', 'Input',
@@ -26,17 +26,26 @@
 
 
 def init_window_css(css_string):
     custom, builtins = console_css(css_string)
 
     for items in custom:
         name, property = items
+        widget = WIDGET_ID_SAFE[name]
 
         if name in WIDGET_ID_SAFE:
-            WIDGET_ID_SAFE[name].setStyleSheet(property)
+            for value in compr:
+                value = value.split('::')
+                _type = value[1]
+
+                if _type in str(type(widget)):
+                    break
+
+            property = property.replace(TYPE_MARKER, _type)
+            widget.setStyleSheet(property)
 
     app.setStyleSheet(builtins)
 
 
 def link(href: None = None):
     if href != None:
         LINK_ITEMS_INCLUDED.append(href)
@@ -53,52 +62,77 @@
             with open(file_path, 'r') as file:
                 file_content = file.read()
 
             init_window_css(file_content)
 
 
 class MainWindow(QMainWindow):
-    def __init__(self, title, icon, size, fixed_size, geometry, style, frame, movable, top):
+    def __init__(self, title, icon, size, fixed_size, geometry, style, frame, movable, win_top, spacing, content_margin, move):
         super().__init__()
 
         self._qwidget = DEFAULT_WINDOW_LAYOUT
         self._title = title
         self._size = size
         self._fixed_size = fixed_size
         self._icon = icon
         self._geometry = geometry
         self._movable = movable
         self._frame = frame
+        self._top = win_top
+        self._spacing = spacing
+        self._content_margin = content_margin
+        self._move = move
 
         self._query_fixed_size = False
         self._custom_title_bar = False
 
         width, height = self._size
         if width != None and height != None:
             self.resize(int(width), int(height))
 
+        positionx, positiony = self._move
+        if positionx != None and positiony != None:
+            self.move(positionx, positiony)
+
         if self._geometry != None:
             if len(self._geometry) == 4:
                 x, y, w, h = self._geometry
                 self.setGeometry(x, y, w, h)
 
         self.setWindowTitle(self._title)
-        if top == True:
+
+        if self._top == True:
             self.setWindowFlags(Qt.WindowStaysOnTopHint)
 
         app.setStyle(style)
 
         fixed_width, fixed_height = self._fixed_size
         if fixed_width != None and fixed_height != None:
             self._query_fixed_size = True
             self.setFixedSize(QSize(int(fixed_width), int(fixed_height)))
 
         global layout
         layout = QVBoxLayout()
 
+        layout.setSpacing(self._spacing)
+
+        if type(self._content_margin) != int:
+            if len(self._content_margin) == 4:
+                left, top, right, bottom = self._content_margin
+                layout.setContentsMargins(left, top, right, bottom)
+            elif len(self._content_margin) == 2:
+                top_bottom, left_right = self._content_margin
+                layout.setContentsMargins(
+                    left_right, top_bottom, left_right, top_bottom)
+            else:
+                ...
+        else:
+            layout.setContentsMargins(
+                self._content_margin, self._content_margin, self._content_margin, self._content_margin)
+
         self._qwidget.setLayout(layout)
 
         if self._frame == False:
             self.setWindowFlag(Qt.FramelessWindowHint)
 
         self.setWindowIcon(QIcon(get_path(self._icon)))
 
@@ -151,16 +185,16 @@
         else:
             raise ValueError(position)
 
         if tool_items != None:
             for item in tool_items:
                 if type(item) != type(list()):
                     widget_type, widget_items = check_func(item)
-                    widget = LayItOut(GRAB_WIDGET, widget_type, widget_items)
-                    toolbar.addWidget(widget)
+                    LayItOut(toolbar, widget_type, widget_items)
+                    # toolbar.addWidget(widget)
                 else:
 
                     item_type = item[0]
 
                     if item_type == ELEM_TYPE_ITEM:
 
                         item_label = item[1]
@@ -189,19 +223,21 @@
             toolbar.setStyleSheet('border-bottom: 0px')
 
     # Status bar functions
 
     def init_status(self):
         self.setStatusBar(QStatusBar(self))
 
-    def ADD_PERMANENT_WIDGET(self, addwidget):
-        self.statusBar().addPermanentWidget(addwidget)
-
-    def ADD_NORMAL_WIDGET(self, addwidget):
-        self.statusBar().addWidget(addwidget)
+    def ADD_PERMANENT_WIDGET(self, widget_type, widget_items):
+        lyt = self.statusBar()
+        LayItOut([lyt, 'addPermanentWidget'], widget_type, widget_items)
+
+    def ADD_NORMAL_WIDGET(self, widget_type, widget_items):
+        lyt = self.statusBar()
+        LayItOut([lyt, 'addWidget'], widget_type, widget_items)
 
     def SHOW_STATUSBAR_MESSAGE(self, text, time):
         if time != None:
             time = time * 1000
             self.statusBar().showMessage(text, time)
         else:
             self.statusBar().showMessage(text)
@@ -211,29 +247,26 @@
 
     def REMOVE_STATUSBAR_WIDGET(self, ID):
         if ID in WIDGET_ID_SAFE:
             self.statusBar().removeWidget(WIDGET_ID_SAFE[ID])
         else:
             raise IdError(f'id "{ID}" does not exist')
 
-    def mousePressEvent(self, event: QMouseEvent):
-        if self._movable == True:
-            try:
-                self.old_position = event.globalPos()
-            except:
-                ...
-
-    def mouseMoveEvent(self, event: QMouseEvent):
-        if self._movable == True:
-            try:
-                omega = QPoint(event.globalPos() - self.old_position)
-                self.move(self.x() + omega.x(), self.y() + omega.y())
-                self.old_position = event.globalPos()
-            except:
-                ...
+    def mousePressEvent(self, event):
+        self.old_position = event.globalPos()
+        return self.old_position
+
+    def mouseMoveEvent(self, event):
+        omega = QPoint(event.globalPos() - self.old_position)
+
+        if self._custom_title_bar == False and self._movable == True and self._frame == False:
+            self.move(self.x() + omega.x(), self.y() + omega.y())
+            self.old_position = event.globalPos()
+        else:
+            return omega
 
     def WindowTitlebar(self, icon, title, widgets, alignment, backgound_color,  text_color, height,
                        button_style):
         current_window_style = window.style().name().lower()
 
         if current_window_style == SYSTEM_PLATFORM_FUSION:
             CONTROL_MINIMIZED, CONTROL_RESTORE, CONTROL_MAXIMIZED = FUSION_CONTROLS()
@@ -275,52 +308,67 @@
                     except:
                         ...
             if icon != None:
                 titlebar_icon = Image(icon, id=ICON_IMAGE_ID, size=20)
             else:
                 titlebar_icon = empty()
 
-            if current_window_style == SYSTEM_PLATFORM_FUSION or current_window_style == SYSTEM_PLATFORM_WINDOWS:
-                title_items = [
-                    titlebar_icon,
-                    Text(title, id=TITLE_TEXT_ID,
-                         sizepolicy=('expand', 'fixed'), alignment=align),
-                    Button(CONTROL_MINIMIZED, id=MINIMIZE_BUTTON_ID,
-                           func=call(control_action, 'min'), focus=False),
-                    Button(CONTROL_MAXIMIZED, id=MAXIMIZE_BUTTON_ID,
-                           func=call(control_action, 'max'), focus=False),
-                    Button(CONTROL_CLOSE, id=CLOSE_BUTTON_ID,
-                           func=Window.quit, focus=False)
-                ]
-            else:
-                if icon != None:
-                    align = 'center'
-                else:
-                    align = 'right'
-
-                title_items = [
-                    Button(CONTROL_CLOSE, id=CLOSE_BUTTON_ID,
-                           func=Window.quit, focus=False),
-                    Button(CONTROL_MINIMIZED, id=MINIMIZE_BUTTON_ID,
-                           func=call(control_action, 'min'), focus=False),
-                    Button(CONTROL_MAXIMIZED, id=MAXIMIZE_BUTTON_ID,
-                           func=call(control_action, 'max'), focus=False),
-                    Text(title, id=TITLE_TEXT_ID,
-                         sizepolicy=('expand', 'fixed'), alignment=align),
-                    titlebar_icon
-                ]
+            title_items = [
+                titlebar_icon,
+                Text(title, id=TITLE_TEXT_ID,
+                     sizepolicy=('expand', 'fixed'), alignment=align),
+                Button(CONTROL_MINIMIZED, id=MINIMIZE_BUTTON_ID,
+                       func=call(control_action, 'min'), focus=False),
+                Button(CONTROL_MAXIMIZED, id=MAXIMIZE_BUTTON_ID,
+                       func=call(control_action, 'max'), focus=False),
+                Button(CONTROL_CLOSE, id=CLOSE_BUTTON_ID,
+                       func=Window.quit, focus=False)
+            ]
 
-            self._movable = True
+            container = INIT_WIDGET(
+                '-clera_titlebar_container-', QToolBar('Container'))
             titlebar = INIT_WIDGET('titlebar', QToolBar('Titlebar'))
 
+            class init_titlebar(QWidget):
+                def __init__(self):
+                    super().__init__()
+                    cs_layout = QHBoxLayout()
+                    self.setLayout(cs_layout)
+                    cs_layout.setContentsMargins(0, 0, 0, 0)
+                    cs_layout.addWidget(titlebar)
+                    window.setCentralWidget(self)
+
+                def mousePressEvent(self, event: QMouseEvent):
+                    self.old_position = window.mousePressEvent(event)
+                    window.setCursor(Qt.SizeAllCursor)
+
+                def mouseMoveEvent(self, event: QMouseEvent):
+                    omega = window.mouseMoveEvent(event)
+                    window.move(window.x() + omega.x(), window.y() + omega.y())
+                    self.old_position = window.mousePressEvent(event)
+
+                def mouseReleaseEvent(self, event: QMouseEvent):
+                    window.setCursor(Qt.ArrowCursor)
+
+            container_socket = init_titlebar()
+            container_socket.setContentsMargins(0, 0, 0, 0)
+
+            container.addWidget(container_socket)
+            container.setStyleSheet('margin: 0; padding: 0; border: 0px;')
+
+            container.setMovable(False)
+            titlebar.setMovable(False)
+
+            self.addToolBar(Qt.TopToolBarArea, container)
+
             titlebar.toggleViewAction().setVisible(False)
 
             titlebar.setIconSize(QSize(20, 20))
 
-            self.addToolBar(Qt.TopToolBarArea, titlebar)
+            # self.addToolBar(Qt.TopToolBarArea, titlebar)
 
             self.addToolBarBreak()
 
             if widgets != None:
                 if align == 'center':
                     for item in title_items:
                         append_items(widgets, item)
@@ -336,18 +384,16 @@
                             append_items(window_title, item)
 
                     title_items = window_title
 
             for item in title_items:
                 if type(item) != type(list()):
                     widget_type, widget_items = check_func(item)
-                    widget = LayItOut(GRAB_WIDGET, widget_type, widget_items)
-                    titlebar.addWidget(widget)
-
-            titlebar.setMovable(False)
+                    LayItOut(titlebar, widget_type, widget_items)
+                    # titlebar.addWidget(widget)
 
             titlebar.setOrientation(Qt.Horizontal)
 
             button_style_query = button_style.lower()
 
             if button_style_query == 'circle':
                 control_button_style = CONTROL_BUTTON_CIRCLE
@@ -363,24 +409,24 @@
 
             def init_title_icon(icon, value: str = 'left'):
                 if icon != None:
                     icon = GET(ICON_IMAGE_ID)
                     icon.style(f'margin-{value}: 10px;')
 
             init_title_icon(icon)
+
             if current_window_style == SYSTEM_PLATFORM_FUSION:
                 fusion_style(minimize, maximize, close, control_button_style)
-            elif current_window_style == SYSTEM_PLATFORM_WINDOWS:
+            elif current_window_style == SYSTEM_PLATFORM_WINDOWS or current_window_style == 'windowsvista':
                 windows_style(minimize, maximize, close)
             else:
-                init_title_icon(icon, 'right')
-                clera_style(minimize, maximize, close)
+                ...
 
             title.style(
-                f'color: {text_color}; padding: 6px 0; margin: 0 {height}px')
+                f'color: {text_color}; padding: 7px 0; margin: 0 {height}px;')
             titlebar.setStyleSheet(
                 f'border-bottom: 0px; background: {backgound_color};')
             self._custom_title_bar = True
 
 
 # ------------------------------------------------------------------------#
 
@@ -390,15 +436,16 @@
 
 # ------------------------------------------------------------------------#
 
 
 class Window:
     def __init__(self, title: str = DEFAULT_WINDOW_TITLE, icon: str = DEFAULT_WINDOW_ICON, size: tuple = DEFAULT_WINDOW_SIZE,
                  geometry: tuple = DEFAULT_WINDOW_GEOMETRY, style: str = DEFAULT_WINDOW_STYLE, fixed_size: tuple = DEFAULT_WINDOW_FIXED_SIZE, frame: bool = True,
-                 movable: bool = False, top: bool = False):
+                 movable: bool = False, top: bool = False, spacing: int = 2, content_margin: tuple = (2, 2, 2, 2),
+                 move: tuple = (None, None)):
         '''
         :param title:
         :param icon:
         :param size:
         :param geometry:
         :param style:
         :param fixed_size:
@@ -412,18 +459,21 @@
         self.window_size = size
         self.window_fixed_size = fixed_size
         self.window_geometry = geometry
         self.window_style = style
         self.frame = frame
         self.movable = movable
         self.top = top
+        self.spacing = spacing
+        self.content_margin = content_margin
+        self.move = move
 
         window = MainWindow(self.window_title, self.window_icon,
                             self.window_size, self.window_fixed_size, self.window_geometry, self.window_style, self.frame,
-                            self.movable, self.top)
+                            self.movable, self.top, self.spacing, self.content_margin, self.move)
 
     def run(self, css: None = None):
         window.show()
         if css != None:
             init_window_css(css)
 
         if len(LINK_ITEMS_INCLUDED) != 0:
@@ -456,20 +506,20 @@
 
     def quit(self):
         app.quit()
 
     def update(self, remove_id, widget):
         replace_widget = WIDGET_ID_SAFE[remove_id]
 
-        WidgetType, property = check_func(widget)
+        widget_type, widget_items = check_func(widget)
 
         try:
             layout.indexOf(replace_widget)
-            temp_widget = LayItOut(GRAB_WIDGET, WidgetType, property)
-            layout.replaceWidget(replace_widget, temp_widget)
+            LayItOut([layout, replace_widget, 'replaceWidget'],
+                     widget_type, widget_items)
             layout.removeWidget(replace_widget)
             replace_widget.deleteLater()
             replace_widget = None
         except:
             pass
 
     def normal(self):
@@ -477,14 +527,41 @@
 
     def minimize(self):
         window.setWindowState(Qt.WindowMinimized)
 
     def maximize(self):
         window.setWindowState(Qt.WindowMaximized)
 
+    def details(self):
+        screen = window.screen().virtualSize()
+        _title = window.windowTitle()
+
+        if len(_title) == 0:
+            _title = None
+
+        window_details = {
+            'position': window.geometry().getCoords()[:2],
+            'screen': (screen.width(), screen.height()),
+            'style': window.style().name(),
+            'title': _title,
+            'system_styles': QStyleFactory().keys()
+        }
+
+        return window_details
+
+    def title(self, value: any = None):
+        if value != None:
+            window.setWindowTitle(value)
+
+    def _move(self, position: tuple = (None, None), top: bool = None):
+        positionx, positiony = position
+
+        if positionx != None and positiony != None:
+            window.move(positionx, positiony)
+
 
 # ------------------------------------------------------------------------#
 
 ###########################################################################
 ############################## CORE HANDLERS ##############################
 ###########################################################################
 
@@ -784,19 +861,17 @@
     def clear(self):
         window.CLEAR_STATUSBAR_MESSAGE()
 
     def add(self, widget, type: str = SET_NORMAL):
         type = type.upper()
         widget_type, widget_items = check_func(widget)
         if type == SET_NORMAL:
-            addwidget = LayItOut(GRAB_WIDGET, widget_type, widget_items)
-            window.ADD_NORMAL_WIDGET(addwidget)
+            window.ADD_NORMAL_WIDGET(widget_type, widget_items)
         elif type == SET_STATIC:
-            addwidget = LayItOut(GRAB_WIDGET, widget_type, widget_items)
-            window.ADD_PERMANENT_WIDGET(addwidget)
+            window.ADD_PERMANENT_WIDGET(widget_type, widget_items)
         else:
             raise ValueError(f'"{type}" is an invalid type value')
 
     def remove(self, id):
         window.REMOVE_STATUSBAR_WIDGET(id)
 
 
@@ -1004,16 +1079,16 @@
             self.widget.setText(str(value))
 
     def update(self, widget):
         widget_type, widget_items = check_func(widget)
 
         try:
             layout.indexOf(self.widget)
-            temp_widget = LayItOut(GRAB_WIDGET, widget_type, widget_items)
-            layout.replaceWidget(self.widget, temp_widget)
+            LayItOut([layout, self.widget, 'replaceWidget'],
+                     widget_type, widget_items)
             layout.removeWidget(self.widget)
             self.widget.deleteLater()
             self.widget = None
         except:
             ...
 
         # WIDGET_ID_SAFE.pop(self.id)
@@ -1066,18 +1141,88 @@
 
     def is_default(self):
         return self.widget.isDefault()
 
     def is_readonly(self):
         return self.widget.isReadonly()
 
-    def style(self, css: None = None):
+    def style(self, css: None = None, reset: bool = False):
         if css != None:
             css = get_style_check(css)  # check for css errors
-            self.widget.setStyleSheet(css)
+            get_css = self.widget.styleSheet()
+
+            if reset == False:
+                if len(get_css) != 0:
+                    def temp_handle(css):
+                        container = []
+                        css = css.split('}')
+                        for item in css:
+                            item = item.split('{')
+                            container.append(item)
+
+                        return container
+
+                    get_css = temp_handle(get_css)
+                    css = temp_handle(css)
+
+                    def make_changes(old, new):
+                        for item in old:
+                            old[old.index(item)] = item.split(':')
+
+                        for item in new:
+                            new[new.index(item)] = item.split(':')
+
+                        space = [' ']
+                        if space in old:
+                            old.remove(space)
+                        elif space in new:
+                            new.remove(space)
+
+                        for old_item in old:
+                            for new_item in new:
+                                if old_item[0].strip() == new_item[0].strip() and len(old_item[0].strip()) != 0:
+                                    old_item[1] = new_item[1]
+                                    new.remove(new_item)
+
+                        for new_item in new:
+                            old.append(new_item)
+
+                        for items in old:
+                            old[old.index(items)] = ':'.join(items)
+
+                        return '; '.join(old)
+
+                    for already in get_css:
+                        for new_css in css:
+                            if len(new_css) == 1:
+                                if ':' not in already[0] and len(already[0]) != 0:
+                                    get_property = already[1].split(';')
+                                    new_property = new_css[0].split(';')
+                                    already[1] = make_changes(
+                                        get_property, new_property)
+                                    # already[1] = already[1] + ' ' + new_css[0] + ' '
+                            else:
+                                if already[0].strip() == new_css[0].strip():
+                                    get_property = already[1].split(';')
+                                    new_property = new_css[1].split(';')
+                                    already[1] = make_changes(
+                                        get_property, new_property)
+                    else:
+                        # print(get_css, new_css)
+                        for item in get_css:
+                            get_css[get_css.index(item)] = '{'.join(item)
+                        else:
+                            new_css = '}'.join(get_css)
+                            # print(new_css)
+
+                    self.widget.setStyleSheet(new_css)
+                else:
+                    self.widget.setStyleSheet(css)
+            else:
+                self.widget.setStyleSheet(css)
 
     def is_checked(self):
         return self.widget.isChecked()
 
     def hidden(self, value: bool | None = None):
         if value != None:
             self.widget.setHidden(value)
```

### Comparing `clera-0.0.6/clera/docs/images/empty_window.png` & `clera-0.0.7/images/window.png`

 * *Files identical despite different names*

### Comparing `clera-0.0.6/clera/icons/hand-drawn-icon.png` & `clera-0.0.7/clera/icons/hand-drawn-icon.png`

 * *Files identical despite different names*

### Comparing `clera-0.0.6/clera/utils/handlers.py` & `clera-0.0.7/clera/utils/handlers.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ID_COUNT_DEFAULT = [0]
 TOOLBAR_COUNT = []
 LINK_ITEMS_INCLUDED = []
 
 SIZE_POLICY_EXPAND = 'expand'
 SIZE_POLICY_FIXED = 'fixed'
 
-GRAB_WIDGET = 'GrabWidget'
+# GRAB_WIDGET = 'GrabWidget'
 
 DEFAULT_SEPARATOR_MARKER = '---'
 
 ELEM_TYPE_ITEM = 'item'
 ELEM_TYPE_SEPARATOR = 'separator'
 ELEM_TYPE_COLUMN = 'column'
 ELEM_TYPE_GROUP = 'group'
@@ -209,25 +209,39 @@
             vertical = QSizePolicy.Expanding
         else:
             raise ValueError(vertical_policy)
 
         widget.setSizePolicy(horizontal, vertical)
 
 
-def set_grid(lyt, grid, widget, grid_pos_x, grid_pos_y):
+def set_widget(lyt, grid, widget, grid_pos_x, grid_pos_y):
     gridx, gridy = grid  # horizontal and vertical occupy rule for grid widgets
 
-    if lyt != GRAB_WIDGET:
+    if type(lyt) != sample_list and type(lyt) != sample_string:
         if grid_pos_x != None and grid_pos_y != None:
             if gridx != None and gridy != None:
                 lyt.addWidget(widget, grid_pos_x, grid_pos_y, gridx, gridy)
             else:
                 lyt.addWidget(widget, grid_pos_x, grid_pos_y)
         else:
             lyt.addWidget(widget)
+    else:
+        if len(lyt) == 2:
+            lyt, _type = lyt
+
+            if _type == 'addWidget':
+                lyt.addWidget(widget)
+            elif _type == 'addPermanentWidget':
+                lyt.addPermanentWidget(widget)
+            else:
+                ...
+        elif len(lyt) == 3:
+            layout, pre_widget, _type = lyt
+            if _type == 'replaceWidget':
+                layout.replaceWidget(pre_widget, widget)
 
 
 def make_alignment(widget, alignments):
     def alignCheck(widget_alignment):
         alignment = widget_alignment.lower()
         if alignment == 'center':
             align = Qt.AlignCenter
@@ -461,54 +475,69 @@
 
 sample_function = type(sample_func())
 
 sample_integer = type(int())
 
 sample_tuple = type(tuple())
 
+if sys.platform.lower() == 'linux':
+    minimize_padding = ' padding: 0 7px 2px 7px'
+    maximize_padding = 'padding: 0px 6px 2px 6px'
+    close_padding = 'padding: 0 4px 1px 4px'
+else:
+    minimize_padding = 'padding: 1px 8px 3px 8px'
+    maximize_padding = 'padding: 1px 6px 3px 6px'
+    close_padding = 'padding: 1px 6px 3px 6px'
+
 
 def fusion_style(minimize, maximize, close, control_button_style):
     minimize.style(f'''
         button [
             color: rgb(18, 18, 18);
             font-weight: bold;
-            padding: 0 7px 2px 7px;
+            {minimize_padding};
             margin: 0 4px 0 5px;
             background: rgb(18, 18, 18);
             border-radius: {control_button_style};
+            min-width: 0px;
+            height: 20px;
         ]
 
         button:hover [
             color: white;
         ]
     ''')
 
     maximize.style(f'''
         button [
             color: rgb(18, 18, 18);
             font-weight: bold;
-            padding: 1px 6px 1px 6px;
+            {maximize_padding};
             margin-right: 4px;
             background: rgb(18, 18, 18);
             border-radius: {control_button_style};
+            min-width: 0px;
+            height: 20px;
         ]
 
         button:hover [
             color: white;
         ]
     ''')
 
     close.style(f'''
         button [
             color: rgb(18, 18, 18);
             margin-right: 8px;
             font-weight: bold;
-            padding: 0 4px 1px 4px;
+            {close_padding};
             background: rgb(56, 109, 209);
             border-radius: {control_button_style};
+            min-width: 0px;
+            height: 20px;
         ]
 
         button:hover [
             color: white;
         ]
     ''')
 
@@ -516,93 +545,100 @@
 def windows_style(minimize, maximize, close):
     minimize.style(f'''
         button [
             font-weight: bold;
             padding: 5.5px 17px 6.5px 17px;
             background: rgba(65, 63, 63, 0);
             border: 0px solid;
+            min-width: 0px;
+            color: white;
         ]
 
         button:hover [
             color: white;
             background: grey;
         ]
     ''')
 
     maximize.style(f'''
         button [
             font-weight: bold;
             padding: 5.5px 15px 6.5px 15px;
             background: rgba(65, 63, 63, 0);
             border: 0px solid;
+            color: white;
+            min-width: 0px;
+
         ]
 
         button:hover [
             color: white;
             background: grey;
         ]
     ''')
 
     close.style(f'''
         button [
             font-weight: bold;
             padding: 5.5px 15px;
             background: rgba(65, 63, 63, 0);
             border: 0px solid;
+            color: white;
+            min-width: 0px;
         ]
 
         button:hover [
             color: white;
             background: red;
         ]
     ''')
 
 
-def clera_style(minimize, maximize, close):
-    minimize.style(f'''
-        button [
-            color: rgb(206, 159, 5);
-            font-weight: bold;
-            margin-left: 4px;
-            padding: 0 7px 2px 7px;
-            background: rgb(206, 159, 5);
-            border-radius: {CONTROL_BUTTON_CIRCLE};
-        ]
-
-        button:hover [
-            color: rgb(122, 94, 0);
-        ]
-    ''')
-
-    maximize.style(f'''
-        button [
-            color: rgb(2, 141, 2);
-            font-weight: bold;
-            margin: 0 5px 0 4px;
-            padding: 1px 6px 1px 6px;
-            background: rgb(2, 141, 2);
-            border-radius: {CONTROL_BUTTON_CIRCLE};
-        ]
-
-        button:hover [
-            color: rgb(0, 41, 0);
-        ]
-    ''')
-
-    close.style(f'''
-        button [
-            color: rgb(172, 3, 3);
-            margin-left: 8px;
-            padding: 0 4px 1px 4px;
-            font-weight: bold;
-            background: rgb(172, 3, 3);
-            border-radius: {CONTROL_BUTTON_CIRCLE};
-        ]
-
-        button:hover [
-            color: rgb(61, 0, 0);
-        ]
-    ''')
+# def clera_style(minimize, maximize, close):
+#     minimize.style(f'''
+#         button [
+#             color: rgb(206, 159, 5);
+#             font-weight: bold;
+#             margin-left: 4px;
+#             padding: 0 7px 2px 7px;
+#             background: rgb(206, 159, 5);
+#             border-radius: {CONTROL_BUTTON_CIRCLE};
+#         ]
+
+#         button:hover [
+#             color: rgb(122, 94, 0);
+#         ]
+#     ''')
+
+#     maximize.style(f'''
+#         button [
+#             color: rgb(2, 141, 2);
+#             font-weight: bold;
+#             margin: 0 5px 0 4px;
+#             padding: 1px 6px 1px 6px;
+#             background: rgb(2, 141, 2);
+#             border-radius: {CONTROL_BUTTON_CIRCLE};
+#         ]
+
+#         button:hover [
+#             color: rgb(0, 41, 0);
+#         ]
+#     ''')
+
+#     close.style(f'''
+#         button [
+#             color: rgb(172, 3, 3);
+#             margin-left: 8px;
+#             padding: 0 4px 1px 4px;
+#             font-weight: bold;
+#             background: rgb(172, 3, 3);
+#             border-radius: {CONTROL_BUTTON_CIRCLE};
+#         ]
+
+#         button:hover [
+#             color: rgb(61, 0, 0);
+#         ]
+#     ''')
 
 
 def append_items(append_list, item):
     append_list.append(item)
```

### Comparing `clera-0.0.6/clera/utils/keys.py` & `clera-0.0.7/clera/utils/keys.py`

 * *Files identical despite different names*

### Comparing `clera-0.0.6/clera/utils/procr.py` & `clera-0.0.7/clera/utils/procr.py`

 * *Files identical despite different names*

### Comparing `clera-0.0.6/clera/utils/style.py` & `clera-0.0.7/clera/utils/style.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+TYPE_MARKER = '%TYPE%'
+SEPERATION_MARKER = ':-sep-:'
+PRE_MARK = '%<%'
+POST_MARK = '%>%'
+
 compr = [
     'button::QPushButton',
     'text:image:img::QLabel',
-    'input:QLineEdit',
+    'input::QLineEdit',
     'checkbox::QCheckBox',
     'radiobutton::QRadioButton',
     'toolbar::QToolBar',
     'fieldset::QGroupBox',
     'item::QToolButton',
     'textarea::QTextEdit',
     'window::QMainWindow',
@@ -39,14 +44,15 @@
 def console_css(user_css):
     css = []
     user_css = user_css.replace('[', '{').replace(']', '}')
     user_css = user_css.split('}')
     stylesheet = ""
 
     key_version = []
+    make_key_version = {}
 
     for item in user_css:
         item = item.replace('\n', '').replace('   ', '')
         item = item.split('{')
         if len(item[0]) != 0:
             css.append(item)
 
@@ -89,19 +95,38 @@
             if valid != True:
                 if '#' in name:
                     name = int(name.replace('#', ''))
                 else:
                     name = name.strip()
 
                 if len(selector) != 0:
-                    property = selector+'{'+property+' }'
+                    property = selector + SEPERATION_MARKER + property
 
                 # name = name + selector
-                x = [name, property]
-                key_version.append(x)
+                # x = [name, property]
+                # key_version.append(x)
+
+                KEY = name
+                if SEPERATION_MARKER in property:
+                    property = property.split(SEPERATION_MARKER)
+                    property = f'{TYPE_MARKER}{property[0]}{PRE_MARK + property[1] + POST_MARK}'
+                else:
+                    property = f'{TYPE_MARKER}{PRE_MARK + property + POST_MARK}'
+
+                property = property.replace(
+                    PRE_MARK, '{').replace(POST_MARK, '}')
+
+                if make_key_version.get(KEY):
+                    make_key_version[KEY] = make_key_version[KEY] + \
+                        ' ' + property
+                else:
+                    make_key_version[KEY] = property
+
+    for KEY in make_key_version.keys():
+        key_version.append([KEY, make_key_version[KEY]])
 
     return (key_version, stylesheet)
 
 
 def get_style_check(css):
     css = css.replace('[', '{').replace(']', '}')
     if '{' in css and '}' in css:
```

### Comparing `clera-0.0.6/clera/widgets.py` & `clera-0.0.7/clera/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 def window_button(lyt, button_text, func, icon,
                   ID, disabled, default, sizepolicy, grid, grid_pos_x, grid_pos_y, checkable,
                   checked, hidden, focus):
 
     button = INIT_WIDGET(ID, QPushButton(button_text))
 
-    set_grid(lyt, grid, button, grid_pos_x, grid_pos_y)
+    set_widget(lyt, grid, button, grid_pos_x, grid_pos_y)
     set_size_policy(button, sizepolicy)
 
     button.setIcon(QIcon(icon))
     button.setEnabled(not disabled)
     button.setDefault(default)
     button.setCheckable(checkable)
     button.setChecked(checked)
@@ -142,15 +142,15 @@
 def window_input(lyt, placeholder, ID, value, type, disabled,
                  readonly, maxlength, hidden, font, fontsize, text_changed, return_pressed,
                  editing_finished, text_edited, selection_changed, sizepolicy, grid,
                  grid_pos_x, grid_pos_y,):
 
     input = INIT_WIDGET(ID, QLineEdit())
 
-    set_grid(lyt, grid, input, grid_pos_x, grid_pos_y)
+    set_widget(lyt, grid, input, grid_pos_x, grid_pos_y)
     set_size_policy(input, sizepolicy)
 
     if fontsize != None:
         input.setFont(QFont(font, fontsize))
     else:
         input.setFont(QFont(font))
 
@@ -235,15 +235,15 @@
 
 
 def window_text(lyt, text, ID, link, hovered, clicked, buddy, alignment, word_wrap,
                 sizepolicy, grid, grid_pos_x, grid_pos_y, hidden):
 
     label = INIT_WIDGET(ID, QLabel(text))
 
-    set_grid(lyt, grid, label, grid_pos_x, grid_pos_y)
+    set_widget(lyt, grid, label, grid_pos_x, grid_pos_y)
     set_size_policy(label, sizepolicy)
 
     if link != None:
         anchor = f'<a href="{link}">{text}</a>'
         label.setText(anchor)
         label.linkActivated.connect(clicked)
         label.linkHovered.connect(hovered)
@@ -303,15 +303,15 @@
 # ------------------------------------------------------------------------#
 
 
 def window_image(lyt, image, ID, size, alignment, hidden, sizepolicy, grid, grid_pos_x, grid_pos_y,):
 
     img = INIT_WIDGET(ID, QLabel())
 
-    set_grid(lyt, grid, img, grid_pos_x, grid_pos_y)
+    set_widget(lyt, grid, img, grid_pos_x, grid_pos_y)
     set_size_policy(img, sizepolicy)
 
     if image != None:
         pixmap = QPixmap(get_path(image))
 
         if type(size) == sample_integer:
             pixmap = pixmap.scaledToWidth(size)
@@ -368,15 +368,15 @@
 
 
 def window_checkbox(lyt, name, checked, ID, state_changed, toggled, sizepolicy,
                     grid, grid_pos_x, grid_pos_y,):
 
     checkbox = INIT_WIDGET(ID, QCheckBox(name))
 
-    set_grid(lyt, grid, checkbox, grid_pos_x, grid_pos_y)
+    set_widget(lyt, grid, checkbox, grid_pos_x, grid_pos_y)
     set_size_policy(checkbox, sizepolicy)
 
     checkbox.setChecked(checked)
     checkbox.stateChanged.connect(state_changed)
     checkbox.toggled.connect(toggled)
 
     return checkbox
@@ -421,15 +421,15 @@
 
 
 def window_radio_button(lyt, name, checked, ID, toggled, sizepolicy, grid,
                         grid_pos_x, grid_pos_y):
 
     radio_button = INIT_WIDGET(ID, QRadioButton(name))
 
-    set_grid(lyt, grid, radio_button, grid_pos_x, grid_pos_y)
+    set_widget(lyt, grid, radio_button, grid_pos_x, grid_pos_y)
     set_size_policy(radio_button, sizepolicy)
 
     radio_button.setChecked(checked)
     radio_button.toggled.connect(toggled)
 
     return radio_button
 
@@ -473,15 +473,15 @@
 
 def window_textarea(lyt, ID, placeholder, hidden, alignment, value, disabled, readonly, text_changed,
                     selection_changed, undo_available, redo_available, maxlength, font, fontsize,
                     sizepolicy, grid, grid_pos_x, grid_pos_y, tabWidth):
 
     textarea = INIT_WIDGET(ID, QTextEdit())
 
-    set_grid(lyt, grid, textarea, grid_pos_x, grid_pos_y)
+    set_widget(lyt, grid, textarea, grid_pos_x, grid_pos_y)
     set_size_policy(textarea, sizepolicy)
 
     textarea.setHidden(hidden)
 
     textarea.setDisabled(disabled)
     textarea.setReadOnly(readonly)
     textarea.setText(value)
@@ -558,15 +558,15 @@
 
 # ------------------------------------------------------------------------#
 
 
 def window_list_widget(lyt, list_items, ID, mode, grid, sizepolicy, grid_pos_x, grid_pos_y, func):
     list_widget = INIT_WIDGET(ID, QListWidget())
 
-    set_grid(lyt, grid, list_widget, grid_pos_x, grid_pos_y)
+    set_widget(lyt, grid, list_widget, grid_pos_x, grid_pos_y)
     set_size_policy(list_widget, sizepolicy)
 
     selection_modes = [
         [ITEM_SELECTION_MODE_NO_SELECTION, QAbstractItemView.NoSelection],
         [ITEM_SELECTION_MODE_SINGLE, QAbstractItemView.SingleSelection],
         [ITEM_SELECTION_MODE_MULTI, QAbstractItemView.MultiSelection],
         [ITEM_SELECTION_MODE_EXTENDED, QAbstractItemView.ExtendedSelection]
@@ -631,15 +631,15 @@
 
 # ------------------------------------------------------------------------#
 
 
 def window_select(lyt, options, ID, placeholder, grid, sizepolicy, grid_pos_x, grid_pos_y, current_text_changed, activated):
     select = INIT_WIDGET(ID, QComboBox())
 
-    set_grid(lyt, grid, select, grid_pos_x, grid_pos_y)
+    set_widget(lyt, grid, select, grid_pos_x, grid_pos_y)
     set_size_policy(select, sizepolicy)
 
     select.setPlaceholderText(placeholder)
 
     if options != None:
         if type(options[0]) == sample_string:
             options = [options]
@@ -690,15 +690,15 @@
 # ------------------------------------------------------------------------#
 
 
 def window_progress_bar(lyt, ID, minimum, maximum, value, orientation, grid,
                         sizepolicy, text_visible, inverted, value_changed, grid_pos_x, grid_pos_y):
     progress_bar = INIT_WIDGET(ID, QProgressBar())
 
-    set_grid(lyt, grid, progress_bar, grid_pos_x, grid_pos_y)
+    set_widget(lyt, grid, progress_bar, grid_pos_x, grid_pos_y)
     set_size_policy(progress_bar, sizepolicy)
 
     progress_bar.setRange(minimum, maximum)
 
     if value != None:
         progress_bar.setValue(value)
 
@@ -768,15 +768,15 @@
     elif orientation.lower() in DEFAULT_HORIZONTAL_TYPES:
         setOrientation = Qt.Horizontal
     else:
         raise ValueError(orientation)
 
     slider = INIT_WIDGET(ID, QSlider(setOrientation))
 
-    set_grid(lyt, grid, slider, grid_pos_x, grid_pos_y)
+    set_widget(lyt, grid, slider, grid_pos_x, grid_pos_y)
     set_size_policy(slider, sizepolicy)
 
     slider.setMinimum(min)
     slider.setMaximum(max)
 
     if value != None:
         slider.setValue(value)
@@ -829,15 +829,15 @@
 
 
 def window_dial(lyt, ID, min, max, value, tick_target, tick, wrapping, grid,
                 sizepolicy, value_changed, grid_pos_x, grid_pos_y):
 
     dial = INIT_WIDGET(ID, QDial())
 
-    set_grid(lyt, grid, dial, grid_pos_x, grid_pos_y)
+    set_widget(lyt, grid, dial, grid_pos_x, grid_pos_y)
     set_size_policy(dial, sizepolicy)
 
     dial.setMinimum(min)
     dial.setMaximum(max)
 
     if value != None:
         dial.setValue(value)
```

### Comparing `clera-0.0.6/setup.py` & `clera-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,39 +5,37 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as readme:
     with codecs.open(os.path.join(here, "CHANGELOG.md"), encoding="utf-8") as changelog:
         LONG_DESCRIPTION = readme.read() + '\n\n\n' + changelog.read()
 
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Write Simple and Quick Python GUI Application'
-KEYWORDS = ['gui', 'clera', 'simple', 'simplegui', 'pyside', 'pyside6']
+KEYWORDS = ['gui', 'clera', 'simple', 'simplegui', 'pyside', 'pyside6', 'python', 'easy']
 
-# LONG_DESCRIPTION = 'A package that allows to build simple streams of video, audio and camera data.'
 
 CLASSIFIERS = [
-    'Development Status :: 2 - Pre-Alpha',
+    'Development Status :: 3 - Alpha',
     'Environment :: Console',
     'Intended Audience :: Developers',
-    'License :: OSI Approved :: MIT License',
+    'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
     'Operating System :: OS Independent',
     'Programming Language :: Python :: 3',
 ]
 
 # Setting up
 setup(
     name="clera",
     version=VERSION,
     author="Erasmus A. Junior",
     author_email="eirasmx@pm.me",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
-    licence='MIT',
+    licence='GNU LGPLv3',
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=['PySide6'],
     keywords=KEYWORDS,
     classifiers=CLASSIFIERS,
     py_modules=['clera']
 )
-
```

