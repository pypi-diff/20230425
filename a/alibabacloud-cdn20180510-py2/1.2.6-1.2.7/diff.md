# Comparing `tmp/alibabacloud_cdn20180510_py2-1.2.6.tar.gz` & `tmp/alibabacloud_cdn20180510_py2-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cdn20180510_py2-1.2.6.tar", last modified: Wed Mar 29 08:13:01 2023, max compression
+gzip compressed data, was "dist/alibabacloud_cdn20180510_py2-1.2.7.tar", last modified: Tue Apr 25 07:16:42 2023, max compression
```

## Comparing `alibabacloud_cdn20180510_py2-1.2.6.tar` & `alibabacloud_cdn20180510_py2-1.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 08:13:01.000000 alibabacloud_cdn20180510_py2-1.2.6/
--rw-r--r--   0 root         (0) root         (0)     1356 2023-03-29 08:13:01.000000 alibabacloud_cdn20180510_py2-1.2.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-03-29 08:13:01.000000 alibabacloud_cdn20180510_py2-1.2.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-03-29 08:13:01.000000 alibabacloud_cdn20180510_py2-1.2.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2486 2023-03-29 08:13:01.000000 alibabacloud_cdn20180510_py2-1.2.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2023-03-29 08:13:01.000000 alibabacloud_cdn20180510_py2-1.2.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-03-29 08:13:01.000000 alibabacloud_cdn20180510_py2-1.2.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 08:13:01.000000 alibabacloud_cdn20180510_py2-1.2.6/alibabacloud_cdn20180510/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-29 08:13:01.000000 alibabacloud_cdn20180510_py2-1.2.6/alibabacloud_cdn20180510/__init__.py
--rw-r--r--   0 root         (0) root         (0)   354436 2023-03-29 08:13:01.000000 alibabacloud_cdn20180510_py2-1.2.6/alibabacloud_cdn20180510/client.py
--rw-r--r--   0 root         (0) root         (0)  1072054 2023-03-29 08:13:01.000000 alibabacloud_cdn20180510_py2-1.2.6/alibabacloud_cdn20180510/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 08:13:01.000000 alibabacloud_cdn20180510_py2-1.2.6/alibabacloud_cdn20180510_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2486 2023-03-29 08:13:01.000000 alibabacloud_cdn20180510_py2-1.2.6/alibabacloud_cdn20180510_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2023-03-29 08:13:01.000000 alibabacloud_cdn20180510_py2-1.2.6/alibabacloud_cdn20180510_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 08:13:01.000000 alibabacloud_cdn20180510_py2-1.2.6/alibabacloud_cdn20180510_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-03-29 08:13:01.000000 alibabacloud_cdn20180510_py2-1.2.6/alibabacloud_cdn20180510_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-03-29 08:13:01.000000 alibabacloud_cdn20180510_py2-1.2.6/alibabacloud_cdn20180510_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-29 08:13:01.000000 alibabacloud_cdn20180510_py2-1.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2917 2023-03-29 08:13:01.000000 alibabacloud_cdn20180510_py2-1.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2486 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   354806 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510/client.py
+-rw-r--r--   0 root         (0) root         (0)  1077740 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2486 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-04-25 07:16:42.000000 alibabacloud_cdn20180510_py2-1.2.7/setup.py
```

### Comparing `alibabacloud_cdn20180510_py2-1.2.6/ChangeLog.md` & `alibabacloud_cdn20180510_py2-1.2.7/ChangeLog.md`

 * *Files 2% similar despite different names*

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

### Comparing `alibabacloud_cdn20180510_py2-1.2.6/LICENSE` & `alibabacloud_cdn20180510_py2-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cdn20180510_py2-1.2.6/PKG-INFO` & `alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_cdn20180510_py2
-Version: 1.2.6
+Name: alibabacloud-cdn20180510-py2
+Version: 1.2.7
 Summary: Alibaba Cloud Alibaba Cloud CDN (20180510) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cdn20180510_py2-1.2.6/README-CN.md` & `alibabacloud_cdn20180510_py2-1.2.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cdn20180510_py2-1.2.6/README.md` & `alibabacloud_cdn20180510_py2-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cdn20180510_py2-1.2.6/alibabacloud_cdn20180510/client.py` & `alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -463,18 +463,18 @@
         @return: BatchStartCdnDomainResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.batch_start_cdn_domain_with_options(request, runtime)
 
     def batch_stop_cdn_domain_with_options(self, request, runtime):
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
@@ -504,18 +504,18 @@
         return TeaCore.from_map(
             cdn_20180510_models.BatchStopCdnDomainResponse(),
             self.call_api(params, req, runtime)
         )
 
     def batch_stop_cdn_domain(self, request):
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
@@ -691,16 +691,16 @@
         @return: CreateCdnDeliverTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_cdn_deliver_task_with_options(request, runtime)
 
     def create_cdn_sub_task_with_options(self, request, runtime):
         """
-        > - This operation allows you to customize an operations report for a specific domain name. You can view the statistics about the domain name in the report.
-        - You can call this API operation up to three times per second per account.
+        This operation allows you to create a custom operations report for a specific domain name. You can view the statistics about the domain name in the report.
+        *   You can call this operation up to three times per second per account.
         
 
         @param request: CreateCdnSubTaskRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CreateCdnSubTaskResponse
@@ -728,16 +728,16 @@
         return TeaCore.from_map(
             cdn_20180510_models.CreateCdnSubTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_cdn_sub_task(self, request):
         """
-        > - This operation allows you to customize an operations report for a specific domain name. You can view the statistics about the domain name in the report.
-        - You can call this API operation up to three times per second per account.
+        This operation allows you to create a custom operations report for a specific domain name. You can view the statistics about the domain name in the report.
+        *   You can call this operation up to three times per second per account.
         
 
         @param request: CreateCdnSubTaskRequest
 
         @return: CreateCdnSubTaskResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -837,16 +837,16 @@
         @return: CreateRealTimeLogDeliveryResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_real_time_log_delivery_with_options(request, runtime)
 
     def create_usage_detail_data_export_task_with_options(self, request, runtime):
         """
-        - You can create a task that queries data of up to the last year. The maximum time range that can be queried is one month.
-        - The maximum number of times that each Alibaba Cloud account can call this operation per second is 100.
+        You can create a task to query data in the last year. The maximum time range that can be queried is one month.
+        *   You can call this operation up to 100 times per second per account.
         
 
         @param request: CreateUsageDetailDataExportTaskRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CreateUsageDetailDataExportTaskResponse
@@ -884,29 +884,29 @@
         return TeaCore.from_map(
             cdn_20180510_models.CreateUsageDetailDataExportTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_usage_detail_data_export_task(self, request):
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
 
     def create_user_usage_data_export_task_with_options(self, request, runtime):
         """
-        >    You can create a task that queries data of up to the last one year. The maximum time range that can be queried is one month.
-        > *   The maximum number of times that each user can call this operation per second is 100.
+        You can create a task to query data in the last year. The maximum time range that can be queried is one month.
+        *   You can call this operation up to 100 times per second per account.
         
 
         @param request: CreateUserUsageDataExportTaskRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: CreateUserUsageDataExportTaskResponse
@@ -938,16 +938,16 @@
         return TeaCore.from_map(
             cdn_20180510_models.CreateUserUsageDataExportTaskResponse(),
             self.call_api(params, req, runtime)
         )
 
     def create_user_usage_data_export_task(self, request):
         """
-        >    You can create a task that queries data of up to the last one year. The maximum time range that can be queried is one month.
-        > *   The maximum number of times that each user can call this operation per second is 100.
+        You can create a task to query data in the last year. The maximum time range that can be queried is one month.
+        *   You can call this operation up to 100 times per second per account.
         
 
         @param request: CreateUserUsageDataExportTaskRequest
 
         @return: CreateUserUsageDataExportTaskResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -1593,15 +1593,15 @@
         @return: DescribeCdnDeletedDomainsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_deleted_domains_with_options(request, runtime)
 
     def describe_cdn_deliver_list_with_options(self, request, runtime):
         """
-        >  You can call this operation up to three times per second.
+        > You can call this operation up to 3 times per second per account.
         
 
         @param request: DescribeCdnDeliverListRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeCdnDeliverListResponse
@@ -1627,27 +1627,27 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnDeliverListResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_deliver_list(self, request):
         """
-        >  You can call this operation up to three times per second.
+        > You can call this operation up to 3 times per second per account.
         
 
         @param request: DescribeCdnDeliverListRequest
 
         @return: DescribeCdnDeliverListResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_deliver_list_with_options(request, runtime)
 
     def describe_cdn_domain_by_certificate_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeCdnDomainByCertificateRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeCdnDomainByCertificateResponse
@@ -1675,15 +1675,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnDomainByCertificateResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_domain_by_certificate(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeCdnDomainByCertificateRequest
 
         @return: DescribeCdnDomainByCertificateResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -1791,17 +1791,18 @@
         @return: DescribeCdnDomainDetailResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_domain_detail_with_options(request, runtime)
 
     def describe_cdn_domain_logs_with_options(self, request, runtime):
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
@@ -1835,17 +1836,18 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnDomainLogsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_domain_logs(self, request):
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
@@ -1897,15 +1899,15 @@
         @return: DescribeCdnDomainStagingConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_domain_staging_config_with_options(request, runtime)
 
     def describe_cdn_https_domain_list_with_options(self, request, runtime):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeCdnHttpsDomainListRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeCdnHttpsDomainListResponse
@@ -1935,15 +1937,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnHttpsDomainListResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_https_domain_list(self, request):
         """
-        >  The maximum number of times that each user can call this operation per second is 100.
+        > You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeCdnHttpsDomainListRequest
 
         @return: DescribeCdnHttpsDomainListResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -2029,15 +2031,15 @@
         @return: DescribeCdnRegionAndIspResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_region_and_isp_with_options(request, runtime)
 
     def describe_cdn_report_with_options(self, request, runtime):
         """
-        >  You can call this operation up to three times per second per account.
+        > You can call this operation up to three times per second per account.
         
 
         @param request: DescribeCdnReportRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeCdnReportResponse
@@ -2075,15 +2077,15 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnReportResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_report(self, request):
         """
-        >  You can call this operation up to three times per second per account.
+        > You can call this operation up to three times per second per account.
         
 
         @param request: DescribeCdnReportRequest
 
         @return: DescribeCdnReportResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -2323,16 +2325,16 @@
         @return: DescribeCdnSubListResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_sub_list_with_options(runtime)
 
     def describe_cdn_user_bill_history_with_options(self, request, runtime):
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - You can query billing history up to the last one month.
+        You can query billing history up to the last one month.
+        *   You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeCdnUserBillHistoryRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeCdnUserBillHistoryResponse
@@ -2360,16 +2362,16 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnUserBillHistoryResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_user_bill_history(self, request):
         """
-        - The maximum number of times that each user can call this operation per second is 100.
-        - You can query billing history up to the last one month.
+        You can query billing history up to the last one month.
+        *   You can call this operation up to 100 times per second per account.
         
 
         @param request: DescribeCdnUserBillHistoryRequest
 
         @return: DescribeCdnUserBillHistoryResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -2436,14 +2438,24 @@
 
         @return: DescribeCdnUserBillPredictionResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_user_bill_prediction_with_options(request, runtime)
 
     def describe_cdn_user_bill_type_with_options(self, request, runtime):
+        """
+        You can call this operation up to 100 times per second per account.
+        
+
+        @param request: DescribeCdnUserBillTypeRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeCdnUserBillTypeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.start_time):
             query['StartTime'] = request.start_time
         req = open_api_models.OpenApiRequest(
@@ -2462,14 +2474,22 @@
         )
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCdnUserBillTypeResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_cdn_user_bill_type(self, request):
+        """
+        You can call this operation up to 100 times per second per account.
+        
+
+        @param request: DescribeCdnUserBillTypeRequest
+
+        @return: DescribeCdnUserBillTypeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_user_bill_type_with_options(request, runtime)
 
     def describe_cdn_user_configs_with_options(self, request, runtime):
         """
         >  The maximum number of times that each user can call this operation per second is 30.
         
@@ -2695,16 +2715,16 @@
 
     def describe_cdn_waf_domain(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_cdn_waf_domain_with_options(request, runtime)
 
     def describe_certificate_info_by_idwith_options(self, request, runtime):
         """
-        > - The maximum number of times that each user can call this operation per second is 100.
-        - If a certificate is associated with a domain name but not enabled, the result of this operation shows that the certificate does not exist.
+        You can call this operation up to 100 times per second per account.
+        *   If a certificate is associated with a domain name but the certificate is not enabled, the result of this operation shows that the certificate does not exist.
         
 
         @param request: DescribeCertificateInfoByIDRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeCertificateInfoByIDResponse
@@ -2728,16 +2748,16 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeCertificateInfoByIDResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_certificate_info_by_id(self, request):
         """
-        > - The maximum number of times that each user can call this operation per second is 100.
-        - If a certificate is associated with a domain name but not enabled, the result of this operation shows that the certificate does not exist.
+        You can call this operation up to 100 times per second per account.
+        *   If a certificate is associated with a domain name but the certificate is not enabled, the result of this operation shows that the certificate does not exist.
         
 
         @param request: DescribeCertificateInfoByIDRequest
 
         @return: DescribeCertificateInfoByIDResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -2851,23 +2871,23 @@
         @return: DescribeDomainAverageResponseTimeResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_average_response_time_with_options(request, runtime)
 
     def describe_domain_bps_data_with_options(self, request, runtime):
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
@@ -2903,43 +2923,43 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainBpsDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_bps_data(self, request):
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
 
     def describe_domain_bps_data_by_layer_with_options(self, request, runtime):
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
@@ -2977,38 +2997,38 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainBpsDataByLayerResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_bps_data_by_layer(self, request):
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
 
     def describe_domain_bps_data_by_time_stamp_with_options(self, request, runtime):
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
@@ -3041,17 +3061,17 @@
             cdn_20180510_models.DescribeDomainBpsDataByTimeStampResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_bps_data_by_time_stamp(self, request):
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
@@ -3299,23 +3319,23 @@
         @return: DescribeDomainDetailDataByLayerResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_detail_data_by_layer_with_options(request, runtime)
 
     def describe_domain_hit_rate_data_with_options(self, request, runtime):
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
@@ -3347,23 +3367,23 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainHitRateDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_hit_rate_data(self, request):
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
@@ -3439,23 +3459,23 @@
         @return: DescribeDomainHttpCodeDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_http_code_data_with_options(request, runtime)
 
     def describe_domain_http_code_data_by_layer_with_options(self, request, runtime):
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
@@ -3493,23 +3513,23 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainHttpCodeDataByLayerResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_http_code_data_by_layer(self, request):
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
@@ -3568,14 +3588,28 @@
 
         @return: DescribeDomainISPDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_ispdata_with_options(request, runtime)
 
     def describe_domain_max_95bps_data_with_options(self, request, runtime):
+        """
+        The unit of the bandwidth is bit/s.
+        *   The time granularity of the queried data is 5 minutes.
+        *   You can query data in the last 90 days.
+        *   You can specify the StartTime and EndTime parameters, or the TimePoint and Cycle parameters to query the 95th percentile bandwidth data. If you specify the StartTime and EndTime parameters and the time range that is specified by these parameters is less than or equal to 24 hours, the 95th percentile bandwidth data on the day of the start time is returned. If the time range that is specified by these parameters is more than 24 hours, the 95th percentile bandwidth data in the month of the start time is returned. If you specify the TimePoint and Cycle parameters, the 95th percentile bandwidth data of the cycle is returned. If you do not specify parameters as previously mentioned, the 95th percentile bandwidth data in the last 24 hours is returned.
+        *   You can call this operation up to 100 times per second per account.
+        
+
+        @param request: DescribeDomainMax95BpsDataRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
+        @return: DescribeDomainMax95BpsDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cycle):
             query['Cycle'] = request.cycle
         if not UtilClient.is_unset(request.domain_name):
             query['DomainName'] = request.domain_name
         if not UtilClient.is_unset(request.end_time):
@@ -3600,14 +3634,26 @@
         )
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainMax95BpsDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_max_95bps_data(self, request):
+        """
+        The unit of the bandwidth is bit/s.
+        *   The time granularity of the queried data is 5 minutes.
+        *   You can query data in the last 90 days.
+        *   You can specify the StartTime and EndTime parameters, or the TimePoint and Cycle parameters to query the 95th percentile bandwidth data. If you specify the StartTime and EndTime parameters and the time range that is specified by these parameters is less than or equal to 24 hours, the 95th percentile bandwidth data on the day of the start time is returned. If the time range that is specified by these parameters is more than 24 hours, the 95th percentile bandwidth data in the month of the start time is returned. If you specify the TimePoint and Cycle parameters, the 95th percentile bandwidth data of the cycle is returned. If you do not specify parameters as previously mentioned, the 95th percentile bandwidth data in the last 24 hours is returned.
+        *   You can call this operation up to 100 times per second per account.
+        
+
+        @param request: DescribeDomainMax95BpsDataRequest
+
+        @return: DescribeDomainMax95BpsDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_max_95bps_data_with_options(request, runtime)
 
     def describe_domain_multi_usage_data_with_options(self, request, runtime):
         """
         >    If you do not set StartTime or EndTime, data collected within the last 10 minutes is queried.
         *   The maximum time range between StartTime and EndTime can be 1 hour.
@@ -3664,15 +3710,15 @@
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_multi_usage_data_with_options(request, runtime)
 
     def describe_domain_path_data_with_options(self, request, runtime):
         """
         This operation is available only to users that are on the whitelist. If the daily peak bandwidth value of your workloads reaches 10 Gbit/s, you can [submit a ticket](https://workorder-intl.console.aliyun.com/?spm=5176.2020520001.aliyun_topbar.18.dbd44bd3e4f845#/ticket/createIndex) to apply to be included in the whitelist.
-        *   The maximum number of times that each user can call this operation per second is 6,000.
+        *   You can call this API operation up to 6,000 times per second per account.
         *   Data collection by directory is available only to specified domain names within your Alibaba Cloud account. It cannot be enabled for all domain names within your Alibaba Cloud account.
         *   The average size of the files that belong to the domain name must be larger than 1 MB.
         *   The number of directories specified for a single domain name cannot exceed 100. If the number of directories exceeds 100, the data accuracy reduces.
         *   If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
         *   You can query data collected within the last 30 days.
         
 
@@ -3702,15 +3748,15 @@
             cdn_20180510_models.DescribeDomainPathDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_path_data(self, request):
         """
         This operation is available only to users that are on the whitelist. If the daily peak bandwidth value of your workloads reaches 10 Gbit/s, you can [submit a ticket](https://workorder-intl.console.aliyun.com/?spm=5176.2020520001.aliyun_topbar.18.dbd44bd3e4f845#/ticket/createIndex) to apply to be included in the whitelist.
-        *   The maximum number of times that each user can call this operation per second is 6,000.
+        *   You can call this API operation up to 6,000 times per second per account.
         *   Data collection by directory is available only to specified domain names within your Alibaba Cloud account. It cannot be enabled for all domain names within your Alibaba Cloud account.
         *   The average size of the files that belong to the domain name must be larger than 1 MB.
         *   The number of directories specified for a single domain name cannot exceed 100. If the number of directories exceeds 100, the data accuracy reduces.
         *   If you do not set StartTime or EndTime, data collected within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
         *   You can query data collected within the last 30 days.
         
 
@@ -3773,23 +3819,23 @@
         @return: DescribeDomainPvDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_pv_data_with_options(request, runtime)
 
     def describe_domain_qps_data_with_options(self, request, runtime):
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
@@ -3825,43 +3871,43 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainQpsDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_qps_data(self, request):
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
 
     def describe_domain_qps_data_by_layer_with_options(self, request, runtime):
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
@@ -3899,43 +3945,42 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainQpsDataByLayerResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_qps_data_by_layer(self, request):
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
 
     def describe_domain_real_time_bps_data_with_options(self, request, runtime):
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
@@ -3959,44 +4004,43 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainRealTimeBpsDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_real_time_bps_data(self, request):
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
 
     def describe_domain_real_time_byte_hit_rate_data_with_options(self, request, runtime):
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
@@ -4020,24 +4064,24 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainRealTimeByteHitRateDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_real_time_byte_hit_rate_data(self, request):
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
@@ -4087,23 +4131,23 @@
         @return: DescribeDomainRealTimeDetailDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_real_time_detail_data_with_options(request, runtime)
 
     def describe_domain_real_time_http_code_data_with_options(self, request, runtime):
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
@@ -4137,43 +4181,43 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainRealTimeHttpCodeDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_real_time_http_code_data(self, request):
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
 
     def describe_domain_real_time_qps_data_with_options(self, request, runtime):
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
@@ -4197,23 +4241,23 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainRealTimeQpsDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_real_time_qps_data(self, request):
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
@@ -4281,23 +4325,23 @@
         @return: DescribeDomainRealTimeReqHitRateDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_real_time_req_hit_rate_data_with_options(request, runtime)
 
     def describe_domain_real_time_src_bps_data_with_options(self, request, runtime):
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
@@ -4327,43 +4371,43 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainRealTimeSrcBpsDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_real_time_src_bps_data(self, request):
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
 
     def describe_domain_real_time_src_http_code_data_with_options(self, request, runtime):
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
@@ -4397,43 +4441,43 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainRealTimeSrcHttpCodeDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_real_time_src_http_code_data(self, request):
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
 
     def describe_domain_real_time_src_traffic_data_with_options(self, request, runtime):
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
@@ -4463,43 +4507,43 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainRealTimeSrcTrafficDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_real_time_src_traffic_data(self, request):
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
 
     def describe_domain_real_time_traffic_data_with_options(self, request, runtime):
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
@@ -4533,23 +4577,23 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainRealTimeTrafficDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_real_time_traffic_data(self, request):
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
@@ -4653,23 +4697,23 @@
         @return: DescribeDomainRegionDataResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_region_data_with_options(request, runtime)
 
     def describe_domain_req_hit_rate_data_with_options(self, request, runtime):
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
@@ -4701,43 +4745,43 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainReqHitRateDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_req_hit_rate_data(self, request):
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
 
     def describe_domain_src_bps_data_with_options(self, request, runtime):
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
@@ -4769,43 +4813,43 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainSrcBpsDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_src_bps_data(self, request):
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
 
     def describe_domain_src_http_code_data_with_options(self, request, runtime):
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
@@ -4837,43 +4881,43 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainSrcHttpCodeDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_src_http_code_data(self, request):
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
 
     def describe_domain_src_qps_data_with_options(self, request, runtime):
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
@@ -4905,23 +4949,23 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainSrcQpsDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_src_qps_data(self, request):
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
@@ -4981,23 +5025,23 @@
         @return: DescribeDomainSrcTopUrlVisitResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_src_top_url_visit_with_options(request, runtime)
 
     def describe_domain_src_traffic_data_with_options(self, request, runtime):
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
@@ -5029,23 +5073,23 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainSrcTrafficDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_src_traffic_data(self, request):
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
@@ -5169,18 +5213,20 @@
         @return: DescribeDomainTopReferVisitResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_top_refer_visit_with_options(request, runtime)
 
     def describe_domain_top_url_visit_with_options(self, request, runtime):
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
@@ -5212,38 +5258,40 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainTopUrlVisitResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_top_url_visit(self, request):
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
 
     def describe_domain_traffic_data_with_options(self, request, runtime):
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
@@ -5279,43 +5327,41 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainTrafficDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_traffic_data(self, request):
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
 
     def describe_domain_usage_data_with_options(self, request, runtime):
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
@@ -5355,38 +5401,37 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainUsageDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_usage_data(self, request):
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
 
     def describe_domain_uv_data_with_options(self, request, runtime):
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
@@ -5416,18 +5461,19 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainUvDataResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domain_uv_data(self, request):
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
@@ -5481,16 +5527,17 @@
         @return: DescribeDomainsBySourceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_domains_by_source_with_options(request, runtime)
 
     def describe_domains_usage_by_day_with_options(self, request, runtime):
         """
-        > - If you do not set StartTime or EndTime, data within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
-        > - You can query the monitoring data of a specific accelerated domain name or all accelerated domain names that belong to your Alibaba Cloud account.
+        You can call this operation up to 10 times per second per account.
+        *   If you do not set StartTime or EndTime, data within the last 24 hours is queried. If you set both StartTime and EndTime, data within the specified time range is queried.
+        *   You can query the monitoring data of a specific accelerated domain name or all accelerated domain names that belong to your Alibaba Cloud account.
         
 
         @param request: DescribeDomainsUsageByDayRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeDomainsUsageByDayResponse
@@ -5520,16 +5567,17 @@
         return TeaCore.from_map(
             cdn_20180510_models.DescribeDomainsUsageByDayResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_domains_usage_by_day(self, request):
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
@@ -5878,15 +5926,15 @@
     def describe_preload_detail_by_id(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_preload_detail_by_id_with_options(request, runtime)
 
     def describe_range_data_by_locate_and_isp_service_with_options(self, request, runtime):
         """
         The data is collected every 5 minutes.
-        *   The maximum number of times that each user can call this operation per second is 20.
+        *   You can call this operation up to 20 times per second per account.
         
 
         @param request: DescribeRangeDataByLocateAndIspServiceRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: DescribeRangeDataByLocateAndIspServiceResponse
@@ -5921,15 +5969,15 @@
             cdn_20180510_models.DescribeRangeDataByLocateAndIspServiceResponse(),
             self.call_api(params, req, runtime)
         )
 
     def describe_range_data_by_locate_and_isp_service(self, request):
         """
         The data is collected every 5 minutes.
-        *   The maximum number of times that each user can call this operation per second is 20.
+        *   You can call this operation up to 20 times per second per account.
         
 
         @param request: DescribeRangeDataByLocateAndIspServiceRequest
 
         @return: DescribeRangeDataByLocateAndIspServiceResponse
         """
         runtime = util_models.RuntimeOptions()
@@ -7239,23 +7287,23 @@
         runtime = util_models.RuntimeOptions()
         return self.publish_staging_config_to_production_with_options(request, runtime)
 
     def push_object_cache_with_options(self, request, runtime):
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
@@ -7293,46 +7341,47 @@
             self.call_api(params, req, runtime)
         )
 
     def push_object_cache(self, request):
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
 
     def refresh_object_caches_with_options(self, request, runtime):
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
@@ -7366,24 +7415,25 @@
             self.call_api(params, req, runtime)
         )
 
     def refresh_object_caches(self, request):
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
```

### Comparing `alibabacloud_cdn20180510_py2-1.2.6/alibabacloud_cdn20180510/models.py` & `alibabacloud_cdn20180510_py2-1.2.7/alibabacloud_cdn20180510/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1084,15 +1084,15 @@
             temp_model = BatchStartCdnDomainResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class BatchStopCdnDomainRequest(TeaModel):
     def __init__(self, domain_names=None, owner_id=None, security_token=None):
-        # You can specify one or more domain names and separate them with commas (,).
+        # The names of the accelerated domain names. You can specify one or more domain names in each request. Separate multiple domain names with commas (,).
         self.domain_names = domain_names  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
 
     def validate(self):
         pass
 
@@ -1578,30 +1578,30 @@
         return self
 
 
 class CreateCdnSubTaskRequest(TeaModel):
     def __init__(self, domain_name=None, report_ids=None):
         # The domain names to be tracked. Separate multiple domain names with commas (,). You can specify up to 500 domain names. If you want to specify more than 500 domain names, [submit a ticket](https://workorder-intl.console.aliyun.com/?spm=5176.2020520001.aliyun_topbar.18.dbd44bd3e4f845#/ticket/createIndex).
         # 
-        # >  If you do not specify a domain name, the custom operations reports are created for all domain names that belong to your Alibaba Cloud account.
+        # > If you do not specify a domain name, the custom operations report is created for all domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name  # type: str
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
         self.report_ids = report_ids  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateCdnSubTaskRequest, self).to_map()
@@ -1895,40 +1895,40 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateUsageDetailDataExportTaskRequest(TeaModel):
     def __init__(self, domain_names=None, end_time=None, group=None, language=None, start_time=None, task_name=None,
                  type=None):
-        # The accelerated domain names based on which the resource usage details are generated. If you do not specify a domain name group, resource usage details are exported based on this parameter.
+        # The domain names. If you do not specify the Group parameter, resource usage details of these domain names are exported.
         # 
-        # If you do not set this parameter, resource usage details are exported based on user accounts.
+        # If you do not specify this parameter, resource usage details are exported based on accounts.
         self.domain_names = domain_names  # type: str
         # The end of the time range to query.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The group of accelerated domain names based on which the resource usage details are generated. If you set this parameter, ignore the **DomainNames** parameter.
+        # The domain name group. If you specify this parameter, the **DomainNames** parameter is ignored.
         self.group = group  # type: str
-        # The language of the exported file. Valid values:
+        # The language in which you want to export the file. Valid values:
         # 
         # *   **zh-cn**: Chinese. This is the default value.
         # *   **en-us**: English
         self.language = language  # type: str
         # The beginning of the time range to query.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
         # The name of the task.
         self.task_name = task_name  # type: str
-        # The type of content based on which the data is generated. Valid values:
+        # The type of resource usage data to query. Valid values:
         # 
-        # *   **flow**: network traffic and bandwidth
+        # *   **flow**: traffic and bandwidth
         # *   **vas**: requests
         self.type = type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1970,19 +1970,19 @@
         if m.get('Type') is not None:
             self.type = m.get('Type')
         return self
 
 
 class CreateUsageDetailDataExportTaskResponseBody(TeaModel):
     def __init__(self, end_time=None, request_id=None, start_time=None, task_id=None):
-        # The end of the time range that was queried.
+        # The end of the time range for which the data was queried.
         self.end_time = end_time  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range that was queried.
+        # The beginning of the time range for which the data was queried.
         self.start_time = start_time  # type: str
         # The ID of the task.
         self.task_id = task_id  # type: str
 
     def validate(self):
         pass
 
@@ -2054,24 +2054,24 @@
         return self
 
 
 class CreateUserUsageDataExportTaskRequest(TeaModel):
     def __init__(self, end_time=None, language=None, start_time=None, task_name=None):
         # The end of the time range to query. The end time must be later than the start time.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.end_time = end_time  # type: str
-        # The language of the exported file.
+        # The language in which you want to export the file. Default value: zh-cn. Valid values:
         # 
-        # *   **zh-cn**: Chinese. This is the default value.
-        # *   **en-us**: English.
+        # *   **zh-cn**: Chinese
+        # *   **en-us**: English
         self.language = language  # type: str
-        # The start of the time range to query. The time interval at which the specified data is collected is five minutes.
+        # The start of the time range to query. The data is collected every 5 minutes.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
         # The name of the task.
         self.task_name = task_name  # type: str
 
     def validate(self):
         pass
 
@@ -2102,19 +2102,19 @@
         if m.get('TaskName') is not None:
             self.task_name = m.get('TaskName')
         return self
 
 
 class CreateUserUsageDataExportTaskResponseBody(TeaModel):
     def __init__(self, end_time=None, request_id=None, start_time=None, task_id=None):
-        # The end of the time range where the QPS data was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
         # The ID of the task.
         self.task_id = task_id  # type: str
 
     def validate(self):
         pass
 
@@ -3924,20 +3924,20 @@
         return self
 
 
 class DescribeCdnDomainByCertificateRequest(TeaModel):
     def __init__(self, sslpub=None, sslstatus=None):
         # The public key of the SSL certificate. You must encode the public key in Base64 and then call the encodeURIComponent function to encode the public key again.
         # 
-        # The public key must be in the PEM format.
+        # The public key must be in the Privacy-Enhanced Mail (PEM) format.
         self.sslpub = sslpub  # type: str
         # Specifies whether the domain name list to return contains only domain names with HTTPS enabled or disabled.
         # 
-        # - true: The domain name list contains only domain names with HTTPS enabled.
-        # - false: The domain name list contains only domain names with HTTPS disabled.
+        # *   true: The list contains only domain names with HTTPS enabled.
+        # *   false: The list contains only domain names with HTTPS disabled.
         self.sslstatus = sslstatus  # type: bool
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnDomainByCertificateRequest, self).to_map()
@@ -3964,32 +3964,32 @@
     def __init__(self, cert_ca_is_legacy=None, cert_expire_time=None, cert_expired=None, cert_start_time=None,
                  cert_subject_common_name=None, cert_type=None, domain_list=None, domain_names=None, issuer=None):
         # Indicates whether the SSL certificate is obsolete. Valid values:
         # 
         # *   **yes**: The SSL certificate is obsolete.
         # *   **no**: The SSL certificate is working as expected.
         self.cert_ca_is_legacy = cert_ca_is_legacy  # type: str
-        # The time when the SSL certificate expires.
+        # The time at which the certificate expires.
         self.cert_expire_time = cert_expire_time  # type: str
         # Indicates whether the SSL certificate is expired. Valid values:
         # 
         # *   **yes**: The SSL certificate is expired.
         # *   **no**: The SSL certificate is not expired.
         self.cert_expired = cert_expired  # type: str
-        # The time when the SSL certificate became effective.
+        # The time at which the certificate became effective.
         self.cert_start_time = cert_start_time  # type: str
         # The name of the SSL certificate owner.
         self.cert_subject_common_name = cert_subject_common_name  # type: str
-        # The type of the certificate. Valid responses: **RSA**, **DSA**, and **ECDSA**.
+        # The type of the certificate. Valid values: **RSA**, **DSA**, and **ECDSA**.
         self.cert_type = cert_type  # type: str
-        # If a value is returned, the value matches the SSL certificate. Multiple domain names are separated with commas (,).
+        # If a value is returned, the value matches the SSL certificate. Multiple domain names are separated by commas (,).
         self.domain_list = domain_list  # type: str
-        # The domain names (DNS fields) that match the SSL certificate. Multiple domain names are separated with commas (,).
+        # The domain names (DNS fields) that match the SSL certificate. Multiple domain names are separated by commas (,).
         self.domain_names = domain_names  # type: str
-        # The certificate authority that issued the SSL certificate.
+        # The certificate authority (CA) that issued the certificate.
         self.issuer = issuer  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnDomainByCertificateResponseBodyCertInfosCertInfo, self).to_map()
@@ -4070,15 +4070,15 @@
                 temp_model = DescribeCdnDomainByCertificateResponseBodyCertInfosCertInfo()
                 self.cert_info.append(temp_model.from_map(k))
         return self
 
 
 class DescribeCdnDomainByCertificateResponseBody(TeaModel):
     def __init__(self, cert_infos=None, request_id=None):
-        # The information about the SSL certificate.
+        # The certificate information.
         self.cert_infos = cert_infos  # type: DescribeCdnDomainByCertificateResponseBodyCertInfos
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.cert_infos:
             self.cert_infos.validate()
@@ -4722,29 +4722,29 @@
             temp_model = DescribeCdnDomainDetailResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCdnDomainLogsRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, page_number=None, page_size=None, start_time=None):
-        # The accelerated domain name. You can specify only one domain name.
+        # The domain name. You can specify only one domain name.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
         # The number of the page to return. Pages start from page **1**.
         self.page_number = page_number  # type: long
         # The number of entries to return on each page. Default value: **300**. Maximum value: **1000**. Valid values: **1** to **1000**.
         self.page_size = page_size  # type: long
         # The beginning of the time range to query.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnDomainLogsRequest, self).to_map()
@@ -4777,23 +4777,23 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeCdnDomainLogsResponseBodyDomainLogDetailsDomainLogDetailLogInfosLogInfoDetail(TeaModel):
     def __init__(self, end_time=None, log_name=None, log_path=None, log_size=None, start_time=None):
-        # The end of the time range where the QPS data was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The name of the log file.
         self.log_name = log_name  # type: str
         # The path of the log file.
         self.log_path = log_path  # type: str
         # The size of the log file.
         self.log_size = log_size  # type: long
-        # The start of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnDomainLogsResponseBodyDomainLogDetailsDomainLogDetailLogInfosLogInfoDetail, self).to_map()
@@ -4899,17 +4899,17 @@
 
 class DescribeCdnDomainLogsResponseBodyDomainLogDetailsDomainLogDetail(TeaModel):
     def __init__(self, domain_name=None, log_count=None, log_infos=None, page_infos=None):
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
         # The total number of entries returned on the current page.
         self.log_count = log_count  # type: long
-        # The detailed log information, which is indicated by the LogInfoDetail parameter.
+        # A set of LogInfoDetail data.
         self.log_infos = log_infos  # type: DescribeCdnDomainLogsResponseBodyDomainLogDetailsDomainLogDetailLogInfos
-        # The detailed log information, which is indicated by the PageInfoDetail parameter.
+        # A set of PageInfoDetail data.
         self.page_infos = page_infos  # type: DescribeCdnDomainLogsResponseBodyDomainLogDetailsDomainLogDetailPageInfos
 
     def validate(self):
         if self.log_infos:
             self.log_infos.validate()
         if self.page_infos:
             self.page_infos.validate()
@@ -4975,15 +4975,15 @@
                 temp_model = DescribeCdnDomainLogsResponseBodyDomainLogDetailsDomainLogDetail()
                 self.domain_log_detail.append(temp_model.from_map(k))
         return self
 
 
 class DescribeCdnDomainLogsResponseBody(TeaModel):
     def __init__(self, domain_log_details=None, request_id=None):
-        # The detailed log information, which is indicated by the DomainLogDetail parameter.
+        # A set of DomainLogDetail data.
         self.domain_log_details = domain_log_details  # type: DescribeCdnDomainLogsResponseBodyDomainLogDetails
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.domain_log_details:
             self.domain_log_details.validate()
@@ -5257,19 +5257,19 @@
             temp_model = DescribeCdnDomainStagingConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCdnHttpsDomainListRequest(TeaModel):
     def __init__(self, keyword=None, page_number=None, page_size=None):
-        # The keyword used for search.
+        # The keyword that is used to search for certificates.
         self.keyword = keyword  # type: str
         # The number of the page to return. Valid values: **1** to **100000**.
         self.page_number = page_number  # type: int
-        # The maximum number of entries to return on each page. Default value: **20**.
+        # The number of entries to return on each page. Default value: **20**.
         self.page_size = page_size  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnHttpsDomainListRequest, self).to_map()
@@ -5295,36 +5295,36 @@
             self.page_size = m.get('PageSize')
         return self
 
 
 class DescribeCdnHttpsDomainListResponseBodyCertInfosCertInfo(TeaModel):
     def __init__(self, cert_common_name=None, cert_expire_time=None, cert_name=None, cert_start_time=None,
                  cert_status=None, cert_type=None, cert_update_time=None, domain_name=None):
-        # The Common Name on the SSL certificate.
+        # The returned primary domain name of the certificate.
         self.cert_common_name = cert_common_name  # type: str
-        # The time when the SSL certificate expires.
+        # The time at which the certificate expires.
         self.cert_expire_time = cert_expire_time  # type: str
-        # The name of the SSL certificate.
+        # The name of the certificate.
         self.cert_name = cert_name  # type: str
-        # The time when the SSL certificate became effective.
+        # The time at which the certificate became effective.
         self.cert_start_time = cert_start_time  # type: str
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
         self.cert_status = cert_status  # type: str
-        # The type of the SSL certificate. Valid values:
+        # The type of the certificate.
         # 
-        # *   **free**: a free SSL certificate.
-        # *   **cas**: an SSL certificate purchased from Alibaba Cloud SSL Certificates Service.
-        # *   **upload**: a user uploaded certificate.
+        # *   **free**: a free certificate.
+        # *   **cas**: a certificate that is purchased from Alibaba Cloud SSL Certificates Service.
+        # *   **upload**: a certificate that is uploaded by the user.
         self.cert_type = cert_type  # type: str
-        # The time when the certificate was renewed.
+        # The time at which the certificate was updated.
         self.cert_update_time = cert_update_time  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
 
     def validate(self):
         pass
 
@@ -5403,15 +5403,15 @@
                 temp_model = DescribeCdnHttpsDomainListResponseBodyCertInfosCertInfo()
                 self.cert_info.append(temp_model.from_map(k))
         return self
 
 
 class DescribeCdnHttpsDomainListResponseBody(TeaModel):
     def __init__(self, cert_infos=None, request_id=None, total_count=None):
-        # The information about the SSL certificate.
+        # The information about the certificate.
         self.cert_infos = cert_infos  # type: DescribeCdnHttpsDomainListResponseBodyCertInfos
         # The ID of the request.
         self.request_id = request_id  # type: str
         # The total number of entries returned.
         self.total_count = total_count  # type: int
 
     def validate(self):
@@ -6690,21 +6690,21 @@
             temp_model = DescribeCdnSubListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCdnUserBillHistoryRequest(TeaModel):
     def __init__(self, end_time=None, start_time=None):
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # The end of the time range to query. The end time must be later than the start time.
+        # The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # The minimum data collection interval is 5 minutes.
+        # The minimum data granularity is 5 minutes.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnUserBillHistoryRequest, self).to_map()
@@ -6729,25 +6729,25 @@
 
 class DescribeCdnUserBillHistoryResponseBodyBillHistoryDataBillHistoryDataItemBillingDataBillingDataItem(TeaModel):
     def __init__(self, bandwidth=None, cdn_region=None, charge_type=None, count=None, flow=None):
         # The bandwidth. Unit: bit/s.
         self.bandwidth = bandwidth  # type: float
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
         self.cdn_region = cdn_region  # type: str
-        # The billable item. Valid values:
+        # The billing method. Valid values:
         # 
         # *   **StaticHttp**: static HTTP requests
         # *   **DynamicHttp**: dynamic HTTP requests
         # *   **DynamicHttps**: dynamic HTTPS requests
         self.charge_type = charge_type  # type: str
         # The number of requests.
         self.count = count  # type: float
@@ -6822,15 +6822,15 @@
         return self
 
 
 class DescribeCdnUserBillHistoryResponseBodyBillHistoryDataBillHistoryDataItem(TeaModel):
     def __init__(self, bill_time=None, bill_type=None, billing_data=None, dimension=None):
         # The beginning of the time range that was queried.
         self.bill_time = bill_time  # type: str
-        # The billing method.
+        # The metering method.
         self.bill_type = bill_type  # type: str
         # The billable items.
         self.billing_data = billing_data  # type: DescribeCdnUserBillHistoryResponseBodyBillHistoryDataBillHistoryDataItemBillingData
         # The dimension.
         self.dimension = dimension  # type: str
 
     def validate(self):
@@ -7201,25 +7201,21 @@
             temp_model = DescribeCdnUserBillPredictionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCdnUserBillTypeRequest(TeaModel):
     def __init__(self, end_time=None, start_time=None):
-        # The end of the time range that was queried.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # Example: 2016-10-20T04:00:00Z.
+        # The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The start of the time range that was queried.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # Example: 2016-10-20T04:00:00Z.
+        # The minimum data granularity is 5 minutes.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnUserBillTypeRequest, self).to_map()
@@ -7241,19 +7237,49 @@
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeCdnUserBillTypeResponseBodyBillTypeDataBillTypeDataItem(TeaModel):
     def __init__(self, bill_type=None, billing_cycle=None, dimension=None, end_time=None, product=None,
                  start_time=None):
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
         self.bill_type = bill_type  # type: str
+        # The billing cycle.
         self.billing_cycle = billing_cycle  # type: str
+        # The dimension. Valid values:
+        # 
+        # *   flow: traffic and bandwidth
+        # *   vas: value-added services (HTTPS and requests for dynamic content)
+        # *   quic: the number of QUIC requests
+        # *   websocket: the WebSocket communications protocol
+        # *   rtlog2sls: log entries delivered to Log Service in real time
+        # *   stationflow: traffic over the internal network
         self.dimension = dimension  # type: str
+        # The time when the metering method ended.
         self.end_time = end_time  # type: str
+        # The name of the product.
         self.product = product  # type: str
+        # The time when the metering method started.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCdnUserBillTypeResponseBodyBillTypeDataBillTypeDataItem, self).to_map()
@@ -7322,14 +7348,15 @@
                 temp_model = DescribeCdnUserBillTypeResponseBodyBillTypeDataBillTypeDataItem()
                 self.bill_type_data_item.append(temp_model.from_map(k))
         return self
 
 
 class DescribeCdnUserBillTypeResponseBody(TeaModel):
     def __init__(self, bill_type_data=None, request_id=None):
+        # Details about the metering methods returned.
         self.bill_type_data = bill_type_data  # type: DescribeCdnUserBillTypeResponseBodyBillTypeData
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.bill_type_data:
             self.bill_type_data.validate()
@@ -8449,15 +8476,15 @@
             temp_model = DescribeCdnWafDomainResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeCertificateInfoByIDRequest(TeaModel):
     def __init__(self, cert_id=None):
-        # The ID of the SSL certificate. You can query only one certificate in each call.
+        # The ID of the certificate. You can query only one certificate in each call.
         self.cert_id = cert_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeCertificateInfoByIDRequest, self).to_map()
@@ -8475,29 +8502,29 @@
             self.cert_id = m.get('CertId')
         return self
 
 
 class DescribeCertificateInfoByIDResponseBodyCertInfosCertInfo(TeaModel):
     def __init__(self, cert_expire_time=None, cert_id=None, cert_name=None, cert_type=None, create_time=None,
                  domain_list=None, https_crt=None):
-        # The expiration time of the certificate.
+        # The time at which the certificate expires.
         self.cert_expire_time = cert_expire_time  # type: str
         # The ID of the certificate.
         self.cert_id = cert_id  # type: str
         # The name of the certificate.
         self.cert_name = cert_name  # type: str
         # The type of the certificate.
         # 
-        # *   free: a free certificate.
-        # *   cas: a certificate purchased by using Certificate Management Service.
-        # *   upload: a user-uploaded certificate.
+        # *   free: a free certificate
+        # *   cas: a certificate purchased by using Certificate Management Service
+        # *   upload: a user-uploaded certificate
         self.cert_type = cert_type  # type: str
         # The time when the certificate became effective.
         self.create_time = create_time  # type: str
-        # A list of domain names that use the certificate.
+        # The domain names that use the certificate.
         self.domain_list = domain_list  # type: str
         # The content of the certificate.
         self.https_crt = https_crt  # type: str
 
     def validate(self):
         pass
 
@@ -8988,35 +9015,35 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainBpsDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, isp_name_en=None, location_name_en=None,
                  start_time=None):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.  
+        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # By default, this operation queries the bandwidth values during back-to-origin routing for all accelerated domain names that belong to your Alibaba Cloud account.
+        # By default, this operation queries bandwidth data for all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.  
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The time interval between the data entries. Unit: seconds. 
+        # The time granularity of the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval  # type: str
-        # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service. You can call the [DescribeCdnRegionAndIsp](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/describecdnregionandisp) operation to query ISP names.  
+        # The name of the Internet service provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
         # 
-        # If you do not set this parameter, all ISPs are queried.
+        # If you do not set this parameter, data of all ISPs is queried.
         self.isp_name_en = isp_name_en  # type: str
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](https://www.alibabacloud.com/help/en/alibaba-cloud-cdn/latest/describecdnregionandisp) operation to query the most recent region list.  
+        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
         # 
-        # If you do not set this parameter, the bandwidth monitoring data of the accelerated domain names in all regions is returned.
+        # If you do not specify a region, data in all regions is queried.
         self.location_name_en = location_name_en  # type: str
-        # The start of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainBpsDataRequest, self).to_map()
@@ -9054,27 +9081,27 @@
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainBpsDataResponseBodyBpsDataPerIntervalDataModule(TeaModel):
     def __init__(self, domestic_value=None, https_domestic_value=None, https_overseas_value=None, https_value=None,
                  overseas_value=None, time_stamp=None, value=None):
-        # The bandwidth values in the Chinese mainland. When the bandwidth data is queried by ISP, no value is returned.
+        # The bandwidth value in the Chinese mainland. When the bandwidth data is queried by ISP, this parameter is empty.
         self.domestic_value = domestic_value  # type: str
-        # The bandwidth values for HTTPS requests in the Chinese mainland. When the bandwidth data is queried by ISP, no value is returned.
+        # The bandwidth data for HTTPS requests in the Chinese mainland. When the bandwidth data is queried by ISP, this parameter is empty.
         self.https_domestic_value = https_domestic_value  # type: str
-        # The bandwidth values for HTTPS requests in regions outside the Chinese mainland. When the bandwidth data is queried by ISP, no value is returned.
+        # The bandwidth data for HTTPS requests in regions outside the Chinese mainland. When the bandwidth data is queried by ISP, this parameter is empty.
         self.https_overseas_value = https_overseas_value  # type: str
-        # The bandwidth values for HTTPS requests. Unit: bit/s.
+        # The bandwidth value for HTTPS requests. Unit: bit/s.
         self.https_value = https_value  # type: str
-        # The bandwidth values in regions outside the Chinese mainland. When the bandwidth data is queried by ISP, no value is returned.
+        # The bandwidth data in regions outside the Chinese mainland. When the bandwidth data is queried by ISP, this parameter is empty.
         self.overseas_value = overseas_value  # type: str
         # The timestamp of the data returned.
         self.time_stamp = time_stamp  # type: str
-        # The bandwidth value. Unit: bit/s.
+        # The bandwidth. Unit: bit/s.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainBpsDataResponseBodyBpsDataPerIntervalDataModule, self).to_map()
@@ -9148,29 +9175,29 @@
                 self.data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainBpsDataResponseBody(TeaModel):
     def __init__(self, bps_data_per_interval=None, data_interval=None, domain_name=None, end_time=None,
                  isp_name_en=None, location_name_en=None, request_id=None, start_time=None):
-        # The bandwidth values collected at each interval.
+        # The list of bandwidth data entries returned at each interval.
         self.bps_data_per_interval = bps_data_per_interval  # type: DescribeDomainBpsDataResponseBodyBpsDataPerInterval
-        # The time interval between the returned entries. Unit: seconds.
+        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
-        # The name of the ISP for your Alibaba Cloud CDN service.
+        # The name of the ISP.
         self.isp_name_en = isp_name_en  # type: str
         # The name of the region.
         self.location_name_en = location_name_en  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.bps_data_per_interval:
             self.bps_data_per_interval.validate()
 
     def to_map(self):
@@ -9257,39 +9284,39 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainBpsDataByLayerRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, isp_name_en=None, layer=None,
                  location_name_en=None, start_time=None):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # >  If you do not specify an accelerated domain name, the bandwidth data of all the accelerated domain names that belong to your Alibaba Cloud account is queried.
+        # > If you do not specify this parameter, the bandwidth data about all accelerated domain names that belong to your Alibaba Cloud account is queried.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The time interval between the data entries. Unit: seconds.
+        # The time granularity of the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval  # type: str
-        # The name of the Internet service provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent ISP list. If you do not specify an ISP, data of all ISPs is queried.
+        # The name of the Internet service provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~DescribeCdnRegionAndIsp~~) operation to query ISPs. If you do not specify an ISP, data of all ISPs is queried.
         self.isp_name_en = isp_name_en  # type: str
-        # The layers at which you want to query the bandwidth data. Valid values:
+        # The layer at which you want to query the bandwidth data. Valid values:
         # 
         # *   Network layer: **IPv4** and **IPv6**.
         # *   Application layer: **http**, **https**, and **quic**.
         # *   **all**: specifies that both the network and application layers are included.
         # 
         # Default value: **all**.
         self.layer = layer  # type: str
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list. If you do not specify a region, data in all regions is queried.
+        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~DescribeCdnRegionAndIsp~~) operation to query regions. If you do not specify a region, data in all regions is queried.
         self.location_name_en = location_name_en  # type: str
         # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
@@ -9334,15 +9361,15 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainBpsDataByLayerResponseBodyBpsDataIntervalDataModule(TeaModel):
     def __init__(self, time_stamp=None, traffic_value=None, value=None):
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
         # The total amount of network traffic. Unit: bytes.
         self.traffic_value = traffic_value  # type: str
         # The peak bandwidth value. Unit: bit/s.
         self.value = value  # type: str
 
     def validate(self):
@@ -9403,15 +9430,15 @@
                 temp_model = DescribeDomainBpsDataByLayerResponseBodyBpsDataIntervalDataModule()
                 self.data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainBpsDataByLayerResponseBody(TeaModel):
     def __init__(self, bps_data_interval=None, data_interval=None, request_id=None):
-        # The number of bytes per second collected at each time interval.
+        # The data returned at each time interval.
         self.bps_data_interval = bps_data_interval  # type: DescribeDomainBpsDataByLayerResponseBodyBpsDataInterval
         # The time interval between the data entries. Unit: seconds.
         self.data_interval = data_interval  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
@@ -9481,27 +9508,27 @@
             temp_model = DescribeDomainBpsDataByLayerResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainBpsDataByTimeStampRequest(TeaModel):
     def __init__(self, domain_name=None, isp_names=None, location_names=None, time_point=None):
-        # The accelerated domain name. You can specify only one domain name in each query.
+        # The accelerated domain name. You can specify only one domain name in each request.
         self.domain_name = domain_name  # type: str
-        # The names of the Internet service providers (ISPs). Separate multiple ISP names with commas (,).
+        # The names of the Internet service providers (ISPs). Separate multiple ISPs with commas (,).
         # 
         # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
         self.isp_names = isp_names  # type: str
-        # The names of the regions. Separate multiple regions with commas (,).
+        # The regions. Separate multiple regions with commas (,).
         # 
         # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
         self.location_names = location_names  # type: str
-        # The beginning of the time range that was queried. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The point in time to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # The data is collected at an interval of five minutes.
+        # > The data is collected every 5 minutes.
         self.time_point = time_point  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainBpsDataByTimeStampRequest, self).to_map()
@@ -9532,19 +9559,19 @@
         return self
 
 
 class DescribeDomainBpsDataByTimeStampResponseBodyBpsDataListBpsDataModel(TeaModel):
     def __init__(self, bps=None, isp_name=None, location_name=None, time_stamp=None):
         # The bandwidth value.
         self.bps = bps  # type: long
-        # The name of the ISP for your Content Delivery Network (CDN) service.
+        # The name of the ISP.
         self.isp_name = isp_name  # type: str
         # The name of the region.
         self.location_name = location_name  # type: str
-        # The timestamp of the data.
+        # The timestamp of the data returned.
         self.time_stamp = time_stamp  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainBpsDataByTimeStampResponseBodyBpsDataListBpsDataModel, self).to_map()
@@ -9605,21 +9632,21 @@
                 temp_model = DescribeDomainBpsDataByTimeStampResponseBodyBpsDataListBpsDataModel()
                 self.bps_data_model.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainBpsDataByTimeStampResponseBody(TeaModel):
     def __init__(self, bps_data_list=None, domain_name=None, request_id=None, time_stamp=None):
-        # A list of bandwidth values queried by ISP and region.
+        # A list of bandwidth values by ISP and region.
         self.bps_data_list = bps_data_list  # type: DescribeDomainBpsDataByTimeStampResponseBodyBpsDataList
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The timestamp of the data.
+        # The point in time.
         self.time_stamp = time_stamp  # type: str
 
     def validate(self):
         if self.bps_data_list:
             self.bps_data_list.validate()
 
     def to_map(self):
@@ -10197,14 +10224,15 @@
             temp_model = DescribeDomainCertificateInfoResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainCnameRequest(TeaModel):
     def __init__(self, domain_name=None):
+        # The accelerated domain name that you want to query. Separate multiple domain names with commas (,). This parameter cannot be left empty.
         self.domain_name = domain_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainCnameRequest, self).to_map()
@@ -10221,16 +10249,22 @@
         if m.get('DomainName') is not None:
             self.domain_name = m.get('DomainName')
         return self
 
 
 class DescribeDomainCnameResponseBodyCnameDatasData(TeaModel):
     def __init__(self, cname=None, domain=None, status=None):
+        # The CNAME assigned to the domain name by Alibaba Cloud CDN.
         self.cname = cname  # type: str
+        # The accelerated domain name.
         self.domain = domain  # type: str
+        # The CNAME detection result. Valid values:
+        # 
+        # *   0: The DNS can detect the CNAME assigned to the domain name.
+        # *   Value other than 0: The DNS cannot detect the CNAME assigned to the domain name.
         self.status = status  # type: int
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainCnameResponseBodyCnameDatasData, self).to_map()
@@ -10287,15 +10321,17 @@
                 temp_model = DescribeDomainCnameResponseBodyCnameDatasData()
                 self.data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainCnameResponseBody(TeaModel):
     def __init__(self, cname_datas=None, request_id=None):
+        # Details about the CNAME detection results.
         self.cname_datas = cname_datas  # type: DescribeDomainCnameResponseBodyCnameDatas
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.cname_datas:
             self.cname_datas.validate()
 
     def to_map(self):
@@ -10730,29 +10766,29 @@
             temp_model = DescribeDomainDetailDataByLayerResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainHitRateDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, start_time=None):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # By default, this operation queries the byte hit ratios of all accelerated domain names that belong to your Alibaba Cloud account.
+        # By default, this operation queries the byte hit ratios for all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The time interval between the data entries. Unit: seconds.
+        # The time granularity of the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval  # type: str
-        # The start of the time range to query.
+        # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
@@ -10857,21 +10893,21 @@
 class DescribeDomainHitRateDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, hit_rate_interval=None, request_id=None,
                  start_time=None):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The byte hit ratio at each time interval. The byte hit ratio is measured in percentage.
         self.hit_rate_interval = hit_rate_interval  # type: DescribeDomainHitRateDataResponseBodyHitRateInterval
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.hit_rate_interval:
             self.hit_rate_interval.validate()
 
     def to_map(self):
@@ -11245,35 +11281,35 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainHttpCodeDataByLayerRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, isp_name_en=None, layer=None,
                  location_name_en=None, start_time=None):
-        # The accelerated domain name. You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # If you do not specify a domain name, data of all domain names is queried.
+        # If you do not specify this parameter, data of all accelerated domain names under your account is queried.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The time interval between the data entries. Unit: seconds.
+        # The time granularity of the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval  # type: str
-        # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
+        # The name of the Internet service provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
         # 
         # If you do not specify an ISP, data of all ISPs is queried.
         self.isp_name_en = isp_name_en  # type: str
         # The protocol by which you want to query HTTP status codes. The network layer supports **IPv4** and **IPv6**. The application layer supports **http**, **https**, and **quic**. You can also set the value to **all**.
         # 
-        # The default value is **all**.
+        # Default value: **all**\
         self.layer = layer  # type: str
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list.
+        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
         # 
         # If you do not specify a region, data in all regions is queried.
         self.location_name_en = location_name_en  # type: str
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
@@ -11320,15 +11356,15 @@
         return self
 
 
 class DescribeDomainHttpCodeDataByLayerResponseBodyHttpCodeDataIntervalDataModule(TeaModel):
     def __init__(self, time_stamp=None, total_value=None, value=None):
         # The timestamp of the data returned.
         self.time_stamp = time_stamp  # type: str
-        # The total number of times that HTTP status codes were returned at each time interval.
+        # The total number of times that HTTP status codes were returned.
         self.total_value = total_value  # type: str
         # The number of times that the HTTP status code was returned.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
@@ -11389,15 +11425,15 @@
         return self
 
 
 class DescribeDomainHttpCodeDataByLayerResponseBody(TeaModel):
     def __init__(self, data_interval=None, http_code_data_interval=None, request_id=None):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
-        # The number of HTTP status codes returned at each time interval.
+        # The statistics of HTTP status codes returned at each time interval.
         self.http_code_data_interval = http_code_data_interval  # type: DescribeDomainHttpCodeDataByLayerResponseBodyHttpCodeDataInterval
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.http_code_data_interval:
             self.http_code_data_interval.validate()
@@ -11728,18 +11764,36 @@
             temp_model = DescribeDomainISPDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainMax95BpsDataRequest(TeaModel):
     def __init__(self, cycle=None, domain_name=None, end_time=None, start_time=None, time_point=None):
+        # The cycle to query the 95th percentile bandwidth data. Default value: **day**. Valid values:
+        # 
+        # *   **day**: queries the 95th percentile bandwidth data by day.
+        # *   **month**: queries the 95th percentile bandwidth data by month.
         self.cycle = cycle  # type: str
+        # The accelerated domain name. If you do not specify this parameter, data of all accelerated domain names under your account is queried.
+        # 
+        # > You cannot specify multiple domain names at a time.
         self.domain_name = domain_name  # type: str
+        # The end of the time range to query.
+        # 
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
+        # The beginning of the time range to query.
+        # 
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
+        # The beginning of the time range to query.
+        # 
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.time_point = time_point  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainMax95BpsDataRequest, self).to_map()
@@ -11770,36 +11824,116 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         if m.get('TimePoint') is not None:
             self.time_point = m.get('TimePoint')
         return self
 
 
+class DescribeDomainMax95BpsDataResponseBodyDetailDataMax95Detail(TeaModel):
+    def __init__(self, area=None, max_95bps=None, max_95bps_peak_time=None, time_stamp=None):
+        self.area = area  # type: str
+        self.max_95bps = max_95bps  # type: float
+        self.max_95bps_peak_time = max_95bps_peak_time  # type: str
+        self.time_stamp = time_stamp  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeDomainMax95BpsDataResponseBodyDetailDataMax95Detail, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, max_95detail=None):
+        self.max_95detail = max_95detail  # type: list[DescribeDomainMax95BpsDataResponseBodyDetailDataMax95Detail]
+
+    def validate(self):
+        if self.max_95detail:
+            for k in self.max_95detail:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeDomainMax95BpsDataResponseBodyDetailData, self).to_map()
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
+    def from_map(self, m=None):
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
-    def __init__(self, domain_name=None, domestic_max_95bps=None, end_time=None, max_95bps=None,
+    def __init__(self, detail_data=None, domain_name=None, domestic_max_95bps=None, end_time=None, max_95bps=None,
                  overseas_max_95bps=None, request_id=None, start_time=None):
+        self.detail_data = detail_data  # type: DescribeDomainMax95BpsDataResponseBodyDetailData
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
+        # The 95th percentile bandwidth in the Chinese mainland.
         self.domestic_max_95bps = domestic_max_95bps  # type: str
+        # The end of the time range for which the data was queried.
         self.end_time = end_time  # type: str
+        # The 95th percentile bandwidth.
         self.max_95bps = max_95bps  # type: str
+        # The 95th percentile bandwidth outside the Chinese mainland.
         self.overseas_max_95bps = overseas_max_95bps  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
+        # The beginning of the time range for which the data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
-        pass
+        if self.detail_data:
+            self.detail_data.validate()
 
     def to_map(self):
         _map = super(DescribeDomainMax95BpsDataResponseBody, self).to_map()
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
@@ -11810,14 +11944,17 @@
             result['RequestId'] = self.request_id
         if self.start_time is not None:
             result['StartTime'] = self.start_time
         return result
 
     def from_map(self, m=None):
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
@@ -12170,31 +12307,27 @@
         return self
 
 
 class DescribeDomainPathDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, page_number=None, page_size=None, path=None, start_time=None):
         # The accelerated domain name.
         # 
-        # >  You can specify only one domain name in each call.
+        # > You can specify only one domain name in each call.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC. The interval between the start time and end time must be less than 30 days. Example: 2016-10-21T04:00:00Z.
         self.end_time = end_time  # type: str
         # The number of the page to return. Pages start from page **1**.
         self.page_number = page_number  # type: int
-        # The number of entries to return on each page.
-        # 
-        # Valid values: integers from **1** to **1000**.
+        # The number of entries to return on each page. Valid values: integers from **1** to **1000**.
         self.page_size = page_size  # type: int
         # The paths that you want to query. Separate paths with forward slashes (/). If you do not set this parameter, all paths are queried. If you set the value to a directory, it must end with a forward slash (/).
         # 
-        # >  Fuzzy match is not supported. If you want data to be collected based on a directory, you can specify a specific directory, for example, directory/path/. In this case, bandwidth data is collected based on directory/path/.
+        # > Fuzzy match is not supported. If you want data to be collected based on a directory, you can specify a specific directory, for example, directory/path/. In this case, bandwidth data is collected based on directory/path/.
         self.path = path  # type: str
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
-        # 
-        # Example: 2016-10-20T04:00:00Z.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC. Example: 2016-10-20T04:00:00Z.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainPathDataRequest, self).to_map()
@@ -12231,15 +12364,15 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainPathDataResponseBodyPathDataPerIntervalUsageData(TeaModel):
     def __init__(self, acc=None, path=None, time=None, traffic=None):
-        # The number of visits to the specified path.
+        # The number of visits to the URL.
         self.acc = acc  # type: int
         # The path.
         self.path = path  # type: str
         # The point in time.
         self.time = time  # type: str
         # The amount of network traffic. Unit: bytes.
         self.traffic = traffic  # type: int
@@ -12307,29 +12440,29 @@
                 self.usage_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainPathDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, page_number=None, page_size=None,
                  path_data_per_interval=None, start_time=None, total_count=None):
-        # The time interval between the data entries. Unit: seconds.
+        # The time interval. Unit: seconds.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The page number of the returned page. Pages start from page **1**.
         self.page_number = page_number  # type: int
-        # The number of entries returned on each page.
+        # The number of entries returned per page.
         self.page_size = page_size  # type: int
         # A list of bandwidth values collected at each time interval.
         self.path_data_per_interval = path_data_per_interval  # type: DescribeDomainPathDataResponseBodyPathDataPerInterval
-        # The start of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
-        # The total count.
+        # The total number of entries returned.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.path_data_per_interval:
             self.path_data_per_interval.validate()
 
     def to_map(self):
@@ -12615,29 +12748,29 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainQpsDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, isp_name_en=None, location_name_en=None,
                  start_time=None):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # By default, this operation queries the number of queries per second for all accelerated domain names that belong to your Alibaba Cloud account.
+        # By default, this operation queries QPS data for all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
         # The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The time interval between the data entries. Unit: seconds.
+        # The time granularity of the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval  # type: str
-        # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs. If you do not set this parameter, all ISPs are queried.
+        # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs. If you do not specify an ISP, data of all ISPs is queried.
         self.isp_name_en = isp_name_en  # type: str
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list. If you do not set this parameter, all regions are queried.
+        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions. If you do not specify a region, data in all regions is queried.
         self.location_name_en = location_name_en  # type: str
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
@@ -12686,31 +12819,31 @@
         self.acc_domestic_value = acc_domestic_value  # type: str
         # The number of requests outside the Chinese mainland.
         self.acc_overseas_value = acc_overseas_value  # type: str
         # The total number of requests.
         self.acc_value = acc_value  # type: str
         # The number of queries per second in the Chinese mainland.
         self.domestic_value = domestic_value  # type: str
-        # The number of HTTPS requests sent to L1 edge nodes in the Chinese mainland.
+        # The number of HTTPS requests sent to POPs in the Chinese mainland.
         self.https_acc_domestic_value = https_acc_domestic_value  # type: str
-        # The number of HTTPS requests sent to L1 edge nodes outside the Chinese mainland.
+        # The number of HTTPS requests sent to POPs outside the Chinese mainland.
         self.https_acc_overseas_value = https_acc_overseas_value  # type: str
-        # The total number of HTTPS requests sent to L1 edge nodes.
+        # The number of HTTPS requests sent to POPs.
         self.https_acc_value = https_acc_value  # type: str
-        # The number of queries per second that is calculated based on the HTTPS requests sent to L1 edge nodes in the Chinese mainland.
+        # The number of queries per second that is calculated based on the HTTPS requests sent to POPs in the Chinese mainland.
         self.https_domestic_value = https_domestic_value  # type: str
-        # The number of queries per second that is calculated based on the HTTPS requests sent to L1 edge nodes outside the Chinese mainland.
+        # The number of queries per second that is calculated based on the HTTPS requests sent to POPs outside the Chinese mainland.
         self.https_overseas_value = https_overseas_value  # type: str
-        # The number of queries per second that is calculated based on the HTTPS requests sent to L1 edge nodes.
+        # The number of queries per second that is calculated based on the HTTPS requests sent to points of presence (POPs).
         self.https_value = https_value  # type: str
         # The number of queries per second outside the Chinese mainland.
         self.overseas_value = overseas_value  # type: str
         # The timestamp of the data returned.
         self.time_stamp = time_stamp  # type: str
-        # The total number of queries per second.
+        # The total QPS.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainQpsDataResponseBodyQpsDataIntervalDataModule, self).to_map()
@@ -12812,21 +12945,21 @@
 class DescribeDomainQpsDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, qps_data_interval=None, request_id=None,
                  start_time=None):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
-        # The number of queries per second at each time interval.
+        # The list of QPS records at each interval.
         self.qps_data_interval = qps_data_interval  # type: DescribeDomainQpsDataResponseBodyQpsDataInterval
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.qps_data_interval:
             self.qps_data_interval.validate()
 
     def to_map(self):
@@ -12905,37 +13038,37 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainQpsDataByLayerRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, isp_name_en=None, layer=None,
                  location_name_en=None, start_time=None):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify a maximum of 500 domain names in a request. Separate multiple domain names with commas (,).
         # 
-        # By default, this operation queries the number of queries per second for all accelerated domain names that belong to your Alibaba Cloud account.
+        # By default, this operation queries the QPS of all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The end of the time range to query. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format in the ISO 8601 standard. The time is displayed in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The time interval between the data entries. Unit: seconds.
+        # The time interval between the data entries to return. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Description**.
         self.interval = interval  # type: str
         # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs. If you do not set this parameter, all ISPs are queried.
         self.isp_name_en = isp_name_en  # type: str
         # The layers at which you want to query the number of queries per second. Valid values:
         # 
         # *   **Network layer**: **IPv4**and **IPv6**.
         # *   **Application layer**: **http**, **https**, and **quic**.
         # *   **all**: The default value. Both the network and application layers are included.
         self.layer = layer  # type: str
         # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list. If you do not set this parameter, all regions are queried.
         self.location_name_en = location_name_en  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format in the ISO 8601 standard. The time is displayed in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainQpsDataByLayerRequest, self).to_map()
@@ -12979,25 +13112,25 @@
 
 
 class DescribeDomainQpsDataByLayerResponseBodyQpsDataIntervalDataModule(TeaModel):
     def __init__(self, acc_domestic_value=None, acc_overseas_value=None, acc_value=None, domestic_value=None,
                  overseas_value=None, time_stamp=None, value=None):
         # The number of requests in the Chinese mainland.
         self.acc_domestic_value = acc_domestic_value  # type: str
-        # The number of requests in the Chinese mainland.
+        # The number of requests outside the Chinese mainland.
         self.acc_overseas_value = acc_overseas_value  # type: str
         # The total number of requests.
         self.acc_value = acc_value  # type: str
         # The number of queries per second in the Chinese mainland.
         self.domestic_value = domestic_value  # type: str
         # The number of queries per second outside the Chinese mainland.
         self.overseas_value = overseas_value  # type: str
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
-        # The total number of queries per second in all regions.
+        # The total number of queries per second.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainQpsDataByLayerResponseBodyQpsDataIntervalDataModule, self).to_map()
@@ -13075,23 +13208,23 @@
 class DescribeDomainQpsDataByLayerResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, layer=None, qps_data_interval=None,
                  request_id=None, start_time=None):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The layer at which the data was collected.
         self.layer = layer  # type: str
-        # The number of queries per second at each time interval.
+        # The number of queries per second at each interval.
         self.qps_data_interval = qps_data_interval  # type: DescribeDomainQpsDataByLayerResponseBodyQpsDataInterval
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.qps_data_interval:
             self.qps_data_interval.validate()
 
     def to_map(self):
@@ -13173,31 +13306,31 @@
             temp_model = DescribeDomainQpsDataByLayerResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainRealTimeBpsDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, isp_name_en=None, location_name_en=None, start_time=None):
-        # The accelerated domain names. You can specify multiple accelerated domain names and separate them with commas (,).
+        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
         # 
-        # >  You can specify at most 500 accelerated domain names in each call.
+        # > You can specify up to 500 domain names in each request.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service.
+        # The name of the Internet service provider (ISP).
         # 
-        # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent ISP list. If you do not set this parameter, all ISPs are queried.
+        # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs. If you do not set this parameter, all ISPs are queried.
         self.isp_name_en = isp_name_en  # type: str
         # The name of the region.
         # 
-        # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list. If you do not set this parameter, all regions are queried.
+        # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions. If you do not set this parameter, all regions are queried.
         self.location_name_en = location_name_en  # type: str
         # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
@@ -13236,15 +13369,15 @@
         return self
 
 
 class DescribeDomainRealTimeBpsDataResponseBodyDataBpsModel(TeaModel):
     def __init__(self, bps=None, time_stamp=None):
         # The bandwidth. Unit: bit/s.
         self.bps = bps  # type: float
-        # The timestamp of the data entry. The time follows the ISO 8601 standard. The time is displayed in UTC.
+        # The timestamp of the data returned. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
         self.time_stamp = time_stamp  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRealTimeBpsDataResponseBodyDataBpsModel, self).to_map()
@@ -13297,15 +13430,15 @@
                 temp_model = DescribeDomainRealTimeBpsDataResponseBodyDataBpsModel()
                 self.bps_model.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainRealTimeBpsDataResponseBody(TeaModel):
     def __init__(self, data=None, request_id=None):
-        # The response parameters.
+        # The data returned.
         self.data = data  # type: DescribeDomainRealTimeBpsDataResponseBodyData
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.data:
             self.data.validate()
@@ -13369,21 +13502,25 @@
             temp_model = DescribeDomainRealTimeBpsDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainRealTimeByteHitRateDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, start_time=None):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 100 domain names in each call.
+        # The accelerated domain name. You can specify up to 100 domain names in each call. Separate multiple domain names with commas (,).
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.  
+        # The end of the time range to query.
         # 
-        # >  The end time must be later than the start time.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query.
+        # 
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRealTimeByteHitRateDataRequest, self).to_map()
@@ -13471,15 +13608,15 @@
                 temp_model = DescribeDomainRealTimeByteHitRateDataResponseBodyDataByteHitRateDataModel()
                 self.byte_hit_rate_data_model.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainRealTimeByteHitRateDataResponseBody(TeaModel):
     def __init__(self, data=None, request_id=None):
-        # The response parameters.
+        # The data returned.
         self.data = data  # type: DescribeDomainRealTimeByteHitRateDataResponseBodyData
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.data:
             self.data.validate()
@@ -13701,27 +13838,27 @@
             temp_model = DescribeDomainRealTimeDetailDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainRealTimeHttpCodeDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, isp_name_en=None, location_name_en=None, start_time=None):
-        # The accelerated domain names. You can specify multiple accelerated domain names and separate them with commas (,).
+        # The accelerated domain name. You can specify multiple accelerated domain names and separate them with commas (,).
         # 
-        # >  You can specify at most 100 accelerated domain names in each call.
+        # > You can specify up to 100 accelerated domain names in each request.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
+        # The name of the Internet service provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
         self.isp_name_en = isp_name_en  # type: str
-        # The name of the region. If you do not set this parameter, all regions are queried. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list.
+        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions. If you do not specify a region, all regions are queried.
         self.location_name_en = location_name_en  # type: str
         # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
@@ -13758,17 +13895,17 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainRealTimeHttpCodeDataResponseBodyRealTimeHttpCodeDataUsageDataValueRealTimeCodeProportionData(TeaModel):
     def __init__(self, code=None, count=None, proportion=None):
-        # The HTTP status code.
+        # The HTTP status code returned.
         self.code = code  # type: str
-        # The total number of HTTP status codes returned.
+        # The total number of entries.
         self.count = count  # type: str
         # The proportion of the HTTP status code.
         self.proportion = proportion  # type: str
 
     def validate(self):
         pass
 
@@ -13895,25 +14032,25 @@
 
 
 class DescribeDomainRealTimeHttpCodeDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, real_time_http_code_data=None,
                  request_id=None, start_time=None):
         # The time interval between the data entries returned. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 60 (1 minute), 300 (5 minutes), and 3600(1 hour). For more information, see the usage notes.
+        # Depending on the maximum time range per query, the value is 60 (1 minute), 300 (5 minutes), or 3600 (1 hour). For more information, see the "Time granularity" section in Usage notes.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The proportions of HTTP status codes at each time interval.
         self.real_time_http_code_data = real_time_http_code_data  # type: DescribeDomainRealTimeHttpCodeDataResponseBodyRealTimeHttpCodeData
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.real_time_http_code_data:
             self.real_time_http_code_data.validate()
 
     def to_map(self):
@@ -13991,31 +14128,31 @@
             temp_model = DescribeDomainRealTimeHttpCodeDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainRealTimeQpsDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, isp_name_en=None, location_name_en=None, start_time=None):
-        # The accelerated domain names. You can specify multiple accelerated domain names and separate them with commas (,).
+        # The accelerated domain name. Separate multiple accelerated domain names with commas (,).
         # 
-        # >  You can specify at most 500 accelerated domain names in each call.
+        # > You can specify up to 500 domain names in each request.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service.
+        # The name of the Internet service provider (ISP).
         # 
-        # If you do not set this parameter, all ISPs are queried. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
+        # If you do not set this parameter, data of all ISPs is queried. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
         self.isp_name_en = isp_name_en  # type: str
         # The name of the region.
         # 
-        # If you do not set this parameter, all regions are queried. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list.
+        # If you do not set this parameter, data in all regions is queried. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions.
         self.location_name_en = location_name_en  # type: str
         # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
@@ -14054,15 +14191,15 @@
         return self
 
 
 class DescribeDomainRealTimeQpsDataResponseBodyDataQpsModel(TeaModel):
     def __init__(self, qps=None, time_stamp=None):
         # The number of queries per second.
         self.qps = qps  # type: float
-        # The timestamp of the data returned. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
+        # The timestamp of the data returned. The time follows the yyyy-MM-ddTHH:mm:ssZ format in the ISO 8601 standard and is in UTC.
         self.time_stamp = time_stamp  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRealTimeQpsDataResponseBodyDataQpsModel, self).to_map()
@@ -14115,15 +14252,15 @@
                 temp_model = DescribeDomainRealTimeQpsDataResponseBodyDataQpsModel()
                 self.qps_model.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainRealTimeQpsDataResponseBody(TeaModel):
     def __init__(self, data=None, request_id=None):
-        # The response parameters.
+        # The data entries returned.
         self.data = data  # type: DescribeDomainRealTimeQpsDataResponseBodyData
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.data:
             self.data.validate()
@@ -14361,21 +14498,23 @@
             temp_model = DescribeDomainRealTimeReqHitRateDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainRealTimeSrcBpsDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, start_time=None):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 100 domain names in each call.
+        # The accelerated domain name. You can specify up to 100 domain names in each request. Separate multiple domain names with commas (,).
         self.domain_name = domain_name  # type: str
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The start of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query.
+        # 
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRealTimeSrcBpsDataRequest, self).to_map()
@@ -14400,15 +14539,15 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainRealTimeSrcBpsDataResponseBodyRealTimeSrcBpsDataPerIntervalDataModule(TeaModel):
     def __init__(self, time_stamp=None, value=None):
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
         # The bandwidth during back-to-origin routing. Unit: bit/s.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
@@ -14466,25 +14605,25 @@
 
 
 class DescribeDomainRealTimeSrcBpsDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None,
                  real_time_src_bps_data_per_interval=None, request_id=None, start_time=None):
         # The time interval between the data entries returned. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 60 (1 minute), 300 (5 minutes), and 3600(1 hour). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 60 (1 minute), 300 (5 minutes), and 3600(1 hour). For more information, see **Usage notes**.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
-        # The back-to-origin bandwidth information at each interval.
+        # The origin bandwidth data at each interval.
         self.real_time_src_bps_data_per_interval = real_time_src_bps_data_per_interval  # type: DescribeDomainRealTimeSrcBpsDataResponseBodyRealTimeSrcBpsDataPerInterval
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range to query.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.real_time_src_bps_data_per_interval:
             self.real_time_src_bps_data_per_interval.validate()
 
     def to_map(self):
@@ -14562,25 +14701,25 @@
             temp_model = DescribeDomainRealTimeSrcBpsDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainRealTimeSrcHttpCodeDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, isp_name_en=None, location_name_en=None, start_time=None):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 100 domain names in each call.
+        # The accelerated domain name. You can specify up to 100 domain names in each call. Separate multiple domain names with commas (,).
         self.domain_name = domain_name  # type: str
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The name of the Internet Service Provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs. If you do not set this parameter, all ISPs are queried.
+        # The name of the Internet service provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs. If you leave this parameter empty, all ISPs are queried.
         self.isp_name_en = isp_name_en  # type: str
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions. If you do not set this parameter, all regions are queried.
+        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query regions. If you leave this parameter empty, all regions are queried.
         self.location_name_en = location_name_en  # type: str
-        # The start of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRealTimeSrcHttpCodeDataRequest, self).to_map()
@@ -14613,17 +14752,17 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainRealTimeSrcHttpCodeDataResponseBodyRealTimeSrcHttpCodeDataUsageDataValueRealTimeSrcCodeProportionData(TeaModel):
     def __init__(self, code=None, count=None, proportion=None):
-        # The HTTP status code.
+        # The HTTP status code returned.
         self.code = code  # type: str
-        # The total number of HTTP status codes returned.
+        # The count of each HTTP status code.
         self.count = count  # type: str
         # The proportion of the HTTP status code.
         self.proportion = proportion  # type: str
 
     def validate(self):
         pass
 
@@ -14682,17 +14821,17 @@
                 temp_model = DescribeDomainRealTimeSrcHttpCodeDataResponseBodyRealTimeSrcHttpCodeDataUsageDataValueRealTimeSrcCodeProportionData()
                 self.real_time_src_code_proportion_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainRealTimeSrcHttpCodeDataResponseBodyRealTimeSrcHttpCodeDataUsageData(TeaModel):
     def __init__(self, time_stamp=None, value=None):
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
-        # The proportions of HTTP status codes.
+        # The proportions of the HTTP status codes.
         self.value = value  # type: DescribeDomainRealTimeSrcHttpCodeDataResponseBodyRealTimeSrcHttpCodeDataUsageDataValue
 
     def validate(self):
         if self.value:
             self.value.validate()
 
     def to_map(self):
@@ -14752,21 +14891,21 @@
 class DescribeDomainRealTimeSrcHttpCodeDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, real_time_src_http_code_data=None,
                  request_id=None, start_time=None):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The proportions of HTTP status codes at each time interval.
         self.real_time_src_http_code_data = real_time_src_http_code_data  # type: DescribeDomainRealTimeSrcHttpCodeDataResponseBodyRealTimeSrcHttpCodeData
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.real_time_src_http_code_data:
             self.real_time_src_http_code_data.validate()
 
     def to_map(self):
@@ -14844,23 +14983,23 @@
             temp_model = DescribeDomainRealTimeSrcHttpCodeDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainRealTimeSrcTrafficDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, start_time=None):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 100 domain names in each call.
+        # The accelerated domain name. You can specify up to 100 domain names in each call. Separate multiple domain names with commas (,).
         self.domain_name = domain_name  # type: str
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The beginning of the time range to query.
+        # The start of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
@@ -14889,15 +15028,15 @@
         return self
 
 
 class DescribeDomainRealTimeSrcTrafficDataResponseBodyRealTimeSrcTrafficDataPerIntervalDataModule(TeaModel):
     def __init__(self, time_stamp=None, value=None):
         # The timestamp of the data returned.
         self.time_stamp = time_stamp  # type: str
-        # The amount of back-to-origin network traffic.
+        # The amount of traffic.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRealTimeSrcTrafficDataResponseBodyRealTimeSrcTrafficDataPerIntervalDataModule, self).to_map()
@@ -14953,25 +15092,25 @@
 
 
 class DescribeDomainRealTimeSrcTrafficDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None,
                  real_time_src_traffic_data_per_interval=None, request_id=None, start_time=None):
         # The time interval between the data entries returned. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 60, (1 minute), 300 (5 minutes), and 3600 (1 hour). For more information, see the usage notes.
+        # Depending on the maximum time range per query, the value is 60 (1 minute), 300 (5 minutes), or 3600 (1 hour). For more information, see the "Time granularity" section in Usage notes.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The end of the time range for which the data was queried.
         self.end_time = end_time  # type: str
-        # The amount of back-to-origin network traffic that was collected at each interval.
+        # The amount of back-to-origin traffic returned at each interval.
         self.real_time_src_traffic_data_per_interval = real_time_src_traffic_data_per_interval  # type: DescribeDomainRealTimeSrcTrafficDataResponseBodyRealTimeSrcTrafficDataPerInterval
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range that was queried.
+        # The start of the time range for which the data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.real_time_src_traffic_data_per_interval:
             self.real_time_src_traffic_data_per_interval.validate()
 
     def to_map(self):
@@ -15049,23 +15188,23 @@
             temp_model = DescribeDomainRealTimeSrcTrafficDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainRealTimeTrafficDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, isp_name_en=None, location_name_en=None, start_time=None):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 100 domain names in each call.
+        # The accelerated domain name. You can specify up to 100 domain names in each call. Separate multiple domain names with commas (,).
         self.domain_name = domain_name  # type: str
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The name of the ISP for your Alibaba Cloud CDN service.
+        # The name of the Internet service provider (ISP).
         # 
         # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list. If you do not set this parameter, all regions are queried.
         self.isp_name_en = isp_name_en  # type: str
         # The name of the region.
         # 
         # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list. If you do not set this parameter, all regions are queried.
         self.location_name_en = location_name_en  # type: str
@@ -15108,17 +15247,17 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainRealTimeTrafficDataResponseBodyRealTimeTrafficDataPerIntervalDataModule(TeaModel):
     def __init__(self, time_stamp=None, value=None):
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
-        # The amount of network traffic.
+        # The traffic value at each time interval.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainRealTimeTrafficDataResponseBodyRealTimeTrafficDataPerIntervalDataModule, self).to_map()
@@ -15174,25 +15313,25 @@
 
 
 class DescribeDomainRealTimeTrafficDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None,
                  real_time_traffic_data_per_interval=None, request_id=None, start_time=None):
         # The time interval between the data entries returned. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 60 (1 minute), 300 (5 minutes), and 3600(1 hour). For more information, see the usage notes.
+        # Depending on the maximum time range per query, the value is 60 (1 minute), 300 (5 minutes), or 3600 (1 hour). For more information, see the "Time granularity" section in Usage notes.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
-        # The amount of network traffic at each time interval. Unit: bytes.
+        # The network traffic returned at each time interval. Unit: bytes.
         self.real_time_traffic_data_per_interval = real_time_traffic_data_per_interval  # type: DescribeDomainRealTimeTrafficDataResponseBodyRealTimeTrafficDataPerInterval
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.real_time_traffic_data_per_interval:
             self.real_time_traffic_data_per_interval.validate()
 
     def to_map(self):
@@ -15649,29 +15788,29 @@
             temp_model = DescribeDomainRegionDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainReqHitRateDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, start_time=None):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # By default, this operation queries the bandwidth values of back-to-origin requests for all accelerated domain names that belong to your Alibaba Cloud account.
+        # By default, this operation queries the request hit ratio for all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The time interval between the data entries. Unit: seconds.
+        # The time granularity of the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval  # type: str
-        # The start of the time range to query.
+        # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
@@ -15704,17 +15843,17 @@
         return self
 
 
 class DescribeDomainReqHitRateDataResponseBodyReqHitRateIntervalDataModule(TeaModel):
     def __init__(self, https_value=None, time_stamp=None, value=None):
         # The hit ratio of HTTPS requests.
         self.https_value = https_value  # type: str
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
-        # The byte hit ratio.
+        # The request hit ratio.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainReqHitRateDataResponseBodyReqHitRateIntervalDataModule, self).to_map()
@@ -15776,21 +15915,21 @@
 class DescribeDomainReqHitRateDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, req_hit_rate_interval=None,
                  request_id=None, start_time=None):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
-        # The request hit ratio at each time interval. The hit ratio is measured in percentage.
+        # The request hit ratio data at each time interval. The hit ratio is measured in percentage.
         self.req_hit_rate_interval = req_hit_rate_interval  # type: DescribeDomainReqHitRateDataResponseBodyReqHitRateInterval
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.req_hit_rate_interval:
             self.req_hit_rate_interval.validate()
 
     def to_map(self):
@@ -15868,29 +16007,29 @@
             temp_model = DescribeDomainReqHitRateDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainSrcBpsDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, start_time=None):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify up to 500 domain names in each call. Separate multiple domain names with commas (,).
         # 
-        # By default, this operation queries the bandwidth values during back-to-origin routing for all accelerated domain names that belong to your Alibaba Cloud account.
+        # By default, this operation queries the geographic distribution of users for all accelerated domain names.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
         # The time interval between the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Description**.
         self.interval = interval  # type: str
-        # The start of the time range to query.
+        # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
@@ -15921,19 +16060,19 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainSrcBpsDataResponseBodySrcBpsDataPerIntervalDataModule(TeaModel):
     def __init__(self, https_value=None, time_stamp=None, value=None):
-        # The bandwidth values of HTTPS requests.
+        # The bandwidth values of origin HTTPS requests.
         self.https_value = https_value  # type: str
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
-        # The bandwidth value.
+        # The traffic value at each time interval.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainSrcBpsDataResponseBodySrcBpsDataPerIntervalDataModule, self).to_map()
@@ -15995,21 +16134,21 @@
 class DescribeDomainSrcBpsDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, request_id=None,
                  src_bps_data_per_interval=None, start_time=None):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The bandwidth value at each time interval. Unit: bit/s.
+        # The origin bandwidth data at each time interval. Unit: bit/s.
         self.src_bps_data_per_interval = src_bps_data_per_interval  # type: DescribeDomainSrcBpsDataResponseBodySrcBpsDataPerInterval
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.src_bps_data_per_interval:
             self.src_bps_data_per_interval.validate()
 
     def to_map(self):
@@ -16087,29 +16226,25 @@
             temp_model = DescribeDomainSrcBpsDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainSrcHttpCodeDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, start_time=None):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify a maximum of 500 domain names in a request. Separate multiple domain names with commas (,).
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query.
+        # The end of the time range to query. Specify the time in the yyyy-MM-ddTHH:mm:ssZ format in the ISO 8601 standard. The time is displayed in UTC.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC. The time must be in UTC.
-        # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The time interval between the data entries. Unit: seconds.
+        # The time interval between the data entries to return. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Description**.
         self.interval = interval  # type: str
-        # The start of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainSrcHttpCodeDataRequest, self).to_map()
@@ -16138,17 +16273,17 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainSrcHttpCodeDataResponseBodyHttpCodeDataUsageDataValueCodeProportionData(TeaModel):
     def __init__(self, code=None, count=None, proportion=None):
-        # The HTTP status code.
+        # The HTTP status code returned.
         self.code = code  # type: str
-        # The total number of HTTP status codes returned.
+        # The total number of entries.
         self.count = count  # type: str
         # The proportion of the HTTP status code.
         self.proportion = proportion  # type: str
 
     def validate(self):
         pass
 
@@ -16207,17 +16342,17 @@
                 temp_model = DescribeDomainSrcHttpCodeDataResponseBodyHttpCodeDataUsageDataValueCodeProportionData()
                 self.code_proportion_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainSrcHttpCodeDataResponseBodyHttpCodeDataUsageData(TeaModel):
     def __init__(self, time_stamp=None, value=None):
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
-        # The proportions of HTTP status codes.
+        # The proportions of the HTTP status codes.
         self.value = value  # type: DescribeDomainSrcHttpCodeDataResponseBodyHttpCodeDataUsageDataValue
 
     def validate(self):
         if self.value:
             self.value.validate()
 
     def to_map(self):
@@ -16277,21 +16412,21 @@
 class DescribeDomainSrcHttpCodeDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, http_code_data=None, request_id=None,
                  start_time=None):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The proportions of HTTP status codes at each time interval.
         self.http_code_data = http_code_data  # type: DescribeDomainSrcHttpCodeDataResponseBodyHttpCodeData
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.http_code_data:
             self.http_code_data.validate()
 
     def to_map(self):
@@ -16369,29 +16504,29 @@
             temp_model = DescribeDomainSrcHttpCodeDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainSrcQpsDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, start_time=None):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify multiple domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # By default, this operation queries the number of back-to-origin requests per second for all accelerated domain names that belong to your Alibaba Cloud account.
+        # By default, this operation queries QPS data for all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The time granularity of the data entries. Unit: seconds.
+        # The time interval between the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval  # type: str
-        # The start of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # If you do not set this parameter, data collected within the last 24 hours is queried.
+        # If you leave this parameter empty, data collected in the last 24 hours is queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainSrcQpsDataRequest, self).to_map()
@@ -16422,15 +16557,15 @@
         return self
 
 
 class DescribeDomainSrcQpsDataResponseBodySrcQpsDataPerIntervalDataModule(TeaModel):
     def __init__(self, time_stamp=None, value=None):
         # The timestamp of the data returned.
         self.time_stamp = time_stamp  # type: str
-        # The number of back-to-origin requests per second.
+        # The QPS value.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainSrcQpsDataResponseBodySrcQpsDataPerIntervalDataModule, self).to_map()
@@ -16488,21 +16623,21 @@
 class DescribeDomainSrcQpsDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, request_id=None,
                  src_qps_data_per_interval=None, start_time=None):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
         # The back-to-origin bandwidth information at each interval.
         self.src_qps_data_per_interval = src_qps_data_per_interval  # type: DescribeDomainSrcQpsDataResponseBodySrcQpsDataPerInterval
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.src_qps_data_per_interval:
             self.src_qps_data_per_interval.validate()
 
     def to_map(self):
@@ -17156,29 +17291,29 @@
             temp_model = DescribeDomainSrcTopUrlVisitResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainSrcTrafficDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, start_time=None):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # By default, this operation queries back-to-origin network traffic for all accelerated domain names that belong to your Alibaba Cloud account.
+        # By default, this operation queries the origin traffic for all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The time interval between the data entries. Unit: seconds.
+        # The time granularity of the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval  # type: str
-        # The start of the time range to query.
+        # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
@@ -17209,19 +17344,19 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainSrcTrafficDataResponseBodySrcTrafficDataPerIntervalDataModule(TeaModel):
     def __init__(self, https_value=None, time_stamp=None, value=None):
-        # The amount of traffic generated by back-to-origin HTTPS requests.
+        # The amount of traffic generated by origin HTTPS requests.
         self.https_value = https_value  # type: str
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
-        # The amount of network traffic.
+        # The traffic value at each time interval.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainSrcTrafficDataResponseBodySrcTrafficDataPerIntervalDataModule, self).to_map()
@@ -17283,21 +17418,21 @@
 class DescribeDomainSrcTrafficDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, request_id=None,
                  src_traffic_data_per_interval=None, start_time=None):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The amount of back-to-origin network traffic at each time interval. Unit: bytes.
+        # The amount of origin traffic returned at each time interval. Unit: bytes.
         self.src_traffic_data_per_interval = src_traffic_data_per_interval  # type: DescribeDomainSrcTrafficDataResponseBodySrcTrafficDataPerInterval
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
 
     def validate(self):
         if self.src_traffic_data_per_interval:
             self.src_traffic_data_per_interval.validate()
 
     def to_map(self):
@@ -17776,28 +17911,32 @@
             temp_model = DescribeDomainTopReferVisitResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainTopUrlVisitRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, sort_by=None, start_time=None):
-        # The accelerated domain name for which you want to query data. If you do not set this parameter, frequently requested URLs of all accelerated domain names of your Alibaba Cloud account are queried.
+        # The accelerated domain name that you want to query.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
+        # The end of the time range to query.
         # 
-        # >  The end time must be later than the start time. The difference between the end time and the start time cannot exceed seven days.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # > The end time must be later than the start time. The maximum time range that can be specified is seven days.
         self.end_time = end_time  # type: str
-        # The method that is used to sort the returned URLs.**** Valid values:
+        # The method that is used to sort the returned URLs. Default value: **pv**. Valid values:
         # 
-        # *   **traf**: network traffic
-        # *   **pv**: by the number of page views. This is the default value.
+        # *   **traf**: by network traffic
+        # *   **pv**: by the number of page views
         self.sort_by = sort_by  # type: str
-        # The start of the time range to query. The time follows the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time is displayed in UTC.
+        # The start of the time range to query.
+        # 
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # If you want to query data within a specific day, we recommend that you set the value in the yyyy-MM-ddT16:00:00Z format.
+        # If you want to query data of a specific day, we recommend that you set the value in the yyyy-MM-ddT16:00:00Z format.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainTopUrlVisitRequest, self).to_map()
@@ -17826,23 +17965,23 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainTopUrlVisitResponseBodyAllUrlListUrlList(TeaModel):
     def __init__(self, flow=None, flow_proportion=None, url_detail=None, visit_data=None, visit_proportion=None):
-        # The amount of network traffic. (Unit: bytes)
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow  # type: str
-        # The proportion of the amount of network traffic consumed for visiting the web page.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion  # type: float
         # The complete URL.
         self.url_detail = url_detail  # type: str
-        # The number of visits to the specified path.
+        # The number of visits to the URL.
         self.visit_data = visit_data  # type: str
-        # The proportion of visits to the web page.
+        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainTopUrlVisitResponseBodyAllUrlListUrlList, self).to_map()
@@ -17907,23 +18046,23 @@
                 temp_model = DescribeDomainTopUrlVisitResponseBodyAllUrlListUrlList()
                 self.url_list.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainTopUrlVisitResponseBodyUrl200ListUrlList(TeaModel):
     def __init__(self, flow=None, flow_proportion=None, url_detail=None, visit_data=None, visit_proportion=None):
-        # The amount of network traffic. (Unit: bytes)
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow  # type: str
-        # The proportion of the amount of network traffic consumed for visiting the web page.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion  # type: float
         # The complete URL.
         self.url_detail = url_detail  # type: str
-        # The number of visits to the specified path.
+        # The number of visits to the URL.
         self.visit_data = visit_data  # type: str
-        # The proportion of visits to the web page.
+        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainTopUrlVisitResponseBodyUrl200ListUrlList, self).to_map()
@@ -17988,23 +18127,23 @@
                 temp_model = DescribeDomainTopUrlVisitResponseBodyUrl200ListUrlList()
                 self.url_list.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainTopUrlVisitResponseBodyUrl300ListUrlList(TeaModel):
     def __init__(self, flow=None, flow_proportion=None, url_detail=None, visit_data=None, visit_proportion=None):
-        # The amount of network traffic. (Unit: bytes)
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow  # type: str
-        # The proportion of the amount of network traffic consumed for visiting the web page.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion  # type: float
         # The complete URL.
         self.url_detail = url_detail  # type: str
         # The number of visits to the URL.
         self.visit_data = visit_data  # type: str
-        # The proportion of visits to the web page.
+        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainTopUrlVisitResponseBodyUrl300ListUrlList, self).to_map()
@@ -18069,23 +18208,23 @@
                 temp_model = DescribeDomainTopUrlVisitResponseBodyUrl300ListUrlList()
                 self.url_list.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainTopUrlVisitResponseBodyUrl400ListUrlList(TeaModel):
     def __init__(self, flow=None, flow_proportion=None, url_detail=None, visit_data=None, visit_proportion=None):
-        # The amount of network traffic. (Unit: bytes)
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow  # type: str
-        # The proportion of the amount of network traffic consumed for visiting the web page.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion  # type: float
         # The complete URL.
         self.url_detail = url_detail  # type: str
         # The number of visits to the URL.
         self.visit_data = visit_data  # type: str
-        # The proportion of visits to the web page.
+        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainTopUrlVisitResponseBodyUrl400ListUrlList, self).to_map()
@@ -18150,23 +18289,23 @@
                 temp_model = DescribeDomainTopUrlVisitResponseBodyUrl400ListUrlList()
                 self.url_list.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainTopUrlVisitResponseBodyUrl500ListUrlList(TeaModel):
     def __init__(self, flow=None, flow_proportion=None, url_detail=None, visit_data=None, visit_proportion=None):
-        # The amount of network traffic. (Unit: bytes)
+        # The amount of network traffic. Unit: bytes.
         self.flow = flow  # type: str
-        # The proportion of the amount of network traffic consumed for visiting the web page.
+        # The proportion of network traffic consumed to access the URL.
         self.flow_proportion = flow_proportion  # type: float
         # The complete URL.
         self.url_detail = url_detail  # type: str
         # The number of visits to the URL.
         self.visit_data = visit_data  # type: str
-        # The proportion of visits to the web page.
+        # The proportion of visits to the URL.
         self.visit_proportion = visit_proportion  # type: float
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainTopUrlVisitResponseBodyUrl500ListUrlList, self).to_map()
@@ -18238,15 +18377,15 @@
                  url_300list=None, url_400list=None, url_500list=None):
         # A list of frequently requested URLs.
         self.all_url_list = all_url_list  # type: DescribeDomainTopUrlVisitResponseBodyAllUrlList
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The start of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
         # A list of URLs for which 2xx status codes were returned.
         self.url_200list = url_200list  # type: DescribeDomainTopUrlVisitResponseBodyUrl200List
         # A list of URLs for which 3xx status codes were returned.
         self.url_300list = url_300list  # type: DescribeDomainTopUrlVisitResponseBodyUrl300List
         # A list of URLs for which 4xx status codes were returned.
         self.url_400list = url_400list  # type: DescribeDomainTopUrlVisitResponseBodyUrl400List
@@ -18353,39 +18492,35 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainTrafficDataRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, interval=None, isp_name_en=None, location_name_en=None,
                  start_time=None):
-        # You can specify multiple domain names and separate them with commas (,). You can specify at most 500 domain names in each call.
+        # The accelerated domain name. You can specify up to 500 domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # By default, this operation queries the monitoring data of network traffic for all accelerated domain names that belong to your Alibaba Cloud account.
+        # By default, this operation queries the network traffic for all accelerated domain names that belong to your Alibaba Cloud account.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time.
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The time interval between the data entries. Unit: seconds.
+        # The time granularity of the data entries. Unit: seconds.
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # The time granularity varies with the maximum time range per query. Valid values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
         self.interval = interval  # type: str
-        # The name of the Internet service provider (ISP) for your Alibaba Cloud CDN service. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISP names.
+        # The name of the Internet service provider (ISP). You can call the [DescribeCdnRegionAndIsp](~~DescribeCdnRegionAndIsp~~) operation to query ISPs.
         # 
-        # If you do not specify an ISP, monitoring data of all ISPs is queried.
+        # If you do not specify an ISP, data of all ISPs is queried.
         self.isp_name_en = isp_name_en  # type: str
-        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list.
+        # The name of the region. You can call the [DescribeCdnRegionAndIsp](~~DescribeCdnRegionAndIsp~~) operation to query regions.
         # 
-        # If you do not specify a region, monitoring data in all regions is queried.
+        # If you do not specify a region, data in all regions is queried.
         self.location_name_en = location_name_en  # type: str
-        # The start of the time range to query.
-        # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainTrafficDataRequest, self).to_map()
@@ -18425,25 +18560,25 @@
 
 
 class DescribeDomainTrafficDataResponseBodyTrafficDataPerIntervalDataModule(TeaModel):
     def __init__(self, domestic_value=None, https_domestic_value=None, https_overseas_value=None, https_value=None,
                  overseas_value=None, time_stamp=None, value=None):
         # The amount of network traffic in the Chinese mainland.
         self.domestic_value = domestic_value  # type: str
-        # The amount of HTTPS network traffic on L1 edge nodes in the Chinese mainland.
+        # The amount of HTTPS traffic on points of presence (POPs) in the Chinese mainland.
         self.https_domestic_value = https_domestic_value  # type: str
-        # The amount of HTTPS network traffic on L1 edge nodes outside the Chinese mainland.
+        # The amount of HTTPS traffic on POPs outside the Chinese mainland.
         self.https_overseas_value = https_overseas_value  # type: str
-        # The total amount of HTTPS network traffic on L1 edge nodes.
+        # The total amount of HTTPS traffic on POPs.
         self.https_value = https_value  # type: str
         # The amount of network traffic outside the Chinese mainland.
         self.overseas_value = overseas_value  # type: str
-        # The timestamp of the data returned.
+        # The timestamp of the returned data.
         self.time_stamp = time_stamp  # type: str
-        # The total amount of network traffic.
+        # The total volume of traffic.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainTrafficDataResponseBodyTrafficDataPerIntervalDataModule, self).to_map()
@@ -18521,19 +18656,19 @@
 class DescribeDomainTrafficDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, request_id=None, start_time=None,
                  traffic_data_per_interval=None):
         # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
         # The amount of network traffic at each time interval. Unit: bytes.
         self.traffic_data_per_interval = traffic_data_per_interval  # type: DescribeDomainTrafficDataResponseBodyTrafficDataPerInterval
 
     def validate(self):
         if self.traffic_data_per_interval:
             self.traffic_data_per_interval.validate()
@@ -18614,69 +18749,69 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeDomainUsageDataRequest(TeaModel):
     def __init__(self, area=None, data_protocol=None, domain_name=None, end_time=None, field=None, interval=None,
                  start_time=None, type=None):
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
         self.area = area  # type: str
-        # The protocol by which the data is queried. Valid values:
+        # The protocol of the data that you want to query. Default value: all. Valid values:
         # 
         # *   **http**: HTTP
         # *   **https**: HTTPS
         # *   **quic**: QUIC
-        # *   **all** (default): HTTP, HTTPS, and QUIC
+        # *   **all**: HTTP, HTTPS, and QUIC
         self.data_protocol = data_protocol  # type: str
-        # The accelerated domain name. You can query the resource usage data for a maximum of 100 domain names in each call. Separate domain names with commas (,).
+        # The accelerated domain name. You can specify up to 100 domain names in each request. Separate multiple domain names with commas (,).
         # 
-        # >  If you do not set this parameter, the usage data of all accelerated domain names within your Alibaba Cloud account is returned.
+        # > If you leave this parameter empty, the usage data of all accelerated domain names in your Alibaba Cloud account is returned.
         self.domain_name = domain_name  # type: str
         # The end of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time. The maximum time range that can be queried is 31 days.
+        # > The end time must be later than the start time. The maximum time range that can be specified is 31 days.
         self.end_time = end_time  # type: str
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
         self.field = field  # type: str
-        # The time interval between the data entries. Unit: seconds.
+        # The time interval between the data entries to return. Unit: seconds. Valid values: **300** (5 minutes), **3600** (1 hour), and **86400** (1 day).
         # 
-        # The time granularity varies with the time range to query. Supported values: 300 (5 minutes), 3600 (1 hour), and 86400 (1 day). For more information, see **Usage notes**.
+        # *   If **Interval** is set to **300**, you can query usage data in the last six months. The maximum time range per query that can be specified is three days.
+        # *   If **Interval** is set to **3600** or **86400**, you can query usage data of the previous year.
+        # *   If you do not set the **Interval** parameter, the maximum time range that you can query is one month. If you specify a time range of 1 to 3 days, the time interval between the entries that are returned is 1 hour. If you specify a time range of at least 4 days, the time interval between the entries that are returned is 1 day.
         self.interval = interval  # type: str
         # The beginning of the time range to query.
         # 
         # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The data is collected every 5 minutes.
+        # > Data is collected every 5 minutes.
         self.start_time = start_time  # type: str
-        # The type of content based on which the data is queried. Valid values:
+        # The type of content that you want to query. Default value: all. Valid values:
         # 
         # *   **static**: static content
         # *   **dynamic**: dynamic content
-        # *   **all** (default): both static and dynamic content
+        # *   **all**: both static and dynamic content
         self.type = type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainUsageDataRequest, self).to_map()
@@ -18721,27 +18856,25 @@
         if m.get('Type') is not None:
             self.type = m.get('Type')
         return self
 
 
 class DescribeDomainUsageDataResponseBodyUsageDataPerIntervalDataModule(TeaModel):
     def __init__(self, peak_time=None, special_value=None, time_stamp=None, value=None):
-        # If the **Field** parameter in the request is set to **bps**, this parameter returns the time of the peak bandwidth value. Otherwise, this parameter returns the same value as the **TimeStamp** parameter.
+        # The time of the peak bandwidth value if the **Field** parameter in the request is set to **bps**. Otherwise, this parameter returns the same value as the **TimeStamp** parameter.
         self.peak_time = peak_time  # type: str
         # The data usage in a specific scenario.
         # 
-        # >  Indicates the data usage in a specific scenario. If no special billable item is specified, ignore this parameter.
+        # > SpecialValue indicates the data usage in a specific scenario. If no special billable item is specified, ignore this parameter.
         self.special_value = special_value  # type: str
         # The timestamp of the data returned.
         # 
-        # >  The **TimeStamp** parameter may return multiple values.
+        # > **TimeStamp** indicates the timestamp of the returned data at each interval.
         self.time_stamp = time_stamp  # type: str
-        # The usage.
-        # 
-        # >  Usage data includes network traffic (measured in bytes), bandwidth values (measured in bits/s), and the number of requests.
+        # The amount of resource usage.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainUsageDataResponseBodyUsageDataPerIntervalDataModule, self).to_map()
@@ -18803,29 +18936,29 @@
                 self.data_module.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainUsageDataResponseBody(TeaModel):
     def __init__(self, area=None, data_interval=None, domain_name=None, end_time=None, request_id=None,
                  start_time=None, type=None, usage_data_per_interval=None):
-        # The billable region where the usage information was collected.
+        # The billable region where the data was collected.
         self.area = area  # type: str
-        # The time interval between the data entries. Unit: seconds.
+        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The beginning of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
-        # The type of content based on which the usage information was collected.
+        # The type of content.
         self.type = type  # type: str
-        # The network traffic that was collected at each interval.
+        # The resource usage that was collected at each interval.
         self.usage_data_per_interval = usage_data_per_interval  # type: DescribeDomainUsageDataResponseBodyUsageDataPerInterval
 
     def validate(self):
         if self.usage_data_per_interval:
             self.usage_data_per_interval.validate()
 
     def to_map(self):
@@ -19014,15 +19147,15 @@
                 self.usage_data.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainUvDataResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, request_id=None, start_time=None,
                  uv_data_interval=None):
-        # The time interval between the data entries. Unit: seconds.
+        # The time interval. Unit: seconds.
         self.data_interval = data_interval  # type: str
         # The accelerated domain name.
         self.domain_name = domain_name  # type: str
         # The end of the time range that was queried.
         self.end_time = end_time  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
@@ -19423,21 +19556,25 @@
         return self
 
 
 class DescribeDomainsUsageByDayRequest(TeaModel):
     def __init__(self, domain_name=None, end_time=None, start_time=None):
         # The accelerated domain name. You can specify only one domain name.
         # 
-        # If you do not specify an accelerated domain name, the monitoring data of all accelerated domain names that belong to your account is queried.
+        # If you do not specify an accelerated domain name, the data of all accelerated domain names that belong to your account is queried.
         self.domain_name = domain_name  # type: str
-        # The end of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The end of the time range to query.
         # 
-        # >  The end time must be later than the start time.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
+        # 
+        # > The end time must be later than the start time.
         self.end_time = end_time  # type: str
-        # The start of the time range to query. Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # The beginning of the time range to query.
+        # 
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeDomainsUsageByDayRequest, self).to_map()
@@ -19463,15 +19600,15 @@
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeDomainsUsageByDayResponseBodyUsageByDaysUsageByDay(TeaModel):
     def __init__(self, bytes_hit_rate=None, max_bps=None, max_bps_time=None, max_src_bps=None,
                  max_src_bps_time=None, qps=None, request_hit_rate=None, time_stamp=None, total_access=None, total_traffic=None):
-        # The cache hit ratio that is calculated based on bytes. The cache hit ratio is measured in percentage.
+        # The byte hit ratio. The byte hit ratio is measured in percentage.
         self.bytes_hit_rate = bytes_hit_rate  # type: str
         # The peak bandwidth value. Unit: bit/s.
         self.max_bps = max_bps  # type: str
         # The time when the bandwidth reached the peak value.
         self.max_bps_time = max_bps_time  # type: str
         # The peak bandwidth value during back-to-origin routing. Unit: bit/s.
         self.max_src_bps = max_src_bps  # type: str
@@ -19575,27 +19712,27 @@
                 self.usage_by_day.append(temp_model.from_map(k))
         return self
 
 
 class DescribeDomainsUsageByDayResponseBodyUsageTotal(TeaModel):
     def __init__(self, bytes_hit_rate=None, max_bps=None, max_bps_time=None, max_src_bps=None,
                  max_src_bps_time=None, request_hit_rate=None, total_access=None, total_traffic=None):
-        # The cache hit ratio that is calculated based on bytes. The cache hit ratio is measured in percentage.
+        # The byte hit ratio. The byte hit ratio is measured in percentage.
         self.bytes_hit_rate = bytes_hit_rate  # type: str
         # The peak bandwidth value. Unit: bit/s.
         self.max_bps = max_bps  # type: str
         # The time when the bandwidth reached the peak value.
         self.max_bps_time = max_bps_time  # type: str
         # The peak bandwidth value during back-to-origin routing. Unit: bit/s.
         self.max_src_bps = max_src_bps  # type: str
         # The time when the bandwidth during back-to-origin routing reached the peak value.
         self.max_src_bps_time = max_src_bps_time  # type: str
         # The cache hit ratio that is calculated based on requests. The cache hit ratio is measured in percentage.
         self.request_hit_rate = request_hit_rate  # type: str
-        # The total number of requests.
+        # The total amount of requests.
         self.total_access = total_access  # type: str
         # The total amount of network traffic. Unit: bytes.
         self.total_traffic = total_traffic  # type: str
 
     def validate(self):
         pass
 
@@ -19643,23 +19780,23 @@
             self.total_traffic = m.get('TotalTraffic')
         return self
 
 
 class DescribeDomainsUsageByDayResponseBody(TeaModel):
     def __init__(self, data_interval=None, domain_name=None, end_time=None, request_id=None, start_time=None,
                  usage_by_days=None, usage_total=None):
-        # The time interval between the data entries. Unit: seconds.
+        # The time interval between the data entries returned. Unit: seconds.
         self.data_interval = data_interval  # type: str
-        # The information about the accelerated domain name.
+        # The accelerated domain name.
         self.domain_name = domain_name  # type: str
-        # The end of the time range that was queried.
+        # The end of the time range during which data was queried.
         self.end_time = end_time  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
-        # The start of the time range that was queried.
+        # The start of the time range during which data was queried.
         self.start_time = start_time  # type: str
         # The monitoring data collected at each time interval.
         self.usage_by_days = usage_by_days  # type: DescribeDomainsUsageByDayResponseBodyUsageByDays
         # The summarized monitoring data.
         self.usage_total = usage_total  # type: DescribeDomainsUsageByDayResponseBodyUsageTotal
 
     def validate(self):
@@ -20950,29 +21087,29 @@
 
 class DescribeRangeDataByLocateAndIspServiceRequest(TeaModel):
     def __init__(self, domain_names=None, end_time=None, isp_names=None, location_names=None, start_time=None):
         # The accelerated domain name.
         self.domain_names = domain_names  # type: str
         # The end of the time range to query.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         # 
-        # >  The end time must be later than the start time. The interval between the end time and the start time cannot exceed 1 hour.
+        # > The end time must be later than the start time. The maximum time range that can be specified is 1 hour.
         self.end_time = end_time  # type: str
         # The name of the ISP. You can specify only one ISP name in each call.
         # 
         # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query ISPs.
         self.isp_names = isp_names  # type: str
-        # The names of the regions. Separate regions with commas (,).
+        # The names of the regions. Separate multiple region names with commas (,).
         # 
         # You can call the [DescribeCdnRegionAndIsp](~~91077~~) operation to query the most recent region list.
         self.location_names = location_names  # type: str
         # The beginning of the time range to query.
         # 
-        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC+0.
+        # Specify the time in the ISO 8601 standard in the yyyy-MM-ddTHH:mm:ssZ format. The time must be in UTC.
         self.start_time = start_time  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeRangeDataByLocateAndIspServiceRequest, self).to_map()
@@ -21005,17 +21142,15 @@
         if m.get('StartTime') is not None:
             self.start_time = m.get('StartTime')
         return self
 
 
 class DescribeRangeDataByLocateAndIspServiceResponseBody(TeaModel):
     def __init__(self, json_result=None, request_id=None):
-        # The response parameters in the JSON format.
-        # 
-        # These parameters indicate the following information in sequence: UNIX time, region, ISP, distribution of HTTP status codes, response time, bandwidth (bit/s), average response rate, page views, cache hit ratio, and request hit ratio.
+        # The response parameters in the JSON format. These parameters indicate the following information in sequence: UNIX time, region, ISP, distribution of HTTP status codes, response time, bandwidth (bit/s), average response rate, page views, cache hit ratio, and request hit ratio.
         self.json_result = json_result  # type: str
         # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
@@ -25570,34 +25705,35 @@
 
 
 class PushObjectCacheRequest(TeaModel):
     def __init__(self, area=None, l_2preload=None, object_path=None, owner_id=None, security_token=None,
                  with_header=None):
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
         self.area = area  # type: str
         # Specifies whether to prefetch content to POPs. Valid values:
         # 
-        # *   **true**: prefetch content to L2 edge nodes.
-        # *   **false**: prefetch content to regular edge nodes. Regular edge nodes can be L2 edge nodes or L3 edge nodes. Default value: **false**.
+        # *   **true**: prefetches content to POPs.
+        # *   **false**: prefetches content to regular POPs. Regular POPs can be L2 POPs or L3 POPs. Default value: **false**.
         self.l_2preload = l_2preload  # type: bool
         # The URLs based on which content is prefetched. Format: **accelerated domain name/files to be prefetched**.
         # 
-        # >  Separate URLs with line feeds (\n or \r\n). Each object path can be up to 1,024 characters in length.
+        # > Separate URLs with line feeds (\n or \r\n). Each object path can be up to 1,024 characters in length.
         self.object_path = object_path  # type: str
         self.owner_id = owner_id  # type: long
         self.security_token = security_token  # type: str
+        # The custom header for prefetch in the JSON format.
         self.with_header = with_header  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(PushObjectCacheRequest, self).to_map()
@@ -25708,15 +25844,15 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RefreshObjectCachesRequest(TeaModel):
     def __init__(self, object_path=None, object_type=None, owner_id=None, security_token=None):
         self.object_path = object_path  # type: str
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

### Comparing `alibabacloud_cdn20180510_py2-1.2.6/alibabacloud_cdn20180510_py2.egg-info/PKG-INFO` & `alibabacloud_cdn20180510_py2-1.2.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-cdn20180510-py2
-Version: 1.2.6
+Name: alibabacloud_cdn20180510_py2
+Version: 1.2.7
 Summary: Alibaba Cloud Alibaba Cloud CDN (20180510) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cdn20180510_py2-1.2.6/setup.py` & `alibabacloud_cdn20180510_py2-1.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cdn20180510_py2.
 
-Created on 29/03/2023
+Created on 25/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cdn20180510"
 NAME = "alibabacloud_cdn20180510_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Alibaba Cloud CDN (20180510) SDK Library for Python2"
```

