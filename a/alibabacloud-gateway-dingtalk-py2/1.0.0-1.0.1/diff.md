# Comparing `tmp/alibabacloud_gateway_dingtalk_py2-1.0.0.tar.gz` & `tmp/alibabacloud_gateway_dingtalk_py2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_gateway_dingtalk_py2-1.0.0.tar", last modified: Fri Apr 21 03:28:34 2023, max compression
+gzip compressed data, was "dist/alibabacloud_gateway_dingtalk_py2-1.0.1.tar", last modified: Tue Apr 25 07:15:07 2023, max compression
```

## Comparing `alibabacloud_gateway_dingtalk_py2-1.0.0.tar` & `alibabacloud_gateway_dingtalk_py2-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 03:28:34.000000 alibabacloud_gateway_dingtalk_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     1035 2023-04-21 03:28:34.000000 alibabacloud_gateway_dingtalk_py2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 03:28:34.000000 alibabacloud_gateway_dingtalk_py2-1.0.0/alibabacloud_gateway_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 03:28:34.000000 alibabacloud_gateway_dingtalk_py2-1.0.0/alibabacloud_gateway_dingtalk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7997 2023-04-21 03:28:34.000000 alibabacloud_gateway_dingtalk_py2-1.0.0/alibabacloud_gateway_dingtalk/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 03:28:34.000000 alibabacloud_gateway_dingtalk_py2-1.0.0/alibabacloud_gateway_dingtalk_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1035 2023-04-21 03:28:34.000000 alibabacloud_gateway_dingtalk_py2-1.0.0/alibabacloud_gateway_dingtalk_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      374 2023-04-21 03:28:34.000000 alibabacloud_gateway_dingtalk_py2-1.0.0/alibabacloud_gateway_dingtalk_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 03:28:34.000000 alibabacloud_gateway_dingtalk_py2-1.0.0/alibabacloud_gateway_dingtalk_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      375 2023-04-21 03:28:34.000000 alibabacloud_gateway_dingtalk_py2-1.0.0/alibabacloud_gateway_dingtalk_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-21 03:28:34.000000 alibabacloud_gateway_dingtalk_py2-1.0.0/alibabacloud_gateway_dingtalk_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 03:28:34.000000 alibabacloud_gateway_dingtalk_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3150 2023-04-21 03:28:34.000000 alibabacloud_gateway_dingtalk_py2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:15:07.000000 alibabacloud_gateway_dingtalk_py2-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-04-25 07:15:07.000000 alibabacloud_gateway_dingtalk_py2-1.0.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:15:07.000000 alibabacloud_gateway_dingtalk_py2-1.0.1/alibabacloud_gateway_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-25 07:15:07.000000 alibabacloud_gateway_dingtalk_py2-1.0.1/alibabacloud_gateway_dingtalk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3335 2023-04-25 07:15:07.000000 alibabacloud_gateway_dingtalk_py2-1.0.1/alibabacloud_gateway_dingtalk/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:15:07.000000 alibabacloud_gateway_dingtalk_py2-1.0.1/alibabacloud_gateway_dingtalk_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-04-25 07:15:07.000000 alibabacloud_gateway_dingtalk_py2-1.0.1/alibabacloud_gateway_dingtalk_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      374 2023-04-25 07:15:07.000000 alibabacloud_gateway_dingtalk_py2-1.0.1/alibabacloud_gateway_dingtalk_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 07:15:07.000000 alibabacloud_gateway_dingtalk_py2-1.0.1/alibabacloud_gateway_dingtalk_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2023-04-25 07:15:07.000000 alibabacloud_gateway_dingtalk_py2-1.0.1/alibabacloud_gateway_dingtalk_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-25 07:15:07.000000 alibabacloud_gateway_dingtalk_py2-1.0.1/alibabacloud_gateway_dingtalk_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 07:15:07.000000 alibabacloud_gateway_dingtalk_py2-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-04-25 07:15:07.000000 alibabacloud_gateway_dingtalk_py2-1.0.1/setup.py
```

### Comparing `alibabacloud_gateway_dingtalk_py2-1.0.0/PKG-INFO` & `alibabacloud_gateway_dingtalk_py2-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_gateway_dingtalk_py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud DingTalk SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-gateway
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,gateway,dingtalk,py2
```

### Comparing `alibabacloud_gateway_dingtalk_py2-1.0.0/alibabacloud_gateway_dingtalk_py2.egg-info/PKG-INFO` & `alibabacloud_gateway_dingtalk_py2-1.0.1/alibabacloud_gateway_dingtalk_py2.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-gateway-dingtalk-py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud DingTalk SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-gateway
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,gateway,dingtalk,py2
```

### Comparing `alibabacloud_gateway_dingtalk_py2-1.0.0/setup.py` & `alibabacloud_gateway_dingtalk_py2-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,35 +21,29 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_gateway_dingtalk_py2.
 
-Created on 21/04/2023
+Created on 25/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_gateway_dingtalk"
 NAME = "alibabacloud_gateway_dingtalk_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud DingTalk SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-gateway"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_gateway_spi_py2>=0.0.1, <1.0.0",
-    "alibabacloud_credentials_py2>=0.1.1, <1.0.0",
-    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
-    "alibabacloud_darabonba_encode_util_py2>=0.0.2, <1.0.0",
-    "alibabacloud_darabonba_signature_util_py2>=0.0.4, <1.0.0",
-    "alibabacloud_darabonba_string_py2>=0.0.4, <1.0.0",
-    "alibabacloud_darabonba_map_py2>=0.0.2, <1.0.0",
-    "alibabacloud_darabonba_array_py2>=0.1.0, <1.0.0"
+    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
         with open("README.md") as fp:
```

