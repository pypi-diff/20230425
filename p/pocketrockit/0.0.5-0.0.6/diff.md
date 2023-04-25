# Comparing `tmp/pocketrockit-0.0.5.tar.gz` & `tmp/pocketrockit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocketrockit-0.0.5.tar", max compression
+gzip compressed data, was "pocketrockit-0.0.6.tar", max compression
```

## Comparing `pocketrockit-0.0.5.tar` & `pocketrockit-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     2639 2023-04-24 09:36:45.137979 pocketrockit-0.0.5/Readme.md
--rw-r--r--   0        0        0        0 2023-04-24 06:41:37.681837 pocketrockit-0.0.5/pocketrockit/__init__.py
--rwxr-xr-x   0        0        0     1015 2023-04-24 09:16:32.725478 pocketrockit-0.0.5/pocketrockit/cli.py
--rwxr-xr-x   0        0        0    11070 2023-04-24 18:56:49.398188 pocketrockit-0.0.5/pocketrockit/decorated.py
--rwxr-xr-x   0        0        0     9258 2023-04-24 14:41:01.517659 pocketrockit-0.0.5/pocketrockit/engine.py
--rw-r--r--   0        0        0     1890 2023-04-24 18:57:25.491195 pocketrockit-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3228 1970-01-01 00:00:00.000000 pocketrockit-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2639 2023-04-25 05:45:46.696906 pocketrockit-0.0.6/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-25 05:45:46.700907 pocketrockit-0.0.6/pocketrockit/__init__.py
+-rwxr-xr-x   0        0        0     1015 2023-04-25 05:45:46.700907 pocketrockit-0.0.6/pocketrockit/cli.py
+-rwxr-xr-x   0        0        0    12298 2023-04-25 07:49:37.468741 pocketrockit-0.0.6/pocketrockit/decorated.py
+-rwxr-xr-x   0        0        0     9521 2023-04-25 07:49:37.468741 pocketrockit-0.0.6/pocketrockit/engine.py
+-rw-r--r--   0        0        0     1890 2023-04-25 07:50:16.968846 pocketrockit-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3649 1970-01-01 00:00:00.000000 pocketrockit-0.0.6/setup.py
+-rw-r--r--   0        0        0     3228 1970-01-01 00:00:00.000000 pocketrockit-0.0.6/PKG-INFO
```

### Comparing `pocketrockit-0.0.5/Readme.md` & `pocketrockit-0.0.6/Readme.md`

 * *Files identical despite different names*

### Comparing `pocketrockit-0.0.5/pocketrockit/cli.py` & `pocketrockit-0.0.6/pocketrockit/cli.py`

 * *Files identical despite different names*

### Comparing `pocketrockit-0.0.5/pocketrockit/decorated.py` & `pocketrockit-0.0.6/pocketrockit/decorated.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python3
 
 """API for fancy decorator based track definitions"""
 
 from collections.abc import Sequence
 from itertools import count
+from functools import wraps
 
-from .engine import Env, Stage, run
+from pocketrockit.engine import Env, Stage, run
 
 stage = Stage()
 
 __all__ = ["track", "player", "Env", "midiseq"]
 
 
 def run_engine(initial_track: str) -> bool:
@@ -40,16 +41,16 @@
         print(f"exception in build: {exc}")
         return
 
     # initialize note generators (and also trigger eventual bugs!)
     for name, stream in stage.new_track:
         print(f"initialize player '{name}' with tick={stage.tick}")
         try:
-            print("X", next(stream))
-            print("Y", stream.send(stage.tick))
+            next(stream)
+            stream.send(stage.tick + 1)
         except StopIteration:
             pass
         except Exception as exc:  # pylint: disable=broad-except
             print(f"exception in player init: {exc}")
 
     # all fine - use the new model
     # if not stage.players:
@@ -109,40 +110,67 @@
 
 
 def midi_commands(string: str, channel: int, force_note: None | str, scale, velocity: int):
     """Turns something like '60', 'c', 'c,d,e' or 't1,t2,t3' into MIDI commands"""
 
     try:
         return (
-            None
+            []
             if string == "."
             else [
                 (
                     channel,
                     resolve(force_note or element, scale),
                     velocity,
                 )
                 for element in string.split(",")
             ]
         )
     except Exception as exc:  # pylint: disable=broad-except
         print(f"could not turn '{string}' into note ({exc})")
-        return None
+        return []
 
 
+def midi_terminator(midi_fn):
+    """Cleans up"""
+    active = {}
+    @wraps(midi_fn)
+    def cleanup(*args, **kwargs):
+        gen =  midi_fn(*args, **kwargs)
+        comm = None
+        for i in count():
+            stoppers = []
+            loop, tick, original, commands = gen.send(comm)
+            for channel, note, _velocity in commands or []:
+                #print((channel, note), active)
+                if (channel, note) in active:
+                    stoppers.append((channel, note, None))
+                    del active[(channel, note)]
+
+                for (c, n) in list(active):
+                    stoppers.append((c, n, None))
+                    del active[(c, n)]
+
+                active[(channel, note)] = i
+            comm = yield loop, tick, original, stoppers + commands
+
+    return cleanup
+
+
+@midi_terminator
 def midiseq(pattern: str, channel=0, note=None, key="C", velocity=30):
     """A minimal MIDI sequencer"""
     elements = pattern.split()
     assert len(elements) == 16
     reset_tick: None | int = None
     scale = midi_scale(key)
     while True:
         if reset_tick is not None:
             print(f"reset to {reset_tick}")
-            yield None
+            yield -1, -1, "", []
 
         start_loop = (reset_tick or 0) // len(elements)
         skip = (reset_tick or 0) % len(elements)
 
         for loop, tick, element in (
             (_loop, _tick, _element)
             for _loop in count(start_loop)
@@ -273,7 +301,24 @@
         (124, {"E9", "e’’’’’’", "124"}, 10548.08),
         (125, {"F9", "E#9", "f’’’’’’", "125"}, 11175.3),
         (126, {"fis’’’’’’", "126", "ges’’’’’’", "Gb9", "F#9"}, 11839.82),
         (127, {"G9", "g’’’’’’", "127"}, 12543.85),
     )
     for name in names
 }
+
+
+
+if __name__ == "__main__":
+    note_generator = midiseq("x " * 16)
+    print(note_generator.send(None))
+    print(note_generator.send(None))
+
+    print(note_generator.send(1))
+
+    print(note_generator.send(None))
+    print(note_generator.send(None))
+
+    print(note_generator.send(1))
+
+    print(note_generator.send(None))
+    print(note_generator.send(None))
```

### Comparing `pocketrockit-0.0.5/pocketrockit/engine.py` & `pocketrockit-0.0.6/pocketrockit/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     """Not yet a Singleton - access to the currently played music"""
 
     env: Env = field(default_factory=Env)
     active: bool = False
     players: list = field(default_factory=list)
     new_track: None | list = None
     file_to_track: str = ""
-    tick: int = 0
+    tick: int = -1
 
 
 @contextmanager
 def mididevice_pygame():
     """
     fluidsynth -vv -a pipewire -z 256 -g 2 FluidR3_GM.sf2
     """
@@ -243,16 +243,21 @@
                         notes.extend(commands)
                 except StopIteration:
                     pass
                 except Exception as exc:  # pylint: disable=broad-except
                     print(f"exception in play: {exc}")
                     print("--")
 
-            for note in notes:
-                midi_out.noteon(*note)
+            for channel, note, velocity in notes:
+                if velocity is None:
+                    #print("OF", (channel, note))
+                    midi_out.noteoff(channel, note)
+                else:
+                    #print("ON", (channel, note, velocity))
+                    midi_out.noteon(channel, note, velocity)
 
             # make me absolute please
             waitfor = 60 / Stage().env.bpm / 4
             await sleep(waitfor)
 
 
 async def watch_changes() -> None:
```

### Comparing `pocketrockit-0.0.5/pyproject.toml` & `pocketrockit-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pocketrockit"
-version = "0.0.5"
+version = "0.0.6"
 description = "pocketrockit"
 authors = ["Frans Fürst <frans.fuerst+gitlab@protonmail.com>"]
 repository = "https://projects.om-office.de/frans/pocketrockit.git"
 readme = "Readme.md"
 packages = [
   {include = "pocketrockit"}
 ]
```

### Comparing `pocketrockit-0.0.5/PKG-INFO` & `pocketrockit-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketrockit
-Version: 0.0.5
+Version: 0.0.6
 Summary: pocketrockit
 Home-page: https://projects.om-office.de/frans/pocketrockit.git
 Author: Frans Fürst
 Author-email: frans.fuerst+gitlab@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

