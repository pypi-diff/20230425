# Comparing `tmp/tencentcloud-sdk-python-tdmq-3.0.880.tar.gz` & `tmp/tencentcloud-sdk-python-tdmq-3.0.881.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.880.tar", last modified: Mon Apr 24 03:39:19 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.881.tar", last modified: Tue Apr 25 00:57:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdmq-3.0.880.tar` & `tencentcloud-sdk-python-tdmq-3.0.881.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/tdmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/tdmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/tdmq/v20200217/
--rw-r--r--   0 root         (0) root         (0)   101085 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/tdmq/v20200217/tdmq_client.py
--rw-r--r--   0 root         (0) root         (0)    10117 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/tdmq/v20200217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/tdmq/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)   374030 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/tdmq/v20200217/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud_sdk_python_tdmq.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:39:19.000000 tencentcloud-sdk-python-tdmq-3.0.880/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:57:02.000000 tencentcloud-sdk-python-tdmq-3.0.881/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-25 00:57:02.000000 tencentcloud-sdk-python-tdmq-3.0.881/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:57:02.000000 tencentcloud-sdk-python-tdmq-3.0.881/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:57:02.000000 tencentcloud-sdk-python-tdmq-3.0.881/tencentcloud/tdmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:57:02.000000 tencentcloud-sdk-python-tdmq-3.0.881/tencentcloud/tdmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:57:02.000000 tencentcloud-sdk-python-tdmq-3.0.881/tencentcloud/tdmq/v20200217/
+-rw-r--r--   0 root         (0) root         (0)   101085 2023-04-25 00:57:02.000000 tencentcloud-sdk-python-tdmq-3.0.881/tencentcloud/tdmq/v20200217/tdmq_client.py
+-rw-r--r--   0 root         (0) root         (0)    10117 2023-04-25 00:57:02.000000 tencentcloud-sdk-python-tdmq-3.0.881/tencentcloud/tdmq/v20200217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:57:02.000000 tencentcloud-sdk-python-tdmq-3.0.881/tencentcloud/tdmq/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   375961 2023-04-25 00:57:02.000000 tencentcloud-sdk-python-tdmq-3.0.881/tencentcloud/tdmq/v20200217/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:57:02.000000 tencentcloud-sdk-python-tdmq-3.0.881/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-25 00:57:02.000000 tencentcloud-sdk-python-tdmq-3.0.881/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:57:02.000000 tencentcloud-sdk-python-tdmq-3.0.881/tencentcloud_sdk_python_tdmq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:57:02.000000 tencentcloud-sdk-python-tdmq-3.0.881/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-25 00:57:02.000000 tencentcloud-sdk-python-tdmq-3.0.881/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-25 00:57:02.000000 tencentcloud-sdk-python-tdmq-3.0.881/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:57:02.000000 tencentcloud-sdk-python-tdmq-3.0.881/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-25 00:57:02.000000 tencentcloud-sdk-python-tdmq-3.0.881/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:57:02.000000 tencentcloud-sdk-python-tdmq-3.0.881/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.880/README.rst` & `tencentcloud-sdk-python-tdmq-3.0.881/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/tdmq/v20200217/tdmq_client.py` & `tencentcloud-sdk-python-tdmq-3.0.881/tencentcloud/tdmq/v20200217/tdmq_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/tdmq/v20200217/errorcodes.py` & `tencentcloud-sdk-python-tdmq-3.0.881/tencentcloud/tdmq/v20200217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/tdmq/v20200217/models.py` & `tencentcloud-sdk-python-tdmq-3.0.881/tencentcloud/tdmq/v20200217/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8650,14 +8650,17 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type Remark: str
         :param SpecName: 实例配置ID
         :type SpecName: str
         :param ExceptionInformation: 集群异常。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ExceptionInformation: str
+        :param ClusterStatus: 实例状态，0表示创建中，1表示正常，2表示隔离中，3表示已销毁，4 - 异常, 5 - 发货失败
+为了和计费区分开，额外开启一个状态位，用于显示。
+        :type ClusterStatus: int
         """
         self.InstanceId = None
         self.InstanceName = None
         self.InstanceVersion = None
         self.Status = None
         self.NodeCount = None
         self.ConfigDisplay = None
@@ -8666,14 +8669,15 @@
         self.MaxStorage = None
         self.ExpireTime = None
         self.AutoRenewFlag = None
         self.PayMode = None
         self.Remark = None
         self.SpecName = None
         self.ExceptionInformation = None
+        self.ClusterStatus = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.InstanceName = params.get("InstanceName")
         self.InstanceVersion = params.get("InstanceVersion")
         self.Status = params.get("Status")
@@ -8684,14 +8688,15 @@
         self.MaxStorage = params.get("MaxStorage")
         self.ExpireTime = params.get("ExpireTime")
         self.AutoRenewFlag = params.get("AutoRenewFlag")
         self.PayMode = params.get("PayMode")
         self.Remark = params.get("Remark")
         self.SpecName = params.get("SpecName")
         self.ExceptionInformation = params.get("ExceptionInformation")
+        self.ClusterStatus = params.get("ClusterStatus")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -9130,14 +9135,20 @@
         :type IsolateTime: int
         :param HttpPublicEndpoint: HTTP协议公网接入地址
 注意：此字段可能返回 null，表示取不到有效值。
         :type HttpPublicEndpoint: str
         :param HttpVpcEndpoint: HTTP协议VPC接入地址
 注意：此字段可能返回 null，表示取不到有效值。
         :type HttpVpcEndpoint: str
+        :param InternalEndpoint: TCP内部接入地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InternalEndpoint: str
+        :param HttpInternalEndpoint: HTTP协议内部接入地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type HttpInternalEndpoint: str
         """
         self.ClusterId = None
         self.ClusterName = None
         self.Region = None
         self.CreateTime = None
         self.Remark = None
         self.PublicEndPoint = None
@@ -9146,14 +9157,16 @@
         self.Vpcs = None
         self.IsVip = None
         self.RocketMQFlag = None
         self.Status = None
         self.IsolateTime = None
         self.HttpPublicEndpoint = None
         self.HttpVpcEndpoint = None
+        self.InternalEndpoint = None
+        self.HttpInternalEndpoint = None
 
 
     def _deserialize(self, params):
         self.ClusterId = params.get("ClusterId")
         self.ClusterName = params.get("ClusterName")
         self.Region = params.get("Region")
         self.CreateTime = params.get("CreateTime")
@@ -9169,14 +9182,16 @@
                 self.Vpcs.append(obj)
         self.IsVip = params.get("IsVip")
         self.RocketMQFlag = params.get("RocketMQFlag")
         self.Status = params.get("Status")
         self.IsolateTime = params.get("IsolateTime")
         self.HttpPublicEndpoint = params.get("HttpPublicEndpoint")
         self.HttpVpcEndpoint = params.get("HttpVpcEndpoint")
+        self.InternalEndpoint = params.get("InternalEndpoint")
+        self.HttpInternalEndpoint = params.get("HttpInternalEndpoint")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -9387,43 +9402,48 @@
 
     """
 
     def __init__(self):
         r"""
         :param NamespaceId: 命名空间名称，3-64个字符，只能包含字母、数字、“-”及“_”
         :type NamespaceId: str
-        :param Ttl: 未消费消息的保留时间，以毫秒单位，范围60秒到15天
+        :param Ttl: 已废弃，未消费消息的保留时间，以毫秒单位，范围60秒到15天
         :type Ttl: int
         :param RetentionTime: 消息持久化后保留的时间，以毫秒单位
         :type RetentionTime: int
         :param Remark: 说明
 注意：此字段可能返回 null，表示取不到有效值。
         :type Remark: str
         :param PublicEndpoint: 公网接入点地址
 注意：此字段可能返回 null，表示取不到有效值。
         :type PublicEndpoint: str
         :param VpcEndpoint: VPC接入点地址
 注意：此字段可能返回 null，表示取不到有效值。
         :type VpcEndpoint: str
+        :param InternalEndpoint: 内部接入点地址
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InternalEndpoint: str
         """
         self.NamespaceId = None
         self.Ttl = None
         self.RetentionTime = None
         self.Remark = None
         self.PublicEndpoint = None
         self.VpcEndpoint = None
+        self.InternalEndpoint = None
 
 
     def _deserialize(self, params):
         self.NamespaceId = params.get("NamespaceId")
         self.Ttl = params.get("Ttl")
         self.RetentionTime = params.get("RetentionTime")
         self.Remark = params.get("Remark")
         self.PublicEndpoint = params.get("PublicEndpoint")
         self.VpcEndpoint = params.get("VpcEndpoint")
+        self.InternalEndpoint = params.get("InternalEndpoint")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -9539,14 +9559,23 @@
         :param PayMode: 0-后付费，1-预付费
         :type PayMode: int
         :param Remark: 备注信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type Remark: str
         :param SpecName: 实例配置ID
         :type SpecName: str
+        :param MaxRetention: 最大可设置消息保留时间，小时为单位
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MaxRetention: int
+        :param MinRetention: 最小可设置消息保留时间，小时为单位
+注意：此字段可能返回 null，表示取不到有效值。
+        :type MinRetention: int
+        :param Retention: 实例消息保留时间，小时为单位
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Retention: int
         """
         self.InstanceId = None
         self.InstanceName = None
         self.InstanceVersion = None
         self.Status = None
         self.NodeCount = None
         self.ConfigDisplay = None
@@ -9554,14 +9583,17 @@
         self.MaxBandWidth = None
         self.MaxStorage = None
         self.ExpireTime = None
         self.AutoRenewFlag = None
         self.PayMode = None
         self.Remark = None
         self.SpecName = None
+        self.MaxRetention = None
+        self.MinRetention = None
+        self.Retention = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.InstanceName = params.get("InstanceName")
         self.InstanceVersion = params.get("InstanceVersion")
         self.Status = params.get("Status")
@@ -9571,14 +9603,17 @@
         self.MaxBandWidth = params.get("MaxBandWidth")
         self.MaxStorage = params.get("MaxStorage")
         self.ExpireTime = params.get("ExpireTime")
         self.AutoRenewFlag = params.get("AutoRenewFlag")
         self.PayMode = params.get("PayMode")
         self.Remark = params.get("Remark")
         self.SpecName = params.get("SpecName")
+        self.MaxRetention = params.get("MaxRetention")
+        self.MinRetention = params.get("MinRetention")
+        self.Retention = params.get("Retention")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdmq-3.0.881/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdmq-3.0.880/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.881/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.880/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.881/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.880/setup.py` & `tencentcloud-sdk-python-tdmq-3.0.881/setup.py`

 * *Files identical despite different names*

