# Comparing `tmp/antchain_partner-1.0.19.tar.gz` & `tmp/antchain_partner-1.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_partner-1.0.19.tar", last modified: Sun Apr 23 09:35:57 2023, max compression
+gzip compressed data, was "dist/antchain_partner-1.0.20.tar", last modified: Tue Apr 25 01:52:16 2023, max compression
```

## Comparing `antchain_partner-1.0.19.tar` & `antchain_partner-1.0.20.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:35:57.000000 antchain_partner-1.0.19/
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-23 09:35:56.000000 antchain_partner-1.0.19/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-23 09:35:56.000000 antchain_partner-1.0.19/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2187 2023-04-23 09:35:57.000000 antchain_partner-1.0.19/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      816 2023-04-23 09:35:56.000000 antchain_partner-1.0.19/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1002 2023-04-23 09:35:56.000000 antchain_partner-1.0.19/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:35:57.000000 antchain_partner-1.0.19/antchain_partner.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2187 2023-04-23 09:35:57.000000 antchain_partner-1.0.19/antchain_partner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      355 2023-04-23 09:35:57.000000 antchain_partner-1.0.19/antchain_partner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 09:35:57.000000 antchain_partner-1.0.19/antchain_partner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-23 09:35:57.000000 antchain_partner-1.0.19/antchain_partner.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-23 09:35:57.000000 antchain_partner-1.0.19/antchain_partner.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 09:35:57.000000 antchain_partner-1.0.19/antchain_sdk_partner/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-23 09:35:56.000000 antchain_partner-1.0.19/antchain_sdk_partner/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46536 2023-04-23 09:35:56.000000 antchain_partner-1.0.19/antchain_sdk_partner/client.py
--rw-r--r--   0 root         (0) root         (0)   108385 2023-04-23 09:35:56.000000 antchain_partner-1.0.19/antchain_sdk_partner/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-23 09:35:57.000000 antchain_partner-1.0.19/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2508 2023-04-23 09:35:56.000000 antchain_partner-1.0.19/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 01:52:16.000000 antchain_partner-1.0.20/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-25 01:52:15.000000 antchain_partner-1.0.20/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-25 01:52:15.000000 antchain_partner-1.0.20/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2187 2023-04-25 01:52:16.000000 antchain_partner-1.0.20/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      816 2023-04-25 01:52:15.000000 antchain_partner-1.0.20/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-25 01:52:15.000000 antchain_partner-1.0.20/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 01:52:16.000000 antchain_partner-1.0.20/antchain_partner.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2187 2023-04-25 01:52:16.000000 antchain_partner-1.0.20/antchain_partner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      355 2023-04-25 01:52:16.000000 antchain_partner-1.0.20/antchain_partner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 01:52:16.000000 antchain_partner-1.0.20/antchain_partner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-04-25 01:52:16.000000 antchain_partner-1.0.20/antchain_partner.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-25 01:52:16.000000 antchain_partner-1.0.20/antchain_partner.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 01:52:16.000000 antchain_partner-1.0.20/antchain_sdk_partner/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-25 01:52:15.000000 antchain_partner-1.0.20/antchain_sdk_partner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46536 2023-04-25 01:52:15.000000 antchain_partner-1.0.20/antchain_sdk_partner/client.py
+-rw-r--r--   0 root         (0) root         (0)   110481 2023-04-25 01:52:15.000000 antchain_partner-1.0.20/antchain_sdk_partner/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-25 01:52:16.000000 antchain_partner-1.0.20/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-04-25 01:52:15.000000 antchain_partner-1.0.20/setup.py
```

### Comparing `antchain_partner-1.0.19/LICENSE` & `antchain_partner-1.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_partner-1.0.19/PKG-INFO` & `antchain_partner-1.0.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_partner
-Version: 1.0.19
+Version: 1.0.20
 Summary: Ant Chain PARTNER SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_partner-1.0.19/README-CN.md` & `antchain_partner-1.0.20/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_partner-1.0.19/README.md` & `antchain_partner-1.0.20/README.md`

 * *Files identical despite different names*

### Comparing `antchain_partner-1.0.19/antchain_partner.egg-info/PKG-INFO` & `antchain_partner-1.0.20/antchain_partner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-partner
-Version: 1.0.19
+Version: 1.0.20
 Summary: Ant Chain PARTNER SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_partner-1.0.19/antchain_sdk_partner/client.py` & `antchain_partner-1.0.20/antchain_sdk_partner/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.19',
+                    'sdk_version': '1.0.20',
                     '_prod_code': 'PARTNER',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.19',
+                    'sdk_version': '1.0.20',
                     '_prod_code': 'PARTNER',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_partner-1.0.19/antchain_sdk_partner/models.py` & `antchain_partner-1.0.20/antchain_sdk_partner/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2742,23 +2742,29 @@
 class QueryAreaProvinceResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         provinces: List[Province] = None,
+        error_message: str = None,
+        code: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
         # 省份信息列表
         self.provinces = provinces
+        # 错误描述
+        self.error_message = error_message
+        # 结果码
+        self.code = code
 
     def validate(self):
         if self.provinces:
             for k in self.provinces:
                 if k:
                     k.validate()
 
@@ -2774,14 +2780,18 @@
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
         result['provinces'] = []
         if self.provinces is not None:
             for k in self.provinces:
                 result['provinces'].append(k.to_map() if k else None)
+        if self.error_message is not None:
+            result['error_message'] = self.error_message
+        if self.code is not None:
+            result['code'] = self.code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
@@ -2789,14 +2799,18 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         self.provinces = []
         if m.get('provinces') is not None:
             for k in m.get('provinces'):
                 temp_model = Province()
                 self.provinces.append(temp_model.from_map(k))
+        if m.get('error_message') is not None:
+            self.error_message = m.get('error_message')
+        if m.get('code') is not None:
+            self.code = m.get('code')
         return self
 
 
 class QueryAreaCityRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
@@ -2841,23 +2855,29 @@
 class QueryAreaCityResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         cities: List[City] = None,
+        code: str = None,
+        error_message: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
         # 城市列表
         self.cities = cities
+        # 结果码
+        self.code = code
+        # 错误描述
+        self.error_message = error_message
 
     def validate(self):
         if self.cities:
             for k in self.cities:
                 if k:
                     k.validate()
 
@@ -2873,14 +2893,18 @@
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
         result['cities'] = []
         if self.cities is not None:
             for k in self.cities:
                 result['cities'].append(k.to_map() if k else None)
+        if self.code is not None:
+            result['code'] = self.code
+        if self.error_message is not None:
+            result['error_message'] = self.error_message
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
@@ -2888,14 +2912,18 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         self.cities = []
         if m.get('cities') is not None:
             for k in m.get('cities'):
                 temp_model = City()
                 self.cities.append(temp_model.from_map(k))
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        if m.get('error_message') is not None:
+            self.error_message = m.get('error_message')
         return self
 
 
 class QueryPbcInstitutionRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
@@ -2933,23 +2961,29 @@
 class QueryPbcInstitutionResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         institutions: List[Institution] = None,
+        code: str = None,
+        error_message: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
         # 银行机构信息列表
         self.institutions = institutions
+        # 结果码
+        self.code = code
+        # 错误描述
+        self.error_message = error_message
 
     def validate(self):
         if self.institutions:
             for k in self.institutions:
                 if k:
                     k.validate()
 
@@ -2965,14 +2999,18 @@
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
         result['institutions'] = []
         if self.institutions is not None:
             for k in self.institutions:
                 result['institutions'].append(k.to_map() if k else None)
+        if self.code is not None:
+            result['code'] = self.code
+        if self.error_message is not None:
+            result['error_message'] = self.error_message
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
@@ -2980,14 +3018,18 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         self.institutions = []
         if m.get('institutions') is not None:
             for k in m.get('institutions'):
                 temp_model = Institution()
                 self.institutions.append(temp_model.from_map(k))
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        if m.get('error_message') is not None:
+            self.error_message = m.get('error_message')
         return self
 
 
 class QueryPbcNameRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
@@ -3049,23 +3091,29 @@
 class QueryPbcNameResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         pbc_infos: List[PbcInfo] = None,
+        error_message: str = None,
+        code: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
         # 查询到的支行信息列表
         self.pbc_infos = pbc_infos
+        # 错误描述
+        self.error_message = error_message
+        # 结果码
+        self.code = code
 
     def validate(self):
         if self.pbc_infos:
             for k in self.pbc_infos:
                 if k:
                     k.validate()
 
@@ -3081,14 +3129,18 @@
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
         result['pbc_infos'] = []
         if self.pbc_infos is not None:
             for k in self.pbc_infos:
                 result['pbc_infos'].append(k.to_map() if k else None)
+        if self.error_message is not None:
+            result['error_message'] = self.error_message
+        if self.code is not None:
+            result['code'] = self.code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
@@ -3096,10 +3148,14 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         self.pbc_infos = []
         if m.get('pbc_infos') is not None:
             for k in m.get('pbc_infos'):
                 temp_model = PbcInfo()
                 self.pbc_infos.append(temp_model.from_map(k))
+        if m.get('error_message') is not None:
+            self.error_message = m.get('error_message')
+        if m.get('code') is not None:
+            self.code = m.get('code')
         return self
```

### Comparing `antchain_partner-1.0.19/setup.py` & `antchain_partner-1.0.20/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_partner.
 
-Created on 23/04/2023
+Created on 25/04/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_partner"
 NAME = "antchain_partner" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain PARTNER SDK Library for Python"
```

