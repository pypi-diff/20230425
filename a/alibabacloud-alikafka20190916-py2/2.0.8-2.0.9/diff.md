# Comparing `tmp/alibabacloud_alikafka20190916_py2-2.0.8.tar.gz` & `tmp/alibabacloud_alikafka20190916_py2-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_alikafka20190916_py2-2.0.8.tar", last modified: Mon Sep  5 12:45:52 2022, max compression
+gzip compressed data, was "dist/alibabacloud_alikafka20190916_py2-2.0.9.tar", last modified: Fri Nov 18 03:15:13 2022, max compression
```

## Comparing `alibabacloud_alikafka20190916_py2-2.0.8.tar` & `alibabacloud_alikafka20190916_py2-2.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-05 12:45:52.000000 alibabacloud_alikafka20190916_py2-2.0.8/
--rw-r--r--   0 root         (0) root         (0)      498 2022-09-05 12:45:51.000000 alibabacloud_alikafka20190916_py2-2.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2022-09-05 12:45:51.000000 alibabacloud_alikafka20190916_py2-2.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-09-05 12:45:51.000000 alibabacloud_alikafka20190916_py2-2.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2506 2022-09-05 12:45:52.000000 alibabacloud_alikafka20190916_py2-2.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2022-09-05 12:45:51.000000 alibabacloud_alikafka20190916_py2-2.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2022-09-05 12:45:51.000000 alibabacloud_alikafka20190916_py2-2.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-05 12:45:52.000000 alibabacloud_alikafka20190916_py2-2.0.8/alibabacloud_alikafka20190916/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-05 12:45:51.000000 alibabacloud_alikafka20190916_py2-2.0.8/alibabacloud_alikafka20190916/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55673 2022-09-05 12:45:51.000000 alibabacloud_alikafka20190916_py2-2.0.8/alibabacloud_alikafka20190916/client.py
--rw-r--r--   0 root         (0) root         (0)   215337 2022-09-05 12:45:51.000000 alibabacloud_alikafka20190916_py2-2.0.8/alibabacloud_alikafka20190916/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-05 12:45:52.000000 alibabacloud_alikafka20190916_py2-2.0.8/alibabacloud_alikafka20190916_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2506 2022-09-05 12:45:52.000000 alibabacloud_alikafka20190916_py2-2.0.8/alibabacloud_alikafka20190916_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2022-09-05 12:45:52.000000 alibabacloud_alikafka20190916_py2-2.0.8/alibabacloud_alikafka20190916_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-05 12:45:52.000000 alibabacloud_alikafka20190916_py2-2.0.8/alibabacloud_alikafka20190916_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2022-09-05 12:45:52.000000 alibabacloud_alikafka20190916_py2-2.0.8/alibabacloud_alikafka20190916_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-09-05 12:45:52.000000 alibabacloud_alikafka20190916_py2-2.0.8/alibabacloud_alikafka20190916_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-09-05 12:45:52.000000 alibabacloud_alikafka20190916_py2-2.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2932 2022-09-05 12:45:51.000000 alibabacloud_alikafka20190916_py2-2.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 03:15:13.000000 alibabacloud_alikafka20190916_py2-2.0.9/
+-rw-r--r--   0 root         (0) root         (0)      577 2022-11-18 03:15:13.000000 alibabacloud_alikafka20190916_py2-2.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2022-11-18 03:15:13.000000 alibabacloud_alikafka20190916_py2-2.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2022-11-18 03:15:13.000000 alibabacloud_alikafka20190916_py2-2.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2506 2022-11-18 03:15:13.000000 alibabacloud_alikafka20190916_py2-2.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2022-11-18 03:15:13.000000 alibabacloud_alikafka20190916_py2-2.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2022-11-18 03:15:13.000000 alibabacloud_alikafka20190916_py2-2.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 03:15:13.000000 alibabacloud_alikafka20190916_py2-2.0.9/alibabacloud_alikafka20190916/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-11-18 03:15:13.000000 alibabacloud_alikafka20190916_py2-2.0.9/alibabacloud_alikafka20190916/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56102 2022-11-18 03:15:13.000000 alibabacloud_alikafka20190916_py2-2.0.9/alibabacloud_alikafka20190916/client.py
+-rw-r--r--   0 root         (0) root         (0)   225840 2022-11-18 03:15:13.000000 alibabacloud_alikafka20190916_py2-2.0.9/alibabacloud_alikafka20190916/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 03:15:13.000000 alibabacloud_alikafka20190916_py2-2.0.9/alibabacloud_alikafka20190916_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2506 2022-11-18 03:15:13.000000 alibabacloud_alikafka20190916_py2-2.0.9/alibabacloud_alikafka20190916_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2022-11-18 03:15:13.000000 alibabacloud_alikafka20190916_py2-2.0.9/alibabacloud_alikafka20190916_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-18 03:15:13.000000 alibabacloud_alikafka20190916_py2-2.0.9/alibabacloud_alikafka20190916_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2022-11-18 03:15:13.000000 alibabacloud_alikafka20190916_py2-2.0.9/alibabacloud_alikafka20190916_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2022-11-18 03:15:13.000000 alibabacloud_alikafka20190916_py2-2.0.9/alibabacloud_alikafka20190916_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-11-18 03:15:13.000000 alibabacloud_alikafka20190916_py2-2.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2932 2022-11-18 03:15:13.000000 alibabacloud_alikafka20190916_py2-2.0.9/setup.py
```

### Comparing `alibabacloud_alikafka20190916_py2-2.0.8/LICENSE` & `alibabacloud_alikafka20190916_py2-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916_py2-2.0.8/PKG-INFO` & `alibabacloud_alikafka20190916_py2-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_alikafka20190916_py2
-Version: 2.0.8
+Version: 2.0.9
 Summary: Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alikafka20190916_py2-2.0.8/README-CN.md` & `alibabacloud_alikafka20190916_py2-2.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916_py2-2.0.8/README.md` & `alibabacloud_alikafka20190916_py2-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916_py2-2.0.8/alibabacloud_alikafka20190916/client.py` & `alibabacloud_alikafka20190916_py2-2.0.9/alibabacloud_alikafka20190916/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,14 +178,16 @@
             query['ConsumerId'] = request.consumer_id
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.remark):
             query['Remark'] = request.remark
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateConsumerGroup',
             version='2019-09-16',
             protocol='HTTPS',
@@ -224,14 +226,16 @@
             query['PartitionNum'] = request.partition_num
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.spec_type):
             query['SpecType'] = request.spec_type
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         if not UtilClient.is_unset(request.topic_quota):
             query['TopicQuota'] = request.topic_quota
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreatePostPayOrder',
@@ -272,14 +276,16 @@
             query['PartitionNum'] = request.partition_num
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.spec_type):
             query['SpecType'] = request.spec_type
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         if not UtilClient.is_unset(request.topic_quota):
             query['TopicQuota'] = request.topic_quota
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreatePrePayOrder',
@@ -358,14 +364,16 @@
             query['PartitionNum'] = request.partition_num
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.remark):
             query['Remark'] = request.remark
         if not UtilClient.is_unset(request.replication_factor):
             query['ReplicationFactor'] = request.replication_factor
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
         if not UtilClient.is_unset(request.topic):
             query['Topic'] = request.topic
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='CreateTopic',
@@ -589,44 +597,14 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_acls(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_acls_with_options(request, runtime)
 
-    def describe_node_status_with_options(self, request, runtime):
-        UtilClient.validate_model(request)
-        query = {}
-        if not UtilClient.is_unset(request.instance_id):
-            query['InstanceId'] = request.instance_id
-        if not UtilClient.is_unset(request.region_id):
-            query['RegionId'] = request.region_id
-        req = open_api_models.OpenApiRequest(
-            query=OpenApiUtilClient.query(query)
-        )
-        params = open_api_models.Params(
-            action='DescribeNodeStatus',
-            version='2019-09-16',
-            protocol='HTTPS',
-            pathname='/',
-            method='POST',
-            auth_type='AK',
-            style='RPC',
-            req_body_type='formData',
-            body_type='json'
-        )
-        return TeaCore.from_map(
-            alikafka_20190916_models.DescribeNodeStatusResponse(),
-            self.call_api(params, req, runtime)
-        )
-
-    def describe_node_status(self, request):
-        runtime = util_models.RuntimeOptions()
-        return self.describe_node_status_with_options(request, runtime)
-
     def describe_sasl_users_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
@@ -807,14 +785,44 @@
             self.call_api(params, req, runtime)
         )
 
     def get_instance_list(self, request):
         runtime = util_models.RuntimeOptions()
         return self.get_instance_list_with_options(request, runtime)
 
+    def get_quota_tip_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetQuotaTip',
+            version='2019-09-16',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            alikafka_20190916_models.GetQuotaTipResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def get_quota_tip(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.get_quota_tip_with_options(request, runtime)
+
     def get_topic_list_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.current_page):
             query['CurrentPage'] = request.current_page
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
@@ -1186,14 +1194,16 @@
     def update_allowed_ip_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.allowed_list_ip):
             query['AllowedListIp'] = request.allowed_list_ip
         if not UtilClient.is_unset(request.allowed_list_type):
             query['AllowedListType'] = request.allowed_list_type
+        if not UtilClient.is_unset(request.description):
+            query['Description'] = request.description
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.port_range):
             query['PortRange'] = request.port_range
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.update_type):
```

### Comparing `alibabacloud_alikafka20190916_py2-2.0.8/alibabacloud_alikafka20190916/models.py` & `alibabacloud_alikafka20190916_py2-2.0.9/alibabacloud_alikafka20190916/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,23 +366,56 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateAclResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateConsumerGroupRequestTag(TeaModel):
+    def __init__(self, key=None, value=None):
+        self.key = key  # type: str
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateConsumerGroupRequestTag, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class CreateConsumerGroupRequest(TeaModel):
-    def __init__(self, consumer_id=None, instance_id=None, region_id=None, remark=None):
+    def __init__(self, consumer_id=None, instance_id=None, region_id=None, remark=None, tag=None):
         self.consumer_id = consumer_id  # type: str
         self.instance_id = instance_id  # type: str
         self.region_id = region_id  # type: str
         self.remark = remark  # type: str
+        self.tag = tag  # type: list[CreateConsumerGroupRequestTag]
 
     def validate(self):
-        pass
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super(CreateConsumerGroupRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -390,26 +423,35 @@
             result['ConsumerId'] = self.consumer_id
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.remark is not None:
             result['Remark'] = self.remark
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ConsumerId') is not None:
             self.consumer_id = m.get('ConsumerId')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('Remark') is not None:
             self.remark = m.get('Remark')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = CreateConsumerGroupRequestTag()
+                self.tag.append(temp_model.from_map(k))
         return self
 
 
 class CreateConsumerGroupResponseBody(TeaModel):
     def __init__(self, code=None, message=None, request_id=None, success=None):
         self.code = code  # type: int
         self.message = message  # type: str
@@ -483,31 +525,64 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateConsumerGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreatePostPayOrderRequestTag(TeaModel):
+    def __init__(self, key=None, value=None):
+        self.key = key  # type: str
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreatePostPayOrderRequestTag, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class CreatePostPayOrderRequest(TeaModel):
     def __init__(self, deploy_type=None, disk_size=None, disk_type=None, eip_max=None, io_max=None, io_max_spec=None,
-                 partition_num=None, region_id=None, resource_group_id=None, spec_type=None, topic_quota=None):
+                 partition_num=None, region_id=None, resource_group_id=None, spec_type=None, tag=None, topic_quota=None):
         self.deploy_type = deploy_type  # type: int
         self.disk_size = disk_size  # type: int
         self.disk_type = disk_type  # type: str
         self.eip_max = eip_max  # type: int
         self.io_max = io_max  # type: int
         self.io_max_spec = io_max_spec  # type: str
         self.partition_num = partition_num  # type: int
         self.region_id = region_id  # type: str
         self.resource_group_id = resource_group_id  # type: str
         self.spec_type = spec_type  # type: str
+        self.tag = tag  # type: list[CreatePostPayOrderRequestTag]
         self.topic_quota = topic_quota  # type: int
 
     def validate(self):
-        pass
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super(CreatePostPayOrderRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -527,14 +602,18 @@
             result['PartitionNum'] = self.partition_num
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
         if self.spec_type is not None:
             result['SpecType'] = self.spec_type
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
         if self.topic_quota is not None:
             result['TopicQuota'] = self.topic_quota
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('DeployType') is not None:
@@ -553,14 +632,19 @@
             self.partition_num = m.get('PartitionNum')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         if m.get('SpecType') is not None:
             self.spec_type = m.get('SpecType')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = CreatePostPayOrderRequestTag()
+                self.tag.append(temp_model.from_map(k))
         if m.get('TopicQuota') is not None:
             self.topic_quota = m.get('TopicQuota')
         return self
 
 
 class CreatePostPayOrderResponseBody(TeaModel):
     def __init__(self, code=None, message=None, order_id=None, request_id=None, success=None):
@@ -641,31 +725,64 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreatePostPayOrderResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreatePrePayOrderRequestTag(TeaModel):
+    def __init__(self, key=None, value=None):
+        self.key = key  # type: str
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreatePrePayOrderRequestTag, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class CreatePrePayOrderRequest(TeaModel):
     def __init__(self, deploy_type=None, disk_size=None, disk_type=None, eip_max=None, io_max=None, io_max_spec=None,
-                 partition_num=None, region_id=None, resource_group_id=None, spec_type=None, topic_quota=None):
+                 partition_num=None, region_id=None, resource_group_id=None, spec_type=None, tag=None, topic_quota=None):
         self.deploy_type = deploy_type  # type: int
         self.disk_size = disk_size  # type: int
         self.disk_type = disk_type  # type: str
         self.eip_max = eip_max  # type: int
         self.io_max = io_max  # type: int
         self.io_max_spec = io_max_spec  # type: str
         self.partition_num = partition_num  # type: int
         self.region_id = region_id  # type: str
         self.resource_group_id = resource_group_id  # type: str
         self.spec_type = spec_type  # type: str
+        self.tag = tag  # type: list[CreatePrePayOrderRequestTag]
         self.topic_quota = topic_quota  # type: int
 
     def validate(self):
-        pass
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super(CreatePrePayOrderRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -685,14 +802,18 @@
             result['PartitionNum'] = self.partition_num
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
         if self.spec_type is not None:
             result['SpecType'] = self.spec_type
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
         if self.topic_quota is not None:
             result['TopicQuota'] = self.topic_quota
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('DeployType') is not None:
@@ -711,14 +832,19 @@
             self.partition_num = m.get('PartitionNum')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         if m.get('SpecType') is not None:
             self.spec_type = m.get('SpecType')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = CreatePrePayOrderRequestTag()
+                self.tag.append(temp_model.from_map(k))
         if m.get('TopicQuota') is not None:
             self.topic_quota = m.get('TopicQuota')
         return self
 
 
 class CreatePrePayOrderResponseBody(TeaModel):
     def __init__(self, code=None, message=None, order_id=None, request_id=None, success=None):
@@ -921,30 +1047,64 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateSaslUserResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateTopicRequestTag(TeaModel):
+    def __init__(self, key=None, value=None):
+        self.key = key  # type: str
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateTopicRequestTag, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class CreateTopicRequest(TeaModel):
     def __init__(self, compact_topic=None, config=None, instance_id=None, local_topic=None,
-                 min_insync_replicas=None, partition_num=None, region_id=None, remark=None, replication_factor=None, topic=None):
+                 min_insync_replicas=None, partition_num=None, region_id=None, remark=None, replication_factor=None, tag=None,
+                 topic=None):
         self.compact_topic = compact_topic  # type: bool
         self.config = config  # type: dict[str, any]
         self.instance_id = instance_id  # type: str
         self.local_topic = local_topic  # type: bool
         self.min_insync_replicas = min_insync_replicas  # type: long
         self.partition_num = partition_num  # type: str
         self.region_id = region_id  # type: str
         self.remark = remark  # type: str
         self.replication_factor = replication_factor  # type: long
+        self.tag = tag  # type: list[CreateTopicRequestTag]
         self.topic = topic  # type: str
 
     def validate(self):
-        pass
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super(CreateTopicRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -962,14 +1122,18 @@
             result['PartitionNum'] = self.partition_num
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.remark is not None:
             result['Remark'] = self.remark
         if self.replication_factor is not None:
             result['ReplicationFactor'] = self.replication_factor
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
         if self.topic is not None:
             result['Topic'] = self.topic
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('CompactTopic') is not None:
@@ -986,35 +1150,74 @@
             self.partition_num = m.get('PartitionNum')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('Remark') is not None:
             self.remark = m.get('Remark')
         if m.get('ReplicationFactor') is not None:
             self.replication_factor = m.get('ReplicationFactor')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = CreateTopicRequestTag()
+                self.tag.append(temp_model.from_map(k))
         if m.get('Topic') is not None:
             self.topic = m.get('Topic')
         return self
 
 
+class CreateTopicShrinkRequestTag(TeaModel):
+    def __init__(self, key=None, value=None):
+        self.key = key  # type: str
+        self.value = value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateTopicShrinkRequestTag, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class CreateTopicShrinkRequest(TeaModel):
     def __init__(self, compact_topic=None, config_shrink=None, instance_id=None, local_topic=None,
-                 min_insync_replicas=None, partition_num=None, region_id=None, remark=None, replication_factor=None, topic=None):
+                 min_insync_replicas=None, partition_num=None, region_id=None, remark=None, replication_factor=None, tag=None,
+                 topic=None):
         self.compact_topic = compact_topic  # type: bool
         self.config_shrink = config_shrink  # type: str
         self.instance_id = instance_id  # type: str
         self.local_topic = local_topic  # type: bool
         self.min_insync_replicas = min_insync_replicas  # type: long
         self.partition_num = partition_num  # type: str
         self.region_id = region_id  # type: str
         self.remark = remark  # type: str
         self.replication_factor = replication_factor  # type: long
+        self.tag = tag  # type: list[CreateTopicShrinkRequestTag]
         self.topic = topic  # type: str
 
     def validate(self):
-        pass
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super(CreateTopicShrinkRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -1032,14 +1235,18 @@
             result['PartitionNum'] = self.partition_num
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.remark is not None:
             result['Remark'] = self.remark
         if self.replication_factor is not None:
             result['ReplicationFactor'] = self.replication_factor
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
         if self.topic is not None:
             result['Topic'] = self.topic
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('CompactTopic') is not None:
@@ -1056,14 +1263,19 @@
             self.partition_num = m.get('PartitionNum')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('Remark') is not None:
             self.remark = m.get('Remark')
         if m.get('ReplicationFactor') is not None:
             self.replication_factor = m.get('ReplicationFactor')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = CreateTopicShrinkRequestTag()
+                self.tag.append(temp_model.from_map(k))
         if m.get('Topic') is not None:
             self.topic = m.get('Topic')
         return self
 
 
 class CreateTopicResponseBody(TeaModel):
     def __init__(self, code=None, message=None, request_id=None, success=None):
@@ -1937,152 +2149,14 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeAclsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class DescribeNodeStatusRequest(TeaModel):
-    def __init__(self, instance_id=None, region_id=None):
-        self.instance_id = instance_id  # type: str
-        self.region_id = region_id  # type: str
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeNodeStatusRequest, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.instance_id is not None:
-            result['InstanceId'] = self.instance_id
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('InstanceId') is not None:
-            self.instance_id = m.get('InstanceId')
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
-        return self
-
-
-class DescribeNodeStatusResponseBodyStatusList(TeaModel):
-    def __init__(self, status=None):
-        self.status = status  # type: list[str]
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super(DescribeNodeStatusResponseBodyStatusList, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.status is not None:
-            result['Status'] = self.status
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Status') is not None:
-            self.status = m.get('Status')
-        return self
-
-
-class DescribeNodeStatusResponseBody(TeaModel):
-    def __init__(self, code=None, message=None, request_id=None, status_list=None, success=None):
-        self.code = code  # type: int
-        self.message = message  # type: str
-        self.request_id = request_id  # type: str
-        self.status_list = status_list  # type: DescribeNodeStatusResponseBodyStatusList
-        self.success = success  # type: bool
-
-    def validate(self):
-        if self.status_list:
-            self.status_list.validate()
-
-    def to_map(self):
-        _map = super(DescribeNodeStatusResponseBody, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.code is not None:
-            result['Code'] = self.code
-        if self.message is not None:
-            result['Message'] = self.message
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.status_list is not None:
-            result['StatusList'] = self.status_list.to_map()
-        if self.success is not None:
-            result['Success'] = self.success
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('Code') is not None:
-            self.code = m.get('Code')
-        if m.get('Message') is not None:
-            self.message = m.get('Message')
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('StatusList') is not None:
-            temp_model = DescribeNodeStatusResponseBodyStatusList()
-            self.status_list = temp_model.from_map(m['StatusList'])
-        if m.get('Success') is not None:
-            self.success = m.get('Success')
-        return self
-
-
-class DescribeNodeStatusResponse(TeaModel):
-    def __init__(self, headers=None, status_code=None, body=None):
-        self.headers = headers  # type: dict[str, str]
-        self.status_code = status_code  # type: int
-        self.body = body  # type: DescribeNodeStatusResponseBody
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super(DescribeNodeStatusResponse, self).to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m=None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = DescribeNodeStatusResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
 class DescribeSaslUsersRequest(TeaModel):
     def __init__(self, instance_id=None, region_id=None):
         self.instance_id = instance_id  # type: str
         self.region_id = region_id  # type: str
 
     def validate(self):
         pass
@@ -2392,64 +2466,74 @@
             self.instance_id = m.get('InstanceId')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         return self
 
 
 class GetAllowedIpListResponseBodyAllowedListInternetList(TeaModel):
-    def __init__(self, allowed_ip_list=None, port_range=None):
+    def __init__(self, allowed_ip_group=None, allowed_ip_list=None, port_range=None):
+        self.allowed_ip_group = allowed_ip_group  # type: dict[str, str]
         self.allowed_ip_list = allowed_ip_list  # type: list[str]
         self.port_range = port_range  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetAllowedIpListResponseBodyAllowedListInternetList, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.allowed_ip_group is not None:
+            result['AllowedIpGroup'] = self.allowed_ip_group
         if self.allowed_ip_list is not None:
             result['AllowedIpList'] = self.allowed_ip_list
         if self.port_range is not None:
             result['PortRange'] = self.port_range
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('AllowedIpGroup') is not None:
+            self.allowed_ip_group = m.get('AllowedIpGroup')
         if m.get('AllowedIpList') is not None:
             self.allowed_ip_list = m.get('AllowedIpList')
         if m.get('PortRange') is not None:
             self.port_range = m.get('PortRange')
         return self
 
 
 class GetAllowedIpListResponseBodyAllowedListVpcList(TeaModel):
-    def __init__(self, allowed_ip_list=None, port_range=None):
+    def __init__(self, allowed_ip_group=None, allowed_ip_list=None, port_range=None):
+        self.allowed_ip_group = allowed_ip_group  # type: dict[str, str]
         self.allowed_ip_list = allowed_ip_list  # type: list[str]
         self.port_range = port_range  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetAllowedIpListResponseBodyAllowedListVpcList, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.allowed_ip_group is not None:
+            result['AllowedIpGroup'] = self.allowed_ip_group
         if self.allowed_ip_list is not None:
             result['AllowedIpList'] = self.allowed_ip_list
         if self.port_range is not None:
             result['PortRange'] = self.port_range
         return result
 
     def from_map(self, m=None):
         m = m or dict()
+        if m.get('AllowedIpGroup') is not None:
+            self.allowed_ip_group = m.get('AllowedIpGroup')
         if m.get('AllowedIpList') is not None:
             self.allowed_ip_list = m.get('AllowedIpList')
         if m.get('PortRange') is not None:
             self.port_range = m.get('PortRange')
         return self
 
 
@@ -3313,16 +3397,17 @@
 
 
 class GetInstanceListResponseBodyInstanceListInstanceVO(TeaModel):
     def __init__(self, all_config=None, create_time=None, deploy_type=None, disk_size=None, disk_type=None,
                  domain_endpoint=None, eip_max=None, end_point=None, expired_time=None, instance_id=None, io_max=None,
                  kms_key_id=None, msg_retain=None, name=None, paid_type=None, region_id=None, resource_group_id=None,
                  sasl_domain_endpoint=None, security_group=None, service_status=None, spec_type=None, ssl_domain_endpoint=None,
-                 ssl_end_point=None, tags=None, topic_num_limit=None, upgrade_service_detail_info=None, used_group_count=None,
-                 used_partition_count=None, used_topic_count=None, v_switch_id=None, vpc_id=None, zone_id=None):
+                 ssl_end_point=None, standard_zone_id=None, tags=None, topic_num_limit=None, upgrade_service_detail_info=None,
+                 used_group_count=None, used_partition_count=None, used_topic_count=None, v_switch_id=None, vpc_id=None,
+                 zone_id=None):
         self.all_config = all_config  # type: str
         self.create_time = create_time  # type: long
         self.deploy_type = deploy_type  # type: int
         self.disk_size = disk_size  # type: int
         self.disk_type = disk_type  # type: int
         self.domain_endpoint = domain_endpoint  # type: str
         self.eip_max = eip_max  # type: int
@@ -3338,14 +3423,15 @@
         self.resource_group_id = resource_group_id  # type: str
         self.sasl_domain_endpoint = sasl_domain_endpoint  # type: str
         self.security_group = security_group  # type: str
         self.service_status = service_status  # type: int
         self.spec_type = spec_type  # type: str
         self.ssl_domain_endpoint = ssl_domain_endpoint  # type: str
         self.ssl_end_point = ssl_end_point  # type: str
+        self.standard_zone_id = standard_zone_id  # type: str
         self.tags = tags  # type: GetInstanceListResponseBodyInstanceListInstanceVOTags
         self.topic_num_limit = topic_num_limit  # type: int
         self.upgrade_service_detail_info = upgrade_service_detail_info  # type: GetInstanceListResponseBodyInstanceListInstanceVOUpgradeServiceDetailInfo
         self.used_group_count = used_group_count  # type: int
         self.used_partition_count = used_partition_count  # type: int
         self.used_topic_count = used_topic_count  # type: int
         self.v_switch_id = v_switch_id  # type: str
@@ -3406,14 +3492,16 @@
             result['ServiceStatus'] = self.service_status
         if self.spec_type is not None:
             result['SpecType'] = self.spec_type
         if self.ssl_domain_endpoint is not None:
             result['SslDomainEndpoint'] = self.ssl_domain_endpoint
         if self.ssl_end_point is not None:
             result['SslEndPoint'] = self.ssl_end_point
+        if self.standard_zone_id is not None:
+            result['StandardZoneId'] = self.standard_zone_id
         if self.tags is not None:
             result['Tags'] = self.tags.to_map()
         if self.topic_num_limit is not None:
             result['TopicNumLimit'] = self.topic_num_limit
         if self.upgrade_service_detail_info is not None:
             result['UpgradeServiceDetailInfo'] = self.upgrade_service_detail_info.to_map()
         if self.used_group_count is not None:
@@ -3474,14 +3562,16 @@
             self.service_status = m.get('ServiceStatus')
         if m.get('SpecType') is not None:
             self.spec_type = m.get('SpecType')
         if m.get('SslDomainEndpoint') is not None:
             self.ssl_domain_endpoint = m.get('SslDomainEndpoint')
         if m.get('SslEndPoint') is not None:
             self.ssl_end_point = m.get('SslEndPoint')
+        if m.get('StandardZoneId') is not None:
+            self.standard_zone_id = m.get('StandardZoneId')
         if m.get('Tags') is not None:
             temp_model = GetInstanceListResponseBodyInstanceListInstanceVOTags()
             self.tags = temp_model.from_map(m['Tags'])
         if m.get('TopicNumLimit') is not None:
             self.topic_num_limit = m.get('TopicNumLimit')
         if m.get('UpgradeServiceDetailInfo') is not None:
             temp_model = GetInstanceListResponseBodyInstanceListInstanceVOUpgradeServiceDetailInfo()
@@ -3614,14 +3704,204 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetInstanceListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetQuotaTipRequest(TeaModel):
+    def __init__(self, instance_id=None, region_id=None):
+        self.instance_id = instance_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetQuotaTipRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class GetQuotaTipResponseBodyQuotaData(TeaModel):
+    def __init__(self, group_left=None, group_used=None, is_partition_buy=None, partition_left=None,
+                 partition_num_of_buy=None, partition_quata=None, partition_used=None, topic_left=None, topic_num_of_buy=None,
+                 topic_quota=None, topic_used=None):
+        self.group_left = group_left  # type: int
+        self.group_used = group_used  # type: int
+        self.is_partition_buy = is_partition_buy  # type: int
+        self.partition_left = partition_left  # type: int
+        self.partition_num_of_buy = partition_num_of_buy  # type: int
+        self.partition_quata = partition_quata  # type: int
+        self.partition_used = partition_used  # type: int
+        self.topic_left = topic_left  # type: int
+        self.topic_num_of_buy = topic_num_of_buy  # type: int
+        self.topic_quota = topic_quota  # type: int
+        self.topic_used = topic_used  # type: int
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetQuotaTipResponseBodyQuotaData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.group_left is not None:
+            result['GroupLeft'] = self.group_left
+        if self.group_used is not None:
+            result['GroupUsed'] = self.group_used
+        if self.is_partition_buy is not None:
+            result['IsPartitionBuy'] = self.is_partition_buy
+        if self.partition_left is not None:
+            result['PartitionLeft'] = self.partition_left
+        if self.partition_num_of_buy is not None:
+            result['PartitionNumOfBuy'] = self.partition_num_of_buy
+        if self.partition_quata is not None:
+            result['PartitionQuata'] = self.partition_quata
+        if self.partition_used is not None:
+            result['PartitionUsed'] = self.partition_used
+        if self.topic_left is not None:
+            result['TopicLeft'] = self.topic_left
+        if self.topic_num_of_buy is not None:
+            result['TopicNumOfBuy'] = self.topic_num_of_buy
+        if self.topic_quota is not None:
+            result['TopicQuota'] = self.topic_quota
+        if self.topic_used is not None:
+            result['TopicUsed'] = self.topic_used
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('GroupLeft') is not None:
+            self.group_left = m.get('GroupLeft')
+        if m.get('GroupUsed') is not None:
+            self.group_used = m.get('GroupUsed')
+        if m.get('IsPartitionBuy') is not None:
+            self.is_partition_buy = m.get('IsPartitionBuy')
+        if m.get('PartitionLeft') is not None:
+            self.partition_left = m.get('PartitionLeft')
+        if m.get('PartitionNumOfBuy') is not None:
+            self.partition_num_of_buy = m.get('PartitionNumOfBuy')
+        if m.get('PartitionQuata') is not None:
+            self.partition_quata = m.get('PartitionQuata')
+        if m.get('PartitionUsed') is not None:
+            self.partition_used = m.get('PartitionUsed')
+        if m.get('TopicLeft') is not None:
+            self.topic_left = m.get('TopicLeft')
+        if m.get('TopicNumOfBuy') is not None:
+            self.topic_num_of_buy = m.get('TopicNumOfBuy')
+        if m.get('TopicQuota') is not None:
+            self.topic_quota = m.get('TopicQuota')
+        if m.get('TopicUsed') is not None:
+            self.topic_used = m.get('TopicUsed')
+        return self
+
+
+class GetQuotaTipResponseBody(TeaModel):
+    def __init__(self, code=None, message=None, quota_data=None, request_id=None, success=None):
+        self.code = code  # type: int
+        self.message = message  # type: str
+        self.quota_data = quota_data  # type: GetQuotaTipResponseBodyQuotaData
+        self.request_id = request_id  # type: str
+        self.success = success  # type: bool
+
+    def validate(self):
+        if self.quota_data:
+            self.quota_data.validate()
+
+    def to_map(self):
+        _map = super(GetQuotaTipResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.quota_data is not None:
+            result['QuotaData'] = self.quota_data.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('QuotaData') is not None:
+            temp_model = GetQuotaTipResponseBodyQuotaData()
+            self.quota_data = temp_model.from_map(m['QuotaData'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetQuotaTipResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetQuotaTipResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetQuotaTipResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetQuotaTipResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetTopicListRequest(TeaModel):
     def __init__(self, current_page=None, instance_id=None, page_size=None, region_id=None, topic=None):
         self.current_page = current_page  # type: str
         self.instance_id = instance_id  # type: str
         self.page_size = page_size  # type: str
         self.region_id = region_id  # type: str
         self.topic = topic  # type: str
@@ -5292,18 +5572,19 @@
         if m.get('body') is not None:
             temp_model = UntagResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateAllowedIpRequest(TeaModel):
-    def __init__(self, allowed_list_ip=None, allowed_list_type=None, instance_id=None, port_range=None,
-                 region_id=None, update_type=None):
+    def __init__(self, allowed_list_ip=None, allowed_list_type=None, description=None, instance_id=None,
+                 port_range=None, region_id=None, update_type=None):
         self.allowed_list_ip = allowed_list_ip  # type: str
         self.allowed_list_type = allowed_list_type  # type: str
+        self.description = description  # type: str
         self.instance_id = instance_id  # type: str
         self.port_range = port_range  # type: str
         self.region_id = region_id  # type: str
         self.update_type = update_type  # type: str
 
     def validate(self):
         pass
@@ -5314,14 +5595,16 @@
             return _map
 
         result = dict()
         if self.allowed_list_ip is not None:
             result['AllowedListIp'] = self.allowed_list_ip
         if self.allowed_list_type is not None:
             result['AllowedListType'] = self.allowed_list_type
+        if self.description is not None:
+            result['Description'] = self.description
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.port_range is not None:
             result['PortRange'] = self.port_range
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.update_type is not None:
@@ -5330,14 +5613,16 @@
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('AllowedListIp') is not None:
             self.allowed_list_ip = m.get('AllowedListIp')
         if m.get('AllowedListType') is not None:
             self.allowed_list_type = m.get('AllowedListType')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('PortRange') is not None:
             self.port_range = m.get('PortRange')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('UpdateType') is not None:
```

### Comparing `alibabacloud_alikafka20190916_py2-2.0.8/alibabacloud_alikafka20190916_py2.egg-info/PKG-INFO` & `alibabacloud_alikafka20190916_py2-2.0.9/alibabacloud_alikafka20190916_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-alikafka20190916-py2
-Version: 2.0.8
+Version: 2.0.9
 Summary: Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alikafka20190916_py2-2.0.8/setup.py` & `alibabacloud_alikafka20190916_py2-2.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,30 +21,30 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_alikafka20190916_py2.
 
-Created on 05/09/2022
+Created on 18/11/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_alikafka20190916"
 NAME = "alibabacloud_alikafka20190916_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.6, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.3, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.0, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

