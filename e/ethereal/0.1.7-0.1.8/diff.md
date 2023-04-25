# Comparing `tmp/ethereal-0.1.7.tar.gz` & `tmp/ethereal-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethereal-0.1.7.tar", max compression
+gzip compressed data, was "ethereal-0.1.8.tar", max compression
```

## Comparing `ethereal-0.1.7.tar` & `ethereal-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1067 2023-04-02 19:03:02.167776 ethereal-0.1.7/LICENSE
--rw-r--r--   0        0        0     1758 2023-04-19 16:04:17.948471 ethereal-0.1.7/README.md
--rw-r--r--   0        0        0     1308 2023-04-16 07:11:11.928618 ethereal-0.1.7/ethereal/__init__.py
--rw-r--r--   0        0        0     1298 2023-04-25 07:56:06.788173 ethereal-0.1.7/ethereal/accounts.py
--rw-r--r--   0        0        0     1402 2023-04-14 14:08:02.175740 ethereal-0.1.7/ethereal/app.py
--rw-r--r--   0        0        0      288 2023-04-14 18:53:08.549415 ethereal-0.1.7/ethereal/base.py
--rw-r--r--   0        0        0     6978 2023-04-16 06:36:31.316428 ethereal-0.1.7/ethereal/cache.py
--rw-r--r--   0        0        0      782 2023-04-14 18:44:54.261252 ethereal-0.1.7/ethereal/config.yml
--rw-r--r--   0        0        0     1061 2023-04-20 20:19:54.363594 ethereal-0.1.7/ethereal/containers.py
--rw-r--r--   0        0        0     8806 2023-04-17 07:14:39.659777 ethereal-0.1.7/ethereal/contracts.py
--rw-r--r--   0        0        0     4652 2023-04-14 18:47:51.186401 ethereal-0.1.7/ethereal/etherscan.py
--rw-r--r--   0        0        0     4135 2023-04-21 13:57:00.795630 ethereal-0.1.7/ethereal/facade.py
--rw-r--r--   0        0        0     1439 2023-04-14 18:59:17.941096 ethereal-0.1.7/ethereal/networks.py
--rw-r--r--   0        0        0      655 2023-04-25 08:03:15.644636 ethereal-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2680 2023-04-25 08:03:40.504931 ethereal-0.1.7/setup.py
--rw-r--r--   0        0        0     2394 2023-04-25 08:03:40.505158 ethereal-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-02 19:03:02.167776 ethereal-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1758 2023-04-19 16:04:17.948471 ethereal-0.1.8/README.md
+-rw-r--r--   0        0        0     1308 2023-04-16 07:11:11.928618 ethereal-0.1.8/ethereal/__init__.py
+-rw-r--r--   0        0        0     1324 2023-04-25 08:16:47.966799 ethereal-0.1.8/ethereal/accounts.py
+-rw-r--r--   0        0        0     1402 2023-04-14 14:08:02.175740 ethereal-0.1.8/ethereal/app.py
+-rw-r--r--   0        0        0      288 2023-04-14 18:53:08.549415 ethereal-0.1.8/ethereal/base.py
+-rw-r--r--   0        0        0     6978 2023-04-16 06:36:31.316428 ethereal-0.1.8/ethereal/cache.py
+-rw-r--r--   0        0        0      782 2023-04-14 18:44:54.261252 ethereal-0.1.8/ethereal/config.yml
+-rw-r--r--   0        0        0     1061 2023-04-20 20:19:54.363594 ethereal-0.1.8/ethereal/containers.py
+-rw-r--r--   0        0        0     8806 2023-04-17 07:14:39.659777 ethereal-0.1.8/ethereal/contracts.py
+-rw-r--r--   0        0        0     4652 2023-04-14 18:47:51.186401 ethereal-0.1.8/ethereal/etherscan.py
+-rw-r--r--   0        0        0     4135 2023-04-21 13:57:00.795630 ethereal-0.1.8/ethereal/facade.py
+-rw-r--r--   0        0        0     1439 2023-04-14 18:59:17.941096 ethereal-0.1.8/ethereal/networks.py
+-rw-r--r--   0        0        0      655 2023-04-25 08:17:01.064951 ethereal-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2680 2023-04-25 12:28:15.390572 ethereal-0.1.8/setup.py
+-rw-r--r--   0        0        0     2394 2023-04-25 12:28:15.390789 ethereal-0.1.8/PKG-INFO
```

### Comparing `ethereal-0.1.7/LICENSE` & `ethereal-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.7/README.md` & `ethereal-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.7/ethereal/__init__.py` & `ethereal-0.1.8/ethereal/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.7/ethereal/accounts.py` & `ethereal-0.1.8/ethereal/accounts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import TypedDict
 from hdwallet import BIP44HDWallet
-from hdwallet.utils import generate_mnemonic
+from hdwallet.utils import generate_seed_phrase as generate_mnemominc
 from hdwallet.symbols import ETH as SYMBOL
 
 
 class Account(TypedDict):
     """
     Account
     """
@@ -42,8 +42,8 @@
         """
         Generate a mnemonic
 
         :param strength: The strength of the mnemonic. Default = 128 (12 words)
 
         :return: The mnemonic
         """
-        return generate_mnemonic(strength=strength)
+        return generate_mnemominc(strength=strength)
```

### Comparing `ethereal-0.1.7/ethereal/app.py` & `ethereal-0.1.8/ethereal/app.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.7/ethereal/cache.py` & `ethereal-0.1.8/ethereal/cache.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.7/ethereal/config.yml` & `ethereal-0.1.8/ethereal/config.yml`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.7/ethereal/containers.py` & `ethereal-0.1.8/ethereal/containers.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.7/ethereal/contracts.py` & `ethereal-0.1.8/ethereal/contracts.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.7/ethereal/etherscan.py` & `ethereal-0.1.8/ethereal/etherscan.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.7/ethereal/facade.py` & `ethereal-0.1.8/ethereal/facade.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.7/ethereal/networks.py` & `ethereal-0.1.8/ethereal/networks.py`

 * *Files identical despite different names*

### Comparing `ethereal-0.1.7/pyproject.toml` & `ethereal-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ethereal"
-version = "0.1.7"
+version = "0.1.8"
 description = "Ergonomic python tooling for web3"
 authors = ["Alex Euler <0xalexeuler@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `ethereal-0.1.7/setup.py` & `ethereal-0.1.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'web3>=6.1.0,<7.0.0']
 
 entry_points = \
 {'console_scripts': ['ethereal = ethereal:cli']}
 
 setup_kwargs = {
     'name': 'ethereal',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Ergonomic python tooling for web3',
     'long_description': '![Ethereal logo](./docs/images/ethereal_cat.png)\n\n## Ethereal\n\n[![docs](https://readthedocs.org/projects/ethereal/badge/?version=latest)](https://ethereal.readthedocs.io/en/latest/?badge=latest)\n\nEthereal is a lightweight wrapper around the [Web3](https://web3py.readthedocs.io/en/stable/web3.main.html#web3.Web3) class that simplifies\nworking with Ethereum smart contracts.\n\nTo use it, simply create a regular [Web3](https://web3py.readthedocs.io/en/stable/web3.main.html#web3.Web3) instance and write `w3 = Ethereal(w3)`.\nThen, you can use w3 as usual, but with additional methods\naccessible under the `e` property.\n\nFor example, you can call `w3.e.get_abi("0x...")` or\n`w3.e.list_events("0x...", "Mint", "2023-01-01", "2023-02-14")`.\n\nFor more available methods, please refer to the [EtherealFacade](https://ethereal.readthedocs.io/en/latest/?badge=latest#ethereal.facade.EtherealFacade) class.\n\n### Demo\n\n![Ethereal demo](./docs/images/demo.gif)\n\n### Example\n\n```python\nfrom web3.auto import w3\nfrom ethereal import Ethereal\nfrom ethereal import load_provider_from_uri\n\n# If WEB3_PROVIDER_URI env is not set, uncomment the lines below\n# w3 = Web3(load_provider_from_uri("https://alchemy.com/..."))\n\nw3 = Ethereal(w3)\n\nADDRESS = "0xB0B195aEFA3650A6908f15CdaC7D92F8a5791B0B"\nprint(w3.e.list_events(ADDRESS))\n# Lists event signatures for the contract at ADDRESS\n\nevents = w3.e.get_events(ADDRESS, "Transfer", "2023-01-01", "2023-02-14")\n# Gets all Transfer events for the contract at ADDRESS between 2023-01-01 and 2023-02-14\nprint(events[:10])\n```\n\n### Install\n\n```\npip install ethereal\n```\n\n### Supported networks\n\n- Ethereum\n- Polygon\n- Avalanche\n- Fantom\n- Arbitrum\n- Optimism\n\n### Contributing\n\nFeel free to create feature requests or pull requests :D\n',
     'author': 'Alex Euler',
     'author_email': '0xalexeuler@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `ethereal-0.1.7/PKG-INFO` & `ethereal-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethereal
-Version: 0.1.7
+Version: 0.1.8
 Summary: Ergonomic python tooling for web3
 License: MIT
 Author: Alex Euler
 Author-email: 0xalexeuler@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

