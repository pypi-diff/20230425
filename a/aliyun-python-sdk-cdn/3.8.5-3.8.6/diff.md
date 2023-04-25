# Comparing `tmp/aliyun-python-sdk-cdn-3.8.5.tar.gz` & `tmp/aliyun-python-sdk-cdn-3.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-cdn-3.8.5.tar", last modified: Wed Mar 29 08:06:59 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-cdn-3.8.6.tar", last modified: Tue Apr 25 07:08:15 2023, max compression
```

## Comparing `aliyun-python-sdk-cdn-3.8.5.tar` & `aliyun-python-sdk-cdn-3.8.6.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 08:06:59.000000 aliyun-python-sdk-cdn-3.8.5/
--rw-r--r--   0 root         (0) root         (0)      575 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1537 2023-03-29 08:06:59.000000 aliyun-python-sdk-cdn-3.8.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 08:06:59.000000 aliyun-python-sdk-cdn-3.8.5/aliyun_python_sdk_cdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-03-29 08:06:59.000000 aliyun-python-sdk-cdn-3.8.5/aliyun_python_sdk_cdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10526 2023-03-29 08:06:59.000000 aliyun-python-sdk-cdn-3.8.5/aliyun_python_sdk_cdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 08:06:59.000000 aliyun-python-sdk-cdn-3.8.5/aliyun_python_sdk_cdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-03-29 08:06:59.000000 aliyun-python-sdk-cdn-3.8.5/aliyun_python_sdk_cdn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-29 08:06:59.000000 aliyun-python-sdk-cdn-3.8.5/aliyun_python_sdk_cdn.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 08:06:59.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1680 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 08:06:59.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 08:06:59.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/
--rw-r--r--   0 root         (0) root         (0)     3573 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/AddCdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/AddFCTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)     3164 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/BatchAddCdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2275 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/BatchDeleteCdnDomainConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2245 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/BatchSetCdnDomainConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     3108 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/BatchSetCdnDomainServerCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1849 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/BatchStartCdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1847 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/BatchStopCdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2454 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/BatchUpdateCdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2730 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/CreateCdnCertificateSigningRequestRequest.py
--rw-r--r--   0 root         (0) root         (0)     2142 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/CreateCdnDeliverTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/CreateCdnSubTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/CreateIllegalUrlExportTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1971 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/CreateRealTimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2527 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/CreateUsageDetailDataExportTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/CreateUserUsageDataExportTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DeleteCdnDeliverTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1829 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DeleteCdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1268 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DeleteCdnSubTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DeleteFCTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1804 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DeleteRealTimeLogLogstoreRequest.py
--rw-r--r--   0 root         (0) root         (0)     1971 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DeleteRealtimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2024 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DeleteSpecificConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2038 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DeleteSpecificStagingConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DeleteUsageDetailDataExportTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1461 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DeleteUserUsageDataExportTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1458 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeBlockedRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1849 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnCertificateDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1857 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnCertificateListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnDeletedDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1461 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnDeliverListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1650 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnDomainByCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2241 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnDomainConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnDomainDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     2189 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnDomainLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1696 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnDomainStagingConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1835 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnHttpsDomainListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1881 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnOrderCommodityCodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnRegionAndIspRequest.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnReportListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2519 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1889 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnSMCertificateDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1861 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnSMCertificateListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1650 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1272 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnSubListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillHistoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1992 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillPredictionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1640 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1483 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnUserConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2056 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnUserDomainsByFuncRequest.py
--rw-r--r--   0 root         (0) root         (0)     1654 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnUserQuotaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1841 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnUserResourcePackageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1688 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnWafDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCertificateInfoByIDRequest.py
--rw-r--r--   0 root         (0) root         (0)     1460 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCustomLogConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2806 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainAverageResponseTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2581 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataByLayerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2064 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataByTimeStampRequest.py
--rw-r--r--   0 root         (0) root         (0)     2406 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2750 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainCcActivityLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     1485 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainCertificateInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainCnameRequest.py
--rw-r--r--   0 root         (0) root         (0)     1484 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainCustomLogConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2568 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainDetailDataByLayerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2014 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainHitRateDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2591 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainHttpCodeDataByLayerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2416 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainHttpCodeDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1827 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainISPDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2183 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainMax95BpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1841 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainMultiUsageDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2357 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainPathDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainPvDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2581 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainQpsDataByLayerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2406 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainQpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2242 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeBpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1858 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeByteHitRateDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2767 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeDetailDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2253 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeHttpCodeDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2242 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeQpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1856 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeReqHitRateDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1849 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcBpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2259 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcHttpCodeDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1857 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcTrafficDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2251 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeTrafficDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1468 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealtimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRegionDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2020 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainReqHitRateDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2012 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainSrcBpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainSrcHttpCodeDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2012 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainSrcQpsDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2008 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainSrcTopUrlVisitRequest.py
--rw-r--r--   0 root         (0) root         (0)     2020 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainSrcTrafficDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2388 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainTopClientIpVisitRequest.py
--rw-r--r--   0 root         (0) root         (0)     2006 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainTopReferVisitRequest.py
--rw-r--r--   0 root         (0) root         (0)     2002 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainTopUrlVisitRequest.py
--rw-r--r--   0 root         (0) root         (0)     2414 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainTrafficDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     2684 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainUsageDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainUvDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainsBySourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1835 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainsUsageByDayRequest.py
--rw-r--r--   0 root         (0) root         (0)     1807 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeEsExceptionDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1803 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeEsExecuteDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1460 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeFCTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1459 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeIllegalUrlExportTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1407 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeIpInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeIpStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1849 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeL2VipsByDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribePreloadDetailByIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     2255 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeRangeDataByLocateAndIspServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2179 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeRealtimeDeliveryAccRequest.py
--rw-r--r--   0 root         (0) root         (0)     1654 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeRefreshQuotaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1449 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeRefreshTaskByIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     3514 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeRefreshTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeStagingIpRequest.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1799 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeTopDomainsByFlowRequest.py
--rw-r--r--   0 root         (0) root         (0)     1304 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeUserCertificateExpireCountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeUserConfigsRequest.py
--rw-r--r--   0 root         (0) root         (0)     4459 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeUserDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1268 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeUserTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeUserUsageDataExportTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1680 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeUserUsageDetailDataExportTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeUserVipsByDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1469 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeVerifyContentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1454 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DisableRealtimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/EnableRealtimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1462 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/ListDomainsByLogConfigIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     1697 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/ListFCTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1814 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/ListRealtimeLogDeliveryDomainsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1291 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/ListRealtimeLogDeliveryInfosRequest.py
--rw-r--r--   0 root         (0) root         (0)     1281 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/ListUserCustomLogConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2444 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/ModifyCdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1666 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/ModifyCdnDomainSchdmByPropertyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1971 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/ModifyRealtimeLogDeliveryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1881 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/OpenCdnServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1491 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/PublishStagingConfigToProductionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2368 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/PushObjectCacheRequest.py
--rw-r--r--   0 root         (0) root         (0)     2034 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/RefreshObjectCachesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1469 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/RollbackStagingConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1712 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/SetCdnDomainCSRCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2267 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/SetCdnDomainSMCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/SetCdnDomainStagingConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     3087 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/SetDomainServerCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2326 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/SetReqHeaderConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2368 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/SetWaitingRoomConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/StartCdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     1831 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/StopCdnDomainRequest.py
--rw-r--r--   0 root         (0) root         (0)     2152 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2130 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2322 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/UpdateCdnDeliverTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1998 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/UpdateCdnSubTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2169 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/UpdateFCTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/VerifyDomainOwnerRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-03-29 08:06:59.000000 aliyun-python-sdk-cdn-3.8.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2452 2023-03-29 08:06:58.000000 aliyun-python-sdk-cdn-3.8.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyun_python_sdk_cdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyun_python_sdk_cdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10526 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyun_python_sdk_cdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyun_python_sdk_cdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyun_python_sdk_cdn.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyun_python_sdk_cdn.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/
+-rw-r--r--   0 root         (0) root         (0)     3573 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/AddCdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/AddFCTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/BatchAddCdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2275 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/BatchDeleteCdnDomainConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/BatchSetCdnDomainConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3108 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/BatchSetCdnDomainServerCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/BatchStartCdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/BatchStopCdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2454 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/BatchUpdateCdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2730 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/CreateCdnCertificateSigningRequestRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2142 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/CreateCdnDeliverTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/CreateCdnSubTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/CreateIllegalUrlExportTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1971 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/CreateRealTimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2527 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/CreateUsageDetailDataExportTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/CreateUserUsageDataExportTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DeleteCdnDeliverTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DeleteCdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DeleteCdnSubTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DeleteFCTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1804 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DeleteRealTimeLogLogstoreRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1971 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DeleteRealtimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2024 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DeleteSpecificConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DeleteSpecificStagingConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DeleteUsageDetailDataExportTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DeleteUserUsageDataExportTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeBlockedRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnCertificateDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnCertificateListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnDeletedDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1461 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnDeliverListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnDomainByCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2241 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnDomainConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnDomainDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnDomainLogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnDomainStagingConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1835 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnHttpsDomainListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnOrderCommodityCodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnRegionAndIspRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnReportListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1889 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnSMCertificateDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1861 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnSMCertificateListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnSubListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillHistoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillPredictionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnUserConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnUserDomainsByFuncRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnUserQuotaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnUserResourcePackageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnWafDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCertificateInfoByIDRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCustomLogConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainAverageResponseTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2581 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataByLayerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2064 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataByTimeStampRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2406 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainCcActivityLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainCertificateInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainCnameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainCustomLogConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainDetailDataByLayerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainHitRateDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2591 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainHttpCodeDataByLayerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainHttpCodeDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainISPDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2183 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainMax95BpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainMultiUsageDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2357 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainPathDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainPvDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2581 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainQpsDataByLayerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2406 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainQpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeBpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeByteHitRateDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2767 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeDetailDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeHttpCodeDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeQpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeReqHitRateDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcBpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcHttpCodeDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcTrafficDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeTrafficDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1468 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealtimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRegionDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2020 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainReqHitRateDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainSrcBpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainSrcHttpCodeDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainSrcQpsDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainSrcTopUrlVisitRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2020 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainSrcTrafficDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainTopClientIpVisitRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainTopReferVisitRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainTopUrlVisitRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2414 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainTrafficDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2684 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainUsageDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainUvDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainsBySourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1835 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainsUsageByDayRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeEsExceptionDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeEsExecuteDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeFCTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1459 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeIllegalUrlExportTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1407 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeIpInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeIpStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeL2VipsByDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribePreloadDetailByIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeRangeDataByLocateAndIspServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeRealtimeDeliveryAccRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeRefreshQuotaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1449 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeRefreshTaskByIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3514 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeRefreshTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeStagingIpRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeTopDomainsByFlowRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1304 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeUserCertificateExpireCountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeUserConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4459 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeUserDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeUserTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeUserUsageDataExportTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeUserUsageDetailDataExportTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeUserVipsByDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeVerifyContentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DisableRealtimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/EnableRealtimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1462 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/ListDomainsByLogConfigIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1697 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/ListFCTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/ListRealtimeLogDeliveryDomainsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1291 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/ListRealtimeLogDeliveryInfosRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/ListUserCustomLogConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/ModifyCdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/ModifyCdnDomainSchdmByPropertyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1971 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/ModifyRealtimeLogDeliveryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/OpenCdnServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1491 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/PublishStagingConfigToProductionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2368 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/PushObjectCacheRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/RefreshObjectCachesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/RollbackStagingConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/SetCdnDomainCSRCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/SetCdnDomainSMCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/SetCdnDomainStagingConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3087 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/SetDomainServerCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/SetReqHeaderConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2368 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/SetWaitingRoomConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/StartCdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/StopCdnDomainRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2130 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2322 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/UpdateCdnDeliverTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/UpdateCdnSubTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/UpdateFCTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/VerifyDomainOwnerRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-04-25 07:08:15.000000 aliyun-python-sdk-cdn-3.8.6/setup.py
```

### Comparing `aliyun-python-sdk-cdn-3.8.5/LICENSE` & `aliyun-python-sdk-cdn-3.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/PKG-INFO` & `aliyun-python-sdk-cdn-3.8.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-cdn
-Version: 3.8.5
+Version: 3.8.6
 Summary: The cdn module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-cdn
```

### Comparing `aliyun-python-sdk-cdn-3.8.5/README.rst` & `aliyun-python-sdk-cdn-3.8.6/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyun_python_sdk_cdn.egg-info/PKG-INFO` & `aliyun-python-sdk-cdn-3.8.6/aliyun_python_sdk_cdn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-cdn
-Version: 3.8.5
+Version: 3.8.6
 Summary: The cdn module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-cdn
```

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyun_python_sdk_cdn.egg-info/SOURCES.txt` & `aliyun-python-sdk-cdn-3.8.6/aliyun_python_sdk_cdn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/endpoint.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/AddCdnDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/AddCdnDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/AddFCTriggerRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/AddFCTriggerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/BatchAddCdnDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/BatchAddCdnDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/BatchDeleteCdnDomainConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/BatchDeleteCdnDomainConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/BatchSetCdnDomainConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/BatchSetCdnDomainConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/BatchSetCdnDomainServerCertificateRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/BatchSetCdnDomainServerCertificateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/BatchStartCdnDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/BatchStartCdnDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/BatchStopCdnDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/BatchStopCdnDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/BatchUpdateCdnDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/BatchUpdateCdnDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/CreateCdnCertificateSigningRequestRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/CreateCdnCertificateSigningRequestRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/CreateCdnDeliverTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/CreateCdnDeliverTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/CreateCdnSubTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/CreateCdnSubTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/CreateIllegalUrlExportTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/CreateIllegalUrlExportTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/CreateRealTimeLogDeliveryRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/CreateRealTimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/CreateUsageDetailDataExportTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/CreateUsageDetailDataExportTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/CreateUserUsageDataExportTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/CreateUserUsageDataExportTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DeleteCdnDeliverTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DeleteCdnDeliverTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DeleteCdnDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DeleteCdnDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DeleteCdnSubTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DeleteCdnSubTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DeleteFCTriggerRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DeleteFCTriggerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DeleteRealTimeLogLogstoreRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DeleteRealTimeLogLogstoreRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DeleteRealtimeLogDeliveryRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DeleteRealtimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DeleteSpecificConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DeleteSpecificConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DeleteSpecificStagingConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DeleteSpecificStagingConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DeleteUsageDetailDataExportTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DeleteUsageDetailDataExportTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DeleteUserUsageDataExportTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DeleteUserUsageDataExportTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeBlockedRegionsRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeBlockedRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnCertificateDetailRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnCertificateDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnCertificateListRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnCertificateListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnDeletedDomainsRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnDeletedDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnDeliverListRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnDeliverListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnDomainByCertificateRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnDomainByCertificateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnDomainConfigsRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnDomainConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnDomainDetailRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnDomainDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnDomainLogsRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnDomainLogsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnDomainStagingConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnDomainStagingConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnHttpsDomainListRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnHttpsDomainListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnOrderCommodityCodeRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnOrderCommodityCodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnRegionAndIspRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnRegionAndIspRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnReportListRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnReportListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnReportRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnReportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnSMCertificateDetailRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnSMCertificateDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnSMCertificateListRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnSMCertificateListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnServiceRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnSubListRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnSubListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillHistoryRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillHistoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillPredictionRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillPredictionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillTypeRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnUserBillTypeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnUserConfigsRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnUserConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnUserDomainsByFuncRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnUserDomainsByFuncRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnUserQuotaRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnUserQuotaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnUserResourcePackageRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnUserResourcePackageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCdnWafDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCdnWafDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCertificateInfoByIDRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCertificateInfoByIDRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeCustomLogConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeCustomLogConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainAverageResponseTimeRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainAverageResponseTimeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataByLayerRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataByLayerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataByTimeStampRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataByTimeStampRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainBpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainCcActivityLogRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainCcActivityLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainCertificateInfoRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainCertificateInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainCnameRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainCnameRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainCustomLogConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainCustomLogConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainDetailDataByLayerRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainDetailDataByLayerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainHitRateDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainHitRateDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainHttpCodeDataByLayerRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainHttpCodeDataByLayerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainHttpCodeDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainHttpCodeDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainISPDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainISPDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainMax95BpsDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainMax95BpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainMultiUsageDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainMultiUsageDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainPathDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainPathDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainPvDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainPvDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainQpsDataByLayerRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainQpsDataByLayerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainQpsDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainQpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeBpsDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeBpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeByteHitRateDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeByteHitRateDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeDetailDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeDetailDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeHttpCodeDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeHttpCodeDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeQpsDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeQpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeReqHitRateDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeReqHitRateDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcBpsDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcBpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcHttpCodeDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcHttpCodeDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcTrafficDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeSrcTrafficDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeTrafficDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealTimeTrafficDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRealtimeLogDeliveryRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRealtimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainRegionDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainRegionDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainReqHitRateDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainReqHitRateDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainSrcBpsDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainSrcBpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainSrcHttpCodeDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainSrcHttpCodeDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainSrcQpsDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainSrcQpsDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainSrcTopUrlVisitRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainSrcTopUrlVisitRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainSrcTrafficDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainSrcTrafficDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainTopClientIpVisitRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainTopClientIpVisitRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainTopReferVisitRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainTopReferVisitRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainTopUrlVisitRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainTopUrlVisitRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainTrafficDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainTrafficDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainUsageDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainUsageDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainUvDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainUvDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainsBySourceRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainsBySourceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeDomainsUsageByDayRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeDomainsUsageByDayRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeEsExceptionDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeEsExceptionDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeEsExecuteDataRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeEsExecuteDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeFCTriggerRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeFCTriggerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeIllegalUrlExportTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeIllegalUrlExportTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeIpInfoRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeIpInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeIpStatusRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeIpStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeL2VipsByDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeL2VipsByDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribePreloadDetailByIdRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribePreloadDetailByIdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeRangeDataByLocateAndIspServiceRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeRangeDataByLocateAndIspServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeRealtimeDeliveryAccRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeRealtimeDeliveryAccRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeRefreshQuotaRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeRefreshQuotaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeRefreshTaskByIdRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeRefreshTaskByIdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeRefreshTasksRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeRefreshTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeStagingIpRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeStagingIpRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeTagResourcesRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeTopDomainsByFlowRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeTopDomainsByFlowRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeUserCertificateExpireCountRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeUserCertificateExpireCountRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeUserConfigsRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeUserConfigsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeUserDomainsRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeUserDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeUserTagsRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeUserTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeUserUsageDataExportTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeUserUsageDataExportTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeUserUsageDetailDataExportTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeUserUsageDetailDataExportTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeUserVipsByDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeUserVipsByDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DescribeVerifyContentRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DescribeVerifyContentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/DisableRealtimeLogDeliveryRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/DisableRealtimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/EnableRealtimeLogDeliveryRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/EnableRealtimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/ListDomainsByLogConfigIdRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/ListDomainsByLogConfigIdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/ListFCTriggerRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/ListFCTriggerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/ListRealtimeLogDeliveryDomainsRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/ListRealtimeLogDeliveryDomainsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/ListRealtimeLogDeliveryInfosRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/ListRealtimeLogDeliveryInfosRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/ListUserCustomLogConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/ListUserCustomLogConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/ModifyCdnDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/ModifyCdnDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/ModifyCdnDomainSchdmByPropertyRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/ModifyCdnDomainSchdmByPropertyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/ModifyRealtimeLogDeliveryRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/ModifyRealtimeLogDeliveryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/OpenCdnServiceRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/OpenCdnServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/PublishStagingConfigToProductionRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/PublishStagingConfigToProductionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/PushObjectCacheRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/PushObjectCacheRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/RefreshObjectCachesRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/RefreshObjectCachesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/RollbackStagingConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/RollbackStagingConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/SetCdnDomainCSRCertificateRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/SetCdnDomainCSRCertificateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/SetCdnDomainSMCertificateRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/SetCdnDomainSMCertificateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/SetCdnDomainStagingConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/SetCdnDomainStagingConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/SetDomainServerCertificateRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/SetDomainServerCertificateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/SetReqHeaderConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/SetReqHeaderConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/SetWaitingRoomConfigRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/SetWaitingRoomConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/StartCdnDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/StartCdnDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/StopCdnDomainRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/StopCdnDomainRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/TagResourcesRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/TagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/UntagResourcesRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/UntagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/UpdateCdnDeliverTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/UpdateCdnDeliverTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/UpdateCdnSubTaskRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/UpdateCdnSubTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/UpdateFCTriggerRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/UpdateFCTriggerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/aliyunsdkcdn/request/v20180510/VerifyDomainOwnerRequest.py` & `aliyun-python-sdk-cdn-3.8.6/aliyunsdkcdn/request/v20180510/VerifyDomainOwnerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cdn-3.8.5/setup.py` & `aliyun-python-sdk-cdn-3.8.6/setup.py`

 * *Files identical despite different names*

