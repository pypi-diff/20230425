# Comparing `tmp/tap_norwaycitybikeapi-0.1.0.tar.gz` & `tmp/tap_norwaycitybikeapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_norwaycitybikeapi-0.1.0.tar", max compression
+gzip compressed data, was "tap_norwaycitybikeapi-0.1.1.tar", max compression
```

## Comparing `tap_norwaycitybikeapi-0.1.0.tar` & `tap_norwaycitybikeapi-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     4188 2023-04-24 19:16:31.775538 tap_norwaycitybikeapi-0.1.0/README.md
--rw-r--r--   0        0        0     1259 2023-04-24 19:16:46.351562 tap_norwaycitybikeapi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       33 2023-04-23 20:13:17.667392 tap_norwaycitybikeapi-0.1.0/tap_norwaycitybikeapi/__init__.py
--rw-r--r--   0        0        0     2376 2023-04-24 19:14:16.777878 tap_norwaycitybikeapi-0.1.0/tap_norwaycitybikeapi/client.py
--rw-r--r--   0        0        0     3069 2023-04-24 16:55:13.041576 tap_norwaycitybikeapi-0.1.0/tap_norwaycitybikeapi/streams.py
--rw-r--r--   0        0        0     1470 2023-04-24 19:15:31.550948 tap_norwaycitybikeapi-0.1.0/tap_norwaycitybikeapi/tap.py
--rw-r--r--   0        0        0     5060 1970-01-01 00:00:00.000000 tap_norwaycitybikeapi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4157 2023-04-24 22:36:14.540106 tap_norwaycitybikeapi-0.1.1/README.md
+-rw-r--r--   0        0        0     1259 2023-04-24 22:36:59.388494 tap_norwaycitybikeapi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       33 2023-04-23 20:13:17.667392 tap_norwaycitybikeapi-0.1.1/tap_norwaycitybikeapi/__init__.py
+-rw-r--r--   0        0        0     2376 2023-04-24 19:14:16.777878 tap_norwaycitybikeapi-0.1.1/tap_norwaycitybikeapi/client.py
+-rw-r--r--   0        0        0     3069 2023-04-24 16:55:13.041576 tap_norwaycitybikeapi-0.1.1/tap_norwaycitybikeapi/streams.py
+-rw-r--r--   0        0        0     1751 2023-04-24 22:35:15.360361 tap_norwaycitybikeapi-0.1.1/tap_norwaycitybikeapi/tap.py
+-rw-r--r--   0        0        0     5029 1970-01-01 00:00:00.000000 tap_norwaycitybikeapi-0.1.1/PKG-INFO
```

### Comparing `tap_norwaycitybikeapi-0.1.0/README.md` & `tap_norwaycitybikeapi-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 <p align="center">
   <img src="assets/bysykkel_logo.png" width="150" title="logo">
 </p>
 
 # tap-norwaycitybikeapi
 
 `tap-norwaycitybikeapi` is a Singer tap for the [Trondheim](https://trondheimbysykkel.no/en/open-data/realtime), [Oslo](https://oslobysykkel.no/en/open-data/realtime) and [Bergen](https://bergenbysykkel.no/en/open-data/realtime) City Bike APIs.
-> **Note*
-> Please note that the City Bike API data is published under the [Norwegian Licence for Open Government Data (NLOD) 2.0](https://data.norge.no/nlod/en/2.0).
 
 Built with the [Meltano Tap SDK](https://sdk.meltano.com) for Singer Taps.
 
+> **Note**
+> The City Bike APIs are published under the [Norwegian Licence for Open Government Data (NLOD) 2.0](https://data.norge.no/nlod/en/2.0).
+
+
 ## Capabilities
 
 * `catalog`
 * `state`
 * `discover`
 * `about`
 * `stream-maps`
 * `schema-flattening`
 
-## Settings
-
-
 ## Installation
 
 Install from PyPi:
 
 ```bash
 pipx install tap-norwaycitybikeapi
 ```
```

### Comparing `tap_norwaycitybikeapi-0.1.0/pyproject.toml` & `tap_norwaycitybikeapi-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-norwaycitybikeapi"
-version = "0.1.0"
+version = "0.1.1"
 description = "`tap-norwaycitybikeapi` is a Singer tap for NorwayCityBikeAPI, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["Kristian André Jakobsen <k.andrejakobsen@gmail.com>"]
 keywords = ["ELT", "NorwayCityBikeAPI"]
 license = "Apache 2.0"
 packages = [{ include = "tap_norwaycitybikeapi" }]
```

### Comparing `tap_norwaycitybikeapi-0.1.0/tap_norwaycitybikeapi/client.py` & `tap_norwaycitybikeapi-0.1.1/tap_norwaycitybikeapi/client.py`

 * *Files identical despite different names*

### Comparing `tap_norwaycitybikeapi-0.1.0/tap_norwaycitybikeapi/streams.py` & `tap_norwaycitybikeapi-0.1.1/tap_norwaycitybikeapi/streams.py`

 * *Files identical despite different names*

### Comparing `tap_norwaycitybikeapi-0.1.0/tap_norwaycitybikeapi/tap.py` & `tap_norwaycitybikeapi-0.1.1/tap_norwaycitybikeapi/tap.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,25 @@
             th.StringType,
             default="oslo",
             required=True,
             description=(
                 "Name of Norwegian city having City Bikes. "
                 "Currently only available for Trondheim, Oslo and Bergen."
             ),
+            allowed_values=[
+                "oslo",
+                "bergen",
+                "trondheim",
+                "Oslo",
+                "Bergen",
+                "Trondheim",
+                "OSLO",
+                "BERGEN",
+                "TRONDHEIM",
+            ],
         ),
     ).to_dict()
 
     def discover_streams(self) -> list[NorwayCityBikeAPIStream]:
         """Return a list of discovered streams.
 
         Returns:
```

### Comparing `tap_norwaycitybikeapi-0.1.0/PKG-INFO` & `tap_norwaycitybikeapi-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-norwaycitybikeapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: `tap-norwaycitybikeapi` is a Singer tap for NorwayCityBikeAPI, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,NorwayCityBikeAPI
 Author: Kristian André Jakobsen
 Author-email: k.andrejakobsen@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
@@ -23,31 +23,30 @@
 <p align="center">
   <img src="assets/bysykkel_logo.png" width="150" title="logo">
 </p>
 
 # tap-norwaycitybikeapi
 
 `tap-norwaycitybikeapi` is a Singer tap for the [Trondheim](https://trondheimbysykkel.no/en/open-data/realtime), [Oslo](https://oslobysykkel.no/en/open-data/realtime) and [Bergen](https://bergenbysykkel.no/en/open-data/realtime) City Bike APIs.
-> **Note*
-> Please note that the City Bike API data is published under the [Norwegian Licence for Open Government Data (NLOD) 2.0](https://data.norge.no/nlod/en/2.0).
 
 Built with the [Meltano Tap SDK](https://sdk.meltano.com) for Singer Taps.
 
+> **Note**
+> The City Bike APIs are published under the [Norwegian Licence for Open Government Data (NLOD) 2.0](https://data.norge.no/nlod/en/2.0).
+
+
 ## Capabilities
 
 * `catalog`
 * `state`
 * `discover`
 * `about`
 * `stream-maps`
 * `schema-flattening`
 
-## Settings
-
-
 ## Installation
 
 Install from PyPi:
 
 ```bash
 pipx install tap-norwaycitybikeapi
 ```
```

