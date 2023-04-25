# Comparing `tmp/alibabacloud_cdn20180510-1.2.6.tar.gz` & `tmp/alibabacloud_cdn20180510-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cdn20180510-1.2.6.tar", last modified: Wed Mar 29 08:13:15 2023, max compression
+gzip compressed data, was "dist/alibabacloud_cdn20180510-1.2.7.tar", last modified: Tue Apr 25 07:17:23 2023, max compression
```

## Comparing `alibabacloud_cdn20180510-1.2.6.tar` & `alibabacloud_cdn20180510-1.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 08:13:15.000000 alibabacloud_cdn20180510-1.2.6/
--rw-r--r--   0 root         (0) root         (0)     1730 2023-03-29 08:13:14.000000 alibabacloud_cdn20180510-1.2.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-29 08:13:14.000000 alibabacloud_cdn20180510-1.2.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-29 08:13:14.000000 alibabacloud_cdn20180510-1.2.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2342 2023-03-29 08:13:15.000000 alibabacloud_cdn20180510-1.2.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-03-29 08:13:14.000000 alibabacloud_cdn20180510-1.2.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-03-29 08:13:14.000000 alibabacloud_cdn20180510-1.2.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 08:13:15.000000 alibabacloud_cdn20180510-1.2.6/alibabacloud_cdn20180510/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-29 08:13:14.000000 alibabacloud_cdn20180510-1.2.6/alibabacloud_cdn20180510/__init__.py
--rw-r--r--   0 root         (0) root         (0)   802993 2023-03-29 08:13:14.000000 alibabacloud_cdn20180510-1.2.6/alibabacloud_cdn20180510/client.py
--rw-r--r--   0 root         (0) root         (0)  1058595 2023-03-29 08:13:14.000000 alibabacloud_cdn20180510-1.2.6/alibabacloud_cdn20180510/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 08:13:15.000000 alibabacloud_cdn20180510-1.2.6/alibabacloud_cdn20180510.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2342 2023-03-29 08:13:15.000000 alibabacloud_cdn20180510-1.2.6/alibabacloud_cdn20180510.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-03-29 08:13:15.000000 alibabacloud_cdn20180510-1.2.6/alibabacloud_cdn20180510.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 08:13:15.000000 alibabacloud_cdn20180510-1.2.6/alibabacloud_cdn20180510.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-03-29 08:13:15.000000 alibabacloud_cdn20180510-1.2.6/alibabacloud_cdn20180510.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-03-29 08:13:15.000000 alibabacloud_cdn20180510-1.2.6/alibabacloud_cdn20180510.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-29 08:13:15.000000 alibabacloud_cdn20180510-1.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2624 2023-03-29 08:13:14.000000 alibabacloud_cdn20180510-1.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/
+-rw-r--r--   0 root         (0) root         (0)     1791 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   803713 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510/client.py
+-rw-r--r--   0 root         (0) root         (0)  1064220 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2624 2023-04-25 07:17:23.000000 alibabacloud_cdn20180510-1.2.7/setup.py
```

### Comparing `alibabacloud_cdn20180510-1.2.6/ChangeLog.md` & `alibabacloud_cdn20180510-1.2.7/ChangeLog.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-03-29 Version: 1.2.6
+- Delete DescribeConfigOfVersion.
+
 2023-03-29 Version: 1.2.5
 - Delete SetConfigOfVersion.
 
 2023-02-25 Version: 1.2.4
 - Add SetCdnDomainSSLCertificate.
 
 2023-02-10 Version: 1.2.3
```

### Comparing `alibabacloud_cdn20180510-1.2.6/LICENSE` & `alibabacloud_cdn20180510-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cdn20180510-1.2.6/PKG-INFO` & `alibabacloud_cdn20180510-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cdn20180510
-Version: 1.2.6
+Version: 1.2.7
 Summary: Alibaba Cloud Alibaba Cloud CDN (20180510) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cdn20180510-1.2.6/README-CN.md` & `alibabacloud_cdn20180510-1.2.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cdn20180510-1.2.6/README.md` & `alibabacloud_cdn20180510-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cdn20180510-1.2.6/alibabacloud_cdn20180510/client.py` & `alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -938,18 +938,18 @@
 
     def batch_stop_cdn_domain_with_options(
         self,
         request: cdn_20180510_models.BatchStopCdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.BatchStopCdnDomainResponse:
         """
-        - After an accelerated domain name is disabled, Alibaba Cloud Content Delivery Network (CDN) retains the information about the accelerated domain name and automatically redirects requests to the origin server.
-        *   If you need to temporary disable CDN acceleration for a domain name, we recommend that you call the StopDomain operation.
-        *   The maximum number of domain names configured at a time is 50.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        After an accelerated domain name is disabled, Alibaba Cloud CDN retains its information and reroutes all the requests that are destined for the accelerated domain name to the origin.
+        *   If you need to temporarily disable CDN acceleration for a domain name, we recommend that you call the StopDomain operation.
+        *   You can call this operation up to 30 times per second per account.
+        *   You can specify up to 50 domain names in each request.
         
         @param request: BatchStopCdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchStopCdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -980,18 +980,18 @@
 
     async def batch_stop_cdn_domain_with_options_async(
         self,
         request: cdn_20180510_models.BatchStopCdnDomainRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.BatchStopCdnDomainResponse:
         """
-        - After an accelerated domain name is disabled, Alibaba Cloud Content Delivery Network (CDN) retains the information about the accelerated domain name and automatically redirects requests to the origin server.
-        *   If you need to temporary disable CDN acceleration for a domain name, we recommend that you call the StopDomain operation.
-        *   The maximum number of domain names configured at a time is 50.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        After an accelerated domain name is disabled, Alibaba Cloud CDN retains its information and reroutes all the requests that are destined for the accelerated domain name to the origin.
+        *   If you need to temporarily disable CDN acceleration for a domain name, we recommend that you call the StopDomain operation.
+        *   You can call this operation up to 30 times per second per account.
+        *   You can specify up to 50 domain names in each request.
         
         @param request: BatchStopCdnDomainRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: BatchStopCdnDomainResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1021,34 +1021,34 @@
         )
 
     def batch_stop_cdn_domain(
         self,
         request: cdn_20180510_models.BatchStopCdnDomainRequest,
     ) -> cdn_20180510_models.BatchStopCdnDomainResponse:
         """
-        - After an accelerated domain name is disabled, Alibaba Cloud Content Delivery Network (CDN) retains the information about the accelerated domain name and automatically redirects requests to the origin server.
-        *   If you need to temporary disable CDN acceleration for a domain name, we recommend that you call the StopDomain operation.
-        *   The maximum number of domain names configured at a time is 50.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        After an accelerated domain name is disabled, Alibaba Cloud CDN retains its information and reroutes all the requests that are destined for the accelerated domain name to the origin.
+        *   If you need to temporarily disable CDN acceleration for a domain name, we recommend that you call the StopDomain operation.
+        *   You can call this operation up to 30 times per second per account.
+        *   You can specify up to 50 domain names in each request.
         
         @param request: BatchStopCdnDomainRequest
         @return: BatchStopCdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.batch_stop_cdn_domain_with_options(request, runtime)
 
     async def batch_stop_cdn_domain_async(
         self,
         request: cdn_20180510_models.BatchStopCdnDomainRequest,
     ) -> cdn_20180510_models.BatchStopCdnDomainResponse:
         """
-        - After an accelerated domain name is disabled, Alibaba Cloud Content Delivery Network (CDN) retains the information about the accelerated domain name and automatically redirects requests to the origin server.
-        *   If you need to temporary disable CDN acceleration for a domain name, we recommend that you call the StopDomain operation.
-        *   The maximum number of domain names configured at a time is 50.
-        *   The maximum number of times that each user can call this operation per second is 30.
+        After an accelerated domain name is disabled, Alibaba Cloud CDN retains its information and reroutes all the requests that are destined for the accelerated domain name to the origin.
+        *   If you need to temporarily disable CDN acceleration for a domain name, we recommend that you call the StopDomain operation.
+        *   You can call this operation up to 30 times per second per account.
+        *   You can specify up to 50 domain names in each request.
         
         @param request: BatchStopCdnDomainRequest
         @return: BatchStopCdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.batch_stop_cdn_domain_with_options_async(request, runtime)
 
@@ -1410,16 +1410,16 @@
 
     def create_cdn_sub_task_with_options(
         self,
         request: cdn_20180510_models.CreateCdnSubTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.CreateCdnSubTaskResponse:
         """
-        > - This operation allows you to customize an operations report for a specific domain name. You can view the statistics about the domain name in the report.
-        - You can call this API operation up to three times per second per account.
+        This operation allows you to create a custom operations report for a specific domain name. You can view the statistics about the domain name in the report.
+        *   You can call this operation up to three times per second per account.
         
         @param request: CreateCdnSubTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateCdnSubTaskResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -1448,16 +1448,16 @@
 
     async def create_cdn_sub_task_with_options_async(
         self,
         request: cdn_20180510_models.CreateCdnSubTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.CreateCdnSubTaskResponse:
         """
-        > - This operation allows you to customize an operations report for a specific domain name. You can view the statistics about the domain name in the report.
-        - You can call this API operation up to three times per second per account.
+        This operation allows you to create a custom operations report for a specific domain name. You can view the statistics about the domain name in the report.
+        *   You can call this operation up to three times per second per account.
         
         @param request: CreateCdnSubTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateCdnSubTaskResponse
         """
         UtilClient.validate_model(request)
         body = {}
@@ -1485,30 +1485,30 @@
         )
 
     def create_cdn_sub_task(
         self,
         request: cdn_20180510_models.CreateCdnSubTaskRequest,
     ) -> cdn_20180510_models.CreateCdnSubTaskResponse:
         """
-        > - This operation allows you to customize an operations report for a specific domain name. You can view the statistics about the domain name in the report.
-        - You can call this API operation up to three times per second per account.
+        This operation allows you to create a custom operations report for a specific domain name. You can view the statistics about the domain name in the report.
+        *   You can call this operation up to three times per second per account.
         
         @param request: CreateCdnSubTaskRequest
         @return: CreateCdnSubTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_cdn_sub_task_with_options(request, runtime)
 
     async def create_cdn_sub_task_async(
         self,
         request: cdn_20180510_models.CreateCdnSubTaskRequest,
     ) -> cdn_20180510_models.CreateCdnSubTaskResponse:
         """
-        > - This operation allows you to customize an operations report for a specific domain name. You can view the statistics about the domain name in the report.
-        - You can call this API operation up to three times per second per account.
+        This operation allows you to create a custom operations report for a specific domain name. You can view the statistics about the domain name in the report.
+        *   You can call this operation up to three times per second per account.
         
         @param request: CreateCdnSubTaskRequest
         @return: CreateCdnSubTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_cdn_sub_task_with_options_async(request, runtime)
 
@@ -1714,16 +1714,16 @@
 
     def create_usage_detail_data_export_task_with_options(
         self,
         request: cdn_20180510_models.CreateUsageDetailDataExportTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.CreateUsageDetailDataExportTaskResponse:
         """
-        - You can create a task that queries data of up to the last year. The maximum time range that can be queried is one month.
-        - The maximum number of times that each Alibaba Cloud account can call this operation per second is 100.
+        You can create a task to query data in the last year. The maximum time range that can be queried is one month.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: CreateUsageDetailDataExportTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateUsageDetailDataExportTaskResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1762,16 +1762,16 @@
 
     async def create_usage_detail_data_export_task_with_options_async(
         self,
         request: cdn_20180510_models.CreateUsageDetailDataExportTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.CreateUsageDetailDataExportTaskResponse:
         """
-        - You can create a task that queries data of up to the last year. The maximum time range that can be queried is one month.
-        - The maximum number of times that each Alibaba Cloud account can call this operation per second is 100.
+        You can create a task to query data in the last year. The maximum time range that can be queried is one month.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: CreateUsageDetailDataExportTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateUsageDetailDataExportTaskResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1809,45 +1809,45 @@
         )
 
     def create_usage_detail_data_export_task(
         self,
         request: cdn_20180510_models.CreateUsageDetailDataExportTaskRequest,
     ) -> cdn_20180510_models.CreateUsageDetailDataExportTaskResponse:
         """
-        - You can create a task that queries data of up to the last year. The maximum time range that can be queried is one month.
-        - The maximum number of times that each Alibaba Cloud account can call this operation per second is 100.
+        You can create a task to query data in the last year. The maximum time range that can be queried is one month.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: CreateUsageDetailDataExportTaskRequest
         @return: CreateUsageDetailDataExportTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_usage_detail_data_export_task_with_options(request, runtime)
 
     async def create_usage_detail_data_export_task_async(
         self,
         request: cdn_20180510_models.CreateUsageDetailDataExportTaskRequest,
     ) -> cdn_20180510_models.CreateUsageDetailDataExportTaskResponse:
         """
-        - You can create a task that queries data of up to the last year. The maximum time range that can be queried is one month.
-        - The maximum number of times that each Alibaba Cloud account can call this operation per second is 100.
+        You can create a task to query data in the last year. The maximum time range that can be queried is one month.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: CreateUsageDetailDataExportTaskRequest
         @return: CreateUsageDetailDataExportTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_usage_detail_data_export_task_with_options_async(request, runtime)
 
     def create_user_usage_data_export_task_with_options(
         self,
         request: cdn_20180510_models.CreateUserUsageDataExportTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.CreateUserUsageDataExportTaskResponse:
         """
-        >    You can create a task that queries data of up to the last one year. The maximum time range that can be queried is one month.
-        > *   The maximum number of times that each user can call this operation per second is 100.
+        You can create a task to query data in the last year. The maximum time range that can be queried is one month.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: CreateUserUsageDataExportTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateUserUsageDataExportTaskResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1880,16 +1880,16 @@
 
     async def create_user_usage_data_export_task_with_options_async(
         self,
         request: cdn_20180510_models.CreateUserUsageDataExportTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.CreateUserUsageDataExportTaskResponse:
         """
-        >    You can create a task that queries data of up to the last one year. The maximum time range that can be queried is one month.
-        > *   The maximum number of times that each user can call this operation per second is 100.
+        You can create a task to query data in the last year. The maximum time range that can be queried is one month.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: CreateUserUsageDataExportTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateUserUsageDataExportTaskResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1921,30 +1921,30 @@
         )
 
     def create_user_usage_data_export_task(
         self,
         request: cdn_20180510_models.CreateUserUsageDataExportTaskRequest,
     ) -> cdn_20180510_models.CreateUserUsageDataExportTaskResponse:
         """
-        >    You can create a task that queries data of up to the last one year. The maximum time range that can be queried is one month.
-        > *   The maximum number of times that each user can call this operation per second is 100.
+        You can create a task to query data in the last year. The maximum time range that can be queried is one month.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: CreateUserUsageDataExportTaskRequest
         @return: CreateUserUsageDataExportTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_user_usage_data_export_task_with_options(request, runtime)
 
     async def create_user_usage_data_export_task_async(
         self,
         request: cdn_20180510_models.CreateUserUsageDataExportTaskRequest,
     ) -> cdn_20180510_models.CreateUserUsageDataExportTaskResponse:
         """
-        >    You can create a task that queries data of up to the last one year. The maximum time range that can be queried is one month.
-        > *   The maximum number of times that each user can call this operation per second is 100.
+        You can create a task to query data in the last year. The maximum time range that can be queried is one month.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: CreateUserUsageDataExportTaskRequest
         @return: CreateUserUsageDataExportTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_user_usage_data_export_task_with_options_async(request, runtime)
 
@@ -3294,15 +3294,15 @@
 
     def describe_cdn_deliver_list_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnDeliverListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnDeliverListResponse:
         """
-        >  You can call this operation up to three times per second.
+        > You can call this operation up to 3 times per second per account.
         
         @param request: DescribeCdnDeliverListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnDeliverListResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3329,15 +3329,15 @@
 
     async def describe_cdn_deliver_list_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnDeliverListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnDeliverListResponse:
         """
-        >  You can call this operation up to three times per second.
+        > You can call this operation up to 3 times per second per account.
         
         @param request: DescribeCdnDeliverListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnDeliverListResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3363,42 +3363,42 @@
         )
 
     def describe_cdn_deliver_list(
         self,
         request: cdn_20180510_models.DescribeCdnDeliverListRequest,
     ) -> cdn_20180510_models.DescribeCdnDeliverListResponse:
         """
-        >  You can call this operation up to three times per second.
+        > You can call this operation up to 3 times per second per account.
         
         @param request: DescribeCdnDeliverListRequest
         @return: DescribeCdnDeliverListResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_deliver_list_with_options(request, runtime)
 
     async def describe_cdn_deliver_list_async(
         self,
         request: cdn_20180510_models.DescribeCdnDeliverListRequest,
     ) -> cdn_20180510_models.DescribeCdnDeliverListResponse:
         """
-        >  You can call this operation up to three times per second.
+        > You can call this operation up to 3 times per second per account.
         
         @param request: DescribeCdnDeliverListRequest
         @return: DescribeCdnDeliverListResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_deliver_list_with_options_async(request, runtime)
 
     def describe_cdn_domain_by_certificate_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnDomainByCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnDomainByCertificateResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeCdnDomainByCertificateRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnDomainByCertificateResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3427,15 +3427,15 @@
 
     async def describe_cdn_domain_by_certificate_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnDomainByCertificateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnDomainByCertificateResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeCdnDomainByCertificateRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnDomainByCertificateResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3463,28 +3463,28 @@
         )
 
     def describe_cdn_domain_by_certificate(
         self,
         request: cdn_20180510_models.DescribeCdnDomainByCertificateRequest,
     ) -> cdn_20180510_models.DescribeCdnDomainByCertificateResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeCdnDomainByCertificateRequest
         @return: DescribeCdnDomainByCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_domain_by_certificate_with_options(request, runtime)
 
     async def describe_cdn_domain_by_certificate_async(
         self,
         request: cdn_20180510_models.DescribeCdnDomainByCertificateRequest,
     ) -> cdn_20180510_models.DescribeCdnDomainByCertificateResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeCdnDomainByCertificateRequest
         @return: DescribeCdnDomainByCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_domain_by_certificate_with_options_async(request, runtime)
 
@@ -3706,17 +3706,18 @@
 
     def describe_cdn_domain_logs_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnDomainLogsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnDomainLogsResponse:
         """
-        >    If you do not set **StartTime** or **EndTime**, data collected within the last 24 hours is queried. If you set both **StartTime** and **EndTime**, data collected within the specified time range is queried.
-        *   The log data was collected at an interval of 1 hour.
-        *   The maximum number of times that each user can call this operation per second is 100.
+        If you do not set **StartTime** or **EndTime**, the request returns the data collected in the last 24 hours. If you set both **StartTime** and **EndTime**, the request returns the data collected within the specified time range.
+        *   The log data is collected every hour.
+        *   You can call this operation up to 100 times per second per account.
+        *   You can query only logs in the last month. The start time and the current time cannot exceed 31 days.
         
         @param request: DescribeCdnDomainLogsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnDomainLogsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3751,17 +3752,18 @@
 
     async def describe_cdn_domain_logs_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnDomainLogsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnDomainLogsResponse:
         """
-        >    If you do not set **StartTime** or **EndTime**, data collected within the last 24 hours is queried. If you set both **StartTime** and **EndTime**, data collected within the specified time range is queried.
-        *   The log data was collected at an interval of 1 hour.
-        *   The maximum number of times that each user can call this operation per second is 100.
+        If you do not set **StartTime** or **EndTime**, the request returns the data collected in the last 24 hours. If you set both **StartTime** and **EndTime**, the request returns the data collected within the specified time range.
+        *   The log data is collected every hour.
+        *   You can call this operation up to 100 times per second per account.
+        *   You can query only logs in the last month. The start time and the current time cannot exceed 31 days.
         
         @param request: DescribeCdnDomainLogsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnDomainLogsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3795,32 +3797,34 @@
         )
 
     def describe_cdn_domain_logs(
         self,
         request: cdn_20180510_models.DescribeCdnDomainLogsRequest,
     ) -> cdn_20180510_models.DescribeCdnDomainLogsResponse:
         """
-        >    If you do not set **StartTime** or **EndTime**, data collected within the last 24 hours is queried. If you set both **StartTime** and **EndTime**, data collected within the specified time range is queried.
-        *   The log data was collected at an interval of 1 hour.
-        *   The maximum number of times that each user can call this operation per second is 100.
+        If you do not set **StartTime** or **EndTime**, the request returns the data collected in the last 24 hours. If you set both **StartTime** and **EndTime**, the request returns the data collected within the specified time range.
+        *   The log data is collected every hour.
+        *   You can call this operation up to 100 times per second per account.
+        *   You can query only logs in the last month. The start time and the current time cannot exceed 31 days.
         
         @param request: DescribeCdnDomainLogsRequest
         @return: DescribeCdnDomainLogsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_domain_logs_with_options(request, runtime)
 
     async def describe_cdn_domain_logs_async(
         self,
         request: cdn_20180510_models.DescribeCdnDomainLogsRequest,
     ) -> cdn_20180510_models.DescribeCdnDomainLogsResponse:
         """
-        >    If you do not set **StartTime** or **EndTime**, data collected within the last 24 hours is queried. If you set both **StartTime** and **EndTime**, data collected within the specified time range is queried.
-        *   The log data was collected at an interval of 1 hour.
-        *   The maximum number of times that each user can call this operation per second is 100.
+        If you do not set **StartTime** or **EndTime**, the request returns the data collected in the last 24 hours. If you set both **StartTime** and **EndTime**, the request returns the data collected within the specified time range.
+        *   The log data is collected every hour.
+        *   You can call this operation up to 100 times per second per account.
+        *   You can query only logs in the last month. The start time and the current time cannot exceed 31 days.
         
         @param request: DescribeCdnDomainLogsRequest
         @return: DescribeCdnDomainLogsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_domain_logs_with_options_async(request, runtime)
 
@@ -3926,15 +3930,15 @@
 
     def describe_cdn_https_domain_list_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnHttpsDomainListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnHttpsDomainListResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeCdnHttpsDomainListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnHttpsDomainListResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3965,15 +3969,15 @@
 
     async def describe_cdn_https_domain_list_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnHttpsDomainListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnHttpsDomainListResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeCdnHttpsDomainListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnHttpsDomainListResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4003,28 +4007,28 @@
         )
 
     def describe_cdn_https_domain_list(
         self,
         request: cdn_20180510_models.DescribeCdnHttpsDomainListRequest,
     ) -> cdn_20180510_models.DescribeCdnHttpsDomainListResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeCdnHttpsDomainListRequest
         @return: DescribeCdnHttpsDomainListResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_https_domain_list_with_options(request, runtime)
 
     async def describe_cdn_https_domain_list_async(
         self,
         request: cdn_20180510_models.DescribeCdnHttpsDomainListRequest,
     ) -> cdn_20180510_models.DescribeCdnHttpsDomainListResponse:
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
         @param request: DescribeCdnHttpsDomainListRequest
         @return: DescribeCdnHttpsDomainListResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_https_domain_list_with_options_async(request, runtime)
 
@@ -4212,15 +4216,15 @@
 
     def describe_cdn_report_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnReportResponse:
         """
-        >  You can call this operation up to three times per second per account.
+        > You can call this operation up to three times per second per account.
         
         @param request: DescribeCdnReportRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnReportResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4259,15 +4263,15 @@
 
     async def describe_cdn_report_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnReportResponse:
         """
-        >  You can call this operation up to three times per second per account.
+        > You can call this operation up to three times per second per account.
         
         @param request: DescribeCdnReportRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnReportResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4305,28 +4309,28 @@
         )
 
     def describe_cdn_report(
         self,
         request: cdn_20180510_models.DescribeCdnReportRequest,
     ) -> cdn_20180510_models.DescribeCdnReportResponse:
         """
-        >  You can call this operation up to three times per second per account.
+        > You can call this operation up to three times per second per account.
         
         @param request: DescribeCdnReportRequest
         @return: DescribeCdnReportResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_report_with_options(request, runtime)
 
     async def describe_cdn_report_async(
         self,
         request: cdn_20180510_models.DescribeCdnReportRequest,
     ) -> cdn_20180510_models.DescribeCdnReportResponse:
         """
-        >  You can call this operation up to three times per second per account.
+        > You can call this operation up to three times per second per account.
         
         @param request: DescribeCdnReportRequest
         @return: DescribeCdnReportResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_report_with_options_async(request, runtime)
 
@@ -4818,16 +4822,16 @@
 
     def describe_cdn_user_bill_history_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnUserBillHistoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnUserBillHistoryResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - You can query billing history up to the last one month.
+        You can query billing history up to the last one month.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeCdnUserBillHistoryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnUserBillHistoryResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4856,16 +4860,16 @@
 
     async def describe_cdn_user_bill_history_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnUserBillHistoryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnUserBillHistoryResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - You can query billing history up to the last one month.
+        You can query billing history up to the last one month.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeCdnUserBillHistoryRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCdnUserBillHistoryResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4893,30 +4897,30 @@
         )
 
     def describe_cdn_user_bill_history(
         self,
         request: cdn_20180510_models.DescribeCdnUserBillHistoryRequest,
     ) -> cdn_20180510_models.DescribeCdnUserBillHistoryResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - You can query billing history up to the last one month.
+        You can query billing history up to the last one month.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeCdnUserBillHistoryRequest
         @return: DescribeCdnUserBillHistoryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_user_bill_history_with_options(request, runtime)
 
     async def describe_cdn_user_bill_history_async(
         self,
         request: cdn_20180510_models.DescribeCdnUserBillHistoryRequest,
     ) -> cdn_20180510_models.DescribeCdnUserBillHistoryResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - You can query billing history up to the last one month.
+        You can query billing history up to the last one month.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeCdnUserBillHistoryRequest
         @return: DescribeCdnUserBillHistoryResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_user_bill_history_with_options_async(request, runtime)
 
@@ -5053,14 +5057,21 @@
         return await self.describe_cdn_user_bill_prediction_with_options_async(request, runtime)
 
     def describe_cdn_user_bill_type_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnUserBillTypeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnUserBillTypeResponse:
+        """
+        You can call this operation up to 100 times per second per account.
+        
+        @param request: DescribeCdnUserBillTypeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeCdnUserBillTypeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.start_time):
             query['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
@@ -5083,14 +5094,21 @@
         )
 
     async def describe_cdn_user_bill_type_with_options_async(
         self,
         request: cdn_20180510_models.DescribeCdnUserBillTypeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCdnUserBillTypeResponse:
+        """
+        You can call this operation up to 100 times per second per account.
+        
+        @param request: DescribeCdnUserBillTypeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeCdnUserBillTypeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.start_time):
             query['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
@@ -5112,21 +5130,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_cdn_user_bill_type(
         self,
         request: cdn_20180510_models.DescribeCdnUserBillTypeRequest,
     ) -> cdn_20180510_models.DescribeCdnUserBillTypeResponse:
+        """
+        You can call this operation up to 100 times per second per account.
+        
+        @param request: DescribeCdnUserBillTypeRequest
+        @return: DescribeCdnUserBillTypeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_user_bill_type_with_options(request, runtime)
 
     async def describe_cdn_user_bill_type_async(
         self,
         request: cdn_20180510_models.DescribeCdnUserBillTypeRequest,
     ) -> cdn_20180510_models.DescribeCdnUserBillTypeResponse:
+        """
+        You can call this operation up to 100 times per second per account.
+        
+        @param request: DescribeCdnUserBillTypeRequest
+        @return: DescribeCdnUserBillTypeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cdn_user_bill_type_with_options_async(request, runtime)
 
     def describe_cdn_user_configs_with_options(
         self,
         request: cdn_20180510_models.DescribeCdnUserConfigsRequest,
         runtime: util_models.RuntimeOptions,
@@ -5614,16 +5644,16 @@
 
     def describe_certificate_info_by_idwith_options(
         self,
         request: cdn_20180510_models.DescribeCertificateInfoByIDRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCertificateInfoByIDResponse:
         """
-        > - The maximum number of times that each user can call this operation per second is 100.
-        - If a certificate is associated with a domain name but not enabled, the result of this operation shows that the certificate does not exist.
+        You can call this operation up to 100 times per second per account.
+        *   If a certificate is associated with a domain name but the certificate is not enabled, the result of this operation shows that the certificate does not exist.
         
         @param request: DescribeCertificateInfoByIDRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCertificateInfoByIDResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -5648,16 +5678,16 @@
 
     async def describe_certificate_info_by_idwith_options_async(
         self,
         request: cdn_20180510_models.DescribeCertificateInfoByIDRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeCertificateInfoByIDResponse:
         """
-        > - The maximum number of times that each user can call this operation per second is 100.
-        - If a certificate is associated with a domain name but not enabled, the result of this operation shows that the certificate does not exist.
+        You can call this operation up to 100 times per second per account.
+        *   If a certificate is associated with a domain name but the certificate is not enabled, the result of this operation shows that the certificate does not exist.
         
         @param request: DescribeCertificateInfoByIDRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeCertificateInfoByIDResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -5681,30 +5711,30 @@
         )
 
     def describe_certificate_info_by_id(
         self,
         request: cdn_20180510_models.DescribeCertificateInfoByIDRequest,
     ) -> cdn_20180510_models.DescribeCertificateInfoByIDResponse:
         """
-        > - The maximum number of times that each user can call this operation per second is 100.
-        - If a certificate is associated with a domain name but not enabled, the result of this operation shows that the certificate does not exist.
+        You can call this operation up to 100 times per second per account.
+        *   If a certificate is associated with a domain name but the certificate is not enabled, the result of this operation shows that the certificate does not exist.
         
         @param request: DescribeCertificateInfoByIDRequest
         @return: DescribeCertificateInfoByIDResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_certificate_info_by_idwith_options(request, runtime)
 
     async def describe_certificate_info_by_id_async(
         self,
         request: cdn_20180510_models.DescribeCertificateInfoByIDRequest,
     ) -> cdn_20180510_models.DescribeCertificateInfoByIDResponse:
         """
-        > - The maximum number of times that each user can call this operation per second is 100.
-        - If a certificate is associated with a domain name but not enabled, the result of this operation shows that the certificate does not exist.
+        You can call this operation up to 100 times per second per account.
+        *   If a certificate is associated with a domain name but the certificate is not enabled, the result of this operation shows that the certificate does not exist.
         
         @param request: DescribeCertificateInfoByIDRequest
         @return: DescribeCertificateInfoByIDResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_certificate_info_by_idwith_options_async(request, runtime)
 
@@ -5938,23 +5968,23 @@
 
     def describe_domain_bps_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainBpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainBpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 150.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 150 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainBpsDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainBpsDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5991,23 +6021,23 @@
 
     async def describe_domain_bps_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainBpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainBpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 150.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 150 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainBpsDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainBpsDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6043,66 +6073,66 @@
         )
 
     def describe_domain_bps_data(
         self,
         request: cdn_20180510_models.DescribeDomainBpsDataRequest,
     ) -> cdn_20180510_models.DescribeDomainBpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 150.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 150 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainBpsDataRequest
         @return: DescribeDomainBpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_bps_data_with_options(request, runtime)
 
     async def describe_domain_bps_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainBpsDataRequest,
     ) -> cdn_20180510_models.DescribeDomainBpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 150.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 150 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainBpsDataRequest
         @return: DescribeDomainBpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_bps_data_with_options_async(request, runtime)
 
     def describe_domain_bps_data_by_layer_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainBpsDataByLayerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainBpsDataByLayerResponse:
         """
-        - The number of times that each user can call this operation per second is 20.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 20 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainBpsDataByLayerRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainBpsDataByLayerResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6141,23 +6171,23 @@
 
     async def describe_domain_bps_data_by_layer_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainBpsDataByLayerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainBpsDataByLayerResponse:
         """
-        - The number of times that each user can call this operation per second is 20.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 20 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainBpsDataByLayerRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainBpsDataByLayerResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6195,61 +6225,61 @@
         )
 
     def describe_domain_bps_data_by_layer(
         self,
         request: cdn_20180510_models.DescribeDomainBpsDataByLayerRequest,
     ) -> cdn_20180510_models.DescribeDomainBpsDataByLayerResponse:
         """
-        - The number of times that each user can call this operation per second is 20.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 20 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainBpsDataByLayerRequest
         @return: DescribeDomainBpsDataByLayerResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_bps_data_by_layer_with_options(request, runtime)
 
     async def describe_domain_bps_data_by_layer_async(
         self,
         request: cdn_20180510_models.DescribeDomainBpsDataByLayerRequest,
     ) -> cdn_20180510_models.DescribeDomainBpsDataByLayerResponse:
         """
-        - The number of times that each user can call this operation per second is 20.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 20 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainBpsDataByLayerRequest
         @return: DescribeDomainBpsDataByLayerResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_bps_data_by_layer_with_options_async(request, runtime)
 
     def describe_domain_bps_data_by_time_stamp_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainBpsDataByTimeStampRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainBpsDataByTimeStampResponse:
         """
         The bandwidth is measured in bit/s.
-        *   You can specify only one domain name in each query.
-        *   The data is collected at an interval of five minutes.
-        *   The maximum number of times that each user can call this operation per second is 20.
+        *   You can specify only one accelerated domain name in each request.
+        *   The data is collected every 5 minutes.
+        *   You can call this operation up to 20 times per second per account.
         
         @param request: DescribeDomainBpsDataByTimeStampRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainBpsDataByTimeStampResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6283,17 +6313,17 @@
     async def describe_domain_bps_data_by_time_stamp_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainBpsDataByTimeStampRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainBpsDataByTimeStampResponse:
         """
         The bandwidth is measured in bit/s.
-        *   You can specify only one domain name in each query.
-        *   The data is collected at an interval of five minutes.
-        *   The maximum number of times that each user can call this operation per second is 20.
+        *   You can specify only one accelerated domain name in each request.
+        *   The data is collected every 5 minutes.
+        *   You can call this operation up to 20 times per second per account.
         
         @param request: DescribeDomainBpsDataByTimeStampRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainBpsDataByTimeStampResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6326,33 +6356,33 @@
 
     def describe_domain_bps_data_by_time_stamp(
         self,
         request: cdn_20180510_models.DescribeDomainBpsDataByTimeStampRequest,
     ) -> cdn_20180510_models.DescribeDomainBpsDataByTimeStampResponse:
         """
         The bandwidth is measured in bit/s.
-        *   You can specify only one domain name in each query.
-        *   The data is collected at an interval of five minutes.
-        *   The maximum number of times that each user can call this operation per second is 20.
+        *   You can specify only one accelerated domain name in each request.
+        *   The data is collected every 5 minutes.
+        *   You can call this operation up to 20 times per second per account.
         
         @param request: DescribeDomainBpsDataByTimeStampRequest
         @return: DescribeDomainBpsDataByTimeStampResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_bps_data_by_time_stamp_with_options(request, runtime)
 
     async def describe_domain_bps_data_by_time_stamp_async(
         self,
         request: cdn_20180510_models.DescribeDomainBpsDataByTimeStampRequest,
     ) -> cdn_20180510_models.DescribeDomainBpsDataByTimeStampResponse:
         """
         The bandwidth is measured in bit/s.
-        *   You can specify only one domain name in each query.
-        *   The data is collected at an interval of five minutes.
-        *   The maximum number of times that each user can call this operation per second is 20.
+        *   You can specify only one accelerated domain name in each request.
+        *   The data is collected every 5 minutes.
+        *   You can call this operation up to 20 times per second per account.
         
         @param request: DescribeDomainBpsDataByTimeStampRequest
         @return: DescribeDomainBpsDataByTimeStampResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_bps_data_by_time_stamp_with_options_async(request, runtime)
 
@@ -6876,23 +6906,23 @@
 
     def describe_domain_hit_rate_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainHitRateDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainHitRateDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainHitRateDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainHitRateDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6925,23 +6955,23 @@
 
     async def describe_domain_hit_rate_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainHitRateDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainHitRateDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainHitRateDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainHitRateDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6973,44 +7003,44 @@
         )
 
     def describe_domain_hit_rate_data(
         self,
         request: cdn_20180510_models.DescribeDomainHitRateDataRequest,
     ) -> cdn_20180510_models.DescribeDomainHitRateDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainHitRateDataRequest
         @return: DescribeDomainHitRateDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_hit_rate_data_with_options(request, runtime)
 
     async def describe_domain_hit_rate_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainHitRateDataRequest,
     ) -> cdn_20180510_models.DescribeDomainHitRateDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainHitRateDataRequest
         @return: DescribeDomainHitRateDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_hit_rate_data_with_options_async(request, runtime)
 
@@ -7164,23 +7194,23 @@
 
     def describe_domain_http_code_data_by_layer_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainHttpCodeDataByLayerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainHttpCodeDataByLayerResponse:
         """
-        - You can call this operation up to 20 times per second.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        You can call this operation up to 20 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        ### Time granularity
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainHttpCodeDataByLayerRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainHttpCodeDataByLayerResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7219,23 +7249,23 @@
 
     async def describe_domain_http_code_data_by_layer_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainHttpCodeDataByLayerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainHttpCodeDataByLayerResponse:
         """
-        - You can call this operation up to 20 times per second.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        You can call this operation up to 20 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        ### Time granularity
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainHttpCodeDataByLayerRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainHttpCodeDataByLayerResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7273,44 +7303,44 @@
         )
 
     def describe_domain_http_code_data_by_layer(
         self,
         request: cdn_20180510_models.DescribeDomainHttpCodeDataByLayerRequest,
     ) -> cdn_20180510_models.DescribeDomainHttpCodeDataByLayerResponse:
         """
-        - You can call this operation up to 20 times per second.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        You can call this operation up to 20 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        ### Time granularity
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainHttpCodeDataByLayerRequest
         @return: DescribeDomainHttpCodeDataByLayerResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_http_code_data_by_layer_with_options(request, runtime)
 
     async def describe_domain_http_code_data_by_layer_async(
         self,
         request: cdn_20180510_models.DescribeDomainHttpCodeDataByLayerRequest,
     ) -> cdn_20180510_models.DescribeDomainHttpCodeDataByLayerResponse:
         """
-        - You can call this operation up to 20 times per second.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        You can call this operation up to 20 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        ### Time granularity
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainHttpCodeDataByLayerRequest
         @return: DescribeDomainHttpCodeDataByLayerResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_http_code_data_by_layer_with_options_async(request, runtime)
 
@@ -7431,14 +7461,25 @@
         return await self.describe_domain_ispdata_with_options_async(request, runtime)
 
     def describe_domain_max_95bps_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainMax95BpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainMax95BpsDataResponse:
+        """
+        The unit of the bandwidth is bit/s.
+        *   The time granularity of the queried data is 5 minutes.
+        *   You can query data in the last 90 days.
+        *   You can specify the StartTime and EndTime parameters, or the TimePoint and Cycle parameters to query the 95th percentile bandwidth data. If you specify the StartTime and EndTime parameters and the time range that is specified by these parameters is less than or equal to 24 hours, the 95th percentile bandwidth data on the day of the start time is returned. If the time range that is specified by these parameters is more than 24 hours, the 95th percentile bandwidth data in the month of the start time is returned. If you specify the TimePoint and Cycle parameters, the 95th percentile bandwidth data of the cycle is returned. If you do not specify parameters as previously mentioned, the 95th percentile bandwidth data in the last 24 hours is returned.
+        *   You can call this operation up to 100 times per second per account.
+        
+        @param request: DescribeDomainMax95BpsDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDomainMax95BpsDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cycle):
             query['Cycle'] = request.cycle
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.end_time):
@@ -7467,14 +7508,25 @@
         )
 
     async def describe_domain_max_95bps_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainMax95BpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainMax95BpsDataResponse:
+        """
+        The unit of the bandwidth is bit/s.
+        *   The time granularity of the queried data is 5 minutes.
+        *   You can query data in the last 90 days.
+        *   You can specify the StartTime and EndTime parameters, or the TimePoint and Cycle parameters to query the 95th percentile bandwidth data. If you specify the StartTime and EndTime parameters and the time range that is specified by these parameters is less than or equal to 24 hours, the 95th percentile bandwidth data on the day of the start time is returned. If the time range that is specified by these parameters is more than 24 hours, the 95th percentile bandwidth data in the month of the start time is returned. If you specify the TimePoint and Cycle parameters, the 95th percentile bandwidth data of the cycle is returned. If you do not specify parameters as previously mentioned, the 95th percentile bandwidth data in the last 24 hours is returned.
+        *   You can call this operation up to 100 times per second per account.
+        
+        @param request: DescribeDomainMax95BpsDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDomainMax95BpsDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cycle):
             query['Cycle'] = request.cycle
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.end_time):
@@ -7502,21 +7554,41 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_domain_max_95bps_data(
         self,
         request: cdn_20180510_models.DescribeDomainMax95BpsDataRequest,
     ) -> cdn_20180510_models.DescribeDomainMax95BpsDataResponse:
+        """
+        The unit of the bandwidth is bit/s.
+        *   The time granularity of the queried data is 5 minutes.
+        *   You can query data in the last 90 days.
+        *   You can specify the StartTime and EndTime parameters, or the TimePoint and Cycle parameters to query the 95th percentile bandwidth data. If you specify the StartTime and EndTime parameters and the time range that is specified by these parameters is less than or equal to 24 hours, the 95th percentile bandwidth data on the day of the start time is returned. If the time range that is specified by these parameters is more than 24 hours, the 95th percentile bandwidth data in the month of the start time is returned. If you specify the TimePoint and Cycle parameters, the 95th percentile bandwidth data of the cycle is returned. If you do not specify parameters as previously mentioned, the 95th percentile bandwidth data in the last 24 hours is returned.
+        *   You can call this operation up to 100 times per second per account.
+        
+        @param request: DescribeDomainMax95BpsDataRequest
+        @return: DescribeDomainMax95BpsDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_max_95bps_data_with_options(request, runtime)
 
     async def describe_domain_max_95bps_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainMax95BpsDataRequest,
     ) -> cdn_20180510_models.DescribeDomainMax95BpsDataResponse:
+        """
+        The unit of the bandwidth is bit/s.
+        *   The time granularity of the queried data is 5 minutes.
+        *   You can query data in the last 90 days.
+        *   You can specify the StartTime and EndTime parameters, or the TimePoint and Cycle parameters to query the 95th percentile bandwidth data. If you specify the StartTime and EndTime parameters and the time range that is specified by these parameters is less than or equal to 24 hours, the 95th percentile bandwidth data on the day of the start time is returned. If the time range that is specified by these parameters is more than 24 hours, the 95th percentile bandwidth data in the month of the start time is returned. If you specify the TimePoint and Cycle parameters, the 95th percentile bandwidth data of the cycle is returned. If you do not specify parameters as previously mentioned, the 95th percentile bandwidth data in the last 24 hours is returned.
+        *   You can call this operation up to 100 times per second per account.
+        
+        @param request: DescribeDomainMax95BpsDataRequest
+        @return: DescribeDomainMax95BpsDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_max_95bps_data_with_options_async(request, runtime)
 
     def describe_domain_multi_usage_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainMultiUsageDataRequest,
         runtime: util_models.RuntimeOptions,
@@ -7639,15 +7711,15 @@
     def describe_domain_path_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainPathDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainPathDataResponse:
         """
         This operation is available only to users that are on the whitelist. If the daily peak bandwidth value of your workloads reaches 10 Gbit/s, you can [submit a ticket](https://workorder-intl.console.aliyun.com/?spm=5176.2020520001.aliyun_topbar.18.dbd44bd3e4f845#/ticket/createIndex) to apply to be included in the whitelist.
-        *   The maximum number of times that each user can call this operation per second is 6,000.
+        *   You can call this API operation up to 6,000 times per second per account.
         *   Data collection by directory is available only to specified domain names within your Alibaba Cloud account. It cannot be enabled for all domain names within your Alibaba Cloud account.
         *   The average size of the files that belong to the domain name must be larger than 1 MB.
         *   The number of directories specified for a single domain name cannot exceed 100. If the number of directories exceeds 100, the data accuracy reduces.
         *   If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
         *   You can query data collected within the last 30 days.
         
         @param request: DescribeDomainPathDataRequest
@@ -7678,15 +7750,15 @@
     async def describe_domain_path_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainPathDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainPathDataResponse:
         """
         This operation is available only to users that are on the whitelist. If the daily peak bandwidth value of your workloads reaches 10 Gbit/s, you can [submit a ticket](https://workorder-intl.console.aliyun.com/?spm=5176.2020520001.aliyun_topbar.18.dbd44bd3e4f845#/ticket/createIndex) to apply to be included in the whitelist.
-        *   The maximum number of times that each user can call this operation per second is 6,000.
+        *   You can call this API operation up to 6,000 times per second per account.
         *   Data collection by directory is available only to specified domain names within your Alibaba Cloud account. It cannot be enabled for all domain names within your Alibaba Cloud account.
         *   The average size of the files that belong to the domain name must be larger than 1 MB.
         *   The number of directories specified for a single domain name cannot exceed 100. If the number of directories exceeds 100, the data accuracy reduces.
         *   If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
         *   You can query data collected within the last 30 days.
         
         @param request: DescribeDomainPathDataRequest
@@ -7716,15 +7788,15 @@
 
     def describe_domain_path_data(
         self,
         request: cdn_20180510_models.DescribeDomainPathDataRequest,
     ) -> cdn_20180510_models.DescribeDomainPathDataResponse:
         """
         This operation is available only to users that are on the whitelist. If the daily peak bandwidth value of your workloads reaches 10 Gbit/s, you can [submit a ticket](https://workorder-intl.console.aliyun.com/?spm=5176.2020520001.aliyun_topbar.18.dbd44bd3e4f845#/ticket/createIndex) to apply to be included in the whitelist.
-        *   The maximum number of times that each user can call this operation per second is 6,000.
+        *   You can call this API operation up to 6,000 times per second per account.
         *   Data collection by directory is available only to specified domain names within your Alibaba Cloud account. It cannot be enabled for all domain names within your Alibaba Cloud account.
         *   The average size of the files that belong to the domain name must be larger than 1 MB.
         *   The number of directories specified for a single domain name cannot exceed 100. If the number of directories exceeds 100, the data accuracy reduces.
         *   If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
         *   You can query data collected within the last 30 days.
         
         @param request: DescribeDomainPathDataRequest
@@ -7735,15 +7807,15 @@
 
     async def describe_domain_path_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainPathDataRequest,
     ) -> cdn_20180510_models.DescribeDomainPathDataResponse:
         """
         This operation is available only to users that are on the whitelist. If the daily peak bandwidth value of your workloads reaches 10 Gbit/s, you can [submit a ticket](https://workorder-intl.console.aliyun.com/?spm=5176.2020520001.aliyun_topbar.18.dbd44bd3e4f845#/ticket/createIndex) to apply to be included in the whitelist.
-        *   The maximum number of times that each user can call this operation per second is 6,000.
+        *   You can call this API operation up to 6,000 times per second per account.
         *   Data collection by directory is available only to specified domain names within your Alibaba Cloud account. It cannot be enabled for all domain names within your Alibaba Cloud account.
         *   The average size of the files that belong to the domain name must be larger than 1 MB.
         *   The number of directories specified for a single domain name cannot exceed 100. If the number of directories exceeds 100, the data accuracy reduces.
         *   If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
         *   You can query data collected within the last 30 days.
         
         @param request: DescribeDomainPathDataRequest
@@ -7866,23 +7938,23 @@
 
     def describe_domain_qps_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainQpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainQpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainQpsDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainQpsDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7919,23 +7991,23 @@
 
     async def describe_domain_qps_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainQpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainQpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainQpsDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainQpsDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7971,66 +8043,66 @@
         )
 
     def describe_domain_qps_data(
         self,
         request: cdn_20180510_models.DescribeDomainQpsDataRequest,
     ) -> cdn_20180510_models.DescribeDomainQpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainQpsDataRequest
         @return: DescribeDomainQpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_qps_data_with_options(request, runtime)
 
     async def describe_domain_qps_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainQpsDataRequest,
     ) -> cdn_20180510_models.DescribeDomainQpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainQpsDataRequest
         @return: DescribeDomainQpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_qps_data_with_options_async(request, runtime)
 
     def describe_domain_qps_data_by_layer_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainQpsDataByLayerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainQpsDataByLayerResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 20.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 20 times per second per user.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainQpsDataByLayerRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainQpsDataByLayerResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8069,23 +8141,23 @@
 
     async def describe_domain_qps_data_by_layer_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainQpsDataByLayerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainQpsDataByLayerResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 20.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 20 times per second per user.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainQpsDataByLayerRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainQpsDataByLayerResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8123,66 +8195,65 @@
         )
 
     def describe_domain_qps_data_by_layer(
         self,
         request: cdn_20180510_models.DescribeDomainQpsDataByLayerRequest,
     ) -> cdn_20180510_models.DescribeDomainQpsDataByLayerResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 20.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 20 times per second per user.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainQpsDataByLayerRequest
         @return: DescribeDomainQpsDataByLayerResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_qps_data_by_layer_with_options(request, runtime)
 
     async def describe_domain_qps_data_by_layer_async(
         self,
         request: cdn_20180510_models.DescribeDomainQpsDataByLayerRequest,
     ) -> cdn_20180510_models.DescribeDomainQpsDataByLayerResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 20.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 20 times per second per user.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainQpsDataByLayerRequest
         @return: DescribeDomainQpsDataByLayerResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_qps_data_by_layer_with_options_async(request, runtime)
 
     def describe_domain_real_time_bps_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeBpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeBpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
+        **Time granularity** The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeBpsDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeBpsDataResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -8207,23 +8278,22 @@
 
     async def describe_domain_real_time_bps_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeBpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeBpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
+        **Time granularity** The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeBpsDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeBpsDataResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -8247,67 +8317,65 @@
         )
 
     def describe_domain_real_time_bps_data(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeBpsDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeBpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
+        **Time granularity** The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeBpsDataRequest
         @return: DescribeDomainRealTimeBpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_real_time_bps_data_with_options(request, runtime)
 
     async def describe_domain_real_time_bps_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeBpsDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeBpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        **Time granularity**\
-        The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
+        **Time granularity** The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeBpsDataRequest
         @return: DescribeDomainRealTimeBpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_real_time_bps_data_with_options_async(request, runtime)
 
     def describe_domain_real_time_byte_hit_rate_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeByteHitRateDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeByteHitRateDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the byte hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
+        You can call this operation up to 10 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
+        * The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the byte hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeByteHitRateDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeByteHitRateDataResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -8332,24 +8400,24 @@
 
     async def describe_domain_real_time_byte_hit_rate_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeByteHitRateDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeByteHitRateDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the byte hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
+        You can call this operation up to 10 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
+        * The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the byte hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeByteHitRateDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeByteHitRateDataResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -8373,46 +8441,46 @@
         )
 
     def describe_domain_real_time_byte_hit_rate_data(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeByteHitRateDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeByteHitRateDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the byte hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
+        You can call this operation up to 10 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
+        * The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the byte hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeByteHitRateDataRequest
         @return: DescribeDomainRealTimeByteHitRateDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_real_time_byte_hit_rate_data_with_options(request, runtime)
 
     async def describe_domain_real_time_byte_hit_rate_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeByteHitRateDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeByteHitRateDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        - The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the byte hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
+        You can call this operation up to 10 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
+        * The network traffic destined for different domain names may be redirected to the same origin server. Therefore, the byte hit ratios may be inaccurate. The accuracy of query results is based on the actual configurations.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeByteHitRateDataRequest
         @return: DescribeDomainRealTimeByteHitRateDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_real_time_byte_hit_rate_data_with_options_async(request, runtime)
 
@@ -8514,23 +8582,23 @@
 
     def describe_domain_real_time_http_code_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeHttpCodeDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeHttpCodeDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 10 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Historical data available | Time range to query | Data delay |
-        | ---------------- | ------------------------- | ------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeHttpCodeDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeHttpCodeDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8565,23 +8633,23 @@
 
     async def describe_domain_real_time_http_code_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeHttpCodeDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeHttpCodeDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 10 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Historical data available | Time range to query | Data delay |
-        | ---------------- | ------------------------- | ------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeHttpCodeDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeHttpCodeDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8615,66 +8683,66 @@
         )
 
     def describe_domain_real_time_http_code_data(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeHttpCodeDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeHttpCodeDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 10 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Historical data available | Time range to query | Data delay |
-        | ---------------- | ------------------------- | ------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeHttpCodeDataRequest
         @return: DescribeDomainRealTimeHttpCodeDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_real_time_http_code_data_with_options(request, runtime)
 
     async def describe_domain_real_time_http_code_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeHttpCodeDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeHttpCodeDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 10 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Historical data available | Time range to query | Data delay |
-        | ---------------- | ------------------------- | ------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeHttpCodeDataRequest
         @return: DescribeDomainRealTimeHttpCodeDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_real_time_http_code_data_with_options_async(request, runtime)
 
     def describe_domain_real_time_qps_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeQpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeQpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 10 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeQpsDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeQpsDataResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -8699,23 +8767,23 @@
 
     async def describe_domain_real_time_qps_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeQpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeQpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 10 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeQpsDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeQpsDataResponse
         """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
@@ -8739,44 +8807,44 @@
         )
 
     def describe_domain_real_time_qps_data(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeQpsDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeQpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 10 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeQpsDataRequest
         @return: DescribeDomainRealTimeQpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_real_time_qps_data_with_options(request, runtime)
 
     async def describe_domain_real_time_qps_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeQpsDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeQpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 10 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeQpsDataRequest
         @return: DescribeDomainRealTimeQpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_real_time_qps_data_with_options_async(request, runtime)
 
@@ -8914,23 +8982,23 @@
 
     def describe_domain_real_time_src_bps_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeSrcBpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeSrcBpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 10 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeSrcBpsDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeSrcBpsDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8961,23 +9029,23 @@
 
     async def describe_domain_real_time_src_bps_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeSrcBpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeSrcBpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 10 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeSrcBpsDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeSrcBpsDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9007,66 +9075,66 @@
         )
 
     def describe_domain_real_time_src_bps_data(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeSrcBpsDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeSrcBpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 10 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeSrcBpsDataRequest
         @return: DescribeDomainRealTimeSrcBpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_real_time_src_bps_data_with_options(request, runtime)
 
     async def describe_domain_real_time_src_bps_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeSrcBpsDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeSrcBpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 10 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeSrcBpsDataRequest
         @return: DescribeDomainRealTimeSrcBpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_real_time_src_bps_data_with_options_async(request, runtime)
 
     def describe_domain_real_time_src_http_code_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeSrcHttpCodeDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeSrcHttpCodeDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 10 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Historical data available | Time range to query | Data delay |
-        | ---------------- | ------------------------- | ------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeSrcHttpCodeDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeSrcHttpCodeDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9101,23 +9169,23 @@
 
     async def describe_domain_real_time_src_http_code_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeSrcHttpCodeDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeSrcHttpCodeDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 10 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Historical data available | Time range to query | Data delay |
-        | ---------------- | ------------------------- | ------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeSrcHttpCodeDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeSrcHttpCodeDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9151,66 +9219,66 @@
         )
 
     def describe_domain_real_time_src_http_code_data(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeSrcHttpCodeDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeSrcHttpCodeDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 10 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Historical data available | Time range to query | Data delay |
-        | ---------------- | ------------------------- | ------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeSrcHttpCodeDataRequest
         @return: DescribeDomainRealTimeSrcHttpCodeDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_real_time_src_http_code_data_with_options(request, runtime)
 
     async def describe_domain_real_time_src_http_code_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeSrcHttpCodeDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeSrcHttpCodeDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 10 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you set both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Historical data available | Time range to query | Data delay |
-        | ---------------- | ------------------------- | ------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeSrcHttpCodeDataRequest
         @return: DescribeDomainRealTimeSrcHttpCodeDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_real_time_src_http_code_data_with_options_async(request, runtime)
 
     def describe_domain_real_time_src_traffic_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeSrcTrafficDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeSrcTrafficDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 10 times per second per account.
+        * If you do not specify the StartTime or EndTime parameter, the request returns the data collected in the last hour by default. If you specify both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Historical data available | Time range to query | Data delay |
-        | ---------------- | ------------------------- | ------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeSrcTrafficDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeSrcTrafficDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9241,23 +9309,23 @@
 
     async def describe_domain_real_time_src_traffic_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeSrcTrafficDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeSrcTrafficDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 10 times per second per account.
+        * If you do not specify the StartTime or EndTime parameter, the request returns the data collected in the last hour by default. If you specify both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Historical data available | Time range to query | Data delay |
-        | ---------------- | ------------------------- | ------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeSrcTrafficDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeSrcTrafficDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9287,66 +9355,66 @@
         )
 
     def describe_domain_real_time_src_traffic_data(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeSrcTrafficDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeSrcTrafficDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 10 times per second per account.
+        * If you do not specify the StartTime or EndTime parameter, the request returns the data collected in the last hour by default. If you specify both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Historical data available | Time range to query | Data delay |
-        | ---------------- | ------------------------- | ------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeSrcTrafficDataRequest
         @return: DescribeDomainRealTimeSrcTrafficDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_real_time_src_traffic_data_with_options(request, runtime)
 
     async def describe_domain_real_time_src_traffic_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeSrcTrafficDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeSrcTrafficDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 10.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 10 times per second per account.
+        * If you do not specify the StartTime or EndTime parameter, the request returns the data collected in the last hour by default. If you specify both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Historical data available | Time range to query | Data delay |
-        | ---------------- | ------------------------- | ------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeSrcTrafficDataRequest
         @return: DescribeDomainRealTimeSrcTrafficDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_real_time_src_traffic_data_with_options_async(request, runtime)
 
     def describe_domain_real_time_traffic_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeTrafficDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeTrafficDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 50.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 50 times per second per account.
+        * If you do not specify the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you specify both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeTrafficDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeTrafficDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9381,23 +9449,23 @@
 
     async def describe_domain_real_time_traffic_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeTrafficDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainRealTimeTrafficDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 50.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 50 times per second per account.
+        * If you do not specify the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you specify both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeTrafficDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainRealTimeTrafficDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9431,44 +9499,44 @@
         )
 
     def describe_domain_real_time_traffic_data(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeTrafficDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeTrafficDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 50.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 50 times per second per account.
+        * If you do not specify the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you specify both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeTrafficDataRequest
         @return: DescribeDomainRealTimeTrafficDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_real_time_traffic_data_with_options(request, runtime)
 
     async def describe_domain_real_time_traffic_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainRealTimeTrafficDataRequest,
     ) -> cdn_20180510_models.DescribeDomainRealTimeTrafficDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 50.
-        - If you do not set StartTime or EndTime, data collected within the last hour is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 50 times per second per account.
+        * If you do not specify the StartTime or EndTime parameter, the request returns the data collected in the last hour. If you specify both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity varies with the time range specified by the StartTime and EndTime parameters. The following table describes the time period within which historical data is available and the data delay.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 1 minute | 1 hour | 7 days | 5 minutes |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |1 minute|1 hour|7 days|5 minutes|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
         
         @param request: DescribeDomainRealTimeTrafficDataRequest
         @return: DescribeDomainRealTimeTrafficDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_real_time_traffic_data_with_options_async(request, runtime)
 
@@ -9682,23 +9750,23 @@
 
     def describe_domain_req_hit_rate_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainReqHitRateDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainReqHitRateDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainReqHitRateDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainReqHitRateDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9731,23 +9799,23 @@
 
     async def describe_domain_req_hit_rate_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainReqHitRateDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainReqHitRateDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainReqHitRateDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainReqHitRateDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9779,66 +9847,66 @@
         )
 
     def describe_domain_req_hit_rate_data(
         self,
         request: cdn_20180510_models.DescribeDomainReqHitRateDataRequest,
     ) -> cdn_20180510_models.DescribeDomainReqHitRateDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainReqHitRateDataRequest
         @return: DescribeDomainReqHitRateDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_req_hit_rate_data_with_options(request, runtime)
 
     async def describe_domain_req_hit_rate_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainReqHitRateDataRequest,
     ) -> cdn_20180510_models.DescribeDomainReqHitRateDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainReqHitRateDataRequest
         @return: DescribeDomainReqHitRateDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_req_hit_rate_data_with_options_async(request, runtime)
 
     def describe_domain_src_bps_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainSrcBpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainSrcBpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not specify the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you specify both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainSrcBpsDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainSrcBpsDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9871,23 +9939,23 @@
 
     async def describe_domain_src_bps_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainSrcBpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainSrcBpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not specify the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you specify both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainSrcBpsDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainSrcBpsDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9919,66 +9987,66 @@
         )
 
     def describe_domain_src_bps_data(
         self,
         request: cdn_20180510_models.DescribeDomainSrcBpsDataRequest,
     ) -> cdn_20180510_models.DescribeDomainSrcBpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not specify the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you specify both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainSrcBpsDataRequest
         @return: DescribeDomainSrcBpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_src_bps_data_with_options(request, runtime)
 
     async def describe_domain_src_bps_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainSrcBpsDataRequest,
     ) -> cdn_20180510_models.DescribeDomainSrcBpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not specify the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you specify both the StartTime and EndTime parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
         The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainSrcBpsDataRequest
         @return: DescribeDomainSrcBpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_src_bps_data_with_options_async(request, runtime)
 
     def describe_domain_src_http_code_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainSrcHttpCodeDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainSrcHttpCodeDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainSrcHttpCodeDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainSrcHttpCodeDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10011,23 +10079,23 @@
 
     async def describe_domain_src_http_code_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainSrcHttpCodeDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainSrcHttpCodeDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainSrcHttpCodeDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainSrcHttpCodeDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10059,66 +10127,66 @@
         )
 
     def describe_domain_src_http_code_data(
         self,
         request: cdn_20180510_models.DescribeDomainSrcHttpCodeDataRequest,
     ) -> cdn_20180510_models.DescribeDomainSrcHttpCodeDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainSrcHttpCodeDataRequest
         @return: DescribeDomainSrcHttpCodeDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_src_http_code_data_with_options(request, runtime)
 
     async def describe_domain_src_http_code_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainSrcHttpCodeDataRequest,
     ) -> cdn_20180510_models.DescribeDomainSrcHttpCodeDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainSrcHttpCodeDataRequest
         @return: DescribeDomainSrcHttpCodeDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_src_http_code_data_with_options_async(request, runtime)
 
     def describe_domain_src_qps_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainSrcQpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainSrcQpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        ### Time granularity
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainSrcQpsDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainSrcQpsDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10151,23 +10219,23 @@
 
     async def describe_domain_src_qps_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainSrcQpsDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainSrcQpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        ### Time granularity
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainSrcQpsDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainSrcQpsDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10199,44 +10267,44 @@
         )
 
     def describe_domain_src_qps_data(
         self,
         request: cdn_20180510_models.DescribeDomainSrcQpsDataRequest,
     ) -> cdn_20180510_models.DescribeDomainSrcQpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        ### Time granularity
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainSrcQpsDataRequest
         @return: DescribeDomainSrcQpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_src_qps_data_with_options(request, runtime)
 
     async def describe_domain_src_qps_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainSrcQpsDataRequest,
     ) -> cdn_20180510_models.DescribeDomainSrcQpsDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
-        **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        ### Time granularity
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainSrcQpsDataRequest
         @return: DescribeDomainSrcQpsDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_src_qps_data_with_options_async(request, runtime)
 
@@ -10358,23 +10426,23 @@
 
     def describe_domain_src_traffic_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainSrcTrafficDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainSrcTrafficDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainSrcTrafficDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainSrcTrafficDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10407,23 +10475,23 @@
 
     async def describe_domain_src_traffic_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainSrcTrafficDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainSrcTrafficDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainSrcTrafficDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainSrcTrafficDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10455,44 +10523,44 @@
         )
 
     def describe_domain_src_traffic_data(
         self,
         request: cdn_20180510_models.DescribeDomainSrcTrafficDataRequest,
     ) -> cdn_20180510_models.DescribeDomainSrcTrafficDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainSrcTrafficDataRequest
         @return: DescribeDomainSrcTrafficDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_src_traffic_data_with_options(request, runtime)
 
     async def describe_domain_src_traffic_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainSrcTrafficDataRequest,
     ) -> cdn_20180510_models.DescribeDomainSrcTrafficDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainSrcTrafficDataRequest
         @return: DescribeDomainSrcTrafficDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_src_traffic_data_with_options_async(request, runtime)
 
@@ -10746,18 +10814,20 @@
 
     def describe_domain_top_url_visit_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainTopUrlVisitRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainTopUrlVisitResponse:
         """
-        > - If you do not set StartTime or EndTime, data within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
-        - You can query data collected within the last 90 days.
-        - You can specify only one domain name in each call.
-        - You can call this operation up to 10 times per second per account.
+        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](~~279577~~) feature for data analysis.
+        >
+        *   If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        *   You can query data collected in the last 90 days.
+        *   You can specify only one domain name in each call.
+        *   You can call this operation up to 10 times per second per account.
         
         @param request: DescribeDomainTopUrlVisitRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainTopUrlVisitResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10790,18 +10860,20 @@
 
     async def describe_domain_top_url_visit_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainTopUrlVisitRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainTopUrlVisitResponse:
         """
-        > - If you do not set StartTime or EndTime, data within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
-        - You can query data collected within the last 90 days.
-        - You can specify only one domain name in each call.
-        - You can call this operation up to 10 times per second per account.
+        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](~~279577~~) feature for data analysis.
+        >
+        *   If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        *   You can query data collected in the last 90 days.
+        *   You can specify only one domain name in each call.
+        *   You can call this operation up to 10 times per second per account.
         
         @param request: DescribeDomainTopUrlVisitRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainTopUrlVisitResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10833,56 +10905,60 @@
         )
 
     def describe_domain_top_url_visit(
         self,
         request: cdn_20180510_models.DescribeDomainTopUrlVisitRequest,
     ) -> cdn_20180510_models.DescribeDomainTopUrlVisitResponse:
         """
-        > - If you do not set StartTime or EndTime, data within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
-        - You can query data collected within the last 90 days.
-        - You can specify only one domain name in each call.
-        - You can call this operation up to 10 times per second per account.
+        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](~~279577~~) feature for data analysis.
+        >
+        *   If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        *   You can query data collected in the last 90 days.
+        *   You can specify only one domain name in each call.
+        *   You can call this operation up to 10 times per second per account.
         
         @param request: DescribeDomainTopUrlVisitRequest
         @return: DescribeDomainTopUrlVisitResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_top_url_visit_with_options(request, runtime)
 
     async def describe_domain_top_url_visit_async(
         self,
         request: cdn_20180510_models.DescribeDomainTopUrlVisitRequest,
     ) -> cdn_20180510_models.DescribeDomainTopUrlVisitResponse:
         """
-        > - If you do not set StartTime or EndTime, data within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
-        - You can query data collected within the last 90 days.
-        - You can specify only one domain name in each call.
-        - You can call this operation up to 10 times per second per account.
+        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](~~279577~~) feature for data analysis.
+        >
+        *   If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        *   You can query data collected in the last 90 days.
+        *   You can specify only one domain name in each call.
+        *   You can call this operation up to 10 times per second per account.
         
         @param request: DescribeDomainTopUrlVisitRequest
         @return: DescribeDomainTopUrlVisitResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_top_url_visit_with_options_async(request, runtime)
 
     def describe_domain_traffic_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainTrafficDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainTrafficDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366|04:00 on the next day|
         
         @param request: DescribeDomainTrafficDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainTrafficDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10919,23 +10995,23 @@
 
     async def describe_domain_traffic_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainTrafficDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainTrafficDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366|04:00 on the next day|
         
         @param request: DescribeDomainTrafficDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainTrafficDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10971,66 +11047,64 @@
         )
 
     def describe_domain_traffic_data(
         self,
         request: cdn_20180510_models.DescribeDomainTrafficDataRequest,
     ) -> cdn_20180510_models.DescribeDomainTrafficDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366|04:00 on the next day|
         
         @param request: DescribeDomainTrafficDataRequest
         @return: DescribeDomainTrafficDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_traffic_data_with_options(request, runtime)
 
     async def describe_domain_traffic_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainTrafficDataRequest,
     ) -> cdn_20180510_models.DescribeDomainTrafficDataResponse:
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data collected within the specified time range is queried.
+        You can call this operation up to 100 times per second per account.
+        * If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
         **Time granularity**\
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 366 days | 366 days | 04:00 on the next day |
+        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the maximum time range per query, as described in the following table.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|366 days|366|04:00 on the next day|
         
         @param request: DescribeDomainTrafficDataRequest
         @return: DescribeDomainTrafficDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_traffic_data_with_options_async(request, runtime)
 
     def describe_domain_usage_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainUsageDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainUsageDataResponse:
         """
-        The maximum number of times that each user can call this operation per second is 10.
-        
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 90 days | 366 days | 04:00 on the next day |
+        You can call this operation up to 10 times per second per account.
+        * The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|90 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainUsageDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainUsageDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11071,23 +11145,21 @@
 
     async def describe_domain_usage_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainUsageDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainUsageDataResponse:
         """
-        The maximum number of times that each user can call this operation per second is 10.
-        
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 90 days | 366 days | 04:00 on the next day |
+        You can call this operation up to 10 times per second per account.
+        * The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|90 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainUsageDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainUsageDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11127,61 +11199,58 @@
         )
 
     def describe_domain_usage_data(
         self,
         request: cdn_20180510_models.DescribeDomainUsageDataRequest,
     ) -> cdn_20180510_models.DescribeDomainUsageDataResponse:
         """
-        The maximum number of times that each user can call this operation per second is 10.
-        
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 90 days | 366 days | 04:00 on the next day |
+        You can call this operation up to 10 times per second per account.
+        * The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|90 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainUsageDataRequest
         @return: DescribeDomainUsageDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_usage_data_with_options(request, runtime)
 
     async def describe_domain_usage_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainUsageDataRequest,
     ) -> cdn_20180510_models.DescribeDomainUsageDataResponse:
         """
-        The maximum number of times that each user can call this operation per second is 10.
-        
-        The time granularity supported by the Interval parameter, the maximum time period within which historical data is available, and the data delay vary with the time range to query, as described in the following table.
-        
-        | Time granularity | Time range to query | Historical data available | Data delay |
-        | ---------------- | ------------------- | ------------------------- | ---------- |
-        | 5 minutes | 3 days | 93 days | 15 minutes |
-        | 1 hour | 31 days | 186 days | 4 hours |
-        | 1 day | 90 days | 366 days | 04:00 on the next day |
+        You can call this operation up to 10 times per second per account.
+        * The time granularity supported by the Interval parameter varies with the maximum time range per query. The following table describes the time period within which historical data is available and the data delay.
+        |Time granularity|Maximum time range per query|Historical data available|Data delay|
+        |---|---|---|---|
+        |5 minutes|3 days|93 days|15 minutes|
+        |1 hour|31 days|186 days|4 hours|
+        |1 day|90 days|366 days|04:00 on the next day|
         
         @param request: DescribeDomainUsageDataRequest
         @return: DescribeDomainUsageDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_usage_data_with_options_async(request, runtime)
 
     def describe_domain_uv_data_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainUvDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainUvDataResponse:
         """
-        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, monitoring data within the last 24 hours is queried. If you set both StartTime and EndTime, monitoring data within the specified time range is queried.
-        - You can specify only one accelerated domain name or all accelerated domain names under your Alibaba Cloud account.
-        - You can call this operation up to 100 times per second per account.
+        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](~~279577~~) feature for data analysis.
+        >
+        *   If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        *   You can specify only one accelerated domain name or all accelerated domain names in your Alibaba Cloud account.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDomainUvDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainUvDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11212,18 +11281,19 @@
 
     async def describe_domain_uv_data_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainUvDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainUvDataResponse:
         """
-        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, monitoring data within the last 24 hours is queried. If you set both StartTime and EndTime, monitoring data within the specified time range is queried.
-        - You can specify only one accelerated domain name or all accelerated domain names under your Alibaba Cloud account.
-        - You can call this operation up to 100 times per second per account.
+        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](~~279577~~) feature for data analysis.
+        >
+        *   If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        *   You can specify only one accelerated domain name or all accelerated domain names in your Alibaba Cloud account.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDomainUvDataRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainUvDataResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11253,34 +11323,36 @@
         )
 
     def describe_domain_uv_data(
         self,
         request: cdn_20180510_models.DescribeDomainUvDataRequest,
     ) -> cdn_20180510_models.DescribeDomainUvDataResponse:
         """
-        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, monitoring data within the last 24 hours is queried. If you set both StartTime and EndTime, monitoring data within the specified time range is queried.
-        - You can specify only one accelerated domain name or all accelerated domain names under your Alibaba Cloud account.
-        - You can call this operation up to 100 times per second per account.
+        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](~~279577~~) feature for data analysis.
+        >
+        *   If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        *   You can specify only one accelerated domain name or all accelerated domain names in your Alibaba Cloud account.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDomainUvDataRequest
         @return: DescribeDomainUvDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_uv_data_with_options(request, runtime)
 
     async def describe_domain_uv_data_async(
         self,
         request: cdn_20180510_models.DescribeDomainUvDataRequest,
     ) -> cdn_20180510_models.DescribeDomainUvDataResponse:
         """
-        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/customize-an-operations-report-template-and-create-a-tracking-task) feature to for data analysis.
-        > - If you do not set StartTime or EndTime, monitoring data within the last 24 hours is queried. If you set both StartTime and EndTime, monitoring data within the specified time range is queried.
-        - You can specify only one accelerated domain name or all accelerated domain names under your Alibaba Cloud account.
-        - You can call this operation up to 100 times per second per account.
+        The statistical analysis feature of Alibaba Cloud CDN is no longer available. The API operations related to the statistical analysis feature are no longer maintained. We recommend that you do not use the API operations because data may be missing or inaccurate. You can use the [operations report](~~279577~~) feature for data analysis.
+        >
+        *   If you do not set the StartTime or EndTime parameter, the request returns the data collected in the last 24 hours. If you set both these parameters, the request returns the data collected within the specified time range.
+        *   You can specify only one accelerated domain name or all accelerated domain names in your Alibaba Cloud account.
+        *   You can call this operation up to 100 times per second per account.
         
         @param request: DescribeDomainUvDataRequest
         @return: DescribeDomainUvDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_uv_data_with_options_async(request, runtime)
 
@@ -11390,16 +11462,17 @@
 
     def describe_domains_usage_by_day_with_options(
         self,
         request: cdn_20180510_models.DescribeDomainsUsageByDayRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainsUsageByDayResponse:
         """
-        > - If you do not set StartTime or EndTime, data within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
-        > - You can query the monitoring data of a specific accelerated domain name or all accelerated domain names that belong to your Alibaba Cloud account.
+        You can call this operation up to 10 times per second per account.
+        *   If you do not set StartTime or EndTime, data within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
+        *   You can query the monitoring data of a specific accelerated domain name or all accelerated domain names that belong to your Alibaba Cloud account.
         
         @param request: DescribeDomainsUsageByDayRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainsUsageByDayResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11430,16 +11503,17 @@
 
     async def describe_domains_usage_by_day_with_options_async(
         self,
         request: cdn_20180510_models.DescribeDomainsUsageByDayRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeDomainsUsageByDayResponse:
         """
-        > - If you do not set StartTime or EndTime, data within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
-        > - You can query the monitoring data of a specific accelerated domain name or all accelerated domain names that belong to your Alibaba Cloud account.
+        You can call this operation up to 10 times per second per account.
+        *   If you do not set StartTime or EndTime, data within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
+        *   You can query the monitoring data of a specific accelerated domain name or all accelerated domain names that belong to your Alibaba Cloud account.
         
         @param request: DescribeDomainsUsageByDayRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDomainsUsageByDayResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11469,30 +11543,32 @@
         )
 
     def describe_domains_usage_by_day(
         self,
         request: cdn_20180510_models.DescribeDomainsUsageByDayRequest,
     ) -> cdn_20180510_models.DescribeDomainsUsageByDayResponse:
         """
-        > - If you do not set StartTime or EndTime, data within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
-        > - You can query the monitoring data of a specific accelerated domain name or all accelerated domain names that belong to your Alibaba Cloud account.
+        You can call this operation up to 10 times per second per account.
+        *   If you do not set StartTime or EndTime, data within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
+        *   You can query the monitoring data of a specific accelerated domain name or all accelerated domain names that belong to your Alibaba Cloud account.
         
         @param request: DescribeDomainsUsageByDayRequest
         @return: DescribeDomainsUsageByDayResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domains_usage_by_day_with_options(request, runtime)
 
     async def describe_domains_usage_by_day_async(
         self,
         request: cdn_20180510_models.DescribeDomainsUsageByDayRequest,
     ) -> cdn_20180510_models.DescribeDomainsUsageByDayResponse:
         """
-        > - If you do not set StartTime or EndTime, data within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
-        > - You can query the monitoring data of a specific accelerated domain name or all accelerated domain names that belong to your Alibaba Cloud account.
+        You can call this operation up to 10 times per second per account.
+        *   If you do not set StartTime or EndTime, data within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
+        *   You can query the monitoring data of a specific accelerated domain name or all accelerated domain names that belong to your Alibaba Cloud account.
         
         @param request: DescribeDomainsUsageByDayRequest
         @return: DescribeDomainsUsageByDayResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domains_usage_by_day_with_options_async(request, runtime)
 
@@ -12239,15 +12315,15 @@
     def describe_range_data_by_locate_and_isp_service_with_options(
         self,
         request: cdn_20180510_models.DescribeRangeDataByLocateAndIspServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeRangeDataByLocateAndIspServiceResponse:
         """
         The data is collected every 5 minutes.
-        *   The maximum number of times that each user can call this operation per second is 20.
+        *   You can call this operation up to 20 times per second per account.
         
         @param request: DescribeRangeDataByLocateAndIspServiceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeRangeDataByLocateAndIspServiceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12283,15 +12359,15 @@
     async def describe_range_data_by_locate_and_isp_service_with_options_async(
         self,
         request: cdn_20180510_models.DescribeRangeDataByLocateAndIspServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.DescribeRangeDataByLocateAndIspServiceResponse:
         """
         The data is collected every 5 minutes.
-        *   The maximum number of times that each user can call this operation per second is 20.
+        *   You can call this operation up to 20 times per second per account.
         
         @param request: DescribeRangeDataByLocateAndIspServiceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeRangeDataByLocateAndIspServiceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12326,29 +12402,29 @@
 
     def describe_range_data_by_locate_and_isp_service(
         self,
         request: cdn_20180510_models.DescribeRangeDataByLocateAndIspServiceRequest,
     ) -> cdn_20180510_models.DescribeRangeDataByLocateAndIspServiceResponse:
         """
         The data is collected every 5 minutes.
-        *   The maximum number of times that each user can call this operation per second is 20.
+        *   You can call this operation up to 20 times per second per account.
         
         @param request: DescribeRangeDataByLocateAndIspServiceRequest
         @return: DescribeRangeDataByLocateAndIspServiceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_range_data_by_locate_and_isp_service_with_options(request, runtime)
 
     async def describe_range_data_by_locate_and_isp_service_async(
         self,
         request: cdn_20180510_models.DescribeRangeDataByLocateAndIspServiceRequest,
     ) -> cdn_20180510_models.DescribeRangeDataByLocateAndIspServiceResponse:
         """
         The data is collected every 5 minutes.
-        *   The maximum number of times that each user can call this operation per second is 20.
+        *   You can call this operation up to 20 times per second per account.
         
         @param request: DescribeRangeDataByLocateAndIspServiceRequest
         @return: DescribeRangeDataByLocateAndIspServiceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_range_data_by_locate_and_isp_service_with_options_async(request, runtime)
 
@@ -15042,23 +15118,23 @@
         self,
         request: cdn_20180510_models.PushObjectCacheRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.PushObjectCacheResponse:
         """
         Alibaba Cloud CDN supports POST requests in which parameters are sent as a form.
         *   You can call the [RefreshObjectCaches](~~91164~~) operation to refresh content and call the [PushObjectCache](~~91161~~) operation to prefetch content.
-        *   Each Alibaba Cloud account can submit at most 1,000 URLs per day. If your daily peak bandwidth exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to increase the upper limit. Alibaba Cloud will review your application and then increase the quota accordingly.
-        *   Each Alibaba Cloud account can submit up to 100 URLs at a time.
+        *   By default, each Alibaba Cloud account can submit up to 1,000 URLs per day. If the daily peak bandwidth value of your workloads exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to increase your daily quota. Alibaba Cloud reviews your application and then increases the quota accordingly.
+        *   You can specify at most 100 URLs in each prefetch request.
         *   For each Alibaba Cloud account, the prefetch queue can contain up to 50,000 URLs. Content is prefetched based on the time when the URLs are submitted. The URL that is submitted the earliest has the highest priority. If the number of URLs in the queue reaches 50,000, you cannot submit more URLs until the number drops below 50,000.
         *   You can call this operation up to 50 times per second per account.
-        *   For more information about how to automate refresh or prefetch tasks, see [Prefetch and refresh task scripts](~~151829~~).
+        *   For more information about how to automate refresh or prefetch tasks, see [Run scripts to refresh and prefetch content](~~151829~~).
         ## Precautions
-        - After a refresh task is submitted and completed, the POPs immediately start to retrieve resources from the origin server. Therefore, a large number of refresh tasks cause a large number of concurrent download tasks. This increases the number of requests that are redirected to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
-        - The time required for a prefetch task to complete is proportional to the size of the prefetched file. In actual practice, most prefetch tasks take 5 to 30 minutes to complete. A task with a smaller average file size takes less time.
-        - To allow Resource Access Management (RAM) users to perform this operation, you must first grant them the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~260300~~).
+        *   After a prefetch task is submitted and completed, the POPs immediately start to retrieve resources from the origin server. Therefore, a large number of refresh tasks cause a large number of concurrent download tasks. This increases the number of requests that are redirected to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
+        *   The time required for a prefetch task to complete is proportional to the size of the prefetched file. In actual practice, most prefetch tasks require 5 to 30 minutes to complete. A task with a smaller average file size requires less time.
+        *   To allow RAM users to perform this operation, you must first grant them the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~260300~~).
         
         @param request: PushObjectCacheRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: PushObjectCacheResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -15097,23 +15173,23 @@
         self,
         request: cdn_20180510_models.PushObjectCacheRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.PushObjectCacheResponse:
         """
         Alibaba Cloud CDN supports POST requests in which parameters are sent as a form.
         *   You can call the [RefreshObjectCaches](~~91164~~) operation to refresh content and call the [PushObjectCache](~~91161~~) operation to prefetch content.
-        *   Each Alibaba Cloud account can submit at most 1,000 URLs per day. If your daily peak bandwidth exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to increase the upper limit. Alibaba Cloud will review your application and then increase the quota accordingly.
-        *   Each Alibaba Cloud account can submit up to 100 URLs at a time.
+        *   By default, each Alibaba Cloud account can submit up to 1,000 URLs per day. If the daily peak bandwidth value of your workloads exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to increase your daily quota. Alibaba Cloud reviews your application and then increases the quota accordingly.
+        *   You can specify at most 100 URLs in each prefetch request.
         *   For each Alibaba Cloud account, the prefetch queue can contain up to 50,000 URLs. Content is prefetched based on the time when the URLs are submitted. The URL that is submitted the earliest has the highest priority. If the number of URLs in the queue reaches 50,000, you cannot submit more URLs until the number drops below 50,000.
         *   You can call this operation up to 50 times per second per account.
-        *   For more information about how to automate refresh or prefetch tasks, see [Prefetch and refresh task scripts](~~151829~~).
+        *   For more information about how to automate refresh or prefetch tasks, see [Run scripts to refresh and prefetch content](~~151829~~).
         ## Precautions
-        - After a refresh task is submitted and completed, the POPs immediately start to retrieve resources from the origin server. Therefore, a large number of refresh tasks cause a large number of concurrent download tasks. This increases the number of requests that are redirected to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
-        - The time required for a prefetch task to complete is proportional to the size of the prefetched file. In actual practice, most prefetch tasks take 5 to 30 minutes to complete. A task with a smaller average file size takes less time.
-        - To allow Resource Access Management (RAM) users to perform this operation, you must first grant them the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~260300~~).
+        *   After a prefetch task is submitted and completed, the POPs immediately start to retrieve resources from the origin server. Therefore, a large number of refresh tasks cause a large number of concurrent download tasks. This increases the number of requests that are redirected to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
+        *   The time required for a prefetch task to complete is proportional to the size of the prefetched file. In actual practice, most prefetch tasks require 5 to 30 minutes to complete. A task with a smaller average file size requires less time.
+        *   To allow RAM users to perform this operation, you must first grant them the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~260300~~).
         
         @param request: PushObjectCacheRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: PushObjectCacheResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -15151,46 +15227,46 @@
     def push_object_cache(
         self,
         request: cdn_20180510_models.PushObjectCacheRequest,
     ) -> cdn_20180510_models.PushObjectCacheResponse:
         """
         Alibaba Cloud CDN supports POST requests in which parameters are sent as a form.
         *   You can call the [RefreshObjectCaches](~~91164~~) operation to refresh content and call the [PushObjectCache](~~91161~~) operation to prefetch content.
-        *   Each Alibaba Cloud account can submit at most 1,000 URLs per day. If your daily peak bandwidth exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to increase the upper limit. Alibaba Cloud will review your application and then increase the quota accordingly.
-        *   Each Alibaba Cloud account can submit up to 100 URLs at a time.
+        *   By default, each Alibaba Cloud account can submit up to 1,000 URLs per day. If the daily peak bandwidth value of your workloads exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to increase your daily quota. Alibaba Cloud reviews your application and then increases the quota accordingly.
+        *   You can specify at most 100 URLs in each prefetch request.
         *   For each Alibaba Cloud account, the prefetch queue can contain up to 50,000 URLs. Content is prefetched based on the time when the URLs are submitted. The URL that is submitted the earliest has the highest priority. If the number of URLs in the queue reaches 50,000, you cannot submit more URLs until the number drops below 50,000.
         *   You can call this operation up to 50 times per second per account.
-        *   For more information about how to automate refresh or prefetch tasks, see [Prefetch and refresh task scripts](~~151829~~).
+        *   For more information about how to automate refresh or prefetch tasks, see [Run scripts to refresh and prefetch content](~~151829~~).
         ## Precautions
-        - After a refresh task is submitted and completed, the POPs immediately start to retrieve resources from the origin server. Therefore, a large number of refresh tasks cause a large number of concurrent download tasks. This increases the number of requests that are redirected to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
-        - The time required for a prefetch task to complete is proportional to the size of the prefetched file. In actual practice, most prefetch tasks take 5 to 30 minutes to complete. A task with a smaller average file size takes less time.
-        - To allow Resource Access Management (RAM) users to perform this operation, you must first grant them the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~260300~~).
+        *   After a prefetch task is submitted and completed, the POPs immediately start to retrieve resources from the origin server. Therefore, a large number of refresh tasks cause a large number of concurrent download tasks. This increases the number of requests that are redirected to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
+        *   The time required for a prefetch task to complete is proportional to the size of the prefetched file. In actual practice, most prefetch tasks require 5 to 30 minutes to complete. A task with a smaller average file size requires less time.
+        *   To allow RAM users to perform this operation, you must first grant them the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~260300~~).
         
         @param request: PushObjectCacheRequest
         @return: PushObjectCacheResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.push_object_cache_with_options(request, runtime)
 
     async def push_object_cache_async(
         self,
         request: cdn_20180510_models.PushObjectCacheRequest,
     ) -> cdn_20180510_models.PushObjectCacheResponse:
         """
         Alibaba Cloud CDN supports POST requests in which parameters are sent as a form.
         *   You can call the [RefreshObjectCaches](~~91164~~) operation to refresh content and call the [PushObjectCache](~~91161~~) operation to prefetch content.
-        *   Each Alibaba Cloud account can submit at most 1,000 URLs per day. If your daily peak bandwidth exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to increase the upper limit. Alibaba Cloud will review your application and then increase the quota accordingly.
-        *   Each Alibaba Cloud account can submit up to 100 URLs at a time.
+        *   By default, each Alibaba Cloud account can submit up to 1,000 URLs per day. If the daily peak bandwidth value of your workloads exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to increase your daily quota. Alibaba Cloud reviews your application and then increases the quota accordingly.
+        *   You can specify at most 100 URLs in each prefetch request.
         *   For each Alibaba Cloud account, the prefetch queue can contain up to 50,000 URLs. Content is prefetched based on the time when the URLs are submitted. The URL that is submitted the earliest has the highest priority. If the number of URLs in the queue reaches 50,000, you cannot submit more URLs until the number drops below 50,000.
         *   You can call this operation up to 50 times per second per account.
-        *   For more information about how to automate refresh or prefetch tasks, see [Prefetch and refresh task scripts](~~151829~~).
+        *   For more information about how to automate refresh or prefetch tasks, see [Run scripts to refresh and prefetch content](~~151829~~).
         ## Precautions
-        - After a refresh task is submitted and completed, the POPs immediately start to retrieve resources from the origin server. Therefore, a large number of refresh tasks cause a large number of concurrent download tasks. This increases the number of requests that are redirected to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
-        - The time required for a prefetch task to complete is proportional to the size of the prefetched file. In actual practice, most prefetch tasks take 5 to 30 minutes to complete. A task with a smaller average file size takes less time.
-        - To allow Resource Access Management (RAM) users to perform this operation, you must first grant them the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~260300~~).
+        *   After a prefetch task is submitted and completed, the POPs immediately start to retrieve resources from the origin server. Therefore, a large number of refresh tasks cause a large number of concurrent download tasks. This increases the number of requests that are redirected to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
+        *   The time required for a prefetch task to complete is proportional to the size of the prefetched file. In actual practice, most prefetch tasks require 5 to 30 minutes to complete. A task with a smaller average file size requires less time.
+        *   To allow RAM users to perform this operation, you must first grant them the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~260300~~).
         
         @param request: PushObjectCacheRequest
         @return: PushObjectCacheResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.push_object_cache_with_options_async(request, runtime)
 
@@ -15198,24 +15274,25 @@
         self,
         request: cdn_20180510_models.RefreshObjectCachesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.RefreshObjectCachesResponse:
         """
         Alibaba Cloud CDN supports POST requests in which parameters are sent as a form.
         *   You can call the [RefreshObjectCaches](~~91164~~) operation to refresh content and call the [PushObjectCache](~~91161~~) operation to prefetch content.
-        *   You can call this operation up to 50 times per second per account.
-        *   For more information about how to automate refresh or prefetch tasks, see [Prefetch and refresh task scripts](~~151829~~).
-        ## Precautions
-        - After a refresh task is submitted and completed, specific resources are removed from POPs. When a POP receives a request for the removed resources, the POP forwards the request to the origin server to retrieve the resources. The retrieved resources are returned to the client and cached on the POP. Multiple refresh tasks may cause a large number of resources to be removed from the POPs. This increases the number of requests that are forwarded to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
-        - A refresh task takes approximately five to six minutes to take effect. If the cache expiration time that you specified for the resources cached on POPs is less than five minutes, you do not need to perform the refresh operation. Wait until the cache expiration time ends.
-        - If you want to use RAM users to refresh or prefetch resources, you must grant the RAM users the permissions to prefetch and refresh resources. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~260300~~).
-        **Refresh quota**- By default, each Alibaba Cloud account can refresh content from up to 10,000 URLs and 100 directories per day. The directories include subdirectories. If the daily peak bandwidth of your Alibaba Cloud account exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to request a quota increase. Alibaba Cloud reviews your request and then increases the quota based on your request.
-        - By default, each Alibaba Cloud account can submit up to 20 refresh rules that contain regular expressions per day. If the daily peak bandwidth of your Alibaba Cloud account exceeds 10 Gbit/s, you can [submit a ticket](https://workorder-intl.console.aliyun.com/#/ticket/createIndex) to request a quota increase.
-        - You can specify up to 1,000 URL refresh rules, 100 directory refresh rules, or 1 refresh rule that contains regular expressions in each call.
-        - You can refresh up to 1,000 URLs per minute for each domain name.
+        *   You can call the RefreshObjectCaches operation up to 50 times per second per account.
+        *   For more information about how to automatically refresh or prefetch tasks, see [Run scripts to refresh and prefetch content](~~151829~~).
+        ## Usage notes
+        *   After a refresh task is submitted and completed, specific resources are removed from POPs. When a POP receives a request for the removed resources, the POP forwards the request to the origin server to retrieve the resources. The retrieved resources are returned to the client and cached on the POP. Multiple refresh tasks may cause a large number of resources to be removed from the POPs. This increases the number of requests that are forwarded to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
+        *   A refresh task takes effect 5 to 6 minutes after being submitted. If the TTL for the resources you want to refresh is less than 5 minutes, you can wait until the TTL expires instead of performing the refresh operation.
+        *   If you want to use RAM users to refresh or prefetch resources, you must obtain the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~260300~~).
+        ### Refresh quota
+        *   By default, each Alibaba Cloud account can refresh content from up to 10,000 URLs and 100 directories per day. The directories include subdirectories. If the daily peak bandwidth value exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to request a quota increase. Alibaba Cloud CDN evaluates your application based on your workloads.
+        *   By default, each Alibaba Cloud account can submit up to 20 refresh rules that contain regular expressions per day. If the daily peak bandwidth of your Alibaba Cloud account exceeds 10 Gbit/s, you can [submit a ticket](https://workorder-intl.console.aliyun.com/#/ticket/createIndex) to request a quota increase.
+        *   You can specify up to 1,000 URL refresh rules, 100 directory refresh rules, or 1 refresh rule that contains regular expressions in each call.
+        *   You can refresh up to 1,000 URLs per minute for each domain name.
         
         @param request: RefreshObjectCachesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: RefreshObjectCachesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -15250,24 +15327,25 @@
         self,
         request: cdn_20180510_models.RefreshObjectCachesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> cdn_20180510_models.RefreshObjectCachesResponse:
         """
         Alibaba Cloud CDN supports POST requests in which parameters are sent as a form.
         *   You can call the [RefreshObjectCaches](~~91164~~) operation to refresh content and call the [PushObjectCache](~~91161~~) operation to prefetch content.
-        *   You can call this operation up to 50 times per second per account.
-        *   For more information about how to automate refresh or prefetch tasks, see [Prefetch and refresh task scripts](~~151829~~).
-        ## Precautions
-        - After a refresh task is submitted and completed, specific resources are removed from POPs. When a POP receives a request for the removed resources, the POP forwards the request to the origin server to retrieve the resources. The retrieved resources are returned to the client and cached on the POP. Multiple refresh tasks may cause a large number of resources to be removed from the POPs. This increases the number of requests that are forwarded to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
-        - A refresh task takes approximately five to six minutes to take effect. If the cache expiration time that you specified for the resources cached on POPs is less than five minutes, you do not need to perform the refresh operation. Wait until the cache expiration time ends.
-        - If you want to use RAM users to refresh or prefetch resources, you must grant the RAM users the permissions to prefetch and refresh resources. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~260300~~).
-        **Refresh quota**- By default, each Alibaba Cloud account can refresh content from up to 10,000 URLs and 100 directories per day. The directories include subdirectories. If the daily peak bandwidth of your Alibaba Cloud account exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to request a quota increase. Alibaba Cloud reviews your request and then increases the quota based on your request.
-        - By default, each Alibaba Cloud account can submit up to 20 refresh rules that contain regular expressions per day. If the daily peak bandwidth of your Alibaba Cloud account exceeds 10 Gbit/s, you can [submit a ticket](https://workorder-intl.console.aliyun.com/#/ticket/createIndex) to request a quota increase.
-        - You can specify up to 1,000 URL refresh rules, 100 directory refresh rules, or 1 refresh rule that contains regular expressions in each call.
-        - You can refresh up to 1,000 URLs per minute for each domain name.
+        *   You can call the RefreshObjectCaches operation up to 50 times per second per account.
+        *   For more information about how to automatically refresh or prefetch tasks, see [Run scripts to refresh and prefetch content](~~151829~~).
+        ## Usage notes
+        *   After a refresh task is submitted and completed, specific resources are removed from POPs. When a POP receives a request for the removed resources, the POP forwards the request to the origin server to retrieve the resources. The retrieved resources are returned to the client and cached on the POP. Multiple refresh tasks may cause a large number of resources to be removed from the POPs. This increases the number of requests that are forwarded to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
+        *   A refresh task takes effect 5 to 6 minutes after being submitted. If the TTL for the resources you want to refresh is less than 5 minutes, you can wait until the TTL expires instead of performing the refresh operation.
+        *   If you want to use RAM users to refresh or prefetch resources, you must obtain the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~260300~~).
+        ### Refresh quota
+        *   By default, each Alibaba Cloud account can refresh content from up to 10,000 URLs and 100 directories per day. The directories include subdirectories. If the daily peak bandwidth value exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to request a quota increase. Alibaba Cloud CDN evaluates your application based on your workloads.
+        *   By default, each Alibaba Cloud account can submit up to 20 refresh rules that contain regular expressions per day. If the daily peak bandwidth of your Alibaba Cloud account exceeds 10 Gbit/s, you can [submit a ticket](https://workorder-intl.console.aliyun.com/#/ticket/createIndex) to request a quota increase.
+        *   You can specify up to 1,000 URL refresh rules, 100 directory refresh rules, or 1 refresh rule that contains regular expressions in each call.
+        *   You can refresh up to 1,000 URLs per minute for each domain name.
         
         @param request: RefreshObjectCachesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: RefreshObjectCachesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -15301,48 +15379,50 @@
     def refresh_object_caches(
         self,
         request: cdn_20180510_models.RefreshObjectCachesRequest,
     ) -> cdn_20180510_models.RefreshObjectCachesResponse:
         """
         Alibaba Cloud CDN supports POST requests in which parameters are sent as a form.
         *   You can call the [RefreshObjectCaches](~~91164~~) operation to refresh content and call the [PushObjectCache](~~91161~~) operation to prefetch content.
-        *   You can call this operation up to 50 times per second per account.
-        *   For more information about how to automate refresh or prefetch tasks, see [Prefetch and refresh task scripts](~~151829~~).
-        ## Precautions
-        - After a refresh task is submitted and completed, specific resources are removed from POPs. When a POP receives a request for the removed resources, the POP forwards the request to the origin server to retrieve the resources. The retrieved resources are returned to the client and cached on the POP. Multiple refresh tasks may cause a large number of resources to be removed from the POPs. This increases the number of requests that are forwarded to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
-        - A refresh task takes approximately five to six minutes to take effect. If the cache expiration time that you specified for the resources cached on POPs is less than five minutes, you do not need to perform the refresh operation. Wait until the cache expiration time ends.
-        - If you want to use RAM users to refresh or prefetch resources, you must grant the RAM users the permissions to prefetch and refresh resources. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~260300~~).
-        **Refresh quota**- By default, each Alibaba Cloud account can refresh content from up to 10,000 URLs and 100 directories per day. The directories include subdirectories. If the daily peak bandwidth of your Alibaba Cloud account exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to request a quota increase. Alibaba Cloud reviews your request and then increases the quota based on your request.
-        - By default, each Alibaba Cloud account can submit up to 20 refresh rules that contain regular expressions per day. If the daily peak bandwidth of your Alibaba Cloud account exceeds 10 Gbit/s, you can [submit a ticket](https://workorder-intl.console.aliyun.com/#/ticket/createIndex) to request a quota increase.
-        - You can specify up to 1,000 URL refresh rules, 100 directory refresh rules, or 1 refresh rule that contains regular expressions in each call.
-        - You can refresh up to 1,000 URLs per minute for each domain name.
+        *   You can call the RefreshObjectCaches operation up to 50 times per second per account.
+        *   For more information about how to automatically refresh or prefetch tasks, see [Run scripts to refresh and prefetch content](~~151829~~).
+        ## Usage notes
+        *   After a refresh task is submitted and completed, specific resources are removed from POPs. When a POP receives a request for the removed resources, the POP forwards the request to the origin server to retrieve the resources. The retrieved resources are returned to the client and cached on the POP. Multiple refresh tasks may cause a large number of resources to be removed from the POPs. This increases the number of requests that are forwarded to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
+        *   A refresh task takes effect 5 to 6 minutes after being submitted. If the TTL for the resources you want to refresh is less than 5 minutes, you can wait until the TTL expires instead of performing the refresh operation.
+        *   If you want to use RAM users to refresh or prefetch resources, you must obtain the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~260300~~).
+        ### Refresh quota
+        *   By default, each Alibaba Cloud account can refresh content from up to 10,000 URLs and 100 directories per day. The directories include subdirectories. If the daily peak bandwidth value exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to request a quota increase. Alibaba Cloud CDN evaluates your application based on your workloads.
+        *   By default, each Alibaba Cloud account can submit up to 20 refresh rules that contain regular expressions per day. If the daily peak bandwidth of your Alibaba Cloud account exceeds 10 Gbit/s, you can [submit a ticket](https://workorder-intl.console.aliyun.com/#/ticket/createIndex) to request a quota increase.
+        *   You can specify up to 1,000 URL refresh rules, 100 directory refresh rules, or 1 refresh rule that contains regular expressions in each call.
+        *   You can refresh up to 1,000 URLs per minute for each domain name.
         
         @param request: RefreshObjectCachesRequest
         @return: RefreshObjectCachesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.refresh_object_caches_with_options(request, runtime)
 
     async def refresh_object_caches_async(
         self,
         request: cdn_20180510_models.RefreshObjectCachesRequest,
     ) -> cdn_20180510_models.RefreshObjectCachesResponse:
         """
         Alibaba Cloud CDN supports POST requests in which parameters are sent as a form.
         *   You can call the [RefreshObjectCaches](~~91164~~) operation to refresh content and call the [PushObjectCache](~~91161~~) operation to prefetch content.
-        *   You can call this operation up to 50 times per second per account.
-        *   For more information about how to automate refresh or prefetch tasks, see [Prefetch and refresh task scripts](~~151829~~).
-        ## Precautions
-        - After a refresh task is submitted and completed, specific resources are removed from POPs. When a POP receives a request for the removed resources, the POP forwards the request to the origin server to retrieve the resources. The retrieved resources are returned to the client and cached on the POP. Multiple refresh tasks may cause a large number of resources to be removed from the POPs. This increases the number of requests that are forwarded to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
-        - A refresh task takes approximately five to six minutes to take effect. If the cache expiration time that you specified for the resources cached on POPs is less than five minutes, you do not need to perform the refresh operation. Wait until the cache expiration time ends.
-        - If you want to use RAM users to refresh or prefetch resources, you must grant the RAM users the permissions to prefetch and refresh resources. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~260300~~).
-        **Refresh quota**- By default, each Alibaba Cloud account can refresh content from up to 10,000 URLs and 100 directories per day. The directories include subdirectories. If the daily peak bandwidth of your Alibaba Cloud account exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to request a quota increase. Alibaba Cloud reviews your request and then increases the quota based on your request.
-        - By default, each Alibaba Cloud account can submit up to 20 refresh rules that contain regular expressions per day. If the daily peak bandwidth of your Alibaba Cloud account exceeds 10 Gbit/s, you can [submit a ticket](https://workorder-intl.console.aliyun.com/#/ticket/createIndex) to request a quota increase.
-        - You can specify up to 1,000 URL refresh rules, 100 directory refresh rules, or 1 refresh rule that contains regular expressions in each call.
-        - You can refresh up to 1,000 URLs per minute for each domain name.
+        *   You can call the RefreshObjectCaches operation up to 50 times per second per account.
+        *   For more information about how to automatically refresh or prefetch tasks, see [Run scripts to refresh and prefetch content](~~151829~~).
+        ## Usage notes
+        *   After a refresh task is submitted and completed, specific resources are removed from POPs. When a POP receives a request for the removed resources, the POP forwards the request to the origin server to retrieve the resources. The retrieved resources are returned to the client and cached on the POP. Multiple refresh tasks may cause a large number of resources to be removed from the POPs. This increases the number of requests that are forwarded to the origin server. The back-to-origin routing process consumes more bandwidth resources and the origin server may be overwhelmed.
+        *   A refresh task takes effect 5 to 6 minutes after being submitted. If the TTL for the resources you want to refresh is less than 5 minutes, you can wait until the TTL expires instead of performing the refresh operation.
+        *   If you want to use RAM users to refresh or prefetch resources, you must obtain the required permissions. For more information, see [Authorize a RAM user to prefetch and refresh resources](~~260300~~).
+        ### Refresh quota
+        *   By default, each Alibaba Cloud account can refresh content from up to 10,000 URLs and 100 directories per day. The directories include subdirectories. If the daily peak bandwidth value exceeds 200 Mbit/s, you can [submit a ticket](https://account.alibabacloud.com/login/login.htm?oauth_callback=https%3A//ticket-intl.console.aliyun.com/%23/ticket/createIndex) to request a quota increase. Alibaba Cloud CDN evaluates your application based on your workloads.
+        *   By default, each Alibaba Cloud account can submit up to 20 refresh rules that contain regular expressions per day. If the daily peak bandwidth of your Alibaba Cloud account exceeds 10 Gbit/s, you can [submit a ticket](https://workorder-intl.console.aliyun.com/#/ticket/createIndex) to request a quota increase.
+        *   You can specify up to 1,000 URL refresh rules, 100 directory refresh rules, or 1 refresh rule that contains regular expressions in each call.
+        *   You can refresh up to 1,000 URLs per minute for each domain name.
         
         @param request: RefreshObjectCachesRequest
         @return: RefreshObjectCachesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.refresh_object_caches_with_options_async(request, runtime)
```

### Comparing `alibabacloud_cdn20180510-1.2.6/alibabacloud_cdn20180510/models.py` & `alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1219,15 +1219,15 @@
 class BatchStopCdnDomainRequest(TeaModel):
     def __init__(
         self,
         domain_names: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
-        # You can specify one or more domain names and separate them with commas (,).
+        # The names of the accelerated domain names. You can specify one or more domain names in each request. Separate multiple domain names with commas (,).
         self.domain_names = domain_names
         self.owner_id = owner_id
         self.security_token = security_token
 
     def validate(self):
         pass
 
@@ -1776,30 +1776,30 @@
     def __init__(
         self,
         domain_name: str = None,
         report_ids: str = None,
     ):
         # The domain names to be tracked. Separate multiple domain names with commas (,). You can specify up to 500 domain names. If you want to specify more than 500 domain names, [submit a ticket](https://workorder-intl.console.aliyun.com/?spm=5176.2020520001.aliyun_topbar.18.dbd44bd3e4f845#/ticket/createIndex).
         # 
-        # >  If you do not specify a domain name, the custom operations reports are created for all domain names that belong to your Alibaba Cloud account.
+        # > If you do not specify a domain name, the custom operations report is created for all domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name
         # The IDs of the metrics that you want to include in the report. Separate multiple IDs with commas (,). Valid values:
         # 
         # *   **1**: frequently requested URLs (ranked by the number of requests)
         # *   **3**: frequently requested URLs (ranked by the amount of network traffic)
-        # *   **5**: frequently used referer headers (ranked by the number of requests)
-        # *   **7**: frequently used referer headers (ranked by the amount of network traffic)
-        # *   **9**: frequently requested back-to-origin URLs (ranked by the number of requests)
-        # *   **11**: frequently requested back-to-origin URLs (ranked by the amount of network traffic)
+        # *   **5**: frequently used Referer headers (ranked by the number of requests)
+        # *   **7**: frequently used Referer headers (ranked by the amount of network traffic)
+        # *   **9**: frequently requested URLs that are redirected to the origin (ranked by the number of requests)
+        # *   **11**: frequently requested URLs that are redirected to the origin (ranked by the amount of network traffic)
         # *   **13**: top client IP addresses (ranked by the number of requests)
         # *   **15**: top client IP addresses (ranked by the amount of network traffic)
         # *   **17**: domain names ranked by the amount of network traffic
         # *   **19**: page views and unique visitors
         # *   **21**: regions from which requests are initiated
-        # *   **23**: distribution of Internet service providers (ISPs)
+        # *   **23**: Internet service providers (ISPs)
         self.report_ids = report_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2136,40 +2136,40 @@
         end_time: str = None,
         group: str = None,
         language: str = None,
         start_time: str = None,
         task_name: str = None,
         type: str = None,
     ):
-        # The accelerated domain names based on which the resource usage details are generated. If you do not specify a domain name group, resource usage details are exported based on this parameter.
+        # The domain names. If you do not specify the Group parameter, resource usage details of these domain names are exported.
         # 
-        # If you do not set this parameter, resource usage details are exported based on user accounts.
+        # If you do not specify this parameter, resource usage details are exported based on accounts.
         self.domain_names = domain_names
         # The end of the time range to query.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The group of accelerated domain names based on which the resource usage details are generated. If you set this parameter, ignore the **DomainNames** parameter.
+        # The domain name group. If you specify this parameter, the **DomainNames** parameter is ignored.
         self.group = group
-        # The language of the exported file. Valid values:
+        # The language in which you want to export the file. Valid values:
         # 
         # *   **zh-cn**: Chinese. This is the default value.
         # *   **en-us**: English
         self.language = language
         # The beginning of the time range to query.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
         # The name of the task.
         self.task_name = task_name
-        # The type of content based on which the data is generated. Valid values:
+        # The type of resource usage data to query. Valid values:
         # 
-        # *   **flow**: network traffic and bandwidth
+        # *   **flow**: traffic and bandwidth
         # *   **vas**: requests
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -2217,19 +2217,19 @@
     def __init__(
         self,
         end_time: str = None,
         request_id: str = None,
         start_time: str = None,
         task_id: str = None,
     ):
-        # The end of the time range that was queried.
+        # The end of the time range for which the data was queried.
         self.end_time = end_time
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range that was queried.
+        # The beginning of the time range for which the data was queried.
         self.start_time = start_time
         # The ID of the task.
         self.task_id = task_id
 
     def validate(self):
         pass
 
@@ -2312,24 +2312,24 @@
         end_time: str = None,
         language: str = None,
         start_time: str = None,
         task_name: str = None,
     ):
         # The end of the time range to query. The end time must be later than the start time.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.end_time = end_time
-        # The language of the exported file.
+        # The language in which you want to export the file. Default value: zh-cn. Valid values:
         # 
-        # *   **zh-cn**: Chinese. This is the default value.
-        # *   **en-us**: English.
+        # *   **zh-cn**: Chinese
+        # *   **en-us**: English
         self.language = language
-        # The start of the time range to query. The time interval at which the specified data is collected is five minutes.
+        # The start of the time range to query. The data is collected every 5 minutes.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
         # The name of the task.
         self.task_name = task_name
 
     def validate(self):
         pass
 
@@ -2366,19 +2366,19 @@
     def __init__(
         self,
         end_time: str = None,
         request_id: str = None,
         start_time: str = None,
         task_id: str = None,
     ):
-        # The end of the time range where the QPS data was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
         # The ID of the task.
         self.task_id = task_id
 
     def validate(self):
         pass
 
@@ -4418,20 +4418,20 @@
     def __init__(
         self,
         sslpub: str = None,
         sslstatus: bool = None,
     ):
         # The public key of the SSL certificate. You must encode the public key in Base64 and then call the encodeURIComponent function to encode the public key again.
         # 
-        # The public key must be in the PEM format.
+        # The public key must be in the Privacy-Enhanced Mail (PEM) format.
         self.sslpub = sslpub
         # Specifies whether the domain name list to return contains only domain names with HTTPS enabled or disabled.
         # 
-        # - true: The domain name list contains only domain names with HTTPS enabled.
-        # - false: The domain name list contains only domain names with HTTPS disabled.
+        # *   true: The list contains only domain names with HTTPS enabled.
+        # *   false: The list contains only domain names with HTTPS disabled.
         self.sslstatus = sslstatus
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4468,32 +4468,32 @@
         issuer: str = None,
     ):
         # Indicates whether the SSL certificate is obsolete. Valid values:
         # 
         # *   **yes**: The SSL certificate is obsolete.
         # *   **no**: The SSL certificate is working as expected.
         self.cert_ca_is_legacy = cert_ca_is_legacy
-        # The time when the SSL certificate expires.
+        # The time at which the certificate expires.
         self.cert_expire_time = cert_expire_time
         # Indicates whether the SSL certificate is expired. Valid values:
         # 
         # *   **yes**: The SSL certificate is expired.
         # *   **no**: The SSL certificate is not expired.
         self.cert_expired = cert_expired
-        # The time when the SSL certificate became effective.
+        # The time at which the certificate became effective.
         self.cert_start_time = cert_start_time
         # The name of the SSL certificate owner.
         self.cert_subject_common_name = cert_subject_common_name
-        # The type of the certificate. Valid responses: **RSA**, **DSA**, and **ECDSA**.
+        # The type of the certificate. Valid values: **RSA**, **DSA**, and **ECDSA**.
         self.cert_type = cert_type
-        # If a value is returned, the value matches the SSL certificate. Multiple domain names are separated with commas (,).
+        # If a value is returned, the value matches the SSL certificate. Multiple domain names are separated by commas (,).
         self.domain_list = domain_list
-        # The domain names (DNS fields) that match the SSL certificate. Multiple domain names are separated with commas (,).
+        # The domain names (DNS fields) that match the SSL certificate. Multiple domain names are separated by commas (,).
         self.domain_names = domain_names
-        # The certificate authority that issued the SSL certificate.
+        # The certificate authority (CA) that issued the certificate.
         self.issuer = issuer
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4581,15 +4581,15 @@
 
 class DescribeCdnDomainByCertificateResponseBody(TeaModel):
     def __init__(
         self,
         cert_infos: DescribeCdnDomainByCertificateResponseBodyCertInfos = None,
         request_id: str = None,
     ):
-        # The information about the SSL certificate.
+        # The certificate information.
         self.cert_infos = cert_infos
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.cert_infos:
             self.cert_infos.validate()
@@ -5315,29 +5315,29 @@
         self,
         domain_name: str = None,
         end_time: str = None,
         page_number: int = None,
         page_size: int = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. You can specify only one domain name.
+        # The domain name. You can specify only one domain name.
         self.domain_name = domain_name
         # The end of the time range to query.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
         # The number of the page to return. Pages start from page **1**.
         self.page_number = page_number
         # The number of entries to return on each page. Default value: **300**. Maximum value: **1000**. Valid values: **1** to **1000**.
         self.page_size = page_size
         # The beginning of the time range to query.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5377,23 +5377,23 @@
         self,
         end_time: str = None,
         log_name: str = None,
         log_path: str = None,
         log_size: int = None,
         start_time: str = None,
     ):
-        # The end of the time range where the QPS data was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
         # The name of the log file.
         self.log_name = log_name
         # The path of the log file.
         self.log_path = log_path
         # The size of the log file.
         self.log_size = log_size
-        # The start of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5513,17 +5513,17 @@
         log_infos: DescribeCdnDomainLogsResponseBodyDomainLogDetailsDomainLogDetailLogInfos = None,
         page_infos: DescribeCdnDomainLogsResponseBodyDomainLogDetailsDomainLogDetailPageInfos = None,
     ):
         # The accelerated domain name.
         self.domain_name = domain_name
         # The total number of entries returned on the current page.
         self.log_count = log_count
-        # The detailed log information, which is indicated by the LogInfoDetail parameter.
+        # A set of LogInfoDetail data.
         self.log_infos = log_infos
-        # The detailed log information, which is indicated by the PageInfoDetail parameter.
+        # A set of PageInfoDetail data.
         self.page_infos = page_infos
 
     def validate(self):
         if self.log_infos:
             self.log_infos.validate()
         if self.page_infos:
             self.page_infos.validate()
@@ -5596,15 +5596,15 @@
 
 class DescribeCdnDomainLogsResponseBody(TeaModel):
     def __init__(
         self,
         domain_log_details: DescribeCdnDomainLogsResponseBodyDomainLogDetails = None,
         request_id: str = None,
     ):
-        # The detailed log information, which is indicated by the DomainLogDetail parameter.
+        # A set of DomainLogDetail data.
         self.domain_log_details = domain_log_details
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.domain_log_details:
             self.domain_log_details.validate()
@@ -5913,19 +5913,19 @@
 class DescribeCdnHttpsDomainListRequest(TeaModel):
     def __init__(
         self,
         keyword: str = None,
         page_number: int = None,
         page_size: int = None,
     ):
-        # The keyword used for search.
+        # The keyword that is used to search for certificates.
         self.keyword = keyword
         # The number of the page to return. Valid values: **1** to **100000**.
         self.page_number = page_number
-        # The maximum number of entries to return on each page. Default value: **20**.
+        # The number of entries to return on each page. Default value: **20**.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5960,36 +5960,36 @@
         cert_name: str = None,
         cert_start_time: str = None,
         cert_status: str = None,
         cert_type: str = None,
         cert_update_time: str = None,
         domain_name: str = None,
     ):
-        # The Common Name on the SSL certificate.
+        # The returned primary domain name of the certificate.
         self.cert_common_name = cert_common_name
-        # The time when the SSL certificate expires.
+        # The time at which the certificate expires.
         self.cert_expire_time = cert_expire_time
-        # The name of the SSL certificate.
+        # The name of the certificate.
         self.cert_name = cert_name
-        # The time when the SSL certificate became effective.
+        # The time at which the certificate became effective.
         self.cert_start_time = cert_start_time
-        # The status of the SSL certificate. Valid values:
+        # The status of the certificate.
         # 
-        # *   **ok**: The SSL certificate is working as expected.
-        # *   **mismatch**: The SSL certificate does not match the specified domain name.
-        # *   **expired**: The SSL certificate has expired.
-        # *   **expire_soon**: The SSL certificate will expire soon.
+        # *   **ok**: The certificate is working as expected.
+        # *   **mismatch**: The certificate does not match the specified domain name.
+        # *   **expired**: The certificate has expired.
+        # *   **expire_soon**: The certificate will expire soon.
         self.cert_status = cert_status
-        # The type of the SSL certificate. Valid values:
+        # The type of the certificate.
         # 
-        # *   **free**: a free SSL certificate.
-        # *   **cas**: an SSL certificate purchased from Alibaba Cloud SSL Certificates Service.
-        # *   **upload**: a user uploaded certificate.
+        # *   **free**: a free certificate.
+        # *   **cas**: a certificate that is purchased from Alibaba Cloud SSL Certificates Service.
+        # *   **upload**: a certificate that is uploaded by the user.
         self.cert_type = cert_type
-        # The time when the certificate was renewed.
+        # The time at which the certificate was updated.
         self.cert_update_time = cert_update_time
         # The accelerated domain name.
         self.domain_name = domain_name
 
     def validate(self):
         pass
 
@@ -6076,15 +6076,15 @@
 class DescribeCdnHttpsDomainListResponseBody(TeaModel):
     def __init__(
         self,
         cert_infos: DescribeCdnHttpsDomainListResponseBodyCertInfos = None,
         request_id: str = None,
         total_count: int = None,
     ):
-        # The information about the SSL certificate.
+        # The information about the certificate.
         self.cert_infos = cert_infos
         # The ID of the request.
         self.request_id = request_id
         # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
@@ -7522,21 +7522,21 @@
 
 class DescribeCdnUserBillHistoryRequest(TeaModel):
     def __init__(
         self,
         end_time: str = None,
         start_time: str = None,
     ):
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # The end of the time range to query. The end time must be later than the start time.
+        # The end time must be later than the start time.
         self.end_time = end_time
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # The minimum data collection interval is 5 minutes.
+        # The minimum data granularity is 5 minutes.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7568,25 +7568,25 @@
         count: float = None,
         flow: float = None,
     ):
         # The bandwidth. Unit: bit/s.
         self.bandwidth = bandwidth
         # The billable region. Valid values:
         # 
-        # *   **CN**: mainland China
-        # *   **OverSeas**: regions outside mainland China
+        # *   **CN**: Chinese mainland
+        # *   **OverSeas**: outside the Chinese mainland
         # *   **AP1**: Asia Pacific 1
         # *   **AP2**: Asia Pacific 2
         # *   **AP3**: Asia Pacific 3
         # *   **NA**: North America
         # *   **SA**: South America
         # *   **EU**: Europe
         # *   **MEAA**: Middle East and Africa
         self.cdn_region = cdn_region
-        # The billable item. Valid values:
+        # The billing method. Valid values:
         # 
         # *   **StaticHttp**: static HTTP requests
         # *   **DynamicHttp**: dynamic HTTP requests
         # *   **DynamicHttps**: dynamic HTTPS requests
         self.charge_type = charge_type
         # The number of requests.
         self.count = count
@@ -7670,15 +7670,15 @@
         bill_time: str = None,
         bill_type: str = None,
         billing_data: DescribeCdnUserBillHistoryResponseBodyBillHistoryDataBillHistoryDataItemBillingData = None,
         dimension: str = None,
     ):
         # The beginning of the time range that was queried.
         self.bill_time = bill_time
-        # The billing method.
+        # The metering method.
         self.bill_type = bill_type
         # The billable items.
         self.billing_data = billing_data
         # The dimension.
         self.dimension = dimension
 
     def validate(self):
@@ -8091,25 +8091,21 @@
 
 class DescribeCdnUserBillTypeRequest(TeaModel):
     def __init__(
         self,
         end_time: str = None,
         start_time: str = None,
     ):
-        # The end of the time range that was queried.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # Example: 2016-10-20T04:00:00Z.
+        # The end time must be later than the start time.
         self.end_time = end_time
-        # The start of the time range that was queried.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # Example: 2016-10-20T04:00:00Z.
+        # The minimum data granularity is 5 minutes.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8138,19 +8134,49 @@
         bill_type: str = None,
         billing_cycle: str = None,
         dimension: str = None,
         end_time: str = None,
         product: str = None,
         start_time: str = None,
     ):
+        # The metering method.
+        # 
+        # > If the metering method is suffixed with \*\*\_overseas\*\*, the billable region is outside the Chinese mainland. For example, "BillType": "month_avg_day_bandwidth_overseas" indicates that the metering method is pay by average daily peak bandwidth per month in a billable region outside the Chinese mainland.
+        # 
+        # Valid values:
+        # 
+        # *   hour_flow: pay by hourly data transfer
+        # *   day_bandwidth: pay by daily bandwidth
+        # *   month\_95: pay by monthly 95th percentile bandwidth
+        # *   month_avg_day_bandwidth: pay by average daily peak bandwidth per month
+        # *   month\_4th_day_bandwidth: pay by monthly 4th peak bandwidth
+        # *   month_avg_day\_95: pay by average daily 95th percentile bandwidth per month
+        # *   month\_95\_night_half: pay by 95th percentile bandwidth with 50% off from 00:00 to 08:00
+        # *   hour_vas: pay by value-added services per hour
+        # *   quic_hour_count: pay by hourly QUIC requests
+        # *   day_count: pay by daily requests
+        # *   hour_count: pay by hourly requests
+        # *   day\_95: pay by daily 95th percentile bandwidth
         self.bill_type = bill_type
+        # The billing cycle.
         self.billing_cycle = billing_cycle
+        # The dimension. Valid values:
+        # 
+        # *   flow: traffic and bandwidth
+        # *   vas: value-added services (HTTPS and requests for dynamic content)
+        # *   quic: the number of QUIC requests
+        # *   websocket: the WebSocket communications protocol
+        # *   rtlog2sls: log entries delivered to Log Service in real time
+        # *   stationflow: traffic over the internal network
         self.dimension = dimension
+        # The time when the metering method ended.
         self.end_time = end_time
+        # The name of the product.
         self.product = product
+        # The time when the metering method started.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8226,14 +8252,15 @@
 
 class DescribeCdnUserBillTypeResponseBody(TeaModel):
     def __init__(
         self,
         bill_type_data: DescribeCdnUserBillTypeResponseBodyBillTypeData = None,
         request_id: str = None,
     ):
+        # Details about the metering methods returned.
         self.bill_type_data = bill_type_data
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.bill_type_data:
             self.bill_type_data.validate()
@@ -9490,15 +9517,15 @@
 
 
 class DescribeCertificateInfoByIDRequest(TeaModel):
     def __init__(
         self,
         cert_id: str = None,
     ):
-        # The ID of the SSL certificate. You can query only one certificate in each call.
+        # The ID of the certificate. You can query only one certificate in each call.
         self.cert_id = cert_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9524,29 +9551,29 @@
         cert_id: str = None,
         cert_name: str = None,
         cert_type: str = None,
         create_time: str = None,
         domain_list: str = None,
         https_crt: str = None,
     ):
-        # The expiration time of the certificate.
+        # The time at which the certificate expires.
         self.cert_expire_time = cert_expire_time
         # The ID of the certificate.
         self.cert_id = cert_id
         # The name of the certificate.
         self.cert_name = cert_name
         # The type of the certificate.
         # 
-        # *   free: a free certificate.
-        # *   cas: a certificate purchased by using Certificate Management Service.
-        # *   upload: a user-uploaded certificate.
+        # *   free: a free certificate
+        # *   cas: a certificate purchased by using Certificate Management Service
+        # *   upload: a user-uploaded certificate
         self.cert_type = cert_type
         # The time when the certificate became effective.
         self.create_time = create_time
-        # A list of domain names that use the certificate.
+        # The domain names that use the certificate.
         self.domain_list = domain_list
         # The content of the certificate.
         self.https_crt = https_crt
 
     def validate(self):
         pass
 
@@ -10098,35 +10125,35 @@
         domain_name: str = None,
         end_time: str = None,
         interval: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.  
+        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # By default, this operation queries the bandwidth values during back-to-origin routing for all accelerated domain names that belong to your Alibaba Cloud account.
+        # By default, this operation queries bandwidth data for all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.  
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The time interval between the data entries. Unit: seconds. 
+        # The time granularity of the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval
-        # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service. You can call the [DescribeCdnRegionAndIsp](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/describecdnregionandisp) operation to query ISP names.  
+        # The name of the Internet service provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
         # 
-        # If you do not set this parameter, all ISPs are queried.
+        # If you do not set this parameter, data of all ISPs is queried.
         self.isp_name_en = isp_name_en
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/describecdnregionandisp) operation to query the most recent region list.  
+        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
         # 
-        # If you do not set this parameter, the bandwidth monitoring data of the accelerated domain names in all regions is returned.
+        # If you do not specify a region, data in all regions is queried.
         self.location_name_en = location_name_en
-        # The start of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10172,27 +10199,27 @@
         https_domestic_value: str = None,
         https_overseas_value: str = None,
         https_value: str = None,
         overseas_value: str = None,
         time_stamp: str = None,
         value: str = None,
     ):
-        # The bandwidth values in the Chinese mainland. When the bandwidth data is queried by ISP, no value is returned.
+        # The bandwidth value in the Chinese mainland. When the bandwidth data is queried by ISP, this parameter is empty.
         self.domestic_value = domestic_value
-        # The bandwidth values for HTTPS requests in the Chinese mainland. When the bandwidth data is queried by ISP, no value is returned.
+        # The bandwidth data for HTTPS requests in the Chinese mainland. When the bandwidth data is queried by ISP, this parameter is empty.
         self.https_domestic_value = https_domestic_value
-        # The bandwidth values for HTTPS requests in regions outside the Chinese mainland. When the bandwidth data is queried by ISP, no value is returned.
+        # The bandwidth data for HTTPS requests in regions outside the Chinese mainland. When the bandwidth data is queried by ISP, this parameter is empty.
         self.https_overseas_value = https_overseas_value
-        # The bandwidth values for HTTPS requests. Unit: bit/s.
+        # The bandwidth value for HTTPS requests. Unit: bit/s.
         self.https_value = https_value
-        # The bandwidth values in regions outside the Chinese mainland. When the bandwidth data is queried by ISP, no value is returned.
+        # The bandwidth data in regions outside the Chinese mainland. When the bandwidth data is queried by ISP, this parameter is empty.
         self.overseas_value = overseas_value
         # The timestamp of the data returned.
         self.time_stamp = time_stamp
-        # The bandwidth value. Unit: bit/s.
+        # The bandwidth. Unit: bit/s.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10278,29 +10305,29 @@
         domain_name: str = None,
         end_time: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         request_id: str = None,
         start_time: str = None,
     ):
-        # The bandwidth values collected at each interval.
+        # The list of bandwidth data entries returned at each interval.
         self.bps_data_per_interval = bps_data_per_interval
-        # The time interval between the returned entries. Unit: seconds.
+        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
-        # The name of the ISP for your Alibaba Cloud CDN service.
+        # The name of the ISP.
         self.isp_name_en = isp_name_en
         # The name of the region.
         self.location_name_en = location_name_en
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.bps_data_per_interval:
             self.bps_data_per_interval.validate()
 
     def to_map(self):
@@ -10400,39 +10427,39 @@
         end_time: str = None,
         interval: str = None,
         isp_name_en: str = None,
         layer: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # >  If you do not specify an accelerated domain name, the bandwidth data of all the accelerated domain names that belong to your Alibaba Cloud account is queried.
+        # > If you do not specify this parameter, the bandwidth data about all accelerated domain names that belong to your Alibaba Cloud account is queried.
         self.domain_name = domain_name
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The time interval between the data entries. Unit: seconds.
+        # The time granularity of the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval
-        # The name of the Internet service provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent ISP list. If you do not specify an ISP, data of all ISPs is queried.
+        # The name of the Internet service provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~DescribeCdnRegionAndIsp~~) operation to query ISPs. If you do not specify an ISP, data of all ISPs is queried.
         self.isp_name_en = isp_name_en
-        # The layers at which you want to query the bandwidth data. Valid values:
+        # The layer at which you want to query the bandwidth data. Valid values:
         # 
         # *   Network layer: **IPv4** and **IPv6**.
         # *   Application layer: **http**, **https**, and **quic**.
         # *   **all**: specifies that both the network and application layers are included.
         # 
         # Default value: **all**.
         self.layer = layer
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list. If you do not specify a region, data in all regions is queried.
+        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~DescribeCdnRegionAndIsp~~) operation to query regions. If you do not specify a region, data in all regions is queried.
         self.location_name_en = location_name_en
         # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
@@ -10482,15 +10509,15 @@
 class DescribeDomainBpsDataByLayerResponseBodyBpsDataIntervalDataModule(TeaModel):
     def __init__(
         self,
         time_stamp: str = None,
         traffic_value: str = None,
         value: str = None,
     ):
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp
         # The total amount of network traffic. Unit: bytes.
         self.traffic_value = traffic_value
         # The peak bandwidth value. Unit: bit/s.
         self.value = value
 
     def validate(self):
@@ -10559,15 +10586,15 @@
 class DescribeDomainBpsDataByLayerResponseBody(TeaModel):
     def __init__(
         self,
         bps_data_interval: DescribeDomainBpsDataByLayerResponseBodyBpsDataInterval = None,
         data_interval: str = None,
         request_id: str = None,
     ):
-        # The number of bytes per second collected at each time interval.
+        # The data returned at each time interval.
         self.bps_data_interval = bps_data_interval
         # The time interval between the data entries. Unit: seconds.
         self.data_interval = data_interval
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
@@ -10648,27 +10675,27 @@
     def __init__(
         self,
         domain_name: str = None,
         isp_names: str = None,
         location_names: str = None,
         time_point: str = None,
     ):
-        # The accelerated domain name. You can specify only one domain name in each query.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name
-        # The names of the Internet service providers (ISPs). Separate multiple ISP names with commas (,).
+        # The names of the Internet service providers (ISPs). Separate multiple ISPs with commas (,).
         # 
         # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
         self.isp_names = isp_names
-        # The names of the regions. Separate multiple regions with commas (,).
+        # The regions. Separate multiple regions with commas (,).
         # 
         # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
         self.location_names = location_names
-        # The beginning of the time range that was queried. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The point in time to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # The data is collected at an interval of five minutes.
+        # > The data is collected every 5 minutes.
         self.time_point = time_point
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10705,19 +10732,19 @@
         bps: int = None,
         isp_name: str = None,
         location_name: str = None,
         time_stamp: str = None,
     ):
         # The bandwidth value.
         self.bps = bps
-        # The name of the ISP for your Content Delivery Network (CDN) service.
+        # The name of the ISP.
         self.isp_name = isp_name
         # The name of the region.
         self.location_name = location_name
-        # The timestamp of the data.
+        # The timestamp of the data returned.
         self.time_stamp = time_stamp
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10787,21 +10814,21 @@
     def __init__(
         self,
         bps_data_list: DescribeDomainBpsDataByTimeStampResponseBodyBpsDataList = None,
         domain_name: str = None,
         request_id: str = None,
         time_stamp: str = None,
     ):
-        # A list of bandwidth values queried by ISP and region.
+        # A list of bandwidth values by ISP and region.
         self.bps_data_list = bps_data_list
         # The accelerated domain name.
         self.domain_name = domain_name
         # The ID of the request.
         self.request_id = request_id
-        # The timestamp of the data.
+        # The point in time.
         self.time_stamp = time_stamp
 
     def validate(self):
         if self.bps_data_list:
             self.bps_data_list.validate()
 
     def to_map(self):
@@ -11446,14 +11473,15 @@
 
 
 class DescribeDomainCnameRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
     ):
+        # The accelerated domain name that you want to query. Separate multiple domain names with commas (,). This parameter cannot be left empty.
         self.domain_name = domain_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11475,16 +11503,22 @@
 class DescribeDomainCnameResponseBodyCnameDatasData(TeaModel):
     def __init__(
         self,
         cname: str = None,
         domain: str = None,
         status: int = None,
     ):
+        # The CNAME assigned to the domain name by Alibaba Cloud CDN.
         self.cname = cname
+        # The accelerated domain name.
         self.domain = domain
+        # The CNAME detection result. Valid values:
+        # 
+        # *   0: The DNS can detect the CNAME assigned to the domain name.
+        # *   Value other than 0: The DNS cannot detect the CNAME assigned to the domain name.
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11548,15 +11582,17 @@
 
 class DescribeDomainCnameResponseBody(TeaModel):
     def __init__(
         self,
         cname_datas: DescribeDomainCnameResponseBodyCnameDatas = None,
         request_id: str = None,
     ):
+        # Details about the CNAME detection results.
         self.cname_datas = cname_datas
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.cname_datas:
             self.cname_datas.validate()
 
     def to_map(self):
@@ -12049,29 +12085,29 @@
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         interval: str = None,
         start_time: str = None,
     ):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # By default, this operation queries the byte hit ratios of all accelerated domain names that belong to your Alibaba Cloud account.
+        # By default, this operation queries the byte hit ratios for all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The time interval between the data entries. Unit: seconds.
+        # The time granularity of the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval
-        # The start of the time range to query.
+        # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
@@ -12191,21 +12227,21 @@
         request_id: str = None,
         start_time: str = None,
     ):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
         # The byte hit ratio at each time interval. The byte hit ratio is measured in percentage.
         self.hit_rate_interval = hit_rate_interval
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.hit_rate_interval:
             self.hit_rate_interval.validate()
 
     def to_map(self):
@@ -12626,35 +12662,35 @@
         end_time: str = None,
         interval: str = None,
         isp_name_en: str = None,
         layer: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name. You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # If you do not specify a domain name, data of all domain names is queried.
+        # If you do not specify this parameter, data of all accelerated domain names under your account is queried.
         self.domain_name = domain_name
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The time interval between the data entries. Unit: seconds.
+        # The time granularity of the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval
-        # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
+        # The name of the Internet service provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
         # 
         # If you do not specify an ISP, data of all ISPs is queried.
         self.isp_name_en = isp_name_en
         # The protocol by which you want to query HTTP status codes. The network layer supports **IPv4** and **IPv6**. The application layer supports **http**, **https**, and **quic**. You can also set the value to **all**.
         # 
-        # The default value is **all**.
+        # Default value: **all**\
         self.layer = layer
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list.
+        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
         # 
         # If you do not specify a region, data in all regions is queried.
         self.location_name_en = location_name_en
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
@@ -12706,15 +12742,15 @@
         self,
         time_stamp: str = None,
         total_value: str = None,
         value: str = None,
     ):
         # The timestamp of the data returned.
         self.time_stamp = time_stamp
-        # The total number of times that HTTP status codes were returned at each time interval.
+        # The total number of times that HTTP status codes were returned.
         self.total_value = total_value
         # The number of times that the HTTP status code was returned.
         self.value = value
 
     def validate(self):
         pass
 
@@ -12783,15 +12819,15 @@
         self,
         data_interval: str = None,
         http_code_data_interval: DescribeDomainHttpCodeDataByLayerResponseBodyHttpCodeDataInterval = None,
         request_id: str = None,
     ):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
-        # The number of HTTP status codes returned at each time interval.
+        # The statistics of HTTP status codes returned at each time interval.
         self.http_code_data_interval = http_code_data_interval
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.http_code_data_interval:
             self.http_code_data_interval.validate()
@@ -13166,18 +13202,36 @@
         self,
         cycle: str = None,
         domain_name: str = None,
         end_time: str = None,
         start_time: str = None,
         time_point: str = None,
     ):
+        # The cycle to query the 95th percentile bandwidth data. Default value: **day**. Valid values:
+        # 
+        # *   **day**: queries the 95th percentile bandwidth data by day.
+        # *   **month**: queries the 95th percentile bandwidth data by month.
         self.cycle = cycle
+        # The accelerated domain name. If you do not specify this parameter, data of all accelerated domain names under your account is queried.
+        # 
+        # > You cannot specify multiple domain names at a time.
         self.domain_name = domain_name
+        # The end of the time range to query.
+        # 
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # > The end time must be later than the start time.
         self.end_time = end_time
+        # The beginning of the time range to query.
+        # 
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
+        # The beginning of the time range to query.
+        # 
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.time_point = time_point
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13208,44 +13262,134 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         if m.get('TimePoint') is not None:
             self.time_point = m.get('TimePoint')
         return self
 
 
+class DescribeDomainMax95BpsDataResponseBodyDetailDataMax95Detail(TeaModel):
+    def __init__(
+        self,
+        area: str = None,
+        max_95bps: float = None,
+        max_95bps_peak_time: str = None,
+        time_stamp: str = None,
+    ):
+        self.area = area
+        self.max_95bps = max_95bps
+        self.max_95bps_peak_time = max_95bps_peak_time
+        self.time_stamp = time_stamp
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
+        if self.area is not None:
+            result['Area'] = self.area
+        if self.max_95bps is not None:
+            result['Max95Bps'] = self.max_95bps
+        if self.max_95bps_peak_time is not None:
+            result['Max95BpsPeakTime'] = self.max_95bps_peak_time
+        if self.time_stamp is not None:
+            result['TimeStamp'] = self.time_stamp
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Area') is not None:
+            self.area = m.get('Area')
+        if m.get('Max95Bps') is not None:
+            self.max_95bps = m.get('Max95Bps')
+        if m.get('Max95BpsPeakTime') is not None:
+            self.max_95bps_peak_time = m.get('Max95BpsPeakTime')
+        if m.get('TimeStamp') is not None:
+            self.time_stamp = m.get('TimeStamp')
+        return self
+
+
+class DescribeDomainMax95BpsDataResponseBodyDetailData(TeaModel):
+    def __init__(
+        self,
+        max_95detail: List[DescribeDomainMax95BpsDataResponseBodyDetailDataMax95Detail] = None,
+    ):
+        self.max_95detail = max_95detail
+
+    def validate(self):
+        if self.max_95detail:
+            for k in self.max_95detail:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Max95Detail'] = []
+        if self.max_95detail is not None:
+            for k in self.max_95detail:
+                result['Max95Detail'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.max_95detail = []
+        if m.get('Max95Detail') is not None:
+            for k in m.get('Max95Detail'):
+                temp_model = DescribeDomainMax95BpsDataResponseBodyDetailDataMax95Detail()
+                self.max_95detail.append(temp_model.from_map(k))
+        return self
+
+
 class DescribeDomainMax95BpsDataResponseBody(TeaModel):
     def __init__(
         self,
+        detail_data: DescribeDomainMax95BpsDataResponseBodyDetailData = None,
         domain_name: str = None,
         domestic_max_95bps: str = None,
         end_time: str = None,
         max_95bps: str = None,
         overseas_max_95bps: str = None,
         request_id: str = None,
         start_time: str = None,
     ):
+        self.detail_data = detail_data
         # The accelerated domain name.
         self.domain_name = domain_name
+        # The 95th percentile bandwidth in the Chinese mainland.
         self.domestic_max_95bps = domestic_max_95bps
+        # The end of the time range for which the data was queried.
         self.end_time = end_time
+        # The 95th percentile bandwidth.
         self.max_95bps = max_95bps
+        # The 95th percentile bandwidth outside the Chinese mainland.
         self.overseas_max_95bps = overseas_max_95bps
         # The ID of the request.
         self.request_id = request_id
+        # The beginning of the time range for which the data was queried.
         self.start_time = start_time
 
     def validate(self):
-        pass
+        if self.detail_data:
+            self.detail_data.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.detail_data is not None:
+            result['DetailData'] = self.detail_data.to_map()
         if self.domain_name is not None:
             result['DomainName'] = self.domain_name
         if self.domestic_max_95bps is not None:
             result['DomesticMax95Bps'] = self.domestic_max_95bps
         if self.end_time is not None:
             result['EndTime'] = self.end_time
         if self.max_95bps is not None:
@@ -13256,14 +13400,17 @@
             result['RequestId'] = self.request_id
         if self.start_time is not None:
             result['StartTime'] = self.start_time
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('DetailData') is not None:
+            temp_model = DescribeDomainMax95BpsDataResponseBodyDetailData()
+            self.detail_data = temp_model.from_map(m['DetailData'])
         if m.get('DomainName') is not None:
             self.domain_name = m.get('DomainName')
         if m.get('DomesticMax95Bps') is not None:
             self.domestic_max_95bps = m.get('DomesticMax95Bps')
         if m.get('EndTime') is not None:
             self.end_time = m.get('EndTime')
         if m.get('Max95Bps') is not None:
@@ -13664,31 +13811,27 @@
         page_number: int = None,
         page_size: int = None,
         path: str = None,
         start_time: str = None,
     ):
         # The accelerated domain name.
         # 
-        # >  You can specify only one domain name in each call.
+        # > You can specify only one domain name in each call.
         self.domain_name = domain_name
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC. The interval between the start time and end time must be less than 30 days. Example: 2016-10-21T04:00:00Z.
         self.end_time = end_time
         # The number of the page to return. Pages start from page **1**.
         self.page_number = page_number
-        # The number of entries to return on each page.
-        # 
-        # Valid values: integers from **1** to **1000**.
+        # The number of entries to return on each page. Valid values: integers from **1** to **1000**.
         self.page_size = page_size
         # The paths that you want to query. Separate paths with forward slashes (/). If you do not set this parameter, all paths are queried. If you set the value to a directory, it must end with a forward slash (/).
         # 
-        # >  Fuzzy match is not supported. If you want data to be collected based on a directory, you can specify a specific directory, for example, directory/path/. In this case, bandwidth data is collected based on directory/path/.
+        # > Fuzzy match is not supported. If you want data to be collected based on a directory, you can specify a specific directory, for example, directory/path/. In this case, bandwidth data is collected based on directory/path/.
         self.path = path
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # Example: 2016-10-20T04:00:00Z.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC. Example: 2016-10-20T04:00:00Z.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13731,15 +13874,15 @@
     def __init__(
         self,
         acc: int = None,
         path: str = None,
         time: str = None,
         traffic: int = None,
     ):
-        # The number of visits to the specified path.
+        # The number of visits to the URL.
         self.acc = acc
         # The path.
         self.path = path
         # The point in time.
         self.time = time
         # The amount of network traffic. Unit: bytes.
         self.traffic = traffic
@@ -13819,29 +13962,29 @@
         end_time: str = None,
         page_number: int = None,
         page_size: int = None,
         path_data_per_interval: DescribeDomainPathDataResponseBodyPathDataPerInterval = None,
         start_time: str = None,
         total_count: int = None,
     ):
-        # The time interval between the data entries. Unit: seconds.
+        # The time interval. Unit: seconds.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
         # The page number of the returned page. Pages start from page **1**.
         self.page_number = page_number
-        # The number of entries returned on each page.
+        # The number of entries returned per page.
         self.page_size = page_size
         # A list of bandwidth values collected at each time interval.
         self.path_data_per_interval = path_data_per_interval
-        # The start of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
-        # The total count.
+        # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.path_data_per_interval:
             self.path_data_per_interval.validate()
 
     def to_map(self):
@@ -14163,29 +14306,29 @@
         domain_name: str = None,
         end_time: str = None,
         interval: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # By default, this operation queries the number of queries per second for all accelerated domain names that belong to your Alibaba Cloud account.
+        # By default, this operation queries QPS data for all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
         # The end time must be later than the start time.
         self.end_time = end_time
-        # The time interval between the data entries. Unit: seconds.
+        # The time granularity of the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval
-        # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs. If you do not set this parameter, all ISPs are queried.
+        # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs. If you do not specify an ISP, data of all ISPs is queried.
         self.isp_name_en = isp_name_en
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list. If you do not set this parameter, all regions are queried.
+        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions. If you do not specify a region, data in all regions is queried.
         self.location_name_en = location_name_en
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
@@ -14247,31 +14390,31 @@
         self.acc_domestic_value = acc_domestic_value
         # The number of requests outside the Chinese mainland.
         self.acc_overseas_value = acc_overseas_value
         # The total number of requests.
         self.acc_value = acc_value
         # The number of queries per second in the Chinese mainland.
         self.domestic_value = domestic_value
-        # The number of HTTPS requests sent to L1 edge nodes in the Chinese mainland.
+        # The number of HTTPS requests sent to POPs in the Chinese mainland.
         self.https_acc_domestic_value = https_acc_domestic_value
-        # The number of HTTPS requests sent to L1 edge nodes outside the Chinese mainland.
+        # The number of HTTPS requests sent to POPs outside the Chinese mainland.
         self.https_acc_overseas_value = https_acc_overseas_value
-        # The total number of HTTPS requests sent to L1 edge nodes.
+        # The number of HTTPS requests sent to POPs.
         self.https_acc_value = https_acc_value
-        # The number of queries per second that is calculated based on the HTTPS requests sent to L1 edge nodes in the Chinese mainland.
+        # The number of queries per second that is calculated based on the HTTPS requests sent to POPs in the Chinese mainland.
         self.https_domestic_value = https_domestic_value
-        # The number of queries per second that is calculated based on the HTTPS requests sent to L1 edge nodes outside the Chinese mainland.
+        # The number of queries per second that is calculated based on the HTTPS requests sent to POPs outside the Chinese mainland.
         self.https_overseas_value = https_overseas_value
-        # The number of queries per second that is calculated based on the HTTPS requests sent to L1 edge nodes.
+        # The number of queries per second that is calculated based on the HTTPS requests sent to points of presence (POPs).
         self.https_value = https_value
         # The number of queries per second outside the Chinese mainland.
         self.overseas_value = overseas_value
         # The timestamp of the data returned.
         self.time_stamp = time_stamp
-        # The total number of queries per second.
+        # The total QPS.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14383,21 +14526,21 @@
         request_id: str = None,
         start_time: str = None,
     ):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
-        # The number of queries per second at each time interval.
+        # The list of QPS records at each interval.
         self.qps_data_interval = qps_data_interval
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.qps_data_interval:
             self.qps_data_interval.validate()
 
     def to_map(self):
@@ -14489,37 +14632,37 @@
         end_time: str = None,
         interval: str = None,
         isp_name_en: str = None,
         layer: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify a maximum of 500 domain names in a request. Separate multiple domain names with commas (,).
         # 
-        # By default, this operation queries the number of queries per second for all accelerated domain names that belong to your Alibaba Cloud account.
+        # By default, this operation queries the QPS of all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The end of the time range to query. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format in the ISO 8601 standard. The time is displayed in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The time interval between the data entries. Unit: seconds.
+        # The time interval between the data entries to return. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Description**.
         self.interval = interval
         # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs. If you do not set this parameter, all ISPs are queried.
         self.isp_name_en = isp_name_en
         # The layers at which you want to query the number of queries per second. Valid values:
         # 
         # *   **Network layer**: **IPv4**and **IPv6**.
         # *   **Application layer**: **http**, **https**, and **quic**.
         # *   **all**: The default value. Both the network and application layers are included.
         self.layer = layer
         # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list. If you do not set this parameter, all regions are queried.
         self.location_name_en = location_name_en
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format in the ISO 8601 standard. The time is displayed in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14571,25 +14714,25 @@
         domestic_value: str = None,
         overseas_value: str = None,
         time_stamp: str = None,
         value: str = None,
     ):
         # The number of requests in the Chinese mainland.
         self.acc_domestic_value = acc_domestic_value
-        # The number of requests in the Chinese mainland.
+        # The number of requests outside the Chinese mainland.
         self.acc_overseas_value = acc_overseas_value
         # The total number of requests.
         self.acc_value = acc_value
         # The number of queries per second in the Chinese mainland.
         self.domestic_value = domestic_value
         # The number of queries per second outside the Chinese mainland.
         self.overseas_value = overseas_value
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp
-        # The total number of queries per second in all regions.
+        # The total number of queries per second.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14678,23 +14821,23 @@
         request_id: str = None,
         start_time: str = None,
     ):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
         # The layer at which the data was collected.
         self.layer = layer
-        # The number of queries per second at each time interval.
+        # The number of queries per second at each interval.
         self.qps_data_interval = qps_data_interval
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.qps_data_interval:
             self.qps_data_interval.validate()
 
     def to_map(self):
@@ -14788,31 +14931,31 @@
         self,
         domain_name: str = None,
         end_time: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain names. You can specify multiple accelerated domain names and separate them with commas (,).
+        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
         # 
-        # >  You can specify at most 500 accelerated domain names in each call.
+        # > You can specify up to 500 domain names in each request.
         self.domain_name = domain_name
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service.
+        # The name of the Internet service provider (ISP).
         # 
-        # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent ISP list. If you do not set this parameter, all ISPs are queried.
+        # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs. If you do not set this parameter, all ISPs are queried.
         self.isp_name_en = isp_name_en
         # The name of the region.
         # 
-        # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list. If you do not set this parameter, all regions are queried.
+        # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions. If you do not set this parameter, all regions are queried.
         self.location_name_en = location_name_en
         # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
@@ -14855,15 +14998,15 @@
     def __init__(
         self,
         bps: float = None,
         time_stamp: str = None,
     ):
         # The bandwidth. Unit: bit/s.
         self.bps = bps
-        # The timestamp of the data entry. The time follows the ISO 8601 standard. The time is displayed in UTC.
+        # The timestamp of the data returned. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         self.time_stamp = time_stamp
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14923,15 +15066,15 @@
 
 class DescribeDomainRealTimeBpsDataResponseBody(TeaModel):
     def __init__(
         self,
         data: DescribeDomainRealTimeBpsDataResponseBodyData = None,
         request_id: str = None,
     ):
-        # The response parameters.
+        # The data returned.
         self.data = data
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.data:
             self.data.validate()
@@ -15005,21 +15148,25 @@
 class DescribeDomainRealTimeByteHitRateDataRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         start_time: str = None,
     ):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 100 domain names in each call.
+        # The accelerated domain name. You can specify up to 100 domain names in each call. Separate multiple domain names with commas (,).
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.  
+        # The end of the time range to query.
         # 
-        # >  The end time must be later than the start time.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query.
+        # 
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15118,15 +15265,15 @@
 
 class DescribeDomainRealTimeByteHitRateDataResponseBody(TeaModel):
     def __init__(
         self,
         data: DescribeDomainRealTimeByteHitRateDataResponseBodyData = None,
         request_id: str = None,
     ):
-        # The response parameters.
+        # The data returned.
         self.data = data
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.data:
             self.data.validate()
@@ -15378,27 +15525,27 @@
         self,
         domain_name: str = None,
         end_time: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain names. You can specify multiple accelerated domain names and separate them with commas (,).
+        # The accelerated domain name. You can specify multiple accelerated domain names and separate them with commas (,).
         # 
-        # >  You can specify at most 100 accelerated domain names in each call.
+        # > You can specify up to 100 accelerated domain names in each request.
         self.domain_name = domain_name
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
+        # The name of the Internet service provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
         self.isp_name_en = isp_name_en
-        # The name of the region. If you do not set this parameter, all regions are queried. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list.
+        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions. If you do not specify a region, all regions are queried.
         self.location_name_en = location_name_en
         # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
@@ -15440,17 +15587,17 @@
 class DescribeDomainRealTimeHttpCodeDataResponseBodyRealTimeHttpCodeDataUsageDataValueRealTimeCodeProportionData(TeaModel):
     def __init__(
         self,
         code: str = None,
         count: str = None,
         proportion: str = None,
     ):
-        # The HTTP status code.
+        # The HTTP status code returned.
         self.code = code
-        # The total number of HTTP status codes returned.
+        # The total number of entries.
         self.count = count
         # The proportion of the HTTP status code.
         self.proportion = proportion
 
     def validate(self):
         pass
 
@@ -15594,25 +15741,25 @@
         end_time: str = None,
         real_time_http_code_data: DescribeDomainRealTimeHttpCodeDataResponseBodyRealTimeHttpCodeData = None,
         request_id: str = None,
         start_time: str = None,
     ):
         # The time interval between the data entries returned. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 60 (1 minute), 300 (5 minutes), and 3600(1 hour). For more information, see the usage notes.
+        # Depending on the maximum time range per query, the value is 60 (1 minute), 300 (5 minutes), or 3600 (1 hour). For more information, see the "Time granularity" section in Usage notes.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
         # The proportions of HTTP status codes at each time interval.
         self.real_time_http_code_data = real_time_http_code_data
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.real_time_http_code_data:
             self.real_time_http_code_data.validate()
 
     def to_map(self):
@@ -15702,31 +15849,31 @@
         self,
         domain_name: str = None,
         end_time: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain names. You can specify multiple accelerated domain names and separate them with commas (,).
+        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
         # 
-        # >  You can specify at most 500 accelerated domain names in each call.
+        # > You can specify up to 500 domain names in each request.
         self.domain_name = domain_name
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service.
+        # The name of the Internet service provider (ISP).
         # 
-        # If you do not set this parameter, all ISPs are queried. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
+        # If you do not set this parameter, data of all ISPs is queried. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
         self.isp_name_en = isp_name_en
         # The name of the region.
         # 
-        # If you do not set this parameter, all regions are queried. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list.
+        # If you do not set this parameter, data in all regions is queried. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
         self.location_name_en = location_name_en
         # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
@@ -15769,15 +15916,15 @@
     def __init__(
         self,
         qps: float = None,
         time_stamp: str = None,
     ):
         # The number of queries per second.
         self.qps = qps
-        # The timestamp of the data returned. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
+        # The timestamp of the data returned. The time follows the yyyy-MM-ddTHH:mm:ssZ format in the ISO 8601 standard and is in UTC.
         self.time_stamp = time_stamp
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15837,15 +15984,15 @@
 
 class DescribeDomainRealTimeQpsDataResponseBody(TeaModel):
     def __init__(
         self,
         data: DescribeDomainRealTimeQpsDataResponseBodyData = None,
         request_id: str = None,
     ):
-        # The response parameters.
+        # The data entries returned.
         self.data = data
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.data:
             self.data.validate()
@@ -16114,21 +16261,23 @@
 class DescribeDomainRealTimeSrcBpsDataRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         start_time: str = None,
     ):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 100 domain names in each call.
+        # The accelerated domain name. You can specify up to 100 domain names in each request. Separate multiple domain names with commas (,).
         self.domain_name = domain_name
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The start of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query.
+        # 
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16157,15 +16306,15 @@
 
 class DescribeDomainRealTimeSrcBpsDataResponseBodyRealTimeSrcBpsDataPerIntervalDataModule(TeaModel):
     def __init__(
         self,
         time_stamp: str = None,
         value: str = None,
     ):
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp
         # The bandwidth during back-to-origin routing. Unit: bit/s.
         self.value = value
 
     def validate(self):
         pass
 
@@ -16233,25 +16382,25 @@
         end_time: str = None,
         real_time_src_bps_data_per_interval: DescribeDomainRealTimeSrcBpsDataResponseBodyRealTimeSrcBpsDataPerInterval = None,
         request_id: str = None,
         start_time: str = None,
     ):
         # The time interval between the data entries returned. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 60 (1 minute), 300 (5 minutes), and 3600(1 hour). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 60 (1 minute), 300 (5 minutes), and 3600(1 hour). For more information, see **Usage notes**.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range to query.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
-        # The back-to-origin bandwidth information at each interval.
+        # The origin bandwidth data at each interval.
         self.real_time_src_bps_data_per_interval = real_time_src_bps_data_per_interval
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range to query.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.real_time_src_bps_data_per_interval:
             self.real_time_src_bps_data_per_interval.validate()
 
     def to_map(self):
@@ -16341,25 +16490,25 @@
         self,
         domain_name: str = None,
         end_time: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 100 domain names in each call.
+        # The accelerated domain name. You can specify up to 100 domain names in each call. Separate multiple domain names with commas (,).
         self.domain_name = domain_name
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The name of the Internet Service Provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs. If you do not set this parameter, all ISPs are queried.
+        # The name of the Internet service provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs. If you leave this parameter empty, all ISPs are queried.
         self.isp_name_en = isp_name_en
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions. If you do not set this parameter, all regions are queried.
+        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions. If you leave this parameter empty, all regions are queried.
         self.location_name_en = location_name_en
-        # The start of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16397,17 +16546,17 @@
 class DescribeDomainRealTimeSrcHttpCodeDataResponseBodyRealTimeSrcHttpCodeDataUsageDataValueRealTimeSrcCodeProportionData(TeaModel):
     def __init__(
         self,
         code: str = None,
         count: str = None,
         proportion: str = None,
     ):
-        # The HTTP status code.
+        # The HTTP status code returned.
         self.code = code
-        # The total number of HTTP status codes returned.
+        # The count of each HTTP status code.
         self.count = count
         # The proportion of the HTTP status code.
         self.proportion = proportion
 
     def validate(self):
         pass
 
@@ -16473,17 +16622,17 @@
 
 class DescribeDomainRealTimeSrcHttpCodeDataResponseBodyRealTimeSrcHttpCodeDataUsageData(TeaModel):
     def __init__(
         self,
         time_stamp: str = None,
         value: DescribeDomainRealTimeSrcHttpCodeDataResponseBodyRealTimeSrcHttpCodeDataUsageDataValue = None,
     ):
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp
-        # The proportions of HTTP status codes.
+        # The proportions of the HTTP status codes.
         self.value = value
 
     def validate(self):
         if self.value:
             self.value.validate()
 
     def to_map(self):
@@ -16553,21 +16702,21 @@
         request_id: str = None,
         start_time: str = None,
     ):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
         # The proportions of HTTP status codes at each time interval.
         self.real_time_src_http_code_data = real_time_src_http_code_data
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.real_time_src_http_code_data:
             self.real_time_src_http_code_data.validate()
 
     def to_map(self):
@@ -16655,23 +16804,23 @@
 class DescribeDomainRealTimeSrcTrafficDataRequest(TeaModel):
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         start_time: str = None,
     ):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 100 domain names in each call.
+        # The accelerated domain name. You can specify up to 100 domain names in each call. Separate multiple domain names with commas (,).
         self.domain_name = domain_name
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The beginning of the time range to query.
+        # The start of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
@@ -16704,15 +16853,15 @@
     def __init__(
         self,
         time_stamp: str = None,
         value: str = None,
     ):
         # The timestamp of the data returned.
         self.time_stamp = time_stamp
-        # The amount of back-to-origin network traffic.
+        # The amount of traffic.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16778,25 +16927,25 @@
         end_time: str = None,
         real_time_src_traffic_data_per_interval: DescribeDomainRealTimeSrcTrafficDataResponseBodyRealTimeSrcTrafficDataPerInterval = None,
         request_id: str = None,
         start_time: str = None,
     ):
         # The time interval between the data entries returned. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 60, (1 minute), 300 (5 minutes), and 3600 (1 hour). For more information, see the usage notes.
+        # Depending on the maximum time range per query, the value is 60 (1 minute), 300 (5 minutes), or 3600 (1 hour). For more information, see the "Time granularity" section in Usage notes.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The end of the time range for which the data was queried.
         self.end_time = end_time
-        # The amount of back-to-origin network traffic that was collected at each interval.
+        # The amount of back-to-origin traffic returned at each interval.
         self.real_time_src_traffic_data_per_interval = real_time_src_traffic_data_per_interval
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range that was queried.
+        # The start of the time range for which the data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.real_time_src_traffic_data_per_interval:
             self.real_time_src_traffic_data_per_interval.validate()
 
     def to_map(self):
@@ -16886,23 +17035,23 @@
         self,
         domain_name: str = None,
         end_time: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 100 domain names in each call.
+        # The accelerated domain name. You can specify up to 100 domain names in each call. Separate multiple domain names with commas (,).
         self.domain_name = domain_name
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The name of the ISP for your Alibaba Cloud CDN service.
+        # The name of the Internet service provider (ISP).
         # 
         # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list. If you do not set this parameter, all regions are queried.
         self.isp_name_en = isp_name_en
         # The name of the region.
         # 
         # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list. If you do not set this parameter, all regions are queried.
         self.location_name_en = location_name_en
@@ -16949,17 +17098,17 @@
 
 class DescribeDomainRealTimeTrafficDataResponseBodyRealTimeTrafficDataPerIntervalDataModule(TeaModel):
     def __init__(
         self,
         time_stamp: str = None,
         value: str = None,
     ):
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp
-        # The amount of network traffic.
+        # The traffic value at each time interval.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17025,25 +17174,25 @@
         end_time: str = None,
         real_time_traffic_data_per_interval: DescribeDomainRealTimeTrafficDataResponseBodyRealTimeTrafficDataPerInterval = None,
         request_id: str = None,
         start_time: str = None,
     ):
         # The time interval between the data entries returned. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 60 (1 minute), 300 (5 minutes), and 3600(1 hour). For more information, see the usage notes.
+        # Depending on the maximum time range per query, the value is 60 (1 minute), 300 (5 minutes), or 3600 (1 hour). For more information, see the "Time granularity" section in Usage notes.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
-        # The amount of network traffic at each time interval. Unit: bytes.
+        # The network traffic returned at each time interval. Unit: bytes.
         self.real_time_traffic_data_per_interval = real_time_traffic_data_per_interval
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.real_time_traffic_data_per_interval:
             self.real_time_traffic_data_per_interval.validate()
 
     def to_map(self):
@@ -17558,29 +17707,29 @@
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         interval: str = None,
         start_time: str = None,
     ):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # By default, this operation queries the bandwidth values of back-to-origin requests for all accelerated domain names that belong to your Alibaba Cloud account.
+        # By default, this operation queries the request hit ratio for all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The time interval between the data entries. Unit: seconds.
+        # The time granularity of the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval
-        # The start of the time range to query.
+        # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
@@ -17618,17 +17767,17 @@
         self,
         https_value: str = None,
         time_stamp: str = None,
         value: str = None,
     ):
         # The hit ratio of HTTPS requests.
         self.https_value = https_value
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp
-        # The byte hit ratio.
+        # The request hit ratio.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17700,21 +17849,21 @@
         request_id: str = None,
         start_time: str = None,
     ):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
-        # The request hit ratio at each time interval. The hit ratio is measured in percentage.
+        # The request hit ratio data at each time interval. The hit ratio is measured in percentage.
         self.req_hit_rate_interval = req_hit_rate_interval
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.req_hit_rate_interval:
             self.req_hit_rate_interval.validate()
 
     def to_map(self):
@@ -17803,29 +17952,29 @@
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         interval: str = None,
         start_time: str = None,
     ):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify up to 500 domain names in each call. Separate multiple domain names with commas (,).
         # 
-        # By default, this operation queries the bandwidth values during back-to-origin routing for all accelerated domain names that belong to your Alibaba Cloud account.
+        # By default, this operation queries the geographic distribution of users for all accelerated domain names.
         self.domain_name = domain_name
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
         # The time interval between the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Description**.
         self.interval = interval
-        # The start of the time range to query.
+        # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
@@ -17861,19 +18010,19 @@
 class DescribeDomainSrcBpsDataResponseBodySrcBpsDataPerIntervalDataModule(TeaModel):
     def __init__(
         self,
         https_value: str = None,
         time_stamp: str = None,
         value: str = None,
     ):
-        # The bandwidth values of HTTPS requests.
+        # The bandwidth values of origin HTTPS requests.
         self.https_value = https_value
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp
-        # The bandwidth value.
+        # The traffic value at each time interval.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17945,21 +18094,21 @@
         src_bps_data_per_interval: DescribeDomainSrcBpsDataResponseBodySrcBpsDataPerInterval = None,
         start_time: str = None,
     ):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
         # The ID of the request.
         self.request_id = request_id
-        # The bandwidth value at each time interval. Unit: bit/s.
+        # The origin bandwidth data at each time interval. Unit: bit/s.
         self.src_bps_data_per_interval = src_bps_data_per_interval
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.src_bps_data_per_interval:
             self.src_bps_data_per_interval.validate()
 
     def to_map(self):
@@ -18048,29 +18197,25 @@
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         interval: str = None,
         start_time: str = None,
     ):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify a maximum of 500 domain names in a request. Separate multiple domain names with commas (,).
         self.domain_name = domain_name
-        # The end of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC. The time must be in UTC.
+        # The end of the time range to query. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format in the ISO 8601 standard. The time is displayed in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The time interval between the data entries. Unit: seconds.
+        # The time interval between the data entries to return. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Description**.
         self.interval = interval
-        # The start of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18104,17 +18249,17 @@
 class DescribeDomainSrcHttpCodeDataResponseBodyHttpCodeDataUsageDataValueCodeProportionData(TeaModel):
     def __init__(
         self,
         code: str = None,
         count: str = None,
         proportion: str = None,
     ):
-        # The HTTP status code.
+        # The HTTP status code returned.
         self.code = code
-        # The total number of HTTP status codes returned.
+        # The total number of entries.
         self.count = count
         # The proportion of the HTTP status code.
         self.proportion = proportion
 
     def validate(self):
         pass
 
@@ -18180,17 +18325,17 @@
 
 class DescribeDomainSrcHttpCodeDataResponseBodyHttpCodeDataUsageData(TeaModel):
     def __init__(
         self,
         time_stamp: str = None,
         value: DescribeDomainSrcHttpCodeDataResponseBodyHttpCodeDataUsageDataValue = None,
     ):
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp
-        # The proportions of HTTP status codes.
+        # The proportions of the HTTP status codes.
         self.value = value
 
     def validate(self):
         if self.value:
             self.value.validate()
 
     def to_map(self):
@@ -18260,21 +18405,21 @@
         request_id: str = None,
         start_time: str = None,
     ):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
         # The proportions of HTTP status codes at each time interval.
         self.http_code_data = http_code_data
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.http_code_data:
             self.http_code_data.validate()
 
     def to_map(self):
@@ -18363,29 +18508,29 @@
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         interval: str = None,
         start_time: str = None,
     ):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify multiple domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # By default, this operation queries the number of back-to-origin requests per second for all accelerated domain names that belong to your Alibaba Cloud account.
+        # By default, this operation queries QPS data for all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The time granularity of the data entries. Unit: seconds.
+        # The time interval between the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval
-        # The start of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # If you do not set this parameter, data collected within the last 24 hours is queried.
+        # If you leave this parameter empty, data collected in the last 24 hours is queried.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18420,15 +18565,15 @@
     def __init__(
         self,
         time_stamp: str = None,
         value: str = None,
     ):
         # The timestamp of the data returned.
         self.time_stamp = time_stamp
-        # The number of back-to-origin requests per second.
+        # The QPS value.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18496,21 +18641,21 @@
         src_qps_data_per_interval: DescribeDomainSrcQpsDataResponseBodySrcQpsDataPerInterval = None,
         start_time: str = None,
     ):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
         # The ID of the request.
         self.request_id = request_id
         # The back-to-origin bandwidth information at each interval.
         self.src_qps_data_per_interval = src_qps_data_per_interval
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.src_qps_data_per_interval:
             self.src_qps_data_per_interval.validate()
 
     def to_map(self):
@@ -19245,29 +19390,29 @@
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         interval: str = None,
         start_time: str = None,
     ):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # By default, this operation queries back-to-origin network traffic for all accelerated domain names that belong to your Alibaba Cloud account.
+        # By default, this operation queries the origin traffic for all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The time interval between the data entries. Unit: seconds.
+        # The time granularity of the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval
-        # The start of the time range to query.
+        # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
@@ -19303,19 +19448,19 @@
 class DescribeDomainSrcTrafficDataResponseBodySrcTrafficDataPerIntervalDataModule(TeaModel):
     def __init__(
         self,
         https_value: str = None,
         time_stamp: str = None,
         value: str = None,
     ):
-        # The amount of traffic generated by back-to-origin HTTPS requests.
+        # The amount of traffic generated by origin HTTPS requests.
         self.https_value = https_value
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp
-        # The amount of network traffic.
+        # The traffic value at each time interval.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19387,21 +19532,21 @@
         src_traffic_data_per_interval: DescribeDomainSrcTrafficDataResponseBodySrcTrafficDataPerInterval = None,
         start_time: str = None,
     ):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
         # The ID of the request.
         self.request_id = request_id
-        # The amount of back-to-origin network traffic at each time interval. Unit: bytes.
+        # The amount of origin traffic returned at each time interval. Unit: bytes.
         self.src_traffic_data_per_interval = src_traffic_data_per_interval
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
 
     def validate(self):
         if self.src_traffic_data_per_interval:
             self.src_traffic_data_per_interval.validate()
 
     def to_map(self):
@@ -19940,28 +20085,32 @@
     def __init__(
         self,
         domain_name: str = None,
         end_time: str = None,
         sort_by: str = None,
         start_time: str = None,
     ):
-        # The accelerated domain name for which you want to query data. If you do not set this parameter, frequently requested URLs of all accelerated domain names of your Alibaba Cloud account are queried.
+        # The accelerated domain name that you want to query.
         self.domain_name = domain_name
-        # The end of the time range to query. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
+        # The end of the time range to query.
         # 
-        # >  The end time must be later than the start time. The difference between the end time and the start time cannot exceed seven days.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # > The end time must be later than the start time. The maximum time range that can be specified is seven days.
         self.end_time = end_time
-        # The method that is used to sort the returned URLs.**** Valid values:
+        # The method that is used to sort the returned URLs. Default value: **pv**. Valid values:
         # 
-        # *   **traf**: network traffic
-        # *   **pv**: by the number of page views. This is the default value.
+        # *   **traf**: by network traffic
+        # *   **pv**: by the number of page views
         self.sort_by = sort_by
-        # The start of the time range to query. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
+        # The start of the time range to query.
         # 
-        # If you want to query data within a specific day, we recommend that you set the value in the yyyy-MM-ddT16:00:00Z format.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # If you want to query data of a specific day, we recommend that you set the value in the yyyy-MM-ddT16:00:00Z format.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19997,23 +20146,23 @@
         self,
         flow: str = None,
         flow_proportion: float = None,
         url_detail: str = None,
         visit_data: str = None,
         visit_proportion: float = None,
     ):
-        # The amount of network traffic. (Unit: bytes)
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow
-        # The proportion of the amount of network traffic consumed for visiting the web page.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion
         # The complete URL.
         self.url_detail = url_detail
-        # The number of visits to the specified path.
+        # The number of visits to the URL.
         self.visit_data = visit_data
-        # The proportion of visits to the web page.
+        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20088,23 +20237,23 @@
         self,
         flow: str = None,
         flow_proportion: float = None,
         url_detail: str = None,
         visit_data: str = None,
         visit_proportion: float = None,
     ):
-        # The amount of network traffic. (Unit: bytes)
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow
-        # The proportion of the amount of network traffic consumed for visiting the web page.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion
         # The complete URL.
         self.url_detail = url_detail
-        # The number of visits to the specified path.
+        # The number of visits to the URL.
         self.visit_data = visit_data
-        # The proportion of visits to the web page.
+        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20179,23 +20328,23 @@
         self,
         flow: str = None,
         flow_proportion: float = None,
         url_detail: str = None,
         visit_data: str = None,
         visit_proportion: float = None,
     ):
-        # The amount of network traffic. (Unit: bytes)
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow
-        # The proportion of the amount of network traffic consumed for visiting the web page.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion
         # The complete URL.
         self.url_detail = url_detail
         # The number of visits to the URL.
         self.visit_data = visit_data
-        # The proportion of visits to the web page.
+        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20270,23 +20419,23 @@
         self,
         flow: str = None,
         flow_proportion: float = None,
         url_detail: str = None,
         visit_data: str = None,
         visit_proportion: float = None,
     ):
-        # The amount of network traffic. (Unit: bytes)
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow
-        # The proportion of the amount of network traffic consumed for visiting the web page.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion
         # The complete URL.
         self.url_detail = url_detail
         # The number of visits to the URL.
         self.visit_data = visit_data
-        # The proportion of visits to the web page.
+        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20361,23 +20510,23 @@
         self,
         flow: str = None,
         flow_proportion: float = None,
         url_detail: str = None,
         visit_data: str = None,
         visit_proportion: float = None,
     ):
-        # The amount of network traffic. (Unit: bytes)
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow
-        # The proportion of the amount of network traffic consumed for visiting the web page.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion
         # The complete URL.
         self.url_detail = url_detail
         # The number of visits to the URL.
         self.visit_data = visit_data
-        # The proportion of visits to the web page.
+        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20461,15 +20610,15 @@
     ):
         # A list of frequently requested URLs.
         self.all_url_list = all_url_list
         # The accelerated domain name.
         self.domain_name = domain_name
         # The ID of the request.
         self.request_id = request_id
-        # The start of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
         # A list of URLs for which 2xx status codes were returned.
         self.url_200list = url_200list
         # A list of URLs for which 3xx status codes were returned.
         self.url_300list = url_300list
         # A list of URLs for which 4xx status codes were returned.
         self.url_400list = url_400list
@@ -20588,39 +20737,35 @@
         domain_name: str = None,
         end_time: str = None,
         interval: str = None,
         isp_name_en: str = None,
         location_name_en: str = None,
         start_time: str = None,
     ):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # By default, this operation queries the monitoring data of network traffic for all accelerated domain names that belong to your Alibaba Cloud account.
+        # By default, this operation queries the network traffic for all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name
-        # The end of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The time interval between the data entries. Unit: seconds.
+        # The time granularity of the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval
-        # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
+        # The name of the Internet service provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~DescribeCdnRegionAndIsp~~) operation to query ISPs.
         # 
-        # If you do not specify an ISP, monitoring data of all ISPs is queried.
+        # If you do not specify an ISP, data of all ISPs is queried.
         self.isp_name_en = isp_name_en
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list.
+        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~DescribeCdnRegionAndIsp~~) operation to query regions.
         # 
-        # If you do not specify a region, monitoring data in all regions is queried.
+        # If you do not specify a region, data in all regions is queried.
         self.location_name_en = location_name_en
-        # The start of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20668,25 +20813,25 @@
         https_value: str = None,
         overseas_value: str = None,
         time_stamp: str = None,
         value: str = None,
     ):
         # The amount of network traffic in the Chinese mainland.
         self.domestic_value = domestic_value
-        # The amount of HTTPS network traffic on L1 edge nodes in the Chinese mainland.
+        # The amount of HTTPS traffic on points of presence (POPs) in the Chinese mainland.
         self.https_domestic_value = https_domestic_value
-        # The amount of HTTPS network traffic on L1 edge nodes outside the Chinese mainland.
+        # The amount of HTTPS traffic on POPs outside the Chinese mainland.
         self.https_overseas_value = https_overseas_value
-        # The total amount of HTTPS network traffic on L1 edge nodes.
+        # The total amount of HTTPS traffic on POPs.
         self.https_value = https_value
         # The amount of network traffic outside the Chinese mainland.
         self.overseas_value = overseas_value
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp
-        # The total amount of network traffic.
+        # The total volume of traffic.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20774,19 +20919,19 @@
         start_time: str = None,
         traffic_data_per_interval: DescribeDomainTrafficDataResponseBodyTrafficDataPerInterval = None,
     ):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
         # The amount of network traffic at each time interval. Unit: bytes.
         self.traffic_data_per_interval = traffic_data_per_interval
 
     def validate(self):
         if self.traffic_data_per_interval:
             self.traffic_data_per_interval.validate()
@@ -20881,69 +21026,69 @@
         domain_name: str = None,
         end_time: str = None,
         field: str = None,
         interval: str = None,
         start_time: str = None,
         type: str = None,
     ):
-        # The ID of the billable region. Valid values:
+        # The billable region. Default value: CN. Valid values:
         # 
-        # *   **CN** (default): the Chinese mainland
+        # *   **CN**: Chinese mainland
         # *   **OverSeas**: outside the Chinese mainland
         # *   **AP1**: Asia Pacific 1
         # *   **AP2**: Asia Pacific 2
         # *   **AP3**: Asia Pacific 3
         # *   **NA**: North America
         # *   **SA**: South America
         # *   **EU**: Europe
         # *   **MEAA**: Middle East and Africa
-        # *   **all**: all billable regions
-        # 
-        # >  For more information about billable regions, see [Billable regions](~~142221~~).
+        # *   **all**: all the preceding billable regions
         self.area = area
-        # The protocol by which the data is queried. Valid values:
+        # The protocol of the data that you want to query. Default value: all. Valid values:
         # 
         # *   **http**: HTTP
         # *   **https**: HTTPS
         # *   **quic**: QUIC
-        # *   **all** (default): HTTP, HTTPS, and QUIC
+        # *   **all**: HTTP, HTTPS, and QUIC
         self.data_protocol = data_protocol
-        # The accelerated domain name. You can query the resource usage data for a maximum of 100 domain names in each call. Separate domain names with commas (,).
+        # The accelerated domain name. You can specify up to 100 domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # >  If you do not set this parameter, the usage data of all accelerated domain names within your Alibaba Cloud account is returned.
+        # > If you leave this parameter empty, the usage data of all accelerated domain names in your Alibaba Cloud account is returned.
         self.domain_name = domain_name
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time. The maximum time range that can be queried is 31 days.
+        # > The end time must be later than the start time. The maximum time range that can be specified is 31 days.
         self.end_time = end_time
-        # The type of data to be queried. Valid values:
+        # The type of data that you want to query. Valid values:
         # 
         # *   **bps**: bandwidth
-        # *   **traf**: network traffic
+        # *   **traf**: traffic
         # *   **acc**: requests
         # 
-        # >  **acc** does not support the **Area** parameter.
+        # > If you set this parameter to **acc**, the **Area** parameter is not supported.
         self.field = field
-        # The time interval between the data entries. Unit: seconds.
+        # The time interval between the data entries to return. Unit: seconds. Valid values: **300** (5 minutes), **3600** (1 hour), and **86400** (1 day).
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # *   If **Interval** is set to **300**, you can query usage data in the last six months. The maximum time range per query that can be specified is three days.
+        # *   If **Interval** is set to **3600** or **86400**, you can query usage data of the previous year.
+        # *   If you do not set the **Interval** parameter, the maximum time range that you can query is one month. If you specify a time range of 1 to 3 days, the time interval between the entries that are returned is 1 hour. If you specify a time range of at least 4 days, the time interval between the entries that are returned is 1 day.
         self.interval = interval
         # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The data is collected every 5 minutes.
+        # > Data is collected every 5 minutes.
         self.start_time = start_time
-        # The type of content based on which the data is queried. Valid values:
+        # The type of content that you want to query. Default value: all. Valid values:
         # 
         # *   **static**: static content
         # *   **dynamic**: dynamic content
-        # *   **all** (default): both static and dynamic content
+        # *   **all**: both static and dynamic content
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20994,27 +21139,25 @@
     def __init__(
         self,
         peak_time: str = None,
         special_value: str = None,
         time_stamp: str = None,
         value: str = None,
     ):
-        # If the **Field** parameter in the request is set to **bps**, this parameter returns the time of the peak bandwidth value. Otherwise, this parameter returns the same value as the **TimeStamp** parameter.
+        # The time of the peak bandwidth value if the **Field** parameter in the request is set to **bps**. Otherwise, this parameter returns the same value as the **TimeStamp** parameter.
         self.peak_time = peak_time
         # The data usage in a specific scenario.
         # 
-        # >  Indicates the data usage in a specific scenario. If no special billable item is specified, ignore this parameter.
+        # > SpecialValue indicates the data usage in a specific scenario. If no special billable item is specified, ignore this parameter.
         self.special_value = special_value
         # The timestamp of the data returned.
         # 
-        # >  The **TimeStamp** parameter may return multiple values.
+        # > **TimeStamp** indicates the timestamp of the returned data at each interval.
         self.time_stamp = time_stamp
-        # The usage.
-        # 
-        # >  Usage data includes network traffic (measured in bytes), bandwidth values (measured in bits/s), and the number of requests.
+        # The amount of resource usage.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -21088,29 +21231,29 @@
         domain_name: str = None,
         end_time: str = None,
         request_id: str = None,
         start_time: str = None,
         type: str = None,
         usage_data_per_interval: DescribeDomainUsageDataResponseBodyUsageDataPerInterval = None,
     ):
-        # The billable region where the usage information was collected.
+        # The billable region where the data was collected.
         self.area = area
-        # The time interval between the data entries. Unit: seconds.
+        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
         # The ID of the request.
         self.request_id = request_id
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
-        # The type of content based on which the usage information was collected.
+        # The type of content.
         self.type = type
-        # The network traffic that was collected at each interval.
+        # The resource usage that was collected at each interval.
         self.usage_data_per_interval = usage_data_per_interval
 
     def validate(self):
         if self.usage_data_per_interval:
             self.usage_data_per_interval.validate()
 
     def to_map(self):
@@ -21323,15 +21466,15 @@
         data_interval: str = None,
         domain_name: str = None,
         end_time: str = None,
         request_id: str = None,
         start_time: str = None,
         uv_data_interval: DescribeDomainUvDataResponseBodyUvDataInterval = None,
     ):
-        # The time interval between the data entries. Unit: seconds.
+        # The time interval. Unit: seconds.
         self.data_interval = data_interval
         # The accelerated domain name.
         self.domain_name = domain_name
         # The end of the time range that was queried.
         self.end_time = end_time
         # The ID of the request.
         self.request_id = request_id
@@ -21778,21 +21921,25 @@
         self,
         domain_name: str = None,
         end_time: str = None,
         start_time: str = None,
     ):
         # The accelerated domain name. You can specify only one domain name.
         # 
-        # If you do not specify an accelerated domain name, the monitoring data of all accelerated domain names that belong to your account is queried.
+        # If you do not specify an accelerated domain name, the data of all accelerated domain names that belong to your account is queried.
         self.domain_name = domain_name
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The end of the time range to query.
         # 
-        # >  The end time must be later than the start time.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # > The end time must be later than the start time.
         self.end_time = end_time
-        # The start of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The beginning of the time range to query.
+        # 
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -21829,15 +21976,15 @@
         max_src_bps_time: str = None,
         qps: str = None,
         request_hit_rate: str = None,
         time_stamp: str = None,
         total_access: str = None,
         total_traffic: str = None,
     ):
-        # The cache hit ratio that is calculated based on bytes. The cache hit ratio is measured in percentage.
+        # The byte hit ratio. The byte hit ratio is measured in percentage.
         self.bytes_hit_rate = bytes_hit_rate
         # The peak bandwidth value. Unit: bit/s.
         self.max_bps = max_bps
         # The time when the bandwidth reached the peak value.
         self.max_bps_time = max_bps_time
         # The peak bandwidth value during back-to-origin routing. Unit: bit/s.
         self.max_src_bps = max_src_bps
@@ -21953,27 +22100,27 @@
         max_bps_time: str = None,
         max_src_bps: str = None,
         max_src_bps_time: str = None,
         request_hit_rate: str = None,
         total_access: str = None,
         total_traffic: str = None,
     ):
-        # The cache hit ratio that is calculated based on bytes. The cache hit ratio is measured in percentage.
+        # The byte hit ratio. The byte hit ratio is measured in percentage.
         self.bytes_hit_rate = bytes_hit_rate
         # The peak bandwidth value. Unit: bit/s.
         self.max_bps = max_bps
         # The time when the bandwidth reached the peak value.
         self.max_bps_time = max_bps_time
         # The peak bandwidth value during back-to-origin routing. Unit: bit/s.
         self.max_src_bps = max_src_bps
         # The time when the bandwidth during back-to-origin routing reached the peak value.
         self.max_src_bps_time = max_src_bps_time
         # The cache hit ratio that is calculated based on requests. The cache hit ratio is measured in percentage.
         self.request_hit_rate = request_hit_rate
-        # The total number of requests.
+        # The total amount of requests.
         self.total_access = total_access
         # The total amount of network traffic. Unit: bytes.
         self.total_traffic = total_traffic
 
     def validate(self):
         pass
 
@@ -22029,23 +22176,23 @@
         domain_name: str = None,
         end_time: str = None,
         request_id: str = None,
         start_time: str = None,
         usage_by_days: DescribeDomainsUsageByDayResponseBodyUsageByDays = None,
         usage_total: DescribeDomainsUsageByDayResponseBodyUsageTotal = None,
     ):
-        # The time interval between the data entries. Unit: seconds.
+        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval
-        # The information about the accelerated domain name.
+        # The accelerated domain name.
         self.domain_name = domain_name
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time
         # The ID of the request.
         self.request_id = request_id
-        # The start of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time
         # The monitoring data collected at each time interval.
         self.usage_by_days = usage_by_days
         # The summarized monitoring data.
         self.usage_total = usage_total
 
     def validate(self):
@@ -23498,29 +23645,29 @@
         location_names: str = None,
         start_time: str = None,
     ):
         # The accelerated domain name.
         self.domain_names = domain_names
         # The end of the time range to query.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time. The interval between the end time and the start time cannot exceed 1 hour.
+        # > The end time must be later than the start time. The maximum time range that can be specified is 1 hour.
         self.end_time = end_time
         # The name of the ISP. You can specify only one ISP name in each call.
         # 
         # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs.
         self.isp_names = isp_names
-        # The names of the regions. Separate regions with commas (,).
+        # The names of the regions. Separate multiple region names with commas (,).
         # 
         # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list.
         self.location_names = location_names
         # The beginning of the time range to query.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -23557,17 +23704,15 @@
 
 class DescribeRangeDataByLocateAndIspServiceResponseBody(TeaModel):
     def __init__(
         self,
         json_result: str = None,
         request_id: str = None,
     ):
-        # The response parameters in the JSON format.
-        # 
-        # These parameters indicate the following information in sequence: UNIX time, region, ISP, distribution of HTTP status codes, response time, bandwidth (bit/s), average response rate, page views, cache hit ratio, and request hit ratio.
+        # The response parameters in the JSON format. These parameters indicate the following information in sequence: UNIX time, region, ISP, distribution of HTTP status codes, response time, bandwidth (bit/s), average response rate, page views, cache hit ratio, and request hit ratio.
         self.json_result = json_result
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
@@ -28678,34 +28823,35 @@
         object_path: str = None,
         owner_id: int = None,
         security_token: str = None,
         with_header: str = None,
     ):
         # The accelerated region where content is to be prefetched. Valid values:
         # 
-        # *   **domestic**: **Chinese Mainland Only**\
-        # *   **overseas**: **Global (Excluding the Chinese Mainland)**\
+        # *   **domestic****: Chinese mainland**\
+        # *   **overseas****: regions outside the Chinese mainland**\
         # 
-        # If you do not set this parameter, content in the accelerated region of the domain name is prefetched. Content is prefetched based on the following rules:
+        # If you do not set this parameter, content in the accelerated region of the domain name is prefetched.
         # 
-        # *   If the accelerated region is set to ****Chinese Mainland Only****, content in regions in the Chinese mainland is prefetched.
+        # *   If the accelerated region is set to **Mainland China Only**, content in regions in the Chinese mainland is prefetched.
         # *   If the accelerated region is set to **Global**, content in all regions is prefetched.
-        # *   If the accelerated region is set to **Global (Excluding the Chinese Mainland)**, content in regions outside the Chinese mainland is prefetched.
+        # *   If the accelerated region is set to **Global (Excluding Mainland China)**, content in regions outside the Chinese mainland is prefetched.
         self.area = area
         # Specifies whether to prefetch content to POPs. Valid values:
         # 
-        # *   **true**: prefetch content to L2 edge nodes.
-        # *   **false**: prefetch content to regular edge nodes. Regular edge nodes can be L2 edge nodes or L3 edge nodes. Default value: **false**.
+        # *   **true**: prefetches content to POPs.
+        # *   **false**: prefetches content to regular POPs. Regular POPs can be L2 POPs or L3 POPs. Default value: **false**.
         self.l_2preload = l_2preload
         # The URLs based on which content is prefetched. Format: **accelerated domain name/files to be prefetched**.
         # 
-        # >  Separate URLs with line feeds (\n or \r\n). Each object path can be up to 1,024 characters in length.
+        # > Separate URLs with line feeds (\n or \r\n). Each object path can be up to 1,024 characters in length.
         self.object_path = object_path
         self.owner_id = owner_id
         self.security_token = security_token
+        # The custom header for prefetch in the JSON format.
         self.with_header = with_header
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -28831,15 +28977,15 @@
         self,
         object_path: str = None,
         object_type: str = None,
         owner_id: int = None,
         security_token: str = None,
     ):
         self.object_path = object_path
-        # The type of the object that you want to refresh. Valid values:
+        # The type of the object that you want to refresh. Default value: File. Valid values:
         # 
         # *   **File**: refreshes one or more files.
         # *   **Directory**: refreshes the files in one or more directories.
         # *   **Regex**: refreshes content based on regular expressions.
         # 
         # If you set the ObjectType parameter to File or Directory, you can view [Refresh and prefetch resources](~~27140~~) to obtain more information. If you set the ObjectType parameter to Regex, you can view [Configure URL refresh rules that contain regular expressions](~~146195~~) to obtain more information.
         #
```

### Comparing `alibabacloud_cdn20180510-1.2.6/alibabacloud_cdn20180510.egg-info/PKG-INFO` & `alibabacloud_cdn20180510-1.2.7/alibabacloud_cdn20180510.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cdn20180510
-Version: 1.2.6
+Version: 1.2.7
 Summary: Alibaba Cloud Alibaba Cloud CDN (20180510) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cdn20180510-1.2.6/setup.py` & `alibabacloud_cdn20180510-1.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cdn20180510.
 
-Created on 29/03/2023
+Created on 25/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cdn20180510"
 NAME = "alibabacloud_cdn20180510" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Alibaba Cloud CDN (20180510) SDK Library for Python"
```

