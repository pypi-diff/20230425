# Comparing `tmp/antchain_partner-1.0.20.tar.gz` & `tmp/antchain_partner-1.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_partner-1.0.20.tar", last modified: Tue Apr 25 01:52:16 2023, max compression
+gzip compressed data, was "dist/antchain_partner-1.0.21.tar", last modified: Tue Apr 25 03:03:41 2023, max compression
```

## Comparing `antchain_partner-1.0.20.tar` & `antchain_partner-1.0.21.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 01:52:16.000000 antchain_partner-1.0.20/
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-25 01:52:15.000000 antchain_partner-1.0.20/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-25 01:52:15.000000 antchain_partner-1.0.20/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2187 2023-04-25 01:52:16.000000 antchain_partner-1.0.20/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      816 2023-04-25 01:52:15.000000 antchain_partner-1.0.20/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1002 2023-04-25 01:52:15.000000 antchain_partner-1.0.20/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 01:52:16.000000 antchain_partner-1.0.20/antchain_partner.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2187 2023-04-25 01:52:16.000000 antchain_partner-1.0.20/antchain_partner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      355 2023-04-25 01:52:16.000000 antchain_partner-1.0.20/antchain_partner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 01:52:16.000000 antchain_partner-1.0.20/antchain_partner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-25 01:52:16.000000 antchain_partner-1.0.20/antchain_partner.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-25 01:52:16.000000 antchain_partner-1.0.20/antchain_partner.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 01:52:16.000000 antchain_partner-1.0.20/antchain_sdk_partner/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-25 01:52:15.000000 antchain_partner-1.0.20/antchain_sdk_partner/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46536 2023-04-25 01:52:15.000000 antchain_partner-1.0.20/antchain_sdk_partner/client.py
--rw-r--r--   0 root         (0) root         (0)   110481 2023-04-25 01:52:15.000000 antchain_partner-1.0.20/antchain_sdk_partner/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-25 01:52:16.000000 antchain_partner-1.0.20/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2508 2023-04-25 01:52:15.000000 antchain_partner-1.0.20/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 03:03:41.000000 antchain_partner-1.0.21/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2187 2023-04-25 03:03:41.000000 antchain_partner-1.0.21/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      816 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 03:03:41.000000 antchain_partner-1.0.21/antchain_partner.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2187 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/antchain_partner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      355 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/antchain_partner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/antchain_partner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/antchain_partner.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/antchain_partner.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 03:03:41.000000 antchain_partner-1.0.21/antchain_sdk_partner/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/antchain_sdk_partner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46536 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/antchain_sdk_partner/client.py
+-rw-r--r--   0 root         (0) root         (0)   111808 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/antchain_sdk_partner/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-25 03:03:41.000000 antchain_partner-1.0.21/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-04-25 03:03:40.000000 antchain_partner-1.0.21/setup.py
```

### Comparing `antchain_partner-1.0.20/LICENSE` & `antchain_partner-1.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_partner-1.0.20/PKG-INFO` & `antchain_partner-1.0.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_partner
-Version: 1.0.20
+Version: 1.0.21
 Summary: Ant Chain PARTNER SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_partner-1.0.20/README-CN.md` & `antchain_partner-1.0.21/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_partner-1.0.20/README.md` & `antchain_partner-1.0.21/README.md`

 * *Files identical despite different names*

### Comparing `antchain_partner-1.0.20/antchain_partner.egg-info/PKG-INFO` & `antchain_partner-1.0.21/antchain_partner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-partner
-Version: 1.0.20
+Version: 1.0.21
 Summary: Ant Chain PARTNER SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_partner-1.0.20/antchain_sdk_partner/client.py` & `antchain_partner-1.0.21/antchain_sdk_partner/client.py`

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
-                    'sdk_version': '1.0.20',
+                    'sdk_version': '1.0.21',
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
-                    'sdk_version': '1.0.20',
+                    'sdk_version': '1.0.21',
                     '_prod_code': 'PARTNER',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_partner-1.0.20/antchain_sdk_partner/models.py` & `antchain_partner-1.0.21/antchain_sdk_partner/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2705,41 +2705,48 @@
 
 
 class QueryAreaProvinceRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         province: str = None,
+        source: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         # 省份, 空:全部省份, 不为空筛选关键字省份
         self.province = province
+        # 租户来源-用于租户间功能和数据的隔离
+        self.source = source
 
     def validate(self):
-        pass
+        self.validate_required(self.source, 'source')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.province is not None:
             result['province'] = self.province
+        if self.source is not None:
+            result['source'] = self.source
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('province') is not None:
             self.province = m.get('province')
+        if m.get('source') is not None:
+            self.source = m.get('source')
         return self
 
 
 class QueryAreaProvinceResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -2812,47 +2819,55 @@
 
 class QueryAreaCityRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         province: str = None,
         city: str = None,
+        source: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         # 省份名称
         self.province = province
         # 城市
         self.city = city
+        # 租户来源-用于租户间功能和数据的隔离
+        self.source = source
 
     def validate(self):
         self.validate_required(self.province, 'province')
+        self.validate_required(self.source, 'source')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.province is not None:
             result['province'] = self.province
         if self.city is not None:
             result['city'] = self.city
+        if self.source is not None:
+            result['source'] = self.source
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('province') is not None:
             self.province = m.get('province')
         if m.get('city') is not None:
             self.city = m.get('city')
+        if m.get('source') is not None:
+            self.source = m.get('source')
         return self
 
 
 class QueryAreaCityResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -2924,41 +2939,49 @@
 
 
 class QueryPbcInstitutionRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         inst_name: str = None,
+        source: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         # 机构名称关键字
         self.inst_name = inst_name
+        # 租户来源-用于租户间功能和数据的隔离
+        self.source = source
 
     def validate(self):
         self.validate_required(self.inst_name, 'inst_name')
+        self.validate_required(self.source, 'source')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.inst_name is not None:
             result['inst_name'] = self.inst_name
+        if self.source is not None:
+            result['source'] = self.source
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('inst_name') is not None:
             self.inst_name = m.get('inst_name')
+        if m.get('source') is not None:
+            self.source = m.get('source')
         return self
 
 
 class QueryPbcInstitutionResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -3033,31 +3056,35 @@
     def __init__(
         self,
         auth_token: str = None,
         province: str = None,
         city: str = None,
         inst_id: str = None,
         branch_name: str = None,
+        source: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         # 省份名称
         self.province = province
         # 城市名称
         self.city = city
         # 银行机构id
         self.inst_id = inst_id
         # 支行名称关键字
         self.branch_name = branch_name
+        # 租户来源-用于租户间功能和数据的隔离
+        self.source = source
 
     def validate(self):
         self.validate_required(self.province, 'province')
         self.validate_required(self.city, 'city')
         self.validate_required(self.inst_id, 'inst_id')
         self.validate_required(self.branch_name, 'branch_name')
+        self.validate_required(self.source, 'source')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -3067,28 +3094,32 @@
             result['province'] = self.province
         if self.city is not None:
             result['city'] = self.city
         if self.inst_id is not None:
             result['inst_id'] = self.inst_id
         if self.branch_name is not None:
             result['branch_name'] = self.branch_name
+        if self.source is not None:
+            result['source'] = self.source
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('province') is not None:
             self.province = m.get('province')
         if m.get('city') is not None:
             self.city = m.get('city')
         if m.get('inst_id') is not None:
             self.inst_id = m.get('inst_id')
         if m.get('branch_name') is not None:
             self.branch_name = m.get('branch_name')
+        if m.get('source') is not None:
+            self.source = m.get('source')
         return self
 
 
 class QueryPbcNameResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
```

### Comparing `antchain_partner-1.0.20/setup.py` & `antchain_partner-1.0.21/setup.py`

 * *Files identical despite different names*

