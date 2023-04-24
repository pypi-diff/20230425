# Comparing `tmp/cochleogram-0.1.7.tar.gz` & `tmp/cochleogram-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cochleogram-0.1.7.tar", last modified: Wed Apr 12 16:25:11 2023, max compression
+gzip compressed data, was "cochleogram-0.1.8.tar", last modified: Mon Apr 24 22:16:13 2023, max compression
```

## Comparing `cochleogram-0.1.7.tar` & `cochleogram-0.1.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:25:11.276329 cochleogram-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:25:11.272329 cochleogram-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:25:11.272329 cochleogram-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-12 16:24:59.000000 cochleogram-0.1.7/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-12 16:24:59.000000 cochleogram-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-12 16:25:11.276329 cochleogram-0.1.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:25:11.272329 cochleogram-0.1.7/cochleogram/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/gui.enaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:25:11.276329 cochleogram-0.1.7/cochleogram/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/icons/cells.png
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/icons/exclude.png
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/icons/main-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/icons/make_icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/icons/spiral.png
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/icons/tile.png
--rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    19656 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    26487 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/presenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-04-12 16:24:59.000000 cochleogram-0.1.7/cochleogram/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 16:25:11.000000 cochleogram-0.1.7/cochleogram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:25:11.276329 cochleogram-0.1.7/cochleogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-12 16:25:11.000000 cochleogram-0.1.7/cochleogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-12 16:25:11.000000 cochleogram-0.1.7/cochleogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:25:11.000000 cochleogram-0.1.7/cochleogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-12 16:25:11.000000 cochleogram-0.1.7/cochleogram.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 16:25:11.000000 cochleogram-0.1.7/cochleogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 16:25:11.000000 cochleogram-0.1.7/cochleogram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-12 16:24:59.000000 cochleogram-0.1.7/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-12 16:24:59.000000 cochleogram-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-12 16:24:59.000000 cochleogram-0.1.7/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 16:25:11.276329 cochleogram-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:13.679224 cochleogram-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:13.675224 cochleogram-0.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:13.675224 cochleogram-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-24 22:16:02.000000 cochleogram-0.1.8/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-24 22:16:02.000000 cochleogram-0.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-24 22:16:13.679224 cochleogram-0.1.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:13.675224 cochleogram-0.1.8/cochleogram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20160 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/gui.enaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:13.679224 cochleogram-0.1.8/cochleogram/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/icons/cells.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/icons/exclude.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/icons/main-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/icons/make_icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/icons/spiral.png
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/icons/tile.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26816 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/presenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-04-24 22:16:02.000000 cochleogram-0.1.8/cochleogram/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 22:16:13.000000 cochleogram-0.1.8/cochleogram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:13.679224 cochleogram-0.1.8/cochleogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-24 22:16:13.000000 cochleogram-0.1.8/cochleogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-24 22:16:13.000000 cochleogram-0.1.8/cochleogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 22:16:13.000000 cochleogram-0.1.8/cochleogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-24 22:16:13.000000 cochleogram-0.1.8/cochleogram.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 22:16:13.000000 cochleogram-0.1.8/cochleogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 22:16:13.000000 cochleogram-0.1.8/cochleogram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-24 22:16:02.000000 cochleogram-0.1.8/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-24 22:16:02.000000 cochleogram-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-24 22:16:02.000000 cochleogram-0.1.8/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 22:16:13.679224 cochleogram-0.1.8/setup.cfg
```

### Comparing `cochleogram-0.1.7/.github/workflows/publish-to-pypi.yml` & `cochleogram-0.1.8/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.7/.gitignore` & `cochleogram-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.7/PKG-INFO` & `cochleogram-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.1.7
+Version: 0.1.8
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: czi
 Provides-Extra: lif
```

### Comparing `cochleogram-0.1.7/cochleogram/gui.enaml` & `cochleogram-0.1.8/cochleogram/gui.enaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 log = logging.getLogger(__name__)
 
 from importlib import resources
 
 from enaml.application import deferred_call
-from enaml.core.api import Looper
+from enaml.core.api import Conditional, Looper
 from enaml.icon import Icon, IconImage
 from enaml.image import Image
 from enaml.layout.api import align, hbox, InsertTab, RemoveItem, spacer, TabLayout, vbox
 from enaml.stdlib.fields import FloatField
 from enaml.stdlib.message_box import critical, information, question
 from enaml.qt.QtCore import Qt
 from enaml.widgets.api import (Action, ButtonGroup, CheckBox, Container,
@@ -97,14 +97,15 @@
         if button is None or button.text == 'No':
             return
     for presenter in presenters:
         try:
             presenter.load_state()
             information(parent, 'Analysis loaded', 'Analysis has been loaded.')
         except Exception as e:
+            log.exception(e)
             information(parent, 'Error', str(e))
 
 
 CELLS = ['IHC', 'OHC1', 'OHC2', 'OHC3', 'Extra']
 
 
 class CochleogramCanvas(MPLCanvas):
@@ -264,26 +265,31 @@
 
         PushButton: action_clear_cells:
             text = 'Clear all cells'
             enabled << presenter.current_cells_artist is not None and presenter.current_cells_artist.has_nodes
             clicked ::
                 button = question(self, 'Confirm action', 'Are you sure you want to remove the current cells?')
                 if button is not None and button.text == 'Yes':
-                    presenter.action_clear_cells()
+                    try:
+                        presenter.action_clear_cells()
+                    except Exception as e:
+                        log.exception(e)
+                        information(self, 'Error', str(e))
 
         PushButton: action_simplify_exclusions:
             text = 'Simplify exclusions'
             enabled << presenter.current_spiral_artist is not None and presenter.current_spiral_artist.has_exclusion
             clicked ::
                 m = f'Are you sure you want to simplify the excluded regions?'
                 button = question(self, 'Confirm action', m)
                 if button is not None and button.text == 'Yes':
                     try:
                         presenter.action_simplify_exclusion(presenter.cells)
                     except Exception as e:
+                        log.exception(e)
                         information(self, 'Error', str(e))
 
         PushButton: action_merge_ohc_exclusions:
             text = 'Combine OHC exclusions'
             enabled << presenter.point_artists['OHC1', 'spiral'].has_spline and \
                 presenter.point_artists['OHC2', 'spiral'].has_spline and \
                 presenter.point_artists['OHC3', 'spiral'].has_spline and (\
@@ -295,14 +301,15 @@
                 m = f'Are you sure you want to merge all OHC excluded regions together?\n' \
                     'This will also simplify the excluded regions.'
                 button = question(self, 'Confirm action', m)
                 if button is not None and button.text == 'Yes':
                     try:
                         presenter.action_merge_exclusion('OHC1', 'OHC2', 'OHC3')
                     except Exception as e:
+                        log.exception(e)
                         information(self, 'Error', str(e))
 
         PushButton: load_analysis:
             text = 'Load'
             clicked ::
                 load_state(self, [presenter])
 
@@ -332,18 +339,22 @@
                 selected << items[0]
 
             PushButton:
                 text = 'update'
                 clicked ::
                     button = question(self, 'Confirm action', f'Are you sure you want to overwrite the existing cells?')
                     if button is not None and button.text == 'Yes':
-                        n = presenter.action_guess_cells(guess_width.value,
-                                                         guess_spacing.value,
-                                                         guess_channel.selected)
-                        information(self, 'Info', f'Found {n} cells')
+                        try:
+                            n = presenter.action_guess_cells(guess_width.value,
+                                                            guess_spacing.value,
+                                                            guess_channel.selected)
+                            information(self, 'Info', f'Found {n} cells')
+                        except Exception as e:
+                            log.exception(e)
+                            information(self, 'Error', str(e))
 
         HGroup: action_copy_exclusion:
             padding = 0
             align_widths = False
             trailing_spacer = spacer(0)
             enabled << presenter.current_spiral_artist is not None and presenter.current_spiral_artist.has_exclusion
             Label:
@@ -356,14 +367,15 @@
                     m = f'Are you sure you want to copy the excluded regions to {copy_exclusion_to.selected}?\n' \
                         f'The exclusion regions will be merged with any already-defined regions on {copy_exclusion_to.selected}.'
                     button = question(self, 'Confirm action', m)
                     if button is not None and button.text == 'Yes':
                         try:
                             presenter.action_copy_exclusion(copy_exclusion_to.selected)
                         except Exception as e:
+                            log.exception(e)
                             information(self, 'Error', str(e))
 
         CochleogramCanvas: canvas:
             figure << presenter.figure
             toolbar_visible = False
             initialized ::
                 deferred_call(bind, figure, presenter)
@@ -383,14 +395,56 @@
         PushButton:
             text = 'Ok'
             enabled << (pb.value == pb.maximum)
             clicked ::
                 window.close()
 
 
+enamldef CompositeWindow(Window):
+
+    modality = 'application_modal'
+    title = 'Generate Composite'
+    attr cochlea
+    attr channels = cochlea.channel_names
+
+    Container:
+        CheckBox: include_freq_map:
+            text = 'Include frequency map?'
+            visible << cochlea.ihc_spiral_complete()
+            checked << visible
+        Label:
+            text = 'Cannot include frequency map because IHC spiral incomplete.'
+            visible << not include_freq_map.visible
+        Label:
+            text = 'Channels to include'
+        Looper:
+            iterable << cochlea.channel_names
+            CheckBox:
+                text = loop_item
+                checked = True
+                checked ::
+                    if checked:
+                        channels.append(loop_item)
+                    else:
+                        channels.remove(loop_item)
+
+        PushButton:
+            text = 'Generate'
+            enabled << len(channels) != 0
+            clicked ::
+                try:
+                    fig = plot.plot_composite(cochlea, include_freq_map=include_freq_map.checked)
+                    fig.suptitle(cochlea.name)
+                    fig.savefig(cochlea.path / f'{cochlea.name}_frequency_map.pdf')
+                    information(self, 'Composite', 'Composite has been generated.')
+                except Exception as e:
+                    log.exception(e)
+                    critical(self, 'Composite', str(e))
+
+
 enamldef CochleagramWindow(MainWindow): window:
 
     initial_size = (900, 900)
     title = 'Cochelogram'
     icon = load_icon('main-icon')
 
     attr cochlea
@@ -435,25 +489,19 @@
                 triggered ::
                     load_state(window, window.presenters)
 
             Action:
                 separator = True
 
             Action:
-                text = 'Generate frequency map\tCtrl+F'
+                text = 'Generate composite (frequency map)\tCtrl+F'
                 enabled << cochlea is not None
                 triggered ::
-                    try:
-                        fig = plot.frequency_map(cochlea)
-                        fig.suptitle(cochlea.name)
-                        fig.savefig(cochlea.path / f'{cochlea.name}_frequency_map.pdf')
-                        information(window, 'Frequency map', 'Frequency map has been generated.')
-                    except Exception as e:
-                        log.exception(e)
-                        critical(window, 'Frequency map', str(e))
+                    window = CompositeWindow(cochlea=cochlea)
+                    window.show()
 
     initialized ::
         for presenter in presenters:
             deferred_call(add_dock_item, workspace, presenter)
 
     closing ::
         if any(p.unsaved_changes for p in presenters):
```

### Comparing `cochleogram-0.1.7/cochleogram/icons/cells.png` & `cochleogram-0.1.8/cochleogram/icons/cells.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.7/cochleogram/icons/exclude.png` & `cochleogram-0.1.8/cochleogram/icons/exclude.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.7/cochleogram/icons/main-icon.png` & `cochleogram-0.1.8/cochleogram/icons/main-icon.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.7/cochleogram/icons/make_icons.py` & `cochleogram-0.1.8/cochleogram/icons/make_icons.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.7/cochleogram/icons/spiral.png` & `cochleogram-0.1.8/cochleogram/icons/spiral.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.7/cochleogram/icons/tile.png` & `cochleogram-0.1.8/cochleogram/icons/tile.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.7/cochleogram/instructions.html` & `cochleogram-0.1.8/cochleogram/instructions.html`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.7/cochleogram/main.py` & `cochleogram-0.1.8/cochleogram/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 from pathlib import Path
 
 from enaml.application import deferred_call
 from enaml.qt.QtCore import QStandardPaths
 
 from cochleogram.model import Piece
-from cochleogram.util import list_lif_stacks, list_pieces, load_lif, load_czi
+from cochleogram.util import list_lif_stacks, list_pieces, load_lif, load_czi, process_lif
 
 
 def config_file():
     config_path = Path(QStandardPaths.standardLocations(QStandardPaths.AppConfigLocation)[0])
     config_file =  config_path / 'cochleogram' / 'config.ini'
     config_file.parent.mkdir(exist_ok=True, parents=True)
     return config_file
@@ -48,15 +48,15 @@
 
 def main_prepare_lif():
     parser = argparse.ArgumentParser('Create cached files for cochleogram from LIF files')
     parser.add_argument('path')
     parser.add_argument('--reprocess', action='store_true')
     args = parser.parse_args()
     filename = Path(args.path)
-    util.process_lif(filename, args.reprocess)
+    process_lif(filename, args.reprocess)
 
 
 def main():
     import enaml
     from enaml.qt.qt_application import QtApplication
     logging.basicConfig(level='INFO')
```

### Comparing `cochleogram-0.1.7/cochleogram/model.py` & `cochleogram-0.1.8/cochleogram/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import json
 from pathlib import Path
 import pickle
 import re
 
 from atom.api import Atom, Dict, Event, Float, Int, List, Typed
 from matplotlib import colors
+from matplotlib import transforms as T
 import numpy as np
 import pandas as pd
 
 from psiaudio.util import octave_space
 from scipy import interpolate
 from scipy import ndimage
 from scipy import signal
@@ -229,15 +230,14 @@
 
 class Tile(Atom):
 
     info = Dict()
     image = Typed(np.ndarray)
     source = Typed(Path)
     extent = List()
-    voxel_size = Float()
     n_channels = Int()
 
     def __init__(self, info, image, source):
         self.info = info
         self.image = image
         self.source = source
         xlb, ylb, zlb = self.info["lower"][:3]
@@ -299,23 +299,65 @@
 
     def nuclei_template(self, radius=2.5):
         voxel_size = self.info["voxel_size"][0]
         pixel_radius = int(np.round(radius / voxel_size))
         template = sphere(pixel_radius * 3, pixel_radius)
         return template / template.sum()
 
-    def get_image_extent(self):
-        # This flips the x and y extents. Seems necessary to make things work
-        # for the Leica SP5.
-        #return tuple(self.extent[2:4] + self.extent[0:2])
-        return tuple(self.extent[:4])
+    def get_image_extent(self, axis='z', norm=False):
+        e = np.array(self.extent).reshape((3, 2))
+        if norm:
+            e = e - e[:, [0]]
+        extent = e.ravel().tolist()
+        x = extent[0:2]
+        y = extent[2:4]
+        z = extent[4:6]
+        if axis == 'x':
+            return tuple(y + z)
+        if axis == 'y':
+            return tuple(x + z)
+        if axis == 'z':
+            return tuple(x + y)
+
+    def get_image_transform(self):
+        return T.Affine2D().rotate_deg_around(*self.get_image_center(),
+                                              self.get_rotation())
+
+    def get_rotated_extent(self):
+        '''
+        Calculate the new extents of the tile after rotation.
+
+        This assumes that the tile is rotated using scipy.ndimage where the
+        resulting array is reshaped to ensure that the input image is contained
+        entirely in the output image.
+        '''
+        e = self.extent[:]
+        ll = e[0], e[2]
+        lr = e[1], e[2]
+        ul = e[0], e[3]
+        ur = e[1], e[3]
+        coords = np.array([ll, lr, ur, ul, ll])
+        t_coords = self.get_image_transform().transform(coords)
+        xlb, ylb = t_coords.min(axis=0)
+        xub, yub = t_coords.max(axis=0)
+        e[:4] = xlb, xub, ylb, yub
+        return e
+
+    def get_image_center(self, axis='z', norm=False):
+        extent = self.get_image_extent()
+        center = np.array(extent).reshape((2, 2)).mean(axis=1)
+        return tuple(center)
 
-    def get_image(self, channel=None, z_slice=None):
+    def get_rotation(self):
+        return self.info.get('rotation', 0)
+
+    def get_image(self, channel=None, z_slice=None, axis='z',
+                  norm_percentile=99):
         if z_slice is None:
-            data = self.image.max(axis=2)
+            data = self.image.max(axis='xyz'.index(axis))
         else:
             data = self.image[:, :, z_slice, :]
 
         x, y = data.shape[:2]
         image = []
         for c, c_info in enumerate(self.info['channels']):
             if isinstance(channel, int):
@@ -323,15 +365,17 @@
             if channel is None or channel == 'All' or c_info['name'] == channel:
                 color = c_info['display_color']
                 rgb = colors.to_rgba(color)[:3]
                 image.append(data[..., c][..., np.newaxis] * rgb)
         if len(image) == 0:
             raise ValueError(f'Channel {channel} does not exist')
         image = np.concatenate([i[np.newaxis] for i in image]).max(axis=0)
-        return image / image.max(axis=(0, 1), keepdims=True)
+        image_max =  np.percentile(image, norm_percentile, axis=(0, 1), keepdims=True)
+        image_mask = image_max != 0
+        return np.divide(image, image_max, where=image_mask).clip(0, 1)
 
     def get_state(self):
         return {"extent": self.extent}
 
     def set_state(self, state):
         self.extent = state["extent"]
 
@@ -425,38 +469,47 @@
         xmin = extents[:, 0].min()
         xmax = extents[:, 1].max()
         ymin = extents[:, 2].min()
         ymax = extents[:, 3].max()
         return [xmin, xmax, ymin, ymax]
 
     def merge_tiles(self):
-        merged_lb = np.vstack([t.extent[::2] for t in self.tiles]).min(axis=0)
-        merged_ub = np.vstack([t.extent[1::2] for t in self.tiles]).max(axis=0)
-        voxel_size = self.tiles[0].info["voxel_size"]
+        '''
+        Merges the information from the tiles into one single tile representing the piece
 
+        This is typically used when we need to do analyses that function across
+        the individual tiles.
+        '''
+        merged_lb = np.vstack([t.get_rotated_extent()[::2] for t in self.tiles]).min(axis=0)
+        merged_ub = np.vstack([t.get_rotated_extent()[1::2] for t in self.tiles]).max(axis=0)
+        voxel_size = self.tiles[0].info["voxel_size"]
         lb_pixels = np.floor(merged_lb / voxel_size).astype("i")
         ub_pixels = np.ceil(merged_ub / voxel_size).astype("i")
         extent_pixels = ub_pixels - lb_pixels
-        shape = extent_pixels.tolist() + [self.tiles[0].n_channels]
-        merged_image = np.full(shape, fill_value=0, dtype=int)
+        shape = [len(self.tiles)] + extent_pixels.tolist() + [self.tiles[0].n_channels]
+        merged_image = np.full(shape, fill_value=np.nan, dtype=float)
 
-        for tile in self.tiles:
-            tile_lb = tile.extent[::2]
+        for i, tile in enumerate(self.tiles):
+            img = ndimage.rotate(tile.image, tile.get_rotation(), cval=np.nan)
+            tile_lb = tile.get_rotated_extent()[::2]
             tile_lb = np.round((tile_lb - merged_lb) / voxel_size).astype("i")
-            tile_ub = tile_lb + tile.image.shape[:-1]
-            s = tuple(np.s_[lb:ub] for lb, ub in zip(tile_lb, tile_ub))
-            merged_image[s] = tile.image
+            tile_ub = tile_lb + img.shape[:-1]
+            s = tuple([i] + [np.s_[lb:ub] for lb, ub in zip(tile_lb, tile_ub)])
+            merged_image[s] = img
+
+        merged_image = np.nan_to_num(np.nanmean(merged_image, axis=0)).astype('i')
 
         info = {
             "lower": merged_lb,
             "voxel_size": voxel_size,
+            "rotation": 0,
         }
 
         t_base = self.tiles[0]
-        extra_keys = set(t_base.info.keys()) - set(('lower', 'voxel_size'))
+        extra_keys = set(t_base.info.keys()) - set(('lower', 'voxel_size', 'rotation'))
         for k in extra_keys:
             for t in self.tiles[1:]:
                 if t_base.info[k] != t.info[k]:
                     raise ValueError(f'Cannot merge tiles. {k} differs.')
             info[k] = t_base.info[k]
         return Tile(info, merged_image, self.path)
 
@@ -519,16 +572,33 @@
     @classmethod
     def from_path(cls, path):
         log.info('Loading cochlea from %s', path)
         path = Path(path)
         pieces = [Piece.from_path(path, p) for p in util.list_pieces(path)]
         return cls(pieces, path)
 
+    @property
+    def channel_names(self):
+        # We assume that each tile has the same set of channels
+        names = set()
+        for piece in self.pieces:
+            names.update(piece.channel_names)
+        return sorted(names)
+
+    def ihc_spiral_complete(self):
+        for piece in self.pieces:
+            s = piece.spirals['IHC']
+            x, y = s.interpolate(resolution=0.001)
+            if len(x) == 0:
+                return False
+        return True
+
     def make_frequency_map(self, freq_start=4, freq_end=64, freq_step=0.5,
-                           species='mouse', spiral='IHC'):
+                           species='mouse', spiral='IHC',
+                           include_extremes=True):
         # First, we need to merge the spirals
         xo, yo = 0, 0
         results = []
         for piece in self.pieces:
             s = piece.spirals[spiral]
             x, y = s.interpolate(resolution=0.001)
             if len(x) == 0:
@@ -556,8 +626,14 @@
         results['distance_norm'] = results['distance_mm'] / results['distance_mm'].max()
         results['frequency'] = freq_fn[species](results['distance_norm'])
 
         info = {}
         for freq in octave_space(freq_start, freq_end, freq_step):
             idx = (results['frequency'] - freq).abs().idxmin()
             info[freq] = results.loc[idx].to_dict()
+
+        if include_extremes:
+            for ix in (0, -1):
+                row = results.iloc[ix].to_dict()
+                info[row['frequency']] = row
+
         return info
```

### Comparing `cochleogram-0.1.7/cochleogram/plot.py` & `cochleogram-0.1.8/cochleogram/plot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,66 @@
 from matplotlib import pyplot as plt
 from matplotlib import patheffects as path_effects
+from matplotlib import transforms
 
 
-def _plot_piece(ax, piece, xo, yo, xmax, ymax, freq_map):
+def _plot_piece(ax, piece, xo, yo, xmax, ymax, freq_map=None):
     tile = piece.merge_tiles()
     img = tile.get_image()
     extent = tile.get_image_extent()
     xr = extent[0] - xo
     yr = extent[2] - yo
     xe = extent[1] - extent[0]
     ye = extent[3] - extent[2]
     extent = (xo, xo+xe, yo, yo+ye)
-    ax.imshow(img.swapaxes(0, 1), origin='lower', extent=extent)
+    t = tile.get_image_transform() + ax.transData
+    ax.imshow(img.swapaxes(0, 1), origin='lower', extent=extent, transform=t)
     xo += xe
     ymax = max(ymax, yo+ye)
     xmax = max(xmax, xo)
-    for freq, freq_df in freq_map.items():
-        if freq_df['piece'] != piece.piece:
-            continue
-        x = freq_df['x_orig']
-        y = freq_df['y_orig']
-        f = f'{freq:.1f}'
-        plt.plot(x-xr, y-yr, 'ko', mec='w', mew=2)
-        t = plt.annotate(f, (x-xr, y-yr), (5, 5), color='white', textcoords='offset points')
-        t.set_path_effects([
-            path_effects.Stroke(linewidth=3, foreground='black'),
-            path_effects.Normal(),
-        ])
+
+    if freq_map is not None:
+        for freq, freq_df in freq_map.items():
+            if freq_df['piece'] != piece.piece:
+                continue
+            x = freq_df['x_orig']
+            y = freq_df['y_orig']
+            f = f'{freq:.1f}'
+            ax.plot(x-xr, y-yr, 'ko', mec='w', mew=2)
+            t = ax.annotate(f, (x-xr, y-yr), (5, 5), color='white', textcoords='offset points')
+            t.set_path_effects([
+                path_effects.Stroke(linewidth=3, foreground='black'),
+                path_effects.Normal(),
+            ])
+
     return xo, yo, xmax, ymax
 
 
-def frequency_map(cochlea):
+def plot_composite(cochlea, include_freq_map=True):
     figure, ax = plt.subplots(1, 1, figsize=(11, 8.5))
-    freq_map = cochlea.make_frequency_map()
+    if include_freq_map:
+        freq_map = cochlea.make_frequency_map()
+    else:
+        freq_map = None
 
     xo, yo = 0, 0
     xmax, ymax = 0, 0
     for piece in cochlea.pieces[:3]:
         xo, yo, xmax, ymax = _plot_piece(ax, piece, xo, yo, xmax, ymax, freq_map)
     xo, yo = 0, ymax
     for piece in cochlea.pieces[3:]:
         xo, yo, xmax, ymax = _plot_piece(ax, piece, xo, yo, xmax, ymax, freq_map)
     ax.set_facecolor('k')
     ax.axis([0, xmax, 0, ymax])
     ax.set_xticks([])
     ax.set_yticks([])
 
     figure.subplots_adjust(left=0.025, right=0.975, top=0.95, bottom=0.025)
-
     return figure
+
+
+def plot_tile(ax, tile):
+    ax.imshow(tile.get_image().swapaxes(0, 1),
+              origin='lower',
+              aspect='equal',
+              transform=tile.get_image_transform() + ax.transData,
+              extent=tile.get_image_extent())
```

### Comparing `cochleogram-0.1.7/cochleogram/presenter.py` & `cochleogram-0.1.8/cochleogram/presenter.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from matplotlib.figure import Figure
 from matplotlib import (
     patheffects,
     ticker,
 )
 from matplotlib import patches as mpatches
 from matplotlib import path as mpath
+from matplotlib import transforms as T
 
 import numpy as np
 from scipy import interpolate
 
 from cochleogram.model import Piece, Points, Tile
 from cochleogram.util import get_region, make_plot_path, shortest_path
 
@@ -208,14 +209,16 @@
     z_slice_max = Int(0)
     shift = Float()
 
     tile = Typed(Tile)
     artist = Value()
     rectangle = Value()
     axes = Value()
+    rotation_transform = Value()
+    transform = Value()
 
     updated = Event()
     needs_redraw = Bool(False)
 
     def get_state(self):
         return {
             "alpha": self.alpha,
@@ -240,16 +243,18 @@
 
     def __init__(self, axes, tile, **kwargs):
         super().__init__(**kwargs)
         self.tile = tile
         self.axes = axes
         self.axes.xaxis.set_major_locator(ticker.NullLocator())
         self.axes.yaxis.set_major_locator(ticker.NullLocator())
-        self.artist = axes.imshow(np.array([[0, 1], [0, 1]]), origin="lower")
-        self.rectangle = mp.patches.Rectangle((0, 0), 0, 0, ec='red', fc='None', zorder=5000)
+        self.rotation_transform = T.Affine2D()
+        self.transform = self.rotation_transform + axes.transData
+        self.artist = axes.imshow(np.array([[0, 1], [0, 1]]), origin="lower", transform=self.transform)
+        self.rectangle = mp.patches.Rectangle((0, 0), 0, 0, ec='red', fc='None', zorder=5000, transform=self.transform)
         self.rectangle.set_alpha(0)
         self.axes.add_patch(self.rectangle)
         self.z_slice_max = self.tile.image.shape[2] - 1
         self.z_slice = self.tile.image.shape[2] // 2
         self.shift = self.tile.info["voxel_size"][0] * 5
         tile.observe('extent', self.request_redraw)
 
@@ -298,14 +303,17 @@
         z_slice = None if self.display_mode == 'projection' else self.z_slice
         image = self.tile.get_image(channel=self.display_channel,
                                     z_slice=z_slice).swapaxes(0, 1)
         self.artist.set_data(image)
         xlb, xub, ylb, yub = extent = self.tile.get_image_extent()[:4]
         self.artist.set_extent(extent)
         self.rectangle.set_bounds(xlb, ylb, xub-xlb, yub-ylb)
+
+        t = self.tile.get_image_transform()
+        self.rotation_transform.set_matrix(t.get_matrix())
         self.updated = True
 
     def contains(self, x, y):
         return self.tile.contains(x, y)
 
 
 class Presenter(Atom):
@@ -521,18 +529,18 @@
                 self.current_artist.move_image(event.key)
         elif event.key in ["shift+right", "shift+left", "shift+up", "shift+down"]:
             if self.current_artist is not None:
                 self.current_artist.move_image(event.key.split('+')[1], 0.25)
 
         elif event.key.lower() == "n":
             i = -1 if self.current_artist_index is None else self.current_artist_index
-            self.current_artist_index = int(np.clip(i + 1, 0, len(self.tile_artists) - 1))
+            self.current_artist_index = (i + 1) % len(self.tile_artists)
         elif event.key.lower() == "p":
             i = len(self.tile_artists) + 1 if self.current_artist_index is None else self.current_artist_index
-            self.current_artist_index = int(np.clip(i - 1, 0, len(self.tile_artists) - 1))
+            self.current_artist_index = (i - 1) % len(self.tile_artists)
 
     def key_press_point_plot(self, event):
         if event.key.startswith('shift+'):
             direction = event.key.split('+')[1]
             scale = 0.025
         else:
             direction = event.key
```

### Comparing `cochleogram-0.1.7/cochleogram/util.py` & `cochleogram-0.1.8/cochleogram/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,16 +59,16 @@
     dx = width * np.cos(a)
     dy = width * np.sin(a)
     x = np.linspace(x - dx, x + dx, 100)
     y = np.linspace(y - dy, y + dy, 100)
     return x, y
 
 
-def find_nuclei(x, y, i, spacing=5, prominence=1):
-    xy_delta = np.mean(np.sqrt(np.diff(x) ** 2 + np.diff(y) ** 2))
+def find_nuclei(x, y, i, spacing=5, prominence=None):
+    xy_delta = np.median(np.sqrt(np.diff(x) ** 2 + np.diff(y) ** 2))
     distance = np.floor(spacing / xy_delta)
     p, _ = signal.find_peaks(i, distance=distance, prominence=prominence)
     return x[p], y[p]
 
 
 def find_centroid(x, y, image, rx, ry, factor=4):
     x_center, y_center = [], []
@@ -137,14 +137,19 @@
     node = root.find(f'.//Element[@Name="{piece}"]')
 
     y_pos = float(node.find('.//FilterSettingRecord[@Attribute="XPos"]').attrib['Variant'])
     x_pos = float(node.find('.//FilterSettingRecord[@Attribute="YPos"]').attrib['Variant'])
     # This seems to work for the Z-axis.
     z_pos = float(node.find('.//DimensionDescription[@DimID="3"]').attrib['Origin'])
 
+    rot = float(node.find('.//FilterSettingRecord[@Attribute="Scan Rotation"]').attrib['Variant'])
+    rot_dir = float(node.find('.//FilterSettingRecord[@Attribute="Rotation Direction"]').attrib['Variant'])
+    if rot_dir != 1:
+        raise ValueError('Rotation direction is unexpected')
+
     system_number = node.find('.//FilterSettingRecord[@Attribute="System_Number"]').attrib['Variant']
     system_type = node.find('.//ScannerSettingRecord[@Identifier="SystemType"]').attrib['Variant']
     system = f'{system_type} {system_number}'
 
     pixels = np.array(stack.dims[:3])
     voxel_size = 1 / np.array(stack.scale[:3])
     lower = np.array([x_pos, y_pos, z_pos]) * 1e6
@@ -185,14 +190,15 @@
         # Reader used to read in data
         'reader': 'lif',
         # System used. I am including this information just in case we have to
         # implement specific tweaks for each confocal system we use.
         'system': system,
         'note': 'XY position from stage coords seem to be swapped',
         'channels': channels,
+        'rotation': rot,
     }
 
     # Rescale to range 0 ... 1
     img = img / img.max(axis=(0, 1, 2), keepdims=True)
     if 'int' in dtype:
         img *= 255
```

### Comparing `cochleogram-0.1.7/cochleogram.egg-info/PKG-INFO` & `cochleogram-0.1.8/cochleogram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.1.7
+Version: 0.1.8
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: czi
 Provides-Extra: lif
```

### Comparing `cochleogram-0.1.7/cochleogram.egg-info/SOURCES.txt` & `cochleogram-0.1.8/cochleogram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.7/pyproject.toml` & `cochleogram-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.1.7/readme.rst` & `cochleogram-0.1.8/readme.rst`

 * *Files identical despite different names*

