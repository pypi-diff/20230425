# Comparing `tmp/tencentcloud-sdk-python-cvm-3.0.880.tar.gz` & `tmp/tencentcloud-sdk-python-cvm-3.0.881.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.880.tar", last modified: Mon Apr 24 03:01:32 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.881.tar", last modified: Tue Apr 25 00:34:25 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cvm-3.0.880.tar` & `tencentcloud-sdk-python-cvm-3.0.881.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:01:32.000000 tencentcloud-sdk-python-cvm-3.0.880/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 03:01:32.000000 tencentcloud-sdk-python-cvm-3.0.880/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:01:32.000000 tencentcloud-sdk-python-cvm-3.0.880/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:01:32.000000 tencentcloud-sdk-python-cvm-3.0.880/tencentcloud/cvm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:01:32.000000 tencentcloud-sdk-python-cvm-3.0.880/tencentcloud/cvm/v20170312/
--rw-r--r--   0 root         (0) root         (0)   119282 2023-04-24 03:01:32.000000 tencentcloud-sdk-python-cvm-3.0.880/tencentcloud/cvm/v20170312/cvm_client.py
--rw-r--r--   0 root         (0) root         (0)    42551 2023-04-24 03:01:32.000000 tencentcloud-sdk-python-cvm-3.0.880/tencentcloud/cvm/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:01:32.000000 tencentcloud-sdk-python-cvm-3.0.880/tencentcloud/cvm/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   429673 2023-04-24 03:01:32.000000 tencentcloud-sdk-python-cvm-3.0.880/tencentcloud/cvm/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:01:32.000000 tencentcloud-sdk-python-cvm-3.0.880/tencentcloud/cvm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:01:32.000000 tencentcloud-sdk-python-cvm-3.0.880/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:01:32.000000 tencentcloud-sdk-python-cvm-3.0.880/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 03:01:32.000000 tencentcloud-sdk-python-cvm-3.0.880/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:01:32.000000 tencentcloud-sdk-python-cvm-3.0.880/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:01:32.000000 tencentcloud-sdk-python-cvm-3.0.880/tencentcloud_sdk_python_cvm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:01:32.000000 tencentcloud-sdk-python-cvm-3.0.880/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-24 03:01:32.000000 tencentcloud-sdk-python-cvm-3.0.880/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:01:32.000000 tencentcloud-sdk-python-cvm-3.0.880/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:01:32.000000 tencentcloud-sdk-python-cvm-3.0.880/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/cvm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/cvm/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   119282 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/cvm/v20170312/cvm_client.py
+-rw-r--r--   0 root         (0) root         (0)    42810 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/cvm/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/cvm/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   429673 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/cvm/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/cvm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud_sdk_python_cvm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:34:25.000000 tencentcloud-sdk-python-cvm-3.0.881/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.880/README.rst` & `tencentcloud-sdk-python-cvm-3.0.881/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.880/tencentcloud/cvm/v20170312/cvm_client.py` & `tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/cvm/v20170312/cvm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.880/tencentcloud/cvm/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/cvm/v20170312/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,14 +391,17 @@
 
 # 镜像不允许执行该操作
 INVALIDPARAMETERVALUE_INVALIDIMAGEID = 'InvalidParameterValue.InvalidImageId'
 
 # 镜像无法用于重装当前实例。
 INVALIDPARAMETERVALUE_INVALIDIMAGEIDFORRETSETINSTANCE = 'InvalidParameterValue.InvalidImageIdForRetsetInstance'
 
+# 指定的镜像ID为共享镜像。
+INVALIDPARAMETERVALUE_INVALIDIMAGEIDISSHARED = 'InvalidParameterValue.InvalidImageIdIsShared'
+
 # 当前地域不支持指定镜像所包含的操作系统。
 INVALIDPARAMETERVALUE_INVALIDIMAGEOSNAME = 'InvalidParameterValue.InvalidImageOsName'
 
 # 镜像被其他操作占用，请检查，并稍后重试。
 INVALIDPARAMETERVALUE_INVALIDIMAGESTATE = 'InvalidParameterValue.InvalidImageState'
 
 # 该实例配置来自免费升配活动，暂不支持3个月内进行降配。
@@ -679,14 +682,17 @@
 
 # 云盘参数不符合规范
 RESOURCEINSUFFICIENT_CLOUDDISKUNAVAILABLE = 'ResourceInsufficient.CloudDiskUnavailable'
 
 # 实例个数超过容灾组的配额
 RESOURCEINSUFFICIENT_DISASTERRECOVERGROUPCVMQUOTA = 'ResourceInsufficient.DisasterRecoverGroupCvmQuota'
 
+# 安全组资源配额不足。
+RESOURCEINSUFFICIENT_INSUFFICIENTGROUPQUOTA = 'ResourceInsufficient.InsufficientGroupQuota'
+
 # 指定的实例类型库存不足。
 RESOURCEINSUFFICIENT_SPECIFIEDINSTANCETYPE = 'ResourceInsufficient.SpecifiedInstanceType'
 
 # 指定的实例类型在选择的可用区已售罄。
 RESOURCEINSUFFICIENT_ZONESOLDOUTFORSPECIFIEDINSTANCE = 'ResourceInsufficient.ZoneSoldOutForSpecifiedInstance'
 
 # 高性能计算集群不存在。
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.880/tencentcloud/cvm/v20170312/models.py` & `tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/cvm/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.880/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cvm-3.0.881/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.880'
+__version__ = '3.0.881'
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.880/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.881/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.880/setup.py` & `tencentcloud-sdk-python-cvm-3.0.881/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.880/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.881/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

