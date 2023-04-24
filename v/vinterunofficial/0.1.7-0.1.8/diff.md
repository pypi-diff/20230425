# Comparing `tmp/vinterunofficial-0.1.7.tar.gz` & `tmp/vinterunofficial-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vinterunofficial-0.1.7.tar", last modified: Sat Apr  8 20:46:58 2023, max compression
+gzip compressed data, was "vinterunofficial-0.1.8.tar", last modified: Mon Apr 24 22:36:22 2023, max compression
```

## Comparing `vinterunofficial-0.1.7.tar` & `vinterunofficial-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:46:58.397491 vinterunofficial-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-04-08 20:46:58.397491 vinterunofficial-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 20:46:58.397491 vinterunofficial-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:46:58.393491 vinterunofficial-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21284 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/tests/test_async_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/tests/test_vinter_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/tests/test_ws.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:46:58.397491 vinterunofficial-0.1.7/vinterunofficial/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/vinterunofficial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/vinterunofficial/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/vinterunofficial/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/vinterunofficial/vinter_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/vinterunofficial/vinter_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)    15517 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/vinterunofficial/vinter_sdk_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-08 20:46:30.000000 vinterunofficial-0.1.7/vinterunofficial/vinter_sdk_ws.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:46:58.397491 vinterunofficial-0.1.7/vinterunofficial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-04-08 20:46:58.000000 vinterunofficial-0.1.7/vinterunofficial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-08 20:46:58.000000 vinterunofficial-0.1.7/vinterunofficial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 20:46:58.000000 vinterunofficial-0.1.7/vinterunofficial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 20:46:58.000000 vinterunofficial-0.1.7/vinterunofficial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-08 20:46:58.000000 vinterunofficial-0.1.7/vinterunofficial.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:36:22.074924 vinterunofficial-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-04-24 22:36:22.074924 vinterunofficial-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-04-24 22:35:25.000000 vinterunofficial-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-24 22:35:25.000000 vinterunofficial-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 22:36:22.074924 vinterunofficial-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:36:22.070924 vinterunofficial-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21284 2023-04-24 22:35:25.000000 vinterunofficial-0.1.8/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-04-24 22:35:25.000000 vinterunofficial-0.1.8/tests/test_async_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-24 22:35:25.000000 vinterunofficial-0.1.8/tests/test_vinter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-24 22:35:25.000000 vinterunofficial-0.1.8/tests/test_ws.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:36:22.070924 vinterunofficial-0.1.8/vinterunofficial/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-24 22:35:25.000000 vinterunofficial-0.1.8/vinterunofficial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-24 22:35:25.000000 vinterunofficial-0.1.8/vinterunofficial/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-04-24 22:35:25.000000 vinterunofficial-0.1.8/vinterunofficial/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-04-24 22:35:25.000000 vinterunofficial-0.1.8/vinterunofficial/vinter_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-04-24 22:35:25.000000 vinterunofficial-0.1.8/vinterunofficial/vinter_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-04-24 22:35:25.000000 vinterunofficial-0.1.8/vinterunofficial/vinter_sdk_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-24 22:35:25.000000 vinterunofficial-0.1.8/vinterunofficial/vinter_sdk_ws.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:36:22.074924 vinterunofficial-0.1.8/vinterunofficial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-04-24 22:36:22.000000 vinterunofficial-0.1.8/vinterunofficial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-24 22:36:22.000000 vinterunofficial-0.1.8/vinterunofficial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 22:36:22.000000 vinterunofficial-0.1.8/vinterunofficial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 22:36:22.000000 vinterunofficial-0.1.8/vinterunofficial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 22:36:22.000000 vinterunofficial-0.1.8/vinterunofficial.egg-info/top_level.txt
```

### Comparing `vinterunofficial-0.1.7/PKG-INFO` & `vinterunofficial-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vinterunofficial
-Version: 0.1.7
+Version: 0.1.8
 Project-URL: homepage, https://rahulmistri1997.github.io/vinterunofficial-pypi
 Project-URL: documentation, https://rahulmistri1997.github.io/vinterunofficial-pypi
 Project-URL: repository, https://github.com/rahulmistri1997/vinterunofficial-pypi
 Description-Content-Type: text/markdown
 
 # Unofficial Wrapper for the Vinter API
 ![Code Coverage](https://img.shields.io/badge/Coverage-100%25-brightgreen.svg)
```

### Comparing `vinterunofficial-0.1.7/README.md` & `vinterunofficial-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `vinterunofficial-0.1.7/pyproject.toml` & `vinterunofficial-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=38.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vinterunofficial"
-version = "0.1.7"
+version = "0.1.8"
 dependencies = ["httpx==0.23.3", "websocket-client==1.5.1"]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [metadata]
```

### Comparing `vinterunofficial-0.1.7/tests/test_api.py` & `vinterunofficial-0.1.8/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `vinterunofficial-0.1.7/tests/test_async_api.py` & `vinterunofficial-0.1.8/tests/test_async_api.py`

 * *Files identical despite different names*

### Comparing `vinterunofficial-0.1.7/tests/test_vinter_utils.py` & `vinterunofficial-0.1.8/tests/test_vinter_utils.py`

 * *Files identical despite different names*

### Comparing `vinterunofficial-0.1.7/tests/test_ws.py` & `vinterunofficial-0.1.8/tests/test_ws.py`

 * *Files identical despite different names*

### Comparing `vinterunofficial-0.1.7/vinterunofficial/config.py` & `vinterunofficial-0.1.8/vinterunofficial/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,53 +1,60 @@
 from enum import Enum
 
 APIBASE = "https://www.vinterapi.com/api/v3"
 WSBASE = "wss://www.vinterapi.com/ws"
 
+
 class WsAssetType(Enum):
     MULTI_ASSET = "multi_assets"
     SINGLE_ASSET = "single_assets"
     NAV = "nav"
 
+
 class WsAssetUrl(Enum):
     MULTI_ASSET = {
         "asset_type": WsAssetType.MULTI_ASSET,
         "url": f"{WSBASE}/{WsAssetType.MULTI_ASSET.value.replace('_', '')}",
     }
     SINGLE_ASSET = {
         "asset_type": WsAssetType.SINGLE_ASSET,
         "url": f"{WSBASE}/{WsAssetType.SINGLE_ASSET.value.replace('_', '')}",
     }
     NAV = {
         "asset_type": WsAssetType.NAV,
         "url": f"{WSBASE}/{WsAssetType.NAV.value}",
     }
 
+
 class Frequency(Enum):
     REAL_TIME = "r"
     HOURLY = "h"
     DAILY = "d"
 
+
 class FrequencyApiType(Enum):
     REAL_TIME = "real_time"
     HOURLY = "hourly"
     DAILY = "daily"
 
+
 class AssetType(Enum):
     MULTI_ASSET = "multi_assets"
     SINGLE_ASSET = "single_assets"
     STAKING_YIELD = "staking_yields"
     NAV = "nav"
 
+
 class ActiveAssetType(Enum):
     MULTI_ASSET = "active_multi_assets"
     SINGLE_ASSET = "active_single_assets"
     STAKING_YIELD = "active_staking_yields"
     NAV = "active_nav"
 
+
 class AssetUrl(Enum):
     MULTI_ASSET_REAL_TIME = {
         "frequency": Frequency.REAL_TIME,
         "asset_type": AssetType.MULTI_ASSET,
         "url": f"{APIBASE}/{AssetType.MULTI_ASSET.value}_{FrequencyApiType.REAL_TIME.value}",
     }
     SINGLE_ASSET_REAL_TIME = {
@@ -110,8 +117,8 @@
         "asset_type": AssetType.STAKING_YIELD,
         "url": f"{APIBASE}/{ActiveAssetType.STAKING_YIELD.value}",
     }
     ACTIVE_NAV = {
         "frequency": None,
         "asset_type": AssetType.NAV,
         "url": f"{APIBASE}/{ActiveAssetType.NAV.value}",
-    }
+    }
```

### Comparing `vinterunofficial-0.1.7/vinterunofficial/utils.py` & `vinterunofficial-0.1.8/vinterunofficial/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 from .config import Frequency, AssetType, AssetUrl, WsAssetType, WsAssetUrl
 
+
 class VinterValidation:
-    
     def __init__(self) -> None:
         pass
 
     @staticmethod
     def validate_asset_type(asset_type: str) -> None:
         """If the asset type is not a valid asset_type , then raise a
         ValueError
@@ -18,15 +18,15 @@
 
         """
         valid_asset_types = [asset_type.value for asset_type in AssetType]
         if asset_type not in valid_asset_types:
             raise ValueError(
                 f"The asset type must be one of the following : {valid_asset_types}"
             )
-        
+
     @staticmethod
     def validate_frequency(frequency: str) -> None:
         """If the frequency is not a valid frequency, then raise a
         ValueError
 
         Parameters
         ----------
@@ -37,34 +37,34 @@
         frequencies = [frequency.value for frequency in Frequency]
         if frequency not in frequencies:
             raise ValueError(
                 "The frequency must be one of the following valid frequencies: {}".format(
                     frequencies
                 )
             )
-        
+
     @staticmethod
     def validate_symbol_frequency(symbol: str) -> tuple:
-        '''It takes a string, splits it on the hyphen, and validates the last part of the string
-        
+        """It takes a string, splits it on the hyphen, and validates the last part of the string
+
         Parameters
         ----------
         symbol : str
             str
-        
+
         Returns
         -------
             A tuple of the symbol and the frequency.
-        
-        '''
-        
+
+        """
+
         sym_frequency = symbol.split("-")[-1]
         VinterValidation.validate_frequency(sym_frequency)
         return symbol, sym_frequency
-    
+
     @staticmethod
     def validate_dates(dates: list) -> None:
         """It raises a ValueError if any of the dates in the dates list are not in the format YYYY-MM-DD
 
         Parameters
         ----------
         dates
@@ -78,19 +78,18 @@
             except ValueError as e:
                 e.args = (
                     "The date must be in the format YYYY-MM-DD. The date: {} is not in the correct format.".format(
                         date
                     ),
                 )
                 raise
-    
-    
-class VinterUrl:
 
-    def __init__(self):    
+
+class VinterUrl:
+    def __init__(self):
         pass
 
     @staticmethod
     def get_active_url(asset_type: str) -> str:
         """This function returns the url to use to get the data"""
         url = None
         for asset_url in AssetUrl:
@@ -98,111 +97,101 @@
                 asset_url.value["asset_type"].value == asset_type
                 and asset_url.value["frequency"] is None
             ):
                 url = asset_url.value["url"]
                 break
 
         if url is None:
-            raise ValueError(
-                f"The asset type must be in {asset_type}"
-            )
-        
+            raise ValueError(f"The asset type must be in {asset_type}")
+
         return url
 
     @staticmethod
     def get_url(asset_type: str, frequency: str = None) -> str:
-        '''It takes in an asset type and a frequency and returns a url
-        
+        """It takes in an asset type and a frequency and returns a url
+
         Parameters
         ----------
         asset_type : str
             str
         frequency : str
             str = None
-        
+
         Returns
         -------
             The url is being returned.
-        
-        '''
+
+        """
 
         asset_types = [asset_type.value for asset_type in AssetType]
-        
+
         url = None
         for asset_url in AssetUrl:
             if (
                 asset_url.value["asset_type"].value == asset_type
                 and asset_url.value["frequency"].value == frequency
             ):
                 url = asset_url.value["url"]
                 break
 
         if url is None:
-            raise ValueError(
-                f"The asset type must be in {asset_types}"
-            )
-        
+            raise ValueError(f"The asset type must be in {asset_types}")
+
         return url
-    
+
     @staticmethod
     def get_url_by_symbol(asset_type: str, symbol: str) -> str:
-        '''It takes in an asset type and a symbol and returns a url
-        
+        """It takes in an asset type and a symbol and returns a url
+
         Parameters
         ----------
         asset_type : str
             str
         symbol : str
             str
-        
+
         Returns
         -------
             The url is being returned.
-        
-        '''
-        
+
+        """
+
         symbol, frequency = VinterValidation.validate_symbol_frequency(symbol)
         url = VinterUrl.get_url(asset_type=asset_type, frequency=frequency)
-        
+
         return url
-    
+
     @staticmethod
     def websocket_url(asset_type: str, symbol: str = None) -> str:
-        '''It takes in an asset type and a frequency and returns a websocket url
-        
+        """It takes in an asset type and a frequency and returns a websocket url
+
         Parameters
         ----------
         asset_type : str
             str
         frequency : str
             str = None
-        
+
         Returns
         -------
             The websocket url is being returned.
-        
-        '''
+
+        """
 
         ws_asset_types = [asset_type.value for asset_type in WsAssetType]
 
         if symbol is None:
-            raise ValueError(
-                "The symbol must be provided."
-            )
-        
+            raise ValueError("The symbol must be provided.")
+
         symbol, frequency = VinterValidation.validate_symbol_frequency(symbol)
-        
+
         url = None
         for asset_url in WsAssetUrl:
-            if (
-                asset_url.value["asset_type"].value == asset_type
-            ):
+            if asset_url.value["asset_type"].value == asset_type:
                 url = asset_url.value["url"]
                 url = url + "/" + symbol
                 break
 
         if url is None:
-            raise ValueError(
-                f"The asset type must be in {ws_asset_types}"
-            )
-        
-        return url
+            raise ValueError(f"The asset type must be in {ws_asset_types}")
+
+        return url
```

### Comparing `vinterunofficial-0.1.7/vinterunofficial/vinter_abc.py` & `vinterunofficial-0.1.8/vinterunofficial/vinter_abc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from abc import ABC, abstractmethod
 from typing import Union
 
+
 class VinterAPIABC(ABC):
-    
     @abstractmethod
-    def __init__(self, api_key: str, asset_type: str): # pragma: no cover
+    def __init__(self, api_key: str, asset_type: str):  # pragma: no cover
         """This function takes in an api_key and asset_type and sets them as attributes of the class
 
         Parameters
         ----------
         api_key : str
             Your API key.
         asset_type : str
             The type of asset you want to get data for. The acceptable asset types listed in the AssetType enum.
         """
         pass
 
     @abstractmethod
-    def get_all_active_symbols(self, frequency: str = None, symbol_only: bool = False) -> Union[list, dict]: # pragma: no cover
+    def get_all_active_symbols(
+        self, frequency: str = None, symbol_only: bool = False
+    ) -> Union[list, dict]:  # pragma: no cover
         """This function returns a dictionary of all the active symbols
 
         Returns
         -------
             A dictionary of all the active symbols
 
         """
         pass
 
-
     @abstractmethod
-    def get_latest_data(self, symbol: str, limit: int = 1) -> dict: # pragma: no cover
+    def get_latest_data(self, symbol: str, limit: int = 1) -> dict:  # pragma: no cover
         """It takes a symbol and a limit as parameters, and returns a dictionary of the latest data for
         that symbol
 
         Parameters
         ----------
         symbol : str
             The symbol of the asset you want to get data for.
@@ -44,31 +45,31 @@
         -------
             A dictionary of the latest data for the symbol and limit.
 
         """
         pass
 
     @abstractmethod
-    def get_latest_value(self, symbol: str) -> float: # pragma: no cover
+    def get_latest_value(self, symbol: str) -> float:  # pragma: no cover
         """This function takes in a symbol and returns the latest value for that symbol
 
         Parameters
         ----------
         symbol : str
             The symbol of the asset you want to get data for.
 
         Returns
         -------
             The latest value for the symbol
 
         """
         pass
-    
+
     @abstractmethod
-    def _filter_by_symbol(self, data: list, symbol: str) -> list: # pragma: no cover
+    def _filter_by_symbol(self, data: list, symbol: str) -> list:  # pragma: no cover
         """This function takes in a list of data and a symbol and returns a list of data for that symbol
 
         Parameters
         ----------
         data : list
             A list of data
         symbol : str
@@ -78,15 +79,15 @@
         -------
             A list of data for the symbol
 
         """
         pass
 
     @abstractmethod
-    def _get_active_asset_data(self, symbol: str) -> dict: # pragma: no cover
+    def _get_active_asset_data(self, symbol: str) -> dict:  # pragma: no cover
         """This function returns the data for the active asset
 
         Parameters
         ----------
         symbol : str
             The symbol of the asset you want to get data for.
 
@@ -94,160 +95,172 @@
         -------
             A dictionary of the data for the active asset
 
         """
         pass
 
     @abstractmethod
-    def get_current_rebalance_weight(self, symbol: str) -> dict: # pragma: no cover
+    def get_current_rebalance_weight(self, symbol: str) -> dict:  # pragma: no cover
         """This function returns the current rebalance weight of multi_assets symbol
 
         Returns
         -------
             Weight of the current rebalance of the multi_assets symbol
-            
+
             OR
-            
+
             ValueError if the symbol is not a present in the list of active symbols for asset_type multi_assets
 
         """
         pass
 
     @abstractmethod
-    def get_contributions(self, symbol: str) -> dict: # pragma: no cover
+    def get_contributions(self, symbol: str) -> dict:  # pragma: no cover
         """This function returns the contributions of the single_assets symbol
 
         Returns
         -------
             A dictionary of the contributions of the single_assets symbol
 
             OR
 
             ValueError if the symbol is not a present in the list of active symbols for asset_type single_assets
 
         """
         pass
 
     @abstractmethod
-    def get_previous_rebalance_date(self, symbol: str) -> Union[str, None]: # pragma: no cover
+    def get_previous_rebalance_date(
+        self, symbol: str
+    ) -> Union[str, None]:  # pragma: no cover
         """This function returns the previous rebalance date of multi_assets symbol
 
         Returns
         -------
             Date of the previous rebalance of the multi_assets symbol
-            
+
             OR
-            
+
             ValueError if the symbol is not a present in the list of active symbols for asset_type multi_assets
-            
+
             OR
-            
+
             None if the symbol Rebalance is not scheduled
 
         """
         pass
 
     @abstractmethod
-    def get_previous_review_date(self, symbol: str) -> Union[str, None]: # pragma: no cover
+    def get_previous_review_date(
+        self, symbol: str
+    ) -> Union[str, None]:  # pragma: no cover
         """This function returns the previous review date of multi_assets symbol
 
         Returns
         -------
             Date of the previous review of the multi_assets symbol
-            
+
             OR
-            
+
             ValueError if the symbol is not a present in the list of active symbols for asset_type multi_assets
-            
+
             OR
-            
+
             None if the symbol Review is not scheduled
 
         """
         pass
 
     @abstractmethod
-    def get_next_review_date(self, symbol: str) -> Union[str, None]: # pragma: no cover
+    def get_next_review_date(self, symbol: str) -> Union[str, None]:  # pragma: no cover
         """This function returns the next review date of multi_assets symbol
 
         Returns
         -------
             Date of the next review of the multi_assets symbol
-            
+
             OR
-            
+
             ValueError if the symbol is not a present in the list of active symbols for asset_type multi_assets
-            
+
             OR
-            
+
             None if the symbol Review is not scheduled
 
         """
         pass
 
     @abstractmethod
-    def get_next_rebalance_date(self, symbol: str) -> Union[str, None]: # pragma: no cover
+    def get_next_rebalance_date(
+        self, symbol: str
+    ) -> Union[str, None]:  # pragma: no cover
         """This function returns the next rebalance date of multi_assets symbol
 
         Returns
         -------
             Date of the next rebalance of the multi_assets symbol
-            
+
             OR
-            
+
             ValueError if the symbol is not a present in the list of active symbols for asset_type multi_assets
-            
+
             OR
-            
+
             None if the symbol Rebalance is not scheduled
 
         """
         pass
 
     @abstractmethod
-    def get_next_rebalance_weight(self, symbol: str) -> Union[str, None]: # pragma: no cover
+    def get_next_rebalance_weight(
+        self, symbol: str
+    ) -> Union[str, None]:  # pragma: no cover
         """This function returns the next rebalance weight of multi_assets symbol
 
         Returns
         -------
             Weight of the next rebalance of the multi_assets symbol
-            
+
             OR
-            
+
             ValueError if the symbol is not a present in the list of active symbols for asset_type multi_assets
-            
+
             OR
 
             None if the symbol Rebalance is not present in the payload
 
         """
         pass
 
     @abstractmethod
-    def get_data_by_date(self, symbol: str, dates: Union[str, list]) -> dict: # pragma: no cover
+    def get_data_by_date(
+        self, symbol: str, dates: Union[str, list]
+    ) -> dict:  # pragma: no cover
         """This function takes in a symbol and a date and returns a dictionary of the data for that date
 
         This function is only for daily data.
-        
+
         Parameters
         ----------
         symbol : str
             The symbol of the asset you want to get data for.
         date : str | list
             The date of the data you want to get. format: YYYY-MM-DD
 
         Returns
         -------
             A dictionary of the data
 
         """
         pass
-           
+
     @abstractmethod
-    def get_data_by_time(self, symbol: str, start: str, end: str = None, limit: int = 1000) -> dict: # pragma: no cover
+    def get_data_by_time(
+        self, symbol: str, start: str, end: str = None, limit: int = 1000
+    ) -> dict:  # pragma: no cover
         """This function takes in a symbol and a start and end date and returns a dictionary of the data
         for that period
 
         Parameters
         ----------
         symbol : str
             The symbol of the asset you want to get data for.
@@ -258,8 +271,7 @@
 
         Returns
         -------
             A dictionary of the data
 
         """
         pass
-
```

### Comparing `vinterunofficial-0.1.7/vinterunofficial/vinter_sdk.py` & `vinterunofficial-0.1.8/vinterunofficial/vinter_sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from datetime import datetime, timedelta
 from .config import Frequency, AssetType, AssetUrl
 from .utils import VinterValidation, VinterUrl
 from .vinter_abc import VinterAPIABC
 
 APIKEY = os.environ.get("VINTER_API_KEY", None)
 
+
 class VinterAPI(VinterAPIABC):
     def __init__(self, api_key: str, asset_type: str):
         """This function takes in an api_key and asset_type and sets them as attributes of the class
 
         Parameters
         ----------
         api_key : str
@@ -24,42 +25,44 @@
         self.api_key = api_key
         self.asset_type = asset_type
         self.frequencies = [frequency.value for frequency in Frequency]
         self.valid_asset_types = [asset_type.value for asset_type in AssetType]
         VinterValidation.validate_asset_type(self.asset_type)
         self.httpx_client = httpx.Client(follow_redirects=True, timeout=10)
 
-    def get_all_active_symbols(self, frequency: str = None, symbol_only: bool = False) -> Union[list, dict]:
+    def get_all_active_symbols(
+        self, frequency: str = None, symbol_only: bool = False
+    ) -> Union[list, dict]:
         """This function returns a dictionary of all the active symbols
 
         Returns
         -------
             A dictionary of all the active symbols
 
         """
         url = VinterUrl.get_active_url(self.asset_type)
         headers = {}
         response = self.httpx_client.get(url, headers=headers)
 
-        response.raise_for_status() # Raise an exception if the request failed
+        response.raise_for_status()  # Raise an exception if the request failed
 
         data = response.json()["data"]
 
         if frequency is not None:
-
             VinterValidation.validate_frequency(frequency)
 
-            data = [asset for asset in data if asset['symbol'].split('-')[-1] == frequency]
+            data = [
+                asset for asset in data if asset["symbol"].split("-")[-1] == frequency
+            ]
 
         if symbol_only:
             data = [asset["symbol"] for asset in data]
 
         return data
 
-
     def get_latest_data(self, symbol: str, limit: int = 1) -> dict:
         """It takes a symbol and a limit as parameters, and returns a dictionary of the latest data for
         that symbol
 
         Parameters
         ----------
         symbol : str
@@ -98,15 +101,15 @@
         Returns
         -------
             The latest value for the symbol
 
         """
         data = self.get_latest_data(symbol=symbol)
         return data[0]["value"]
-    
+
     def _filter_by_symbol(self, data: list, symbol: str) -> list:
         """This function takes in a list of data and a symbol and returns a list of data for that symbol
 
         Parameters
         ----------
         data : list
             A list of data
@@ -131,15 +134,15 @@
         Returns
         -------
             A dictionary of the data for the active asset
 
         """
 
         symbol, frequency = VinterValidation.validate_symbol_frequency(symbol)
-        
+
         data = self.get_all_active_symbols()
 
         output = self._filter_by_symbol(data=data, symbol=symbol)
 
         if len(output) == 0:
             raise ValueError("No data was found for the symbol: {}".format(symbol))
 
@@ -147,17 +150,17 @@
 
     def get_current_rebalance_weight(self, symbol: str) -> dict:
         """This function returns the current rebalance weight of multi_assets symbol
 
         Returns
         -------
             Weight of the current rebalance of the multi_assets symbol
-            
+
             OR
-            
+
             ValueError if the symbol is not a present in the list of active symbols for asset_type multi_assets
 
         """
 
         if self.asset_type != AssetType.MULTI_ASSET.value:
             raise ValueError(
                 f"The asset type must be {AssetType.MULTI_ASSET.value} to use this function"
@@ -167,15 +170,15 @@
 
         data = self._get_active_asset_data(symbol=symbol)
 
         output = data.get("weights", None)
 
         if output is None or output == "":
             raise ValueError("No data was found for the symbol: {}".format(symbol))
-        
+
         return output
 
     def get_contributions(self, symbol: str) -> dict:
         """This function returns the contributions of the single_assets symbol
 
         Returns
         -------
@@ -207,21 +210,21 @@
 
     def get_previous_rebalance_date(self, symbol: str) -> Union[str, None]:
         """This function returns the previous rebalance date of multi_assets symbol
 
         Returns
         -------
             Date of the previous rebalance of the multi_assets symbol
-            
+
             OR
-            
+
             ValueError if the symbol is not a present in the list of active symbols for asset_type multi_assets
-            
+
             OR
-            
+
             None if the symbol Rebalance is not scheduled
 
         """
 
         if self.asset_type != AssetType.MULTI_ASSET.value:
             raise ValueError(
                 f"The asset type must be {AssetType.MULTI_ASSET.value} to use this function"
@@ -237,21 +240,21 @@
 
     def get_previous_review_date(self, symbol: str) -> Union[str, None]:
         """This function returns the previous review date of multi_assets symbol
 
         Returns
         -------
             Date of the previous review of the multi_assets symbol
-            
+
             OR
-            
+
             ValueError if the symbol is not a present in the list of active symbols for asset_type multi_assets
-            
+
             OR
-            
+
             None if the symbol Review is not scheduled
 
         """
 
         if self.asset_type != AssetType.MULTI_ASSET.value:
             raise ValueError(
                 f"The asset type must be {AssetType.MULTI_ASSET.value} to use this function"
@@ -267,21 +270,21 @@
 
     def get_next_review_date(self, symbol: str) -> Union[str, None]:
         """This function returns the next review date of multi_assets symbol
 
         Returns
         -------
             Date of the next review of the multi_assets symbol
-            
+
             OR
-            
+
             ValueError if the symbol is not a present in the list of active symbols for asset_type multi_assets
-            
+
             OR
-            
+
             None if the symbol Review is not scheduled
 
         """
 
         if self.asset_type != AssetType.MULTI_ASSET.value:
             raise ValueError(
                 f"The asset type must be {AssetType.MULTI_ASSET.value} to use this function"
@@ -297,21 +300,21 @@
 
     def get_next_rebalance_date(self, symbol: str) -> Union[str, None]:
         """This function returns the next rebalance date of multi_assets symbol
 
         Returns
         -------
             Date of the next rebalance of the multi_assets symbol
-            
+
             OR
-            
+
             ValueError if the symbol is not a present in the list of active symbols for asset_type multi_assets
-            
+
             OR
-            
+
             None if the symbol Rebalance is not scheduled
 
         """
 
         if self.asset_type != AssetType.MULTI_ASSET.value:
             raise ValueError(
                 f"The asset type must be {AssetType.MULTI_ASSET.value} to use this function"
@@ -327,19 +330,19 @@
 
     def get_next_rebalance_weight(self, symbol: str) -> Union[str, None]:
         """This function returns the next rebalance weight of multi_assets symbol
 
         Returns
         -------
             Weight of the next rebalance of the multi_assets symbol
-            
+
             OR
-            
+
             ValueError if the symbol is not a present in the list of active symbols for asset_type multi_assets
-            
+
             OR
 
             None if the symbol Rebalance is not present in the payload
 
         """
 
         if self.asset_type != AssetType.MULTI_ASSET.value:
@@ -351,20 +354,19 @@
 
         data = self._get_active_asset_data(symbol=symbol)
 
         output = data.get("next_rebalance_weights", None)
 
         return output
 
-
     def get_data_by_date(self, symbol: str, dates: Union[str, list]) -> dict:
         """This function takes in a symbol and a date and returns a dictionary of the data for that date
 
         This function is only for daily data.
-        
+
         Parameters
         ----------
         symbol : str
             The symbol of the asset you want to get data for.
         date : str | list
             The date of the data you want to get. format: YYYY-MM-DD
 
@@ -391,16 +393,18 @@
 
         # Converting the datetime object to string
         last_date = last_date.strftime("%Y-%m-%d")
 
         data = self.get_data_by_time(symbol=symbol, start=start_date, end=last_date)
 
         return data
-           
-    def get_data_by_time(self, symbol: str, start: str, end: str = None, limit: int = 1000) -> dict:
+
+    def get_data_by_time(
+        self, symbol: str, start: str, end: str = None, limit: int = 1000
+    ) -> dict:
         """This function takes in a symbol and a start and end date and returns a dictionary of the data
         for that period
 
         Parameters
         ----------
         symbol : str
             The symbol of the asset you want to get data for.
@@ -412,30 +416,37 @@
         Returns
         -------
             A dictionary of the data
 
         """
         url = VinterUrl.get_url_by_symbol(asset_type=self.asset_type, symbol=symbol)
 
-        params = {"symbol": symbol, "start_time": start, "end_time": end, "limit": limit}
+        params = {
+            "symbol": symbol,
+            "start_time": start,
+            "end_time": end,
+            "limit": limit,
+        }
         headers = {"Authorization": self.api_key}
         response = self.httpx_client.get(url, params=params, headers=headers)
 
-        response.raise_for_status() # Raise an exception if the request fails
+        response.raise_for_status()  # Raise an exception if the request fails
 
         data = response.json()["data"]
 
-        if len(data) == 0:               
-            raise ValueError(f"No data was found for the symbol: {symbol} between {start} and {end}.")
+        if len(data) == 0:
+            raise ValueError(
+                f"No data was found for the symbol: {symbol} between {start} and {end}."
+            )
 
         return data
 
     def save_data_to_file(
         self, data: dict, filename: str, file_type: str = "csv", seprator: str = ","
-    ) -> None: # pragma: no cover
+    ) -> None:  # pragma: no cover
         """This function takes in a dictionary of data and a filename and saves the data to a csv file
 
         Parameters
         ----------
         data : dict
             A dictionary of data to save to a csv file.
         filename : str
@@ -445,15 +456,14 @@
             ["csv", "json"]
         seprator : str
             The seprator to use when saving the data to the csv file.
 
         """
         file_type = file_type.lower()
         if file_type not in ["csv", "json"]:
-
             raise ValueError("The file type must be either csv or json")
 
         if file_type == "json":
             with open(filename, "w") as f:
                 json.dump(data, f, indent=4)
             return
 
@@ -468,9 +478,7 @@
                     for key, value in row.items():
                         if isinstance(value, (dict, list)):
                             row[key] = json.dumps(value)
 
                     csv.DictWriter(
                         f, row.keys(), delimiter=seprator, lineterminator="\n"
                     ).writerow(row)
-
-
```

### Comparing `vinterunofficial-0.1.7/vinterunofficial/vinter_sdk_async.py` & `vinterunofficial-0.1.8/vinterunofficial/vinter_sdk_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import json
 from typing import Union
 from datetime import datetime, timedelta
 from .config import Frequency, AssetType, AssetUrl
 from .utils import VinterValidation, VinterUrl
 from .vinter_abc import VinterAPIABC
 
+
 class VinterAPIAsync(VinterAPIABC):
     def __init__(self, api_key: str, asset_type: str):
         """This function takes in an api_key and asset_type and sets them as attributes of the class
 
         Parameters
         ----------
         api_key : str
@@ -22,42 +23,44 @@
         self.api_key = api_key
         self.asset_type = asset_type
         self.frequencies = [frequency.value for frequency in Frequency]
         self.valid_asset_types = [asset_type.value for asset_type in AssetType]
         VinterValidation.validate_asset_type(self.asset_type)
         self.httpx_client = httpx.AsyncClient(follow_redirects=True, timeout=10)
 
-    async def get_all_active_symbols(self, frequency: str = None, symbol_only: bool = False) -> Union[list, dict]:
+    async def get_all_active_symbols(
+        self, frequency: str = None, symbol_only: bool = False
+    ) -> Union[list, dict]:
         """This function returns a dictionary of all the active symbols
 
         Returns
         -------
             A dictionary of all the active symbols
 
         """
         url = VinterUrl.get_active_url(self.asset_type)
         headers = {}
         response = await self.httpx_client.get(url, headers=headers)
 
-        response.raise_for_status() # Raise an exception if the request failed
+        response.raise_for_status()  # Raise an exception if the request failed
 
         data = response.json()["data"]
 
         if frequency is not None:
-
             VinterValidation.validate_frequency(frequency)
 
-            data = [asset for asset in data if asset['symbol'].split('-')[-1] == frequency]
+            data = [
+                asset for asset in data if asset["symbol"].split("-")[-1] == frequency
+            ]
 
         if symbol_only:
             data = [asset["symbol"] for asset in data]
 
         return data
 
-
     async def get_latest_data(self, symbol: str, limit: int = 1) -> dict:
         """It takes a symbol and a limit as parameters, and returns a dictionary of the latest data for
         that symbol
 
         Parameters
         ----------
         symbol : str
@@ -96,15 +99,15 @@
         Returns
         -------
             The latest value for the symbol
 
         """
         data = await self.get_latest_data(symbol=symbol)
         return data[0]["value"]
-    
+
     def _filter_by_symbol(self, data: list, symbol: str) -> list:
         """This function takes in a list of data and a symbol and returns a list of data for that symbol
 
         Parameters
         ----------
         data : list
             A list of data
@@ -129,15 +132,15 @@
         Returns
         -------
             A dictionary of the data for the active asset
 
         """
 
         symbol, frequency = VinterValidation.validate_symbol_frequency(symbol)
-        
+
         data = await self.get_all_active_symbols()
 
         output = self._filter_by_symbol(data=data, symbol=symbol)
 
         if len(output) == 0:
             raise ValueError("No data was found for the symbol: {}".format(symbol))
 
@@ -145,17 +148,17 @@
 
     async def get_current_rebalance_weight(self, symbol: str) -> dict:
         """This function returns the current rebalance weight of multi_assets symbol
 
         Returns
         -------
             Weight of the current rebalance of the multi_assets symbol
-            
+
             OR
-            
+
             ValueError if the symbol is not a present in the list of active symbols for asset_type multi_assets
 
         """
 
         if self.asset_type != AssetType.MULTI_ASSET.value:
             raise ValueError(
                 f"The asset type must be {AssetType.MULTI_ASSET.value} to use this function"
@@ -165,15 +168,15 @@
 
         data = await self._get_active_asset_data(symbol=symbol)
 
         output = data.get("weights", None)
 
         if output is None or output == "":
             raise ValueError("No data was found for the symbol: {}".format(symbol))
-        
+
         return output
 
     async def get_contributions(self, symbol: str) -> dict:
         """This function returns the contributions of the single_assets symbol
 
         Returns
         -------
@@ -205,21 +208,21 @@
 
     async def get_previous_rebalance_date(self, symbol: str) -> Union[str, None]:
         """This function returns the previous rebalance date of multi_assets symbol
 
         Returns
         -------
             Date of the previous rebalance of the multi_assets symbol
-            
+
             OR
-            
+
             ValueError if the symbol is not a present in the list of active symbols for asset_type multi_assets
-            
+
             OR
-            
+
             None if the symbol Rebalance is not scheduled
 
         """
 
         if self.asset_type != AssetType.MULTI_ASSET.value:
             raise ValueError(
                 f"The asset type must be {AssetType.MULTI_ASSET.value} to use this function"
@@ -235,21 +238,21 @@
 
     async def get_previous_review_date(self, symbol: str) -> Union[str, None]:
         """This function returns the previous review date of multi_assets symbol
 
         Returns
         -------
             Date of the previous review of the multi_assets symbol
-            
+
             OR
-            
+
             ValueError if the symbol is not a present in the list of active symbols for asset_type multi_assets
-            
+
             OR
-            
+
             None if the symbol Review is not scheduled
 
         """
 
         if self.asset_type != AssetType.MULTI_ASSET.value:
             raise ValueError(
                 f"The asset type must be {AssetType.MULTI_ASSET.value} to use this function"
@@ -265,21 +268,21 @@
 
     async def get_next_review_date(self, symbol: str) -> Union[str, None]:
         """This function returns the next review date of multi_assets symbol
 
         Returns
         -------
             Date of the next review of the multi_assets symbol
-            
+
             OR
-            
+
             ValueError if the symbol is not a present in the list of active symbols for asset_type multi_assets
-            
+
             OR
-            
+
             None if the symbol Review is not scheduled
 
         """
 
         if self.asset_type != AssetType.MULTI_ASSET.value:
             raise ValueError(
                 f"The asset type must be {AssetType.MULTI_ASSET.value} to use this function"
@@ -295,21 +298,21 @@
 
     async def get_next_rebalance_date(self, symbol: str) -> Union[str, None]:
         """This function returns the next rebalance date of multi_assets symbol
 
         Returns
         -------
             Date of the next rebalance of the multi_assets symbol
-            
+
             OR
-            
+
             ValueError if the symbol is not a present in the list of active symbols for asset_type multi_assets
-            
+
             OR
-            
+
             None if the symbol Rebalance is not scheduled
 
         """
 
         if self.asset_type != AssetType.MULTI_ASSET.value:
             raise ValueError(
                 f"The asset type must be {AssetType.MULTI_ASSET.value} to use this function"
@@ -325,19 +328,19 @@
 
     async def get_next_rebalance_weight(self, symbol: str) -> Union[str, None]:
         """This function returns the next rebalance weight of multi_assets symbol
 
         Returns
         -------
             Weight of the next rebalance of the multi_assets symbol
-            
+
             OR
-            
+
             ValueError if the symbol is not a present in the list of active symbols for asset_type multi_assets
-            
+
             OR
 
             None if the symbol Rebalance is not present in the payload
 
         """
 
         if self.asset_type != AssetType.MULTI_ASSET.value:
@@ -349,20 +352,19 @@
 
         data = await self._get_active_asset_data(symbol=symbol)
 
         output = data.get("next_rebalance_weights", None)
 
         return output
 
-
     async def get_data_by_date(self, symbol: str, dates: Union[str, list]) -> dict:
         """This function takes in a symbol and a date and returns a dictionary of the data for that date
 
         This function is only for daily data.
-        
+
         Parameters
         ----------
         symbol : str
             The symbol of the asset you want to get data for.
         date : str | list
             The date of the data you want to get. format: YYYY-MM-DD
 
@@ -386,19 +388,23 @@
 
         # Adding 1 day to the last date to get the data for the last date
         last_date = datetime.strptime(last_date, "%Y-%m-%d") + timedelta(days=1)
 
         # Converting the datetime object to string
         last_date = last_date.strftime("%Y-%m-%d")
 
-        data = await self.get_data_by_time(symbol=symbol, start=start_date, end=last_date)
+        data = await self.get_data_by_time(
+            symbol=symbol, start=start_date, end=last_date
+        )
 
         return data
-           
-    async def get_data_by_time(self, symbol: str, start: str, end: str = None, limit: int = 1000) -> dict:
+
+    async def get_data_by_time(
+        self, symbol: str, start: str, end: str = None, limit: int = 1000
+    ) -> dict:
         """This function takes in a symbol and a start and end date and returns a dictionary of the data
         for that period
 
         Parameters
         ----------
         symbol : str
             The symbol of the asset you want to get data for.
@@ -410,30 +416,37 @@
         Returns
         -------
             A dictionary of the data
 
         """
         url = VinterUrl.get_url_by_symbol(asset_type=self.asset_type, symbol=symbol)
 
-        params = {"symbol": symbol, "start_time": start, "end_time": end, "limit": limit}
+        params = {
+            "symbol": symbol,
+            "start_time": start,
+            "end_time": end,
+            "limit": limit,
+        }
         headers = {"Authorization": self.api_key}
         response = await self.httpx_client.get(url, params=params, headers=headers)
 
-        response.raise_for_status() # Raise an exception if the request fails
+        response.raise_for_status()  # Raise an exception if the request fails
 
         data = response.json()["data"]
 
-        if len(data) == 0:               
-            raise ValueError(f"No data was found for the symbol: {symbol} between {start} and {end}.")
+        if len(data) == 0:
+            raise ValueError(
+                f"No data was found for the symbol: {symbol} between {start} and {end}."
+            )
 
         return data
 
     def save_data_to_file(
         self, data: dict, filename: str, file_type: str = "csv", seprator: str = ","
-    ) -> None: # pragma: no cover
+    ) -> None:  # pragma: no cover
         """This function takes in a dictionary of data and a filename and saves the data to a csv file
 
         Parameters
         ----------
         data : dict
             A dictionary of data to save to a csv file.
         filename : str
@@ -443,15 +456,14 @@
             ["csv", "json"]
         seprator : str
             The seprator to use when saving the data to the csv file.
 
         """
         file_type = file_type.lower()
         if file_type not in ["csv", "json"]:
-
             raise ValueError("The file type must be either csv or json")
 
         if file_type == "json":
             with open(filename, "w") as f:
                 json.dump(data, f, indent=4)
             return
```

### Comparing `vinterunofficial-0.1.7/vinterunofficial/vinter_sdk_ws.py` & `vinterunofficial-0.1.8/vinterunofficial/vinter_sdk_ws.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import websocket
 from .utils import VinterUrl
 
+
 class VinterAPIWS:
-    def __init__(self, symbol, token, asset_type, on_message, on_error, on_close, on_open):
-        '''The function takes in a symbol, token, asset type, and four callback functions. It then creates
+    def __init__(
+        self, symbol, token, asset_type, on_message, on_error, on_close, on_open
+    ):
+        """The function takes in a symbol, token, asset type, and four callback functions. It then creates
         a websocket connection to the url for the symbol and asset type.
-        
+
         Parameters
         ----------
         symbol
             The symbol you want to subscribe to.
         token
             Your API token.
         asset_type
@@ -18,48 +21,43 @@
             This is the callback function that will be called when a message is received from the server.
         on_error
             This is a callback function that will be called when an error occurs.
         on_close
             A function that will be called when the websocket is closed.
         on_open
             This is a callback function that will be called when the connection is opened.
-        
-        '''
+
+        """
         self.ws = None
         self.symbol = symbol
         self.token = token
         self.asset_type = asset_type
         self.url = self.get_ws_url() + "/?token=" + self.token
         self.on_message = on_message
         self.on_error = on_error
         self.on_close = on_close
         self.on_open = on_open
 
     def get_ws_url(self):
-        '''It takes the asset type and symbol and returns the websocket url
-        
+        """It takes the asset type and symbol and returns the websocket url
+
         Returns
         -------
             The websocket url for the asset type and symbol.
-        
-        '''
+
+        """
         return VinterUrl.websocket_url(self.asset_type, self.symbol)
 
     def open(self):
-        '''The function opens a websocket connection to the url specified in the constructor
-        
-        '''
+        """The function opens a websocket connection to the url specified in the constructor"""
         self.ws = websocket.WebSocketApp(
             self.url,
             on_message=self.on_message,
             on_error=self.on_error,
             on_close=self.on_close,
             on_open=self.on_open,
         )
         self.ws.run_forever()
 
     def close(self):
-        '''The function closes the websocket connection
-        
-        '''
+        """The function closes the websocket connection"""
         self.ws.close()
-
```

### Comparing `vinterunofficial-0.1.7/vinterunofficial.egg-info/PKG-INFO` & `vinterunofficial-0.1.8/vinterunofficial.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vinterunofficial
-Version: 0.1.7
+Version: 0.1.8
 Project-URL: homepage, https://rahulmistri1997.github.io/vinterunofficial-pypi
 Project-URL: documentation, https://rahulmistri1997.github.io/vinterunofficial-pypi
 Project-URL: repository, https://github.com/rahulmistri1997/vinterunofficial-pypi
 Description-Content-Type: text/markdown
 
 # Unofficial Wrapper for the Vinter API
 ![Code Coverage](https://img.shields.io/badge/Coverage-100%25-brightgreen.svg)
```

### Comparing `vinterunofficial-0.1.7/vinterunofficial.egg-info/SOURCES.txt` & `vinterunofficial-0.1.8/vinterunofficial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

