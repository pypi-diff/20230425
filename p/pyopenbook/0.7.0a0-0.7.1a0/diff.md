# Comparing `tmp/pyopenbook-0.7.0a0.tar.gz` & `tmp/pyopenbook-0.7.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopenbook-0.7.0a0.tar", last modified: Tue Apr 25 01:09:28 2023, max compression
+gzip compressed data, was "pyopenbook-0.7.1a0.tar", last modified: Tue Apr 25 03:56:06 2023, max compression
```

## Comparing `pyopenbook-0.7.0a0.tar` & `pyopenbook-0.7.1a0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 01:09:28.513039 pyopenbook-0.7.0a0/
--rw-r--r--   0 waterquarks   (501) staff       (20)      541 2023-04-25 01:09:28.512889 pyopenbook-0.7.0a0/PKG-INFO
--rw-r--r--   0 waterquarks   (501) staff       (20)     3360 2023-04-25 01:09:01.000000 pyopenbook-0.7.0a0/README.md
-drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 01:09:28.507141 pyopenbook-0.7.0a0/pyopenbook.egg-info/
--rw-r--r--   0 waterquarks   (501) staff       (20)      541 2023-04-25 01:09:28.000000 pyopenbook-0.7.0a0/pyopenbook.egg-info/PKG-INFO
--rw-r--r--   0 waterquarks   (501) staff       (20)      948 2023-04-25 01:09:28.000000 pyopenbook-0.7.0a0/pyopenbook.egg-info/SOURCES.txt
--rw-r--r--   0 waterquarks   (501) staff       (20)        1 2023-04-25 01:09:28.000000 pyopenbook-0.7.0a0/pyopenbook.egg-info/dependency_links.txt
--rw-r--r--   0 waterquarks   (501) staff       (20)        1 2023-04-25 01:09:28.000000 pyopenbook-0.7.0a0/pyopenbook.egg-info/not-zip-safe
--rw-r--r--   0 waterquarks   (501) staff       (20)       79 2023-04-25 01:09:28.000000 pyopenbook-0.7.0a0/pyopenbook.egg-info/requires.txt
--rw-r--r--   0 waterquarks   (501) staff       (20)        8 2023-04-25 01:09:28.000000 pyopenbook-0.7.0a0/pyopenbook.egg-info/top_level.txt
-drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 01:09:28.509455 pyopenbook-0.7.0a0/pyserum/
--rw-r--r--   0 waterquarks   (501) staff       (20)      121 2022-12-21 03:49:05.000000 pyopenbook-0.7.0a0/pyserum/__init__.py
-drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 01:09:28.510765 pyopenbook-0.7.0a0/pyserum/_layouts/
--rw-r--r--   0 waterquarks   (501) staff       (20)        0 2022-12-21 03:49:05.000000 pyopenbook-0.7.0a0/pyserum/_layouts/__init__.py
--rw-r--r--   0 waterquarks   (501) staff       (20)      486 2022-12-21 03:49:05.000000 pyopenbook-0.7.0a0/pyserum/_layouts/account_flags.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     2727 2022-12-21 03:49:05.000000 pyopenbook-0.7.0a0/pyserum/_layouts/instructions.py
--rw-r--r--   0 waterquarks   (501) staff       (20)      934 2022-12-21 03:49:05.000000 pyopenbook-0.7.0a0/pyserum/_layouts/market.py
--rw-r--r--   0 waterquarks   (501) staff       (20)      601 2022-12-21 03:49:05.000000 pyopenbook-0.7.0a0/pyserum/_layouts/open_orders.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     1571 2023-04-24 14:44:58.000000 pyopenbook-0.7.0a0/pyserum/_layouts/queue.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     1794 2023-04-24 14:44:58.000000 pyopenbook-0.7.0a0/pyserum/_layouts/slab.py
--rw-r--r--   0 waterquarks   (501) staff       (20)      670 2023-04-24 14:44:58.000000 pyopenbook-0.7.0a0/pyserum/async_connection.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     1206 2023-04-24 14:44:58.000000 pyopenbook-0.7.0a0/pyserum/async_open_orders_account.py
--rw-r--r--   0 waterquarks   (501) staff       (20)      630 2023-04-25 01:09:01.000000 pyopenbook-0.7.0a0/pyserum/async_utils.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     1105 2023-04-24 14:44:58.000000 pyopenbook-0.7.0a0/pyserum/connection.py
--rw-r--r--   0 waterquarks   (501) staff       (20)      406 2022-12-21 03:49:05.000000 pyopenbook-0.7.0a0/pyserum/enums.py
--rw-r--r--   0 waterquarks   (501) staff       (20)    27650 2023-04-24 14:44:58.000000 pyopenbook-0.7.0a0/pyserum/instructions.py
-drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 01:09:28.512257 pyopenbook-0.7.0a0/pyserum/market/
--rw-r--r--   0 waterquarks   (501) staff       (20)      194 2022-12-21 03:49:05.000000 pyopenbook-0.7.0a0/pyserum/market/__init__.py
-drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 01:09:28.512702 pyopenbook-0.7.0a0/pyserum/market/_internal/
--rw-r--r--   0 waterquarks   (501) staff       (20)        0 2022-12-21 03:49:05.000000 pyopenbook-0.7.0a0/pyserum/market/_internal/__init__.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     4309 2023-04-24 14:44:58.000000 pyopenbook-0.7.0a0/pyserum/market/_internal/queue.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     5043 2023-04-24 14:44:58.000000 pyopenbook-0.7.0a0/pyserum/market/_internal/slab.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     7780 2023-04-25 01:08:59.000000 pyopenbook-0.7.0a0/pyserum/market/async_market.py
--rw-r--r--   0 waterquarks   (501) staff       (20)    20549 2023-04-25 01:08:59.000000 pyopenbook-0.7.0a0/pyserum/market/core.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     7430 2023-04-25 01:09:01.000000 pyopenbook-0.7.0a0/pyserum/market/market.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     3389 2023-04-25 01:09:01.000000 pyopenbook-0.7.0a0/pyserum/market/orderbook.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     6639 2023-04-25 01:08:59.000000 pyopenbook-0.7.0a0/pyserum/market/state.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     2592 2023-04-25 00:58:11.000000 pyopenbook-0.7.0a0/pyserum/market/types.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     5668 2023-04-24 14:44:58.000000 pyopenbook-0.7.0a0/pyserum/open_orders_account.py
--rw-r--r--   0 waterquarks   (501) staff       (20)        0 2022-12-21 03:49:06.000000 pyopenbook-0.7.0a0/pyserum/py.typed
--rw-r--r--   0 waterquarks   (501) staff       (20)      938 2023-04-25 01:09:01.000000 pyopenbook-0.7.0a0/pyserum/utils.py
--rw-r--r--   0 waterquarks   (501) staff       (20)       38 2023-04-25 01:09:28.513076 pyopenbook-0.7.0a0/setup.cfg
--rw-r--r--   0 waterquarks   (501) staff       (20)      961 2023-04-25 01:09:01.000000 pyopenbook-0.7.0a0/setup.py
+drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 03:56:06.121765 pyopenbook-0.7.1a0/
+-rw-r--r--   0 waterquarks   (501) staff       (20)     1072 2023-04-25 03:49:01.000000 pyopenbook-0.7.1a0/LICENSE
+-rw-r--r--   0 waterquarks   (501) staff       (20)      563 2023-04-25 03:56:06.121606 pyopenbook-0.7.1a0/PKG-INFO
+-rw-r--r--   0 waterquarks   (501) staff       (20)     3329 2023-04-25 03:49:01.000000 pyopenbook-0.7.1a0/README.md
+drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 03:56:06.116221 pyopenbook-0.7.1a0/pyopenbook.egg-info/
+-rw-r--r--   0 waterquarks   (501) staff       (20)      563 2023-04-25 03:56:06.000000 pyopenbook-0.7.1a0/pyopenbook.egg-info/PKG-INFO
+-rw-r--r--   0 waterquarks   (501) staff       (20)      956 2023-04-25 03:56:06.000000 pyopenbook-0.7.1a0/pyopenbook.egg-info/SOURCES.txt
+-rw-r--r--   0 waterquarks   (501) staff       (20)        1 2023-04-25 03:56:06.000000 pyopenbook-0.7.1a0/pyopenbook.egg-info/dependency_links.txt
+-rw-r--r--   0 waterquarks   (501) staff       (20)        1 2023-04-25 03:56:06.000000 pyopenbook-0.7.1a0/pyopenbook.egg-info/not-zip-safe
+-rw-r--r--   0 waterquarks   (501) staff       (20)       79 2023-04-25 03:56:06.000000 pyopenbook-0.7.1a0/pyopenbook.egg-info/requires.txt
+-rw-r--r--   0 waterquarks   (501) staff       (20)        8 2023-04-25 03:56:06.000000 pyopenbook-0.7.1a0/pyopenbook.egg-info/top_level.txt
+drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 03:56:06.118356 pyopenbook-0.7.1a0/pyserum/
+-rw-r--r--   0 waterquarks   (501) staff       (20)      121 2022-12-21 03:49:05.000000 pyopenbook-0.7.1a0/pyserum/__init__.py
+drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 03:56:06.119464 pyopenbook-0.7.1a0/pyserum/_layouts/
+-rw-r--r--   0 waterquarks   (501) staff       (20)        0 2022-12-21 03:49:05.000000 pyopenbook-0.7.1a0/pyserum/_layouts/__init__.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)      486 2022-12-21 03:49:05.000000 pyopenbook-0.7.1a0/pyserum/_layouts/account_flags.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     2727 2022-12-21 03:49:05.000000 pyopenbook-0.7.1a0/pyserum/_layouts/instructions.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)      934 2022-12-21 03:49:05.000000 pyopenbook-0.7.1a0/pyserum/_layouts/market.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)      601 2022-12-21 03:49:05.000000 pyopenbook-0.7.1a0/pyserum/_layouts/open_orders.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     1526 2023-04-25 03:49:01.000000 pyopenbook-0.7.1a0/pyserum/_layouts/queue.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     1758 2023-04-25 03:49:01.000000 pyopenbook-0.7.1a0/pyserum/_layouts/slab.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)      640 2023-04-25 03:49:01.000000 pyopenbook-0.7.1a0/pyserum/async_connection.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     1211 2023-04-25 03:49:01.000000 pyopenbook-0.7.1a0/pyserum/async_open_orders_account.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)      641 2023-04-25 03:49:01.000000 pyopenbook-0.7.1a0/pyserum/async_utils.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     1063 2023-04-25 03:49:01.000000 pyopenbook-0.7.1a0/pyserum/connection.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)      406 2022-12-21 03:49:05.000000 pyopenbook-0.7.1a0/pyserum/enums.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)    27738 2023-04-25 03:49:01.000000 pyopenbook-0.7.1a0/pyserum/instructions.py
+drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 03:56:06.120955 pyopenbook-0.7.1a0/pyserum/market/
+-rw-r--r--   0 waterquarks   (501) staff       (20)      194 2022-12-21 03:49:05.000000 pyopenbook-0.7.1a0/pyserum/market/__init__.py
+drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 03:56:06.121405 pyopenbook-0.7.1a0/pyserum/market/_internal/
+-rw-r--r--   0 waterquarks   (501) staff       (20)        0 2022-12-21 03:49:05.000000 pyopenbook-0.7.1a0/pyserum/market/_internal/__init__.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     4163 2023-04-25 03:49:01.000000 pyopenbook-0.7.1a0/pyserum/market/_internal/queue.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     5044 2023-04-25 03:49:01.000000 pyopenbook-0.7.1a0/pyserum/market/_internal/slab.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     7672 2023-04-25 03:49:01.000000 pyopenbook-0.7.1a0/pyserum/market/async_market.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)    19934 2023-04-25 03:49:01.000000 pyopenbook-0.7.1a0/pyserum/market/core.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     7342 2023-04-25 03:49:01.000000 pyopenbook-0.7.1a0/pyserum/market/market.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     3345 2023-04-25 03:49:01.000000 pyopenbook-0.7.1a0/pyserum/market/orderbook.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     6290 2023-04-25 03:49:01.000000 pyopenbook-0.7.1a0/pyserum/market/state.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     2615 2023-04-25 03:51:31.000000 pyopenbook-0.7.1a0/pyserum/market/types.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     5618 2023-04-25 03:49:01.000000 pyopenbook-0.7.1a0/pyserum/open_orders_account.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)        0 2022-12-21 03:49:06.000000 pyopenbook-0.7.1a0/pyserum/py.typed
+-rw-r--r--   0 waterquarks   (501) staff       (20)      949 2023-04-25 03:49:01.000000 pyopenbook-0.7.1a0/pyserum/utils.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)       38 2023-04-25 03:56:06.121809 pyopenbook-0.7.1a0/setup.cfg
+-rw-r--r--   0 waterquarks   (501) staff       (20)      961 2023-04-25 03:56:02.000000 pyopenbook-0.7.1a0/setup.py
```

### Comparing `pyopenbook-0.7.0a0/PKG-INFO` & `pyopenbook-0.7.1a0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: pyopenbook
-Version: 0.7.0a0
+Version: 0.7.1a0
 Summary: Python client library for interacting with the Project Serum DEX.
 Home-page: https://github.com/blockworks-foundation/pyopenbook
 Author: serum-community
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7, <4
+License-File: LICENSE
```

### Comparing `pyopenbook-0.7.0a0/README.md` & `pyopenbook-0.7.1a0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+[![Actions
+Status](https://github.com/serum-community/pyserum/workflows/CI/badge.svg)](https://github.com/serum-community/pyserum/actions?query=workflow%3ACI)
+[![Codecov](https://codecov.io/gh/serum-community/pyserum/branch/alpha/graph/badge.svg)](https://codecov.io/gh/serum-community/pyserum/branches/alpha)
+
 # PySerum
 
 Python client library for interacting with the [Project Serum](https://projectserum.com/) DEX.
 
 ## Install
 
 ```sh
@@ -139,20 +143,7 @@
 ```bash
 ./scripts/bootstrap_dex.sh
 ```
 
 This will start a docker container with `solana` image and deploy a serum DEX which you can use for testing.
 
 The market address, program id, and wallet addresses can be found in the new `crank.log` file after the script runs successfully.
-
-
-### Release
-
-To release a new version remember to update the version in the `setup.py` file and then run on the latest commit:
-
-```sh
-git tag -a v0.7.0a0 -m "[MESSAGE]"
-git push origin --tags
-python setup.py sdist bdist_wheel
-```
-
-Go on github and create the new release with the latest tag and upload the artifacts from the `dist` folder.
```

### Comparing `pyopenbook-0.7.0a0/pyopenbook.egg-info/PKG-INFO` & `pyopenbook-0.7.1a0/pyopenbook.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: pyopenbook
-Version: 0.7.0a0
+Version: 0.7.1a0
 Summary: Python client library for interacting with the Project Serum DEX.
 Home-page: https://github.com/blockworks-foundation/pyopenbook
 Author: serum-community
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7, <4
+License-File: LICENSE
```

### Comparing `pyopenbook-0.7.0a0/pyopenbook.egg-info/SOURCES.txt` & `pyopenbook-0.7.1a0/pyopenbook.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 pyopenbook.egg-info/PKG-INFO
 pyopenbook.egg-info/SOURCES.txt
 pyopenbook.egg-info/dependency_links.txt
 pyopenbook.egg-info/not-zip-safe
 pyopenbook.egg-info/requires.txt
```

### Comparing `pyopenbook-0.7.0a0/pyserum/_layouts/instructions.py` & `pyopenbook-0.7.1a0/pyserum/_layouts/instructions.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.0a0/pyserum/_layouts/market.py` & `pyopenbook-0.7.1a0/pyserum/_layouts/market.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.0a0/pyserum/_layouts/open_orders.py` & `pyopenbook-0.7.1a0/pyserum/_layouts/open_orders.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.0a0/pyserum/_layouts/queue.py` & `pyopenbook-0.7.1a0/pyserum/_layouts/queue.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,8 @@
-from construct import (
-    BitsInteger,
-    BitsSwapped,
-    BitStruct,
-    Bytes,
-    Const,
-    Flag,
-    Int8ul,
-    Int32ul,
-    Int64ul,
-    Padding,
-)
+from construct import BitsInteger, BitsSwapped, BitStruct, Bytes, Const, Flag, Int8ul, Int32ul, Int64ul, Padding
 from construct import Struct as cStruct
 
 from .account_flags import ACCOUNT_FLAGS_LAYOUT
 
 QUEUE_HEADER_LAYOUT = cStruct(
     Padding(5),
     "account_flags" / ACCOUNT_FLAGS_LAYOUT,
```

### Comparing `pyopenbook-0.7.0a0/pyserum/_layouts/slab.py` & `pyopenbook-0.7.1a0/pyserum/_layouts/slab.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,17 +29,15 @@
     LEAF_NODE = 2
     FREE_NODE = 3
     LAST_FREE_NODE = 4
 
 
 # Different node types, we pad it all to size of 68 bytes.
 UNINTIALIZED = cStruct(Padding(68))
-INNER_NODE = cStruct(
-    "prefix_len" / Int32ul, "key" / KEY, "children" / Int32ul[2], Padding(40)
-)
+INNER_NODE = cStruct("prefix_len" / Int32ul, "key" / KEY, "children" / Int32ul[2], Padding(40))
 LEAF_NODE = cStruct(
     "owner_slot" / Int8ul,
     "fee_tier" / Int8ul,
     Padding(2),
     "key" / KEY,
     "owner" / Bytes(32),
     "quantity" / Int64ul,
@@ -59,18 +57,10 @@
             NodeType.LEAF_NODE: LEAF_NODE,
             NodeType.FREE_NODE: FREE_NODE,
             NodeType.LAST_FREE_NODE: LAST_FREE_NODE,
         },
     ),
 )
 
-SLAB_LAYOUT = cStruct(
-    "header" / SLAB_HEADER_LAYOUT,
-    "nodes" / SLAB_NODE_LAYOUT[lambda this: this.header.bump_index],
-)
+SLAB_LAYOUT = cStruct("header" / SLAB_HEADER_LAYOUT, "nodes" / SLAB_NODE_LAYOUT[lambda this: this.header.bump_index])
 
-ORDER_BOOK_LAYOUT = cStruct(
-    Padding(5),
-    "account_flags" / ACCOUNT_FLAGS_LAYOUT,
-    "slab_layout" / SLAB_LAYOUT,
-    Padding(7),
-)
+ORDER_BOOK_LAYOUT = cStruct(Padding(5), "account_flags" / ACCOUNT_FLAGS_LAYOUT, "slab_layout" / SLAB_LAYOUT, Padding(7))
```

### Comparing `pyopenbook-0.7.0a0/pyserum/async_connection.py` & `pyopenbook-0.7.1a0/pyserum/async_connection.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,13 @@
 from typing import List
 
 import httpx
-from solana.rpc.async_api import (
-    AsyncClient as async_conn,
-)  # pylint: disable=unused-import # noqa:F401
+from solana.rpc.async_api import AsyncClient as async_conn  # pylint: disable=unused-import # noqa:F401
 
-from .connection import (
-    LIVE_MARKETS_URL,
-    TOKEN_MINTS_URL,
-    parse_live_markets,
-    parse_token_mints,
-)
+from .connection import LIVE_MARKETS_URL, TOKEN_MINTS_URL, parse_live_markets, parse_token_mints
 from .market.types import MarketInfo, TokenInfo
 
 
 async def get_live_markets(httpx_client: httpx.AsyncClient) -> List[MarketInfo]:
     resp = await httpx_client.get(LIVE_MARKETS_URL)
     return parse_live_markets(resp.json())
```

### Comparing `pyopenbook-0.7.0a0/pyserum/connection.py` & `pyopenbook-0.7.1a0/pyserum/connection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 from typing import Any, Dict, List
 
 import requests
-from solders.pubkey import Pubkey
+from solana.publickey import PublicKey
 from solana.rpc.api import Client as conn  # pylint: disable=unused-import # noqa:F401
 
 from .market.types import MarketInfo, TokenInfo
 
 LIVE_MARKETS_URL = "https://raw.githubusercontent.com/project-serum/serum-ts/master/packages/serum/src/markets.json"
 TOKEN_MINTS_URL = "https://raw.githubusercontent.com/project-serum/serum-ts/master/packages/serum/src/token-mints.json"
 
 
 def parse_live_markets(data: List[Dict[str, Any]]) -> List[MarketInfo]:
     return [
-        MarketInfo(name=m["name"], address=m["address"], program_id=m["programId"])
-        for m in data
-        if not m["deprecated"]
+        MarketInfo(name=m["name"], address=m["address"], program_id=m["programId"]) for m in data if not m["deprecated"]
     ]
 
 
 def parse_token_mints(data: List[Dict[str, str]]) -> List[TokenInfo]:
-    return [
-        TokenInfo(name=t["name"], address=Pubkey.from_string(t["address"]))
-        for t in data
-    ]
+    return [TokenInfo(name=t["name"], address=PublicKey(t["address"])) for t in data]
 
 
 def get_live_markets() -> List[MarketInfo]:
     return parse_live_markets(requests.get(LIVE_MARKETS_URL).json())
 
 
 def get_token_mints() -> List[TokenInfo]:
```

### Comparing `pyopenbook-0.7.0a0/pyserum/instructions.py` & `pyopenbook-0.7.1a0/pyserum/instructions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,212 +1,209 @@
 """Serum Dex Instructions."""
 from typing import Dict, List, NamedTuple, Optional
 
 from construct import Container
-from solders.sysvar import RENT
-from solana.transaction import AccountMeta
-from solders.instruction import Instruction
+from solana.publickey import PublicKey
+from solana.sysvar import SYSVAR_RENT_PUBKEY
+from solana.transaction import AccountMeta, TransactionInstruction
 from solana.utils.validate import validate_instruction_keys, validate_instruction_type
-from solders.pubkey import Pubkey
 from spl.token.constants import TOKEN_PROGRAM_ID
 
 from ._layouts.instructions import INSTRUCTIONS_LAYOUT, InstructionType
 from .enums import OrderType, SelfTradeBehavior, Side
 
 # V3
-DEFAULT_DEX_PROGRAM_ID = Pubkey.from_string(
-    "9xQeWvG816bUx9EPjHmaT23yvVM2ZWbrrpZb9PusVFin"
-)
+DEFAULT_DEX_PROGRAM_ID = PublicKey("9xQeWvG816bUx9EPjHmaT23yvVM2ZWbrrpZb9PusVFin")
 
 
 class InitializeMarketParams(NamedTuple):
     """Initalize market params."""
 
-    market: Pubkey
+    market: PublicKey
     """"""
-    request_queue: Pubkey
+    request_queue: PublicKey
     """"""
-    event_queue: Pubkey
+    event_queue: PublicKey
     """"""
-    bids: Pubkey
+    bids: PublicKey
     """"""
-    asks: Pubkey
+    asks: PublicKey
     """"""
-    base_vault: Pubkey
+    base_vault: PublicKey
     """"""
-    quote_vault: Pubkey
+    quote_vault: PublicKey
     """"""
-    base_mint: Pubkey
+    base_mint: PublicKey
     """"""
-    quote_mint: Pubkey
+    quote_mint: PublicKey
     """"""
     base_lot_size: int
     """"""
     quote_lot_size: int
     """"""
     fee_rate_bps: int
     """"""
     vault_signer_nonce: int
     """"""
     quote_dust_threshold: int
     """"""
-    program_id: Pubkey = DEFAULT_DEX_PROGRAM_ID
+    program_id: PublicKey = DEFAULT_DEX_PROGRAM_ID
 
 
 class NewOrderParams(NamedTuple):
     """New order params."""
 
-    market: Pubkey
+    market: PublicKey
     """"""
-    open_orders: Pubkey
+    open_orders: PublicKey
     """"""
-    payer: Pubkey
+    payer: PublicKey
     """"""
-    owner: Pubkey
+    owner: PublicKey
     """"""
-    request_queue: Pubkey
+    request_queue: PublicKey
     """"""
-    base_vault: Pubkey
+    base_vault: PublicKey
     """"""
-    quote_vault: Pubkey
+    quote_vault: PublicKey
     """"""
     side: Side
     """"""
     limit_price: int
     """"""
     max_quantity: int
     """"""
     order_type: OrderType
     """"""
     client_id: int = 0
     """"""
-    program_id: Pubkey = DEFAULT_DEX_PROGRAM_ID
+    program_id: PublicKey = DEFAULT_DEX_PROGRAM_ID
     """"""
 
 
 class MatchOrdersParams(NamedTuple):
     """Match order params."""
 
-    market: Pubkey
+    market: PublicKey
     """"""
-    request_queue: Pubkey
+    request_queue: PublicKey
     """"""
-    event_queue: Pubkey
+    event_queue: PublicKey
     """"""
-    bids: Pubkey
+    bids: PublicKey
     """"""
-    asks: Pubkey
+    asks: PublicKey
     """"""
-    base_vault: Pubkey
+    base_vault: PublicKey
     """"""
-    quote_vault: Pubkey
+    quote_vault: PublicKey
     """"""
     limit: int
     """"""
-    program_id: Pubkey = DEFAULT_DEX_PROGRAM_ID
+    program_id: PublicKey = DEFAULT_DEX_PROGRAM_ID
     """"""
 
 
 class ConsumeEventsParams(NamedTuple):
     """Consume events params."""
 
-    market: Pubkey
+    market: PublicKey
     """"""
-    event_queue: Pubkey
+    event_queue: PublicKey
     """"""
-    open_orders_accounts: List[Pubkey]
+    open_orders_accounts: List[PublicKey]
     """"""
     limit: int
     """"""
-    program_id: Pubkey = DEFAULT_DEX_PROGRAM_ID
+    program_id: PublicKey = DEFAULT_DEX_PROGRAM_ID
     """"""
 
 
 class CancelOrderParams(NamedTuple):
     """Cancel order params."""
 
-    market: Pubkey
+    market: PublicKey
     """"""
-    open_orders: Pubkey
+    open_orders: PublicKey
     """"""
-    owner: Pubkey
+    owner: PublicKey
     """"""
-    request_queue: Pubkey
+    request_queue: PublicKey
     """"""
     side: Side
     """"""
     order_id: int
     """"""
     open_orders_slot: int
     """"""
-    program_id: Pubkey = DEFAULT_DEX_PROGRAM_ID
+    program_id: PublicKey = DEFAULT_DEX_PROGRAM_ID
     """"""
 
 
 class CancelOrderByClientIDParams(NamedTuple):
     """Cancel order by client ID params."""
 
-    market: Pubkey
+    market: PublicKey
     """"""
-    open_orders: Pubkey
+    open_orders: PublicKey
     """"""
-    owner: Pubkey
+    owner: PublicKey
     """"""
-    request_queue: Pubkey
+    request_queue: PublicKey
     """"""
     client_id: int
     """"""
-    program_id: Pubkey = DEFAULT_DEX_PROGRAM_ID
+    program_id: PublicKey = DEFAULT_DEX_PROGRAM_ID
     """"""
 
 
 class SettleFundsParams(NamedTuple):
     """Settle fund params."""
 
-    market: Pubkey
+    market: PublicKey
     """"""
-    open_orders: Pubkey
+    open_orders: PublicKey
     """"""
-    owner: Pubkey
+    owner: PublicKey
     """"""
-    base_vault: Pubkey
+    base_vault: PublicKey
     """"""
-    quote_vault: Pubkey
+    quote_vault: PublicKey
     """"""
-    base_wallet: Pubkey
+    base_wallet: PublicKey
     """"""
-    quote_wallet: Pubkey
+    quote_wallet: PublicKey
     """"""
-    vault_signer: Pubkey
+    vault_signer: PublicKey
     """"""
-    program_id: Pubkey = DEFAULT_DEX_PROGRAM_ID
+    program_id: PublicKey = DEFAULT_DEX_PROGRAM_ID
 
 
 class NewOrderV3Params(NamedTuple):
     """New order params."""
 
-    market: Pubkey
+    market: PublicKey
     """"""
-    open_orders: Pubkey
+    open_orders: PublicKey
     """"""
-    payer: Pubkey
+    payer: PublicKey
     """"""
-    owner: Pubkey
+    owner: PublicKey
     """"""
-    request_queue: Pubkey
+    request_queue: PublicKey
     """"""
-    event_queue: Pubkey
+    event_queue: PublicKey
     """"""
-    bids: Pubkey
+    bids: PublicKey
     """"""
-    asks: Pubkey
+    asks: PublicKey
     """"""
-    base_vault: Pubkey
+    base_vault: PublicKey
     """"""
-    quote_vault: Pubkey
+    quote_vault: PublicKey
     """"""
     side: Side
     """"""
     limit_price: int
     """"""
     max_base_quantity: int
     """"""
@@ -216,97 +213,97 @@
     """"""
     self_trade_behavior: SelfTradeBehavior
     """"""
     limit: Optional[int]
     """"""
     client_id: int = 0
     """"""
-    program_id: Pubkey = DEFAULT_DEX_PROGRAM_ID
+    program_id: PublicKey = DEFAULT_DEX_PROGRAM_ID
     """"""
-    fee_discount_pubkey: Optional[Pubkey] = None
+    fee_discount_pubkey: Optional[PublicKey] = None
 
 
 class CancelOrderV2Params(NamedTuple):
     """Cancel order params."""
 
-    market: Pubkey
+    market: PublicKey
     """"""
-    bids: Pubkey
+    bids: PublicKey
     """"""
-    asks: Pubkey
+    asks: PublicKey
     """"""
-    event_queue: Pubkey
+    event_queue: PublicKey
     """"""
-    open_orders: Pubkey
+    open_orders: PublicKey
     """"""
-    owner: Pubkey
+    owner: PublicKey
     """"""
     side: Side
     """"""
     order_id: int
     """"""
     open_orders_slot: int
     """"""
-    program_id: Pubkey = DEFAULT_DEX_PROGRAM_ID
+    program_id: PublicKey = DEFAULT_DEX_PROGRAM_ID
     """"""
 
 
 class CancelOrderByClientIDV2Params(NamedTuple):
     """Cancel order by client ID params."""
 
-    market: Pubkey
+    market: PublicKey
     """"""
-    bids: Pubkey
+    bids: PublicKey
     """"""
-    asks: Pubkey
+    asks: PublicKey
     """"""
-    event_queue: Pubkey
+    event_queue: PublicKey
     """"""
-    open_orders: Pubkey
+    open_orders: PublicKey
     """"""
-    owner: Pubkey
+    owner: PublicKey
     """"""
     client_id: int
     """"""
-    program_id: Pubkey = DEFAULT_DEX_PROGRAM_ID
+    program_id: PublicKey = DEFAULT_DEX_PROGRAM_ID
     """"""
 
 
 class CloseOpenOrdersParams(NamedTuple):
     """Cancel order by client ID params."""
 
-    open_orders: Pubkey
+    open_orders: PublicKey
     """"""
-    owner: Pubkey
+    owner: PublicKey
     """"""
-    sol_wallet: Pubkey
+    sol_wallet: PublicKey
     """"""
-    market: Pubkey
+    market: PublicKey
     """"""
-    program_id: Pubkey = DEFAULT_DEX_PROGRAM_ID
+    program_id: PublicKey = DEFAULT_DEX_PROGRAM_ID
     """"""
 
 
 class InitOpenOrdersParams(NamedTuple):
     """Cancel order by client ID params."""
 
-    open_orders: Pubkey
+    open_orders: PublicKey
     """"""
-    owner: Pubkey
+    owner: PublicKey
     """"""
-    market: Pubkey
+    market: PublicKey
     """"""
-    market_authority: Optional[Pubkey] = None
+    market_authority: Optional[PublicKey] = None
     """"""
-    program_id: Pubkey = DEFAULT_DEX_PROGRAM_ID
+    program_id: PublicKey = DEFAULT_DEX_PROGRAM_ID
     """"""
 
 
 def __parse_and_validate_instruction(
-    instruction: Instruction, instruction_type: InstructionType
+    instruction: TransactionInstruction, instruction_type: InstructionType
 ) -> Container:
     instruction_type_to_length_map: Dict[InstructionType, int] = {
         InstructionType.INITIALIZE_MARKET: 9,
         InstructionType.NEW_ORDER: 9,
         InstructionType.MATCH_ORDER: 7,
         InstructionType.CONSUME_EVENTS: 2,
         InstructionType.CANCEL_ORDER: 4,
@@ -314,222 +311,208 @@
         InstructionType.SETTLE_FUNDS: 9,
         InstructionType.NEW_ORDER_V3: 12,
         InstructionType.CANCEL_ORDER_V2: 6,
         InstructionType.CANCEL_ORDER_BY_CLIENT_ID_V2: 6,
         InstructionType.CLOSE_OPEN_ORDERS: 4,
         InstructionType.INIT_OPEN_ORDERS: 3,
     }
-    validate_instruction_keys(
-        instruction, instruction_type_to_length_map[instruction_type]
-    )
+    validate_instruction_keys(instruction, instruction_type_to_length_map[instruction_type])
     data = INSTRUCTIONS_LAYOUT.parse(instruction.data)
     validate_instruction_type(data, instruction_type)
     return data
 
 
 def decode_initialize_market(
-    instruction: Instruction,
+    instruction: TransactionInstruction,
 ) -> InitializeMarketParams:
     """Decode an instialize market instruction and retrieve the instruction params."""
-    data = __parse_and_validate_instruction(
-        instruction, InstructionType.INITIALIZE_MARKET
-    )
+    data = __parse_and_validate_instruction(instruction, InstructionType.INITIALIZE_MARKET)
     return InitializeMarketParams(
-        market=instruction.accounts[0].pubkey,
-        request_queue=instruction.accounts[1].pubkey,
-        event_queue=instruction.accounts[2].pubkey,
-        bids=instruction.accounts[3].pubkey,
-        asks=instruction.accounts[4].pubkey,
-        base_vault=instruction.accounts[5].pubkey,
-        quote_vault=instruction.accounts[6].pubkey,
-        base_mint=instruction.accounts[7].pubkey,
-        quote_mint=instruction.accounts[8].pubkey,
+        market=instruction.keys[0].pubkey,
+        request_queue=instruction.keys[1].pubkey,
+        event_queue=instruction.keys[2].pubkey,
+        bids=instruction.keys[3].pubkey,
+        asks=instruction.keys[4].pubkey,
+        base_vault=instruction.keys[5].pubkey,
+        quote_vault=instruction.keys[6].pubkey,
+        base_mint=instruction.keys[7].pubkey,
+        quote_mint=instruction.keys[8].pubkey,
         base_lot_size=data.args.base_lot_size,
         quote_lot_size=data.args.quote_lot_size,
         fee_rate_bps=data.args.fee_rate_bps,
         vault_signer_nonce=data.args.vault_signer_nonce,
         quote_dust_threshold=data.args.quote_dust_threshold,
         program_id=instruction.program_id,
     )
 
 
-def decode_new_order(instruction: Instruction) -> NewOrderParams:
+def decode_new_order(instruction: TransactionInstruction) -> NewOrderParams:
     data = __parse_and_validate_instruction(instruction, InstructionType.NEW_ORDER)
     return NewOrderParams(
-        market=instruction.accounts[0].pubkey,
-        open_orders=instruction.accounts[1].pubkey,
-        request_queue=instruction.accounts[2].pubkey,
-        payer=instruction.accounts[3].pubkey,
-        owner=instruction.accounts[4].pubkey,
-        base_vault=instruction.accounts[5].pubkey,
-        quote_vault=instruction.accounts[6].pubkey,
+        market=instruction.keys[0].pubkey,
+        open_orders=instruction.keys[1].pubkey,
+        request_queue=instruction.keys[2].pubkey,
+        payer=instruction.keys[3].pubkey,
+        owner=instruction.keys[4].pubkey,
+        base_vault=instruction.keys[5].pubkey,
+        quote_vault=instruction.keys[6].pubkey,
         side=data.args.side,
         limit_price=data.args.limit_price,
         max_quantity=data.args.max_quantity,
         order_type=data.args.order_type,
         client_id=data.args.client_id,
     )
 
 
-def decode_match_orders(instruction: Instruction) -> MatchOrdersParams:
+def decode_match_orders(instruction: TransactionInstruction) -> MatchOrdersParams:
     """Decode a match orders instruction and retrieve the instruction params."""
     data = __parse_and_validate_instruction(instruction, InstructionType.MATCH_ORDER)
     return MatchOrdersParams(
-        market=instruction.accounts[0].pubkey,
-        request_queue=instruction.accounts[1].pubkey,
-        event_queue=instruction.accounts[2].pubkey,
-        bids=instruction.accounts[3].pubkey,
-        asks=instruction.accounts[4].pubkey,
-        base_vault=instruction.accounts[5].pubkey,
-        quote_vault=instruction.accounts[6].pubkey,
+        market=instruction.keys[0].pubkey,
+        request_queue=instruction.keys[1].pubkey,
+        event_queue=instruction.keys[2].pubkey,
+        bids=instruction.keys[3].pubkey,
+        asks=instruction.keys[4].pubkey,
+        base_vault=instruction.keys[5].pubkey,
+        quote_vault=instruction.keys[6].pubkey,
         limit=data.args.limit,
     )
 
 
-def decode_consume_events(instruction: Instruction) -> ConsumeEventsParams:
+def decode_consume_events(instruction: TransactionInstruction) -> ConsumeEventsParams:
     """Decode a consume events instruction and retrieve the instruction params."""
     data = __parse_and_validate_instruction(instruction, InstructionType.CONSUME_EVENTS)
     return ConsumeEventsParams(
-        open_orders_accounts=[a_m.pubkey for a_m in instruction.accounts[:-4]],
-        market=instruction.accounts[-4].pubkey,
-        event_queue=instruction.accounts[-3].pubkey,
+        open_orders_accounts=[a_m.pubkey for a_m in instruction.keys[:-4]],
+        market=instruction.keys[-4].pubkey,
+        event_queue=instruction.keys[-3].pubkey,
         # NOTE - ignoring pc_fee and coin_fee as unused
         limit=data.args.limit,
     )
 
 
-def decode_cancel_order(instruction: Instruction) -> CancelOrderParams:
+def decode_cancel_order(instruction: TransactionInstruction) -> CancelOrderParams:
     data = __parse_and_validate_instruction(instruction, InstructionType.CANCEL_ORDER)
     return CancelOrderParams(
-        market=instruction.accounts[0].pubkey,
-        open_orders=instruction.accounts[1].pubkey,
-        request_queue=instruction.accounts[2].pubkey,
-        owner=instruction.accounts[3].pubkey,
+        market=instruction.keys[0].pubkey,
+        open_orders=instruction.keys[1].pubkey,
+        request_queue=instruction.keys[2].pubkey,
+        owner=instruction.keys[3].pubkey,
         side=Side(data.args.side),
         order_id=int.from_bytes(data.args.order_id, "little"),
         open_orders_slot=data.args.open_orders_slot,
     )
 
 
-def decode_settle_funds(instruction: Instruction) -> SettleFundsParams:
+def decode_settle_funds(instruction: TransactionInstruction) -> SettleFundsParams:
     # data = __parse_and_validate_instruction(instruction, InstructionType.SettleFunds)
     return SettleFundsParams(
-        market=instruction.accounts[0].pubkey,
-        open_orders=instruction.accounts[1].pubkey,
-        owner=instruction.accounts[2].pubkey,
-        base_vault=instruction.accounts[3].pubkey,
-        quote_vault=instruction.accounts[4].pubkey,
-        base_wallet=instruction.accounts[5].pubkey,
-        quote_wallet=instruction.accounts[6].pubkey,
-        vault_signer=instruction.accounts[7].pubkey,
+        market=instruction.keys[0].pubkey,
+        open_orders=instruction.keys[1].pubkey,
+        owner=instruction.keys[2].pubkey,
+        base_vault=instruction.keys[3].pubkey,
+        quote_vault=instruction.keys[4].pubkey,
+        base_wallet=instruction.keys[5].pubkey,
+        quote_wallet=instruction.keys[6].pubkey,
+        vault_signer=instruction.keys[7].pubkey,
     )
 
 
 def decode_cancel_order_by_client_id(
-    instruction: Instruction,
+    instruction: TransactionInstruction,
 ) -> CancelOrderByClientIDParams:
-    data = __parse_and_validate_instruction(
-        instruction, InstructionType.CANCEL_ORDER_BY_CLIENT_ID
-    )
+    data = __parse_and_validate_instruction(instruction, InstructionType.CANCEL_ORDER_BY_CLIENT_ID)
     return CancelOrderByClientIDParams(
-        market=instruction.accounts[0].pubkey,
-        open_orders=instruction.accounts[1].pubkey,
-        request_queue=instruction.accounts[2].pubkey,
-        owner=instruction.accounts[3].pubkey,
+        market=instruction.keys[0].pubkey,
+        open_orders=instruction.keys[1].pubkey,
+        request_queue=instruction.keys[2].pubkey,
+        owner=instruction.keys[3].pubkey,
         client_id=data.args.client_id,
     )
 
 
-def decode_new_order_v3(instruction: Instruction) -> NewOrderV3Params:
+def decode_new_order_v3(instruction: TransactionInstruction) -> NewOrderV3Params:
     data = __parse_and_validate_instruction(instruction, InstructionType.NEW_ORDER_V3)
     return NewOrderV3Params(
-        market=instruction.accounts[0].pubkey,
-        open_orders=instruction.accounts[1].pubkey,
-        request_queue=instruction.accounts[2].pubkey,
-        event_queue=instruction.accounts[3].pubkey,
-        bids=instruction.accounts[4].pubkey,
-        asks=instruction.accounts[5].pubkey,
-        payer=instruction.accounts[6].pubkey,
-        owner=instruction.accounts[7].pubkey,
-        base_vault=instruction.accounts[8].pubkey,
-        quote_vault=instruction.accounts[9].pubkey,
+        market=instruction.keys[0].pubkey,
+        open_orders=instruction.keys[1].pubkey,
+        request_queue=instruction.keys[2].pubkey,
+        event_queue=instruction.keys[3].pubkey,
+        bids=instruction.keys[4].pubkey,
+        asks=instruction.keys[5].pubkey,
+        payer=instruction.keys[6].pubkey,
+        owner=instruction.keys[7].pubkey,
+        base_vault=instruction.keys[8].pubkey,
+        quote_vault=instruction.keys[9].pubkey,
         side=data.args.side,
         limit_price=data.args.limit_price,
         max_base_quantity=data.args.max_base_quantity,
         max_quote_quantity=data.args.max_quote_quantity,
         self_trade_behavior=SelfTradeBehavior(data.args.self_trade_behavior),
         order_type=OrderType(data.args.order_type),
         client_id=data.args.client_id,
         limit=data.args.limit,
     )
 
 
-def decode_cancel_order_v2(instruction: Instruction) -> CancelOrderV2Params:
-    data = __parse_and_validate_instruction(
-        instruction, InstructionType.CANCEL_ORDER_V2
-    )
+def decode_cancel_order_v2(instruction: TransactionInstruction) -> CancelOrderV2Params:
+    data = __parse_and_validate_instruction(instruction, InstructionType.CANCEL_ORDER_V2)
     return CancelOrderV2Params(
-        market=instruction.accounts[0].pubkey,
-        bids=instruction.accounts[1].pubkey,
-        asks=instruction.accounts[2].pubkey,
-        open_orders=instruction.accounts[3].pubkey,
-        owner=instruction.accounts[4].pubkey,
-        event_queue=instruction.accounts[5].pubkey,
+        market=instruction.keys[0].pubkey,
+        bids=instruction.keys[1].pubkey,
+        asks=instruction.keys[2].pubkey,
+        open_orders=instruction.keys[3].pubkey,
+        owner=instruction.keys[4].pubkey,
+        event_queue=instruction.keys[5].pubkey,
         side=Side(data.args.side),
         order_id=int.from_bytes(data.args.order_id, "little"),
         open_orders_slot=data.args.open_orders_slot,
     )
 
 
-def decode_cancel_order_by_client_id_v2(
-    instruction: Instruction,
-) -> CancelOrderByClientIDV2Params:
-    data = __parse_and_validate_instruction(
-        instruction, InstructionType.CANCEL_ORDER_BY_CLIENT_ID_V2
-    )
+def decode_cancel_order_by_client_id_v2(instruction: TransactionInstruction) -> CancelOrderByClientIDV2Params:
+    data = __parse_and_validate_instruction(instruction, InstructionType.CANCEL_ORDER_BY_CLIENT_ID_V2)
     return CancelOrderByClientIDV2Params(
-        market=instruction.accounts[0].pubkey,
-        bids=instruction.accounts[1].pubkey,
-        asks=instruction.accounts[2].pubkey,
-        open_orders=instruction.accounts[3].pubkey,
-        owner=instruction.accounts[4].pubkey,
-        event_queue=instruction.accounts[5].pubkey,
+        market=instruction.keys[0].pubkey,
+        bids=instruction.keys[1].pubkey,
+        asks=instruction.keys[2].pubkey,
+        open_orders=instruction.keys[3].pubkey,
+        owner=instruction.keys[4].pubkey,
+        event_queue=instruction.keys[5].pubkey,
         client_id=data.args.client_id,
     )
 
 
 def decode_close_open_orders(
-    instruction: Instruction,
+    instruction: TransactionInstruction,
 ) -> CloseOpenOrdersParams:
     return CloseOpenOrdersParams(
-        open_orders=instruction.accounts[0].pubkey,
-        owner=instruction.accounts[1].pubkey,
-        sol_wallet=instruction.accounts[2].pubkey,
-        market=instruction.accounts[3].pubkey,
+        open_orders=instruction.keys[0].pubkey,
+        owner=instruction.keys[1].pubkey,
+        sol_wallet=instruction.keys[2].pubkey,
+        market=instruction.keys[3].pubkey,
     )
 
 
 def decode_init_open_orders(
-    instruction: Instruction,
+    instruction: TransactionInstruction,
 ) -> InitOpenOrdersParams:
-    market_authority = (
-        instruction.accounts[-1].pubkey if len(instruction.accounts) == 5 else None
-    )
+    market_authority = instruction.keys[-1].pubkey if len(instruction.keys) == 5 else None
     return InitOpenOrdersParams(
-        open_orders=instruction.accounts[0].pubkey,
-        owner=instruction.accounts[1].pubkey,
-        market=instruction.accounts[2].pubkey,
+        open_orders=instruction.keys[0].pubkey,
+        owner=instruction.keys[1].pubkey,
+        market=instruction.keys[2].pubkey,
         market_authority=market_authority,
     )
 
 
-def initialize_market(params: InitializeMarketParams) -> Instruction:
+def initialize_market(params: InitializeMarketParams) -> TransactionInstruction:
     """Generate a transaction instruction to initialize a Serum market."""
-    return Instruction(
-        accounts=[
+    return TransactionInstruction(
+        keys=[
             AccountMeta(pubkey=params.market, is_signer=False, is_writable=False),
             AccountMeta(pubkey=params.request_queue, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.event_queue, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.bids, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.asks, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.base_vault, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.quote_vault, is_signer=False, is_writable=True),
@@ -548,27 +531,27 @@
                     quote_dust_threshold=params.quote_dust_threshold,
                 ),
             ),
         ),
     )
 
 
-def new_order(params: NewOrderParams) -> Instruction:
+def new_order(params: NewOrderParams) -> TransactionInstruction:
     """Generate a transaction instruction to place new order."""
-    return Instruction(
-        accounts=[
+    return TransactionInstruction(
+        keys=[
             AccountMeta(pubkey=params.market, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.open_orders, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.request_queue, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.payer, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.owner, is_signer=True, is_writable=False),
             AccountMeta(pubkey=params.base_vault, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.quote_vault, is_signer=False, is_writable=True),
             AccountMeta(pubkey=TOKEN_PROGRAM_ID, is_signer=False, is_writable=False),
-            AccountMeta(pubkey=RENT, is_signer=False, is_writable=False),
+            AccountMeta(pubkey=SYSVAR_RENT_PUBKEY, is_signer=False, is_writable=False),
         ],
         program_id=params.program_id,
         data=INSTRUCTIONS_LAYOUT.build(
             dict(
                 instruction_type=InstructionType.NEW_ORDER,
                 args=dict(
                     side=params.side,
@@ -578,18 +561,18 @@
                     client_id=params.client_id,
                 ),
             )
         ),
     )
 
 
-def match_orders(params: MatchOrdersParams) -> Instruction:
+def match_orders(params: MatchOrdersParams) -> TransactionInstruction:
     """Generate a transaction instruction to match order."""
-    return Instruction(
-        accounts=[
+    return TransactionInstruction(
+        keys=[
             AccountMeta(pubkey=params.market, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.request_queue, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.event_queue, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.bids, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.asks, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.base_vault, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.quote_vault, is_signer=False, is_writable=True),
@@ -600,38 +583,37 @@
                 instruction_type=InstructionType.MATCH_ORDER,
                 args=dict(limit=params.limit),
             )
         ),
     )
 
 
-def consume_events(params: ConsumeEventsParams) -> Instruction:
+def consume_events(params: ConsumeEventsParams) -> TransactionInstruction:
     """Generate a transaction instruction to consume market events."""
-    accounts = [
+    keys = [
         AccountMeta(pubkey=pubkey, is_signer=False, is_writable=True)
         # NOTE - last two accounts are required for backwards compatibility but are ignored
-        for pubkey in params.open_orders_accounts
-        + (2 * [params.market, params.event_queue])
+        for pubkey in params.open_orders_accounts + (2 * [params.market, params.event_queue])
     ]
-    return Instruction(
-        accounts=accounts,
+    return TransactionInstruction(
+        keys=keys,
         program_id=params.program_id,
         data=INSTRUCTIONS_LAYOUT.build(
             dict(
                 instruction_type=InstructionType.CONSUME_EVENTS,
                 args=dict(limit=params.limit),
             )
         ),
     )
 
 
-def cancel_order(params: CancelOrderParams) -> Instruction:
+def cancel_order(params: CancelOrderParams) -> TransactionInstruction:
     """Generate a transaction instruction to cancel order."""
-    return Instruction(
-        accounts=[
+    return TransactionInstruction(
+        keys=[
             AccountMeta(pubkey=params.market, is_signer=False, is_writable=False),
             AccountMeta(pubkey=params.open_orders, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.request_queue, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.owner, is_signer=True, is_writable=False),
         ],
         program_id=params.program_id,
         data=INSTRUCTIONS_LAYOUT.build(
@@ -644,41 +626,39 @@
                     open_orders_slot=params.open_orders_slot,
                 ),
             )
         ),
     )
 
 
-def settle_funds(params: SettleFundsParams) -> Instruction:
+def settle_funds(params: SettleFundsParams) -> TransactionInstruction:
     """Generate a transaction instruction to settle fund."""
-    return Instruction(
-        accounts=[
+    return TransactionInstruction(
+        keys=[
             AccountMeta(pubkey=params.market, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.open_orders, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.owner, is_signer=True, is_writable=False),
             AccountMeta(pubkey=params.base_vault, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.quote_vault, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.base_wallet, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.quote_wallet, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.vault_signer, is_signer=False, is_writable=False),
             AccountMeta(pubkey=TOKEN_PROGRAM_ID, is_signer=False, is_writable=False),
         ],
         program_id=params.program_id,
-        data=INSTRUCTIONS_LAYOUT.build(
-            dict(instruction_type=InstructionType.SETTLE_FUNDS, args=dict())
-        ),
+        data=INSTRUCTIONS_LAYOUT.build(dict(instruction_type=InstructionType.SETTLE_FUNDS, args=dict())),
     )
 
 
 def cancel_order_by_client_id(
     params: CancelOrderByClientIDParams,
-) -> Instruction:
+) -> TransactionInstruction:
     """Generate a transaction instruction to cancel order by client id."""
-    return Instruction(
-        accounts=[
+    return TransactionInstruction(
+        keys=[
             AccountMeta(pubkey=params.market, is_signer=False, is_writable=False),
             AccountMeta(pubkey=params.open_orders, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.request_queue, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.owner, is_signer=True, is_writable=False),
         ],
         program_id=params.program_id,
         data=INSTRUCTIONS_LAYOUT.build(
@@ -688,38 +668,36 @@
                     client_id=params.client_id,
                 ),
             )
         ),
     )
 
 
-def new_order_v3(params: NewOrderV3Params) -> Instruction:
+def new_order_v3(params: NewOrderV3Params) -> TransactionInstruction:
     """Generate a transaction instruction to place new order."""
-    touched_accounts = [
+    touched_keys = [
         AccountMeta(pubkey=params.market, is_signer=False, is_writable=True),
         AccountMeta(pubkey=params.open_orders, is_signer=False, is_writable=True),
         AccountMeta(pubkey=params.request_queue, is_signer=False, is_writable=True),
         AccountMeta(pubkey=params.event_queue, is_signer=False, is_writable=True),
         AccountMeta(pubkey=params.bids, is_signer=False, is_writable=True),
         AccountMeta(pubkey=params.asks, is_signer=False, is_writable=True),
         AccountMeta(pubkey=params.payer, is_signer=False, is_writable=True),
         AccountMeta(pubkey=params.owner, is_signer=True, is_writable=False),
         AccountMeta(pubkey=params.base_vault, is_signer=False, is_writable=True),
         AccountMeta(pubkey=params.quote_vault, is_signer=False, is_writable=True),
         AccountMeta(pubkey=TOKEN_PROGRAM_ID, is_signer=False, is_writable=False),
-        AccountMeta(pubkey=RENT, is_signer=False, is_writable=False),
+        AccountMeta(pubkey=SYSVAR_RENT_PUBKEY, is_signer=False, is_writable=False),
     ]
     if params.fee_discount_pubkey:
-        touched_accounts.append(
-            AccountMeta(
-                pubkey=params.fee_discount_pubkey, is_signer=False, is_writable=False
-            ),
+        touched_keys.append(
+            AccountMeta(pubkey=params.fee_discount_pubkey, is_signer=False, is_writable=False),
         )
-    return Instruction(
-        accounts=touched_accounts,
+    return TransactionInstruction(
+        keys=touched_keys,
         program_id=params.program_id,
         data=INSTRUCTIONS_LAYOUT.build(
             dict(
                 instruction_type=InstructionType.NEW_ORDER_V3,
                 args=dict(
                     side=params.side,
                     limit_price=params.limit_price,
@@ -731,18 +709,18 @@
                     limit=65535,
                 ),
             )
         ),
     )
 
 
-def cancel_order_v2(params: CancelOrderV2Params) -> Instruction:
+def cancel_order_v2(params: CancelOrderV2Params) -> TransactionInstruction:
     """Generate a transaction instruction to cancel order."""
-    return Instruction(
-        accounts=[
+    return TransactionInstruction(
+        keys=[
             AccountMeta(pubkey=params.market, is_signer=False, is_writable=False),
             AccountMeta(pubkey=params.bids, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.asks, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.open_orders, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.owner, is_signer=True, is_writable=False),
             AccountMeta(pubkey=params.event_queue, is_signer=False, is_writable=True),
         ],
@@ -757,18 +735,18 @@
             )
         ),
     )
 
 
 def cancel_order_by_client_id_v2(
     params: CancelOrderByClientIDV2Params,
-) -> Instruction:
+) -> TransactionInstruction:
     """Generate a transaction instruction to cancel order by client id."""
-    return Instruction(
-        accounts=[
+    return TransactionInstruction(
+        keys=[
             AccountMeta(pubkey=params.market, is_signer=False, is_writable=False),
             AccountMeta(pubkey=params.bids, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.asks, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.open_orders, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.owner, is_signer=True, is_writable=False),
             AccountMeta(pubkey=params.event_queue, is_signer=False, is_writable=True),
         ],
@@ -780,44 +758,38 @@
                     client_id=params.client_id,
                 ),
             )
         ),
     )
 
 
-def close_open_orders(params: CloseOpenOrdersParams) -> Instruction:
+def close_open_orders(params: CloseOpenOrdersParams) -> TransactionInstruction:
     """Generate a transaction instruction to close open orders account."""
-    return Instruction(
-        accounts=[
+    return TransactionInstruction(
+        keys=[
             AccountMeta(pubkey=params.open_orders, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.owner, is_signer=True, is_writable=False),
             AccountMeta(pubkey=params.sol_wallet, is_signer=False, is_writable=True),
             AccountMeta(pubkey=params.market, is_signer=False, is_writable=False),
         ],
         program_id=params.program_id,
-        data=INSTRUCTIONS_LAYOUT.build(
-            dict(instruction_type=InstructionType.CLOSE_OPEN_ORDERS, args=dict())
-        ),
+        data=INSTRUCTIONS_LAYOUT.build(dict(instruction_type=InstructionType.CLOSE_OPEN_ORDERS, args=dict())),
     )
 
 
-def init_open_orders(params: InitOpenOrdersParams) -> Instruction:
+def init_open_orders(params: InitOpenOrdersParams) -> TransactionInstruction:
     """Generate a transaction instruction to initialize open orders account."""
-    touched_accounts = [
+    touched_keys = [
         AccountMeta(pubkey=params.open_orders, is_signer=False, is_writable=True),
         AccountMeta(pubkey=params.owner, is_signer=True, is_writable=False),
         AccountMeta(pubkey=params.market, is_signer=False, is_writable=False),
-        AccountMeta(pubkey=RENT, is_signer=False, is_writable=False),
+        AccountMeta(pubkey=SYSVAR_RENT_PUBKEY, is_signer=False, is_writable=False),
     ]
     if params.market_authority:
-        touched_accounts.append(
-            AccountMeta(
-                pubkey=params.market_authority, is_signer=False, is_writable=False
-            ),
+        touched_keys.append(
+            AccountMeta(pubkey=params.market_authority, is_signer=False, is_writable=False),
         )
-    return Instruction(
-        accounts=touched_accounts,
+    return TransactionInstruction(
+        keys=touched_keys,
         program_id=params.program_id,
-        data=INSTRUCTIONS_LAYOUT.build(
-            dict(instruction_type=InstructionType.INIT_OPEN_ORDERS, args=dict())
-        ),
+        data=INSTRUCTIONS_LAYOUT.build(dict(instruction_type=InstructionType.INIT_OPEN_ORDERS, args=dict())),
     )
```

### Comparing `pyopenbook-0.7.0a0/pyserum/market/_internal/queue.py` & `pyopenbook-0.7.1a0/pyserum/market/_internal/queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,40 @@
 import math
 from enum import IntEnum
 from typing import List, Optional, Tuple, Union, cast
 
 from construct import Container
-from solders.pubkey import Pubkey
+from solana.publickey import PublicKey
+
 from ..._layouts.queue import EVENT_LAYOUT, QUEUE_HEADER_LAYOUT, REQUEST_LAYOUT
 from ..types import Event, EventFlags, Request, ReuqestFlags
 
 
 class QueueType(IntEnum):
     EVENT = 1
     REQUEST = 2
 
 
 def __from_bytes(
     buffer: bytes, queue_type: QueueType, history: Optional[int]
 ) -> Tuple[Container, List[Union[Event, Request]]]:
     header = QUEUE_HEADER_LAYOUT.parse(buffer)
-    layout_size = (
-        EVENT_LAYOUT.sizeof()
-        if queue_type == QueueType.EVENT
-        else REQUEST_LAYOUT.sizeof()
-    )
+    layout_size = EVENT_LAYOUT.sizeof() if queue_type == QueueType.EVENT else REQUEST_LAYOUT.sizeof()
     alloc_len = math.floor((len(buffer) - QUEUE_HEADER_LAYOUT.sizeof()) / layout_size)
     nodes: List[Union[Event, Request]] = []
     if history:
         for i in range(min(history, alloc_len)):
             node_index = (header.head + header.count + alloc_len - 1 - i) % alloc_len
             offset = QUEUE_HEADER_LAYOUT.sizeof() + node_index * layout_size
-            nodes.append(
-                __parse_queue_item(buffer[offset : offset + layout_size], queue_type)
-            )  # noqa: E203
+            nodes.append(__parse_queue_item(buffer[offset : offset + layout_size], queue_type))  # noqa: E203
     else:
         for i in range(header.count):
             node_index = (header.head + i) % alloc_len
             offset = QUEUE_HEADER_LAYOUT.sizeof() + node_index * layout_size
-            nodes.append(
-                __parse_queue_item(buffer[offset : offset + layout_size], queue_type)
-            )  # noqa: E203
+            nodes.append(__parse_queue_item(buffer[offset : offset + layout_size], queue_type))  # noqa: E203
     return header, nodes
 
 
 def __parse_queue_item(buffer: bytes, queue_type: QueueType) -> Union[Event, Request]:
     if queue_type == QueueType.EVENT:  # pylint: disable=no-else-return
         parsed_item = EVENT_LAYOUT.parse(buffer)
         parsed_event_flags = parsed_item.event_flags
@@ -56,15 +49,15 @@
             event_flags=event_flags,
             open_order_slot=parsed_item.open_order_slot,
             fee_tier=parsed_item.fee_tier,
             native_quantity_released=parsed_item.native_quantity_released,
             native_quantity_paid=parsed_item.native_quantity_paid,
             native_fee_or_rebate=parsed_item.native_fee_or_rebate,
             order_id=int.from_bytes(parsed_item.order_id, "little"),
-            public_key=Pubkey.from_bytes(parsed_item.public_key),
+            public_key=PublicKey(parsed_item.public_key),
             client_order_id=parsed_item.client_order_id,
         )
     else:
         parsed_item = REQUEST_LAYOUT.parse(buffer)
         parsed_request_flags = parsed_item.request_flags
         request_flags = ReuqestFlags(
             new_order=parsed_request_flags.new_order,
@@ -77,28 +70,24 @@
         return Request(
             request_flags=request_flags,
             open_order_slot=parsed_item.open_order_slot,
             fee_tier=parsed_item.fee_tier,
             max_base_size_or_cancel_id=parsed_item.max_base_size_or_cancel_id,
             native_quote_quantity_locked=parsed_item.native_quote_quantity_locked,
             order_id=int.from_bytes(parsed_item.order_id, "little"),
-            open_orders=Pubkey.from_bytes(parsed_item.open_orders),
+            open_orders=PublicKey(parsed_item.open_orders),
             client_order_id=parsed_item.client_order_id,
         )
 
 
 def decode_request_queue(buffer: bytes, history: Optional[int] = None) -> List[Request]:
     header, nodes = __from_bytes(buffer, QueueType.REQUEST, history)
     if not header.account_flags.initialized or not header.account_flags.request_queue:
-        raise Exception(
-            "Invalid requests queue, either not initialized or not a request queue."
-        )
+        raise Exception("Invalid requests queue, either not initialized or not a request queue.")
     return cast(List[Request], nodes)
 
 
 def decode_event_queue(buffer: bytes, history: Optional[int] = None) -> List[Event]:
     header, nodes = __from_bytes(buffer, QueueType.EVENT, history)
     if not header.account_flags.initialized or not header.account_flags.event_queue:
-        raise Exception(
-            "Invalid events queue, either not initialized or not a event queue."
-        )
+        raise Exception("Invalid events queue, either not initialized or not a event queue.")
     return cast(List[Event], nodes)
```

### Comparing `pyopenbook-0.7.0a0/pyserum/market/_internal/slab.py` & `pyopenbook-0.7.1a0/pyserum/market/_internal/slab.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Iterable, List, NamedTuple, Optional
 
 from construct import ListContainer
-from solders.pubkey import Pubkey
+from solana.publickey import PublicKey
+
 from ..._layouts.slab import SLAB_LAYOUT, NodeType
 
 
 class SlabHeader(NamedTuple):
     bump_index: int
     free_list_length: int
     free_list_root: int
@@ -28,15 +29,15 @@
 
 
 @dataclass(frozen=True)
 class SlabLeafNode(SlabNode):
     owner_slot: int
     fee_tier: int
     key: int
-    owner: Pubkey
+    owner: PublicKey
     quantity: int
     client_order_id: int
 
 
 @dataclass(frozen=True)
 class SlabInnerNode(SlabNode):
     prefix_len: int
@@ -59,15 +60,15 @@
                 res.append(SlabNode(is_initialized=False, next=-1))
             elif node_type == NodeType.LEAF_NODE:
                 res.append(
                     SlabLeafNode(
                         owner_slot=node.owner_slot,
                         fee_tier=node.fee_tier,
                         key=int.from_bytes(node.key, "little"),
-                        owner=Pubkey.from_bytes(node.owner),
+                        owner=PublicKey(node.owner),
                         quantity=node.quantity,
                         client_order_id=node.client_order_id,
                         is_initialized=True,
                         next=NONE_NEXT,
                     )
                 )
             elif node_type == NodeType.INNER_NODE:
```

### Comparing `pyopenbook-0.7.0a0/pyserum/market/async_market.py` & `pyopenbook-0.7.1a0/pyserum/market/market.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,131 +1,121 @@
 """Market module to interact with Serum DEX."""
 from __future__ import annotations
 
 from typing import List
 
-from solders.keypair import Keypair
-from solders.pubkey import Pubkey
-from solana.rpc.async_api import AsyncClient
+from solana.keypair import Keypair
+from solana.publickey import PublicKey
+from solana.rpc.api import Client
 from solana.rpc.types import TxOpts
 from solana.transaction import Transaction
 from solders.rpc.responses import SendTransactionResp
 
 import pyserum.market.types as t
 from pyserum import instructions
 
 from .._layouts.open_orders import OPEN_ORDERS_LAYOUT
-from ..async_open_orders_account import AsyncOpenOrdersAccount
-from ..async_utils import load_bytes_data
 from ..enums import OrderType, Side
+from ..open_orders_account import OpenOrdersAccount
+from ..utils import load_bytes_data
 from ._internal.queue import decode_event_queue, decode_request_queue
 from .core import MarketCore
 from .orderbook import OrderBook
 from .state import MarketState
 
 LAMPORTS_PER_SOL = 1000000000
 
 
 # pylint: disable=too-many-public-methods,abstract-method
-class AsyncMarket(MarketCore):
+class Market(MarketCore):
     """Represents a Serum Market."""
 
     def __init__(
         self,
-        conn: AsyncClient,
+        conn: Client,
         market_state: MarketState,
         force_use_request_queue: bool = False,
     ) -> None:
-        super().__init__(
-            market_state=market_state, force_use_request_queue=force_use_request_queue
-        )
+        super().__init__(market_state=market_state, force_use_request_queue=force_use_request_queue)
         self._conn = conn
 
     @classmethod
     # pylint: disable=unused-argument
-    async def load(
+    def load(
         cls,
-        conn: AsyncClient,
-        market_address: Pubkey,
-        program_id: Pubkey = instructions.DEFAULT_DEX_PROGRAM_ID,
+        conn: Client,
+        market_address: PublicKey,
+        program_id: PublicKey = instructions.DEFAULT_DEX_PROGRAM_ID,
         force_use_request_queue: bool = False,
-    ) -> AsyncMarket:
+    ) -> Market:
         """Factory method to create a Market.
 
         :param conn: The connection that we use to load the data, created from `solana.rpc.api`.
         :param market_address: The market address that you want to connect to.
         :param program_id: The program id of the given market, it will use the default value if not provided.
         """
-        market_state = await MarketState.async_load(conn, market_address, program_id)
+        market_state = MarketState.load(conn, market_address, program_id)
         return cls(conn, market_state, force_use_request_queue)
 
-    async def find_open_orders_accounts_for_owner(
-        self, owner_address: Pubkey
-    ) -> List[AsyncOpenOrdersAccount]:
-        return await AsyncOpenOrdersAccount.find_for_market_and_owner(
+    def find_open_orders_accounts_for_owner(self, owner_address: PublicKey) -> List[OpenOrdersAccount]:
+        return OpenOrdersAccount.find_for_market_and_owner(
             self._conn, self.state.public_key(), owner_address, self.state.program_id()
         )
 
-    async def load_bids(self) -> OrderBook:
+    def load_bids(self) -> OrderBook:
         """Load the bid order book"""
-        bytes_data = await load_bytes_data(self.state.bids(), self._conn)
+        bytes_data = load_bytes_data(self.state.bids(), self._conn)
         return self._parse_bids_or_asks(bytes_data)
 
-    async def load_asks(self) -> OrderBook:
+    def load_asks(self) -> OrderBook:
         """Load the ask order book."""
-        bytes_data = await load_bytes_data(self.state.asks(), self._conn)
+        bytes_data = load_bytes_data(self.state.asks(), self._conn)
         return self._parse_bids_or_asks(bytes_data)
 
-    async def load_orders_for_owner(self, owner_address: Pubkey) -> List[t.Order]:
+    def load_orders_for_owner(self, owner_address: PublicKey) -> List[t.Order]:
         """Load orders for owner."""
-        bids = await self.load_bids()
-        asks = await self.load_asks()
-        open_orders_accounts = await self.find_open_orders_accounts_for_owner(
-            owner_address
-        )
+        bids = self.load_bids()
+        asks = self.load_asks()
+        open_orders_accounts = self.find_open_orders_accounts_for_owner(owner_address)
         return self._parse_orders_for_owner(bids, asks, open_orders_accounts)
 
-    async def load_event_queue(self) -> List[t.Event]:
+    def load_event_queue(self) -> List[t.Event]:
         """Load the event queue which includes the fill item and out item. For any trades two fill items are added to
         the event queue. And in case of a trade, cancel or IOC order that missed, out items are added to the event
         queue.
         """
-        bytes_data = await load_bytes_data(self.state.event_queue(), self._conn)
+        bytes_data = load_bytes_data(self.state.event_queue(), self._conn)
         return decode_event_queue(bytes_data)
 
-    async def load_request_queue(self) -> List[t.Request]:
-        bytes_data = await load_bytes_data(self.state.request_queue(), self._conn)
+    def load_request_queue(self) -> List[t.Request]:
+        bytes_data = load_bytes_data(self.state.request_queue(), self._conn)
         return decode_request_queue(bytes_data)
 
-    async def load_fills(self, limit=100) -> List[t.FilledOrder]:
-        bytes_data = await load_bytes_data(self.state.event_queue(), self._conn)
+    def load_fills(self, limit=100) -> List[t.FilledOrder]:
+        bytes_data = load_bytes_data(self.state.event_queue(), self._conn)
         return self._parse_fills(bytes_data, limit)
 
-    async def place_order(  # pylint: disable=too-many-arguments,too-many-locals
+    def place_order(  # pylint: disable=too-many-arguments,too-many-locals
         self,
-        payer: Pubkey,
+        payer: PublicKey,
         owner: Keypair,
         order_type: OrderType,
         side: Side,
         limit_price: float,
         max_quantity: float,
         client_id: int = 0,
         opts: TxOpts = TxOpts(),
     ) -> SendTransactionResp:  # TODO: Add open_orders_address_key param and fee_discount_pubkey
         transaction = Transaction()
         signers: List[Keypair] = [owner]
-        open_order_accounts = await self.find_open_orders_accounts_for_owner(
-            owner.pubkey()
-        )
+        open_order_accounts = self.find_open_orders_accounts_for_owner(owner.public_key)
         if open_order_accounts:
             place_order_open_order_account = open_order_accounts[0].address
         else:
-            mbfre_resp = await self._conn.get_minimum_balance_for_rent_exemption(
-                OPEN_ORDERS_LAYOUT.sizeof()
-            )
+            mbfre_resp = self._conn.get_minimum_balance_for_rent_exemption(OPEN_ORDERS_LAYOUT.sizeof())
             place_order_open_order_account = self._after_oo_mbfre_resp(
                 mbfre_resp=mbfre_resp,
                 owner=owner,
                 signers=signers,
                 transaction=transaction,
             )
             # TODO: Cache new_open_orders_account
@@ -140,59 +130,53 @@
             signers=signers,
             limit_price=limit_price,
             max_quantity=max_quantity,
             client_id=client_id,
             open_order_accounts=open_order_accounts,
             place_order_open_order_account=place_order_open_order_account,
         )
-        return await self._conn.send_transaction(transaction, *signers, opts=opts)
+        return self._conn.send_transaction(transaction, *signers, opts=opts)
 
-    async def cancel_order_by_client_id(
+    def cancel_order_by_client_id(
         self,
         owner: Keypair,
-        open_orders_account: Pubkey,
+        open_orders_account: PublicKey,
         client_id: int,
         opts: TxOpts = TxOpts(),
     ) -> SendTransactionResp:
         txs = self._build_cancel_order_by_client_id_tx(
             owner=owner, open_orders_account=open_orders_account, client_id=client_id
         )
-        return await self._conn.send_transaction(txs, owner, opts=opts)
+        return self._conn.send_transaction(txs, owner, opts=opts)
 
-    async def cancel_order(
-        self, owner: Keypair, order: t.Order, opts: TxOpts = TxOpts()
-    ) -> SendTransactionResp:
+    def cancel_order(self, owner: Keypair, order: t.Order, opts: TxOpts = TxOpts()) -> SendTransactionResp:
         txn = self._build_cancel_order_tx(owner=owner, order=order)
-        return await self._conn.send_transaction(txn, owner, opts=opts)
+        return self._conn.send_transaction(txn, owner, opts=opts)
 
-    async def match_orders(
-        self, fee_payer: Keypair, limit: int, opts: TxOpts = TxOpts()
-    ) -> SendTransactionResp:
+    def match_orders(self, fee_payer: Keypair, limit: int, opts: TxOpts = TxOpts()) -> SendTransactionResp:
         txn = self._build_match_orders_tx(limit)
-        return await self._conn.send_transaction(txn, fee_payer, opts=opts)
+        return self._conn.send_transaction(txn, fee_payer, opts=opts)
 
-    async def settle_funds(  # pylint: disable=too-many-arguments
+    def settle_funds(  # pylint: disable=too-many-arguments
         self,
         owner: Keypair,
-        open_orders: AsyncOpenOrdersAccount,
-        base_wallet: Pubkey,
-        quote_wallet: Pubkey,  # TODO: add referrer_quote_wallet.
+        open_orders: OpenOrdersAccount,
+        base_wallet: PublicKey,
+        quote_wallet: PublicKey,  # TODO: add referrer_quote_wallet.
         opts: TxOpts = TxOpts(),
     ) -> SendTransactionResp:
         # TODO: Handle wrapped sol accounts
         should_wrap_sol = self._settle_funds_should_wrap_sol()
-        if should_wrap_sol:
-            mbfre_resp = await self._conn.get_minimum_balance_for_rent_exemption(165)
-            min_bal_for_rent_exemption = mbfre_resp.value
-        else:
-            min_bal_for_rent_exemption = 0  # value only matters if should_wrap_sol
+        min_bal_for_rent_exemption = (
+            self._conn.get_minimum_balance_for_rent_exemption(165).value if should_wrap_sol else 0
+        )  # value only matters if should_wrap_sol
         signers = [owner]
         transaction = self._build_settle_funds_tx(
             owner=owner,
             signers=signers,
             open_orders=open_orders,
             base_wallet=base_wallet,
             quote_wallet=quote_wallet,
             min_bal_for_rent_exemption=min_bal_for_rent_exemption,
             should_wrap_sol=should_wrap_sol,
         )
-        return await self._conn.send_transaction(transaction, *signers, opts=opts)
+        return self._conn.send_transaction(transaction, *signers, opts=opts)
```

### Comparing `pyopenbook-0.7.0a0/pyserum/market/core.py` & `pyopenbook-0.7.1a0/pyserum/market/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Market module to interact with Serum DEX."""
 from __future__ import annotations
 
 import itertools
 import logging
 from typing import List, Union
 
-from solders.keypair import Keypair
-from solders.pubkey import Pubkey
-from solders.system_program import CreateAccountParams, create_account
-from solana.transaction import Transaction
-from solders.instruction import Instruction
+from solana.keypair import Keypair
+from solana.publickey import PublicKey
+from solana.system_program import CreateAccountParams, create_account
+from solana.transaction import Transaction, TransactionInstruction
 from solders.rpc.responses import GetMinimumBalanceForRentExemptionResp
 from spl.token.constants import ACCOUNT_LEN, TOKEN_PROGRAM_ID, WRAPPED_SOL_MINT
 from spl.token.instructions import (
     CloseAccountParams,
     InitializeAccountParams,
     close_account,
     initialize_account,
@@ -25,74 +24,63 @@
 from ..async_open_orders_account import AsyncOpenOrdersAccount
 from ..enums import OrderType, SelfTradeBehavior, Side
 from ..open_orders_account import OpenOrdersAccount, make_create_account_instruction
 from ._internal.queue import decode_event_queue
 from .orderbook import OrderBook
 from .state import MarketState
 
-from decimal import Decimal
-
 LAMPORTS_PER_SOL = 1000000000
 
 
 # pylint: disable=too-many-public-methods
 class MarketCore:
     """Represents a Serum Market."""
 
     logger = logging.getLogger("pyserum.market.Market")
 
-    def __init__(
-        self, market_state: MarketState, force_use_request_queue: bool = False
-    ) -> None:
+    def __init__(self, market_state: MarketState, force_use_request_queue: bool = False) -> None:
         self.state = market_state
         self.force_use_request_queue = force_use_request_queue
 
     def _use_request_queue(self) -> bool:
         return (
             # DEX Version 1
-            self.state.program_id
-            == Pubkey.from_string("4ckmDgGdxQoPDLUkDT3vHgSAkzA3QRdNq5ywwY4sUSJn")
+            self.state.program_id == PublicKey("4ckmDgGdxQoPDLUkDT3vHgSAkzA3QRdNq5ywwY4sUSJn")
             or
             # DEX Version 1
-            self.state.program_id
-            == Pubkey.from_string("BJ3jrUzddfuSrZHXSCxMUUQsjKEyLmuuyZebkcaFp2fg")
+            self.state.program_id == PublicKey("BJ3jrUzddfuSrZHXSCxMUUQsjKEyLmuuyZebkcaFp2fg")
             or
             # DEX Version 2
-            self.state.program_id
-            == Pubkey.from_string("EUqojwWA2rd19FZrzeBncJsm38Jm1hEhE3zsmX3bRc2o")
+            self.state.program_id == PublicKey("EUqojwWA2rd19FZrzeBncJsm38Jm1hEhE3zsmX3bRc2o")
             or self.force_use_request_queue
         )
 
     def support_srm_fee_discounts(self) -> bool:
         raise NotImplementedError("support_srm_fee_discounts not implemented")
 
-    def find_fee_discount_keys(self, owner: Pubkey, cache_duration: int):
+    def find_fee_discount_keys(self, owner: PublicKey, cache_duration: int):
         raise NotImplementedError("find_fee_discount_keys not implemented")
 
-    def find_best_fee_discount_key(self, owner: Pubkey, cache_duration: int):
+    def find_best_fee_discount_key(self, owner: PublicKey, cache_duration: int):
         raise NotImplementedError("find_best_fee_discount_key not implemented")
 
-    def find_quote_token_accounts_for_owner(
-        self, owner_address: Pubkey, include_unwrapped_sol: bool = False
-    ):
+    def find_quote_token_accounts_for_owner(self, owner_address: PublicKey, include_unwrapped_sol: bool = False):
         raise NotImplementedError("find_quote_token_accounts_for_owner not implemented")
 
     def _parse_bids_or_asks(self, bytes_data: bytes) -> OrderBook:
         return OrderBook.from_bytes(self.state, bytes_data)
 
     @staticmethod
     def _parse_orders_for_owner(bids, asks, open_orders_accounts) -> List[t.Order]:
         if not open_orders_accounts:
             return []
 
         all_orders = itertools.chain(bids.orders(), asks.orders())
         open_orders_addresses = {str(o.address) for o in open_orders_accounts}
-        orders = [
-            o for o in all_orders if str(o.open_order_address) in open_orders_addresses
-        ]
+        orders = [o for o in all_orders if str(o.open_order_address) in open_orders_addresses]
         return orders
 
     def load_base_token_for_owner(self):
         raise NotImplementedError("load_base_token_for_owner not implemented")
 
     def _parse_fills(self, bytes_data: bytes, limit: int) -> List[t.FilledOrder]:
         events = decode_event_queue(bytes_data, limit)
@@ -100,122 +88,108 @@
             self.parse_fill_event(event)
             for event in events
             if event.event_flags.fill and event.native_quantity_paid > 0
         ]
 
     def parse_fill_event(self, event: t.Event) -> t.FilledOrder:
         if event.event_flags.bid:
-            side = 'bids'
-
+            side = Side.BUY
             price_before_fees = (
-                event.native_quantity_paid + event.native_fee_or_rebate
+                event.native_quantity_released + event.native_fee_or_rebate
                 if event.event_flags.maker
-                else event.native_quantity_paid - event.native_fee_or_rebate
-            )
-
-            price = (price_before_fees * self.state.base_spl_token_multiplier()) / (
-                    self.state.quote_spl_token_multiplier() * event.native_quantity_released
+                else event.native_quantity_released - event.native_fee_or_rebate
             )
-
-            size = event.native_quantity_released / self.state.base_spl_token_multiplier()
         else:
-            side = 'asks'
-
+            side = Side.SELL
             price_before_fees = (
                 event.native_quantity_released - event.native_fee_or_rebate
                 if event.event_flags.maker
                 else event.native_quantity_released + event.native_fee_or_rebate
             )
 
-            price = (price_before_fees * self.state.base_spl_token_multiplier()) / (
-                self.state.quote_spl_token_multiplier() * event.native_quantity_paid
-            )
-
-            size = event.native_quantity_paid / self.state.base_spl_token_multiplier()
-
+        price = (price_before_fees * self.state.base_spl_token_multiplier()) / (
+            self.state.quote_spl_token_multiplier() * event.native_quantity_paid
+        )
+        size = event.native_quantity_paid / self.state.base_spl_token_multiplier()
         return t.FilledOrder(
-            client_order_id=event.client_order_id,
+            order_id=event.order_id,
             side=side,
             price=price,
             size=size,
-            fee_cost=float(
-                (Decimal(event.native_fee_or_rebate) / Decimal(self.state.base_spl_token_multiplier())) * Decimal(1 if event.event_flags.maker else -1)
-            )
+            fee_cost=event.native_fee_or_rebate * (1 if event.event_flags.maker else -1),
         )
 
     def _prepare_new_oo_account(
         self,
         owner: Keypair,
         balance_needed: int,
         signers: List[Keypair],
         transaction: Transaction,
-    ) -> Pubkey:
+    ) -> PublicKey:
         # new_open_orders_account = Account()
         new_open_orders_account = Keypair()
-        place_order_open_order_account = new_open_orders_account.pubkey()
+        place_order_open_order_account = new_open_orders_account.public_key
         transaction.add(
             make_create_account_instruction(
-                owner_address=owner.pubkey(),
-                new_account_address=new_open_orders_account.pubkey(),
+                owner_address=owner.public_key,
+                new_account_address=new_open_orders_account.public_key,
                 lamports=balance_needed,
                 program_id=self.state.program_id(),
             )
         )
         signers.append(new_open_orders_account)
         return place_order_open_order_account
 
     def _prepare_order_transaction(  # pylint: disable=too-many-arguments,too-many-locals
         self,
         transaction: Transaction,
-        payer: Pubkey,
+        payer: PublicKey,
         owner: Keypair,
         order_type: OrderType,
         side: Side,
         signers: List[Keypair],
         limit_price: float,
         max_quantity: float,
         client_id: int,
-        open_order_accounts: Union[
-            List[OpenOrdersAccount], List[AsyncOpenOrdersAccount]
-        ],
-        place_order_open_order_account: Pubkey,
+        open_order_accounts: Union[List[OpenOrdersAccount], List[AsyncOpenOrdersAccount]],
+        place_order_open_order_account: PublicKey,
     ) -> None:
         # unwrapped SOL cannot be used for payment
-        if payer == owner.pubkey():
+        if payer == owner.public_key:
             raise ValueError("Invalid payer account. Cannot use unwrapped SOL.")
 
         # TODO: add integration test for SOL wrapping.
-        should_wrap_sol = (
-            side == Side.BUY and self.state.quote_mint() == WRAPPED_SOL_MINT
-        ) or (side == Side.SELL and self.state.base_mint() == WRAPPED_SOL_MINT)
+        should_wrap_sol = (side == Side.BUY and self.state.quote_mint() == WRAPPED_SOL_MINT) or (
+            side == Side.SELL and self.state.base_mint() == WRAPPED_SOL_MINT
+        )
 
         if should_wrap_sol:
             # wrapped_sol_account = Account()
             wrapped_sol_account = Keypair()
-            payer = wrapped_sol_account.pubkey()
+            payer = wrapped_sol_account.public_key
             signers.append(wrapped_sol_account)
             transaction.add(
                 create_account(
                     CreateAccountParams(
-                        from_pubkey=owner.pubkey(),
-                        to_pubkey=wrapped_sol_account.pubkey(),
+                        from_pubkey=owner.public_key,
+                        new_account_pubkey=wrapped_sol_account.public_key,
                         lamports=self._get_lamport_need_for_sol_wrapping(
                             limit_price, max_quantity, side, open_order_accounts
                         ),
                         space=ACCOUNT_LEN,
-                        owner=TOKEN_PROGRAM_ID,
+                        program_id=TOKEN_PROGRAM_ID,
                     )
                 )
             )
             transaction.add(
                 initialize_account(
                     InitializeAccountParams(
-                        account=wrapped_sol_account.pubkey(),
+                        account=wrapped_sol_account.public_key,
                         mint=WRAPPED_SOL_MINT,
-                        owner=owner.pubkey(),
+                        owner=owner.public_key,
                         program_id=TOKEN_PROGRAM_ID,
                     )
                 )
             )
 
         transaction.add(
             self.make_place_order_instruction(
@@ -230,43 +204,39 @@
             )
         )
 
         if should_wrap_sol:
             transaction.add(
                 close_account(
                     CloseAccountParams(
-                        account=wrapped_sol_account.pubkey(),
-                        owner=owner.pubkey(),
-                        dest=owner.pubkey(),
+                        account=wrapped_sol_account.public_key,
+                        owner=owner.public_key,
+                        dest=owner.public_key,
                         program_id=TOKEN_PROGRAM_ID,
                     )
                 )
             )
 
     def _after_oo_mbfre_resp(
         self,
         mbfre_resp: GetMinimumBalanceForRentExemptionResp,
         owner: Keypair,
         signers: List[Keypair],
         transaction: Transaction,
-    ) -> Pubkey:
+    ) -> PublicKey:
         balance_needed = mbfre_resp.value
-        place_order_open_order_account = self._prepare_new_oo_account(
-            owner, balance_needed, signers, transaction
-        )
+        place_order_open_order_account = self._prepare_new_oo_account(owner, balance_needed, signers, transaction)
         return place_order_open_order_account
 
     @staticmethod
     def _get_lamport_need_for_sol_wrapping(
         price: float,
         size: float,
         side: Side,
-        open_orders_accounts: Union[
-            List[OpenOrdersAccount], List[AsyncOpenOrdersAccount]
-        ],
+        open_orders_accounts: Union[List[OpenOrdersAccount], List[AsyncOpenOrdersAccount]],
     ) -> int:
         lamports = 0
         if side == Side.BUY:
             lamports = round(price * size * 1.01 * LAMPORTS_PER_SOL)
             if open_orders_accounts:
                 lamports -= open_orders_accounts[0].quote_token_free
         else:
@@ -274,35 +244,35 @@
             if open_orders_accounts:
                 lamports -= open_orders_accounts[0].base_token_free
 
         return max(lamports, 0) + 10000000
 
     def make_place_order_instruction(  # pylint: disable=too-many-arguments
         self,
-        payer: Pubkey,
+        payer: PublicKey,
         owner: Keypair,
         order_type: OrderType,
         side: Side,
         limit_price: float,
         max_quantity: float,
         client_id: int,
-        open_order_account: Pubkey,
-        fee_discount_pubkey: Pubkey = None,
-    ) -> Instruction:
+        open_order_account: PublicKey,
+        fee_discount_pubkey: PublicKey = None,
+    ) -> TransactionInstruction:
         if self.state.base_size_number_to_lots(max_quantity) < 0:
             raise Exception(f"Size lot %d is too small {max_quantity}")
         if self.state.price_number_to_lots(limit_price) < 0:
             raise Exception(f"Price lot %d is too small {limit_price}")
         if self._use_request_queue():
             return instructions.new_order(
                 instructions.NewOrderParams(
                     market=self.state.public_key(),
                     open_orders=open_order_account,
                     payer=payer,
-                    owner=owner.pubkey(),
+                    owner=owner.public_key,
                     request_queue=self.state.request_queue(),
                     base_vault=self.state.base_vault(),
                     quote_vault=self.state.quote_vault(),
                     side=side,
                     limit_price=self.state.price_number_to_lots(limit_price),
                     max_quantity=self.state.base_size_number_to_lots(max_quantity),
                     order_type=order_type,
@@ -311,15 +281,15 @@
                 )
             )
         return instructions.new_order_v3(
             instructions.NewOrderV3Params(
                 market=self.state.public_key(),
                 open_orders=open_order_account,
                 payer=payer,
-                owner=owner.pubkey(),
+                owner=owner.public_key,
                 request_queue=self.state.request_queue(),
                 event_queue=self.state.event_queue(),
                 bids=self.state.bids(),
                 asks=self.state.asks(),
                 base_vault=self.state.base_vault(),
                 quote_vault=self.state.quote_vault(),
                 side=side,
@@ -334,57 +304,49 @@
                 self_trade_behavior=SelfTradeBehavior.DECREMENT_TAKE,
                 fee_discount_pubkey=fee_discount_pubkey,
                 limit=65535,
             )
         )
 
     def _build_cancel_order_by_client_id_tx(
-        self, owner: Keypair, open_orders_account: Pubkey, client_id: int
+        self, owner: Keypair, open_orders_account: PublicKey, client_id: int
     ) -> Transaction:
-        return Transaction().add(
-            self.make_cancel_order_by_client_id_instruction(
-                owner, open_orders_account, client_id
-            )
-        )
+        return Transaction().add(self.make_cancel_order_by_client_id_instruction(owner, open_orders_account, client_id))
 
     def make_cancel_order_by_client_id_instruction(
-        self, owner: Keypair, open_orders_account: Pubkey, client_id: int
-    ) -> Instruction:
+        self, owner: Keypair, open_orders_account: PublicKey, client_id: int
+    ) -> TransactionInstruction:
         if self._use_request_queue():
             return instructions.cancel_order_by_client_id(
                 instructions.CancelOrderByClientIDParams(
                     market=self.state.public_key(),
-                    owner=owner.pubkey(),
+                    owner=owner.public_key,
                     open_orders=open_orders_account,
                     request_queue=self.state.request_queue(),
                     client_id=client_id,
                     program_id=self.state.program_id(),
                 )
             )
         return instructions.cancel_order_by_client_id_v2(
             instructions.CancelOrderByClientIDV2Params(
                 market=self.state.public_key(),
-                owner=owner.pubkey(),
+                owner=owner.public_key,
                 open_orders=open_orders_account,
                 bids=self.state.bids(),
                 asks=self.state.asks(),
                 event_queue=self.state.event_queue(),
                 client_id=client_id,
                 program_id=self.state.program_id(),
             )
         )
 
     def _build_cancel_order_tx(self, owner: Keypair, order: t.Order) -> Transaction:
-        return Transaction().add(
-            self.make_cancel_order_instruction(owner.pubkey(), order)
-        )
+        return Transaction().add(self.make_cancel_order_instruction(owner.public_key, order))
 
-    def make_cancel_order_instruction(
-        self, owner: Pubkey, order: t.Order
-    ) -> Instruction:
+    def make_cancel_order_instruction(self, owner: PublicKey, order: t.Order) -> TransactionInstruction:
         if self._use_request_queue():
             return instructions.cancel_order(
                 instructions.CancelOrderParams(
                     market=self.state.public_key(),
                     owner=owner,
                     open_orders=order.open_order_address,
                     request_queue=self.state.request_queue(),
@@ -408,15 +370,15 @@
                 program_id=self.state.program_id(),
             )
         )
 
     def _build_match_orders_tx(self, limit: int) -> Transaction:
         return Transaction().add(self.make_match_orders_instruction(limit))
 
-    def make_match_orders_instruction(self, limit: int) -> Instruction:
+    def make_match_orders_instruction(self, limit: int) -> TransactionInstruction:
         params = instructions.MatchOrdersParams(
             market=self.state.public_key(),
             request_queue=self.state.request_queue(),
             event_queue=self.state.event_queue(),
             bids=self.state.bids(),
             asks=self.state.asks(),
             base_vault=self.state.base_vault(),
@@ -427,23 +389,23 @@
         return instructions.match_orders(params)
 
     def _build_settle_funds_tx(  # pylint: disable=too-many-arguments
         self,
         owner: Keypair,
         signers: List[Keypair],
         open_orders: Union[OpenOrdersAccount, AsyncOpenOrdersAccount],
-        base_wallet: Pubkey,
-        quote_wallet: Pubkey,  # TODO: add referrer_quote_wallet.
+        base_wallet: PublicKey,
+        quote_wallet: PublicKey,  # TODO: add referrer_quote_wallet.
         min_bal_for_rent_exemption: int,
         should_wrap_sol: bool,
     ) -> Transaction:
         # TODO: Handle wrapped sol accounts
-        if open_orders.owner != owner.pubkey():
+        if open_orders.owner != owner.public_key:
             raise Exception("Invalid open orders account")
-        vault_signer = Pubkey.create_program_address(
+        vault_signer = PublicKey.create_program_address(
             [
                 bytes(self.state.public_key()),
                 self.state.vault_signer_nonce().to_bytes(8, byteorder="little"),
             ],
             self.state.program_id(),
         )
         transaction = Transaction()
@@ -452,73 +414,67 @@
             wrapped_sol_account = Keypair()
             signers.append(wrapped_sol_account)
             # make a wrapped SOL account with enough balance to
             # fund the trade, run the program, then send itself back home
             transaction.add(
                 create_account(
                     CreateAccountParams(
-                        from_pubkey=owner.pubkey(),
-                        to_pubkey=wrapped_sol_account.pubkey(),
+                        from_pubkey=owner.public_key,
+                        new_account_pubkey=wrapped_sol_account.public_key,
                         lamports=min_bal_for_rent_exemption,
                         space=ACCOUNT_LEN,
-                        owner=TOKEN_PROGRAM_ID,
+                        program_id=TOKEN_PROGRAM_ID,
                     )
                 )
             )
             # this was also broken upstream. it should be minting wrapped SOL, and using the token program ID
             transaction.add(
                 initialize_account(
                     InitializeAccountParams(
-                        account=wrapped_sol_account.pubkey(),
+                        account=wrapped_sol_account.public_key,
                         mint=WRAPPED_SOL_MINT,
-                        owner=owner.pubkey(),
+                        owner=owner.public_key,
                         program_id=TOKEN_PROGRAM_ID,
                     )
                 )
             )
 
         transaction.add(
             self.make_settle_funds_instruction(
                 open_orders,
-                base_wallet
-                if self.state.base_mint() != WRAPPED_SOL_MINT
-                else wrapped_sol_account.pubkey(),
-                quote_wallet
-                if self.state.quote_mint() != WRAPPED_SOL_MINT
-                else wrapped_sol_account.pubkey(),
+                base_wallet if self.state.base_mint() != WRAPPED_SOL_MINT else wrapped_sol_account.public_key,
+                quote_wallet if self.state.quote_mint() != WRAPPED_SOL_MINT else wrapped_sol_account.public_key,
                 vault_signer,
             )
         )
 
         if should_wrap_sol:
             # close out the account and send the funds home when the trade is completed/cancelled
             transaction.add(
                 close_account(
                     CloseAccountParams(
-                        account=wrapped_sol_account.pubkey(),
-                        owner=owner.pubkey(),
-                        dest=owner.pubkey(),
+                        account=wrapped_sol_account.public_key,
+                        owner=owner.public_key,
+                        dest=owner.public_key,
                         program_id=TOKEN_PROGRAM_ID,
                     )
                 )
             )
         return transaction
 
     def _settle_funds_should_wrap_sol(self) -> bool:
-        return (self.state.quote_mint() == WRAPPED_SOL_MINT) or (
-            self.state.base_mint() == WRAPPED_SOL_MINT
-        )
+        return (self.state.quote_mint() == WRAPPED_SOL_MINT) or (self.state.base_mint() == WRAPPED_SOL_MINT)
 
     def make_settle_funds_instruction(
         self,
         open_orders_account: Union[OpenOrdersAccount, AsyncOpenOrdersAccount],
-        base_wallet: Pubkey,
-        quote_wallet: Pubkey,
-        vault_signer: Pubkey,
-    ) -> Instruction:
+        base_wallet: PublicKey,
+        quote_wallet: PublicKey,
+        vault_signer: PublicKey,
+    ) -> TransactionInstruction:
         if base_wallet == self.state.base_vault():
             raise ValueError("base_wallet should not be a vault address")
         if quote_wallet == self.state.quote_vault():
             raise ValueError("quote_wallet should not be a vault address")
 
         return instructions.settle_funds(
             instructions.SettleFundsParams(
```

### Comparing `pyopenbook-0.7.0a0/pyserum/market/market.py` & `pyopenbook-0.7.1a0/pyserum/market/async_market.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,127 +1,121 @@
 """Market module to interact with Serum DEX."""
 from __future__ import annotations
 
 from typing import List
 
-from solders.keypair import Keypair
-from solders.pubkey import Pubkey
-from solana.rpc.api import Client
+from solana.keypair import Keypair
+from solana.publickey import PublicKey
+from solana.rpc.async_api import AsyncClient
 from solana.rpc.types import TxOpts
 from solana.transaction import Transaction
 from solders.rpc.responses import SendTransactionResp
 
 import pyserum.market.types as t
 from pyserum import instructions
 
 from .._layouts.open_orders import OPEN_ORDERS_LAYOUT
+from ..async_open_orders_account import AsyncOpenOrdersAccount
+from ..async_utils import load_bytes_data
 from ..enums import OrderType, Side
-from ..open_orders_account import OpenOrdersAccount
-from ..utils import load_bytes_data
 from ._internal.queue import decode_event_queue, decode_request_queue
 from .core import MarketCore
 from .orderbook import OrderBook
 from .state import MarketState
 
 LAMPORTS_PER_SOL = 1000000000
 
 
 # pylint: disable=too-many-public-methods,abstract-method
-class Market(MarketCore):
+class AsyncMarket(MarketCore):
     """Represents a Serum Market."""
 
     def __init__(
         self,
-        conn: Client,
+        conn: AsyncClient,
         market_state: MarketState,
         force_use_request_queue: bool = False,
     ) -> None:
-        super().__init__(
-            market_state=market_state, force_use_request_queue=force_use_request_queue
-        )
+        super().__init__(market_state=market_state, force_use_request_queue=force_use_request_queue)
         self._conn = conn
 
     @classmethod
     # pylint: disable=unused-argument
-    def load(
+    async def load(
         cls,
-        conn: Client,
-        market_address: Pubkey,
-        program_id: Pubkey = instructions.DEFAULT_DEX_PROGRAM_ID,
+        conn: AsyncClient,
+        market_address: PublicKey,
+        program_id: PublicKey = instructions.DEFAULT_DEX_PROGRAM_ID,
         force_use_request_queue: bool = False,
-    ) -> Market:
+    ) -> AsyncMarket:
         """Factory method to create a Market.
 
         :param conn: The connection that we use to load the data, created from `solana.rpc.api`.
         :param market_address: The market address that you want to connect to.
         :param program_id: The program id of the given market, it will use the default value if not provided.
         """
-        market_state = MarketState.load(conn, market_address, program_id)
+        market_state = await MarketState.async_load(conn, market_address, program_id)
         return cls(conn, market_state, force_use_request_queue)
 
-    def find_open_orders_accounts_for_owner(
-        self, owner_address: Pubkey
-    ) -> List[OpenOrdersAccount]:
-        return OpenOrdersAccount.find_for_market_and_owner(
+    async def find_open_orders_accounts_for_owner(self, owner_address: PublicKey) -> List[AsyncOpenOrdersAccount]:
+        return await AsyncOpenOrdersAccount.find_for_market_and_owner(
             self._conn, self.state.public_key(), owner_address, self.state.program_id()
         )
 
-    def load_bids(self) -> OrderBook:
+    async def load_bids(self) -> OrderBook:
         """Load the bid order book"""
-        bytes_data = load_bytes_data(self.state.bids(), self._conn)
+        bytes_data = await load_bytes_data(self.state.bids(), self._conn)
         return self._parse_bids_or_asks(bytes_data)
 
-    def load_asks(self) -> OrderBook:
+    async def load_asks(self) -> OrderBook:
         """Load the ask order book."""
-        bytes_data = load_bytes_data(self.state.asks(), self._conn)
+        bytes_data = await load_bytes_data(self.state.asks(), self._conn)
         return self._parse_bids_or_asks(bytes_data)
 
-    def load_orders_for_owner(self, owner_address: Pubkey) -> List[t.Order]:
+    async def load_orders_for_owner(self, owner_address: PublicKey) -> List[t.Order]:
         """Load orders for owner."""
-        bids = self.load_bids()
-        asks = self.load_asks()
-        open_orders_accounts = self.find_open_orders_accounts_for_owner(owner_address)
+        bids = await self.load_bids()
+        asks = await self.load_asks()
+        open_orders_accounts = await self.find_open_orders_accounts_for_owner(owner_address)
         return self._parse_orders_for_owner(bids, asks, open_orders_accounts)
 
-    def load_event_queue(self) -> List[t.Event]:
+    async def load_event_queue(self) -> List[t.Event]:
         """Load the event queue which includes the fill item and out item. For any trades two fill items are added to
         the event queue. And in case of a trade, cancel or IOC order that missed, out items are added to the event
         queue.
         """
-        bytes_data = load_bytes_data(self.state.event_queue(), self._conn)
+        bytes_data = await load_bytes_data(self.state.event_queue(), self._conn)
         return decode_event_queue(bytes_data)
 
-    def load_request_queue(self) -> List[t.Request]:
-        bytes_data = load_bytes_data(self.state.request_queue(), self._conn)
+    async def load_request_queue(self) -> List[t.Request]:
+        bytes_data = await load_bytes_data(self.state.request_queue(), self._conn)
         return decode_request_queue(bytes_data)
 
-    def load_fills(self, limit=100) -> List[t.FilledOrder]:
-        bytes_data = load_bytes_data(self.state.event_queue(), self._conn)
+    async def load_fills(self, limit=100) -> List[t.FilledOrder]:
+        bytes_data = await load_bytes_data(self.state.event_queue(), self._conn)
         return self._parse_fills(bytes_data, limit)
 
-    def place_order(  # pylint: disable=too-many-arguments,too-many-locals
+    async def place_order(  # pylint: disable=too-many-arguments,too-many-locals
         self,
-        payer: Pubkey,
+        payer: PublicKey,
         owner: Keypair,
         order_type: OrderType,
         side: Side,
         limit_price: float,
         max_quantity: float,
         client_id: int = 0,
         opts: TxOpts = TxOpts(),
     ) -> SendTransactionResp:  # TODO: Add open_orders_address_key param and fee_discount_pubkey
         transaction = Transaction()
         signers: List[Keypair] = [owner]
-        open_order_accounts = self.find_open_orders_accounts_for_owner(owner.pubkey())
+        open_order_accounts = await self.find_open_orders_accounts_for_owner(owner.public_key)
         if open_order_accounts:
             place_order_open_order_account = open_order_accounts[0].address
         else:
-            mbfre_resp = self._conn.get_minimum_balance_for_rent_exemption(
-                OPEN_ORDERS_LAYOUT.sizeof()
-            )
+            mbfre_resp = await self._conn.get_minimum_balance_for_rent_exemption(OPEN_ORDERS_LAYOUT.sizeof())
             place_order_open_order_account = self._after_oo_mbfre_resp(
                 mbfre_resp=mbfre_resp,
                 owner=owner,
                 signers=signers,
                 transaction=transaction,
             )
             # TODO: Cache new_open_orders_account
@@ -136,59 +130,55 @@
             signers=signers,
             limit_price=limit_price,
             max_quantity=max_quantity,
             client_id=client_id,
             open_order_accounts=open_order_accounts,
             place_order_open_order_account=place_order_open_order_account,
         )
-        return self._conn.send_transaction(transaction, *signers, opts=opts)
+        return await self._conn.send_transaction(transaction, *signers, opts=opts)
 
-    def cancel_order_by_client_id(
+    async def cancel_order_by_client_id(
         self,
         owner: Keypair,
-        open_orders_account: Pubkey,
+        open_orders_account: PublicKey,
         client_id: int,
         opts: TxOpts = TxOpts(),
     ) -> SendTransactionResp:
         txs = self._build_cancel_order_by_client_id_tx(
             owner=owner, open_orders_account=open_orders_account, client_id=client_id
         )
-        return self._conn.send_transaction(txs, owner, opts=opts)
+        return await self._conn.send_transaction(txs, owner, opts=opts)
 
-    def cancel_order(
-        self, owner: Keypair, order: t.Order, opts: TxOpts = TxOpts()
-    ) -> SendTransactionResp:
+    async def cancel_order(self, owner: Keypair, order: t.Order, opts: TxOpts = TxOpts()) -> SendTransactionResp:
         txn = self._build_cancel_order_tx(owner=owner, order=order)
-        return self._conn.send_transaction(txn, owner, opts=opts)
+        return await self._conn.send_transaction(txn, owner, opts=opts)
 
-    def match_orders(
-        self, fee_payer: Keypair, limit: int, opts: TxOpts = TxOpts()
-    ) -> SendTransactionResp:
+    async def match_orders(self, fee_payer: Keypair, limit: int, opts: TxOpts = TxOpts()) -> SendTransactionResp:
         txn = self._build_match_orders_tx(limit)
-        return self._conn.send_transaction(txn, fee_payer, opts=opts)
+        return await self._conn.send_transaction(txn, fee_payer, opts=opts)
 
-    def settle_funds(  # pylint: disable=too-many-arguments
+    async def settle_funds(  # pylint: disable=too-many-arguments
         self,
         owner: Keypair,
-        open_orders: OpenOrdersAccount,
-        base_wallet: Pubkey,
-        quote_wallet: Pubkey,  # TODO: add referrer_quote_wallet.
+        open_orders: AsyncOpenOrdersAccount,
+        base_wallet: PublicKey,
+        quote_wallet: PublicKey,  # TODO: add referrer_quote_wallet.
         opts: TxOpts = TxOpts(),
     ) -> SendTransactionResp:
         # TODO: Handle wrapped sol accounts
         should_wrap_sol = self._settle_funds_should_wrap_sol()
-        min_bal_for_rent_exemption = (
-            self._conn.get_minimum_balance_for_rent_exemption(165).value
-            if should_wrap_sol
-            else 0
-        )  # value only matters if should_wrap_sol
+        if should_wrap_sol:
+            mbfre_resp = await self._conn.get_minimum_balance_for_rent_exemption(165)
+            min_bal_for_rent_exemption = mbfre_resp.value
+        else:
+            min_bal_for_rent_exemption = 0  # value only matters if should_wrap_sol
         signers = [owner]
         transaction = self._build_settle_funds_tx(
             owner=owner,
             signers=signers,
             open_orders=open_orders,
             base_wallet=base_wallet,
             quote_wallet=quote_wallet,
             min_bal_for_rent_exemption=min_bal_for_rent_exemption,
             should_wrap_sol=should_wrap_sol,
         )
-        return self._conn.send_transaction(transaction, *signers, opts=opts)
+        return await self._conn.send_transaction(transaction, *signers, opts=opts)
```

### Comparing `pyopenbook-0.7.0a0/pyserum/market/orderbook.py` & `pyopenbook-0.7.1a0/pyserum/market/orderbook.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,21 +12,17 @@
 class OrderBook:
     """Represents an order book."""
 
     _market_state: MarketState
     _is_bids: bool
     _slab: Slab
 
-    def __init__(
-        self, market_state: MarketState, account_flags: t.AccountFlags, slab: Slab
-    ) -> None:
+    def __init__(self, market_state: MarketState, account_flags: t.AccountFlags, slab: Slab) -> None:
         if not account_flags.initialized or not account_flags.bids ^ account_flags.asks:
-            raise Exception(
-                "Invalid order book, either not initialized or neither of bids or asks"
-            )
+            raise Exception("Invalid order book, either not initialized or neither of bids or asks")
         self._market_state = market_state
         self._is_bids = account_flags.bids
         self._slab = slab
 
     @staticmethod
     def __get_price_from_slab(node: Union[SlabInnerNode, SlabLeafNode]) -> int:
         """Get price from a slab node key.
```

### Comparing `pyopenbook-0.7.0a0/pyserum/market/state.py` & `pyopenbook-0.7.1a0/pyserum/market/state.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 from __future__ import annotations
 
 import math
 
 from construct import Container, Struct
-from solders.pubkey import Pubkey
+from solana.publickey import PublicKey
 from solana.rpc.api import Client
 from solana.rpc.async_api import AsyncClient
 
 from pyserum import async_utils, utils
 
 from .._layouts.market import MARKET_LAYOUT
 from .types import AccountFlags
 
 
 class MarketState:  # pylint: disable=too-many-public-methods
     def __init__(
-        self,
-        parsed_market: Container,
-        program_id: Pubkey,
-        base_mint_decimals: int,
-        quote_mint_decimals: int,
+        self, parsed_market: Container, program_id: PublicKey, base_mint_decimals: int, quote_mint_decimals: int
     ) -> None:
         self._decoded = parsed_market
         self._program_id = program_id
         self._base_mint_decimals = base_mint_decimals
         self._quote_mint_decimals = quote_mint_decimals
 
     @staticmethod
@@ -32,107 +28,85 @@
         return MARKET_LAYOUT
 
     @staticmethod
     def _make_parsed_market(bytes_data: bytes) -> Container:
         parsed_market = MARKET_LAYOUT.parse(bytes_data)
         # TODO: add ownAddress check!
 
-        if (
-            not parsed_market.account_flags.initialized
-            or not parsed_market.account_flags.market
-        ):
+        if not parsed_market.account_flags.initialized or not parsed_market.account_flags.market:
             raise Exception("Invalid market")
         return parsed_market
 
     @classmethod
-    def load(
-        cls, conn: Client, market_address: Pubkey, program_id: Pubkey
-    ) -> MarketState:
+    def load(cls, conn: Client, market_address: PublicKey, program_id: PublicKey) -> MarketState:
         bytes_data = utils.load_bytes_data(market_address, conn)
         parsed_market = cls._make_parsed_market(bytes_data)
 
-        base_mint_decimals = utils.get_mint_decimals(
-            conn, Pubkey.from_bytes(parsed_market.base_mint)
-        )
-        quote_mint_decimals = utils.get_mint_decimals(
-            conn, Pubkey.from_bytes(parsed_market.quote_mint)
-        )
+        base_mint_decimals = utils.get_mint_decimals(conn, PublicKey(parsed_market.base_mint))
+        quote_mint_decimals = utils.get_mint_decimals(conn, PublicKey(parsed_market.quote_mint))
         return cls(parsed_market, program_id, base_mint_decimals, quote_mint_decimals)
 
     @classmethod
-    async def async_load(
-        cls, conn: AsyncClient, market_address: Pubkey, program_id: Pubkey
-    ) -> MarketState:
+    async def async_load(cls, conn: AsyncClient, market_address: PublicKey, program_id: PublicKey) -> MarketState:
         bytes_data = await async_utils.load_bytes_data(market_address, conn)
         parsed_market = cls._make_parsed_market(bytes_data)
-        base_mint_decimals = await async_utils.get_mint_decimals(
-            conn, Pubkey.from_bytes(parsed_market.base_mint)
-        )
-        quote_mint_decimals = await async_utils.get_mint_decimals(
-            conn, Pubkey.from_bytes(parsed_market.quote_mint)
-        )
+        base_mint_decimals = await async_utils.get_mint_decimals(conn, PublicKey(parsed_market.base_mint))
+        quote_mint_decimals = await async_utils.get_mint_decimals(conn, PublicKey(parsed_market.quote_mint))
         return cls(parsed_market, program_id, base_mint_decimals, quote_mint_decimals)
 
     @classmethod
     def from_bytes(
-        cls,
-        program_id: Pubkey,
-        base_mint_decimals: int,
-        quote_mint_decimals: int,
-        buffer: bytes,
+        cls, program_id: PublicKey, base_mint_decimals: int, quote_mint_decimals: int, buffer: bytes
     ) -> MarketState:
         parsed_market = MARKET_LAYOUT.parse(buffer)
         # TODO: add ownAddress check!
 
-        if (
-            not parsed_market.account_flags.initialized
-            or not parsed_market.account_flags.market
-        ):
+        if not parsed_market.account_flags.initialized or not parsed_market.account_flags.market:
             raise Exception("Invalid market")
 
         return cls(parsed_market, program_id, base_mint_decimals, quote_mint_decimals)
 
-    def program_id(self) -> Pubkey:
+    def program_id(self) -> PublicKey:
         return self._program_id
 
-    def public_key(self) -> Pubkey:
-        return Pubkey.from_bytes(self._decoded.own_address)
+    def public_key(self) -> PublicKey:
+        return PublicKey(self._decoded.own_address)
 
     def account_flags(self) -> AccountFlags:
         return AccountFlags(**self._decoded.account_flags)
 
-    def asks(self) -> Pubkey:
-        return Pubkey.from_bytes(self._decoded.asks)
+    def asks(self) -> PublicKey:
+        return PublicKey(self._decoded.asks)
 
-    def bids(self) -> Pubkey:
-        return Pubkey.from_bytes(self._decoded.bids)
+    def bids(self) -> PublicKey:
+        return PublicKey(self._decoded.bids)
 
     def fee_rate_bps(self) -> int:
         return self._decoded.fee_rate_bps
 
-    def event_queue(self) -> Pubkey:
-        return Pubkey.from_bytes(self._decoded.event_queue)
+    def event_queue(self) -> PublicKey:
+        return PublicKey(self._decoded.event_queue)
 
-    def request_queue(self) -> Pubkey:
-        return Pubkey.from_bytes(self._decoded.request_queue)
+    def request_queue(self) -> PublicKey:
+        return PublicKey(self._decoded.request_queue)
 
     def vault_signer_nonce(self) -> int:
         return self._decoded.vault_signer_nonce
 
-    def base_mint(self) -> Pubkey:
-        return Pubkey.from_bytes(self._decoded.base_mint)
+    def base_mint(self) -> PublicKey:
+        return PublicKey(self._decoded.base_mint)
 
-    def quote_mint(self) -> Pubkey:
-        return Pubkey.from_bytes(self._decoded.quote_mint)
+    def quote_mint(self) -> PublicKey:
+        return PublicKey(self._decoded.quote_mint)
 
-    def base_vault(self) -> Pubkey:
-        return Pubkey.from_bytes(self._decoded.base_vault)
+    def base_vault(self) -> PublicKey:
+        return PublicKey(self._decoded.base_vault)
 
-    def quote_vault(self) -> Pubkey:
-        return Pubkey.from_bytes(self._decoded.quote_vault)
+    def quote_vault(self) -> PublicKey:
+        return PublicKey(self._decoded.quote_vault)
 
     def base_deposits_total(self) -> int:
         return self._decoded.base_deposits_total
 
     def quote_deposits_total(self) -> int:
         return self._decoded.quote_deposits_total
 
@@ -166,34 +140,30 @@
     def base_lot_size(self) -> int:
         return self._decoded.base_lot_size
 
     def quote_lot_size(self) -> int:
         return self._decoded.quote_lot_size
 
     def price_lots_to_number(self, price: int) -> float:
-        return float(
-            price * self.quote_lot_size() * self.base_spl_token_multiplier()
-        ) / (self.base_lot_size() * self.quote_spl_token_multiplier())
+        return float(price * self.quote_lot_size() * self.base_spl_token_multiplier()) / (
+            self.base_lot_size() * self.quote_spl_token_multiplier()
+        )
 
     def price_number_to_lots(self, price: float) -> int:
         return int(
             round(
                 (price * self.quote_spl_token_multiplier() * self.base_lot_size())
                 / (self.base_spl_token_multiplier() * self.quote_lot_size())
             )
         )
 
     def base_size_lots_to_number(self, size: int) -> float:
         return float(size * self.base_lot_size()) / self.base_spl_token_multiplier()
 
     def base_size_number_to_lots(self, size: float) -> int:
-        return int(
-            math.floor(size * self.base_spl_token_multiplier()) / self.base_lot_size()
-        )
+        return int(math.floor(size * self.base_spl_token_multiplier()) / self.base_lot_size())
 
     def quote_size_lots_to_number(self, size: int) -> float:
         return float(size * self.quote_lot_size()) / self.quote_spl_token_multiplier()
 
     def quote_size_number_to_lots(self, size: float) -> int:
-        return int(
-            math.floor(size * self.quote_spl_token_multiplier()) / self.quote_lot_size()
-        )
+        return int(math.floor(size * self.quote_spl_token_multiplier()) / self.quote_lot_size())
```

### Comparing `pyopenbook-0.7.0a0/pyserum/market/types.py` & `pyopenbook-0.7.1a0/pyserum/market/types.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import NamedTuple
 
-from solders.pubkey import Pubkey
+from solana.publickey import PublicKey
 
 from .._layouts.account_flags import ACCOUNT_FLAGS_LAYOUT
 from ..enums import Side
 
 
 class AccountFlags(NamedTuple):
     initialized: bool = False
@@ -63,15 +63,15 @@
 
 
 class Order(NamedTuple):
     order_id: int
     """"""
     client_id: int
     """"""
-    open_order_address: Pubkey
+    open_order_address: PublicKey
     """"""
     open_order_slot: int
     """"""
     fee_tier: int
     """"""
     info: OrderInfo
     """"""
@@ -96,15 +96,15 @@
     """"""
     max_base_size_or_cancel_id: int
     """"""
     native_quote_quantity_locked: int
     """"""
     order_id: int
     """"""
-    open_orders: Pubkey
+    open_orders: PublicKey
     """"""
     client_order_id: int
     """"""
 
 
 class EventFlags(NamedTuple):
     fill: bool
@@ -124,27 +124,27 @@
     """"""
     native_quantity_paid: int
     """"""
     native_fee_or_rebate: int
     """"""
     order_id: int
     """"""
-    public_key: Pubkey
+    public_key: PublicKey
     """"""
     client_order_id: int
     """"""
 
 
 class MarketInfo(NamedTuple):
     name: str
     """"""
-    address: Pubkey
+    address: PublicKey
     """"""
-    program_id: Pubkey
+    program_id: PublicKey
     """"""
 
 
 class TokenInfo(NamedTuple):
     name: str
     """"""
-    address: Pubkey
+    address: PublicKey
     """"""
```

### Comparing `pyopenbook-0.7.0a0/pyserum/utils.py` & `pyopenbook-0.7.1a0/pyserum/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from solders.pubkey import Pubkey
+from solana.publickey import PublicKey
 from solana.rpc.api import Client
 from solders.account import Account
 from solders.rpc.responses import GetAccountInfoResp
 from spl.token.constants import WRAPPED_SOL_MINT
 
 from pyserum._layouts.market import MINT_LAYOUT
 
 
 def parse_bytes_data(res: GetAccountInfoResp) -> bytes:
     if not isinstance(res.value, Account):
         raise Exception("Cannot load byte data.")
     return res.value.data
 
 
-def load_bytes_data(addr: Pubkey, conn: Client) -> bytes:
+def load_bytes_data(addr: PublicKey, conn: Client) -> bytes:
     res = conn.get_account_info(addr)
     return parse_bytes_data(res)
 
 
 def parse_mint_decimals(bytes_data: bytes) -> int:
     return MINT_LAYOUT.parse(bytes_data).decimals
 
 
-def get_mint_decimals(conn: Client, mint_pub_key: Pubkey) -> int:
+def get_mint_decimals(conn: Client, mint_pub_key: PublicKey) -> int:
     """Get the mint decimals for a token mint"""
     if mint_pub_key == WRAPPED_SOL_MINT:
         return 9
 
     bytes_data = load_bytes_data(mint_pub_key, conn)
     return parse_mint_decimals(bytes_data)
```

### Comparing `pyopenbook-0.7.0a0/setup.py` & `pyopenbook-0.7.1a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """setuptools module for PySerum."""
 
 from setuptools import find_packages, setup
 
 setup(
     name="pyopenbook",
-    version="0.7.0a",
+    version="0.7.1a",
     author="serum-community",
     description="""Python client library for interacting with the Project Serum DEX.""",
     install_requires=[
         "construct>=2.10.56, <3.0.0",
         "construct-typing>=0.5.1, <1.0.0",
         "solana>=0.11.3, <1.0.0",
     ],
```

