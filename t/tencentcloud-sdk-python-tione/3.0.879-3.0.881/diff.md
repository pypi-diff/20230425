# Comparing `tmp/tencentcloud-sdk-python-tione-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-tione-3.0.881.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.879.tar", last modified: Fri Apr 21 01:04:01 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.881.tar", last modified: Tue Apr 25 00:58:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tione-3.0.879.tar` & `tencentcloud-sdk-python-tione-3.0.881.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/
--rw-r--r--   0 root         (0) root         (0)      743 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/tencentcloud/tione/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/tencentcloud/tione/v20211111/
--rw-r--r--   0 root         (0) root         (0)    51024 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/tencentcloud/tione/v20211111/tione_client.py
--rw-r--r--   0 root         (0) root         (0)    10731 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   329804 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/tencentcloud/tione/v20211111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/tencentcloud/tione/v20191022/
--rw-r--r--   0 root         (0) root         (0)    22010 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/tencentcloud/tione/v20191022/tione_client.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/tencentcloud/tione/v20191022/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/tencentcloud/tione/v20191022/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91250 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/tencentcloud/tione/v20191022/models.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/tencentcloud_sdk_python_tione.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 01:04:01.000000 tencentcloud-sdk-python-tione-3.0.879/tencentcloud_sdk_python_tione.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20211111/
+-rw-r--r--   0 root         (0) root         (0)    51024 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20211111/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)    10731 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   331524 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20211111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20191022/
+-rw-r--r--   0 root         (0) root         (0)    22010 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20191022/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20191022/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20191022/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91250 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20191022/models.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud_sdk_python_tione.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      633 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:58:21.000000 tencentcloud-sdk-python-tione-3.0.881/tencentcloud_sdk_python_tione.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tione-3.0.879/README.rst` & `tencentcloud-sdk-python-tione-3.0.881/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tione-3.0.881/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.879'
+__version__ = '3.0.881'
```

### Comparing `tencentcloud-sdk-python-tione-3.0.879/tencentcloud/tione/v20211111/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20211111/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.879/tencentcloud/tione/v20211111/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.879/tencentcloud/tione/v20211111/models.py` & `tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20211111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1010,31 +1010,31 @@
 class CreateModelServiceRequest(AbstractModel):
     """CreateModelService请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param ImageInfo: 镜像信息，配置服务运行所需的镜像地址等信息
-        :type ImageInfo: :class:`tencentcloud.tione.v20211111.models.ImageInfo`
         :param ServiceGroupId: 新增版本时需要填写
         :type ServiceGroupId: str
         :param ServiceGroupName: 不超过60个字，仅支持英文、数字、下划线"_"、短横"-"，只能以英文、数字开头
         :type ServiceGroupName: str
         :param ServiceDescription: 模型服务的描述
         :type ServiceDescription: str
-        :param ChargeType: 付费模式,有 PREPAID 、 POSTPAID_BY_HOUR 和 HYBRID_PAID 三种
+        :param ChargeType: 付费模式,有 PREPAID （包年包月）和 POSTPAID_BY_HOUR（按量付费）
         :type ChargeType: str
         :param ResourceGroupId: 预付费模式下所属的资源组id，同服务组下唯一
         :type ResourceGroupId: str
         :param ModelInfo: 模型信息，需要挂载模型时填写
         :type ModelInfo: :class:`tencentcloud.tione.v20211111.models.ModelInfo`
+        :param ImageInfo: 镜像信息，配置服务运行所需的镜像地址等信息
+        :type ImageInfo: :class:`tencentcloud.tione.v20211111.models.ImageInfo`
         :param Env: 环境变量，可选参数，用于配置容器中的环境变量
         :type Env: list of EnvVar
-        :param Resources: 资源描述，指定预付费模式下的cpu,mem,gpu等信息，后付费无需填写
+        :param Resources: 资源描述，指定包年包月模式下的cpu,mem,gpu等信息，后付费无需填写
         :type Resources: :class:`tencentcloud.tione.v20211111.models.ResourceInfo`
         :param InstanceType: 使用DescribeBillingSpecs接口返回的规格列表中的值，或者参考实例列表:
 TI.S.MEDIUM.POST	2C4G
 TI.S.LARGE.POST	4C8G
 TI.S.2XLARGE16.POST	8C16G
 TI.S.2XLARGE32.POST	8C32G
 TI.S.4XLARGE32.POST	16C32G
@@ -1088,21 +1088,21 @@
         :param VolumeMount: 挂载配置，目前只支持CFS
         :type VolumeMount: :class:`tencentcloud.tione.v20211111.models.VolumeMount`
         :param ServiceLimit: 服务限速限流相关配置
         :type ServiceLimit: :class:`tencentcloud.tione.v20211111.models.ServiceLimit`
         :param CallbackUrl: 回调地址，用于回调创建服务状态信息，回调格式&内容详情见：[TI-ONE 接口回调说明](https://cloud.tencent.com/document/product/851/84292)
         :type CallbackUrl: str
         """
-        self.ImageInfo = None
         self.ServiceGroupId = None
         self.ServiceGroupName = None
         self.ServiceDescription = None
         self.ChargeType = None
         self.ResourceGroupId = None
         self.ModelInfo = None
+        self.ImageInfo = None
         self.Env = None
         self.Resources = None
         self.InstanceType = None
         self.ScaleMode = None
         self.Replicas = None
         self.HorizontalPodAutoscaler = None
         self.LogEnable = None
@@ -1118,25 +1118,25 @@
         self.ScheduledAction = None
         self.VolumeMount = None
         self.ServiceLimit = None
         self.CallbackUrl = None
 
 
     def _deserialize(self, params):
-        if params.get("ImageInfo") is not None:
-            self.ImageInfo = ImageInfo()
-            self.ImageInfo._deserialize(params.get("ImageInfo"))
         self.ServiceGroupId = params.get("ServiceGroupId")
         self.ServiceGroupName = params.get("ServiceGroupName")
         self.ServiceDescription = params.get("ServiceDescription")
         self.ChargeType = params.get("ChargeType")
         self.ResourceGroupId = params.get("ResourceGroupId")
         if params.get("ModelInfo") is not None:
             self.ModelInfo = ModelInfo()
             self.ModelInfo._deserialize(params.get("ModelInfo"))
+        if params.get("ImageInfo") is not None:
+            self.ImageInfo = ImageInfo()
+            self.ImageInfo._deserialize(params.get("ImageInfo"))
         if params.get("Env") is not None:
             self.Env = []
             for item in params.get("Env"):
                 obj = EnvVar()
                 obj._deserialize(item)
                 self.Env.append(obj)
         if params.get("Resources") is not None:
@@ -2991,15 +2991,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param TaskType: 枚举值：TRAIN、NOTEBOOK、INFERENCE
         :type TaskType: str
-        :param ChargeType: 付费模式：POSTPAID_BY_HOUR后付费、PREPAID预付费
+        :param ChargeType: 付费模式：POSTPAID_BY_HOUR按量付费、PREPAID包年包月
         :type ChargeType: str
         :param ResourceType: 资源类型：CALC 计算资源、CPU CPU资源、GPU GPU资源、CBS云硬盘
         :type ResourceType: str
         """
         self.TaskType = None
         self.ChargeType = None
         self.ResourceType = None
@@ -6877,15 +6877,15 @@
         :type Region: str
         :param Namespace: 命名空间
 注意：此字段可能返回 null，表示取不到有效值。
         :type Namespace: str
         :param ChargeType: 付费类型
 注意：此字段可能返回 null，表示取不到有效值。
         :type ChargeType: str
-        :param ResourceGroupId: 后付费资源组id
+        :param ResourceGroupId: 包年包月服务的资源组id，按量计费的服务为空
 注意：此字段可能返回 null，表示取不到有效值。
         :type ResourceGroupId: str
         :param CreatedBy: 创建者
 注意：此字段可能返回 null，表示取不到有效值。
         :type CreatedBy: str
         :param CreateTime: 创建时间
 注意：此字段可能返回 null，表示取不到有效值。
@@ -6944,15 +6944,15 @@
         :type ServiceLimit: :class:`tencentcloud.tione.v20211111.models.ServiceLimit`
         :param ScheduledAction: 定时停止的配置
 注意：此字段可能返回 null，表示取不到有效值。
         :type ScheduledAction: :class:`tencentcloud.tione.v20211111.models.ScheduledAction`
         :param CreateFailedReason: 服务创建失败的原因，创建成功后该字段为默认值 CREATE_SUCCEED
 注意：此字段可能返回 null，表示取不到有效值。
         :type CreateFailedReason: str
-        :param ResourceGroupName: 预付费服务对应的资源组名字
+        :param ResourceGroupName: 包年包月服务对应的资源组名字
 注意：此字段可能返回 null，表示取不到有效值。
         :type ResourceGroupName: str
         :param Tags: 服务的标签
 注意：此字段可能返回 null，表示取不到有效值。
         :type Tags: list of Tag
         """
         self.ServiceGroupId = None
@@ -7327,14 +7327,30 @@
         :type ModelHotUpdateEnable: bool
         :param Pods: Pod列表信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type Pods: :class:`tencentcloud.tione.v20211111.models.Pod`
         :param PodInfos: Pod列表信息
 注意：此字段可能返回 null，表示取不到有效值。
         :type PodInfos: list of Pod
+        :param ScaleStrategy: 定时伸缩策略
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ScaleStrategy: str
+        :param CronScaleJobs: 定时伸缩任务
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CronScaleJobs: list of CronScaleJob
+        :param ScaleMode: 实例数量调节方式,默认为手动
+支持：自动 - "AUTO", 手动 - "MANUAL"
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ScaleMode: str
+        :param ServiceLimit: 服务限速限流相关配置
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ServiceLimit: :class:`tencentcloud.tione.v20211111.models.ServiceLimit`
+        :param ScheduledAction: 定时停止的配置
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ScheduledAction: str
         """
         self.Replicas = None
         self.ImageInfo = None
         self.Env = None
         self.Resources = None
         self.InstanceType = None
         self.ModelInfo = None
@@ -7348,14 +7364,19 @@
         self.ResourceTotal = None
         self.OldReplicas = None
         self.HybridBillingPrepaidReplicas = None
         self.OldHybridBillingPrepaidReplicas = None
         self.ModelHotUpdateEnable = None
         self.Pods = None
         self.PodInfos = None
+        self.ScaleStrategy = None
+        self.CronScaleJobs = None
+        self.ScaleMode = None
+        self.ServiceLimit = None
+        self.ScheduledAction = None
 
 
     def _deserialize(self, params):
         self.Replicas = params.get("Replicas")
         if params.get("ImageInfo") is not None:
             self.ImageInfo = ImageInfo()
             self.ImageInfo._deserialize(params.get("ImageInfo"))
@@ -7397,14 +7418,26 @@
             self.Pods._deserialize(params.get("Pods"))
         if params.get("PodInfos") is not None:
             self.PodInfos = []
             for item in params.get("PodInfos"):
                 obj = Pod()
                 obj._deserialize(item)
                 self.PodInfos.append(obj)
+        self.ScaleStrategy = params.get("ScaleStrategy")
+        if params.get("CronScaleJobs") is not None:
+            self.CronScaleJobs = []
+            for item in params.get("CronScaleJobs"):
+                obj = CronScaleJob()
+                obj._deserialize(item)
+                self.CronScaleJobs.append(obj)
+        self.ScaleMode = params.get("ScaleMode")
+        if params.get("ServiceLimit") is not None:
+            self.ServiceLimit = ServiceLimit()
+            self.ServiceLimit._deserialize(params.get("ServiceLimit"))
+        self.ScheduledAction = params.get("ScheduledAction")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tione-3.0.879/tencentcloud/tione/v20191022/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20191022/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.879/tencentcloud/tione/v20191022/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20191022/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.879/tencentcloud/tione/v20191022/models.py` & `tencentcloud-sdk-python-tione-3.0.881/tencentcloud/tione/v20191022/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.881/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.879
+Version: 3.0.881
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tione-3.0.879/setup.py` & `tencentcloud-sdk-python-tione-3.0.881/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.879/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tione-3.0.881/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.879/tencentcloud_sdk_python_tione.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.881/tencentcloud_sdk_python_tione.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.879
+Version: 3.0.881
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

