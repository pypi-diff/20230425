# Comparing `tmp/pure_protobuf-3.0.0a1.tar.gz` & `tmp/pure_protobuf-3.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure_protobuf-3.0.0a1.tar", max compression
+gzip compressed data, was "pure_protobuf-3.0.0a2.tar", max compression
```

## Comparing `pure_protobuf-3.0.0a1.tar` & `pure_protobuf-3.0.0a2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1089 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/LICENSE
--rw-r--r--   0        0        0     3210 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/README.md
--rw-r--r--   0        0        0        0 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/__init__.py
--rw-r--r--   0        0        0     2375 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/_accumulators.py
--rw-r--r--   0        0        0     1679 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/_mergers.py
--rw-r--r--   0        0        0     3239 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/annotations.py
--rw-r--r--   0        0        0        0 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/descriptors/__init__.py
--rw-r--r--   0        0        0     4769 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/descriptors/_field.py
--rw-r--r--   0        0        0     7826 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/descriptors/record.py
--rw-r--r--   0        0        0      685 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/helpers/__init__.py
--rw-r--r--   0        0        0      211 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/helpers/_dataclasses.py
--rw-r--r--   0        0        0     1085 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/helpers/_typing.py
--rw-r--r--   0        0        0      441 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/helpers/datetime.py
--rw-r--r--   0        0        0      581 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/helpers/io.py
--rw-r--r--   0        0        0      542 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/helpers/itertools.py
--rw-r--r--   0        0        0        0 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/interfaces/__init__.py
--rw-r--r--   0        0        0      917 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/interfaces/_repr.py
--rw-r--r--   0        0        0      650 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/interfaces/_skip.py
--rw-r--r--   0        0        0      522 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/interfaces/_vars.py
--rw-r--r--   0        0        0      746 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/interfaces/accumulate.py
--rw-r--r--   0        0        0      516 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/interfaces/merge.py
--rw-r--r--   0        0        0      848 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/interfaces/read.py
--rw-r--r--   0        0        0      432 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/interfaces/write.py
--rw-r--r--   0        0        0        0 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/io/__init__.py
--rw-r--r--   0        0        0     1420 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/io/bytes_.py
--rw-r--r--   0        0        0      269 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/io/fixed32.py
--rw-r--r--   0        0        0      250 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/io/fixed64.py
--rw-r--r--   0        0        0     1053 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/io/struct_.py
--rw-r--r--   0        0        0     1446 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/io/tag.py
--rw-r--r--   0        0        0      619 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/io/url.py
--rw-r--r--   0        0        0     4541 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/io/varint.py
--rw-r--r--   0        0        0     1204 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/io/wire_type.py
--rw-r--r--   0        0        0     4840 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/io/wrappers.py
--rw-r--r--   0        0        0     4576 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/message.py
--rw-r--r--   0        0        0     2376 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/one_of.py
--rw-r--r--   0        0        0     3720 2023-03-04 14:52:43.772826 pure_protobuf-3.0.0a1/pure_protobuf/well_known.py
--rw-r--r--   0        0        0     3478 2023-03-04 14:52:57.309013 pure_protobuf-3.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     4855 1970-01-01 00:00:00.000000 pure_protobuf-3.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-25 11:49:12.039312 pure_protobuf-3.0.0a2/LICENSE
+-rw-r--r--   0        0        0     3210 2023-04-25 11:49:12.039312 pure_protobuf-3.0.0a2/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/__init__.py
+-rw-r--r--   0        0        0     2375 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/_accumulators.py
+-rw-r--r--   0        0        0     1679 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/_mergers.py
+-rw-r--r--   0        0        0     3239 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/annotations.py
+-rw-r--r--   0        0        0        0 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/descriptors/__init__.py
+-rw-r--r--   0        0        0     4769 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/descriptors/_field.py
+-rw-r--r--   0        0        0     7833 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/descriptors/record.py
+-rw-r--r--   0        0        0      685 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/helpers/__init__.py
+-rw-r--r--   0        0        0      211 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/helpers/_dataclasses.py
+-rw-r--r--   0        0        0     1085 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/helpers/_typing.py
+-rw-r--r--   0        0        0      441 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/helpers/datetime.py
+-rw-r--r--   0        0        0      589 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/helpers/io.py
+-rw-r--r--   0        0        0      635 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/helpers/itertools.py
+-rw-r--r--   0        0        0        0 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/interfaces/__init__.py
+-rw-r--r--   0        0        0      935 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/interfaces/_repr.py
+-rw-r--r--   0        0        0      620 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/interfaces/_skip.py
+-rw-r--r--   0        0        0      522 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/interfaces/_vars.py
+-rw-r--r--   0        0        0      716 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/interfaces/accumulate.py
+-rw-r--r--   0        0        0      486 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/interfaces/merge.py
+-rw-r--r--   0        0        0      818 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/interfaces/read.py
+-rw-r--r--   0        0        0      402 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/interfaces/write.py
+-rw-r--r--   0        0        0        0 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/io/__init__.py
+-rw-r--r--   0        0        0     1420 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/io/bytes_.py
+-rw-r--r--   0        0        0      269 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/io/fixed32.py
+-rw-r--r--   0        0        0      250 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/io/fixed64.py
+-rw-r--r--   0        0        0     1112 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/io/struct_.py
+-rw-r--r--   0        0        0     1446 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/io/tag.py
+-rw-r--r--   0        0        0      619 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/io/url.py
+-rw-r--r--   0        0        0     4541 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/io/varint.py
+-rw-r--r--   0        0        0     1204 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/io/wire_type.py
+-rw-r--r--   0        0        0     4976 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/io/wrappers.py
+-rw-r--r--   0        0        0     4576 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/message.py
+-rw-r--r--   0        0        0     2376 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/one_of.py
+-rw-r--r--   0        0        0        0 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/py.typed
+-rw-r--r--   0        0        0     3720 2023-04-25 11:49:12.043313 pure_protobuf-3.0.0a2/pure_protobuf/well_known.py
+-rw-r--r--   0        0        0     3425 2023-04-25 11:49:29.247636 pure_protobuf-3.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     4755 1970-01-01 00:00:00.000000 pure_protobuf-3.0.0a2/PKG-INFO
```

### Comparing `pure_protobuf-3.0.0a1/LICENSE` & `pure_protobuf-3.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a1/README.md` & `pure_protobuf-3.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/_accumulators.py` & `pure_protobuf-3.0.0a2/pure_protobuf/_accumulators.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/_mergers.py` & `pure_protobuf-3.0.0a2/pure_protobuf/_mergers.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/annotations.py` & `pure_protobuf-3.0.0a2/pure_protobuf/annotations.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/descriptors/_field.py` & `pure_protobuf-3.0.0a2/pure_protobuf/descriptors/_field.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/descriptors/record.py` & `pure_protobuf-3.0.0a2/pure_protobuf/descriptors/record.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     read: ReadTyped[RecordT]
     """
     Read a record from the stream.
 
     This behaves differently from the [`write`][pure_protobuf.descriptors.record.RecordDescriptor.write],
     because it's only supposed to read a single record from the stream
-    (it may be, for example, just one item of a repeated field).
+    (it may be, for example, just one item of a packed repeated field).
     Also, it assumes that the tag has already been read by [`BaseMessage`][base-message].
     """
 
     accumulate: Accumulate[RecordT, RecordT] = AccumulateLastOneWins()
     """
     Accumulate a value from the stream into an existing field value.
     It follows the `read` to decide which value should be assigned to the attribute.
```

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/exceptions.py` & `pure_protobuf-3.0.0a2/pure_protobuf/exceptions.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/helpers/_typing.py` & `pure_protobuf-3.0.0a2/pure_protobuf/helpers/_typing.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/helpers/io.py` & `pure_protobuf-3.0.0a2/pure_protobuf/helpers/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,10 +20,10 @@
     """
     Read the specified number of bytes.
 
     Raises:
         EOFError: the stream has ended
     """
     buffer = io.read(count)
-    if len(buffer) != count:
-        raise EOFError(f"{count} bytes expected, {len(buffer)} read")
+    if len(buffer) < count:
+        raise EOFError(f"{count} bytes expected, but only {len(buffer)} read")
     return buffer
```

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/helpers/itertools.py` & `pure_protobuf-3.0.0a2/pure_protobuf/helpers/itertools.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from pure_protobuf.interfaces._repr import ReprWithInner
 
 P = ParamSpec("P")
 R = TypeVar("R")
 
 
 class ReadCallback(ReprWithInner, Generic[P, R]):
+    """Convert a reader, which returns a singular scalar value, into an iterable reader."""
+
     __slots__ = ("inner",)
 
     # noinspection PyProtocol
     inner: Callable[P, R]
 
     def __init__(self, inner: Callable[P, R]) -> None:  # noqa: D107
         self.inner = inner
```

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/interfaces/_repr.py` & `pure_protobuf-3.0.0a2/pure_protobuf/interfaces/_repr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-from typing_extensions import Protocol
+from typing import Protocol
+
 from typing_extensions import get_args as get_type_args
 
 
 class Repr(Protocol):
     """
     Provides default implementations for `str(self)` and `repr(self)` to make
     debugging easier.
     """
 
     def __str__(self) -> str:
         return repr(self)
 
     def __repr__(self) -> str:
         try:
-            orig_class = self.__orig_class__  # type: ignore
+            orig_class = self.__orig_class__  # type: ignore[attr-defined]
         except AttributeError:
             args = ""
         else:
             args = f"[{get_type_args(orig_class)[0]!r}]"
         return f"{type(self).__name__}{args}()"
 
 
 class ReprWithInner(Repr, Protocol):
     inner: Repr
 
     def __repr__(self) -> str:
         try:
-            orig_class = self.__orig_class__  # type: ignore
+            orig_class = self.__orig_class__  # type: ignore[attr-defined]
         except AttributeError:
             args = ""
         else:
             args = f"[{get_type_args(orig_class)[0]!r}]"
         return f"{type(self).__name__}{args}({self.inner!r})"
```

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/interfaces/_skip.py` & `pure_protobuf-3.0.0a2/pure_protobuf/interfaces/_skip.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from abc import abstractmethod
-from typing import IO
-
-from typing_extensions import Protocol
+from typing import IO, Protocol
 
 from pure_protobuf.interfaces._repr import Repr
 
 
 class Skip(Repr, Protocol):
     """
     Knows how to skip a value. It's equivalent to `Read`, but is supposed to be a little
```

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/interfaces/_vars.py` & `pure_protobuf-3.0.0a2/pure_protobuf/interfaces/_vars.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/interfaces/accumulate.py` & `pure_protobuf-3.0.0a2/pure_protobuf/interfaces/accumulate.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from abc import abstractmethod
-from typing import Iterable, Optional
-
-from typing_extensions import Protocol
+from typing import Iterable, Optional, Protocol
 
 from pure_protobuf.interfaces._repr import Repr
 from pure_protobuf.interfaces._vars import FieldT, RecordT_contra
 
 
 class Accumulate(Repr, Protocol[FieldT, RecordT_contra]):
     """
```

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/interfaces/read.py` & `pure_protobuf-3.0.0a2/pure_protobuf/interfaces/read.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from abc import abstractmethod
-from typing import IO, Iterator
-
-from typing_extensions import Protocol
+from typing import IO, Iterator, Protocol
 
 from pure_protobuf.interfaces._repr import Repr
 from pure_protobuf.interfaces._vars import RecordT_co
 from pure_protobuf.io.wire_type import WireType
 
 
 class ReadSingular(Repr, Protocol[RecordT_co]):
```

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/io/bytes_.py` & `pure_protobuf-3.0.0a2/pure_protobuf/io/bytes_.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/io/struct_.py` & `pure_protobuf-3.0.0a2/pure_protobuf/io/struct_.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from struct import Struct
 from typing import IO, Generic, Iterator
 
+from pure_protobuf.helpers.io import read_checked
 from pure_protobuf.interfaces._repr import ReprWithInner
 from pure_protobuf.interfaces._vars import RecordT_co, RecordT_contra
 from pure_protobuf.interfaces.read import Read
 from pure_protobuf.interfaces.write import Write
 
 
 class ReadStruct(Read[RecordT_co], ReprWithInner, Generic[RecordT_co]):
@@ -14,15 +15,15 @@
 
     # noinspection PyProtocol
     def __init__(self, format_: str) -> None:  # noqa: D107
         self.inner = Struct(format_)
 
     def __call__(self, io: IO[bytes]) -> Iterator[RecordT_co]:
         inner = self.inner
-        yield from inner.unpack(io.read(inner.size))
+        yield from inner.unpack(read_checked(io, inner.size))
 
 
 class WriteStruct(Write[RecordT_contra], ReprWithInner, Generic[RecordT_contra]):
     inner: Struct
 
     __slots__ = ("inner",)
```

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/io/tag.py` & `pure_protobuf-3.0.0a2/pure_protobuf/io/tag.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/io/url.py` & `pure_protobuf-3.0.0a2/pure_protobuf/io/url.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/io/varint.py` & `pure_protobuf-3.0.0a2/pure_protobuf/io/varint.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/io/wire_type.py` & `pure_protobuf-3.0.0a2/pure_protobuf/io/wire_type.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/io/wrappers.py` & `pure_protobuf-3.0.0a2/pure_protobuf/io/wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,20 @@
         else:
             raise UnexpectedWireTypeError(
                 f"expected {self.unpacked_wire_type!r} or a packed record but received {actual_wire_type!r}",
             )
 
 
 class ReadLengthDelimited(Read[RecordT], ReprWithInner):
-    """Wraps the inner reader on a length-delimited buffer."""
+    """
+    Make the inner reader length-delimited.
+
+    This reader wraps the inner reader so that it would first read a byte string,
+    and then call the inner reader on that byte string.
+    """
 
     __slots__ = ("inner",)
 
     # noinspection PyProtocol
     def __init__(self, inner: Read[RecordT]) -> None:
         self.inner = inner
```

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/message.py` & `pure_protobuf-3.0.0a2/pure_protobuf/message.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/one_of.py` & `pure_protobuf-3.0.0a2/pure_protobuf/one_of.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a1/pure_protobuf/well_known.py` & `pure_protobuf-3.0.0a2/pure_protobuf/well_known.py`

 * *Files identical despite different names*

### Comparing `pure_protobuf-3.0.0a1/pyproject.toml` & `pure_protobuf-3.0.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,46 +9,45 @@
 ]
 description = "Protocol Buffers using Python type annotations"
 keywords = ["protobuf", "protocol-buffers"]
 license = "MIT"
 name = "pure-protobuf"
 readme = "README.md"
 repository = "https://github.com/eigenein/protobuf"
-version = "3.0.0a1"
+version = "3.0.0a2"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Typing :: Typed",
 ]
 
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry.dependencies]
 get-annotations = { version = "^0.1.2", python = "<3.10" }
-python = "^3.7.0"
+python = "^3.8.0"
 typing-extensions = "^4.4.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
-mypy = "^1.0.0"
+mypy = "^1.2.0"
 pydantic = "^1.10.4"
 pytest = "^7.2.0"
 pytest-benchmark = "^4.0.0"
 pytest-cov = "^4.0.0"
 ruff = "^0.0.247"
 mkdocs-material = "^9.0.12"
 pillow = "^9.4.0"
@@ -92,19 +91,19 @@
     "pragma: no cover",
     "raise AssertionError",
     "raise NotImplementedError",
 ]
 
 [tool.black]
 line-length = 120
-target-version = ["py37", "py38", "py39", "py310", "py311"]
+target-version = ["py38", "py39", "py310", "py311"]
 
 [tool.ruff]
 line-length = 120
-target-version = "py37"
+target-version = "py38"
 select = [
     "A",
     "ANN",
     "B",
     "C4",
     "COM",
     "D",
```

### Comparing `pure_protobuf-3.0.0a1/PKG-INFO` & `pure_protobuf-3.0.0a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: pure-protobuf
-Version: 3.0.0a1
+Version: 3.0.0a2
 Summary: Protocol Buffers using Python type annotations
 Home-page: https://github.com/eigenein/protobuf
 License: MIT
 Keywords: protobuf,protocol-buffers
 Author: Pavel Perestoronin
 Author-email: eigenein@gmail.com
-Requires-Python: >=3.7.0,<4.0.0
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: get-annotations (>=0.1.2,<0.2.0) ; python_version < "3.10"
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
```

