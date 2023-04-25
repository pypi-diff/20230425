# Comparing `tmp/upathlib-0.7.9.tar.gz` & `tmp/upathlib-0.8.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upathlib-0.7.9.tar", last modified: Mon Apr 24 18:30:06 2023, max compression
+gzip compressed data, was "upathlib-0.8.0b1.tar", last modified: Tue Apr 25 07:51:21 2023, max compression
```

## Comparing `upathlib-0.7.9.tar` & `upathlib-0.8.0b1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2022-12-13 07:44:37.384893 upathlib-0.7.9/LICENSE
--rw-r--r--   0        0        0      993 2023-03-30 16:49:23.794031 upathlib-0.7.9/README.rst
--rw-r--r--   0        0        0     1726 2023-04-24 18:14:03.529696 upathlib-0.7.9/pyproject.toml
--rw-r--r--   0        0        0     2317 2023-04-24 18:28:07.086273 upathlib-0.7.9/src/upathlib/__init__.py
--rw-r--r--   0        0        0     4694 2023-04-20 04:34:46.179551 upathlib-0.7.9/src/upathlib/_blob.py
--rw-r--r--   0        0        0    10997 2023-04-20 04:34:46.179551 upathlib-0.7.9/src/upathlib/_local.py
--rw-r--r--   0        0        0     7935 2023-04-20 04:34:46.179551 upathlib-0.7.9/src/upathlib/_tests.py
--rw-r--r--   0        0        0    34513 2023-04-24 18:21:32.197286 upathlib-0.7.9/src/upathlib/_upath.py
--rw-r--r--   0        0        0    12562 2023-04-10 08:06:32.346660 upathlib-0.7.9/src/upathlib/azure.py
--rw-r--r--   0        0        0    26106 2023-04-24 18:21:32.197286 upathlib-0.7.9/src/upathlib/gcs.py
--rw-r--r--   0        0        0        0 2022-12-13 07:44:37.384893 upathlib-0.7.9/src/upathlib/py.typed
--rw-r--r--   0        0        0     3763 2023-04-10 08:06:32.346660 upathlib-0.7.9/src/upathlib/serializer.py
--rw-r--r--   0        0        0     2381 1970-01-01 00:00:00.000000 upathlib-0.7.9/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-12-13 07:44:37.384893 upathlib-0.8.0b1/LICENSE
+-rw-r--r--   0        0        0      993 2023-03-30 16:49:23.794031 upathlib-0.8.0b1/README.rst
+-rw-r--r--   0        0        0     1726 2023-04-25 03:21:53.568059 upathlib-0.8.0b1/pyproject.toml
+-rw-r--r--   0        0        0     2321 2023-04-25 07:47:53.076783 upathlib-0.8.0b1/src/upathlib/__init__.py
+-rw-r--r--   0        0        0     4694 2023-04-20 04:34:46.179551 upathlib-0.8.0b1/src/upathlib/_blob.py
+-rw-r--r--   0        0        0    10954 2023-04-25 03:21:53.568059 upathlib-0.8.0b1/src/upathlib/_local.py
+-rw-r--r--   0        0        0     7935 2023-04-20 04:34:46.179551 upathlib-0.8.0b1/src/upathlib/_tests.py
+-rw-r--r--   0        0        0    34484 2023-04-25 03:21:53.568059 upathlib-0.8.0b1/src/upathlib/_upath.py
+-rw-r--r--   0        0        0    12562 2023-04-10 08:06:32.346660 upathlib-0.8.0b1/src/upathlib/azure.py
+-rw-r--r--   0        0        0    25613 2023-04-25 07:49:10.489394 upathlib-0.8.0b1/src/upathlib/gcs.py
+-rw-r--r--   0        0        0        0 2022-12-13 07:44:37.384893 upathlib-0.8.0b1/src/upathlib/py.typed
+-rw-r--r--   0        0        0     3763 2023-04-10 08:06:32.346660 upathlib-0.8.0b1/src/upathlib/serializer.py
+-rw-r--r--   0        0        0     2383 1970-01-01 00:00:00.000000 upathlib-0.8.0b1/PKG-INFO
```

### Comparing `upathlib-0.7.9/LICENSE` & `upathlib-0.8.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.9/README.rst` & `upathlib-0.8.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.9/pyproject.toml` & `upathlib-0.8.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.9/src/upathlib/__init__.py` & `upathlib-0.8.0b1/src/upathlib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 
 One use case is the package `biglist <https://biglist.readthedocs.io/en/latest/>`__,
 where the class `Biglist <https://biglist.readthedocs.io/en/latest/#biglist.Biglist>`__ takes a Upath object to indicate its location of storage.
 It does not care whether the storage is local or in a cloud blob store---it
 simply uses the common API to operate the storage.
 """
 
-__version__ = "0.7.9"
+__version__ = "0.8.0b1"
+
+
 from pathlib import Path
 from typing import Union
 
 from ._blob import BlobUpath
 from ._local import LocalPathType, LocalUpath
 from ._upath import FileInfo, LockAcquireError, LockReleaseError, Upath
```

### Comparing `upathlib-0.7.9/src/upathlib/_blob.py` & `upathlib-0.8.0b1/src/upathlib/_blob.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.9/src/upathlib/_local.py` & `upathlib-0.8.0b1/src/upathlib/_local.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import os.path
 import pathlib
 import shutil
 import sys
 import time
 from collections.abc import Iterator
 from io import BufferedReader
-from typing import Optional, Union
 
 import filelock
 
 # `filelock` is also called `py-filelock`.
 # Tried `fasteners` also. In one use case,
 # `filelock` worked whereas `fasteners.InterprocessLock` failed.
 #
@@ -101,15 +100,15 @@
 
     def is_file(self) -> bool:
         """
         Return whether the current path is a file.
         """
         return self.path.is_file()
 
-    def file_info(self) -> Optional[FileInfo]:
+    def file_info(self) -> FileInfo | None:
         """
         Return file info if the current path is a file;
         otherwise return ``None``.
         """
         if not self.is_file():
             return None
         st = self.path.stat()
@@ -332,8 +331,8 @@
         finally:
             try:
                 lock.release()  # in a re-entry situation, this may not actually "release" the lock
             except Exception as e:
                 raise LockReleaseError(f"failed to release lock on file {self}") from e
 
 
-LocalPathType = Union[str, pathlib.Path, LocalUpath]
+LocalPathType = str | pathlib.Path | LocalUpath
```

### Comparing `upathlib-0.7.9/src/upathlib/_tests.py` & `upathlib-0.8.0b1/src/upathlib/_tests.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.9/src/upathlib/_upath.py` & `upathlib-0.8.0b1/src/upathlib/_upath.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 import threading
 from collections.abc import Iterable, Iterator
 from dataclasses import dataclass
 from io import BufferedReader, UnsupportedOperation
 from typing import (
     Any,
     Callable,
-    Optional,
 )
 
 from mpservice.concurrent.futures import get_shared_thread_pool
 from mpservice.threading import MAX_THREADS
 from tqdm.auto import tqdm
 from typing_extensions import Self
 
@@ -408,15 +407,15 @@
         User is recommended to avoid such namings.
 
         This situation does not happen in a local file system.
         """
         raise NotImplementedError
 
     @abc.abstractmethod
-    def file_info(self) -> Optional[FileInfo]:
+    def file_info(self) -> FileInfo | None:
         """
         If :meth:`is_file` is ``False``, return ``None``; otherwise, return file info.
         """
         raise NotImplementedError
 
     @property
     def parent(self) -> Self:
@@ -546,31 +545,31 @@
         raise NotImplementedError
 
     def write_text(
         self,
         data: str,
         *,
         overwrite: bool = False,
-        encoding: Optional[str] = None,
-        errors: Optional[str] = None,
+        encoding: str | None = None,
+        errors: str | None = None,
     ) -> None:
         """Write text ``data`` to the current file.
 
         Parent "directories" are created as needed, if applicable.
 
         If ``overwrite`` is ``False`` and the current file exists, ``FileExistsError`` is raised.
 
         ``encoding`` and ``errors`` are passed to `encode() <https://docs.python.org/3/library/stdtypes.html#str.encode>`_.
         Usually you should leave them at the default values.
         """
         z = data.encode(encoding=encoding or "utf-8", errors=errors or "strict")
         self.write_bytes(z, overwrite=overwrite)
 
     def read_text(
-        self, *, encoding: Optional[str] = None, errors: Optional[str] = None
+        self, *, encoding: str | None = None, errors: str | None = None
     ) -> str:
         """
         Return the decoded contents of the pointed-to file as a string.
 
         If ``self`` is not a file or does not exist,
         ``FileNotFoundError`` is raised.
```

### Comparing `upathlib-0.7.9/src/upathlib/azure.py` & `upathlib-0.8.0b1/src/upathlib/azure.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.9/src/upathlib/gcs.py` & `upathlib-0.8.0b1/src/upathlib/gcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,31 +7,25 @@
 import contextlib
 import logging
 import os
 import time
 from collections.abc import Iterator
 from datetime import datetime, timezone
 from io import BufferedReader, BytesIO, UnsupportedOperation
-from typing import Optional
 
 import google.auth
 from google import resumable_media
 from google.api_core import exceptions
 from google.cloud import storage
 
 # 60 seconds; this is the "connection timeout" to server.
 # From my reading, it's the `timeout` parameter to `google.cloud.storage.client._connection.api_request`,
 # that is, the `timeout` parameter to `google.cloud._http.JSONConnection.api_request`.
 # `google.cloud` is repo python-cloud-core.
-from google.cloud.storage.retry import (
-    DEFAULT_RETRY,
-    DEFAULT_RETRY_IF_GENERATION_SPECIFIED,
-    ConditionalRetryPolicy,
-    is_generation_specified,
-)
+from google.cloud.storage.retry import DEFAULT_RETRY
 from mpservice.concurrent.futures import get_shared_thread_pool
 from mpservice.threading import MAX_THREADS
 from typing_extensions import Self
 
 from ._blob import BlobUpath, LocalPathType, _resolve_local_path
 from ._upath import FileInfo, LockAcquireError, LockReleaseError, Upath
 
@@ -48,24 +42,14 @@
 MEGABYTES32 = 33554432
 MEGABYTES64 = 67108864
 LARGE_FILE_SIZE = MEGABYTES64
 
 # DEFAULT_RETRY has default timeout 120 seconds.
 
 
-def retry_if_generation_specified(retry_timeout=None):
-    if retry_timeout is None:
-        return DEFAULT_RETRY_IF_GENERATION_SPECIFIED
-    return ConditionalRetryPolicy(
-        DEFAULT_RETRY.with_timeout(retry_timeout),
-        is_generation_specified,
-        ["query_params"],
-    )
-
-
 def get_google_auth(
     project_id=None,
     credentials=None,
     *,
     scopes: list[str] = None,
     valid_for_seconds: int = 300,
 ):
@@ -274,15 +258,15 @@
             prefix=prefix,
             max_results=1,
             page_size=1,
             fields="items(name),nextPageToken",
         )
         return len(list(blobs)) > 0
 
-    def file_info(self, *, request_timeout=60) -> Optional[FileInfo]:
+    def file_info(self, *, request_timeout=60) -> FileInfo | None:
         """
         Return file info if the current path is a file;
         otherwise return ``None``.
 
         ``request_timeout`` is the http request timeout, not "retry" timeout.
         The default is 60 (``google.cloud.storage.constants._DEFAULT_TIMEOUT``).
         """
@@ -321,27 +305,25 @@
     def _write_from_buffer(
         self,
         file_obj,
         *,
         overwrite=False,
         content_type=None,
         size=None,
-        retry_timeout=None,
     ):
         if self._path == "/":
             raise UnsupportedOperation("can not write to root as a blob", self)
 
         try:
             self._blob().upload_from_file(
                 file_obj,
                 content_type=content_type,
                 size=size,
                 client=self._client(),
                 if_generation_match=None if overwrite else 0,
-                retry=retry_if_generation_specified(retry_timeout=retry_timeout),
             )
             # TODO: set "create_time", 'update_time" to be the same
             # as the source local file?
             # Blob objects has methods `_set_properties`, `_patch_property`,
             # `patch`.
         except exceptions.PreconditionFailed:
             raise FileExistsError(self)
@@ -624,17 +606,22 @@
         # `timeout = None` with infinite wait, the default wait
         # is a long period.
         if self._path == "/":
             raise UnsupportedOperation("can not write to root as a blob", self)
         if timeout is None:
             timeout = 120  # seconds
 
+        retry = DEFAULT_RETRY.with_timeout(timeout).with_predicate(
+            lambda exc: DEFAULT_RETRY._predicate(exc)
+            or isinstance(exc, FileExistsError)
+        )
+
         t0 = time.perf_counter()
         try:
-            self._write_bytes(b"0", retry_timeout=timeout)
+            retry(self._write_bytes)(b'0')
             self._generation = self._blob().generation
         except FileExistsError as e:
             finfo = self.file_info(request_timeout=timeout)
             now = datetime.utcnow().replace(tzinfo=timezone.utc)
             file_age = (now - finfo.time_created).total_seconds()
             if file_age - timeout > self._LOCK_EXPIRE_IN_SECONDS:
                 # If the file is old,
@@ -682,16 +669,14 @@
             yield
         finally:
             self._lock_count -= 1
             if self._lock_count == 0:
                 try:
                     self._blob().delete(
                         if_generation_match=self._generation,  # TODO: should we remove this condition?
-                        timeout=150,
-                        retry=retry_if_generation_specified(retry_timeout=300),
                     )
 
                 except Exception as e:
                     raise LockReleaseError(f"failed to delete lock file {self}") from e
 
     def open(self, mode="r", **kwargs):
         """
```

### Comparing `upathlib-0.7.9/src/upathlib/serializer.py` & `upathlib-0.8.0b1/src/upathlib/serializer.py`

 * *Files identical despite different names*

### Comparing `upathlib-0.7.9/PKG-INFO` & `upathlib-0.8.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upathlib
-Version: 0.7.9
+Version: 0.8.0b1
 Summary: The package *upathlib*
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

