# Comparing `tmp/ewoksdata-0.2.4.tar.gz` & `tmp/ewoksdata-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksdata-0.2.4.tar", last modified: Tue Apr 18 16:13:46 2023, max compression
+gzip compressed data, was "dist/ewoksdata-0.2.5.tar", last modified: Tue Apr 25 11:46:26 2023, max compression
```

## Comparing `ewoksdata-0.2.4.tar` & `ewoksdata-0.2.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-18 16:12:04.000000 ewoksdata-0.2.4/src/ewoksdata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 16:13:40.000000 ewoksdata-0.2.4/src/ewoksdata/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7007 2023-04-18 15:13:18.000000 ewoksdata-0.2.4/src/ewoksdata/data/bliss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata/data/hdf5/
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/data/hdf5/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6085 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/data/hdf5/config.py
--rw-rw-rw-   0 root         (0) root         (0)     4017 2023-04-18 16:12:04.000000 ewoksdata-0.2.4/src/ewoksdata/data/hdf5/dataset_writer.py
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/data/hdf5/types.py
--rw-rw-rw-   0 root         (0) root         (0)     3057 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/data/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/data/url.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/data/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 16:13:40.000000 ewoksdata-0.2.4/src/ewoksdata/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3468 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/tests/data/bliss_scans.py
--rw-rw-rw-   0 root         (0) root         (0)      906 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/tests/test_data_bliss.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/tests/test_data_hdf5.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/tests/test_data_nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-04-18 16:12:04.000000 ewoksdata-0.2.4/src/ewoksdata/tests/test_dataset_writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      850 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      207 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-25 11:44:45.000000 ewoksdata-0.2.5/src/ewoksdata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:46:20.000000 ewoksdata-0.2.5/src/ewoksdata/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8187 2023-04-25 07:40:11.000000 ewoksdata-0.2.5/src/ewoksdata/data/bliss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata/data/hdf5/
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/data/hdf5/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6086 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/data/hdf5/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     4017 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/data/hdf5/dataset_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/data/hdf5/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     3076 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/data/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/data/url.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/data/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 11:46:20.000000 ewoksdata-0.2.5/src/ewoksdata/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/tests/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3468 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/tests/data/bliss_scans.py
+-rw-rw-rw-   0 root         (0) root         (0)      906 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/tests/test_data_bliss.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/tests/test_data_hdf5.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/tests/test_data_nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2023-04-25 06:43:39.000000 ewoksdata-0.2.5/src/ewoksdata/tests/test_dataset_writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      850 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      207 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-25 11:46:26.000000 ewoksdata-0.2.5/src/ewoksdata.egg-info/top_level.txt
```

### Comparing `ewoksdata-0.2.4/LICENSE.md` & `ewoksdata-0.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.4/PKG-INFO` & `ewoksdata-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksdata
-Version: 0.2.4
+Version: 0.2.5
 Summary: Ewoks tasks for data access
 Home-page: https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Project-URL: Documentation, https://ewoksdata.readthedocs.io
```

### Comparing `ewoksdata-0.2.4/setup.cfg` & `ewoksdata-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.4/src/ewoksdata/data/bliss.py` & `ewoksdata-0.2.5/src/ewoksdata/data/bliss.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from numbers import Integral, Number
 from typing import Iterator, List, Optional, Tuple, Sequence, Union
 
 import numpy
 import h5py
 import hdf5plugin  # noqa F401
 from numpy.typing import ArrayLike
@@ -9,22 +10,26 @@
 from silx.utils import retry as retrymod
 from silx.io.utils import get_data as silx_get_data
 from blissdata.h5api import dynamic_hdf5
 
 try:
     import gevent.queue  # noqa F401 bliss MR 5369
     from blissdata.data.node import get_node
+    from blissdata.data.events.lima import ImageNotSaved
 except ImportError:
     get_node = None
 
 from . import hdf5
 from . import nexus
 from . import url
 
 
+logger = logging.getLogger(__name__)
+
+
 def get_data(
     data: Union[str, ArrayLike, Number], **options
 ) -> Union[numpy.ndarray, Number]:
     if isinstance(data, str):
         filename, h5path, idx = url.h5dataset_url_parse(data)
         if filename.endswith(".h5") or filename.endswith(".nx"):
             return get_hdf5_data(filename, h5path, idx=idx, **options)
@@ -145,54 +150,81 @@
     return image.data
 
 
 def iter_bliss_scan_data_from_memory(
     db_name: str,
     lima_names: List[str],
     counter_names: List[str],
-    retry_timeout: Optional[Number],
-    retry_period: Optional[Number],
+    retry_timeout: Optional[Number] = None,
+    retry_period: Optional[Number] = None,
 ):
-    node = _get_node(
+    scan_node = _get_node(
         db_name, "scan", retry_timeout=retry_timeout, retry_period=retry_period
     )
     indices = {name: 0 for name in lima_names + counter_names}
     buffers = {name: list() for name in lima_names + counter_names}
-    for event_type, node, event_data in node.walk_events():
-        if event_type == event_type.END_SCAN:
-            break
+    lima_acq_nb = dict()
+    for event_type, node, event_data in scan_node.walk_events():
         if node.type == "lima":
             name = node.db_name.split(":")[-2]
             if name not in lima_names:
                 continue
-            dataview = node.get(indices[name], -1)
-            data = list(dataview)
+            dataview = _get_lima_dataview(
+                node,
+                indices[name],
+                retry_timeout=retry_timeout,
+                retry_period=retry_period,
+            )
+            current_lima_acq_nb = dataview.status_event.status["lima_acq_nb"]
+            first_lima_acq_nb = lima_acq_nb.setdefault(name, current_lima_acq_nb)
+            if first_lima_acq_nb != current_lima_acq_nb:
+                logger.warning("lima is already acquiring the next scan")
+                continue
+            try:
+                data = list(dataview)
+            except ImageNotSaved:
+                logger.warning(
+                    "cannot read lima data from file because it is not saving"
+                )
+                continue
             indices[name] += len(data)
             buffers[name].extend(data)
-        if node.type == "channel":
+        elif node.type == "channel":
             name = node.db_name.split(":")[-1]
             if name not in counter_names:
                 continue
             if event_data:
                 data = event_data.data
             else:
                 data = node.get_as_array(indices[name], -1)
             indices[name] += len(data)
             buffers[name].extend(data)
-        n = min(len(v) for v in buffers.values())
-        if n == 0:
-            continue
-        for i in range(n):
-            yield {name: values[i] for name, values in buffers.items()}
-        buffers = {name: values[n:] for name, values in buffers.items()}
+        nyield = min(len(v) for v in buffers.values())
+        if nyield:
+            for i in range(nyield):
+                yield {name: values[i] for name, values in buffers.items()}
+            buffers = {name: values[nyield:] for name, values in buffers.items()}
+        if event_type == event_type.END_SCAN:
+            break
 
 
 @retrymod.retry()
 def _get_node(db_name: str, node_type: str):
     if get_node is None:
         raise ModuleNotFoundError("No module named 'blissdata'")
     node = get_node(db_name)
     if node is None:
         raise retrymod.RetryError(f"Redis node {db_name} does not exist")
     if node.type != node_type:
         raise RuntimeError(f"Not a Redis {node_type} node")
     return node
+
+
+@retrymod.retry()
+def _get_lima_dataview(node, start_index: int):
+    dataview = node.get(start_index, -1)
+    try:
+        if dataview.status_event.proxy is None:
+            raise retrymod.RetryError("Lima proxy not known (yet)")
+    except Exception:
+        raise retrymod.RetryError("Lima proxy not known (yet)")
+    return dataview
```

### Comparing `ewoksdata-0.2.4/src/ewoksdata/data/hdf5/__init__.py` & `ewoksdata-0.2.5/src/ewoksdata/data/hdf5/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.4/src/ewoksdata/data/hdf5/config.py` & `ewoksdata-0.2.5/src/ewoksdata/data/hdf5/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 ) -> Optional[ShapeType]:
     """Try to guess the optimal chunk shape with these constraints:
     * Split any dimension for partial access
     * Below the maximal chunk size (1 MB by default, uncompressed)
 
     The inner-most dimensions are split in `chunk_split` parts
     until chunk_nbytes is reached. The chunk size in the outer
-    dimensions will be 1, unless the data size is to small.
+    dimensions will be 1, unless the data size is too small.
     """
     if chunk_nbytes is None:
         chunk_nbytes = DEFAULT_CHUNK_NBYTES
     if chunk_split is None:
         chunk_split = DEFAULT_CHUNK_SPLIT
     itemsize = dtype_nbytes(dtype)
     size = shape_to_size(data_shape)
```

### Comparing `ewoksdata-0.2.4/src/ewoksdata/data/hdf5/dataset_writer.py` & `ewoksdata-0.2.5/src/ewoksdata/data/hdf5/dataset_writer.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.4/src/ewoksdata/data/nexus.py` & `ewoksdata-0.2.5/src/ewoksdata/data/nexus.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,22 +53,22 @@
     retry_period=None,
     default_levels: Optional[Tuple[str]] = None,
     **open_options,
 ) -> Iterator[Tuple[h5py.Group, bool]]:
     """
     :yields: (h5group, already_existed)
     """
-    if isinstance(url, DataUrl):
+    if not isinstance(url, DataUrl):
         url = DataUrl(url)
-    url = DataUrl(url)
     filename = url.file_path()
     itemname = url.data_path()
     if not itemname:
         itemname = "/"
-    os.makedirs(os.path.dirname(filename), exist_ok=True)
+    if os.path.dirname(filename):
+        os.makedirs(os.path.dirname(filename), exist_ok=True)
     open_options.setdefault("mode", "a")
     with h5py_utils.open_item(
         filename,
         "/",
         retry_timeout=retry_timeout,
         retry_period=retry_period,
         **open_options,
```

### Comparing `ewoksdata-0.2.4/src/ewoksdata/data/utils.py` & `ewoksdata-0.2.5/src/ewoksdata/data/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.4/src/ewoksdata/tests/data/bliss_scans.py` & `ewoksdata-0.2.5/src/ewoksdata/tests/data/bliss_scans.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.4/src/ewoksdata/tests/test_data_bliss.py` & `ewoksdata-0.2.5/src/ewoksdata/tests/test_data_bliss.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.4/src/ewoksdata/tests/test_data_nexus.py` & `ewoksdata-0.2.5/src/ewoksdata/tests/test_data_nexus.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.4/src/ewoksdata/tests/test_dataset_writer.py` & `ewoksdata-0.2.5/src/ewoksdata/tests/test_dataset_writer.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.4/src/ewoksdata.egg-info/PKG-INFO` & `ewoksdata-0.2.5/src/ewoksdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksdata
-Version: 0.2.4
+Version: 0.2.5
 Summary: Ewoks tasks for data access
 Home-page: https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Project-URL: Documentation, https://ewoksdata.readthedocs.io
```

### Comparing `ewoksdata-0.2.4/src/ewoksdata.egg-info/SOURCES.txt` & `ewoksdata-0.2.5/src/ewoksdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

