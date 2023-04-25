# Comparing `tmp/alibabacloud_alikafka20190916-2.0.8.tar.gz` & `tmp/alibabacloud_alikafka20190916-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_alikafka20190916-2.0.8.tar", last modified: Mon Sep  5 12:46:27 2022, max compression
+gzip compressed data, was "dist/alibabacloud_alikafka20190916-2.0.9.tar", last modified: Fri Nov 18 03:15:44 2022, max compression
```

## Comparing `alibabacloud_alikafka20190916-2.0.8.tar` & `alibabacloud_alikafka20190916-2.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-05 12:46:27.000000 alibabacloud_alikafka20190916-2.0.8/
--rw-r--r--   0 root         (0) root         (0)      757 2022-09-05 12:46:27.000000 alibabacloud_alikafka20190916-2.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-09-05 12:46:27.000000 alibabacloud_alikafka20190916-2.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-09-05 12:46:27.000000 alibabacloud_alikafka20190916-2.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2362 2022-09-05 12:46:27.000000 alibabacloud_alikafka20190916-2.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2022-09-05 12:46:27.000000 alibabacloud_alikafka20190916-2.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2022-09-05 12:46:27.000000 alibabacloud_alikafka20190916-2.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-05 12:46:27.000000 alibabacloud_alikafka20190916-2.0.8/alibabacloud_alikafka20190916/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-05 12:46:27.000000 alibabacloud_alikafka20190916-2.0.8/alibabacloud_alikafka20190916/__init__.py
--rw-r--r--   0 root         (0) root         (0)   130352 2022-09-05 12:46:27.000000 alibabacloud_alikafka20190916-2.0.8/alibabacloud_alikafka20190916/client.py
--rw-r--r--   0 root         (0) root         (0)   214243 2022-09-05 12:46:27.000000 alibabacloud_alikafka20190916-2.0.8/alibabacloud_alikafka20190916/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-05 12:46:27.000000 alibabacloud_alikafka20190916-2.0.8/alibabacloud_alikafka20190916.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2362 2022-09-05 12:46:27.000000 alibabacloud_alikafka20190916-2.0.8/alibabacloud_alikafka20190916.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2022-09-05 12:46:27.000000 alibabacloud_alikafka20190916-2.0.8/alibabacloud_alikafka20190916.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-05 12:46:27.000000 alibabacloud_alikafka20190916-2.0.8/alibabacloud_alikafka20190916.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-09-05 12:46:27.000000 alibabacloud_alikafka20190916-2.0.8/alibabacloud_alikafka20190916.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-09-05 12:46:27.000000 alibabacloud_alikafka20190916-2.0.8/alibabacloud_alikafka20190916.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-09-05 12:46:27.000000 alibabacloud_alikafka20190916-2.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2639 2022-09-05 12:46:27.000000 alibabacloud_alikafka20190916-2.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 03:15:44.000000 alibabacloud_alikafka20190916-2.0.9/
+-rw-r--r--   0 root         (0) root         (0)      836 2022-11-18 03:15:43.000000 alibabacloud_alikafka20190916-2.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-11-18 03:15:43.000000 alibabacloud_alikafka20190916-2.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-11-18 03:15:43.000000 alibabacloud_alikafka20190916-2.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2362 2022-11-18 03:15:44.000000 alibabacloud_alikafka20190916-2.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2022-11-18 03:15:43.000000 alibabacloud_alikafka20190916-2.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2022-11-18 03:15:43.000000 alibabacloud_alikafka20190916-2.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 03:15:44.000000 alibabacloud_alikafka20190916-2.0.9/alibabacloud_alikafka20190916/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-11-18 03:15:43.000000 alibabacloud_alikafka20190916-2.0.9/alibabacloud_alikafka20190916/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   131154 2022-11-18 03:15:43.000000 alibabacloud_alikafka20190916-2.0.9/alibabacloud_alikafka20190916/client.py
+-rw-r--r--   0 root         (0) root         (0)   224701 2022-11-18 03:15:43.000000 alibabacloud_alikafka20190916-2.0.9/alibabacloud_alikafka20190916/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-18 03:15:44.000000 alibabacloud_alikafka20190916-2.0.9/alibabacloud_alikafka20190916.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2362 2022-11-18 03:15:43.000000 alibabacloud_alikafka20190916-2.0.9/alibabacloud_alikafka20190916.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2022-11-18 03:15:43.000000 alibabacloud_alikafka20190916-2.0.9/alibabacloud_alikafka20190916.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-18 03:15:43.000000 alibabacloud_alikafka20190916-2.0.9/alibabacloud_alikafka20190916.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-11-18 03:15:43.000000 alibabacloud_alikafka20190916-2.0.9/alibabacloud_alikafka20190916.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2022-11-18 03:15:43.000000 alibabacloud_alikafka20190916-2.0.9/alibabacloud_alikafka20190916.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-11-18 03:15:44.000000 alibabacloud_alikafka20190916-2.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2639 2022-11-18 03:15:43.000000 alibabacloud_alikafka20190916-2.0.9/setup.py
```

### Comparing `alibabacloud_alikafka20190916-2.0.8/LICENSE` & `alibabacloud_alikafka20190916-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916-2.0.8/PKG-INFO` & `alibabacloud_alikafka20190916-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_alikafka20190916
-Version: 2.0.8
+Version: 2.0.9
 Summary: Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alikafka20190916-2.0.8/README-CN.md` & `alibabacloud_alikafka20190916-2.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916-2.0.8/README.md` & `alibabacloud_alikafka20190916-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alikafka20190916-2.0.8/alibabacloud_alikafka20190916/client.py` & `alibabacloud_alikafka20190916-2.0.9/alibabacloud_alikafka20190916/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,14 +339,16 @@
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
@@ -373,14 +375,16 @@
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
@@ -433,14 +437,16 @@
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
@@ -481,14 +487,16 @@
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
@@ -543,14 +551,16 @@
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
@@ -591,14 +601,16 @@
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
@@ -741,14 +753,16 @@
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
@@ -791,14 +805,16 @@
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
@@ -1322,88 +1338,14 @@
     async def describe_acls_async(
         self,
         request: alikafka_20190916_models.DescribeAclsRequest,
     ) -> alikafka_20190916_models.DescribeAclsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_acls_with_options_async(request, runtime)
 
-    def describe_node_status_with_options(
-        self,
-        request: alikafka_20190916_models.DescribeNodeStatusRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> alikafka_20190916_models.DescribeNodeStatusResponse:
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
-    async def describe_node_status_with_options_async(
-        self,
-        request: alikafka_20190916_models.DescribeNodeStatusRequest,
-        runtime: util_models.RuntimeOptions,
-    ) -> alikafka_20190916_models.DescribeNodeStatusResponse:
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
-            await self.call_api_async(params, req, runtime)
-        )
-
-    def describe_node_status(
-        self,
-        request: alikafka_20190916_models.DescribeNodeStatusRequest,
-    ) -> alikafka_20190916_models.DescribeNodeStatusResponse:
-        runtime = util_models.RuntimeOptions()
-        return self.describe_node_status_with_options(request, runtime)
-
-    async def describe_node_status_async(
-        self,
-        request: alikafka_20190916_models.DescribeNodeStatusRequest,
-    ) -> alikafka_20190916_models.DescribeNodeStatusResponse:
-        runtime = util_models.RuntimeOptions()
-        return await self.describe_node_status_with_options_async(request, runtime)
-
     def describe_sasl_users_with_options(
         self,
         request: alikafka_20190916_models.DescribeSaslUsersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.DescribeSaslUsersResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -1856,14 +1798,88 @@
     async def get_instance_list_async(
         self,
         request: alikafka_20190916_models.GetInstanceListRequest,
     ) -> alikafka_20190916_models.GetInstanceListResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_instance_list_with_options_async(request, runtime)
 
+    def get_quota_tip_with_options(
+        self,
+        request: alikafka_20190916_models.GetQuotaTipRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> alikafka_20190916_models.GetQuotaTipResponse:
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
+    async def get_quota_tip_with_options_async(
+        self,
+        request: alikafka_20190916_models.GetQuotaTipRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> alikafka_20190916_models.GetQuotaTipResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_quota_tip(
+        self,
+        request: alikafka_20190916_models.GetQuotaTipRequest,
+    ) -> alikafka_20190916_models.GetQuotaTipResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_quota_tip_with_options(request, runtime)
+
+    async def get_quota_tip_async(
+        self,
+        request: alikafka_20190916_models.GetQuotaTipRequest,
+    ) -> alikafka_20190916_models.GetQuotaTipResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_quota_tip_with_options_async(request, runtime)
+
     def get_topic_list_with_options(
         self,
         request: alikafka_20190916_models.GetTopicListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alikafka_20190916_models.GetTopicListResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -2751,14 +2767,16 @@
     ) -> alikafka_20190916_models.UpdateAllowedIpResponse:
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
@@ -2789,14 +2807,16 @@
     ) -> alikafka_20190916_models.UpdateAllowedIpResponse:
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

### Comparing `alibabacloud_alikafka20190916-2.0.8/alibabacloud_alikafka20190916/models.py` & `alibabacloud_alikafka20190916-2.0.9/alibabacloud_alikafka20190916/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
-from typing import Dict, Any, List
+from typing import Dict, List, Any
 
 
 class ChangeResourceGroupRequest(TeaModel):
     def __init__(
         self,
         new_resource_group_id: str = None,
         region_id: str = None,
@@ -420,29 +420,67 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateAclResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateConsumerGroupRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class CreateConsumerGroupRequest(TeaModel):
     def __init__(
         self,
         consumer_id: str = None,
         instance_id: str = None,
         region_id: str = None,
         remark: str = None,
+        tag: List[CreateConsumerGroupRequestTag] = None,
     ):
         self.consumer_id = consumer_id
         self.instance_id = instance_id
         self.region_id = region_id
         self.remark = remark
+        self.tag = tag
 
     def validate(self):
-        pass
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -450,26 +488,35 @@
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
 
     def from_map(self, m: dict = None):
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
     def __init__(
         self,
         code: int = None,
@@ -554,43 +601,81 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateConsumerGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreatePostPayOrderRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class CreatePostPayOrderRequest(TeaModel):
     def __init__(
         self,
         deploy_type: int = None,
         disk_size: int = None,
         disk_type: str = None,
         eip_max: int = None,
         io_max: int = None,
         io_max_spec: str = None,
         partition_num: int = None,
         region_id: str = None,
         resource_group_id: str = None,
         spec_type: str = None,
+        tag: List[CreatePostPayOrderRequestTag] = None,
         topic_quota: int = None,
     ):
         self.deploy_type = deploy_type
         self.disk_size = disk_size
         self.disk_type = disk_type
         self.eip_max = eip_max
         self.io_max = io_max
         self.io_max_spec = io_max_spec
         self.partition_num = partition_num
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         self.spec_type = spec_type
+        self.tag = tag
         self.topic_quota = topic_quota
 
     def validate(self):
-        pass
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -610,14 +695,18 @@
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('DeployType') is not None:
@@ -636,14 +725,19 @@
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
     def __init__(
@@ -736,43 +830,81 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreatePostPayOrderResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreatePrePayOrderRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class CreatePrePayOrderRequest(TeaModel):
     def __init__(
         self,
         deploy_type: int = None,
         disk_size: int = None,
         disk_type: str = None,
         eip_max: int = None,
         io_max: int = None,
         io_max_spec: str = None,
         partition_num: int = None,
         region_id: str = None,
         resource_group_id: str = None,
         spec_type: str = None,
+        tag: List[CreatePrePayOrderRequestTag] = None,
         topic_quota: int = None,
     ):
         self.deploy_type = deploy_type
         self.disk_size = disk_size
         self.disk_type = disk_type
         self.eip_max = eip_max
         self.io_max = io_max
         self.io_max_spec = io_max_spec
         self.partition_num = partition_num
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         self.spec_type = spec_type
+        self.tag = tag
         self.topic_quota = topic_quota
 
     def validate(self):
-        pass
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -792,14 +924,18 @@
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('DeployType') is not None:
@@ -818,14 +954,19 @@
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
     def __init__(
@@ -1058,41 +1199,79 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateSaslUserResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateTopicRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class CreateTopicRequest(TeaModel):
     def __init__(
         self,
         compact_topic: bool = None,
         config: Dict[str, Any] = None,
         instance_id: str = None,
         local_topic: bool = None,
         min_insync_replicas: int = None,
         partition_num: str = None,
         region_id: str = None,
         remark: str = None,
         replication_factor: int = None,
+        tag: List[CreateTopicRequestTag] = None,
         topic: str = None,
     ):
         self.compact_topic = compact_topic
         self.config = config
         self.instance_id = instance_id
         self.local_topic = local_topic
         self.min_insync_replicas = min_insync_replicas
         self.partition_num = partition_num
         self.region_id = region_id
         self.remark = remark
         self.replication_factor = replication_factor
+        self.tag = tag
         self.topic = topic
 
     def validate(self):
-        pass
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -1110,14 +1289,18 @@
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CompactTopic') is not None:
@@ -1134,46 +1317,89 @@
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
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
 class CreateTopicShrinkRequest(TeaModel):
     def __init__(
         self,
         compact_topic: bool = None,
         config_shrink: str = None,
         instance_id: str = None,
         local_topic: bool = None,
         min_insync_replicas: int = None,
         partition_num: str = None,
         region_id: str = None,
         remark: str = None,
         replication_factor: int = None,
+        tag: List[CreateTopicShrinkRequestTag] = None,
         topic: str = None,
     ):
         self.compact_topic = compact_topic
         self.config_shrink = config_shrink
         self.instance_id = instance_id
         self.local_topic = local_topic
         self.min_insync_replicas = min_insync_replicas
         self.partition_num = partition_num
         self.region_id = region_id
         self.remark = remark
         self.replication_factor = replication_factor
+        self.tag = tag
         self.topic = topic
 
     def validate(self):
-        pass
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -1191,14 +1417,18 @@
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CompactTopic') is not None:
@@ -1215,14 +1445,19 @@
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
     def __init__(
@@ -2219,171 +2454,14 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeAclsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class DescribeNodeStatusRequest(TeaModel):
-    def __init__(
-        self,
-        instance_id: str = None,
-        region_id: str = None,
-    ):
-        self.instance_id = instance_id
-        self.region_id = region_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('InstanceId') is not None:
-            self.instance_id = m.get('InstanceId')
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
-        return self
-
-
-class DescribeNodeStatusResponseBodyStatusList(TeaModel):
-    def __init__(
-        self,
-        status: List[str] = None,
-    ):
-        self.status = status
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.status is not None:
-            result['Status'] = self.status
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('Status') is not None:
-            self.status = m.get('Status')
-        return self
-
-
-class DescribeNodeStatusResponseBody(TeaModel):
-    def __init__(
-        self,
-        code: int = None,
-        message: str = None,
-        request_id: str = None,
-        status_list: DescribeNodeStatusResponseBodyStatusList = None,
-        success: bool = None,
-    ):
-        self.code = code
-        self.message = message
-        self.request_id = request_id
-        self.status_list = status_list
-        self.success = success
-
-    def validate(self):
-        if self.status_list:
-            self.status_list.validate()
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: DescribeNodeStatusResponseBody = None,
-    ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
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
-    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
     ):
         self.instance_id = instance_id
@@ -2738,70 +2816,82 @@
             self.region_id = m.get('RegionId')
         return self
 
 
 class GetAllowedIpListResponseBodyAllowedListInternetList(TeaModel):
     def __init__(
         self,
+        allowed_ip_group: Dict[str, str] = None,
         allowed_ip_list: List[str] = None,
         port_range: str = None,
     ):
+        self.allowed_ip_group = allowed_ip_group
         self.allowed_ip_list = allowed_ip_list
         self.port_range = port_range
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('AllowedIpGroup') is not None:
+            self.allowed_ip_group = m.get('AllowedIpGroup')
         if m.get('AllowedIpList') is not None:
             self.allowed_ip_list = m.get('AllowedIpList')
         if m.get('PortRange') is not None:
             self.port_range = m.get('PortRange')
         return self
 
 
 class GetAllowedIpListResponseBodyAllowedListVpcList(TeaModel):
     def __init__(
         self,
+        allowed_ip_group: Dict[str, str] = None,
         allowed_ip_list: List[str] = None,
         port_range: str = None,
     ):
+        self.allowed_ip_group = allowed_ip_group
         self.allowed_ip_list = allowed_ip_list
         self.port_range = port_range
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('AllowedIpGroup') is not None:
+            self.allowed_ip_group = m.get('AllowedIpGroup')
         if m.get('AllowedIpList') is not None:
             self.allowed_ip_list = m.get('AllowedIpList')
         if m.get('PortRange') is not None:
             self.port_range = m.get('PortRange')
         return self
 
 
@@ -3798,14 +3888,15 @@
         resource_group_id: str = None,
         sasl_domain_endpoint: str = None,
         security_group: str = None,
         service_status: int = None,
         spec_type: str = None,
         ssl_domain_endpoint: str = None,
         ssl_end_point: str = None,
+        standard_zone_id: str = None,
         tags: GetInstanceListResponseBodyInstanceListInstanceVOTags = None,
         topic_num_limit: int = None,
         upgrade_service_detail_info: GetInstanceListResponseBodyInstanceListInstanceVOUpgradeServiceDetailInfo = None,
         used_group_count: int = None,
         used_partition_count: int = None,
         used_topic_count: int = None,
         v_switch_id: str = None,
@@ -3831,14 +3922,15 @@
         self.resource_group_id = resource_group_id
         self.sasl_domain_endpoint = sasl_domain_endpoint
         self.security_group = security_group
         self.service_status = service_status
         self.spec_type = spec_type
         self.ssl_domain_endpoint = ssl_domain_endpoint
         self.ssl_end_point = ssl_end_point
+        self.standard_zone_id = standard_zone_id
         self.tags = tags
         self.topic_num_limit = topic_num_limit
         self.upgrade_service_detail_info = upgrade_service_detail_info
         self.used_group_count = used_group_count
         self.used_partition_count = used_partition_count
         self.used_topic_count = used_topic_count
         self.v_switch_id = v_switch_id
@@ -3899,14 +3991,16 @@
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
@@ -3967,14 +4061,16 @@
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
@@ -4122,14 +4218,231 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetInstanceListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetQuotaTipRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        region_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class GetQuotaTipResponseBodyQuotaData(TeaModel):
+    def __init__(
+        self,
+        group_left: int = None,
+        group_used: int = None,
+        is_partition_buy: int = None,
+        partition_left: int = None,
+        partition_num_of_buy: int = None,
+        partition_quata: int = None,
+        partition_used: int = None,
+        topic_left: int = None,
+        topic_num_of_buy: int = None,
+        topic_quota: int = None,
+        topic_used: int = None,
+    ):
+        self.group_left = group_left
+        self.group_used = group_used
+        self.is_partition_buy = is_partition_buy
+        self.partition_left = partition_left
+        self.partition_num_of_buy = partition_num_of_buy
+        self.partition_quata = partition_quata
+        self.partition_used = partition_used
+        self.topic_left = topic_left
+        self.topic_num_of_buy = topic_num_of_buy
+        self.topic_quota = topic_quota
+        self.topic_used = topic_used
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        code: int = None,
+        message: str = None,
+        quota_data: GetQuotaTipResponseBodyQuotaData = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        self.code = code
+        self.message = message
+        self.quota_data = quota_data
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.quota_data:
+            self.quota_data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetQuotaTipResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         current_page: str = None,
         instance_id: str = None,
         page_size: str = None,
         region_id: str = None,
@@ -6038,21 +6351,23 @@
 
 
 class UpdateAllowedIpRequest(TeaModel):
     def __init__(
         self,
         allowed_list_ip: str = None,
         allowed_list_type: str = None,
+        description: str = None,
         instance_id: str = None,
         port_range: str = None,
         region_id: str = None,
         update_type: str = None,
     ):
         self.allowed_list_ip = allowed_list_ip
         self.allowed_list_type = allowed_list_type
+        self.description = description
         self.instance_id = instance_id
         self.port_range = port_range
         self.region_id = region_id
         self.update_type = update_type
 
     def validate(self):
         pass
@@ -6063,14 +6378,16 @@
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
@@ -6079,14 +6396,16 @@
 
     def from_map(self, m: dict = None):
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

### Comparing `alibabacloud_alikafka20190916-2.0.8/alibabacloud_alikafka20190916.egg-info/PKG-INFO` & `alibabacloud_alikafka20190916-2.0.9/alibabacloud_alikafka20190916.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-alikafka20190916
-Version: 2.0.8
+Version: 2.0.9
 Summary: Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alikafka20190916-2.0.8/setup.py` & `alibabacloud_alikafka20190916-2.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_alikafka20190916.
 
-Created on 05/09/2022
+Created on 18/11/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_alikafka20190916"
 NAME = "alibabacloud_alikafka20190916" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud MQ for Kafka (20190916) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.0, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

