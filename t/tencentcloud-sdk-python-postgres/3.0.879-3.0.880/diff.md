# Comparing `tmp/tencentcloud-sdk-python-postgres-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-postgres-3.0.880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.879.tar", last modified: Fri Apr 21 00:57:42 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-postgres-3.0.880.tar", last modified: Mon Apr 24 03:24:25 2023, max compression
```

## Comparing `tencentcloud-sdk-python-postgres-3.0.879.tar` & `tencentcloud-sdk-python-postgres-3.0.880.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:57:42.000000 tencentcloud-sdk-python-postgres-3.0.879/
--rw-r--r--   0 root         (0) root         (0)      752 2023-04-21 00:57:42.000000 tencentcloud-sdk-python-postgres-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:57:42.000000 tencentcloud-sdk-python-postgres-3.0.879/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:57:42.000000 tencentcloud-sdk-python-postgres-3.0.879/tencentcloud/postgres/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:57:42.000000 tencentcloud-sdk-python-postgres-3.0.879/tencentcloud/postgres/v20170312/
--rw-r--r--   0 root         (0) root         (0)    81533 2023-04-21 00:57:42.000000 tencentcloud-sdk-python-postgres-3.0.879/tencentcloud/postgres/v20170312/postgres_client.py
--rw-r--r--   0 root         (0) root         (0)    20657 2023-04-21 00:57:42.000000 tencentcloud-sdk-python-postgres-3.0.879/tencentcloud/postgres/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:57:42.000000 tencentcloud-sdk-python-postgres-3.0.879/tencentcloud/postgres/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   270908 2023-04-21 00:57:42.000000 tencentcloud-sdk-python-postgres-3.0.879/tencentcloud/postgres/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:57:42.000000 tencentcloud-sdk-python-postgres-3.0.879/tencentcloud/postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:57:42.000000 tencentcloud-sdk-python-postgres-3.0.879/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-04-21 00:57:42.000000 tencentcloud-sdk-python-postgres-3.0.879/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-04-21 00:57:42.000000 tencentcloud-sdk-python-postgres-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:57:42.000000 tencentcloud-sdk-python-postgres-3.0.879/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:57:42.000000 tencentcloud-sdk-python-postgres-3.0.879/tencentcloud_sdk_python_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:57:42.000000 tencentcloud-sdk-python-postgres-3.0.879/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-04-21 00:57:42.000000 tencentcloud-sdk-python-postgres-3.0.879/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-04-21 00:57:42.000000 tencentcloud-sdk-python-postgres-3.0.879/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:57:42.000000 tencentcloud-sdk-python-postgres-3.0.879/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:24:25.000000 tencentcloud-sdk-python-postgres-3.0.880/
+-rw-r--r--   0 root         (0) root         (0)      752 2023-04-24 03:24:25.000000 tencentcloud-sdk-python-postgres-3.0.880/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:24:25.000000 tencentcloud-sdk-python-postgres-3.0.880/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:24:25.000000 tencentcloud-sdk-python-postgres-3.0.880/tencentcloud/postgres/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:24:25.000000 tencentcloud-sdk-python-postgres-3.0.880/tencentcloud/postgres/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    84591 2023-04-24 03:24:25.000000 tencentcloud-sdk-python-postgres-3.0.880/tencentcloud/postgres/v20170312/postgres_client.py
+-rw-r--r--   0 root         (0) root         (0)    20657 2023-04-24 03:24:25.000000 tencentcloud-sdk-python-postgres-3.0.880/tencentcloud/postgres/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:24:25.000000 tencentcloud-sdk-python-postgres-3.0.880/tencentcloud/postgres/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   277276 2023-04-24 03:24:25.000000 tencentcloud-sdk-python-postgres-3.0.880/tencentcloud/postgres/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:24:25.000000 tencentcloud-sdk-python-postgres-3.0.880/tencentcloud/postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:24:25.000000 tencentcloud-sdk-python-postgres-3.0.880/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-04-24 03:24:25.000000 tencentcloud-sdk-python-postgres-3.0.880/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-04-24 03:24:25.000000 tencentcloud-sdk-python-postgres-3.0.880/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:24:25.000000 tencentcloud-sdk-python-postgres-3.0.880/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:24:25.000000 tencentcloud-sdk-python-postgres-3.0.880/tencentcloud_sdk_python_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:24:25.000000 tencentcloud-sdk-python-postgres-3.0.880/tencentcloud_sdk_python_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-04-24 03:24:25.000000 tencentcloud-sdk-python-postgres-3.0.880/tencentcloud_sdk_python_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-04-24 03:24:25.000000 tencentcloud-sdk-python-postgres-3.0.880/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:24:25.000000 tencentcloud-sdk-python-postgres-3.0.880/tencentcloud_sdk_python_postgres.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.879/README.rst` & `tencentcloud-sdk-python-postgres-3.0.880/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.879/tencentcloud/postgres/v20170312/postgres_client.py` & `tencentcloud-sdk-python-postgres-3.0.880/tencentcloud/postgres/v20170312/postgres_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -528,14 +528,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeBackupDownloadRestriction(self, request):
+        """本接口（DescribeBackupDownloadRestriction）用于查询备份文件下载限制。
+
+        :param request: Request instance for DescribeBackupDownloadRestriction.
+        :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeBackupDownloadRestrictionRequest`
+        :rtype: :class:`tencentcloud.postgres.v20170312.models.DescribeBackupDownloadRestrictionResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeBackupDownloadRestriction", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeBackupDownloadRestrictionResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeBackupDownloadURL(self, request):
         """本接口 (DescribeBackupDownloadURL) 用于获取备份下载链接。
 
         :param request: Request instance for DescribeBackupDownloadURL.
         :type request: :class:`tencentcloud.postgres.v20170312.models.DescribeBackupDownloadURLRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.DescribeBackupDownloadURLResponse`
 
@@ -1425,14 +1448,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ModifyBackupDownloadRestriction(self, request):
+        """本接口（ModifyBackupDownloadRestriction）用于修改备份文件下载限制。
+
+        :param request: Request instance for ModifyBackupDownloadRestriction.
+        :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyBackupDownloadRestrictionRequest`
+        :rtype: :class:`tencentcloud.postgres.v20170312.models.ModifyBackupDownloadRestrictionResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyBackupDownloadRestriction", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyBackupDownloadRestrictionResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ModifyBackupPlan(self, request):
         """本接口 (ModifyBackupPlan) 用于实例备份计划的修改，默认是在每天的凌晨开始全量备份，备份保留时长是7天。可以根据此接口指定时间进行实例的备份。
 
         :param request: Request instance for ModifyBackupPlan.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyBackupPlanRequest`
         :rtype: :class:`tencentcloud.postgres.v20170312.models.ModifyBackupPlanResponse`
 
@@ -1469,14 +1515,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ModifyDBInstanceChargeType(self, request):
+        """支持实例的计费类型转换（目前仅支持按量计费转包年包月）
+
+        :param request: Request instance for ModifyDBInstanceChargeType.
+        :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyDBInstanceChargeTypeRequest`
+        :rtype: :class:`tencentcloud.postgres.v20170312.models.ModifyDBInstanceChargeTypeResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyDBInstanceChargeType", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyDBInstanceChargeTypeResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifyDBInstanceDeployment(self, request):
         """本接口（ModifyDBInstanceDeployment）用于修改节点可用区部署方式，仅支持主实例。
 
         :param request: Request instance for ModifyDBInstanceDeployment.
         :type request: :class:`tencentcloud.postgres.v20170312.models.ModifyDBInstanceDeploymentRequest`
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.879/tencentcloud/postgres/v20170312/errorcodes.py` & `tencentcloud-sdk-python-postgres-3.0.880/tencentcloud/postgres/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.879/tencentcloud/postgres/v20170312/models.py` & `tencentcloud-sdk-python-postgres-3.0.880/tencentcloud/postgres/v20170312/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2306,14 +2306,61 @@
 
     def _deserialize(self, params):
         self.RecoveryBeginTime = params.get("RecoveryBeginTime")
         self.RecoveryEndTime = params.get("RecoveryEndTime")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeBackupDownloadRestrictionRequest(AbstractModel):
+    """DescribeBackupDownloadRestriction请求参数结构体
+
+    """
+
+
+class DescribeBackupDownloadRestrictionResponse(AbstractModel):
+    """DescribeBackupDownloadRestriction返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RestrictionType: 备份文件下载限制类型，NONE 无限制，内外网都可以下载；INTRANET 只允许内网下载；CUSTOMIZE 自定义限制下载的vpc或ip。
+        :type RestrictionType: str
+        :param VpcRestrictionEffect: vpc限制效力，ALLOW 允许；DENY 拒绝。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcRestrictionEffect: str
+        :param VpcIdSet: 允许或拒绝下载备份文件的vpcId列表。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VpcIdSet: list of str
+        :param IpRestrictionEffect: ip限制效力，ALLOW 允许；DENY 拒绝。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IpRestrictionEffect: str
+        :param IpSet: 允许或拒绝下载备份文件的ip列表。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IpSet: list of str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RestrictionType = None
+        self.VpcRestrictionEffect = None
+        self.VpcIdSet = None
+        self.IpRestrictionEffect = None
+        self.IpSet = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RestrictionType = params.get("RestrictionType")
+        self.VpcRestrictionEffect = params.get("VpcRestrictionEffect")
+        self.VpcIdSet = params.get("VpcIdSet")
+        self.IpRestrictionEffect = params.get("IpRestrictionEffect")
+        self.IpSet = params.get("IpSet")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeBackupDownloadURLRequest(AbstractModel):
     """DescribeBackupDownloadURL请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5078,14 +5125,71 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class ModifyBackupDownloadRestrictionRequest(AbstractModel):
+    """ModifyBackupDownloadRestriction请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RestrictionType: 备份文件下载限制类型，NONE 无限制，内外网都可以下载；INTRANET 只允许内网下载；CUSTOMIZE 自定义限制下载的vpc或ip。
+        :type RestrictionType: str
+        :param VpcRestrictionEffect: vpc限制效力，ALLOW 允许；DENY 拒绝。
+        :type VpcRestrictionEffect: str
+        :param VpcIdSet: 允许或拒绝下载备份文件的vpcId列表。
+        :type VpcIdSet: list of str
+        :param IpRestrictionEffect: ip限制效力，ALLOW 允许；DENY 拒绝。
+        :type IpRestrictionEffect: str
+        :param IpSet: 允许或拒绝下载备份文件的ip列表。
+        :type IpSet: list of str
+        """
+        self.RestrictionType = None
+        self.VpcRestrictionEffect = None
+        self.VpcIdSet = None
+        self.IpRestrictionEffect = None
+        self.IpSet = None
+
+
+    def _deserialize(self, params):
+        self.RestrictionType = params.get("RestrictionType")
+        self.VpcRestrictionEffect = params.get("VpcRestrictionEffect")
+        self.VpcIdSet = params.get("VpcIdSet")
+        self.IpRestrictionEffect = params.get("IpRestrictionEffect")
+        self.IpSet = params.get("IpSet")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyBackupDownloadRestrictionResponse(AbstractModel):
+    """ModifyBackupDownloadRestriction返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class ModifyBackupPlanRequest(AbstractModel):
     """ModifyBackupPlan请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -5184,14 +5288,75 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class ModifyDBInstanceChargeTypeRequest(AbstractModel):
+    """ModifyDBInstanceChargeType请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DBInstanceId: 实例ID，形如postgres-6fego161
+        :type DBInstanceId: str
+        :param InstanceChargeType: 实例计费类型。目前支持：PREPAID（预付费，即包年包月），POSTPAID_BY_HOUR（后付费，即按量计费）。默认值：PREPAID。
+        :type InstanceChargeType: str
+        :param Period: 购买时长，单位：月。目前只支持1,2,3,4,5,6,7,8,9,10,11,12,24,36这些值，按量计费模式下该参数传1。
+        :type Period: int
+        :param AutoRenewFlag: 续费标记：0-正常续费（默认）；1-自动续费。
+        :type AutoRenewFlag: int
+        :param AutoVoucher: 是否自动使用代金券,1是,0否，默认不使用
+        :type AutoVoucher: int
+        """
+        self.DBInstanceId = None
+        self.InstanceChargeType = None
+        self.Period = None
+        self.AutoRenewFlag = None
+        self.AutoVoucher = None
+
+
+    def _deserialize(self, params):
+        self.DBInstanceId = params.get("DBInstanceId")
+        self.InstanceChargeType = params.get("InstanceChargeType")
+        self.Period = params.get("Period")
+        self.AutoRenewFlag = params.get("AutoRenewFlag")
+        self.AutoVoucher = params.get("AutoVoucher")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyDBInstanceChargeTypeResponse(AbstractModel):
+    """ModifyDBInstanceChargeType返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DealName: 订单名
+        :type DealName: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.DealName = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.DealName = params.get("DealName")
+        self.RequestId = params.get("RequestId")
+
+
 class ModifyDBInstanceDeploymentRequest(AbstractModel):
     """ModifyDBInstanceDeployment请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-postgres-3.0.880/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.879'
+__version__ = '3.0.880'
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.880/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-postgres-3.0.879/setup.py` & `tencentcloud-sdk-python-postgres-3.0.880/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-postgres-3.0.879/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO` & `tencentcloud-sdk-python-postgres-3.0.880/tencentcloud_sdk_python_postgres.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-postgres
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Postgres SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

