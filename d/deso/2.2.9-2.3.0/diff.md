# Comparing `tmp/deso-2.2.9.tar.gz` & `tmp/deso-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deso-2.2.9.tar", last modified: Thu Apr 20 15:12:46 2023, max compression
+gzip compressed data, was "deso-2.3.0.tar", last modified: Tue Apr 25 05:09:43 2023, max compression
```

## Comparing `deso-2.2.9.tar` & `deso-2.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 15:12:46.579748 deso-2.2.9/
--rw-rw-rw-   0        0        0     1085 2022-10-22 06:55:06.000000 deso-2.2.9/LICENSE
--rw-rw-rw-   0        0        0    20360 2023-04-20 15:12:46.578495 deso-2.2.9/PKG-INFO
--rw-rw-rw-   0        0        0    19062 2023-02-08 08:09:20.000000 deso-2.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 15:12:46.554368 deso-2.2.9/deso/
--rw-rw-rw-   0        0        0     2262 2022-10-22 06:55:06.000000 deso-2.2.9/deso/Derived.py
--rw-rw-rw-   0        0        0     2838 2023-02-08 08:09:20.000000 deso-2.2.9/deso/Identity.py
--rw-rw-rw-   0        0        0     1032 2022-10-22 06:55:06.000000 deso-2.2.9/deso/Media.py
--rw-rw-rw-   0        0        0     1745 2022-10-22 06:55:06.000000 deso-2.2.9/deso/Metadata.py
--rw-rw-rw-   0        0        0     5422 2023-04-20 15:06:54.000000 deso-2.2.9/deso/Posts.py
--rw-rw-rw-   0        0        0     3759 2023-04-16 19:32:16.000000 deso-2.2.9/deso/Sign.py
--rw-rw-rw-   0        0        0    28489 2023-04-16 19:32:16.000000 deso-2.2.9/deso/Social.py
--rw-rw-rw-   0        0        0    15734 2022-10-22 06:55:06.000000 deso-2.2.9/deso/Trade.py
--rw-rw-rw-   0        0        0     7817 2023-02-08 08:09:20.000000 deso-2.2.9/deso/User.py
--rw-rw-rw-   0        0        0      256 2022-10-22 06:55:06.000000 deso-2.2.9/deso/__init__.py
--rw-rw-rw-   0        0        0     1634 2022-10-22 06:55:06.000000 deso-2.2.9/deso/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-20 15:12:46.575496 deso-2.2.9/deso.egg-info/
--rw-rw-rw-   0        0        0    20360 2023-04-20 15:12:46.000000 deso-2.2.9/deso.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-04-20 15:12:46.000000 deso-2.2.9/deso.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 15:12:46.000000 deso-2.2.9/deso.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-20 15:12:46.000000 deso-2.2.9/deso.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-20 15:12:46.000000 deso-2.2.9/deso.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 15:12:46.580755 deso-2.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1425 2023-04-20 15:12:35.000000 deso-2.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 05:09:42.996905 deso-2.3.0/
+-rw-rw-rw-   0        0        0     1085 2022-10-22 06:55:06.000000 deso-2.3.0/LICENSE
+-rw-rw-rw-   0        0        0    20360 2023-04-25 05:09:42.995188 deso-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    19062 2023-02-08 08:09:20.000000 deso-2.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 05:09:42.967928 deso-2.3.0/deso/
+-rw-rw-rw-   0        0        0     2262 2022-10-22 06:55:06.000000 deso-2.3.0/deso/Derived.py
+-rw-rw-rw-   0        0        0     2838 2023-02-08 08:09:20.000000 deso-2.3.0/deso/Identity.py
+-rw-rw-rw-   0        0        0     1032 2022-10-22 06:55:06.000000 deso-2.3.0/deso/Media.py
+-rw-rw-rw-   0        0        0     1745 2022-10-22 06:55:06.000000 deso-2.3.0/deso/Metadata.py
+-rw-rw-rw-   0        0        0     5422 2023-04-20 15:06:54.000000 deso-2.3.0/deso/Posts.py
+-rw-rw-rw-   0        0        0     4411 2023-04-25 05:08:33.000000 deso-2.3.0/deso/Sign.py
+-rw-rw-rw-   0        0        0    28489 2023-04-16 19:32:16.000000 deso-2.3.0/deso/Social.py
+-rw-rw-rw-   0        0        0    15734 2022-10-22 06:55:06.000000 deso-2.3.0/deso/Trade.py
+-rw-rw-rw-   0        0        0     7817 2023-02-08 08:09:20.000000 deso-2.3.0/deso/User.py
+-rw-rw-rw-   0        0        0      256 2022-10-22 06:55:06.000000 deso-2.3.0/deso/__init__.py
+-rw-rw-rw-   0        0        0     1634 2022-10-22 06:55:06.000000 deso-2.3.0/deso/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-25 05:09:42.989519 deso-2.3.0/deso.egg-info/
+-rw-rw-rw-   0        0        0    20360 2023-04-25 05:09:42.000000 deso-2.3.0/deso.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-04-25 05:09:42.000000 deso-2.3.0/deso.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 05:09:42.000000 deso-2.3.0/deso.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-25 05:09:42.000000 deso-2.3.0/deso.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-25 05:09:42.000000 deso-2.3.0/deso.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 05:09:42.996905 deso-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1425 2023-04-25 05:09:25.000000 deso-2.3.0/setup.py
```

### Comparing `deso-2.2.9/LICENSE` & `deso-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deso-2.2.9/PKG-INFO` & `deso-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deso
-Version: 2.2.9
+Version: 2.3.0
 Summary: A python module for deso
 Author: ItsAditya (https://itsaditya.xyz)
 Author-email: <chaudharyaditya0005@gmail.com>
 Keywords: deso,python,bitclout,social media,crypto,blockchain,decentralisation,decentralized social media
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deso-2.2.9/README.md` & `deso-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `deso-2.2.9/deso/Derived.py` & `deso-2.3.0/deso/Derived.py`

 * *Files identical despite different names*

### Comparing `deso-2.2.9/deso/Identity.py` & `deso-2.3.0/deso/Identity.py`

 * *Files identical despite different names*

### Comparing `deso-2.2.9/deso/Media.py` & `deso-2.3.0/deso/Media.py`

 * *Files identical despite different names*

### Comparing `deso-2.2.9/deso/Metadata.py` & `deso-2.3.0/deso/Metadata.py`

 * *Files identical despite different names*

### Comparing `deso-2.2.9/deso/Posts.py` & `deso-2.3.0/deso/Posts.py`

 * *Files identical despite different names*

### Comparing `deso-2.2.9/deso/Sign.py` & `deso-2.3.0/deso/Sign.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# This file has code for signing a transaction --> Credit: MiniGlome
+# This file has code for signing a transaction --> Credit: MiniGlome and nathanwells
 import hashlib
 import hmac
-
+import requests
+from deso.Route import getRoute
 
 def inverse_mod(k, p):
     """Returns the inverse of k modulo p.
     This function returns the only integer x such that (x * k) % p == 1.
     k must be non-zero and p must be a prime.
     """
     if k == 0:
@@ -127,31 +128,43 @@
 
 
 def hexify(n):
     n = hex(n)[2:]
     if len(n) % 2 != 0:
         n = "0" + n
     return n
+# New for the Balance Model fork
+def getTransactionIndex(TransactionHex):
+    endpointURL = getRoute() + "signature-index"
+    payload = {"TransactionHex": TransactionHex}
+    response = requests.post(endpointURL, json=payload)
+    return response.json()['SignatureIndex']
 
 
 def Sign_Transaction(seedHex, TransactionHex):
+    transactionBytes = bytes.fromhex(TransactionHex)
     s256 = hashlib.sha256(
-        hashlib.sha256(bytes.fromhex(TransactionHex)).digest()
+        hashlib.sha256(transactionBytes).digest()
     ).digest()
     drbg = hmac_drbg(entropy=bytes.fromhex(seedHex), string=s256)
     k = int.from_bytes(drbg, "big")
     kp = scalar_mult(k, g)
     kpX = kp[0]
     r = kpX % n
     s = inverse_mod(k, n) * (r * int(seedHex, 16) + int(s256.hex(), 16))
     s = s % n
     # Enforce low-s -> credit to @Nathanwells 
     if s > n // 2:
         s = n - s
     signature = to_DER(hexify(r), hexify(s))
+    # Added for Balance Model fork
+    signatureIndex = int(getTransactionIndex(TransactionHex))
+    v0FieldsWithoutSignature = transactionBytes[:signatureIndex]
+    v1FieldsBuffer = transactionBytes[1 + signatureIndex:]
     signed_transaction = (
-        TransactionHex[:-2]
+        v0FieldsWithoutSignature.hex()
         + hex(len(bytearray.fromhex(signature)))[2:]
         + signature
+        + v1FieldsBuffer.hex()
     )
 
     return signed_transaction
```

### Comparing `deso-2.2.9/deso/Social.py` & `deso-2.3.0/deso/Social.py`

 * *Files identical despite different names*

### Comparing `deso-2.2.9/deso/Trade.py` & `deso-2.3.0/deso/Trade.py`

 * *Files identical despite different names*

### Comparing `deso-2.2.9/deso/User.py` & `deso-2.3.0/deso/User.py`

 * *Files identical despite different names*

### Comparing `deso-2.2.9/deso/utils.py` & `deso-2.3.0/deso/utils.py`

 * *Files identical despite different names*

### Comparing `deso-2.2.9/deso.egg-info/PKG-INFO` & `deso-2.3.0/deso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deso
-Version: 2.2.9
+Version: 2.3.0
 Summary: A python module for deso
 Author: ItsAditya (https://itsaditya.xyz)
 Author-email: <chaudharyaditya0005@gmail.com>
 Keywords: deso,python,bitclout,social media,crypto,blockchain,decentralisation,decentralized social media
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deso-2.2.9/setup.py` & `deso-2.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "2.2.9"
+VERSION = "2.3.0"
 DESCRIPTION = "A python module for DeSo"
 LONG_DESCRIPTION = "DesoPy is a python module that enables devs to interact with DeSo Blockchain using node.deso.org node by default. Includes all functions to read from or write to DeSo Blockchain"
 # Setting up
 setup(
     name="deso",
     version=VERSION,
     author="ItsAditya (https://itsaditya.xyz)",
```

