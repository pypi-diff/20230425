# Comparing `tmp/aliyun-python-sdk-alikafka-1.0.4.tar.gz` & `tmp/aliyun-python-sdk-alikafka-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-alikafka-1.0.4.tar", last modified: Wed Dec 14 03:32:38 2022, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-alikafka-1.0.5.tar", last modified: Tue Apr 25 11:50:10 2023, max compression
```

## Comparing `aliyun-python-sdk-alikafka-1.0.4.tar` & `aliyun-python-sdk-alikafka-1.0.5.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 03:32:38.000000 aliyun-python-sdk-alikafka-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      575 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1562 2022-12-14 03:32:38.000000 aliyun-python-sdk-alikafka-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      537 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 03:32:38.000000 aliyun-python-sdk-alikafka-1.0.4/aliyun_python_sdk_alikafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1562 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyun_python_sdk_alikafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2697 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyun_python_sdk_alikafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyun_python_sdk_alikafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyun_python_sdk_alikafka.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyun_python_sdk_alikafka.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 03:32:38.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 03:32:38.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 03:32:38.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/
--rw-r--r--   0 root         (0) root         (0)     1725 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/ChangeResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1667 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/ConvertPostPayOrderRequest.py
--rw-r--r--   0 root         (0) root         (0)     2577 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/CreateAclRequest.py
--rw-r--r--   0 root         (0) root         (0)     2263 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/CreateConsumerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     3580 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/CreatePostPayOrderRequest.py
--rw-r--r--   0 root         (0) root         (0)     3578 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/CreatePrePayOrderRequest.py
--rw-r--r--   0 root         (0) root         (0)     1989 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/CreateSaslUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     3443 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/CreateTopicRequest.py
--rw-r--r--   0 root         (0) root         (0)     2577 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/DeleteAclRequest.py
--rw-r--r--   0 root         (0) root         (0)     1677 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/DeleteConsumerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1476 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/DeleteInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1810 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/DeleteSaslUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     1631 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/DeleteTopicRequest.py
--rw-r--r--   0 root         (0) root         (0)     2356 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/DescribeAclsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1482 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/DescribeSaslUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1297 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/GetAllInstanceIdListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1480 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/GetAllowedIpListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1669 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/GetConsumerListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1677 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/GetConsumerProgressRequest.py
--rw-r--r--   0 root         (0) root         (0)     2370 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/GetInstanceListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1470 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/GetQuotaTipRequest.py
--rw-r--r--   0 root         (0) root         (0)     2009 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/GetTopicListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1637 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/GetTopicStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2366 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1687 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/ModifyInstanceNameRequest.py
--rw-r--r--   0 root         (0) root         (0)     1868 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/ModifyPartitionNumRequest.py
--rw-r--r--   0 root         (0) root         (0)     1810 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/ModifyTopicRemarkRequest.py
--rw-r--r--   0 root         (0) root         (0)     1725 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/ReleaseInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     4763 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/StartInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2364 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2151 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2481 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/UpdateAllowedIpRequest.py
--rw-r--r--   0 root         (0) root         (0)     1655 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/UpdateInstanceConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1701 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/UpgradeInstanceVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2942 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/UpgradePostPayOrderRequest.py
--rw-r--r--   0 root         (0) root         (0)     2940 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/UpgradePrePayOrderRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2022-12-14 03:32:38.000000 aliyun-python-sdk-alikafka-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2477 2022-12-14 03:32:37.000000 aliyun-python-sdk-alikafka-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      537 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyun_python_sdk_alikafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyun_python_sdk_alikafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2764 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyun_python_sdk_alikafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyun_python_sdk_alikafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyun_python_sdk_alikafka.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyun_python_sdk_alikafka.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/
+-rw-r--r--   0 root         (0) root         (0)     1714 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ChangeResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ConvertPostPayOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreateAclRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreateConsumerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3569 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreatePostPayOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3567 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreatePrePayOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreateSaslUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3432 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreateTopicRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DeleteAclRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DeleteConsumerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DeleteInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DeleteSaslUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DeleteTopicRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DescribeAclsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DescribeSaslUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetAllInstanceIdListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetAllowedIpListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetConsumerListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetConsumerProgressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetInstanceListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1459 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetQuotaTipRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetTopicListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetTopicStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ModifyInstanceNameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ModifyPartitionNumRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ModifyTopicRemarkRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1714 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ReleaseInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4752 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/StartInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2353 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2470 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpdateAllowedIpRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpdateConsumerOffsetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpdateInstanceConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpgradeInstanceVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2931 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpgradePostPayOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2929 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpgradePrePayOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/setup.py
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/LICENSE` & `aliyun-python-sdk-alikafka-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alikafka-1.0.4/PKG-INFO` & `aliyun-python-sdk-alikafka-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-alikafka
-Version: 1.0.4
+Version: 1.0.5
 Summary: The alikafka module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-alikafka
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/README.rst` & `aliyun-python-sdk-alikafka-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyun_python_sdk_alikafka.egg-info/PKG-INFO` & `aliyun-python-sdk-alikafka-1.0.5/aliyun_python_sdk_alikafka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-alikafka
-Version: 1.0.4
+Version: 1.0.5
 Summary: The alikafka module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-alikafka
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyun_python_sdk_alikafka.egg-info/SOURCES.txt` & `aliyun-python-sdk-alikafka-1.0.5/aliyun_python_sdk_alikafka.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,12 +39,13 @@
 aliyunsdkalikafka/request/v20190916/ModifyPartitionNumRequest.py
 aliyunsdkalikafka/request/v20190916/ModifyTopicRemarkRequest.py
 aliyunsdkalikafka/request/v20190916/ReleaseInstanceRequest.py
 aliyunsdkalikafka/request/v20190916/StartInstanceRequest.py
 aliyunsdkalikafka/request/v20190916/TagResourcesRequest.py
 aliyunsdkalikafka/request/v20190916/UntagResourcesRequest.py
 aliyunsdkalikafka/request/v20190916/UpdateAllowedIpRequest.py
+aliyunsdkalikafka/request/v20190916/UpdateConsumerOffsetRequest.py
 aliyunsdkalikafka/request/v20190916/UpdateInstanceConfigRequest.py
 aliyunsdkalikafka/request/v20190916/UpgradeInstanceVersionRequest.py
 aliyunsdkalikafka/request/v20190916/UpgradePostPayOrderRequest.py
 aliyunsdkalikafka/request/v20190916/UpgradePrePayOrderRequest.py
 aliyunsdkalikafka/request/v20190916/__init__.py
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/endpoint.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/ChangeResourceGroupRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ChangeResourceGroupRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class ChangeResourceGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ChangeResourceGroup','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ChangeResourceGroup')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/ConvertPostPayOrderRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ConvertPostPayOrderRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class ConvertPostPayOrderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ConvertPostPayOrder','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ConvertPostPayOrder')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/CreateAclRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreateAclRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class CreateAclRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreateAcl','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreateAcl')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/CreateConsumerGroupRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreateConsumerGroupRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class CreateConsumerGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreateConsumerGroup','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreateConsumerGroup')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/CreatePostPayOrderRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreatePostPayOrderRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class CreatePostPayOrderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreatePostPayOrder','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreatePostPayOrder')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/CreatePrePayOrderRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreatePrePayOrderRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class CreatePrePayOrderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreatePrePayOrder','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreatePrePayOrder')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/CreateSaslUserRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreateSaslUserRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class CreateSaslUserRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreateSaslUser','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreateSaslUser')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/CreateTopicRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreateTopicRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class CreateTopicRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreateTopic','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreateTopic')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/DeleteAclRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DeleteAclRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class DeleteAclRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DeleteAcl','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DeleteAcl')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/DeleteConsumerGroupRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DeleteConsumerGroupRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class DeleteConsumerGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DeleteConsumerGroup','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DeleteConsumerGroup')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/DeleteInstanceRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ReleaseInstanceRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,23 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
-class DeleteInstanceRequest(RpcRequest):
+class ReleaseInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DeleteInstance','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ReleaseInstance')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ForceDeleteInstance(self): # Boolean
+		return self.get_query_params().get('ForceDeleteInstance')
+
+	def set_ForceDeleteInstance(self, ForceDeleteInstance):  # Boolean
+		self.add_query_param('ForceDeleteInstance', ForceDeleteInstance)
 	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/DeleteSaslUserRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DeleteSaslUserRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class DeleteSaslUserRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DeleteSaslUser','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DeleteSaslUser')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/DeleteTopicRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetTopicStatusRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
-class DeleteTopicRequest(RpcRequest):
+class GetTopicStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DeleteTopic','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetTopicStatus')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/DescribeAclsRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DescribeAclsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class DescribeAclsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DescribeAcls','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DescribeAcls')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/DescribeSaslUsersRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DescribeSaslUsersRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class DescribeSaslUsersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DescribeSaslUsers','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DescribeSaslUsers')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/GetAllInstanceIdListRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetAllInstanceIdListRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class GetAllInstanceIdListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetAllInstanceIdList','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetAllInstanceIdList')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/GetAllowedIpListRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetAllowedIpListRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class GetAllowedIpListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetAllowedIpList','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetAllowedIpList')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/GetConsumerListRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetConsumerListRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class GetConsumerListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetConsumerList','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetConsumerList')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/GetConsumerProgressRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetConsumerProgressRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class GetConsumerProgressRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetConsumerProgress','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetConsumerProgress')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/GetInstanceListRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetInstanceListRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class GetInstanceListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetInstanceList','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetInstanceList')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/GetQuotaTipRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DeleteInstanceRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
-class GetQuotaTipRequest(RpcRequest):
+class DeleteInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetQuotaTip','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DeleteInstance')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/GetTopicListRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetTopicListRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class GetTopicListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetTopicList','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetTopicList')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/GetTopicStatusRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ModifyTopicRemarkRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
-class GetTopicStatusRequest(RpcRequest):
+class ModifyTopicRemarkRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetTopicStatus','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ModifyTopicRemark')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,7 +37,12 @@
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
 	def get_Topic(self): # String
 		return self.get_query_params().get('Topic')
 
 	def set_Topic(self, Topic):  # String
 		self.add_query_param('Topic', Topic)
+	def get_Remark(self): # String
+		return self.get_query_params().get('Remark')
+
+	def set_Remark(self, Remark):  # String
+		self.add_query_param('Remark', Remark)
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/ListTagResourcesRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ListTagResourcesRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class ListTagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ListTagResources','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ListTagResources')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/ModifyInstanceNameRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ModifyInstanceNameRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class ModifyInstanceNameRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ModifyInstanceName','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ModifyInstanceName')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/ModifyPartitionNumRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ModifyPartitionNumRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class ModifyPartitionNumRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ModifyPartitionNum','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ModifyPartitionNum')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/ModifyTopicRemarkRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DeleteTopicRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
-class ModifyTopicRemarkRequest(RpcRequest):
+class DeleteTopicRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ModifyTopicRemark','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DeleteTopic')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,12 +37,7 @@
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
 	def get_Topic(self): # String
 		return self.get_query_params().get('Topic')
 
 	def set_Topic(self, Topic):  # String
 		self.add_query_param('Topic', Topic)
-	def get_Remark(self): # String
-		return self.get_query_params().get('Remark')
-
-	def set_Remark(self, Remark):  # String
-		self.add_query_param('Remark', Remark)
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/ReleaseInstanceRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetQuotaTipRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,28 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
-class ReleaseInstanceRequest(RpcRequest):
+class GetQuotaTipRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ReleaseInstance','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetQuotaTip')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ForceDeleteInstance(self): # Boolean
-		return self.get_query_params().get('ForceDeleteInstance')
-
-	def set_ForceDeleteInstance(self, ForceDeleteInstance):  # Boolean
-		self.add_query_param('ForceDeleteInstance', ForceDeleteInstance)
 	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/StartInstanceRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/StartInstanceRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class StartInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'StartInstance','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'StartInstance')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/TagResourcesRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/TagResourcesRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class TagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'TagResources','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'TagResources')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/UntagResourcesRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UntagResourcesRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class UntagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UntagResources','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UntagResources')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/UpdateAllowedIpRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpdateAllowedIpRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class UpdateAllowedIpRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpdateAllowedIp','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpdateAllowedIp')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/UpdateInstanceConfigRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpdateInstanceConfigRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class UpdateInstanceConfigRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpdateInstanceConfig','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpdateInstanceConfig')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/UpgradeInstanceVersionRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpgradeInstanceVersionRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class UpgradeInstanceVersionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpgradeInstanceVersion','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpgradeInstanceVersion')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/UpgradePostPayOrderRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpgradePostPayOrderRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class UpgradePostPayOrderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpgradePostPayOrder','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpgradePostPayOrder')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/aliyunsdkalikafka/request/v20190916/UpgradePrePayOrderRequest.py` & `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpgradePrePayOrderRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class UpgradePrePayOrderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpgradePrePayOrder','alikafka')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpgradePrePayOrder')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.4/setup.py` & `aliyun-python-sdk-alikafka-1.0.5/setup.py`

 * *Files identical despite different names*

