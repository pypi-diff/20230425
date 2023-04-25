# Comparing `tmp/wiliot-core-4.0.6.tar.gz` & `tmp/wiliot-core-4.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-core-4.0.6.tar", last modified: Mon Mar  6 13:31:30 2023, max compression
+gzip compressed data, was "wiliot-core-4.0.8.tar", last modified: Tue Apr 25 08:27:47 2023, max compression
```

## Comparing `wiliot-core-4.0.6.tar` & `wiliot-core-4.0.8.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-06 13:31:30.155662 wiliot-core-4.0.6/
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     2483 2023-03-06 13:31:30.155662 wiliot-core-4.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1971 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)     7184 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-03-06 13:31:30.155662 wiliot-core-4.0.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1869 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-06 13:31:30.147662 wiliot-core-4.0.6/wiliot_core/
--rw-rw-rw-   0 root         (0) root         (0)     4596 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-06 13:31:30.147662 wiliot-core-4.0.6/wiliot_core/local_gateway/
--rw-rw-rw-   0 root         (0) root         (0)     4010 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/local_gateway/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12755 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/local_gateway/continuous_listener.py
--rw-rw-rw-   0 root         (0) root         (0)    12763 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/local_gateway/custom_energy_pattern.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-06 13:31:30.147662 wiliot-core-4.0.6/wiliot_core/local_gateway/examples/
--rw-rw-rw-   0 root         (0) root         (0)     4010 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/local_gateway/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6666 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/local_gateway/examples/local_gateway_basic_example.py
--rw-rw-rw-   0 root         (0) root         (0)    82917 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/local_gateway/local_gateway_core.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-06 13:31:30.151662 wiliot-core-4.0.6/wiliot_core/local_gateway/local_gateway_versions/
--rw-rw-rw-   0 root         (0) root         (0)   253422 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/local_gateway/local_gateway_versions/3.8.14_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   448599 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/local_gateway/local_gateway_versions/3.8.14_sd_bl_gw_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   229471 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/local_gateway/local_gateway_versions/4.0.4_app.zip
--rw-rw-rw-   0 root         (0) root         (0)   424656 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/local_gateway/local_gateway_versions/4.0.4_sd_bl_gw_app.zip
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/local_gateway/local_gateway_versions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)  1242814 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/local_gateway/local_gateway_versions/wifi_3.8.14.hex
--rw-rw-rw-   0 root         (0) root         (0)  1176930 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.4.hex
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-06 13:31:30.151662 wiliot-core-4.0.6/wiliot_core/packet_data/
--rw-rw-rw-   0 root         (0) root         (0)     4010 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/packet_data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26807 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/packet_data/packet.py
--rw-rw-rw-   0 root         (0) root         (0)    29498 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/packet_data/packet_list.py
--rw-rw-rw-   0 root         (0) root         (0)    10335 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/packet_data/tag_collection.py
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-06 13:31:30.155662 wiliot-core-4.0.6/wiliot_core/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6045 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)    10577 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/utils/update_wiliot_packages.py
--rw-rw-rw-   0 root         (0) root         (0)    12888 2023-03-06 13:31:10.000000 wiliot-core-4.0.6/wiliot_core/utils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-03-06 13:31:29.000000 wiliot-core-4.0.6/wiliot_core/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-06 13:31:30.147662 wiliot-core-4.0.6/wiliot_core.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     2483 2023-03-06 13:31:29.000000 wiliot-core-4.0.6/wiliot_core.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1439 2023-03-06 13:31:30.000000 wiliot-core-4.0.6/wiliot_core.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-06 13:31:29.000000 wiliot-core-4.0.6/wiliot_core.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-06 13:31:29.000000 wiliot-core-4.0.6/wiliot_core.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-03-06 13:31:29.000000 wiliot-core-4.0.6/wiliot_core.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-06 13:31:29.000000 wiliot-core-4.0.6/wiliot_core.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:27:47.389662 wiliot-core-4.0.8/
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     3247 2023-04-25 08:27:47.389662 wiliot-core-4.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2735 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     7184 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-25 08:27:47.389662 wiliot-core-4.0.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1834 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:27:47.381662 wiliot-core-4.0.8/wiliot_core/
+-rw-rw-rw-   0 root         (0) root         (0)     4596 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:27:47.381662 wiliot-core-4.0.8/wiliot_core/local_gateway/
+-rw-rw-rw-   0 root         (0) root         (0)     4010 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13748 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/continuous_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)    12763 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/custom_energy_pattern.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:27:47.381662 wiliot-core-4.0.8/wiliot_core/local_gateway/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     4010 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/examples/local_gateway_basic_example.py
+-rw-rw-rw-   0 root         (0) root         (0)    86026 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_core.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:27:47.385662 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/
+-rw-rw-rw-   0 root         (0) root         (0)   253422 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/3.8.14_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   448599 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/3.8.14_sd_bl_gw_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   122153 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/4.0.16_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   317338 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/4.0.16_sd_bl_gw_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   229471 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/4.0.4_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)   424656 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/4.0.4_sd_bl_gw_app.zip
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)  1242814 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/wifi_3.8.14.hex
+-rw-rw-rw-   0 root         (0) root         (0)  1176930 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.4.hex
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:27:47.389662 wiliot-core-4.0.8/wiliot_core/packet_data/
+-rw-rw-rw-   0 root         (0) root         (0)     4010 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/packet_data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26863 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/packet_data/packet.py
+-rw-rw-rw-   0 root         (0) root         (0)    29498 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/packet_data/packet_list.py
+-rw-rw-rw-   0 root         (0) root         (0)    10335 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/packet_data/tag_collection.py
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:27:47.389662 wiliot-core-4.0.8/wiliot_core/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6045 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     9296 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/utils/release_for_partners.py
+-rw-rw-rw-   0 root         (0) root         (0)    14010 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/utils/update_wiliot_packages.py
+-rw-rw-rw-   0 root         (0) root         (0)    12888 2023-04-25 08:27:30.000000 wiliot-core-4.0.8/wiliot_core/utils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-25 08:27:46.000000 wiliot-core-4.0.8/wiliot_core/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:27:47.381662 wiliot-core-4.0.8/wiliot_core.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     3247 2023-04-25 08:27:46.000000 wiliot-core-4.0.8/wiliot_core.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2023-04-25 08:27:47.000000 wiliot-core-4.0.8/wiliot_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-25 08:27:46.000000 wiliot-core-4.0.8/wiliot_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-25 08:27:46.000000 wiliot-core-4.0.8/wiliot_core.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-04-25 08:27:46.000000 wiliot-core-4.0.8/wiliot_core.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-25 08:27:46.000000 wiliot-core-4.0.8/wiliot_core.egg-info/top_level.txt
```

### Comparing `wiliot-core-4.0.6/LICENSE` & `wiliot-core-4.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.6/PKG-INFO` & `wiliot-core-4.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-core
-Version: 4.0.6
+Version: 4.0.8
 Summary: A library for interacting with Wiliot's private core functions
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -56,14 +56,29 @@
 * [gateway communication](wiliot_core/local_gateway/examples)
 * [packet data](wiliot_core/packet_data) (at the end of each script)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
+Version 4.0.8:
+-----------------
+* continuous listener as multi-processes:
+    * add option to specify log path and communicate reading error using event
+    * connect to gw in a more robust way including printing exceptions if needed
+* local gw core:
+    * connect only to “Silicon Lab”/"CP210.." ports (Wiliot's gw driver)
+    * added a function to check gw response using version command check_gw_responds including is_gw_alive function
+    * better handling ACK msg from the GW
+    * get reading status function get_read_error_status. 
+    * better stop gw app including writing a log if no ACK was received for the cancel command
+    * add new GW FW version
+* packet:
+    * add new function to packet to retrieve basic data: get_adva, get_flow, get_rssi
+
 
 Version 4.0.6:
 -----------------
 * First version
 
 
 The package previous content was published under the name 'wiliot' package.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wiliot-core-4.0.6/README.md` & `wiliot-core-4.0.8/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -39,14 +39,29 @@
 * [gateway communication](wiliot_core/local_gateway/examples)
 * [packet data](wiliot_core/packet_data) (at the end of each script)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
+Version 4.0.8:
+-----------------
+* continuous listener as multi-processes:
+    * add option to specify log path and communicate reading error using event
+    * connect to gw in a more robust way including printing exceptions if needed
+* local gw core:
+    * connect only to “Silicon Lab”/"CP210.." ports (Wiliot's gw driver)
+    * added a function to check gw response using version command check_gw_responds including is_gw_alive function
+    * better handling ACK msg from the GW
+    * get reading status function get_read_error_status. 
+    * better stop gw app including writing a log if no ACK was received for the cancel command
+    * add new GW FW version
+* packet:
+    * add new function to packet to retrieve basic data: get_adva, get_flow, get_rssi
+
 
 Version 4.0.6:
 -----------------
 * First version
 
 
 The package previous content was published under the name 'wiliot' package.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wiliot-core-4.0.6/bitbucket-pipelines.yml` & `wiliot-core-4.0.8/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.6/setup.py` & `wiliot-core-4.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,13 @@
                      'setuptools_scm',
                      'pyserial',
                      'pc_ble_driver_py',
                      'nrfutil',
                      'pandas',
                      'numpy',
                      'PySimpleGUI',
-                     'appdirs',
-                     'wiliot-api'
+                     'appdirs'
                  ],
                  zip_safe=False,
                  python_requires='>=3.6',
                  include_package_data=True,
                  )
```

### Comparing `wiliot-core-4.0.6/wiliot_core/__init__.py` & `wiliot-core-4.0.8/wiliot_core/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.6/wiliot_core/local_gateway/__init__.py` & `wiliot-core-4.0.8/wiliot_core/local_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.6/wiliot_core/local_gateway/continuous_listener.py` & `wiliot-core-4.0.8/wiliot_core/local_gateway/continuous_listener.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,56 +88,62 @@
     write - write command to serial, return the gw respond (add to rsp q)
     read - read specific msg from serial, return the gw respond (add to rsp/packet q)
     disconnect - close serial port, return if connected (connected event)
     reset - reset serial buffer
     check - number of bytes waiting in buffer (n_bytes Value
     stop - stop the process
     """
-    def __init__(self, cmd_q, gw_rsp_q, packets_q, change_connection_status):
+    def __init__(self, cmd_q, gw_rsp_q, packets_q, change_connection_status, error_event, log_dir_path=None):
         """
 
-        :param cmd_q:
+        :param cmd_q: queue of commands to the listener including cmd = the state in the state machine,
+                      and data if needed
         :type cmd_q: Queue
-        :param gw_rsp_q:
+        :param gw_rsp_q: the listener put into this queue the gw responds
         :type gw_rsp_q: Queue
-        :param packets_q:
+        :param packets_q: the listener put into this queue the packets received from gw
         :type packets_q: Queue
-        :param change_connection_status:
-        :type connected_event: Event
+        :param change_connection_status: listener set this event if there was a change in the connection status
+        :type change_connection_status: Event
+        :param error_event: listener set this event if an error occurs during run
+        :type error_event: Event
+        :param log_dir_path: the logging directory
+        :type log_dir_path: str
         """
         # serial port variables:
         self._comPortObj = None
         self.write_wait_time = 0.001  # [sec]
         self.cmd_q = cmd_q
         self.gw_rsp_q = gw_rsp_q
         self.packets_q = packets_q
         self.change_connection_status = change_connection_status
+        self.error_event = error_event
         self.connected = False
         self.gw_start_time = datetime.datetime.now()
         self.buf = b''
 
         # set logging:
         self.logger = logging.getLogger('WiliotListener')
-        self.logger_path = None
-        self.set_logger()
+        self.set_logger(log_dir_path)
         # start run:
         self.run_sm()
 
-    def set_logger(self):
+    def set_logger(self, logger_dir_path):
         formatter = logging.Formatter('%(asctime)s,%(msecs)d %(name)s %(levelname)s: %(message)s', '%Y-%m-%d %H:%M:%S')
         stream_handler = logging.StreamHandler()
         stream_handler.setLevel(logging.INFO)
         stream_handler.setFormatter(formatter)
-        wiliot_dir = WiliotDir()
-        logger_path = os.path.join(wiliot_dir.get_wiliot_root_app_dir(), 'wiliot_continuous_listener')
-        if not os.path.isdir(logger_path):
-            os.mkdir(logger_path)
+        if logger_dir_path is None:
+            wiliot_dir = WiliotDir()
+            logger_dir_path = os.path.join(wiliot_dir.get_wiliot_root_app_dir(), 'wiliot_continuous_listener')
+        if not os.path.isdir(logger_dir_path):
+            os.mkdir(logger_dir_path)
         logger_name = 'listener_log_{}.log'.format(datetime.datetime.now().strftime('%Y%m%d_%H%M%S'))
-        self.logger_path = os.path.join(logger_path, logger_name)
-        file_handler = logging.FileHandler(self.logger_path, mode='a')
+        logger_path = os.path.join(logger_dir_path, logger_name)
+        file_handler = logging.FileHandler(logger_path, mode='a')
         file_formatter = logging.Formatter('%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s', '%H:%M:%S')
         file_handler.setFormatter(file_formatter)
         self.logger.addHandler(file_handler)
         self.logger.addHandler(stream_handler)
         self.logger.setLevel(logging.DEBUG)
 
     def run_sm(self):
@@ -149,14 +155,15 @@
                 cmd = None
                 state = SerialProcessState.IDLE
 
             if state == SerialProcessState.CONNECT:
                 self.connect(port=cmd['data']['port'], baud=cmd['data']['baud'])
             elif state == SerialProcessState.WRITE:
                 self.write(gw_cmd=cmd['data']['gw_cmd'])
+                self.read()
             elif state == SerialProcessState.READ:
                 self.gw_start_time = datetime.datetime.now()
                 self.read()
             elif state == SerialProcessState.DISCONNECT:
                 self.disconnect()
             elif state == SerialProcessState.RESET:
                 self.reset()
@@ -172,23 +179,27 @@
                     continue
         self.logger.log(logging.INFO, 'serial process state machine is done')
 
     def connect(self, port, baud):
         if self.connected:
             self.change_connection_status.set()
         else:
-            self._comPortObj = serial.Serial(port, baud, timeout=0.001)
-            for i in range(5):
-                if self._comPortObj.isOpen():
-                    break
-                time.sleep(0.1)
+            try:
                 self._comPortObj = serial.Serial(port, baud, timeout=0.001)
-            if self._comPortObj.isOpen():
-                self.change_connection_status.set()
-                self.connected = True
+                for i in range(5):
+                    if self._comPortObj.isOpen():
+                        break
+                    time.sleep(0.1)
+                    self._comPortObj = serial.Serial(port, baud, timeout=0.001)
+                if self._comPortObj.isOpen():
+                    self.change_connection_status.set()
+                    self.connected = True
+                    self.logger.log(logging.INFO, 'Connected to port: {}'.format(port))
+            except Exception as e:
+                self.logger.log(logging.WARNING, 'Exception during connection to port {}: {}'.format(port, e))
 
     def disconnect(self):
         if self.connected:
             try:
                 self._comPortObj.close()
                 self.change_connection_status.set()
                 self.connected = False
@@ -249,19 +260,20 @@
                         self.gw_rsp_q.put(msg_dict)
                     self.buf = b''
 
                 # check buffer status:
                 if self._comPortObj.in_waiting > 2 * packet_bytes:
                     self.logger.log(logging.WARNING, 'buffer contains {} bytes'.format(self._comPortObj.in_waiting))
             except serial.SerialException as e:
-                self.logger.log(logging.WARNING, ' problem during reading: {}'.format(e))
+                self.logger.log(logging.WARNING, ' Serial Exception during reading: {}'.format(e))
                 if 'PermissionError' in str(e):
                     self.logger.log(logging.WARNING, 'disconnecting')
                     self.disconnect()
             except Exception as e:
+                self.error_event.set()
                 self.logger.log(logging.WARNING, ' problem during reading: {}\nreset buffer'.format(e))
                 self.reset()
 
 
 if __name__ == '__main__':
     commands = Queue(maxsize=100)
     gw_rsp = Queue(maxsize=100)
```

### Comparing `wiliot-core-4.0.6/wiliot_core/local_gateway/custom_energy_pattern.py` & `wiliot-core-4.0.8/wiliot_core/local_gateway/custom_energy_pattern.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.6/wiliot_core/local_gateway/examples/__init__.py` & `wiliot-core-4.0.8/wiliot_core/local_gateway/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.6/wiliot_core/local_gateway/examples/local_gateway_basic_example.py` & `wiliot-core-4.0.8/wiliot_core/local_gateway/examples/local_gateway_basic_example.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.6/wiliot_core/local_gateway/local_gateway_core.py` & `wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,14 +109,15 @@
     {'abs_power': 6, 'gw_output_power': 'neg12dBm', 'bypass_pa': '0'},
     {'abs_power': 10, 'gw_output_power': 'neg8dBm', 'bypass_pa': '0'},
     {'abs_power': 15, 'gw_output_power': 'neg4dBm', 'bypass_pa': '0'},
     {'abs_power': 20, 'gw_output_power': 'pos0dBm', 'bypass_pa': '0'},
     {'abs_power': 21, 'gw_output_power': 'pos2dBm', 'bypass_pa': '0'},
     {'abs_power': 22, 'gw_output_power': 'pos3dBm', 'bypass_pa': '0'}
 ]
+cmds_no_default_ack = ['print', 'set_energizing_pattern', 'move_to_bootloader', 'version', 'pce', 'trigger_pl']
 
 
 class ConfigParam:
     def __init__(self):
         self.energy_pattern = None
         self.received_channel = None
         self.time_profile_on = None
@@ -210,15 +211,15 @@
     :type auto_connect: bool
     :param auto_connect: If TRUE, connect automatically to the GW.
 
     :exception during open serial port process
     """
 
     def __init__(self, baud=921600, port=None, auto_connect=False, lock_print=None, logger_name=None, verbose=True,
-                 socket_host='localhost', socket_port=2022, is_multi_processes=False):
+                 socket_host='localhost', socket_port=2022, is_multi_processes=False, log_dir_for_multi_processes=None):
         """
         :type baud: int
         :param baud: the GW baud rate
         :type port: str
         :param port: The GW port if it is already know.
         :type auto_connect: bool
         :param auto_connect: If TRUE, connect automatically to the GW.
@@ -243,14 +244,15 @@
         else:
             self._lock_print = lock_print
 
         # flag variable:
         self._is_running_analysis = False
         self.available_data = False
         self.connected = False
+        self.reading_exception = False
         self.verbose = verbose
 
         # serial port variables:
         self._comPortObj = None
         self.port = ''
         self.baud = baud
         self.write_wait_time = 0.001  # [sec]
@@ -268,28 +270,33 @@
         # multi-processing
         self.multi_process = is_multi_processes
         if self.multi_process:
             cmd_serial_process_q = mp.Queue(maxsize=100)
             com_rsp_str_input_q = mp.Queue(maxsize=100)
             com_pkt_str_input_q = mp.Queue(maxsize=1000)
             connected_event = mp.Event()
+            read_error_event = mp.Event()
             self._port_listener_thread = mp.Process(target=SerialProcess,
                                                     args=(cmd_serial_process_q,
                                                           com_rsp_str_input_q,
                                                           com_pkt_str_input_q,
-                                                          connected_event))
+                                                          connected_event,
+                                                          read_error_event,
+                                                          log_dir_for_multi_processes))
             self._port_listener_thread.start()
 
             self.cmd_serial_process_q = cmd_serial_process_q
             self.com_rsp_str_input_q = com_rsp_str_input_q
             self.com_pkt_str_input_q = com_pkt_str_input_q
             self.connected_event = connected_event
+            self.read_error_event = read_error_event
         else:
             self.cmd_serial_process_q = None
             self.connected_event = None
+            self.read_error_event = None
             self.com_rsp_str_input_q = Queue(maxsize=100)
             self.com_pkt_str_input_q = Queue(maxsize=1000)
 
         self.start_time_lock = threading.Lock()
         self.stop_listen_event = threading.Event()
 
         self.continuous_listener_enabled = False
@@ -322,17 +329,19 @@
             if self.open_port(port, self.baud):
                 self._printing_func("connection was established: {}={}".format(self.hw_version, self.sw_version),
                                     'init')
                 self.connected = True
                 return
 
         # if port is None - let's search for all available ports
-        self.available_ports = [s.device for s in serial.tools.list_ports.comports()]
+        self.available_ports = [s.device for s in serial.tools.list_ports.comports()
+                                if 'Silicon Labs' in s.description or 'CP210' in s.description]
         if len(self.available_ports) == 0:
-            self.available_ports = [s.name for s in serial.tools.list_ports.comports()]
+            self.available_ports = [s.name for s in serial.tools.list_ports.comports()
+                                    if 'Silicon Labs' in s.description or 'CP210' in s.description]
             if len(self.available_ports) == 0:
                 self._printing_func("no serial ports were found. please check your connections", "init", True)
                 return
 
         # if user want to connect automatically - connecting to the first available COM with valid gw version
         if auto_connect:
             for p in self.available_ports:
@@ -344,14 +353,44 @@
                         break
                 except Exception as e:
                     self._printing_func("tried to connect {} but failed, moving to the next port".format(p), 'init')
 
     def set_verbosity(self, verbose=True):
         self.verbose = verbose
 
+    def check_gw_responds(self):
+        if self.multi_process:
+            max_try = 5  # [sec] <~4 seconds
+            version_msg = ''
+            self.reset_buffer()
+            for i in range(max_try):  # try to get ping from gw
+                self.cmd_serial_process_q.put({'cmd': SerialProcessState.WRITE, 'data': {'gw_cmd': '!version'}})
+                try:
+                    version_msg = self.com_rsp_str_input_q.get(timeout=1)
+                    version_msg = version_msg['raw']
+                    if 'WILIOT_GW' in version_msg:
+                        break
+                    elif version_msg != '':
+                        self._printing_func("got the following msg, while waiting for version: {}".format(version_msg),
+                                            'check_gw_responds')
+                except Empty:
+                    continue
+            self.clear_rsp_str_input_q()
+        else:
+            self._write("!version")
+            time.sleep(0.1)
+            # read GW version:
+            version_msg = self.read_specific_message(msg='SW_VER', read_timeout=3)
+
+        return version_msg
+
+    def is_gw_alive(self):
+        gw_ver = self.check_gw_responds()
+        return 'WILIOT_GW' in gw_ver
+
     def open_port(self, port, baud):
         """
         Open a serial connection according to the port and baud
         If the port is open, The GW version is read (All last messages are read since some messages can contains the tag
         packets)
         If the version name is valid (contains 'SW_VER') the GW type (BLE/WIFI/LTI) is saved together with the software
         version. If the version name is invalid, closing the serial port.
@@ -362,48 +401,36 @@
         :param baud: the GW baud rate - mandatory
 
         :return: TRUE if GW is connection and FALSE otherwise
 
         :exception:
         * could not open port 'COMX'... - make sure the baud rate and port are correct
         """
-        if self.connected:
+        if self.is_connected():
             self._printing_func("GW is already connected", 'open_port')
             return self.connected
         # open UART connection
         try:
             if self.multi_process:
                 version_msg = ''
                 self.cmd_serial_process_q.put({'cmd': SerialProcessState.CONNECT, 'data': {'port': port, 'baud': baud}})
-                self.connected_event.wait(2)
+                self.connected_event.wait(5)  # wait for few seconds is needed if the gw is already sending packets
                 if self.connected_event.is_set():
+                    self.connected = True
                     self.connected_event.clear()
-                    version_msg = ''
-                    for i in range(5):  # try to get ping from gw
-                        self.cmd_serial_process_q.put({'cmd': SerialProcessState.WRITE, 'data': {'gw_cmd': '!version'}})
-                        try:
-                            version_msg = self.com_rsp_str_input_q.get(timeout=1)
-                            if 'WILIOT_GW' in version_msg['raw']:
-                                version_msg = version_msg['raw']
-                                break
-                        except Empty:
-                            continue
-                    self.clear_rsp_str_input_q()
+                    version_msg = self.check_gw_responds()
                 else:
                     self._printing_func('connection failed', 'open_port')
                     self.cmd_serial_process_q.put({'cmd': SerialProcessState.DISCONNECT})
             else:
                 self._comPortObj = serial.Serial(port, baud, timeout=0.1)
                 time.sleep(0.5)
                 if self._comPortObj.isOpen():
                     self.connected = True
-                    self._write("!version")
-                    time.sleep(0.1)
-                    # read GW version:
-                    version_msg = self.read_specific_message(msg='SW_VER', read_timeout=3)
+                    version_msg = self.check_gw_responds()
                 else:
                     self.connected = False
                     return self.connected
 
             if 'WILIOT_GW' in version_msg:
                 self.sw_version = version_msg.split('=', 1)[1].split(' ', 1)[0]
                 self.hw_version = version_msg.split('=', 1)[0]
@@ -412,14 +439,15 @@
                 self.update_version(check_only=True)
                 return self.connected
             else:
                 # we read all the last lines and cannot find a valid version name
                 self._printing_func('serial connection was established but gw version could not be read.\n'
                                     'Check your baud rate and port.\nDisconnecting and closing port', 'open_port')
                 self.close_port(True)
+                self.connected = False
                 return self.connected
 
         except Exception as e:
             self._printing_func('connection failed', 'open_port')
             raise e
 
     def _write(self, cmd):
@@ -456,66 +484,77 @@
                                         .format(e), 'write')
                     raise e
         else:
             self._printing_func("gateway is not connected. please initiate connection and then send a command", 'write')
         self.quick_wait()  # wait to prevent buffer overflow:
 
     def write(self, cmd, with_ack=False, max_time=0.01):
-        data_in = self.write_get_response(cmd)
+        if not self.is_connected():
+            self._printing_func("gateway is not connected. write can not be done", 'write')
+        data_in, got_ack = self.write_get_response(cmd)
         if with_ack:
-            if data_in is not None and (data_in['raw'] == '' or 'unsupported' in data_in['raw'].lower()):
+            if data_in is not None and not got_ack:
                 t_i = datetime.datetime.now()
                 dt = 0
-                while (data_in['raw'] == '' or 'unsupported' in data_in['raw'].lower()) and dt < max_time:
-                    data_in = self.write_get_response(cmd)
+                while not got_ack and dt < max_time:
+                    data_in, got_ack = self.write_get_response(cmd, need_to_clear=False)
                     dt = (datetime.datetime.now() - t_i).total_seconds()
+
                 self.clear_rsp_str_input_q()
+        # print msg:
+        msg = "For cmd {} GW responded with {}".format(cmd, data_in['raw'])
+        if "UNSUPPORTED" in data_in['raw'].upper():
+            self._printing_func(f"GW responded unsupported to cmd {cmd}, response: {data_in}",
+                                'write', log_level=logging.WARNING)
+        elif got_ack:
+            self._printing_func(msg, 'write', log_level=logging.INFO)
+        else:
+            self._printing_func(f"GW did not respond with command complete event. cmd: {cmd}, response: {data_in}",
+                                'write', log_level=logging.INFO)
         return data_in
 
-    def write_get_response(self, cmd):
-        self.clear_rsp_str_input_q()
+    def write_get_response(self, cmd, need_to_clear=True):
+        if need_to_clear:
+            self.clear_rsp_str_input_q()
         if self.multi_process:
             self.cmd_serial_process_q.put({'cmd': SerialProcessState.WRITE, 'data': {'gw_cmd': cmd}})
         else:
             self._write(cmd)
         if self.continuous_listener_enabled or self.multi_process:
             try:
                 data_in = self.com_rsp_str_input_q.get(timeout=0.1)
             except Empty as e:
                 data_in = {'raw': '', 'time': 0}
+                is_ack = False
+                return data_in, is_ack
 
-            msg = "GW write_get_response {} respond with {}".format(cmd, data_in['raw'])
-            #             self._printing_func(
-            #                 msg, "write_get_response {}".format(cmd),"write_get_response")
-            self._printing_func(msg, 'write_get_response', log_level=logging.DEBUG)
-            if "UNSUPPORTED" in data_in['raw'].upper():
-                self._printing_func(f"GW respond unsupported to cmd {cmd}, response: {data_in}",
-                                    'write_get_response', log_level=logging.WARNING)
-            if "Energizing" in data_in['raw']:
+            if "energizing" in data_in['raw'].lower():
                 try:
                     data_in_2nd_row = self.com_rsp_str_input_q.get(timeout=0.01)
                     data_in['raw'] += '\n{}'.format(data_in_2nd_row['raw'])
                     data_in_3rd_row = self.com_rsp_str_input_q.get(timeout=0.01)
                     data_in['raw'] += '\n{}'.format(data_in_3rd_row['raw'])
                 except Exception as e:
                     print('could not found a second/third row to gw respond {}'.format(e))
-            if "Command Complete Event" not in data_in['raw'] and 'print' not in cmd \
-                    and "set_energizing_pattern" not in cmd and 'move_to_bootloader' not in cmd and \
-                    'WILIOT' not in data_in['raw']:
-                self._printing_func(f"GW did not respond with command complete event. cmd: {cmd}, response: {data_in}",
-                                    'write_get_response', log_level=logging.INFO)
-            return data_in
+
+            if "unsupported" in data_in['raw'].lower():
+                is_ack = False
+            else:
+                is_ack = any([s in cmd for s in cmds_no_default_ack]) or \
+                         "command complete event" in data_in['raw'].lower()
+
+            return data_in, is_ack
         else:
+            is_ack = True
             data = self.readline_from_buffer()
-            msg = "GW write_get_response {} respond with {}".format(cmd, data)
-            self._printing_func(msg, 'write_get_response', log_level=logging.DEBUG)
             self._printing_func(
-                "GW write_get_response {} is not supported without continuous_listener_enabled".format(cmd),
-                "write_get_response {}".format(cmd))
-            return {'raw': data, 'time': 0}
+                "GW write_get_response {} respond with {} is not supported "
+                "without continuous_listener_enabled".format(cmd, data),
+                "write_get_response")
+            return {'raw': data, 'time': 0}, is_ack
 
     def get_curr_timestamp_in_sec(self):
         return (datetime.datetime.now() - self.start_time).total_seconds()
 
     def read_specific_message(self, msg, read_timeout=1, clear=False):
         """
         search for specific message in the input buffer
@@ -568,14 +607,17 @@
                             return data_in
                         else:
                             if self.verbose and data_in is not None and data_in != '':
                                 self._printing_func(
                                     "Discard GW data while waiting for specific data:\n {}".format(data_in),
                                     "read_specific_message {}".format(msg))
                     except Exception as e:
+                        self.reading_exception = True
+                        self._printing_func('could not read line fro serial', func_name='read_specific_message',
+                                            log_level=logging.WARNING)
                         pass
                     dt_check_version = self.get_curr_timestamp_in_sec() - time_start_msg
 
                 # we read all the last lines and cannot find the specific message till read timeout
                 return ''
 
     def close_port(self, is_reset=False):
@@ -584,15 +626,15 @@
         Closing GW serial port
 
         :type is_reset: bool
         :param is_reset: if TRUE, running the Reset function before closing the port
         :return:
         """
         # close UART connection
-        if self.connected:
+        if self.is_connected():
             if is_reset:
                 # reset for stop receiving messages from tag.
                 try:
                     self.reset_gw()
                 except Exception as e:
                     raise e
             try:
@@ -607,27 +649,35 @@
                     self._comPortObj.close()
                     self.connected = self._comPortObj.isOpen()
             except Exception as e:
                 self._printing_func('Exception during close_port:{}'.format(e), 'close_port')
         else:
             self._printing_func('The gateway is already disconnected', 'close_port')
 
+    def get_read_error_status(self):
+        if self.multi_process:
+            self.reading_exception = self.read_error_event.is_set()
+            self.read_error_event.clear()
+        current_reading_exception = self.reading_exception
+        self.reading_exception = False  # reset flag
+        return current_reading_exception
+
     def reset_gw(self, reset_gw=True, reset_port=True):
         """
         Reset the GW serial port
         Flush and reset input buffer
 
         :type reset_gw: bool
         :param reset_gw: if True sends a reset command
         :type reset_port: bool
         :param reset_port: if True reset the serial port
         :return:
         """
         self._printing_func("reset_gw called", "reset_gw")
-        if self.connected:
+        if self.is_connected():
             if reset_port:
                 try:
                     if self.multi_process:
                         self.cmd_serial_process_q.put({'cmd': SerialProcessState.RESET})
                     else:
                         self._comPortObj.flush()
                         self.reset_buffer()
@@ -651,31 +701,35 @@
         """
         Reset input buffer of the GW serial COM and reset software queue (raw data and processed data)
         :return:
         """
         # reset software buffers:
         self.available_data = False
         # reset serial input buffer:
-        if self.connected:
+        if self.is_connected():
             # reset input buffer
             if self.multi_process:
                 self.cmd_serial_process_q.put({'cmd': SerialProcessState.RESET})
             else:
                 try:
                     if self._comPortObj.in_waiting:
                         self._comPortObj.reset_input_buffer()
                 except Exception as e:
-                    self._printing_func("Exception during reset_buffer:\n{}".format(e), 'reset_buffer')
-                    raise
-
+                    self._printing_func("Exception during reset_buffer:\n{}".format(e), 'reset_buffer',
+                                        log_level=logging.WARNING)
+                    raise e
+        else:
+            self._printing_func("GW is disconnected, can not reset buffer", 'reset_buffer')
         self.clear_pkt_str_input_q()
         self.clear_rsp_str_input_q()
 
     def stop_gw_app(self):
-        self.write('!cancel', with_ack=True)
+        rsp = self.write('!cancel', with_ack=True, max_time=0.100)
+        if 'Command Complete Event' not in rsp['raw']:
+            self._printing_func("Did not get ACK from GW to stop txrx: {}".format(rsp), 'stop_gw_app')
         self.reset_buffer()
 
     def config_gw(self, filter_val=None, pacer_val=None, energy_pattern_val=None, time_profile_val=None,
                   beacons_backoff_val=None, received_channel=None,
                   output_power_val=None, effective_output_power_val=None, sub1g_output_power_val=None,
                   bypass_pa_val=None, pl_delay_val=None, rssi_thr_val=None,
                   max_wait=1, check_validity=False, check_current_config_only=False, start_gw_app=True, with_ack=False,
@@ -1046,15 +1100,15 @@
         return self.config_param, gateway_output  # return the config parameters
 
     def check_current_config(self):
         """
         print the current gw configuration
         :return:
         """
-        data_in = self.write("!print_config")
+        data_in = self.write("!print_config_extended")
         # read current configuration:
         if data_in != '':
             self._printing_func("current gateway configuration:\n{}".format(data_in), 'config_gw')
             return
         else:
             # we read all the last lines and cannot find a valid message
             self._printing_func("cannot read gateway configuration", 'config_gw')
@@ -1113,15 +1167,15 @@
                                          f"version file {new_version_path}")
         else:
             new_version_path = '"{}"'.format(versions_path)  # to avoid failure when path contains spaces
 
         # a version need to be updated:
 
         # change the GW to bootloader state
-        if self.connected:
+        if self.is_connected():
             self.write('!move_to_bootloader')
             time.sleep(0.1)
             self.close_port()
 
             # run the nRF Util to burn the version:
             time.sleep(.1)
             # wait until burn was completed
@@ -1179,20 +1233,28 @@
             self.init_socket_connection_thread.join()
 
     def _printing_func(self, str_to_print, func_name="MISSING", is_info=False, log_level=logging.INFO):
         if self.verbose or not is_info:
             with self._lock_print:
                 self.logger.log(log_level, 'GW API: {}: {}'.format(func_name, str_to_print.strip()))
 
+    def is_connected(self):
+        if self.multi_process:
+            connection_status_changed = self.connected_event.is_set()
+            if connection_status_changed:
+                self.connected = not self.connected
+                self.connected_event.clear()
+        return self.connected
+
     def get_connection_status(self, check_port=False):
         """
         :return: if gateway is connected, return True, the serial port and baud rate used for the connection.
                  if not, return False, and None for port and baud
         """
-        if self.connected:
+        if self.is_connected():
             if check_port:
                 try:
                     self._write("!version")
                     version_msg = self.read_specific_message(msg='SW_VER', read_timeout=3)
                     # read GW version:
                     if version_msg != '':
                         self.sw_version = version_msg.split('=', 1)[1].split(' ', 1)[0]
@@ -1392,15 +1454,15 @@
                     buf += data
 
                 # complete the loop with no exceptions
                 consecutive_exception_counter = 0
 
             except Exception as e:
                 # saving the first exception
-
+                self.reading_exception = True
                 if consecutive_exception_counter == 0:
                     self.exceptions_threads[0] = str(e)
                 self._printing_func("received: {}\ncomPortListener Exception({}/10):\n{}".
                                     format(data, consecutive_exception_counter, e), 'run_packet_listener')
                 consecutive_exception_counter = consecutive_exception_counter + 1
                 buf = b''
                 if consecutive_exception_counter > 10:
@@ -1752,7 +1814,20 @@
                 elif data == '':
                     done = True
             except Exception as e:
                 self._printing_func(f"Failed to readline with exception {str(e)}")
             if not done:
                 time.sleep(0.1)
         return msg
+
+
+if __name__ == '__main__':
+    print(datetime.datetime.now())
+    gw = WiliotGateway(auto_connect=True, is_multi_processes=True)
+    if gw.is_connected():
+        # gw.start_continuous_listener()
+        gw.reset_gw(reset_port=False)
+        print(f'is gw alive {gw.is_gw_alive()}')
+        print(gw.write('!set_tester_mode 1', with_ack=True))
+        gw.config_gw(energy_pattern_val=18, time_profile_val=[5, 15], effective_output_power_val=22)
+    print(datetime.datetime.now())
+    gw.exit_gw_api()
```

### Comparing `wiliot-core-4.0.6/wiliot_core/local_gateway/local_gateway_versions/3.8.14_app.zip` & `wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/3.8.14_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.6/wiliot_core/local_gateway/local_gateway_versions/3.8.14_sd_bl_gw_app.zip` & `wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/3.8.14_sd_bl_gw_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.6/wiliot_core/local_gateway/local_gateway_versions/4.0.4_app.zip` & `wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/4.0.4_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.6/wiliot_core/local_gateway/local_gateway_versions/4.0.4_sd_bl_gw_app.zip` & `wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/4.0.4_sd_bl_gw_app.zip`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.6/wiliot_core/local_gateway/local_gateway_versions/wifi_3.8.14.hex` & `wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/wifi_3.8.14.hex`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.6/wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.4.hex` & `wiliot-core-4.0.8/wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.4.hex`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.6/wiliot_core/packet_data/__init__.py` & `wiliot-core-4.0.8/wiliot_core/packet_data/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.6/wiliot_core/packet_data/packet.py` & `wiliot-core-4.0.8/wiliot_core/packet_data/packet.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 #     (C) EVEN IF ANY REMEDY FAILS OF ITS ESSENTIAL PURPOSE.
 #  """
 
 import numpy as np
 import pandas as pd
 import copy
 import re
+from enum import Enum
 
 packet_data_dict = {
     'adv_address': (0, 6),
     'en': (6, 1),
     'type': (7, 1),
     'data_uid': (8, 2),
     # 'group_id': (10, 3), #group id is only 22bits, we have a dedicated function for it
@@ -90,24 +91,35 @@
 packet_tag_length = 74
 rssi_char_last_index = 76
 stat_param_last_index = 80
 
 max_stat_param_val = 65535  # 2 bytes
 
 
+class InlayTypes(Enum):
+    TEO_086 = '086'
+    TIKI_096 = '096'
+    TIKI_099 = '099'
+    BATTERY_107 = '107'
+    TIKI_117 = '117'
+    TIKI_118 = '118'
+    TIKI_121 = '121'
+    TIKI_122 = '122'
+
+
 class Packet(object):
     """
     Wiliot Packet Object
 
         :param raw_packet: the raw packet to create a Packet object
         :type raw_packet: str or dict
 
         :return:
     """
-    
+
     def __init__(self, raw_packet, time_from_start=None, custom_data=None, inlay_type=None):
         """
         :param raw_packet:
         :type raw_packet: str or dict
         :param time_from_start: the time when the packet was received according to the gw timer
         :type time_from_start: float
         :param custom_data: the packet custom data as dictionary
@@ -121,15 +133,15 @@
                 get_packet_content = self.get_packet_content(raw_packet['packet'], get_gw_data=True)
                 self.packet_data = {
                     'raw_packet': self.get_packet_content(raw_packet['packet']),
                     'adv_address': raw_packet['adv_address'],
                     'decrypted_packet_type': (int(raw_packet['packet'][24:25], 16) & 0xc) >> 2,
                     'group_id': self.extract_group_id(raw_packet['group_id'])
                 }
-                
+
                 self.gw_data = {
                     'gw_packet': np.array(get_packet_content[packet_tag_length:]),
                     'rssi': np.array(raw_packet['rssi']),
                     'stat_param': np.array(raw_packet['stat_param']),  # gw_time
                     'time_from_start': np.array(raw_packet['time_from_start']),  # pc_time
                     'counter_tag': np.array(raw_packet['counter_tag']),
                     'is_valid_tag_packet': np.array(raw_packet['is_valid_tag_packet']),
@@ -141,61 +153,61 @@
         elif type(raw_packet) is str:
             try:
                 if not any(ext in raw_packet for ext in ['user_event', 'Command Complete Event']):
                     packet_data = self.get_packet_content(raw_packet)
                     raw_packet = self.get_packet_content(raw_packet, get_gw_data=True)
                     rssi_hex = raw_packet[packet_tag_length:rssi_char_last_index]
                     stat_param_hex = raw_packet[rssi_char_last_index:stat_param_last_index]
-                    
+
                     self.packet_data = {
                         'raw_packet': packet_data,
                         'adv_address': packet_data[:12],
                         'decrypted_packet_type': (int(packet_data[24:25], 16) & 0xc) >> 2,
                         'group_id': self.extract_group_id(packet_data[20:26]),
                     }
-                    
+
                     rssi_in = np.array(float('nan'))
                     stat_param_in = np.array(float('nan'))
                     if rssi_hex != '':
                         rssi_in = np.array(int(rssi_hex, base=16))
                     if stat_param_hex != '':
                         stat_param_in = np.array(int(stat_param_hex, base=16))
                     self.gw_data = {
                         'gw_packet': np.array(raw_packet[packet_tag_length:]),
                         'rssi': rssi_in,
                         'stat_param': stat_param_in,
                         'time_from_start': np.array(time_from_start),
                         'counter_tag': np.array(float('nan')),
                         'is_valid_tag_packet': np.array(float('nan')),
                     }
-                    
+
                     self.gw_process = False
                     self.is_valid_packet = True
                 else:
                     self.is_valid_packet = False
             except Exception as e:
                 print('got corrupted packet: {}'.format(raw_packet))
         self.decoded_data = {}
         if custom_data is not None:
             self.custom_data = custom_data
         else:
             self.custom_data = {}
         self.inlay_type = inlay_type
         if self.is_valid_packet:
-            
+
             self.packet_data['flow_ver'] = hex(
                 int(self.packet_data['adv_address'][0:2] + self.packet_data['adv_address'][-2:], 16))
-            
+
             self.packet_data['test_mode'] = 0
             flow_version = hex(int(self.packet_data['flow_ver'], 16))
-            
+
             for key in packet_data_dict.keys():
                 packet_data_value = self.get_attribute(self.packet_data['raw_packet'], packet_data_dict.get(key))
                 self.packet_data[key] = packet_data_value
-            
+
             if flow_version < hex(0x42c):
                 if 'FFFFFFFF' in self.packet_data['adv_address']:
                     self.packet_data['test_mode'] = 1
             elif flow_version < hex(0x500):
                 if self.packet_data['adv_address'].startswith('FFFF') or self.packet_data['adv_address'].endswith(
                         'FFFF'):
                     self.packet_data['test_mode'] = 1
@@ -208,43 +220,43 @@
                     if tx_lpm_hpm == 0:
                         self.decoded_data['tx_lpm_hpm_str'] = 'LPM'
                     else:
                         self.decoded_data['tx_lpm_hpm_str'] = 'HPM'
                     # battery mode:
                     battery_tag_ind = (self.packet_data['decrypted_packet_type'] & 2) >> 1
                     self.decoded_data['battery_tag_ind'] = battery_tag_ind
-    
+
     def __len__(self):
         """
         gets number of sprinkler occurrences in packet
         """
         return self.gw_data['rssi'].size
-    
+
     def __eq__(self, packet):
         """
         packet comparison
         """
         if self.is_same_sprinkler(packet):
             if packet.gw_data['gw_packet'].item() == self.gw_data['gw_packet'].item():
                 return True
         return False
-    
+
     def __str__(self):
         """
         packet print method
         """
         return str(
             'packet_data={packet_data}, gw_data={gw_data}'.format(packet_data=self.packet_data, gw_data=self.gw_data))
-    
+
     def is_packet_from_bridge(self):
         return self.packet_data['raw_packet'][0] != '0'
-    
+
     def get_payload(self):
         return self.packet_data['raw_packet'][16:74]
-    
+
     def extract_group_id(self, raw_group_id, zero_bits=None, num_char=6):
         """
         extract group id from the raw group id packet
         :param raw_group_id: as it received by the gw
         :type raw_group_id: str
         :param zero_bits: number of bits from the group id that were taken to other feauture an should be ignored
         :type zero_bits: list
@@ -261,136 +273,147 @@
         b = self.hex2bin(raw_group_id)
         if zero_bits is not None:
             b_list = list(b)
             for z in zero_bits:
                 b_list[z] = '0'
             b = ''.join(b_list)
         return hex(int(b, 2))[2:].zfill(num_char)
-    
+
     @staticmethod
     def hex2bin(hex, min_dig=0, zfill=True):
         b = bin(int(hex, 16))[2:]
         if zfill:
             b = bin(int(hex, 16))[2:].zfill(24)
         if len(b) > min_dig:
             pass
         else:
             b = b.zfill(min_dig)
         return b
-    
+
     def set_inlay_type(self, inlay_type):
         self.inlay_type = inlay_type
-    
+
     def is_in(self, packet):
         """
         is packet contains another packet
 
         :param packet: the other packet to verify
         :type packet: Packet
 
         :return: bool
         """
         if self.is_same_sprinkler(packet):
             if packet.gw_data['gw_packet'].item() in self.gw_data['gw_packet']:
                 return True
         return False
-    
+
     def get_packet(self):
         """
         gets raw packet string
         """
         return str(self.packet_data['raw_packet'])
-    
+
     def split_packet(self, index):
         """
         split packet by index
         """
         packet_a = self.copy()
         packet_b = self.copy()
         remain = len(self) - index
         for key in self.gw_data.keys():
             for i in range(index):
                 packet_a.gw_data[key] = np.delete(packet_a.gw_data[key], -1)
-            
+
             for i in range(remain):
                 packet_b.gw_data[key] = np.delete(packet_b.gw_data[key], 0)
-        
+
         return packet_a, packet_b
-    
+
     def copy(self):
         return copy.deepcopy(self)
-    
+
     def sort(self):
         """
         sort gw_data lists according to gw_time
         """
         isort = np.argsort(self.gw_data['stat_param'])
         for key in self.gw_data.keys():
             self.gw_data[key] = self.gw_data[key][isort]
-    
+
     def get_average_rssi(self):
         return np.average(self.gw_data['rssi'])
-    
+
     # @staticmethod
     def is_short_packet(self):
         return len(self.get_packet_string(process_packet=False)) < packet_length
-    
+
     @staticmethod
     def get_packet_content(raw_packet, get_gw_data=False):
         if 'process_packet' in raw_packet:
             raw_packet = raw_packet.split('(')[1]
             raw_packet = re.sub(r'\W+', '', raw_packet)
-        
+
         if get_gw_data:
             return raw_packet
         else:
             return raw_packet[0:packet_tag_length]
-    
+
     def get_packet_string(self, i=0, gw_data=True, process_packet=True):
         """
         gets process_packet string
         """
         process_packet_string = ['', '']
         if process_packet:
             process_packet_string = ['process_packet("', '")']
-        
+
         if not self.is_valid_packet:
             return None
         if gw_data:
             gw_data = self.gw_data['gw_packet'].take(i)
         else:
             gw_data = ''
         return '{raw_packet}{gw_data}'.format(raw_packet=self.packet_data['raw_packet'],
                                               gw_data=gw_data).join(process_packet_string)
-    
+
+    def get_adva(self):
+        return self.packet_data['adv_address']
+
+    def get_flow(self):
+        flow_version = hex(int(self.packet_data['flow_ver'], 16))
+        return flow_version
+
+
+    def get_rssi(self):
+        return str(self.gw_data['rssi'])
+
     def get_packet_data_names(self):
         """
         extract all keys name which can potentially be a column in packet df
         :return:
         :rtype: list
         """
         dict_temp = self.__dict__
         keys = list(dict_temp.keys())
         for k in dict_temp.keys():
             if isinstance(dict_temp[k], dict):
                 keys = keys + list(dict_temp[k].keys())
         return keys
-    
+
     @staticmethod
     def get_attribute(raw_packet, loc_length):
         loc = loc_length[0] * 2
         length = loc_length[1] * 2
         return raw_packet[loc:loc + length]
-    
+
     def is_same_sprinkler(self, packet):
         raw_packet = packet.packet_data['raw_packet']
         if raw_packet == self.packet_data['raw_packet']:
             return True
         return False
-    
+
     def append_to_sprinkler(self, packet, output_log=True):
         status = True
         if self.is_same_sprinkler(packet):
             for i in range(len(packet)):
                 try:
                     # stat param should be unique (time + rssi for same packet)- we make sure no duplications are added.
                     if np.take(packet.gw_data['stat_param'], i).item() not in self.gw_data['stat_param'] or \
@@ -409,15 +432,15 @@
                 except Exception as e:
                     print('Failed to add packet {} to sprinkler, exception: {}'.format(packet, str(e)))
         else:
             print('Not from the same sprinkler')
             status = False
         # self.sort()
         return status
-    
+
     def as_dict(self, sprinkler_index=None):  # None not tested
         packet_data = self.packet_data.copy()
         sprinkler_gw_data = self.gw_data.copy()
         custom_data = self.custom_data.copy()
         if sprinkler_index is not None:
             if sprinkler_index > self.gw_data['stat_param'].size:
                 return None
@@ -426,80 +449,80 @@
             for custom_attr in self.custom_data.keys():
                 custom_data[custom_attr] = np.take(self.custom_data[custom_attr], sprinkler_index)
             dict_len = 1
         else:
             dict_len = len(self)
             for k, v in packet_data.items():
                 packet_data[k] = [v] * dict_len
-        
+
         data = {**packet_data, **sprinkler_gw_data, **custom_data}
         data['gw_process'] = [self.gw_process] * dict_len  # bool should be a list for pd.DataFrame.from_dict(data)
         data['is_valid_packet'] = [self.is_valid_packet] * dict_len  # bool should be a list
         data['inlay_type'] = [self.inlay_type] * dict_len
         return data
-    
+
     def as_dataframe(self, sprinkler_index=None):
         data = self.as_dict(sprinkler_index=sprinkler_index)
         packet_df = pd.DataFrame.from_dict(data)
-        
+
         return packet_df
-    
+
     def get_per(self, expected_sprinkler_count=6):
         """
         Calculates the packet per at the sprinkler
         @param expected_sprinkler_count - in case of no beacons environment, sprinkler can be bigger than 6.
         @return packet per at percentage
         """
         return 100 * (1 - len(self) / expected_sprinkler_count)
-    
+
     def get_tbp(self):
         """
         calculates the rate of packets from the same sprinkler
         :return: min_times_found - in msec
         :rtype: int
         """
-        
+
         def triad_ratio_logic(diff_time_1, diff_time_2, ratio=1.0, error=10):
             """ estimate the time between successive packet according to only 3 packets out of 6 """
             if abs(diff_time_1 - ratio * diff_time_2) <= diff_time_2 / error:
                 return True
             elif abs(diff_time_1 - (1 / ratio) * diff_time_2) <= diff_time_1 / error:
                 return True
             else:
                 return False
-        
+
         def estimate_diff_packet_time(times_list, pc_time_list):
             if times_list.size < 3:
                 return None
             sort_idx = pc_time_list.argsort()
             pc_time_list_sorted = pc_time_list.copy()[sort_idx]
             times_list_sorted = times_list.copy()[sort_idx]
-            
+
             fix_sort_idx = []
             ind = 0
             pc_time_unique, pc_time_counts = np.unique(pc_time_list_sorted, return_counts=True)
             for unique, counts in zip(pc_time_unique, pc_time_counts):
                 if counts > 1:  # several packets
                     ind_with_same_time = [i for i, t in enumerate(pc_time_list_sorted) if t == unique]
                     fix_sort_idx += list(times_list_sorted[ind_with_same_time].argsort() + ind_with_same_time[0])
                 else:
                     fix_sort_idx.append(sort_idx[ind])
                 ind += counts
-            
+
             times_list_sorted = times_list_sorted[fix_sort_idx]
-            
+
             dt = []
             for i, t_hw in enumerate(zip(times_list_sorted[1::], times_list_sorted[:-1])):
                 dt_tmp = t_hw[0] - t_hw[1]
                 if dt_tmp < 0:  # HW timing was zeroing during the same packets sprinkler
                     n_wrap = 1 + (round(
                         (pc_time_list_sorted[i + 1] - pc_time_list_sorted[i]) * 1000) // max_stat_param_val)
                     dt_tmp = (n_wrap * max_stat_param_val) + t_hw[0] - t_hw[1]
                 dt.append(dt_tmp)
-            
+
             return dt
 
         def check_if_nan(lst):
             is_nan = pd.isnull(lst)
             if (not isinstance(is_nan, np.ndarray) and is_nan) or (isinstance(is_nan, np.ndarray) and any(is_nan)):
                 return True
             return False
@@ -518,26 +541,26 @@
                     if triad_ratio_logic(estimate_diff_time[0], estimate_diff_time[1], ratio=ratio):
                         estimate_diff_time = [min(estimate_diff_time[0], estimate_diff_time[1]),
                                               max(estimate_diff_time[0], estimate_diff_time[1]) / ratio]
                         break
                 if triad_ratio_logic(estimate_diff_time[0], estimate_diff_time[1], ratio=1.5):
                     estimate_diff_time = [min(estimate_diff_time[0], estimate_diff_time[1]) / 2,
                                           max(estimate_diff_time[0], estimate_diff_time[1]) / 3]
-        
+
         return int(min(estimate_diff_time))
-    
+
     def extract_packet_data_by_name(self, key):
         """
         extract data from all packet attribute according to the key name
         :param key: the name of the data (the key of the relevant dictionary)
         :type key: str
         :return: list of the data
         :rtype: list
         """
-        
+
         if key in self.packet_data:
             data_attr = self.packet_data[key]
         elif hasattr(self, 'decoded_data') and key in self.decoded_data:
             data_attr = self.decoded_data[key]
         elif key in self.gw_data:
             data_attr = self.gw_data[key]
         elif key in self.custom_data:
@@ -546,41 +569,41 @@
             print('key:{} does not exist in packet structure')
             return None
         if isinstance(data_attr, np.ndarray):
             data_attr = data_attr.tolist()
         if not isinstance(data_attr, list):
             data_attr = [data_attr]
         return data_attr
-    
+
     def filter_by_sprinkler_id(self, sprinkler_ids):
         """
         keep only specific sprinklers in a packet according to the sprinkler id
         :param sprinkler_ids:
         :type sprinkler_ids: list
         :return: filtered packet
         :rtype: Packet or DecryptedPacket
         """
-        
+
         def filter_per_attr(data_attr):
             for key in data_attr.keys():
                 if isinstance(data_attr[key], list) or \
                         (isinstance(data_attr[key], np.ndarray) and data_attr[key].size > 1):
                     filtered_data = [data_attr[key][i] for i in sprinkler_ids]
                     if isinstance(data_attr[key], np.ndarray):
                         data_attr[key] = np.array(filtered_data)
                     else:
                         data_attr[key] = filtered_data
             return data_attr
-        
+
         filtered_packet = self.copy()
         filtered_packet.gw_data = filter_per_attr(filtered_packet.gw_data)
         filtered_packet.custom_data = filter_per_attr(filtered_packet.custom_data)
-        
+
         return filtered_packet
-    
+
     def add_custom_data(self, custom_data):
         for key in custom_data.keys():
             if isinstance(custom_data[key], list):
                 if len(custom_data[key]) == self.__len__():
                     self.custom_data[key] = custom_data[key]
                 else:
                     print('add_custom_data failed - '
@@ -594,25 +617,25 @@
                 'is_valid_tag_packet': True, 'adv_address': '03B28DCD9920', 'group_id': 'FE0000', 'rssi': 54,
                 'stat_param': 44687,
                 'time_from_start': 1.528374, 'counter_tag': 1}
     packet_2 = {'packet': '03B28DCD99201EFF0005FE0000E0210FFF93B635EBFF1DB118C6D782DC2ED98C404200486436AE82',
                 'is_valid_tag_packet': True, 'adv_address': '03B28DCD9920', 'group_id': 'FE0000', 'rssi': 60,
                 'stat_param': 44688,
                 'time_from_start': 2.528374, 'counter_tag': 2}
-    
+
     p1 = Packet(packet_1)
     p2 = Packet(packet_2)
-    
+
     print(p1.get_packet_string(0))
     print(p1.get_average_rssi())
-    
+
     print(p1 == p2)
     print(p1.append_to_sprinkler(p2))
-    
+
     print(len(p1))
     print(p1.get_average_rssi())
-    
+
     p1_dict = p1.as_dict()
     p1_df = pd.DataFrame(data=p1_dict)
     print(p1_df)
-    
+
     print('end')
```

### Comparing `wiliot-core-4.0.6/wiliot_core/packet_data/packet_list.py` & `wiliot-core-4.0.8/wiliot_core/packet_data/packet_list.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.6/wiliot_core/packet_data/tag_collection.py` & `wiliot-core-4.0.8/wiliot_core/packet_data/tag_collection.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.6/wiliot_core/utils/get_version.py` & `wiliot-core-4.0.8/wiliot_core/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.6/wiliot_core/utils/update_wiliot_packages.py` & `wiliot-core-4.0.8/wiliot_core/utils/update_wiliot_packages.py`

 * *Files 23% similar despite different names*

```diff
@@ -53,136 +53,193 @@
 #     FOR ANY LOSS OF USE OR DATA OR BUSINESS INTERRUPTION, AND/OR FOR ANY ECONOMIC LOSS
 #     (SUCH AS LOST PROFITS, REVENUE, ANTICIPATED SAVINGS). THE FOREGOING SHALL APPLY:
 #     (A) HOWEVER CAUSED AND REGARDLESS OF THE THEORY OR BASIS LIABILITY, WHETHER IN
 #     CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE);
 #     (B) EVEN IF ANYONE IS ADVISED OF THE POSSIBILITY OF ANY DAMAGES, LOSSES, OR COSTS; AND
 #     (C) EVEN IF ANY REMEDY FAILS OF ITS ESSENTIAL PURPOSE.
 #  """
+
+import shutil
 from os import popen
-from os.path import join
+from os.path import join, isdir
 from sys import platform
 from enum import Enum
 
 
 class WiliotPackages(Enum):
     CLOUD = ['pywiliot-api']
     CORE = ['pywiliot-core', 'pywiliot-api']
     TOOLS = ['pywiliot-tools', 'pywiliot-core', 'pywiliot-api']
     DEPLOYMENT = ['pywiliot-deployment-tools', 'pywiliot-tools', 'pywiliot-core', 'pywiliot-api']
     TESTERS = ['pywiliot-testers', 'pywiliot-tools', 'pywiliot-core', 'pywiliot-api']
 
 
-def update_internal_wiliot_packages(wiliot_repo=WiliotPackages.CLOUD, branch_name='master', username=''):
+def update_internal_wiliot_packages(wiliot_repo=WiliotPackages.CLOUD, branch_name='master',
+                                    overwrite=False, no_wiliot_dep=False,
+                                    username_bitbucket=None, password_bitbucket=None,
+                                    install_from_local_folder='', branch_name_for_dep='master'):
     # check platform command prefix
-    commandPrefix = ''
-    if platform == "darwin":
-        # OS X
-        commandPrefix = '/usr/local/bin/'
+    python_ver = ''
+    if platform == "darwin" or platform == 'linux':
+        # macos or linux
+        python_ver = '3'
     # install pywiliot and requirements:
     # update dependencies
     print("----------------------------------\nupdate pip:\n----------------------------------")
-    p = popen(commandPrefix + 'pip install --upgrade pip')
+    p = popen(f'python{python_ver} -m pip install --upgrade pip')
     rsp = p.read()
     print(rsp)
     pkg_versions = []
     req_status = []
     for repo_num, repo_name in enumerate(wiliot_repo.value):
         package_name = repo_name.replace('py', '')
         folder_name = package_name.replace('-', '_')
         print('check if package already exist')
-        p = popen(commandPrefix + f'pip show {package_name}')
+        p = popen(f'pip{python_ver} show {package_name}')
         rsp = p.read()
         print(rsp)
         if package_name in rsp:
-            print(f'--------------------------------------------------------------------\n'
-                  f'for uninstall existing package: {package_name}, please press ENTER\n'
-                  f'--------------------------------------------------------------------\n')
-            p = popen(commandPrefix + f'pip uninstall {package_name}')
+            if overwrite:
+                print(f'--------------------------------------------------------------------\n'
+                      f'uninstall existing package: {package_name}\n'
+                      f'--------------------------------------------------------------------\n')
+                p = popen(f'pip{python_ver} uninstall {package_name} -y')
+            else:
+                print(f'--------------------------------------------------------------------\n'
+                      f'for uninstall existing package: {package_name}, please press ENTER\n'
+                      f'--------------------------------------------------------------------\n')
+                p = popen(f'pip{python_ver} uninstall {package_name}')
             rsp = p.read()
             print(rsp)
         print(f'--------------------------------------------------------------------\n'
               f'update wiliot package: {package_name}\n'
               f'--------------------------------------------------------------------')
-        if repo_num == 0:
-            p = popen(commandPrefix + f'pip install git+ssh://git@bitbucket.org/wiliot/{repo_name}.git'
-                                      f'@{branch_name}#egg={folder_name} --upgrade')
+        if install_from_local_folder:
+            local_repo_path = join(install_from_local_folder, repo_name)
+            if not isdir(local_repo_path):
+                print(f'{repo_name} does not exist in local folder, skip installation')
+                pkg_versions.append('')
+                req_status.append(False)
+                continue
+            p = popen(f'pip{python_ver} install -e {local_repo_path}')
+            rsp = p.read()
+            print(rsp)
+        elif username_bitbucket is None and password_bitbucket is None:
+            if repo_num == 0:
+                p = popen(f'pip{python_ver} install git+ssh://git@bitbucket.org/wiliot/{repo_name}.git'
+                          f'@{branch_name}#egg={folder_name} --upgrade')
+            else:
+                p = popen(f'pip{python_ver} install git+ssh://git@bitbucket.org/wiliot/{repo_name}.git'
+                          f'@{branch_name_for_dep}#egg={folder_name} --upgrade')
+            rsp = p.read()
+            print(rsp)
+            if 'Successfully installed' not in rsp.split('\n')[-2]:
+                print(f'problem with ssh key credentials. Please rerun the script using username (-u) and password (-p).'
+                      f'\nTo extract Attlasian username and password go to '
+                      f'https://wiliot.atlassian.net/wiki/spaces/SW/pages/2890662124/'
+                      f'PyWiliot+Installation+Guidelines+-+Private#using-username-and-password%3A')
+                return
+        elif username_bitbucket is not None and password_bitbucket is not None:
+            if repo_num == 0:
+                p = popen(f'pip{python_ver} install git+https://{username_bitbucket}:{password_bitbucket}@bitbucket.org'
+                          f'/wiliot/{repo_name}.git@{branch_name}#egg={folder_name} --upgrade')
+            else:
+                p = popen(f'pip{python_ver} install git+https://{username_bitbucket}:{password_bitbucket}@bitbucket.org'
+                          f'/wiliot/{repo_name}.git#egg={folder_name} --upgrade')
+            rsp = p.read()
+            print(rsp)
         else:
-            p = popen(commandPrefix + f'pip install git+ssh://git@bitbucket.org/wiliot/{repo_name}.git'
-                                      f'#egg={folder_name} --upgrade')
-        rsp = p.read()
-        print(rsp)
-        if 'Successfully installed' not in rsp.split('\n')[-2]:
-            print('problem with ssh key credentials. Please try to install using username and password.\n'
-                  'please rerun the function with your bitbucket username and check in the readme how to extract '
-                  'the "app password" from bitbucket')
-            if username:
-                print(f'update wiliot package (using username and password): {package_name}')
-                if repo_num == 0:
-                    p = popen(commandPrefix + f'pip install git+https://{username}@bitbucket.org/wiliot/{repo_name}.git'
-                                              f'@{branch_name}#egg={folder_name} --upgrade')
-                else:
-                    p = popen(commandPrefix + f'pip install git+https://{username}@bitbucket.org/wiliot/{repo_name}.git'
-                                              f'#egg={folder_name} --upgrade')
-                rsp = p.read()
-                print(rsp)
+            print('you Must specified both username and password or do NOT specified neither '
+                  'for installation using SSH key')
+            return
 
         print(f'check wiliot package: {package_name}')
-        p = popen(commandPrefix + f'pip show {package_name}')
+        p = popen(f'pip{python_ver} show {package_name}')
         rsp = p.read()
         print(rsp)
         if 'Location' in rsp:
             pkg_versions.append(rsp.split('Version: ')[1].split('\n')[0])
             req_path = rsp.split('Location: ')[-1].split('\n')[0]
+            if install_from_local_folder:
+                site_packages_path = join(req_path, folder_name)
+                if isdir(site_packages_path):
+                    shutil.rmtree(site_packages_path)
+                shutil.copytree(join(install_from_local_folder, repo_name, folder_name), site_packages_path)
+                req_path = join(install_from_local_folder, repo_name)
+
             print("--------------------------------------------------------------------\n"
                   "update dependencies:\n"
                   "--------------------------------------------------------------------")
             requirements_path = join(req_path, folder_name, 'requirements.txt')
-            p = popen(commandPrefix + f'pip install -r {requirements_path}')
+            p = popen(f'pip{python_ver} install -r {requirements_path}')
             rsp = p.read()
             print(rsp)
             req_status.append('ERROR' not in rsp)
         else:
             pkg_versions.append('')
             req_status.append(False)
 
+        if no_wiliot_dep:
+            break
+
     print('done installation')
     print("************************************************************************\n"
           "********************            Summary            *********************\n"
           "************************************************************************")
     for i, repo_name in enumerate(wiliot_repo.value):
         package_name = repo_name.replace('py', '')
         is_installed = f'installed [{pkg_versions[i]}]' if pkg_versions[i] else 'NOT installed'
         sum_str = f'{package_name} was {is_installed}'
         if is_installed:
             req_is_installed = 'installed' if req_status[i] else 'NOT installed'
             sum_str += f'and the dependencies were {req_is_installed}'
         print(sum_str)
+        if no_wiliot_dep:
+            break
 
 
 if __name__ == '__main__':
     import argparse
     parser = argparse.ArgumentParser(description='Update Wiliot Internal Packages')
     parser.add_argument('-p', '--package_name', help='The package name. valid option(wiliot-api, wiliot-core, '
                                                      'wiliot-tools, wiliot-testers, wiliot-deployment-tools')
     parser.add_argument('-b', '--branch_name', help='The branch name you want to use. the default is master',
                         default='master')
-    parser.add_argument('-u', '--username', help='If SSH key installation is not working, install using '
-                                                 'BitBucket username')
+    parser.add_argument('-w', '--overwrite', help='If specified, all wiliot existed packages will be overwrite '
+                                                  'with the new installation', default=False, action='store_true')
+    parser.add_argument('-n', '--no_wiliot_dep', help='If specified, install the main package without wiliot '
+                                                      'dependencies packages', default=False, action='store_true')
+    parser.add_argument('-u', '--username', help='If specified, install based username and password and not SHH key',
+                        default=None)
+    parser.add_argument('-pass', '--password', help='If specified, install based username and password and not SHH key',
+                        default=None)
+    parser.add_argument('-l', '--local_folder', help='If specified, install packages from the specified local folder')
+    parser.add_argument('-b-for-dep', '--branch_for_dependencies',
+                        help='if specified, all wiliot package dependencies will be installed for this branch '
+                             '(default master)', default='master')
     args = parser.parse_args()
     package_name = args.package_name
     branch_name = args.branch_name
-    user_name = args.username
+    is_overwrite = args.overwrite
+    is_no_wiliot_dep = args.no_wiliot_dep
+    username = args.username
+    password = args.password
+    local_folder = args.local_folder
+    branch_for_dep = args.branch_for_dependencies
     err_msg = 'please add package name, e.g. update_wiliot_packages.py -p wiliot-api.\n' \
               'The valid packages names are: wiliot-api, wiliot-core, wiliot-tools, wiliot-testers, ' \
               'wiliot-deployment-tools'
     try:
         repo_name = None
         for package in WiliotPackages.__members__.values():
             if package_name in package.value[0]:
                 repo_name = package
                 break
         if repo_name is None:
             print(err_msg)
         else:
-            update_internal_wiliot_packages(wiliot_repo=repo_name, branch_name=branch_name, username=user_name)
+            update_internal_wiliot_packages(wiliot_repo=repo_name, branch_name=branch_name,
+                                            overwrite=is_overwrite, no_wiliot_dep=is_no_wiliot_dep,
+                                            username_bitbucket=username, password_bitbucket=password,
+                                            install_from_local_folder=local_folder, branch_name_for_dep=branch_for_dep)
     except Exception as e:
-        print(err_msg + ' [ERROR: {}]'.format(e))
+        print('Error during update packages  [ERROR: {}]'.format(e))
```

### Comparing `wiliot-core-4.0.6/wiliot_core/utils/utils.py` & `wiliot-core-4.0.8/wiliot_core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `wiliot-core-4.0.6/wiliot_core.egg-info/PKG-INFO` & `wiliot-core-4.0.8/wiliot_core.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-core
-Version: 4.0.6
+Version: 4.0.8
 Summary: A library for interacting with Wiliot's private core functions
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -56,14 +56,29 @@
 * [gateway communication](wiliot_core/local_gateway/examples)
 * [packet data](wiliot_core/packet_data) (at the end of each script)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
+Version 4.0.8:
+-----------------
+* continuous listener as multi-processes:
+    * add option to specify log path and communicate reading error using event
+    * connect to gw in a more robust way including printing exceptions if needed
+* local gw core:
+    * connect only to “Silicon Lab”/"CP210.." ports (Wiliot's gw driver)
+    * added a function to check gw response using version command check_gw_responds including is_gw_alive function
+    * better handling ACK msg from the GW
+    * get reading status function get_read_error_status. 
+    * better stop gw app including writing a log if no ACK was received for the cancel command
+    * add new GW FW version
+* packet:
+    * add new function to packet to retrieve basic data: get_adva, get_flow, get_rssi
+
 
 Version 4.0.6:
 -----------------
 * First version
 
 
 The package previous content was published under the name 'wiliot' package.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wiliot-core-4.0.6/wiliot_core.egg-info/SOURCES.txt` & `wiliot-core-4.0.8/wiliot_core.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,20 +19,23 @@
 wiliot_core/local_gateway/continuous_listener.py
 wiliot_core/local_gateway/custom_energy_pattern.py
 wiliot_core/local_gateway/local_gateway_core.py
 wiliot_core/local_gateway/examples/__init__.py
 wiliot_core/local_gateway/examples/local_gateway_basic_example.py
 wiliot_core/local_gateway/local_gateway_versions/3.8.14_app.zip
 wiliot_core/local_gateway/local_gateway_versions/3.8.14_sd_bl_gw_app.zip
+wiliot_core/local_gateway/local_gateway_versions/4.0.16_app.zip
+wiliot_core/local_gateway/local_gateway_versions/4.0.16_sd_bl_gw_app.zip
 wiliot_core/local_gateway/local_gateway_versions/4.0.4_app.zip
 wiliot_core/local_gateway/local_gateway_versions/4.0.4_sd_bl_gw_app.zip
 wiliot_core/local_gateway/local_gateway_versions/__init__.py
 wiliot_core/local_gateway/local_gateway_versions/wifi_3.8.14.hex
 wiliot_core/local_gateway/local_gateway_versions/wifi_4.0.4.hex
 wiliot_core/packet_data/__init__.py
 wiliot_core/packet_data/packet.py
 wiliot_core/packet_data/packet_list.py
 wiliot_core/packet_data/tag_collection.py
 wiliot_core/utils/__init__.py
 wiliot_core/utils/get_version.py
+wiliot_core/utils/release_for_partners.py
 wiliot_core/utils/update_wiliot_packages.py
 wiliot_core/utils/utils.py
```

