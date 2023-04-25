# Comparing `tmp/pyass-0.1.0.tar.gz` & `tmp/pyass-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyass-0.1.0.tar", max compression
+gzip compressed data, was "pyass-0.1.1.tar", max compression
```

## Comparing `pyass-0.1.0.tar` & `pyass-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1067 2022-11-11 08:39:45.819096 pyass-0.1.0/LICENSE
--rw-r--r--   0        0        0       89 2022-11-11 08:39:45.819096 pyass-0.1.0/README.md
--rw-r--r--   0        0        0     1347 2022-11-11 08:39:45.819096 pyass-0.1.0/pyass/__init__.py
--rw-r--r--   0        0        0      847 2022-11-11 08:39:45.819096 pyass-0.1.0/pyass/color.py
--rw-r--r--   0        0        0      112 2022-11-11 08:39:45.819096 pyass-0.1.0/pyass/drawing.py
--rw-r--r--   0        0        0      896 2022-11-11 08:39:45.819096 pyass-0.1.0/pyass/enum.py
--rw-r--r--   0        0        0     4078 2022-11-11 08:39:45.819096 pyass-0.1.0/pyass/event.py
--rw-r--r--   0        0        0      124 2022-11-11 08:39:45.819096 pyass-0.1.0/pyass/float.py
--rw-r--r--   0        0        0      419 2022-11-11 08:39:45.819096 pyass-0.1.0/pyass/position.py
--rw-r--r--   0        0        0     3752 2022-11-11 08:39:45.819096 pyass-0.1.0/pyass/script.py
--rw-r--r--   0        0        0     5579 2022-11-11 08:39:45.819096 pyass-0.1.0/pyass/section.py
--rw-r--r--   0        0        0     4239 2022-11-11 08:39:45.819096 pyass-0.1.0/pyass/style.py
--rw-r--r--   0        0        0    27281 2022-11-11 08:39:45.819096 pyass-0.1.0/pyass/tag.py
--rw-r--r--   0        0        0     3592 2022-11-11 08:39:45.819096 pyass-0.1.0/pyass/timedelta.py
--rw-r--r--   0        0        0      673 2022-11-11 08:39:45.819096 pyass-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 pyass-0.1.0/setup.py
--rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 pyass-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-25 07:33:42.674438 pyass-0.1.1/LICENSE
+-rw-r--r--   0        0        0       89 2023-04-25 07:33:42.674438 pyass-0.1.1/README.md
+-rw-r--r--   0        0        0     1349 2023-04-25 07:33:42.674438 pyass-0.1.1/pyass/__init__.py
+-rw-r--r--   0        0        0      847 2023-04-25 07:33:42.674438 pyass-0.1.1/pyass/color.py
+-rw-r--r--   0        0        0      112 2023-04-25 07:33:42.674438 pyass-0.1.1/pyass/drawing.py
+-rw-r--r--   0        0        0      896 2023-04-25 07:33:42.674438 pyass-0.1.1/pyass/enum.py
+-rw-r--r--   0        0        0     4780 2023-04-25 07:33:42.674438 pyass-0.1.1/pyass/event.py
+-rw-r--r--   0        0        0      124 2023-04-25 07:33:42.674438 pyass-0.1.1/pyass/float.py
+-rw-r--r--   0        0        0      419 2023-04-25 07:33:42.674438 pyass-0.1.1/pyass/position.py
+-rw-r--r--   0        0        0     3749 2023-04-25 07:33:42.674438 pyass-0.1.1/pyass/script.py
+-rw-r--r--   0        0        0     5579 2023-04-25 07:33:42.674438 pyass-0.1.1/pyass/section.py
+-rw-r--r--   0        0        0     4239 2023-04-25 07:33:42.674438 pyass-0.1.1/pyass/style.py
+-rw-r--r--   0        0        0    27281 2023-04-25 07:33:42.674438 pyass-0.1.1/pyass/tag.py
+-rw-r--r--   0        0        0     3592 2023-04-25 07:33:42.674438 pyass-0.1.1/pyass/timedelta.py
+-rw-r--r--   0        0        0      673 2023-04-25 07:33:42.674438 pyass-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 pyass-0.1.1/PKG-INFO
```

### Comparing `pyass-0.1.0/LICENSE` & `pyass-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyass-0.1.0/pyass/__init__.py` & `pyass-0.1.1/pyass/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,21 +57,21 @@
     TransformTag,
     UnderlineTag,
     WrappingStyleTag,
 )
 from .timedelta import timedelta
 
 
-def load(fp: _typing.TextIO) -> Script:
+def load(fp: _typing.IO[str]) -> Script:
     return loads(fp.read())
 
 
 def loads(s: str) -> Script:
     return Script.parse(s)
 
 
-def dump(o: Script, fp: _typing.TextIO) -> None:
+def dump(o: Script, fp: _typing.IO[str]) -> None:
     o.dump(fp)
 
 
 def dumps(o: Script) -> str:
     return o.dumps()
```

### Comparing `pyass-0.1.0/pyass/color.py` & `pyass-0.1.1/pyass/color.py`

 * *Files identical despite different names*

### Comparing `pyass-0.1.0/pyass/enum.py` & `pyass-0.1.1/pyass/enum.py`

 * *Files identical despite different names*

### Comparing `pyass-0.1.0/pyass/event.py` & `pyass-0.1.1/pyass/event.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+import threading
 from dataclasses import dataclass
 from datetime import timedelta
 from typing import Sequence, TypeVar
 
 import pyass
 from pyass.enum import EventFormat
 from pyass.tag import Tag, Tags
@@ -51,35 +52,60 @@
         self.end = end
         self.style = style
         self.name = name
         self.marginL = marginL
         self.marginR = marginR
         self.marginV = marginV
         self.effect = effect
-        self.parts = parts
+        self._parts = parts
+
+        self._textParseLock = threading.Lock()
+        self._unparsedText = ""
 
         if text:
-            self._set_parts_from_text(text)
+            self.text = text
 
         self._unknownRawText = ""
 
     def __str__(self) -> str:
         if self._unknownRawText:
             return self._unknownRawText
 
         # Format: Layer, Start, End, Style, Name, MarginL, MarginR, MarginV, Effect, Text
         return f"{self.format}: {self.layer},{pyass.timedelta(self.start)},{pyass.timedelta(self.end)},{self.style},{self.name},{self.marginL},{self.marginR},{self.marginV},{self.effect},{self.text}"
 
     @property
     def text(self) -> str:
-        return "".join([str(part) for part in self.parts])
+        with self._textParseLock:
+            if self._unparsedText:
+                return self._unparsedText
+
+        return "".join([str(part) for part in self._parts])
 
     @text.setter
     def text(self, text: str) -> None:
-        self._set_parts_from_text(text)
+        with self._textParseLock:
+            self._unparsedText = text
+
+    @property
+    def parts(self) -> Sequence[EventPart]:
+        with self._textParseLock:
+            if not self._unparsedText:
+                return self._parts
+
+            self._set_parts_from_text(self._unparsedText)
+            self._unparsedText = ""
+
+        return self._parts
+
+    @parts.setter
+    def parts(self, parts: Sequence[EventPart]) -> None:
+        with self._textParseLock:
+            self._parts = parts
+            self._unparsedText = ""
 
     @property
     def length(self) -> timedelta:
         return self.end - self.start
 
     @staticmethod
     def parse(s: str) -> Event:
@@ -111,34 +137,34 @@
             ret._unknownRawText = s
 
         return ret
 
     def _set_parts_from_text(self, text: str) -> None:
         # Short-circuit for empty string
         if not text:
-            self.parts = []
+            self._parts = []
             return
 
         # Short-circuit for text with no tags
         if "{" not in text or "}" not in text:
-            self.parts = [EventPart(text=text)]
+            self._parts = [EventPart(text=text)]
             return
 
         originalText = text
         try:
-            self.parts = []
+            self._parts = []
 
             if not text.startswith("{"):
                 # Consume everything up to the first {
                 tagStartIdx = text.index("{")
-                self.parts.append(EventPart(text=text[:tagStartIdx]))
+                self._parts.append(EventPart(text=text[:tagStartIdx]))
                 text = text[tagStartIdx:]
 
             # Then try to parse the rest of the line
-            self.parts.extend(
+            self._parts.extend(
                 [
                     EventPart(tags=Tags.parse(tagPart), text=textPart)
                     for tagPart, textPart in re.findall(r"\{([^\}]*)\}([^\{]*)", text)
                 ]
             )
         except:
-            self.parts = [EventPart(text=originalText)]
+            self._parts = [EventPart(text=originalText)]
```

### Comparing `pyass-0.1.0/pyass/script.py` & `pyass-0.1.1/pyass/script.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Sequence, TextIO, TypeVar
+from typing import IO, Sequence, TypeVar
 
 from pyass.event import Event
 from pyass.section import (
     AegisubGarbageSection,
     EventsSection,
     ScriptInfoSection,
     Section,
@@ -103,15 +103,15 @@
     def events(self) -> EventsSection:
         return self._get_section_by_type(EventsSection)
 
     @events.setter
     def events(self, s: Sequence[Event]):
         self._set_section(EventsSection(s))
 
-    def dump(self, fp: TextIO) -> None:
+    def dump(self, fp: IO[str]) -> None:
         fp.write(self.dumps())
 
     def dumps(self) -> str:
         return str(self)
 
     def _get_section_by_type(self, t: type[SectionT]) -> SectionT:
         for section in self.sections:
```

### Comparing `pyass-0.1.0/pyass/section.py` & `pyass-0.1.1/pyass/section.py`

 * *Files identical despite different names*

### Comparing `pyass-0.1.0/pyass/style.py` & `pyass-0.1.1/pyass/style.py`

 * *Files identical despite different names*

### Comparing `pyass-0.1.0/pyass/tag.py` & `pyass-0.1.1/pyass/tag.py`

 * *Files identical despite different names*

### Comparing `pyass-0.1.0/pyass/timedelta.py` & `pyass-0.1.1/pyass/timedelta.py`

 * *Files identical despite different names*

### Comparing `pyass-0.1.0/pyproject.toml` & `pyass-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry]
 name = "pyass"
-version = "0.1.0"
+version = "0.1.1"
 description = "A library to read, manipulate, and write Advanced SubStation Alpha (.ass) files"
 authors = ["xIceArcher <xicearcher@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/xIceArcher/pyass"
 
 [tool.poetry.dependencies]
```

### Comparing `pyass-0.1.0/PKG-INFO` & `pyass-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyass
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library to read, manipulate, and write Advanced SubStation Alpha (.ass) files
 Home-page: https://github.com/xIceArcher/pyass
 License: MIT
 Author: xIceArcher
 Author-email: xicearcher@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

