# Comparing `tmp/pyopenbook-0.7.2a0.tar.gz` & `tmp/pyopenbook-0.7.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopenbook-0.7.2a0.tar", last modified: Tue Apr 25 04:12:23 2023, max compression
+gzip compressed data, was "pyopenbook-0.7.3a0.tar", last modified: Tue Apr 25 04:46:48 2023, max compression
```

## Comparing `pyopenbook-0.7.2a0.tar` & `pyopenbook-0.7.3a0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 04:12:23.609612 pyopenbook-0.7.2a0/
--rw-r--r--   0 waterquarks   (501) staff       (20)     1072 2023-04-25 03:49:01.000000 pyopenbook-0.7.2a0/LICENSE
--rw-r--r--   0 waterquarks   (501) staff       (20)      563 2023-04-25 04:12:23.609483 pyopenbook-0.7.2a0/PKG-INFO
--rw-r--r--   0 waterquarks   (501) staff       (20)     3329 2023-04-25 03:49:01.000000 pyopenbook-0.7.2a0/README.md
-drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 04:12:23.604707 pyopenbook-0.7.2a0/pyopenbook.egg-info/
--rw-r--r--   0 waterquarks   (501) staff       (20)      563 2023-04-25 04:12:23.000000 pyopenbook-0.7.2a0/pyopenbook.egg-info/PKG-INFO
--rw-r--r--   0 waterquarks   (501) staff       (20)      956 2023-04-25 04:12:23.000000 pyopenbook-0.7.2a0/pyopenbook.egg-info/SOURCES.txt
--rw-r--r--   0 waterquarks   (501) staff       (20)        1 2023-04-25 04:12:23.000000 pyopenbook-0.7.2a0/pyopenbook.egg-info/dependency_links.txt
--rw-r--r--   0 waterquarks   (501) staff       (20)        1 2023-04-25 04:12:23.000000 pyopenbook-0.7.2a0/pyopenbook.egg-info/not-zip-safe
--rw-r--r--   0 waterquarks   (501) staff       (20)       79 2023-04-25 04:12:23.000000 pyopenbook-0.7.2a0/pyopenbook.egg-info/requires.txt
--rw-r--r--   0 waterquarks   (501) staff       (20)        8 2023-04-25 04:12:23.000000 pyopenbook-0.7.2a0/pyopenbook.egg-info/top_level.txt
-drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 04:12:23.606428 pyopenbook-0.7.2a0/pyserum/
--rw-r--r--   0 waterquarks   (501) staff       (20)      121 2022-12-21 03:49:05.000000 pyopenbook-0.7.2a0/pyserum/__init__.py
-drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 04:12:23.607662 pyopenbook-0.7.2a0/pyserum/_layouts/
--rw-r--r--   0 waterquarks   (501) staff       (20)        0 2022-12-21 03:49:05.000000 pyopenbook-0.7.2a0/pyserum/_layouts/__init__.py
--rw-r--r--   0 waterquarks   (501) staff       (20)      486 2022-12-21 03:49:05.000000 pyopenbook-0.7.2a0/pyserum/_layouts/account_flags.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     2727 2022-12-21 03:49:05.000000 pyopenbook-0.7.2a0/pyserum/_layouts/instructions.py
--rw-r--r--   0 waterquarks   (501) staff       (20)      934 2022-12-21 03:49:05.000000 pyopenbook-0.7.2a0/pyserum/_layouts/market.py
--rw-r--r--   0 waterquarks   (501) staff       (20)      601 2022-12-21 03:49:05.000000 pyopenbook-0.7.2a0/pyserum/_layouts/open_orders.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     1526 2023-04-25 03:49:01.000000 pyopenbook-0.7.2a0/pyserum/_layouts/queue.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     1758 2023-04-25 03:49:01.000000 pyopenbook-0.7.2a0/pyserum/_layouts/slab.py
--rw-r--r--   0 waterquarks   (501) staff       (20)      640 2023-04-25 03:49:01.000000 pyopenbook-0.7.2a0/pyserum/async_connection.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     1211 2023-04-25 03:49:01.000000 pyopenbook-0.7.2a0/pyserum/async_open_orders_account.py
--rw-r--r--   0 waterquarks   (501) staff       (20)      641 2023-04-25 03:49:01.000000 pyopenbook-0.7.2a0/pyserum/async_utils.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     1063 2023-04-25 03:49:01.000000 pyopenbook-0.7.2a0/pyserum/connection.py
--rw-r--r--   0 waterquarks   (501) staff       (20)      406 2022-12-21 03:49:05.000000 pyopenbook-0.7.2a0/pyserum/enums.py
--rw-r--r--   0 waterquarks   (501) staff       (20)    27738 2023-04-25 03:49:01.000000 pyopenbook-0.7.2a0/pyserum/instructions.py
-drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 04:12:23.608857 pyopenbook-0.7.2a0/pyserum/market/
--rw-r--r--   0 waterquarks   (501) staff       (20)      194 2022-12-21 03:49:05.000000 pyopenbook-0.7.2a0/pyserum/market/__init__.py
-drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 04:12:23.609282 pyopenbook-0.7.2a0/pyserum/market/_internal/
--rw-r--r--   0 waterquarks   (501) staff       (20)        0 2022-12-21 03:49:05.000000 pyopenbook-0.7.2a0/pyserum/market/_internal/__init__.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     4163 2023-04-25 03:49:01.000000 pyopenbook-0.7.2a0/pyserum/market/_internal/queue.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     5044 2023-04-25 03:49:01.000000 pyopenbook-0.7.2a0/pyserum/market/_internal/slab.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     7672 2023-04-25 03:49:01.000000 pyopenbook-0.7.2a0/pyserum/market/async_market.py
--rw-r--r--   0 waterquarks   (501) staff       (20)    20205 2023-04-25 04:11:39.000000 pyopenbook-0.7.2a0/pyserum/market/core.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     7342 2023-04-25 03:49:01.000000 pyopenbook-0.7.2a0/pyserum/market/market.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     3345 2023-04-25 03:49:01.000000 pyopenbook-0.7.2a0/pyserum/market/orderbook.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     6290 2023-04-25 03:49:01.000000 pyopenbook-0.7.2a0/pyserum/market/state.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     2615 2023-04-25 03:51:31.000000 pyopenbook-0.7.2a0/pyserum/market/types.py
--rw-r--r--   0 waterquarks   (501) staff       (20)     5618 2023-04-25 03:49:01.000000 pyopenbook-0.7.2a0/pyserum/open_orders_account.py
--rw-r--r--   0 waterquarks   (501) staff       (20)        0 2022-12-21 03:49:06.000000 pyopenbook-0.7.2a0/pyserum/py.typed
--rw-r--r--   0 waterquarks   (501) staff       (20)      949 2023-04-25 03:49:01.000000 pyopenbook-0.7.2a0/pyserum/utils.py
--rw-r--r--   0 waterquarks   (501) staff       (20)       38 2023-04-25 04:12:23.609652 pyopenbook-0.7.2a0/setup.cfg
--rw-r--r--   0 waterquarks   (501) staff       (20)      961 2023-04-25 04:11:57.000000 pyopenbook-0.7.2a0/setup.py
+drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 04:46:48.358046 pyopenbook-0.7.3a0/
+-rw-r--r--   0 waterquarks   (501) staff       (20)     1072 2023-04-25 03:49:01.000000 pyopenbook-0.7.3a0/LICENSE
+-rw-r--r--   0 waterquarks   (501) staff       (20)      563 2023-04-25 04:46:48.357911 pyopenbook-0.7.3a0/PKG-INFO
+-rw-r--r--   0 waterquarks   (501) staff       (20)     3329 2023-04-25 03:49:01.000000 pyopenbook-0.7.3a0/README.md
+drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 04:46:48.352917 pyopenbook-0.7.3a0/pyopenbook.egg-info/
+-rw-r--r--   0 waterquarks   (501) staff       (20)      563 2023-04-25 04:46:48.000000 pyopenbook-0.7.3a0/pyopenbook.egg-info/PKG-INFO
+-rw-r--r--   0 waterquarks   (501) staff       (20)      956 2023-04-25 04:46:48.000000 pyopenbook-0.7.3a0/pyopenbook.egg-info/SOURCES.txt
+-rw-r--r--   0 waterquarks   (501) staff       (20)        1 2023-04-25 04:46:48.000000 pyopenbook-0.7.3a0/pyopenbook.egg-info/dependency_links.txt
+-rw-r--r--   0 waterquarks   (501) staff       (20)        1 2023-04-25 04:46:48.000000 pyopenbook-0.7.3a0/pyopenbook.egg-info/not-zip-safe
+-rw-r--r--   0 waterquarks   (501) staff       (20)       79 2023-04-25 04:46:48.000000 pyopenbook-0.7.3a0/pyopenbook.egg-info/requires.txt
+-rw-r--r--   0 waterquarks   (501) staff       (20)        8 2023-04-25 04:46:48.000000 pyopenbook-0.7.3a0/pyopenbook.egg-info/top_level.txt
+drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 04:46:48.354838 pyopenbook-0.7.3a0/pyserum/
+-rw-r--r--   0 waterquarks   (501) staff       (20)      121 2022-12-21 03:49:05.000000 pyopenbook-0.7.3a0/pyserum/__init__.py
+drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 04:46:48.355960 pyopenbook-0.7.3a0/pyserum/_layouts/
+-rw-r--r--   0 waterquarks   (501) staff       (20)        0 2022-12-21 03:49:05.000000 pyopenbook-0.7.3a0/pyserum/_layouts/__init__.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)      486 2022-12-21 03:49:05.000000 pyopenbook-0.7.3a0/pyserum/_layouts/account_flags.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     2727 2022-12-21 03:49:05.000000 pyopenbook-0.7.3a0/pyserum/_layouts/instructions.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)      934 2022-12-21 03:49:05.000000 pyopenbook-0.7.3a0/pyserum/_layouts/market.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)      601 2022-12-21 03:49:05.000000 pyopenbook-0.7.3a0/pyserum/_layouts/open_orders.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     1526 2023-04-25 03:49:01.000000 pyopenbook-0.7.3a0/pyserum/_layouts/queue.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     1758 2023-04-25 03:49:01.000000 pyopenbook-0.7.3a0/pyserum/_layouts/slab.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)      640 2023-04-25 03:49:01.000000 pyopenbook-0.7.3a0/pyserum/async_connection.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     1211 2023-04-25 03:49:01.000000 pyopenbook-0.7.3a0/pyserum/async_open_orders_account.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)      641 2023-04-25 03:49:01.000000 pyopenbook-0.7.3a0/pyserum/async_utils.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     1063 2023-04-25 03:49:01.000000 pyopenbook-0.7.3a0/pyserum/connection.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)      406 2022-12-21 03:49:05.000000 pyopenbook-0.7.3a0/pyserum/enums.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)    27738 2023-04-25 03:49:01.000000 pyopenbook-0.7.3a0/pyserum/instructions.py
+drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 04:46:48.357213 pyopenbook-0.7.3a0/pyserum/market/
+-rw-r--r--   0 waterquarks   (501) staff       (20)      194 2022-12-21 03:49:05.000000 pyopenbook-0.7.3a0/pyserum/market/__init__.py
+drwxr-xr-x   0 waterquarks   (501) staff       (20)        0 2023-04-25 04:46:48.357712 pyopenbook-0.7.3a0/pyserum/market/_internal/
+-rw-r--r--   0 waterquarks   (501) staff       (20)        0 2022-12-21 03:49:05.000000 pyopenbook-0.7.3a0/pyserum/market/_internal/__init__.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     4163 2023-04-25 04:39:48.000000 pyopenbook-0.7.3a0/pyserum/market/_internal/queue.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     5044 2023-04-25 03:49:01.000000 pyopenbook-0.7.3a0/pyserum/market/_internal/slab.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     7672 2023-04-25 03:49:01.000000 pyopenbook-0.7.3a0/pyserum/market/async_market.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)    20308 2023-04-25 04:46:21.000000 pyopenbook-0.7.3a0/pyserum/market/core.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     7342 2023-04-25 03:49:01.000000 pyopenbook-0.7.3a0/pyserum/market/market.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     3345 2023-04-25 03:49:01.000000 pyopenbook-0.7.3a0/pyserum/market/orderbook.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     6290 2023-04-25 03:49:01.000000 pyopenbook-0.7.3a0/pyserum/market/state.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     2596 2023-04-25 04:46:21.000000 pyopenbook-0.7.3a0/pyserum/market/types.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)     5618 2023-04-25 03:49:01.000000 pyopenbook-0.7.3a0/pyserum/open_orders_account.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)        0 2022-12-21 03:49:06.000000 pyopenbook-0.7.3a0/pyserum/py.typed
+-rw-r--r--   0 waterquarks   (501) staff       (20)      949 2023-04-25 03:49:01.000000 pyopenbook-0.7.3a0/pyserum/utils.py
+-rw-r--r--   0 waterquarks   (501) staff       (20)       38 2023-04-25 04:46:48.358085 pyopenbook-0.7.3a0/setup.cfg
+-rw-r--r--   0 waterquarks   (501) staff       (20)      961 2023-04-25 04:46:44.000000 pyopenbook-0.7.3a0/setup.py
```

### Comparing `pyopenbook-0.7.2a0/LICENSE` & `pyopenbook-0.7.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/PKG-INFO` & `pyopenbook-0.7.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopenbook
-Version: 0.7.2a0
+Version: 0.7.3a0
 Summary: Python client library for interacting with the Project Serum DEX.
 Home-page: https://github.com/blockworks-foundation/pyopenbook
 Author: serum-community
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyopenbook-0.7.2a0/README.md` & `pyopenbook-0.7.3a0/README.md`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/pyopenbook.egg-info/PKG-INFO` & `pyopenbook-0.7.3a0/pyopenbook.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopenbook
-Version: 0.7.2a0
+Version: 0.7.3a0
 Summary: Python client library for interacting with the Project Serum DEX.
 Home-page: https://github.com/blockworks-foundation/pyopenbook
 Author: serum-community
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyopenbook-0.7.2a0/pyopenbook.egg-info/SOURCES.txt` & `pyopenbook-0.7.3a0/pyopenbook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/pyserum/_layouts/instructions.py` & `pyopenbook-0.7.3a0/pyserum/_layouts/instructions.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/pyserum/_layouts/market.py` & `pyopenbook-0.7.3a0/pyserum/_layouts/market.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/pyserum/_layouts/open_orders.py` & `pyopenbook-0.7.3a0/pyserum/_layouts/open_orders.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/pyserum/_layouts/queue.py` & `pyopenbook-0.7.3a0/pyserum/_layouts/queue.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/pyserum/_layouts/slab.py` & `pyopenbook-0.7.3a0/pyserum/_layouts/slab.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/pyserum/async_connection.py` & `pyopenbook-0.7.3a0/pyserum/async_connection.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/pyserum/async_open_orders_account.py` & `pyopenbook-0.7.3a0/pyserum/async_open_orders_account.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/pyserum/async_utils.py` & `pyopenbook-0.7.3a0/pyserum/async_utils.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/pyserum/connection.py` & `pyopenbook-0.7.3a0/pyserum/connection.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/pyserum/instructions.py` & `pyopenbook-0.7.3a0/pyserum/instructions.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/pyserum/market/_internal/queue.py` & `pyopenbook-0.7.3a0/pyserum/market/_internal/queue.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/pyserum/market/_internal/slab.py` & `pyopenbook-0.7.3a0/pyserum/market/_internal/slab.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/pyserum/market/async_market.py` & `pyopenbook-0.7.3a0/pyserum/market/async_market.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/pyserum/market/core.py` & `pyopenbook-0.7.3a0/pyserum/market/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,19 +112,21 @@
                 else event.native_quantity_released + event.native_fee_or_rebate
             )
 
             price = (price_before_fees * self.state.base_spl_token_multiplier()) / (self.state.quote_spl_token_multiplier() * event.native_quantity_paid)
 
             size = event.native_quantity_paid / self.state.base_spl_token_multiplier()
         return t.FilledOrder(
-            client_order_id=event.order_id,
             side=side,
+            type='maker' if event.event_flags.maker else 'taker',
             price=price,
             size=size,
-            fee_cost=self.state.quote_spl_size_to_number(event.native_fee_or_rebate) * (-1 if event.event_flags.maker else 1),
+            fee=self.state.quote_spl_size_to_number(event.native_fee_or_rebate) * (-1 if event.event_flags.maker else 1),
+            open_orders=event.public_key,
+            client_order_id=event.order_id,
         )
 
     def _prepare_new_oo_account(
         self,
         owner: Keypair,
         balance_needed: int,
         signers: List[Keypair],
```

### Comparing `pyopenbook-0.7.2a0/pyserum/market/market.py` & `pyopenbook-0.7.3a0/pyserum/market/market.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/pyserum/market/orderbook.py` & `pyopenbook-0.7.3a0/pyserum/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/pyserum/market/state.py` & `pyopenbook-0.7.3a0/pyserum/market/state.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/pyserum/market/types.py` & `pyopenbook-0.7.3a0/pyserum/market/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,24 +35,21 @@
             event_queue=con.event_queue,
             bids=con.bids,
             asks=con.asks,
         )
 
 
 class FilledOrder(NamedTuple):
-    client_order_id: int
-    """"""
     side: str
-    """"""
+    type: str
     price: float
-    """"""
     size: float
-    """"""
-    fee_cost: float
-    """"""
+    fee: float
+    open_orders: PublicKey
+    client_order_id: int
 
 
 class OrderInfo(NamedTuple):
     price: float
     """"""
     size: float
     """"""
```

### Comparing `pyopenbook-0.7.2a0/pyserum/open_orders_account.py` & `pyopenbook-0.7.3a0/pyserum/open_orders_account.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/pyserum/utils.py` & `pyopenbook-0.7.3a0/pyserum/utils.py`

 * *Files identical despite different names*

### Comparing `pyopenbook-0.7.2a0/setup.py` & `pyopenbook-0.7.3a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """setuptools module for PySerum."""
 
 from setuptools import find_packages, setup
 
 setup(
     name="pyopenbook",
-    version="0.7.2a",
+    version="0.7.3a",
     author="serum-community",
     description="""Python client library for interacting with the Project Serum DEX.""",
     install_requires=[
         "construct>=2.10.56, <3.0.0",
         "construct-typing>=0.5.1, <1.0.0",
         "solana>=0.11.3, <1.0.0",
     ],
```

