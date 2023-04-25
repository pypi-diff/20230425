# Comparing `tmp/pytonconnect-0.0.2.tar.gz` & `tmp/pytonconnect-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytonconnect-0.0.2.tar", last modified: Wed Apr 19 18:00:48 2023, max compression
+gzip compressed data, was "pytonconnect-0.1.0.tar", last modified: Tue Apr 25 09:30:06 2023, max compression
```

## Comparing `pytonconnect-0.0.2.tar` & `pytonconnect-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 18:00:48.892852 pytonconnect-0.0.2/
--rw-rw-rw-   0        0        0    11558 2023-04-04 12:05:05.000000 pytonconnect-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4689 2023-04-19 18:00:48.892852 pytonconnect-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3744 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 18:00:48.862851 pytonconnect-0.0.2/pytonconnect/
--rw-rw-rw-   0        0        0       49 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:00:48.882852 pytonconnect-0.0.2/pytonconnect/crypto/
--rw-rw-rw-   0        0        0       43 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/crypto/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/crypto/session_crypto.py
--rw-rw-rw-   0        0        0     1414 2023-04-19 17:56:13.000000 pytonconnect-0.0.2/pytonconnect/exceptions.py
--rw-rw-rw-   0        0        0       96 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:00:48.885853 pytonconnect-0.0.2/pytonconnect/parsers/
--rw-rw-rw-   0        0        0       53 2023-04-19 17:56:13.000000 pytonconnect-0.0.2/pytonconnect/parsers/__init__.py
--rw-rw-rw-   0        0        0      521 2023-04-19 17:56:13.000000 pytonconnect-0.0.2/pytonconnect/parsers/rpc_parser.py
--rw-rw-rw-   0        0        0     1493 2023-04-19 17:56:13.000000 pytonconnect-0.0.2/pytonconnect/parsers/send_transaction.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:00:48.888851 pytonconnect-0.0.2/pytonconnect/provider/
--rw-rw-rw-   0        0        0       88 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/provider/__init__.py
--rw-rw-rw-   0        0        0     4451 2023-04-19 17:58:30.000000 pytonconnect-0.0.2/pytonconnect/provider/bridge_gateway.py
--rw-rw-rw-   0        0        0     8592 2023-04-19 17:56:12.000000 pytonconnect-0.0.2/pytonconnect/provider/bridge_provider.py
--rw-rw-rw-   0        0        0      876 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/provider/bridge_session.py
--rw-rw-rw-   0        0        0      613 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/provider/provider.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:00:48.890850 pytonconnect-0.0.2/pytonconnect/storage/
--rw-rw-rw-   0        0        0       78 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/storage/__init__.py
--rw-rw-rw-   0        0        0      523 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/storage/default_storage.py
--rw-rw-rw-   0        0        0     1009 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/storage/interface.py
--rw-rw-rw-   0        0        0     9927 2023-04-19 17:58:30.000000 pytonconnect-0.0.2/pytonconnect/ton_connect.py
--rw-rw-rw-   0        0        0     4737 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/pytonconnect/wallets_list_manager.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:00:48.881849 pytonconnect-0.0.2/pytonconnect.egg-info/
--rw-rw-rw-   0        0        0     4689 2023-04-19 18:00:48.000000 pytonconnect-0.0.2/pytonconnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      865 2023-04-19 18:00:48.000000 pytonconnect-0.0.2/pytonconnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 18:00:48.000000 pytonconnect-0.0.2/pytonconnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-11 12:27:07.000000 pytonconnect-0.0.2/pytonconnect.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       57 2023-04-19 18:00:48.000000 pytonconnect-0.0.2/pytonconnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-19 18:00:48.000000 pytonconnect-0.0.2/pytonconnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1160 2023-04-19 18:00:48.897850 pytonconnect-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-04-19 17:53:09.000000 pytonconnect-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:30:06.018261 pytonconnect-0.1.0/
+-rw-rw-rw-   0        0        0    11558 2023-04-04 12:05:05.000000 pytonconnect-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4688 2023-04-25 09:30:06.018261 pytonconnect-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3744 2023-04-19 17:53:09.000000 pytonconnect-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 09:30:05.968652 pytonconnect-0.1.0/pytonconnect/
+-rw-rw-rw-   0        0        0      181 2023-04-25 09:15:01.000000 pytonconnect-0.1.0/pytonconnect/__init__.py
+-rw-rw-rw-   0        0        0     9176 2023-04-25 09:29:28.000000 pytonconnect-0.1.0/pytonconnect/_ton_connect.py
+-rw-rw-rw-   0        0        0     4737 2023-04-25 09:14:58.000000 pytonconnect-0.1.0/pytonconnect/_wallets_list_manager.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:30:05.998242 pytonconnect-0.1.0/pytonconnect/crypto/
+-rw-rw-rw-   0        0        0       84 2023-04-25 08:52:45.000000 pytonconnect-0.1.0/pytonconnect/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-04-19 17:53:09.000000 pytonconnect-0.1.0/pytonconnect/crypto/_session_crypto.py
+-rw-rw-rw-   0        0        0     1928 2023-04-24 21:57:27.000000 pytonconnect-0.1.0/pytonconnect/exceptions.py
+-rw-rw-rw-   0        0        0       96 2023-04-19 17:53:09.000000 pytonconnect-0.1.0/pytonconnect/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:30:06.003239 pytonconnect-0.1.0/pytonconnect/parsers/
+-rw-rw-rw-   0        0        0      293 2023-04-25 08:56:29.000000 pytonconnect-0.1.0/pytonconnect/parsers/__init__.py
+-rw-rw-rw-   0        0        0     6304 2023-04-25 07:36:03.000000 pytonconnect-0.1.0/pytonconnect/parsers/_connect_event.py
+-rw-rw-rw-   0        0        0      521 2023-04-19 17:56:13.000000 pytonconnect-0.1.0/pytonconnect/parsers/_rpc_parser.py
+-rw-rw-rw-   0        0        0     1491 2023-04-25 08:54:29.000000 pytonconnect-0.1.0/pytonconnect/parsers/_send_transaction.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:30:06.011242 pytonconnect-0.1.0/pytonconnect/provider/
+-rw-rw-rw-   0        0        0      153 2023-04-25 08:59:01.000000 pytonconnect-0.1.0/pytonconnect/provider/__init__.py
+-rw-rw-rw-   0        0        0     4451 2023-04-25 09:29:28.000000 pytonconnect-0.1.0/pytonconnect/provider/_bridge_gateway.py
+-rw-rw-rw-   0        0        0     8595 2023-04-25 08:59:03.000000 pytonconnect-0.1.0/pytonconnect/provider/_bridge_provider.py
+-rw-rw-rw-   0        0        0      876 2023-04-19 17:53:09.000000 pytonconnect-0.1.0/pytonconnect/provider/_bridge_session.py
+-rw-rw-rw-   0        0        0      613 2023-04-19 17:53:09.000000 pytonconnect-0.1.0/pytonconnect/provider/_provider.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:30:06.015240 pytonconnect-0.1.0/pytonconnect/storage/
+-rw-rw-rw-   0        0        0      138 2023-04-25 09:00:29.000000 pytonconnect-0.1.0/pytonconnect/storage/__init__.py
+-rw-rw-rw-   0        0        0      524 2023-04-25 09:00:27.000000 pytonconnect-0.1.0/pytonconnect/storage/_default_storage.py
+-rw-rw-rw-   0        0        0     1009 2023-04-19 17:53:09.000000 pytonconnect-0.1.0/pytonconnect/storage/_interface.py
+drwxrwxrwx   0        0        0        0 2023-04-25 09:30:05.995240 pytonconnect-0.1.0/pytonconnect.egg-info/
+-rw-rw-rw-   0        0        0     4688 2023-04-25 09:30:05.000000 pytonconnect-0.1.0/pytonconnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      915 2023-04-25 09:30:05.000000 pytonconnect-0.1.0/pytonconnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 09:30:05.000000 pytonconnect-0.1.0/pytonconnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-11 12:27:07.000000 pytonconnect-0.1.0/pytonconnect.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       57 2023-04-25 09:30:05.000000 pytonconnect-0.1.0/pytonconnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-25 09:30:05.000000 pytonconnect-0.1.0/pytonconnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1159 2023-04-25 09:30:06.023563 pytonconnect-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-04-19 17:53:09.000000 pytonconnect-0.1.0/setup.py
```

### Comparing `pytonconnect-0.0.2/LICENSE` & `pytonconnect-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.0.2/PKG-INFO` & `pytonconnect-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pytonconnect
-Version: 0.0.2
+Version: 0.1.0
 Summary: Python SDK for TON Connect 2.0
 Author: XaBbl4
 Author-email: xabbl4@gmail.com
 License: Apache 2.0
 Project-URL: Github, https://github.com/XaBbl4/pytonconnect
 Keywords: TON,TON Connect,TON Connect SDK
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pytonconnect-0.0.2/README.md` & `pytonconnect-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.0.2/pytonconnect/crypto/session_crypto.py` & `pytonconnect-0.1.0/pytonconnect/crypto/_session_crypto.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.0.2/pytonconnect/parsers/rpc_parser.py` & `pytonconnect-0.1.0/pytonconnect/parsers/_rpc_parser.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.0.2/pytonconnect/parsers/send_transaction.py` & `pytonconnect-0.1.0/pytonconnect/parsers/_send_transaction.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 
 from enum import IntEnum
 
 from pytonconnect.exceptions import TonConnectError, UnknownError, BadRequestError, UnknownAppError, UserRejectsError
-from .rpc_parser import RpcParser
+from ._rpc_parser import RpcParser
 
 
 class SEND_TRANSACTION_ERROR_CODES(IntEnum):
     UNKNOWN_ERROR = 0
     BAD_REQUEST_ERROR = 1
     UNKNOWN_APP_ERROR = 100
     USER_REJECTS_ERROR = 300
@@ -34,15 +34,15 @@
     def convert_from_rpc_response(rpc_response: dict) -> dict:
         return {
             'boc': rpc_response['result']
         }
 
 
     def parse_and_throw_error(response: dict) -> None:
-        error_constructor: TonConnectError = TonConnectError
+        error_constructor: TonConnectError = UnknownError
 
         code = response.get('error', {}).get('code', None)
         if code is not None and code in SEND_TRANSACTION_ERRORS:
             error_constructor = SEND_TRANSACTION_ERRORS[code]
         
         message = response.get('error', {}).get('message', None)
         raise error_constructor(message)
```

### Comparing `pytonconnect-0.0.2/pytonconnect/provider/bridge_gateway.py` & `pytonconnect-0.1.0/pytonconnect/provider/_bridge_gateway.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.0.2/pytonconnect/provider/bridge_provider.py` & `pytonconnect-0.1.0/pytonconnect/provider/_bridge_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from urllib.parse import quote_plus
 
 from pytonconnect.crypto import SessionCrypto
 from pytonconnect.exceptions import TonConnectError
 from pytonconnect.logger import _LOGGER
 from pytonconnect.storage import IStorage
 
-from .provider import BaseProvider
-from .bridge_gateway import BridgeGateway
-from .bridge_session import BridgeSession
+from ._provider import BaseProvider
+from ._bridge_gateway import BridgeGateway
+from ._bridge_session import BridgeSession
 
 
 class BridgeProvider(BaseProvider):
 
     DISCONNECT_TIMEOUT = 600
     STANDART_UNIVERSAL_URL = 'tc://'
```

### Comparing `pytonconnect-0.0.2/pytonconnect/provider/bridge_session.py` & `pytonconnect-0.1.0/pytonconnect/provider/_bridge_session.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.0.2/pytonconnect/provider/provider.py` & `pytonconnect-0.1.0/pytonconnect/provider/_provider.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.0.2/pytonconnect/storage/default_storage.py` & `pytonconnect-0.1.0/pytonconnect/storage/_default_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .interface import IStorage
+from ._interface import IStorage
 
 
 class DefaultStorage(IStorage):
 
     _cache: dict
 
     def __init__(self):
```

### Comparing `pytonconnect-0.0.2/pytonconnect/storage/interface.py` & `pytonconnect-0.1.0/pytonconnect/storage/_interface.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.0.2/pytonconnect/ton_connect.py` & `pytonconnect-0.1.0/pytonconnect/_ton_connect.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from pytonconnect.exceptions import TonConnectError, WalletAlreadyConnectedError, WalletNotConnectedError, WalletNotSupportFeatureError
-from pytonconnect.parsers import SendTransactionParser
-from pytonconnect.storage import IStorage, DefaultStorage
-from pytonconnect.wallets_list_manager import WalletsListManager
-from pytonconnect.provider import BridgeProvider
+from pytonconnect import WalletsListManager
+from pytonconnect.exceptions import ManifestContentError, ManifestNotFoundError, WalletAlreadyConnectedError, WalletNotConnectedError, WalletNotSupportFeatureError
 from pytonconnect.logger import _LOGGER
+from pytonconnect.parsers import SendTransactionParser, ConnectEventParser, WalletInfo
+from pytonconnect.provider import BridgeProvider
+from pytonconnect.storage import IStorage, DefaultStorage
 
 
 class TonConnect:
 
     _wallets_list = WalletsListManager()
 
     _provider: BridgeProvider
     _manifest_url: str
     _storage: IStorage
 
-    _wallet: dict
+    _wallet: WalletInfo
 
     _status_change_subscriptions: list
     _status_change_error_subscriptions: list
 
     @property
     def connected(self):
         """Shows if the wallet is connected right now."""
         return self._wallet is not None
 
     @property
     def account(self):
         """Current connected account or None if no account is connected."""
-        return self._wallet.get('account', None) if self.connected else None
+        return self._wallet.account if self.connected else None
 
     @property
     def wallet(self):
         """Current connected wallet or None if no account is connected."""
         return self._wallet
 
 
@@ -104,32 +104,31 @@
         if not self._provider:
             return False
 
         self._provider.listen(self._wallet_events_listener)
         return await self._provider.restore_connection()
 
 
-    async def send_transaction(self, transaction):
+    async def send_transaction(self, transaction: dict):
         """Asks connected wallet to sign and send the transaction.
         
         :param transaction: transaction to send.
         :return: signed transaction boc that allows you to find the transaction in the blockchain.
         If user rejects transaction, method will throw the corresponding error.
         """
         if not self.connected:
             raise WalletNotConnectedError()
 
-        features = self._wallet['device']['features']
         options = {'required_messages_number': len(transaction.get('messages', []))}
-        self._check_send_transaction_support(features, options)
+        self._check_send_transaction_support(self._wallet.device.features, options)
 
         request = {
             'valid_until': transaction.get('valid_until', None),
-            'from': transaction.get('from', self._wallet['account']['address']),
-            'network': transaction.get('network', self._wallet['account']['chain']),
+            'from': transaction.get('from', self._wallet.account.address),
+            'network': transaction.get('network', self._wallet.account.chain),
             'messages': transaction.get('messages', [])
         }
 
         response = await self._provider.send_request(SendTransactionParser.convert_to_rpc_request(request))
 
         if SendTransactionParser.is_error(response):
             return SendTransactionParser.parse_and_throw_error(response)
@@ -190,54 +189,28 @@
             self._on_wallet_connect_error(data['payload'])
 
         elif data['event'] == 'disconnect':
             self._on_wallet_disconnected()
 
 
     def _on_wallet_connected(self, payload):
-        if 'items' not in payload:
-            raise TonConnectError('items was not found in payload')
-
-        ton_addr = None
-        ton_proof = None
-        for item in payload['items']:
-            if 'name' in item:
-                if item['name'] == 'ton_addr':
-                    ton_addr = item
-                elif item['name'] == 'ton_proof':
-                    ton_proof = item
-
-        if not ton_addr:
-            raise TonConnectError('ton_addr connection item was not found')
-
-        wallet = {
-            'device': payload['device'],
-            'account': {
-                'address': ton_addr['address'],
-                'chain': ton_addr['network'],
-                'wallet_state_init': ton_addr['walletStateInit'],
-                'public_key': ton_addr.get('publicKey', None)
-            }
-        }
-
-        if ton_proof is not None:
-            wallet['connect_items'] = {
-                'ton_proof': ton_proof
-            }
-
-        self._wallet = wallet
+        self._wallet = ConnectEventParser.parse_response(payload)
         for listener in self._status_change_subscriptions:
             listener(self._wallet)
 
 
     def _on_wallet_connect_error(self, payload):
         _LOGGER.debug('connect error %s', payload)
+        error = ConnectEventParser.parse_error(payload)
         for listener in self._status_change_error_subscriptions:
-            listener(payload)
-        # TODO: add check of errors
+            listener(error)
+        
+        if isinstance(error, ManifestNotFoundError) or isinstance(error, ManifestContentError):
+            _LOGGER.exception(error)
+            raise error
 
 
     def _on_wallet_disconnected(self):
         self._wallet = None
         for listener in self._status_change_subscriptions:
             listener(None)
 
@@ -245,17 +218,17 @@
     def _create_connect_request(self, request):
         items = [
             {
                 'name': 'ton_addr'
             }
         ]
 
-        if request and 'ton_proof' in request:
+        if isinstance(request, dict) and 'ton_proof' in request:
             items.append({
                 'name': 'ton_proof',
-                'payload': request['tonProof']
+                'payload': request['ton_proof']
             })
 
         return {
             'manifestUrl': self._manifest_url,
             'items': items
         }
```

### Comparing `pytonconnect-0.0.2/pytonconnect/wallets_list_manager.py` & `pytonconnect-0.1.0/pytonconnect/_wallets_list_manager.py`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.0.2/pytonconnect.egg-info/PKG-INFO` & `pytonconnect-0.1.0/pytonconnect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pytonconnect
-Version: 0.0.2
+Version: 0.1.0
 Summary: Python SDK for TON Connect 2.0
 Author: XaBbl4
 Author-email: xabbl4@gmail.com
 License: Apache 2.0
 Project-URL: Github, https://github.com/XaBbl4/pytonconnect
 Keywords: TON,TON Connect,TON Connect SDK
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pytonconnect-0.0.2/pytonconnect.egg-info/SOURCES.txt` & `pytonconnect-0.1.0/pytonconnect.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 pytonconnect/__init__.py
+pytonconnect/_ton_connect.py
+pytonconnect/_wallets_list_manager.py
 pytonconnect/exceptions.py
 pytonconnect/logger.py
-pytonconnect/ton_connect.py
-pytonconnect/wallets_list_manager.py
 pytonconnect.egg-info/PKG-INFO
 pytonconnect.egg-info/SOURCES.txt
 pytonconnect.egg-info/dependency_links.txt
 pytonconnect.egg-info/not-zip-safe
 pytonconnect.egg-info/requires.txt
 pytonconnect.egg-info/top_level.txt
 pytonconnect/crypto/__init__.py
-pytonconnect/crypto/session_crypto.py
+pytonconnect/crypto/_session_crypto.py
 pytonconnect/parsers/__init__.py
-pytonconnect/parsers/rpc_parser.py
-pytonconnect/parsers/send_transaction.py
+pytonconnect/parsers/_connect_event.py
+pytonconnect/parsers/_rpc_parser.py
+pytonconnect/parsers/_send_transaction.py
 pytonconnect/provider/__init__.py
-pytonconnect/provider/bridge_gateway.py
-pytonconnect/provider/bridge_provider.py
-pytonconnect/provider/bridge_session.py
-pytonconnect/provider/provider.py
+pytonconnect/provider/_bridge_gateway.py
+pytonconnect/provider/_bridge_provider.py
+pytonconnect/provider/_bridge_session.py
+pytonconnect/provider/_provider.py
 pytonconnect/storage/__init__.py
-pytonconnect/storage/default_storage.py
-pytonconnect/storage/interface.py
+pytonconnect/storage/_default_storage.py
+pytonconnect/storage/_interface.py
```

### Comparing `pytonconnect-0.0.2/setup.cfg` & `pytonconnect-0.1.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7974 6f6e 636f 6e6e 6563 740d   = pytonconnect.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e32  .version = 0.0.2
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e30  .version = 0.1.0
 00000030: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000040: 5079 7468 6f6e 2053 444b 2066 6f72 2054  Python SDK for T
 00000050: 4f4e 2043 6f6e 6e65 6374 2032 2e30 0d0a  ON Connect 2.0..
 00000060: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000070: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
 00000080: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
 00000090: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
 000000a0: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
 000000b0: 6e0d 0a6b 6579 776f 7264 7320 3d20 544f  n..keywords = TO
 000000c0: 4e2c 2054 4f4e 2043 6f6e 6e65 6374 2c20  N, TON Connect, 
 000000d0: 544f 4e20 436f 6e6e 6563 7420 5344 4b0d  TON Connect SDK.
 000000e0: 0a6c 6963 656e 7365 203d 2041 7061 6368  .license = Apach
 000000f0: 6520 322e 300d 0a63 6c61 7373 6966 6965  e 2.0..classifie
 00000100: 7273 203d 200d 0a09 4465 7665 6c6f 706d  rs = ...Developm
-00000110: 656e 7420 5374 6174 7573 203a 3a20 3320  ent Status :: 3 
-00000120: 2d20 416c 7068 610d 0a09 496e 7465 6e64  - Alpha...Intend
-00000130: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
-00000140: 6576 656c 6f70 6572 730d 0a09 4c69 6365  evelopers...Lice
-00000150: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-00000160: 7665 6420 3a3a 2041 7061 6368 6520 536f  ved :: Apache So
-00000170: 6674 7761 7265 204c 6963 656e 7365 0d0a  ftware License..
-00000180: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
-00000190: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-000001a0: 656e 740d 0a09 5072 6f67 7261 6d6d 696e  ent...Programmin
-000001b0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000001c0: 7468 6f6e 203a 3a20 330d 0a09 5072 6f67  thon :: 3...Prog
-000001d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000001e0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-000001f0: 370d 0a09 5072 6f67 7261 6d6d 696e 6720  7...Programming 
-00000200: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000210: 6f6e 203a 3a20 332e 380d 0a09 5072 6f67  on :: 3.8...Prog
-00000220: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000230: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000240: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
-00000250: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000260: 6f6e 203a 3a20 332e 3130 0d0a 0950 726f  on :: 3.10...Pro
-00000270: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000280: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000290: 2e31 310d 0a09 546f 7069 6320 3a3a 2053  .11...Topic :: S
-000002a0: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
-000002b0: 656e 7420 3a3a 204c 6962 7261 7269 6573  ent :: Libraries
-000002c0: 203a 3a20 5079 7468 6f6e 204d 6f64 756c   :: Python Modul
-000002d0: 6573 0d0a 6175 7468 6f72 203d 2058 6142  es..author = XaB
-000002e0: 626c 340d 0a61 7574 686f 725f 656d 6169  bl4..author_emai
-000002f0: 6c20 3d20 7861 6262 6c34 4067 6d61 696c  l = xabbl4@gmail
-00000300: 2e63 6f6d 0d0a 7072 6f6a 6563 745f 7572  .com..project_ur
-00000310: 6c73 203d 200d 0a09 4769 7468 7562 203d  ls = ...Github =
-00000320: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000330: 636f 6d2f 5861 4262 6c34 2f70 7974 6f6e  com/XaBbl4/pyton
-00000340: 636f 6e6e 6563 740d 0a0d 0a5b 6f70 7469  connect....[opti
-00000350: 6f6e 735d 0d0a 7a69 705f 7361 6665 203d  ons]..zip_safe =
-00000360: 2046 616c 7365 0d0a 696e 636c 7564 655f   False..include_
-00000370: 7061 636b 6167 655f 6461 7461 203d 2054  package_data = T
-00000380: 7275 650d 0a70 6163 6b61 6765 7320 3d20  rue..packages = 
-00000390: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
-000003a0: 7175 6972 6573 203d 203e 3d33 2e37 0d0a  quires = >=3.7..
-000003b0: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-000003c0: 203d 200d 0a09 6169 6f68 7474 702d 7373   = ...aiohttp-ss
-000003d0: 652d 636c 6965 6e74 3e3d 302e 322e 310d  e-client>=0.2.1.
-000003e0: 0a09 7079 6e61 636c 3e3d 312e 352e 300d  ..pynacl>=1.5.0.
-000003f0: 0a09 7265 7175 6573 7473 3e3d 322e 3238  ..requests>=2.28
-00000400: 2e32 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .2....[options.p
-00000410: 6163 6b61 6765 732e 6669 6e64 5d0d 0a65  ackages.find]..e
-00000420: 7863 6c75 6465 203d 200d 0a09 6578 616d  xclude = ...exam
-00000430: 706c 6573 2a0d 0a09 6465 7674 6f6f 6c73  ples*...devtools
-00000440: 2a0d 0a09 646f 6373 2a0d 0a09 7465 7374  *...docs*...test
-00000450: 732a 0d0a 0976 656e 762a 0d0a 0d0a 5b65  s*...venv*....[e
-00000460: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-00000470: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-00000480: 203d 2030 0d0a 0d0a                       = 0....
+00000110: 656e 7420 5374 6174 7573 203a 3a20 3420  ent Status :: 4 
+00000120: 2d20 4265 7461 0d0a 0949 6e74 656e 6465  - Beta...Intende
+00000130: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
+00000140: 7665 6c6f 7065 7273 0d0a 094c 6963 656e  velopers...Licen
+00000150: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+00000160: 6564 203a 3a20 4170 6163 6865 2053 6f66  ed :: Apache Sof
+00000170: 7477 6172 6520 4c69 6365 6e73 650d 0a09  tware License...
+00000180: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+00000190: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+000001a0: 6e74 0d0a 0950 726f 6772 616d 6d69 6e67  nt...Programming
+000001b0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000001c0: 686f 6e20 3a3a 2033 0d0a 0950 726f 6772  hon :: 3...Progr
+000001d0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000001e0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e37  :: Python :: 3.7
+000001f0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000200: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000210: 6e20 3a3a 2033 2e38 0d0a 0950 726f 6772  n :: 3.8...Progr
+00000220: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000230: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
+00000240: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000250: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000260: 6e20 3a3a 2033 2e31 300d 0a09 5072 6f67  n :: 3.10...Prog
+00000270: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000280: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000290: 3131 0d0a 0954 6f70 6963 203a 3a20 536f  11...Topic :: So
+000002a0: 6674 7761 7265 2044 6576 656c 6f70 6d65  ftware Developme
+000002b0: 6e74 203a 3a20 4c69 6272 6172 6965 7320  nt :: Libraries 
+000002c0: 3a3a 2050 7974 686f 6e20 4d6f 6475 6c65  :: Python Module
+000002d0: 730d 0a61 7574 686f 7220 3d20 5861 4262  s..author = XaBb
+000002e0: 6c34 0d0a 6175 7468 6f72 5f65 6d61 696c  l4..author_email
+000002f0: 203d 2078 6162 626c 3440 676d 6169 6c2e   = xabbl4@gmail.
+00000300: 636f 6d0d 0a70 726f 6a65 6374 5f75 726c  com..project_url
+00000310: 7320 3d20 0d0a 0947 6974 6875 6220 3d20  s = ...Github = 
+00000320: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000330: 6f6d 2f58 6142 626c 342f 7079 746f 6e63  om/XaBbl4/pytonc
+00000340: 6f6e 6e65 6374 0d0a 0d0a 5b6f 7074 696f  onnect....[optio
+00000350: 6e73 5d0d 0a7a 6970 5f73 6166 6520 3d20  ns]..zip_safe = 
+00000360: 4661 6c73 650d 0a69 6e63 6c75 6465 5f70  False..include_p
+00000370: 6163 6b61 6765 5f64 6174 6120 3d20 5472  ackage_data = Tr
+00000380: 7565 0d0a 7061 636b 6167 6573 203d 2066  ue..packages = f
+00000390: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
+000003a0: 7569 7265 7320 3d20 3e3d 332e 370d 0a69  uires = >=3.7..i
+000003b0: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
+000003c0: 3d20 0d0a 0961 696f 6874 7470 2d73 7365  = ...aiohttp-sse
+000003d0: 2d63 6c69 656e 743e 3d30 2e32 2e31 0d0a  -client>=0.2.1..
+000003e0: 0970 796e 6163 6c3e 3d31 2e35 2e30 0d0a  .pynacl>=1.5.0..
+000003f0: 0972 6571 7565 7374 733e 3d32 2e32 382e  .requests>=2.28.
+00000400: 320d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  2....[options.pa
+00000410: 636b 6167 6573 2e66 696e 645d 0d0a 6578  ckages.find]..ex
+00000420: 636c 7564 6520 3d20 0d0a 0965 7861 6d70  clude = ...examp
+00000430: 6c65 732a 0d0a 0964 6576 746f 6f6c 732a  les*...devtools*
+00000440: 0d0a 0964 6f63 732a 0d0a 0974 6573 7473  ...docs*...tests
+00000450: 2a0d 0a09 7665 6e76 2a0d 0a0d 0a5b 6567  *...venv*....[eg
+00000460: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000470: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000480: 3d20 300d 0a0d 0a                        = 0....
```

