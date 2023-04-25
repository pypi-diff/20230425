# Comparing `tmp/pocketrockit-0.0.4.tar.gz` & `tmp/pocketrockit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocketrockit-0.0.4.tar", max compression
+gzip compressed data, was "pocketrockit-0.0.5.tar", max compression
```

## Comparing `pocketrockit-0.0.4.tar` & `pocketrockit-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2636 2023-04-24 06:41:37.681837 pocketrockit-0.0.4/Readme.md
--rw-r--r--   0        0        0        0 2023-04-24 06:41:37.681837 pocketrockit-0.0.4/pocketrockit/__init__.py
--rwxr-xr-x   0        0        0     1001 2023-04-24 08:54:19.945411 pocketrockit-0.0.4/pocketrockit/cli.py
--rwxr-xr-x   0        0        0    10829 2023-04-24 08:05:55.081996 pocketrockit-0.0.4/pocketrockit/decorated.py
--rwxr-xr-x   0        0        0     8272 2023-04-24 09:13:17.669566 pocketrockit-0.0.4/pocketrockit/engine.py
--rw-r--r--   0        0        0     1892 2023-04-24 09:11:14.225621 pocketrockit-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3225 1970-01-01 00:00:00.000000 pocketrockit-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2639 2023-04-24 09:36:45.137979 pocketrockit-0.0.5/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-24 06:41:37.681837 pocketrockit-0.0.5/pocketrockit/__init__.py
+-rwxr-xr-x   0        0        0     1015 2023-04-24 09:16:32.725478 pocketrockit-0.0.5/pocketrockit/cli.py
+-rwxr-xr-x   0        0        0    11070 2023-04-24 18:56:49.398188 pocketrockit-0.0.5/pocketrockit/decorated.py
+-rwxr-xr-x   0        0        0     9258 2023-04-24 14:41:01.517659 pocketrockit-0.0.5/pocketrockit/engine.py
+-rw-r--r--   0        0        0     1890 2023-04-24 18:57:25.491195 pocketrockit-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3228 1970-01-01 00:00:00.000000 pocketrockit-0.0.5/PKG-INFO
```

### Comparing `pocketrockit-0.0.4/Readme.md` & `pocketrockit-0.0.5/Readme.md`

 * *Files 0% similar despite different names*

```diff
@@ -91,16 +91,19 @@
 poetry install
 ```
 
 
 ## Stuff to read / Sources
 
 ### SoundFonts
+
 * https://musescore.org/en/handbook/3/soundfonts-and-sfz-files
 * https://www.producersbuzz.com/category/downloads/download-free-soundfonts-sf2/
 * https://archive.org/details/500-soundfonts-full-gm-sets
 * https://ia802502.us.archive.org/view_archive.php?archive=/27/items/500-soundfonts-full-gm-sets/500_Soundfonts_Full_GM_Sets.zip
 * https://musical-artifacts.com/artifacts?formats=sf2&tags=soundfont
 
+
 ### Music theory
+
 * https://pianoscales.org/major.html
 * https://www.inspiredacoustics.com/en/MIDI_note_numbers_and_center_frequencies
```

### Comparing `pocketrockit-0.0.4/pocketrockit/cli.py` & `pocketrockit-0.0.5/pocketrockit/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,23 +16,25 @@
     parser.add_argument("path", type=Path)
 
     return parser.parse_args()
 
 
 def main() -> int:
     """Entry point for everything else"""
-    print("""
+    print(
+        """
     This executable does not do anything yet. Later in time it can be used to run one or multiple
     pocketrockit tracks simultaneously and to configure run time behavior.
     
     For now, please follow the steps described on https://projects.om-office.de/frans/pocketrockit
 
     In short:
     * create a working folder and provide FluidR3_GM.sf2 and JV_1080_Drums.sf2
     * create an executable track script, e.g. mytrack.py
     * directly run this track script
-    """)
+    """
+    )
     return 0
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pocketrockit-0.0.4/pocketrockit/decorated.py` & `pocketrockit-0.0.5/pocketrockit/decorated.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,81 +1,71 @@
 #!/usr/bin/env python3
 
 """API for fancy decorator based track definitions"""
 
 from collections.abc import Sequence
-from dataclasses import dataclass, field
 from itertools import count
 
-from .engine import run
+from .engine import Env, Stage, run
 
+stage = Stage()
 
-@dataclass
-class Env:
-    """Some global environment"""
-    bpm: int = 60
+__all__ = ["track", "player", "Env", "midiseq"]
 
 
-@dataclass
-class Singleton:
-    """Not yet a Singleton - access to the currently played music"""
-    env: Env = field(default_factory=Env)
-    active: bool = False
-    players: None | list = None
-    new_track: None | list = None
-    file_to_track: None | str = None
-    tick: int = 0
+def run_engine(initial_track: str) -> bool:
+    """If engine is not yet running, run it and never return"""
+    if stage.active:
+        return False
 
+    stage.active = True
+    stage.file_to_track = initial_track
+    run()
+    return True
 
-singleton = Singleton()
 
-
-def run_engine(initial_track):
-    if singleton.active:
+def track(track_definition_fn) -> None:
+    """Creates a track (a list of note generators called players) by running provided
+    @track_definition_fn
+    Only effective starting from second run."""
+    if run_engine(track_definition_fn.__globals__["__file__"]):
         return
 
-    singleton.active = True
-    singleton.file_to_track = initial_track
-    run(singleton)
-
-
-def track(track_definition_fn):
-    run_engine(track_definition_fn.__globals__["__file__"])
-
     print(f"define track '{track_definition_fn.__name__}'")
-    singleton.new_track = []
-    env = Env(bpm=singleton.env.bpm)
+    stage.new_track = []
+    env = Env(bpm=stage.env.bpm)
     try:
         # create the new track model
         track_definition_fn(env)
-    except Exception as exc:
+    except Exception as exc:  # pylint: disable=broad-except
         print(f"exception in build: {exc}")
         return
 
     # initialize note generators (and also trigger eventual bugs!)
-    for name, stream in singleton.new_track:
-        print(f"initialize player '{name}' with tick={singleton.tick}")
+    for name, stream in stage.new_track:
+        print(f"initialize player '{name}' with tick={stage.tick}")
         try:
             print("X", next(stream))
-            print("Y", stream.send(singleton.tick))
+            print("Y", stream.send(stage.tick))
         except StopIteration:
             pass
-        except Exception as exc:
+        except Exception as exc:  # pylint: disable=broad-except
             print(f"exception in player init: {exc}")
 
     # all fine - use the new model
-    # if not singleton.players:
+    # if not stage.players:
 
-    singleton.players = singleton.new_track
-    singleton.env = env
+    stage.players = stage.new_track
+    stage.env = env
 
 
-def player(arg):
-    print(f"define player '{arg.__name__}'")
-    singleton.new_track.append((arg.__name__, arg()))
+def player(player_definition_fn):
+    """Adds generator created from @player_definition_fn to new track definition"""
+    print(f"define player '{player_definition_fn.__name__}'")
+    stage.new_track.append((player_definition_fn.__name__, player_definition_fn()))
 
 
 # @contextmanager
 # def FX(name, controller):
 # try:
 # print(f"enter FX {name}")
 # yield "bla"
@@ -94,49 +84,51 @@
     E.g. 'C' => 'C4', etc.
     Numeric values will be directly interpreted as MIDI values
     """
     base = key.strip("-")
     minor = key[-1] == "-"
     octave = (
         ""
-        if any(base[i] in {"0", "1", "2", "3", "4", "5", "6", "7", "8", "9"} for i in {0, -1})
+        if any(base[i] in {"0", "1", "2", "3", "4", "5", "6", "7", "8", "9"} for i in (0, -1))
         # else "3"
         # if minor and key[0].lower() in {"a", "b"}
         else "4"
     )
 
     return [
         NOTES[f"{base}{octave}"] + e
         for e in ([0, 2, 3, 5, 7, 8, 10, 12] if minor else [0, 2, 4, 5, 7, 9, 11, 12])
     ]
 
 
-def midi_commands(
-    string: str, channel: int, force_note: None | int, key: str, scale, velocity: int
-):
+def resolve(note_str: str, scale: Sequence[int]) -> int:
+    """Not in the mood to write a comment"""
+    shift = sum(12 if e == "+" else -12 if e == "-" else 0 for e in note_str)
+    if note_str[0] in {"t", "n"}:
+        return scale[int(note_str[1]) - 1] + shift
+    return NOTES[note_str] + shift
+
+
+def midi_commands(string: str, channel: int, force_note: None | str, scale, velocity: int):
     """Turns something like '60', 'c', 'c,d,e' or 't1,t2,t3' into MIDI commands"""
 
     try:
         return (
             None
             if string == "."
             else [
                 (
                     channel,
-                    force_note
-                    if force_note is not None
-                    else scale[int(element[1:]) - 1]
-                    if element[0] in {"t", "n"}
-                    else NOTES[element],
+                    resolve(force_note or element, scale),
                     velocity,
                 )
                 for element in string.split(",")
             ]
         )
-    except Exception as exc:
+    except Exception as exc:  # pylint: disable=broad-except
         print(f"could not turn '{string}' into note ({exc})")
         return None
 
 
 def midiseq(pattern: str, channel=0, note=None, key="C", velocity=30):
     """A minimal MIDI sequencer"""
     elements = pattern.split()
@@ -160,15 +152,15 @@
                 skip -= 1
                 continue
 
             reset_tick = yield (
                 loop,
                 tick,
                 element,
-                midi_commands(element, channel, note, key, scale, velocity),
+                midi_commands(element, channel, note, scale, velocity),
             )
             if reset_tick is not None:
                 break
 
 
 # B2!!
 # A2!!
```

### Comparing `pocketrockit-0.0.4/pocketrockit/engine.py` & `pocketrockit-0.0.5/pocketrockit/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,29 +3,60 @@
 """Demonstrates the midi music player
 
 https://newt.phys.unsw.edu.au/jw/notes.html
 
 """
 
 import asyncio
-import concurrent
 import logging
 import threading
 from asyncio import sleep
-from collections.abc import Iterable
+from collections.abc import Iterable, MutableMapping
 from contextlib import ExitStack, contextmanager, suppress
+from dataclasses import dataclass, field
 from importlib.util import module_from_spec, spec_from_file_location
 from itertools import count
 from pathlib import Path
+from types import ModuleType
 
 import fluidsynth
 import pygame.midi
 from asyncinotify import Inotify, Mask
 
 
+class Singleton(type):
+    """Yes, a Singleton"""
+
+    _instances: MutableMapping[type, object] = {}
+
+    def __call__(cls, *args, **kwargs):
+        if cls not in cls._instances:
+            cls._instances[cls] = super().__call__(*args, **kwargs)
+        return cls._instances[cls]
+
+
+@dataclass
+class Env:
+    """Some global environment"""
+
+    bpm: int = 60
+
+
+@dataclass
+class Stage(metaclass=Singleton):
+    """Not yet a Singleton - access to the currently played music"""
+
+    env: Env = field(default_factory=Env)
+    active: bool = False
+    players: list = field(default_factory=list)
+    new_track: None | list = None
+    file_to_track: str = ""
+    tick: int = 0
+
+
 @contextmanager
 def mididevice_pygame():
     """
     fluidsynth -vv -a pipewire -z 256 -g 2 FluidR3_GM.sf2
     """
     try:
         pygame.midi.init()
@@ -62,15 +93,15 @@
 
 def pygame_thread_fn(loop, event_queue, terminator):
     """Pygame thread"""
     try:
         logger().debug(">> pygame_thread_fn")
         pygame.init()
         pygame.display.set_caption("pygame+asyncio")
-        screen = pygame.display.set_mode((512, 512))
+        pygame.display.set_mode((512, 512))
 
         while not terminator.is_set():
             event = pygame.event.wait()
             asyncio.run_coroutine_threadsafe(event_queue.put(event), loop=loop)
 
         logger().debug("pygame_thread_fn: got termination signal")
 
@@ -88,40 +119,40 @@
 def choose(choices: Iterable[str], *wishlist: str) -> str:
     for wish in wishlist:
         with suppress(StopIteration):
             return next(name for name in choices if wish in name)
     raise KeyError(f"{wishlist}")
 
 
-#def read_midi(loop, event_queue, terminator):
-    #logger().debug(">> read_midi")
+# def read_midi(loop, event_queue, terminator):
+# logger().debug(">> read_midi")
 
-    #try:
-        #available_input_ports = set(mido.get_input_names())
-        #logger().info("Available MIDI input ports: \n%s", "  \n".join(available_input_ports))
+# try:
+# available_input_ports = set(mido.get_input_names())
+# logger().info("Available MIDI input ports: \n%s", "  \n".join(available_input_ports))
 
-        #chosen_input = choose(
-            #available_input_ports, "OP-1", "Sylphyo", "USB MIDI Interface", "Midi Through"
-        #)
-        #logger().info("Chosen: %r", chosen_input)
+# chosen_input = choose(
+# available_input_ports, "OP-1", "Sylphyo", "USB MIDI Interface", "Midi Through"
+# )
+# logger().info("Chosen: %r", chosen_input)
 
-        #with mido.open_input(chosen_input) as inport:
-            #while not terminator.is_set():
-                #if (event := inport.receive()).type == "clock":
-                    #continue
-                #asyncio.run_coroutine_threadsafe(event_queue.put(event), loop=loop)
-            #logger().debug("read_midi: got termination signal")
+# with mido.open_input(chosen_input) as inport:
+# while not terminator.is_set():
+# if (event := inport.receive()).type == "clock":
+# continue
+# asyncio.run_coroutine_threadsafe(event_queue.put(event), loop=loop)
+# logger().debug("read_midi: got termination signal")
 
-    #except Exception as exc:
-        #logger().error("Unhandled exception in read_midi thread: %s", exc)
+# except Exception as exc:
+# logger().error("Unhandled exception in read_midi thread: %s", exc)
 
-    #logger().debug("<< read_midi")
+# logger().debug("<< read_midi")
 
 
-async def handle_events(event_queue, task, terminator):
+async def handle_events(event_queue: asyncio.Queue, _task, terminator):
     logger().debug(">> handle_events")
     try:
         while not terminator.is_set():
             try:
                 event = await event_queue.get()
                 if event.type in {pygame.WINDOWCLOSE, pygame.QUIT}:
                     logger().debug("quit/windowclose")
@@ -136,130 +167,136 @@
                     pass
                 elif event.type == "note_on":
                     print("NOTEON", event)
                 elif event.type == "note_off":
                     print("NOTEOFF", event)
                 else:
                     logger().debug("event %s", event)
-            except Exception as exc:
+            except Exception as exc:  # pylint: disable=broad-except
                 print(exc)
         logger().debug("handle_events: got termination signal")
 
     finally:
         # Close the connection to the output device and quit the MIDI system
         # midi_out.delete()
 
         asyncio.get_event_loop().stop()
         logger().debug("<< handle_events")
 
 
-def terminate(terminator):
+def terminate(terminator) -> None:
     terminator.set()
     pygame.event.post(pygame.event.Event(pygame.MOUSEMOTION))
 
 
-def logger():
+def logger() -> logging.Logger:
     return logging.getLogger("silmaril")
 
 
-def setup_logging():
+def setup_logging() -> None:
     def thread_id_filter(record):
         """Inject thread_id to log records"""
         record.thread_id = threading.get_native_id()
         return record
 
     handler = logging.StreamHandler()
     handler.setFormatter(
         logging.Formatter("%(asctime)s | %(levelname)s | %(thread_id)s | %(message)s")
     )
     handler.addFilter(thread_id_filter)
     logger().addHandler(handler)
     logger().setLevel("DEBUG")
 
 
-def load_module(filepath: str | Path):
+def load_module(filepath: str | Path) -> ModuleType:
     print(r"load module '{Path(filepath).stem}'")
     spec = spec_from_file_location(Path(filepath).stem, filepath)
+    assert spec and spec.loader
     module = module_from_spec(spec)
+    assert module
     # here the actual track definition takes place
     spec.loader.exec_module(module)
     return module
 
 
-async def tick(singleton):
+async def music_loop() -> None:
     with mididevice_fluidsynth() as midi_out:
         # wait for players to emerge (otherwise `tick` won't start at 0)
         while True:
-            if singleton.players:
+            if Stage().players:
                 break
             print("no players yet..")
             await sleep(1)
             continue
 
         for tick in count():
-            singleton.tick = tick
+            Stage().tick = tick
 
             notes = []
             if tick % 1 == 0:
                 print(f"== {tick // 16} {tick // 4} {tick % 4} {tick} ==")
 
-            for name, stream in singleton.players:
+            for name, stream in Stage().players:
                 try:
                     source_loop, source_tick, origin, commands = next(stream)
                     print(f"{name}: {source_loop}:{source_tick}:{origin} => {commands}")
                     if commands:
                         notes.extend(commands)
                 except StopIteration:
                     pass
-                except Exception as exc:
+                except Exception as exc:  # pylint: disable=broad-except
                     print(f"exception in play: {exc}")
                     print("--")
 
             for note in notes:
                 midi_out.noteon(*note)
 
             # make me absolute please
-            waitfor = 60 / singleton.env.bpm / 4
+            waitfor = 60 / Stage().env.bpm / 4
             await sleep(waitfor)
 
 
-async def watch_changes(filepath):
-    load_module(filepath)
+async def watch_changes() -> None:
+    """Watches for file changes in track definition file and reload on change"""
+    stage = Stage()
+    load_module(stage.file_to_track)
     with Inotify() as inotify:
         inotify.add_watch(
-            Path(filepath).parent,
+            Path(Stage().file_to_track).parent,
             Mask.CLOSE_WRITE,
         )
         async for event in inotify:
             print(event.path, event.mask)
             try:
+                assert event.path
                 load_module(event.path)
-            except Exception as exc:
+            except Exception as exc:  # pylint: disable=broad-except
                 print("caught {exc}")
 
 
-def run(singleton):
+def run() -> None:
+    """Runs the pocketrockit event loop forever"""
     setup_logging()
     logger().info("Hello from main thread")
-    event_queue = asyncio.Queue()
+    event_queue: asyncio.Queue = asyncio.Queue()
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
     terminator = threading.Event()
 
     with ExitStack() as context:
         # context.enter_context(setup_midi(event_queue))
-        pool = context.enter_context(concurrent.futures.ThreadPoolExecutor())
+        # pool = context.enter_context(concurrent.futures.ThreadPoolExecutor())
 
-        #midi_reader = loop.run_in_executor(pool, read_midi, loop, event_queue, terminator)
+        # midi_reader = loop.run_in_executor(pool, read_midi, loop, event_queue, terminator)
         pygame_task = (
             None  # loop.run_in_executor(pool, pygame_thread_fn, loop, event_queue, terminator)
         )
-        event_task = asyncio.ensure_future(handle_events(event_queue, pygame_task, terminator))
-        asyncio.ensure_future(tick(singleton))
-        asyncio.ensure_future(watch_changes(singleton.file_to_track))
+        asyncio.ensure_future(handle_events(event_queue, pygame_task, terminator))
+        asyncio.ensure_future(music_loop())
+        asyncio.ensure_future(watch_changes())
 
         try:
             loop.run_forever()
         except KeyboardInterrupt:
             logger().debug("KeyboardInterrput in main()")
             terminate(terminator)
```

### Comparing `pocketrockit-0.0.4/pyproject.toml` & `pocketrockit-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pocketrockit"
-version = "0.0.4"
+version = "0.0.5"
 description = "pocketrockit"
 authors = ["Frans Fürst <frans.fuerst+gitlab@protonmail.com>"]
 repository = "https://projects.om-office.de/frans/pocketrockit.git"
 readme = "Readme.md"
 packages = [
   {include = "pocketrockit"}
 ]
@@ -23,15 +23,15 @@
 
 [tool.poetry.dev-dependencies]
 black = "^22.6.0"
 isort = "^5.10.1"
 flake8 = "^4.0.1"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
-mypy = "^0.991"
+mypy = "^1.2"
 pylint = "^2.15.3"
 ipython = "^8.8.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pocketrockit-0.0.4/PKG-INFO` & `pocketrockit-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketrockit
-Version: 0.0.4
+Version: 0.0.5
 Summary: pocketrockit
 Home-page: https://projects.om-office.de/frans/pocketrockit.git
 Author: Frans Fürst
 Author-email: frans.fuerst+gitlab@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -107,17 +107,20 @@
 poetry install
 ```
 
 
 ## Stuff to read / Sources
 
 ### SoundFonts
+
 * https://musescore.org/en/handbook/3/soundfonts-and-sfz-files
 * https://www.producersbuzz.com/category/downloads/download-free-soundfonts-sf2/
 * https://archive.org/details/500-soundfonts-full-gm-sets
 * https://ia802502.us.archive.org/view_archive.php?archive=/27/items/500-soundfonts-full-gm-sets/500_Soundfonts_Full_GM_Sets.zip
 * https://musical-artifacts.com/artifacts?formats=sf2&tags=soundfont
 
+
 ### Music theory
+
 * https://pianoscales.org/major.html
 * https://www.inspiredacoustics.com/en/MIDI_note_numbers_and_center_frequencies
```

