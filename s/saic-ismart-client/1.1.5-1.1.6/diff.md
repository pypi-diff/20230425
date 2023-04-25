# Comparing `tmp/saic_ismart_client-1.1.5.tar.gz` & `tmp/saic_ismart_client-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saic_ismart_client-1.1.5.tar", last modified: Wed Apr 12 06:45:12 2023, max compression
+gzip compressed data, was "saic_ismart_client-1.1.6.tar", last modified: Tue Apr 25 08:06:03 2023, max compression
```

## Comparing `saic_ismart_client-1.1.5.tar` & `saic_ismart_client-1.1.6.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 06:45:12.386515 saic_ismart_client-1.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.378515 saic_ismart_client-1.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/src/saic_ismart_client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.378515 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20928 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/common_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v1_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v1_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v1_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v2_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v2_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v2_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v3_0/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v3_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v3_0/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    22997 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/src/saic_ismart_client/saic_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/src/saic_ismart_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-12 06:45:12.000000 saic_ismart_client-1.1.5/src/saic_ismart_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-12 06:45:12.000000 saic_ismart_client-1.1.5/src/saic_ismart_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 06:45:12.000000 saic_ismart_client-1.1.5/src/saic_ismart_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 06:45:12.000000 saic_ismart_client-1.1.5/src/saic_ismart_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 06:45:12.000000 saic_ismart_client-1.1.5/src/saic_ismart_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:45:12.382515 saic_ismart_client-1.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/tests/test_Message_v1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/tests/test_Message_v2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/tests/test_Message_v3_0.py
--rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-04-12 06:45:02.000000 saic_ismart_client-1.1.5/tests/test_ws_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.358740 saic_ismart_client-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-25 08:06:03.358740 saic_ismart_client-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:06:03.358740 saic_ismart_client-1.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.350740 saic_ismart_client-1.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.354740 saic_ismart_client-1.1.6/src/saic_ismart_client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.350740 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.354740 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.354740 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.354740 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20928 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/common_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.354740 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v1_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v1_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v1_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.354740 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v2_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v2_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v2_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.358740 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v3_0/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v3_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v3_0/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22997 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/src/saic_ismart_client/saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.354740 saic_ismart_client-1.1.6/src/saic_ismart_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-25 08:06:03.000000 saic_ismart_client-1.1.6/src/saic_ismart_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-25 08:06:03.000000 saic_ismart_client-1.1.6/src/saic_ismart_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:06:03.000000 saic_ismart_client-1.1.6/src/saic_ismart_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-25 08:06:03.000000 saic_ismart_client-1.1.6/src/saic_ismart_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-25 08:06:03.000000 saic_ismart_client-1.1.6/src/saic_ismart_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:06:03.358740 saic_ismart_client-1.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/tests/test_Message_v1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/tests/test_Message_v2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/tests/test_Message_v3_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/tests/test_abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-04-25 08:05:47.000000 saic_ismart_client-1.1.6/tests/test_ws_api.py
```

### Comparing `saic_ismart_client-1.1.5/LICENSE` & `saic_ismart_client-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.5/PKG-INFO` & `saic_ismart_client-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic_ismart_client
-Version: 1.1.5
+Version: 1.1.6
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.1.5/README.md` & `saic_ismart_client-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.5/pyproject.toml` & `saic_ismart_client-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saic_ismart_client"
-version = "1.1.5"
+version = "1.1.6"
 authors = [
     { name = "Thomas Salm", email="saic-python-client@devtom.de"},
 ]
 dependencies = [
     "asn1tools >= 0.165.0",
     "requests >= 2.28.2",
     "urllib3 >= 1.26.14",
```

### Comparing `saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1` & `saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1` & `saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1` & `saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.5/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1` & `saic_ismart_client-1.1.6/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.5/src/saic_ismart_client/abrp_api.py` & `saic_ismart_client-1.1.6/src/saic_ismart_client/abrp_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,22 @@
-import urllib.parse
+import json
 
 import requests
 from saic_ismart_client.ota_v2_1.data_model import OtaRvmVehicleStatusResp25857
 from saic_ismart_client.ota_v3_0.data_model import OtaChrgMangDataResp
 
 
+class AbrpApiException(Exception):
+    def __init__(self, msg: str):
+        self.message = msg
+
+    def __str__(self):
+        return self.message
+
+
 class AbrpApi:
     def __init__(self, abrp_api_key: str, abrp_user_token: str) -> None:
         self.abrp_api_key = abrp_api_key
         self.abrp_user_token = abrp_user_token
 
     def update_abrp(self, vehicle_status: OtaRvmVehicleStatusResp25857, charge_status: OtaChrgMangDataResp):
         if (
@@ -44,14 +52,25 @@
             mileage = vehicle_status.get_basic_vehicle_status().mileage
             if mileage > 0:
                 data['odometer'] = mileage / 10.0
             range_elec = vehicle_status.get_basic_vehicle_status().fuel_range_elec
             if range_elec > 0:
                 data['est_battery_range'] = range_elec / 10.0
 
-            tlm_response = requests.get(tlm_send_url, params={
-                'api_key': self.abrp_api_key,
-                'token': self.abrp_user_token,
-                'tlm': urllib.parse.urlencode(data)
-            })
-            tlm_response.raise_for_status()
-            print(f'ABRP: {tlm_response.content}')
+            headers = {
+                'Authorization': f'APIKEY {self.abrp_api_key}'
+            }
+
+            try:
+                response = requests.post(url=tlm_send_url, headers=headers, params={
+                    'token': self.abrp_user_token,
+                    'tlm': json.dumps(data)
+                })
+                print(f'ABRP: {response.content}')
+            except requests.exceptions.ConnectionError as ece:
+                raise AbrpApiException(f'Connection error: {ece}')
+            except requests.exceptions.Timeout as et:
+                raise AbrpApiException(f'Timeout error {et}')
+            except requests.exceptions.HTTPError as ehttp:
+                raise AbrpApiException(f'HTTP error {ehttp}')
+            except requests.exceptions.RequestException as e:
+                raise AbrpApiException(f'{e}')
```

### Comparing `saic_ismart_client-1.1.5/src/saic_ismart_client/common_model.py` & `saic_ismart_client-1.1.6/src/saic_ismart_client/common_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v1_1/Message.py` & `saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v1_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v1_1/data_model.py` & `saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v1_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v2_1/Message.py` & `saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v2_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v2_1/data_model.py` & `saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v2_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v3_0/Message.py` & `saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v3_0/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.5/src/saic_ismart_client/ota_v3_0/data_model.py` & `saic_ismart_client-1.1.6/src/saic_ismart_client/ota_v3_0/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.5/src/saic_ismart_client/saic_api.py` & `saic_ismart_client-1.1.6/src/saic_ismart_client/saic_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.5/src/saic_ismart_client.egg-info/PKG-INFO` & `saic_ismart_client-1.1.6/src/saic_ismart_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic-ismart-client
-Version: 1.1.5
+Version: 1.1.6
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.1.5/src/saic_ismart_client.egg-info/SOURCES.txt` & `saic_ismart_client-1.1.6/src/saic_ismart_client.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,9 @@
 src/saic_ismart_client/ota_v2_1/data_model.py
 src/saic_ismart_client/ota_v3_0/Message.py
 src/saic_ismart_client/ota_v3_0/__init__.py
 src/saic_ismart_client/ota_v3_0/data_model.py
 tests/test_Message_v1_1.py
 tests/test_Message_v2_1.py
 tests/test_Message_v3_0.py
+tests/test_abrp_api.py
 tests/test_ws_api.py
```

### Comparing `saic_ismart_client-1.1.5/tests/test_Message_v1_1.py` & `saic_ismart_client-1.1.6/tests/test_Message_v1_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.5/tests/test_Message_v2_1.py` & `saic_ismart_client-1.1.6/tests/test_Message_v2_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.5/tests/test_Message_v3_0.py` & `saic_ismart_client-1.1.6/tests/test_Message_v3_0.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.1.5/tests/test_ws_api.py` & `saic_ismart_client-1.1.6/tests/test_ws_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     MpAlarmSettingType
 from saic_ismart_client.ota_v2_1.Message import MessageCoderV21
 from saic_ismart_client.ota_v2_1.data_model import OtaRvmVehicleStatusResp25857, RvsPosition, RvsWayPoint,\
     RvsWgs84Point, Timestamp4Short, RvsBasicStatus25857
 from saic_ismart_client.ota_v3_0.Message import MessageBodyV30, MessageV30, MessageCoderV30
 from saic_ismart_client.ota_v3_0.data_model import OtaChrgMangDataResp, RvsChargingStatus
 
-from saic_api import SaicApi
+from saic_ismart_client.saic_api import SaicApi
 
 TOKEN = '99X9999X-90XX-99X9-99X9-9XX9XX0X9X9XXX9X'
 UID = '00000000000000000000000000000000000090000000099999'
 VIN = 'vin10000000000000'
 
 
 def mock_login_response_hex(message_coder: MessageCoderV11) -> str:
```

