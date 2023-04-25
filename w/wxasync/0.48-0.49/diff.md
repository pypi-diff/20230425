# Comparing `tmp/wxasync-0.48.tar.gz` & `tmp/wxasync-0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxasync-0.48.tar", last modified: Fri Nov 25 09:02:16 2022, max compression
+gzip compressed data, was "wxasync-0.49.tar", last modified: Tue Apr 25 08:09:31 2023, max compression
```

## Comparing `wxasync-0.48.tar` & `wxasync-0.49.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 09:02:16.481386 wxasync-0.48/
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2022-11-25 09:02:07.000000 wxasync-0.48/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      308 2022-11-25 09:02:16.481386 wxasync-0.48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3779 2022-11-25 09:02:07.000000 wxasync-0.48/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-25 09:02:16.481386 wxasync-0.48/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      521 2022-11-25 09:02:07.000000 wxasync-0.48/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 09:02:16.481386 wxasync-0.48/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 09:02:16.481386 wxasync-0.48/src/wxasync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      308 2022-11-25 09:02:16.000000 wxasync-0.48/src/wxasync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      264 2022-11-25 09:02:16.000000 wxasync-0.48/src/wxasync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-25 09:02:16.000000 wxasync-0.48/src/wxasync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2022-11-25 09:02:16.000000 wxasync-0.48/src/wxasync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2022-11-25 09:02:16.000000 wxasync-0.48/src/wxasync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-25 09:02:16.000000 wxasync-0.48/src/wxasync.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     7093 2022-11-25 09:02:07.000000 wxasync-0.48/src/wxasync.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 09:02:16.481386 wxasync-0.48/test/
--rw-r--r--   0 runner    (1001) docker     (122)    20514 2022-11-25 09:02:07.000000 wxasync-0.48/test/test_perfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:09:31.144590 wxasync-0.49/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-25 08:09:13.000000 wxasync-0.49/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-25 08:09:31.144590 wxasync-0.49/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-25 08:09:13.000000 wxasync-0.49/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:09:31.144590 wxasync-0.49/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-25 08:09:13.000000 wxasync-0.49/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:09:31.140590 wxasync-0.49/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:09:31.144590 wxasync-0.49/src/wxasync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-25 08:09:31.000000 wxasync-0.49/src/wxasync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-25 08:09:31.000000 wxasync-0.49/src/wxasync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:09:31.000000 wxasync-0.49/src/wxasync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 08:09:31.000000 wxasync-0.49/src/wxasync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 08:09:31.000000 wxasync-0.49/src/wxasync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:09:30.000000 wxasync-0.49/src/wxasync.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-04-25 08:09:13.000000 wxasync-0.49/src/wxasync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:09:31.144590 wxasync-0.49/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    20514 2023-04-25 08:09:13.000000 wxasync-0.49/test/test_perfs.py
```

### Comparing `wxasync-0.48/LICENSE` & `wxasync-0.49/LICENSE`

 * *Files identical despite different names*

### Comparing `wxasync-0.48/README.md` & `wxasync-0.49/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # wxasync
 ## asyncio support for wxpython
 
 wxasync it a library for using python 3 asyncio (async/await) with wxpython.
- It does GUI message polling every 5ms and runs the asyncio message loop the rest of the time. 
- The polling doesn't have a noticable effect on CPU usage (still 0% when idle). 
+ The library polls UI messages every 20ms and runs the asyncio message loop the rest of the time. 
+ When idle, the CPU usage is 0% on windows and about 1-2% on MacOS. 
 
 ### Installation
 wxasync requires python 3.7. For earlier versions of python use wxasync 0.45.
 
 Install using: 
 ```sh
 pip install wxasync
@@ -33,15 +33,15 @@
 ```
 task = StartCoroutine(update_clock_coroutine, frame)
 ```
 If you need to stop it run:
 ```
 task.cancel()
 ```
-Any coroutine started using **AsyncBind** or using **StartCoroutine** is attached to a wx Window. It is automatically cancelled when the Window is destroyed. This makes it easier to use, as you don't need to take care of cancelling them yourselve. 
+Any coroutine started using **AsyncBind** or using **StartCoroutine** is attached to a wx.Window. It is automatically cancelled when the Window is destroyed. This makes it easier to use, as you don't need to take care of cancelling them yourselve. 
 
 To show a Dialog, use **AsyncShowDialog** or **AsyncShowDialogModal**. This allows
 to use 'await' to wait until the dialog completes. Don't use dlg.ShowModal() directly as it would block the event loop.
 
 You start the application using:
 ```python
 await app.MainLoop()
@@ -49,15 +49,14 @@
 
 Below is full example with AsyncBind, WxAsyncApp, and StartCoroutine:
 
 ```python
 import wx
 from wxasync import AsyncBind, WxAsyncApp, StartCoroutine
 import asyncio
-from asyncio.events import get_event_loop
 import time
 
 
 class TestFrame(wx.Frame):
     def __init__(self, parent=None):
         super(TestFrame, self).__init__(parent)
         vbox = wx.BoxSizer(wx.VERTICAL)
```

### Comparing `wxasync-0.48/setup.py` & `wxasync-0.49/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='wxasync',
-      version='0.48',
+      version='0.49',
       description='asyncio for wxpython',
       long_description='wxasync it a library for using python 3 asyncio (async/await) with wxpython.',
       url='http://github.com/sirk390/wxasync',
       author='C.Bodt',
       author_email='sirk390@gmail.com',
       license='MIT',
       package_dir={'': 'src'},
```

### Comparing `wxasync-0.48/src/wxasync.py` & `wxasync-0.49/src/wxasync.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,37 +11,43 @@
 from wx._html import HtmlHelpDialog
 from wx._adv import PropertySheetDialog
 
 
 IS_MAC = platform.system() == "Darwin"
 
 class WxAsyncApp(wx.App):
-    def __init__(self, warn_on_cancel_callback=False, **kwargs):
+    def __init__(self, warn_on_cancel_callback=False, sleep_duration=0.02, **kwargs):
         self.BoundObjects = {}
         self.RunningTasks = defaultdict(set)
         self.exiting = False
+        self.ui_idle = True
+        self.sleep_duration = sleep_duration
         self.warn_on_cancel_callback = warn_on_cancel_callback
         super(WxAsyncApp, self).__init__(**kwargs)
         self.SetExitOnFrameDelete(True)
 
     async def MainLoop(self):
         # inspired by https://github.com/wxWidgets/Phoenix/blob/master/samples/mainloop/mainloop.py
         evtloop = wx.GUIEventLoop()
         with wx.EventLoopActivator(evtloop):
             while not self.exiting:
                 if IS_MAC:
                     # evtloop.Pending() just returns True on MacOs
                     evtloop.DispatchTimeout(0)
+                    self.ui_idle = False
                 else:
                     while evtloop.Pending():
                         evtloop.Dispatch()
                         await asyncio.sleep(0)
-                await asyncio.sleep(0.005)
+                        self.ui_idle = False
+                await asyncio.sleep(self.sleep_duration)
                 self.ProcessPendingEvents()
-                evtloop.ProcessIdle()
+                if not self.ui_idle:
+                    evtloop.ProcessIdle()
+                    self.ui_idle = True
             self.exiting = False
 
     def ExitMainLoop(self):
         self.exiting = True
 
     def AsyncBind(self, event_binder, async_callback, object, source=None, id=wx.ID_ANY, id2=wx.ID_ANY):
         """Bind a coroutine to a wx Event. Note that when wx object is destroyed, any coroutine still running will be cancelled automatically.
```

### Comparing `wxasync-0.48/test/test_perfs.py` & `wxasync-0.49/test/test_perfs.py`

 * *Files identical despite different names*

