# Comparing `tmp/uuid6-2022.6.25.tar.gz` & `tmp/uuid6-2023.4.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uuid6-2022.6.25.tar", last modified: Sat Jun 25 16:38:17 2022, max compression
+gzip compressed data, was "uuid6-2023.4.25.tar", last modified: Tue Apr 25 10:03:57 2023, max compression
```

## Comparing `uuid6-2022.6.25.tar` & `uuid6-2023.4.25.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 16:38:17.386726 uuid6-2022.6.25/
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-06-25 16:38:03.000000 uuid6-2022.6.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6777 2022-06-25 16:38:17.382726 uuid6-2022.6.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5959 2022-06-25 16:38:03.000000 uuid6-2022.6.25/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-06-25 16:38:03.000000 uuid6-2022.6.25/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-25 16:38:17.386726 uuid6-2022.6.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1633 2022-06-25 16:38:03.000000 uuid6-2022.6.25/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 16:38:17.382726 uuid6-2022.6.25/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 16:38:17.382726 uuid6-2022.6.25/src/uuid6/
--rw-r--r--   0 runner    (1001) docker     (121)     4402 2022-06-25 16:38:03.000000 uuid6-2022.6.25/src/uuid6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-25 16:38:03.000000 uuid6-2022.6.25/src/uuid6/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 16:38:17.382726 uuid6-2022.6.25/src/uuid6.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6777 2022-06-25 16:38:16.000000 uuid6-2022.6.25/src/uuid6.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-06-25 16:38:17.000000 uuid6-2022.6.25/src/uuid6.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-25 16:38:16.000000 uuid6-2022.6.25/src/uuid6.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-25 16:38:16.000000 uuid6-2022.6.25/src/uuid6.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-25 16:38:17.000000 uuid6-2022.6.25/src/uuid6.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 16:38:17.382726 uuid6-2022.6.25/test/
--rw-r--r--   0 runner    (1001) docker     (121)     4648 2022-06-25 16:38:03.000000 uuid6-2022.6.25/test/test_uuid6.py
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-06-25 16:38:03.000000 uuid6-2022.6.25/test/test_vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:03:57.554544 uuid6-2023.4.25/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-25 10:03:43.000000 uuid6-2023.4.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-25 10:03:57.554544 uuid6-2023.4.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-04-25 10:03:43.000000 uuid6-2023.4.25/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-25 10:03:43.000000 uuid6-2023.4.25/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 10:03:57.554544 uuid6-2023.4.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-25 10:03:43.000000 uuid6-2023.4.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:03:57.550544 uuid6-2023.4.25/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:03:57.554544 uuid6-2023.4.25/src/uuid6/
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-04-25 10:03:43.000000 uuid6-2023.4.25/src/uuid6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:03:43.000000 uuid6-2023.4.25/src/uuid6/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:03:57.554544 uuid6-2023.4.25/src/uuid6.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-25 10:03:57.000000 uuid6-2023.4.25/src/uuid6.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-25 10:03:57.000000 uuid6-2023.4.25/src/uuid6.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:03:57.000000 uuid6-2023.4.25/src/uuid6.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:03:57.000000 uuid6-2023.4.25/src/uuid6.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 10:03:57.000000 uuid6-2023.4.25/src/uuid6.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:03:57.554544 uuid6-2023.4.25/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-04-25 10:03:43.000000 uuid6-2023.4.25/test/test_uuid6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-25 10:03:43.000000 uuid6-2023.4.25/test/test_vectors.py
```

### Comparing `uuid6-2022.6.25/LICENSE` & `uuid6-2023.4.25/LICENSE`

 * *Files identical despite different names*

### Comparing `uuid6-2022.6.25/PKG-INFO` & `uuid6-2023.4.25/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,72 @@
 Metadata-Version: 2.1
 Name: uuid6
-Version: 2022.6.25
+Version: 2023.4.25
 Summary: New time-based UUID formats which are suited for use as a database key
 Home-page: https://github.com/oittaa/uuid6-python
 Author: Oittaa
 Author-email: 
-Keywords: uuid,uuid6,uuid7,uuidv6,uuidv7
+Keywords: uuid,uuid6,uuid7,uuid8,uuidv6,uuidv7,uuidv8
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # uuid6
 New time-based UUID formats which are suited for use as a database key.
 
 [![CI](https://github.com/oittaa/uuid6-python/actions/workflows/main.yml/badge.svg)](https://github.com/oittaa/uuid6-python/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/oittaa/uuid6-python/branch/main/graph/badge.svg?token=O59DZ6UWQV)](https://codecov.io/gh/oittaa/uuid6-python)
 [![PyPI status](https://badge.fury.io/py/uuid6.svg)](https://pypi.org/project/uuid6/)
 [![Python versions supported](https://img.shields.io/pypi/pyversions/uuid6.svg?logo=python)](https://pypi.org/project/uuid6/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-This module extends immutable UUID objects (the UUID class) with the functions `uuid6()` and `uuid7()` from [the IETF draft][draft repository].
+This module extends immutable UUID objects (the UUID class) with the functions `uuid6()`, `uuid7()`, and `uuid8()` from [the IETF draft][draft repository].
 
 ## Install
 
 ```shell
 pip install uuid6
 ```
 
 ## Usage
 
 ```python
-from uuid6 import uuid6, uuid7
+from uuid6 import uuid6, uuid7, uuid8
 
 my_uuid = uuid6()
 print(my_uuid)
 assert my_uuid < uuid6()
 
 my_uuid = uuid7()
 print(my_uuid)
 assert my_uuid < uuid7()
+
+my_uuid = uuid8()
+print(my_uuid)
+assert my_uuid < uuid8()
 ```
 
+## Which UUID version should I use?
+
+> Implementations SHOULD utilize UUID version 7 over UUID version 1 and 6 if possible.
+
+UUID version 7 features a time-ordered value field derived from the widely implemented and well known Unix Epoch timestamp source, the number of milliseconds since midnight 1 Jan 1970 UTC, leap seconds excluded. As well as improved entropy characteristics over versions 1 or 6.
+
+If your use case requires greater granularity than UUID version 7 can provide, you might consider UUID version 8. UUID version 8 doesn't provide as good entropy characteristics as UUID version 7, but it utilizes timestamp with nanosecond level of precision.
+
 ## UUIDv6 Field and Bit Layout
 
 ```
         0                   1                   2                   3
         0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |                           time_high                           |
@@ -65,31 +77,29 @@
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |                         node (2-5)                            |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 ```
 
 ## UUIDv7 Field and Bit Layout
 
-### [Draft 04][draft 04]
-
 ```
         0                   1                   2                   3
         0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |                           unix_ts_ms                          |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |          unix_ts_ms           |  ver  |       rand_a          |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |var|                        rand_b                             |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |                            rand_b                             |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 ```
 
-### This implementation
+## UUIDv8 Field and Bit Layout
 
 ```
         0                   1                   2                   3
         0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |                           unix_ts_ms                          |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
@@ -98,53 +108,39 @@
         |var|   subsec_b    |         rand                              |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |                             rand                              |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 ```
 
 - `unix_ts_ms`: 48 bit big-endian unsigned number of Unix epoch timestamp with millisecond level of precision
-- `ver`: The 4 bit UUIDv7 version (0111)
+- `ver`: The 4 bit UUIDv8 version (1000)
 - `subsec_a`: 12 bits allocated to sub-second precision values
 - `var`: 2 bit UUID variant (10)
 - `subsec_b`: 8 bits allocated to sub-second precision values
-- `rand`: The remaining 54 bits are filled with pseudo-random data
+- `rand`: The remaining 54 bits are filled with [cryptographically strong random data][python randbits]
 
- 20 extra bits dedicated to sub-second precision provide nanosecond resolution. The `unix_ts` and `subsec` fields guarantee the order of UUIDs generated within the same nanosecond by monotonically incrementing the timer.
+ 20 extra bits dedicated to sub-second precision provide nanosecond resolution. The `unix_ts_ms`, `subsec_a`,  and `subsec_b` fields guarantee the order of UUIDs generated within the same nanosecond by monotonically incrementing the timer.
 
 ## Performance
 
 Run the shell script [bench.sh][bench] to test on your own machine.
 
 ### Results
 
 MacBook Air 2020
 ```
-Python 3.10.2
-Mean +- std dev: 1.02 us +- 0.01 us
-Mean +- std dev: 1.13 us +- 0.02 us
-Mean +- std dev: 2.33 us +- 0.02 us
-Mean +- std dev: 1.91 us +- 0.02 us
-+-----------+---------+-----------------------+-----------------------+-----------------------+
-| Benchmark | uuid1   | uuid4                 | uuid6                 | uuid7                 |
-+===========+=========+=======================+=======================+=======================+
-| timeit    | 1.02 us | 1.13 us: 1.11x slower | 2.33 us: 2.29x slower | 1.91 us: 1.87x slower |
-+-----------+---------+-----------------------+-----------------------+-----------------------+
-```
-
-Google [Cloud Shell][cloud shell] VM
-```
-Python 3.9.2
-Mean +- std dev: 12.6 us +- 0.5 us
-Mean +- std dev: 3.06 us +- 0.14 us
-Mean +- std dev: 6.42 us +- 0.37 us
-Mean +- std dev: 4.94 us +- 0.24 us
-+-----------+---------+-----------------------+-----------------------+-----------------------+
-| Benchmark | uuid1   | uuid4                 | uuid6                 | uuid7                 |
-+===========+=========+=======================+=======================+=======================+
-| timeit    | 12.6 us | 3.06 us: 4.11x faster | 6.42 us: 1.95x faster | 4.94 us: 2.54x faster |
-+-----------+---------+-----------------------+-----------------------+-----------------------+
-```
-
-[draft repository]: https://github.com/uuid6/uuid6-ietf-draft
-[draft 04]: https://datatracker.ietf.org/doc/html/draft-peabody-dispatch-new-uuid-format-04#section-5.2
-[cloud shell]: https://cloud.google.com/shell/docs
+Python 3.10.4
+Mean +- std dev: 870 ns +- 11 ns
+Mean +- std dev: 1.17 us +- 0.01 us
+Mean +- std dev: 2.18 us +- 0.02 us
+Mean +- std dev: 1.60 us +- 0.02 us
+Mean +- std dev: 1.78 us +- 0.02 us
++-----------+--------+-----------------------+-----------------------+-----------------------+-----------------------+
+| Benchmark | uuid1  | uuid4                 | uuid6                 | uuid7                 | uuid8                 |
++===========+========+=======================+=======================+=======================+=======================+
+| timeit    | 870 ns | 1.17 us: 1.35x slower | 2.18 us: 2.51x slower | 1.60 us: 1.84x slower | 1.78 us: 2.04x slower |
++-----------+--------+-----------------------+-----------------------+-----------------------+-----------------------+
+```
+
+[draft repository]: https://github.com/ietf-wg-uuidrev/rfc4122bis
+[python randbits]: https://docs.python.org/3/library/secrets.html#secrets.randbits
 [bench]: https://github.com/oittaa/uuid6-python/blob/main/bench.sh
```

### Comparing `uuid6-2022.6.25/setup.py` & `uuid6-2023.4.25/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,32 +29,34 @@
     author_email=AUTHOR_EMAIL,
     include_package_data=True,
     zip_safe=False,
     keywords=[
         "uuid",
         "uuid6",
         "uuid7",
+        "uuid8",
         "uuidv6",
         "uuidv7",
+        "uuidv8",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     setup_requires=[
         "wheel",
     ],
     package_dir={"": "src"},
     package_data={
         "": ["py.typed"],
     },
     packages=find_packages(where="src"),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 )
```

### Comparing `uuid6-2022.6.25/src/uuid6/__init__.py` & `uuid6-2023.4.25/src/uuid6/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 r"""UUID draft version objects (universally unique identifiers).
-This module provides the functions uuid6() and uuid7() for
-generating version 6 and 7 UUIDs as specified in
-https://github.com/uuid6/uuid6-ietf-draft.
+This module provides the functions uuid6(), uuid7(), and uuid8() for
+generating version 6, 7, and 8 UUIDs as specified in
+https://github.com/ietf-wg-uuidrev/rfc4122bis
 """
 
 import secrets
 import time
 import uuid
-from typing import Tuple
+from typing import Optional, Tuple
 
 
 class UUID(uuid.UUID):
     r"""UUID draft version objects"""
 
+    __slots__ = ()
+
     def __init__(
         self,
-        hex: str = None,
-        bytes: bytes = None,
-        bytes_le: bytes = None,
-        fields: Tuple[int, int, int, int, int, int] = None,
-        int: int = None,
-        version: int = None,
+        hex: Optional[str] = None,
+        bytes: Optional[bytes] = None,
+        bytes_le: Optional[bytes] = None,
+        fields: Optional[Tuple[int, int, int, int, int, int]] = None,
+        int: Optional[int] = None,
+        version: Optional[int] = None,
         *,
-        is_safe=uuid.SafeUUID.unknown
+        is_safe: uuid.SafeUUID = uuid.SafeUUID.unknown
     ) -> None:
         r"""Create a UUID."""
 
         if int is None or [hex, bytes, bytes_le, fields].count(None) != 4:
             return super().__init__(
                 hex=hex,
                 bytes=bytes,
@@ -35,15 +37,15 @@
                 int=int,
                 version=version,
                 is_safe=is_safe,
             )
         if not 0 <= int < 1 << 128:
             raise ValueError("int is out of range (need a 128-bit value)")
         if version is not None:
-            if not 6 <= version <= 7:
+            if not 6 <= version <= 8:
                 raise ValueError("illegal version number")
             # Set the variant to RFC 4122.
             int &= ~(0xC000 << 48)
             int |= 0x8000 << 48
             # Set the version number.
             int &= ~(0xF000 << 64)
             int |= version << 76
@@ -58,74 +60,98 @@
         if self.version == 6:
             return (
                 (self.time_low << 28)
                 | (self.time_mid << 12)
                 | (self.time_hi_version & 0x0FFF)
             )
         if self.version == 7:
+            return self.int >> 80
+        if self.version == 8:
             return (self.int >> 80) * 10**6 + _subsec_decode(self.subsec)
         return super().time
 
 
 def _subsec_decode(value: int) -> int:
     return -(-value * 10**6 // 2**20)
 
 
 def _subsec_encode(value: int) -> int:
     return value * 2**20 // 10**6
 
 
 _last_v6_timestamp = None
 _last_v7_timestamp = None
+_last_v8_timestamp = None
+
 
+def uuid6(clock_seq: Optional[int] = None) -> UUID:
+    r"""UUID version 6 is a field-compatible version of UUIDv1, reordered for
+    improved DB locality. It is expected that UUIDv6 will primarily be
+    used in contexts where there are existing v1 UUIDs. Systems that do
+    not involve legacy UUIDv1 SHOULD consider using UUIDv7 instead.
 
-def uuid6(clock_seq: int = None) -> UUID:
-    r"""Generate a UUID from sequence number, and the current time.
     If 'clock_seq' is given, it is used as the sequence number;
     otherwise a random 14-bit sequence number is chosen."""
 
     global _last_v6_timestamp
 
     nanoseconds = time.time_ns()
     # 0x01b21dd213814000 is the number of 100-ns intervals between the
     # UUID epoch 1582-10-15 00:00:00 and the Unix epoch 1970-01-01 00:00:00.
     timestamp = nanoseconds // 100 + 0x01B21DD213814000
     if _last_v6_timestamp is not None and timestamp <= _last_v6_timestamp:
         timestamp = _last_v6_timestamp + 1
     _last_v6_timestamp = timestamp
     if clock_seq is None:
         clock_seq = secrets.randbits(14)  # instead of stable storage
-    node = secrets.randbits(48)
     time_high_and_time_mid = (timestamp >> 12) & 0xFFFFFFFFFFFF
     time_low_and_version = timestamp & 0x0FFF
     uuid_int = time_high_and_time_mid << 80
     uuid_int |= time_low_and_version << 64
     uuid_int |= (clock_seq & 0x3FFF) << 48
-    uuid_int |= node
+    uuid_int |= secrets.randbits(48)
     return UUID(int=uuid_int, version=6)
 
 
 def uuid7() -> UUID:
-    r"""The UUIDv7 format is designed to encode a Unix timestamp with
-    arbitrary sub-second precision.  The key property provided by UUIDv7
-    is that timestamp values generated by one system and parsed by
-    another are guaranteed to have sub-second precision of either the
-    generator or the parser, whichever is less.  Additionally, the system
-    parsing the UUIDv7 value does not need to know which precision was
-    used during encoding in order to function correctly."""
+    r"""UUID version 7 features a time-ordered value field derived from the
+    widely implemented and well known Unix Epoch timestamp source, the
+    number of milliseconds since midnight 1 Jan 1970 UTC, leap seconds
+    excluded. As well as improved entropy characteristics over versions
+    1 or 6.
+
+    Implementations SHOULD utilize UUID version 7 over UUID version 1 and
+    6 if possible."""
 
     global _last_v7_timestamp
 
     nanoseconds = time.time_ns()
-    if _last_v7_timestamp is not None and nanoseconds <= _last_v7_timestamp:
-        nanoseconds = _last_v7_timestamp + 1
-    _last_v7_timestamp = nanoseconds
+    timestamp_ms = nanoseconds // 10**6
+    if _last_v7_timestamp is not None and timestamp_ms <= _last_v7_timestamp:
+        timestamp_ms = _last_v7_timestamp + 1
+    _last_v7_timestamp = timestamp_ms
+    uuid_int = (timestamp_ms & 0xFFFFFFFFFFFF) << 80
+    uuid_int |= secrets.randbits(76)
+    return UUID(int=uuid_int, version=7)
+
+
+def uuid8() -> UUID:
+    r"""UUID version 8 features a time-ordered value field derived from the
+    widely implemented and well known Unix Epoch timestamp source, the
+    number of nanoseconds since midnight 1 Jan 1970 UTC, leap seconds
+    excluded."""
+
+    global _last_v8_timestamp
+
+    nanoseconds = time.time_ns()
+    if _last_v8_timestamp is not None and nanoseconds <= _last_v8_timestamp:
+        nanoseconds = _last_v8_timestamp + 1
+    _last_v8_timestamp = nanoseconds
     timestamp_ms, timestamp_ns = divmod(nanoseconds, 10**6)
     subsec = _subsec_encode(timestamp_ns)
     subsec_a = subsec >> 8
     subsec_b = subsec & 0xFF
-    rand = secrets.randbits(54)
     uuid_int = (timestamp_ms & 0xFFFFFFFFFFFF) << 80
     uuid_int |= subsec_a << 64
     uuid_int |= subsec_b << 54
-    uuid_int |= rand
-    return UUID(int=uuid_int, version=7)
+    uuid_int |= secrets.randbits(54)
+    return UUID(int=uuid_int, version=8)
```

### Comparing `uuid6-2022.6.25/src/uuid6.egg-info/PKG-INFO` & `uuid6-2023.4.25/src/uuid6.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,72 @@
 Metadata-Version: 2.1
 Name: uuid6
-Version: 2022.6.25
+Version: 2023.4.25
 Summary: New time-based UUID formats which are suited for use as a database key
 Home-page: https://github.com/oittaa/uuid6-python
 Author: Oittaa
 Author-email: 
-Keywords: uuid,uuid6,uuid7,uuidv6,uuidv7
+Keywords: uuid,uuid6,uuid7,uuid8,uuidv6,uuidv7,uuidv8
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # uuid6
 New time-based UUID formats which are suited for use as a database key.
 
 [![CI](https://github.com/oittaa/uuid6-python/actions/workflows/main.yml/badge.svg)](https://github.com/oittaa/uuid6-python/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/oittaa/uuid6-python/branch/main/graph/badge.svg?token=O59DZ6UWQV)](https://codecov.io/gh/oittaa/uuid6-python)
 [![PyPI status](https://badge.fury.io/py/uuid6.svg)](https://pypi.org/project/uuid6/)
 [![Python versions supported](https://img.shields.io/pypi/pyversions/uuid6.svg?logo=python)](https://pypi.org/project/uuid6/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-This module extends immutable UUID objects (the UUID class) with the functions `uuid6()` and `uuid7()` from [the IETF draft][draft repository].
+This module extends immutable UUID objects (the UUID class) with the functions `uuid6()`, `uuid7()`, and `uuid8()` from [the IETF draft][draft repository].
 
 ## Install
 
 ```shell
 pip install uuid6
 ```
 
 ## Usage
 
 ```python
-from uuid6 import uuid6, uuid7
+from uuid6 import uuid6, uuid7, uuid8
 
 my_uuid = uuid6()
 print(my_uuid)
 assert my_uuid < uuid6()
 
 my_uuid = uuid7()
 print(my_uuid)
 assert my_uuid < uuid7()
+
+my_uuid = uuid8()
+print(my_uuid)
+assert my_uuid < uuid8()
 ```
 
+## Which UUID version should I use?
+
+> Implementations SHOULD utilize UUID version 7 over UUID version 1 and 6 if possible.
+
+UUID version 7 features a time-ordered value field derived from the widely implemented and well known Unix Epoch timestamp source, the number of milliseconds since midnight 1 Jan 1970 UTC, leap seconds excluded. As well as improved entropy characteristics over versions 1 or 6.
+
+If your use case requires greater granularity than UUID version 7 can provide, you might consider UUID version 8. UUID version 8 doesn't provide as good entropy characteristics as UUID version 7, but it utilizes timestamp with nanosecond level of precision.
+
 ## UUIDv6 Field and Bit Layout
 
 ```
         0                   1                   2                   3
         0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |                           time_high                           |
@@ -65,31 +77,29 @@
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |                         node (2-5)                            |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 ```
 
 ## UUIDv7 Field and Bit Layout
 
-### [Draft 04][draft 04]
-
 ```
         0                   1                   2                   3
         0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |                           unix_ts_ms                          |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |          unix_ts_ms           |  ver  |       rand_a          |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |var|                        rand_b                             |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |                            rand_b                             |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 ```
 
-### This implementation
+## UUIDv8 Field and Bit Layout
 
 ```
         0                   1                   2                   3
         0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |                           unix_ts_ms                          |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
@@ -98,53 +108,39 @@
         |var|   subsec_b    |         rand                              |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
         |                             rand                              |
         +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
 ```
 
 - `unix_ts_ms`: 48 bit big-endian unsigned number of Unix epoch timestamp with millisecond level of precision
-- `ver`: The 4 bit UUIDv7 version (0111)
+- `ver`: The 4 bit UUIDv8 version (1000)
 - `subsec_a`: 12 bits allocated to sub-second precision values
 - `var`: 2 bit UUID variant (10)
 - `subsec_b`: 8 bits allocated to sub-second precision values
-- `rand`: The remaining 54 bits are filled with pseudo-random data
+- `rand`: The remaining 54 bits are filled with [cryptographically strong random data][python randbits]
 
- 20 extra bits dedicated to sub-second precision provide nanosecond resolution. The `unix_ts` and `subsec` fields guarantee the order of UUIDs generated within the same nanosecond by monotonically incrementing the timer.
+ 20 extra bits dedicated to sub-second precision provide nanosecond resolution. The `unix_ts_ms`, `subsec_a`,  and `subsec_b` fields guarantee the order of UUIDs generated within the same nanosecond by monotonically incrementing the timer.
 
 ## Performance
 
 Run the shell script [bench.sh][bench] to test on your own machine.
 
 ### Results
 
 MacBook Air 2020
 ```
-Python 3.10.2
-Mean +- std dev: 1.02 us +- 0.01 us
-Mean +- std dev: 1.13 us +- 0.02 us
-Mean +- std dev: 2.33 us +- 0.02 us
-Mean +- std dev: 1.91 us +- 0.02 us
-+-----------+---------+-----------------------+-----------------------+-----------------------+
-| Benchmark | uuid1   | uuid4                 | uuid6                 | uuid7                 |
-+===========+=========+=======================+=======================+=======================+
-| timeit    | 1.02 us | 1.13 us: 1.11x slower | 2.33 us: 2.29x slower | 1.91 us: 1.87x slower |
-+-----------+---------+-----------------------+-----------------------+-----------------------+
-```
-
-Google [Cloud Shell][cloud shell] VM
-```
-Python 3.9.2
-Mean +- std dev: 12.6 us +- 0.5 us
-Mean +- std dev: 3.06 us +- 0.14 us
-Mean +- std dev: 6.42 us +- 0.37 us
-Mean +- std dev: 4.94 us +- 0.24 us
-+-----------+---------+-----------------------+-----------------------+-----------------------+
-| Benchmark | uuid1   | uuid4                 | uuid6                 | uuid7                 |
-+===========+=========+=======================+=======================+=======================+
-| timeit    | 12.6 us | 3.06 us: 4.11x faster | 6.42 us: 1.95x faster | 4.94 us: 2.54x faster |
-+-----------+---------+-----------------------+-----------------------+-----------------------+
-```
-
-[draft repository]: https://github.com/uuid6/uuid6-ietf-draft
-[draft 04]: https://datatracker.ietf.org/doc/html/draft-peabody-dispatch-new-uuid-format-04#section-5.2
-[cloud shell]: https://cloud.google.com/shell/docs
+Python 3.10.4
+Mean +- std dev: 870 ns +- 11 ns
+Mean +- std dev: 1.17 us +- 0.01 us
+Mean +- std dev: 2.18 us +- 0.02 us
+Mean +- std dev: 1.60 us +- 0.02 us
+Mean +- std dev: 1.78 us +- 0.02 us
++-----------+--------+-----------------------+-----------------------+-----------------------+-----------------------+
+| Benchmark | uuid1  | uuid4                 | uuid6                 | uuid7                 | uuid8                 |
++===========+========+=======================+=======================+=======================+=======================+
+| timeit    | 870 ns | 1.17 us: 1.35x slower | 2.18 us: 2.51x slower | 1.60 us: 1.84x slower | 1.78 us: 2.04x slower |
++-----------+--------+-----------------------+-----------------------+-----------------------+-----------------------+
+```
+
+[draft repository]: https://github.com/ietf-wg-uuidrev/rfc4122bis
+[python randbits]: https://docs.python.org/3/library/secrets.html#secrets.randbits
 [bench]: https://github.com/oittaa/uuid6-python/blob/main/bench.sh
```

### Comparing `uuid6-2022.6.25/test/test_uuid6.py` & `uuid6-2023.4.25/test/test_uuid6.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import unittest
 from time import time_ns
 from unittest.mock import patch
 from uuid import uuid1
 
-from uuid6 import UUID, uuid6, uuid7
+from uuid6 import UUID, uuid6, uuid7, uuid8
 
 REGEX_UUID6 = r"^[0-9a-f]{8}-[0-9a-f]{4}-6[0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}$"
 REGEX_UUID7 = r"^[0-9a-f]{8}-[0-9a-f]{4}-7[0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}$"
+REGEX_UUID8 = r"^[0-9a-f]{8}-[0-9a-f]{4}-8[0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}$"
 YEAR_IN_NS = 3600 * 24 * 36525 * 10**7
 
 
 class UUIDTests(unittest.TestCase):
     def test_uuid6_generation(self):
         uuid6_1 = uuid6()
         self.assertEqual(uuid6_1.version, 6)
@@ -25,14 +26,23 @@
         self.assertEqual(uuid7_1.version, 7)
         for _ in range(1000):
             self.assertRegex(str(uuid7_1), REGEX_UUID7)
             uuid7_2 = uuid7()
             self.assertLess(uuid7_1, uuid7_2)
             uuid7_1 = uuid7_2
 
+    def test_uuid8_generation(self):
+        uuid8_1 = uuid8()
+        self.assertEqual(uuid8_1.version, 8)
+        for _ in range(1000):
+            self.assertRegex(str(uuid8_1), REGEX_UUID8)
+            uuid8_2 = uuid8()
+            self.assertLess(uuid8_1, uuid8_2)
+            uuid8_1 = uuid8_2
+
     def test_invalid_int(self):
         with self.assertRaises(ValueError):
             _ = UUID(int=-1)
         with self.assertRaises(ValueError):
             _ = UUID(int=1 << 128)
 
     def test_valid_int(self):
@@ -51,14 +61,23 @@
     def test_uuid7_same_nanosecond(self, mocktime):
         uuid7_1 = uuid7()
         for _ in range(1000):
             uuid7_2 = uuid7()
             self.assertLess(uuid7_1, uuid7_2)
             uuid7_1 = uuid7_2
 
+    @patch("uuid6._last_v8_timestamp", 1)
+    @patch("time.time_ns", return_value=1234)
+    def test_uuid8_same_nanosecond(self, mocktime):
+        uuid8_1 = uuid8()
+        for _ in range(1000):
+            uuid8_2 = uuid8()
+            self.assertLess(uuid8_1, uuid8_2)
+            uuid8_1 = uuid8_2
+
     @patch("uuid6._last_v6_timestamp", 1)
     @patch("secrets.randbits", return_value=678)
     @patch("time.time_ns", return_value=12345)
     def test_uuid6_fields_without_randomness(self, mocktime, mockrand):
         uuid6_1 = uuid6(clock_seq=123)
         for _ in range(10):
             uuid6_2 = uuid6(clock_seq=123)
@@ -92,33 +111,49 @@
             uuid_prev = uuid7()
         for i in range(1, 8000, 10):
             with patch("time.time_ns", return_value=i * YEAR_IN_NS):
                 uuid_cur = uuid7()
                 self.assertLess(uuid_prev, uuid_cur)
                 uuid_prev = uuid_cur
 
+    @patch("uuid6._last_v8_timestamp", 1)
+    def test_uuid8_far_in_future(self):
+        with patch("time.time_ns", return_value=1):
+            uuid_prev = uuid8()
+        for i in range(1, 8000, 10):
+            with patch("time.time_ns", return_value=i * YEAR_IN_NS):
+                uuid_cur = uuid8()
+                self.assertLess(uuid_prev, uuid_cur)
+                uuid_prev = uuid_cur
+
     def test_time(self):
         uuid_1 = uuid1()
         uuid_6 = uuid6()
         self.assertAlmostEqual(uuid_6.time / 10**7, uuid_1.time / 10**7, 3)
         cur_time = time_ns()
         uuid_7 = uuid7()
-        self.assertAlmostEqual(uuid_7.time / 10**9, cur_time / 10**9, 3)
+        self.assertAlmostEqual(uuid_7.time / 10**3, cur_time / 10**9, 2)
+        uuid_8 = uuid8()
+        self.assertAlmostEqual(uuid_8.time / 10**9, cur_time / 10**9, 3)
 
     def test_zero_time(self):
         uuid_6 = UUID(hex="00000000-0000-6000-8000-000000000000")
         self.assertEqual(uuid_6.time, 0)
         uuid_7 = UUID(hex="00000000-0000-7000-8000-000000000000")
         self.assertEqual(uuid_7.time, 0)
+        uuid_8 = UUID(hex="00000000-0000-8000-8000-000000000000")
+        self.assertEqual(uuid_8.time, 0)
 
     def test_max_time(self):
         uuid_6 = UUID(hex="ffffffff-ffff-6fff-bfff-ffffffffffff")
         self.assertEqual(uuid_6.time, 1152921504606846975)
         uuid_7 = UUID(hex="ffffffff-ffff-7fff-bfff-ffffffffffff")
-        self.assertEqual(uuid_7.time, 281474976710656000000)
+        self.assertEqual(uuid_7.time, 281474976710655)
+        uuid_8 = UUID(hex="ffffffff-ffff-8fff-bfff-ffffffffffff")
+        self.assertEqual(uuid_8.time, 281474976710656000000)
 
     def test_multiple_arguments(self):
         with self.assertRaises(TypeError):
             _ = UUID(int=0, hex="061d0edc-bea0-75cc-9892-f6295fd7d295")
 
 
 if __name__ == "__main__":
```

