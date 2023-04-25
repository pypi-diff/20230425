# Comparing `tmp/tencentcloud-sdk-python-cfs-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-cfs-3.0.881.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.879.tar", last modified: Fri Apr 21 00:39:23 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.881.tar", last modified: Tue Apr 25 00:29:15 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfs-3.0.879.tar` & `tencentcloud-sdk-python-cfs-3.0.881.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:39:23.000000 tencentcloud-sdk-python-cfs-3.0.879/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 00:39:23.000000 tencentcloud-sdk-python-cfs-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:39:23.000000 tencentcloud-sdk-python-cfs-3.0.879/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:39:23.000000 tencentcloud-sdk-python-cfs-3.0.879/tencentcloud/cfs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:39:23.000000 tencentcloud-sdk-python-cfs-3.0.879/tencentcloud/cfs/v20190719/
--rw-r--r--   0 root         (0) root         (0)    13740 2023-04-21 00:39:23.000000 tencentcloud-sdk-python-cfs-3.0.879/tencentcloud/cfs/v20190719/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    37934 2023-04-21 00:39:23.000000 tencentcloud-sdk-python-cfs-3.0.879/tencentcloud/cfs/v20190719/cfs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:39:23.000000 tencentcloud-sdk-python-cfs-3.0.879/tencentcloud/cfs/v20190719/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112598 2023-04-21 00:39:23.000000 tencentcloud-sdk-python-cfs-3.0.879/tencentcloud/cfs/v20190719/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:39:23.000000 tencentcloud-sdk-python-cfs-3.0.879/tencentcloud/cfs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:39:23.000000 tencentcloud-sdk-python-cfs-3.0.879/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:39:23.000000 tencentcloud-sdk-python-cfs-3.0.879/tencentcloud_sdk_python_cfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:39:23.000000 tencentcloud-sdk-python-cfs-3.0.879/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 00:39:23.000000 tencentcloud-sdk-python-cfs-3.0.879/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:39:23.000000 tencentcloud-sdk-python-cfs-3.0.879/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:39:23.000000 tencentcloud-sdk-python-cfs-3.0.879/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:39:23.000000 tencentcloud-sdk-python-cfs-3.0.879/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 00:39:23.000000 tencentcloud-sdk-python-cfs-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:39:23.000000 tencentcloud-sdk-python-cfs-3.0.879/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:29:15.000000 tencentcloud-sdk-python-cfs-3.0.881/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-25 00:29:15.000000 tencentcloud-sdk-python-cfs-3.0.881/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:29:15.000000 tencentcloud-sdk-python-cfs-3.0.881/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:29:15.000000 tencentcloud-sdk-python-cfs-3.0.881/tencentcloud/cfs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:29:15.000000 tencentcloud-sdk-python-cfs-3.0.881/tencentcloud/cfs/v20190719/
+-rw-r--r--   0 root         (0) root         (0)    14458 2023-04-25 00:29:15.000000 tencentcloud-sdk-python-cfs-3.0.881/tencentcloud/cfs/v20190719/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    39796 2023-04-25 00:29:15.000000 tencentcloud-sdk-python-cfs-3.0.881/tencentcloud/cfs/v20190719/cfs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:29:15.000000 tencentcloud-sdk-python-cfs-3.0.881/tencentcloud/cfs/v20190719/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   116607 2023-04-25 00:29:15.000000 tencentcloud-sdk-python-cfs-3.0.881/tencentcloud/cfs/v20190719/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:29:15.000000 tencentcloud-sdk-python-cfs-3.0.881/tencentcloud/cfs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:29:15.000000 tencentcloud-sdk-python-cfs-3.0.881/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:29:15.000000 tencentcloud-sdk-python-cfs-3.0.881/tencentcloud_sdk_python_cfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:29:15.000000 tencentcloud-sdk-python-cfs-3.0.881/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-25 00:29:15.000000 tencentcloud-sdk-python-cfs-3.0.881/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:29:15.000000 tencentcloud-sdk-python-cfs-3.0.881/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:29:15.000000 tencentcloud-sdk-python-cfs-3.0.881/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:29:15.000000 tencentcloud-sdk-python-cfs-3.0.881/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-25 00:29:15.000000 tencentcloud-sdk-python-cfs-3.0.881/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:29:15.000000 tencentcloud-sdk-python-cfs-3.0.881/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.879/README.rst` & `tencentcloud-sdk-python-cfs-3.0.881/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.879/tencentcloud/cfs/v20190719/errorcodes.py` & `tencentcloud-sdk-python-cfs-3.0.881/tencentcloud/cfs/v20190719/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,17 @@
 
 # 文件系统配额设置超出上限。
 INVALIDPARAMETERVALUE_FSSIZELIMITEXCEEDED = 'InvalidParameterValue.FsSizeLimitExceeded'
 
 # 规则IP错误。
 INVALIDPARAMETERVALUE_INVALIDAUTHCLIENTIP = 'InvalidParameterValue.InvalidAuthClientIp'
 
+# 扩容策略参数无效
+INVALIDPARAMETERVALUE_INVALIDAUTOSCALEUPPARAMS = 'InvalidParameterValue.InvalidAutoScaleUpParams'
+
 # 用于保证请求幂等性的字符串错误。
 INVALIDPARAMETERVALUE_INVALIDCLIENTTOKEN = 'InvalidParameterValue.InvalidClientToken'
 
 # 加密参数错误。
 INVALIDPARAMETERVALUE_INVALIDENCRYPTED = 'InvalidParameterValue.InvalidEncrypted'
 
 # FileSystemId无效。
@@ -160,14 +163,17 @@
 
 # 参数值错误: 资源标签值错误。
 INVALIDPARAMETERVALUE_INVALIDRESOURCETAGS = 'InvalidParameterValue.InvalidResourceTags'
 
 # 读写权限设置错误。
 INVALIDPARAMETERVALUE_INVALIDRWPERMISSION = 'InvalidParameterValue.InvalidRwPermission'
 
+# 扩容目标容量参数错误
+INVALIDPARAMETERVALUE_INVALIDSCALEUPTARGETCAPACITY = 'InvalidParameterValue.InvalidScaleupTargetCapacity'
+
 # 无效的快照状态。
 INVALIDPARAMETERVALUE_INVALIDSNAPSHOTSTATUS = 'InvalidParameterValue.InvalidSnapshotStatus'
 
 # 资源包不存在或已绑定。
 INVALIDPARAMETERVALUE_INVALIDSTORAGERESOURCEPKG = 'InvalidParameterValue.InvalidStorageResourcePkg'
 
 # 存储类型参数错误。
@@ -322,32 +328,44 @@
 
 # 资源不存在。
 RESOURCENOTFOUND = 'ResourceNotFound'
 
 # 该文件系统不存在。
 RESOURCENOTFOUND_FILESYSTEMNOTFOUND = 'ResourceNotFound.FileSystemNotFound'
 
+# 文件系统不存在。
+RESOURCENOTFOUND_FSNOTEXIST = 'ResourceNotFound.FsNotExist'
+
 # 挂载点不存在。
 RESOURCENOTFOUND_MOUNTTARGETNOTFOUND = 'ResourceNotFound.MountTargetNotFound'
 
 # 权限组不存在。
 RESOURCENOTFOUND_PGROUPNOTFOUND = 'ResourceNotFound.PgroupNotFound'
 
+# 资源不存在：资源ID 不存在。
+RESOURCENOTFOUND_RESOURCEPACKAGENOTFOUND = 'ResourceNotFound.ResourcePackageNotFound'
+
 # 权限规则不存在。
 RESOURCENOTFOUND_RULENOTFOUND = 'ResourceNotFound.RuleNotFound'
 
 # 快照ID 不存在。
 RESOURCENOTFOUND_SNAPSHOTNOTFOUND = 'ResourceNotFound.SnapshotNotFound'
 
+# 未授权操作。
+UNAUTHORIZEDOPERATION = 'UnauthorizedOperation'
+
 # 操作不支持。
 UNSUPPORTEDOPERATION = 'UnsupportedOperation'
 
 # 该可用区不支持基础网络。
 UNSUPPORTEDOPERATION_BASICNETINTERFACENOTSUPPORTED = 'UnsupportedOperation.BasicNetInterfaceNotSupported'
 
+# appid不在kms白名单(kms目前是白名单开启状态)。
+UNSUPPORTEDOPERATION_MISSINGKMSACCESSPERMISSION = 'UnsupportedOperation.MissingKmsAccessPermission'
+
 # 用户已欠费, 请充值后重试。
 UNSUPPORTEDOPERATION_OUTOFSERVICE = 'UnsupportedOperation.OutOfService'
 
 # cfs角色未被授权。
 UNSUPPORTEDOPERATION_UNAUTHORIZEDCFSQCSROLE = 'UnsupportedOperation.UnauthorizedCfsQcsRole'
 
 # 用户未经过实名认证。
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.879/tencentcloud/cfs/v20190719/cfs_client.py` & `tencentcloud-sdk-python-cfs-3.0.881/tencentcloud/cfs/v20190719/cfs_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -693,14 +693,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ModifyFileSystemAutoScaleUpRule(self, request):
+        """用来设置文件系统扩容策略
+
+        :param request: Request instance for ModifyFileSystemAutoScaleUpRule.
+        :type request: :class:`tencentcloud.cfs.v20190719.models.ModifyFileSystemAutoScaleUpRuleRequest`
+        :rtype: :class:`tencentcloud.cfs.v20190719.models.ModifyFileSystemAutoScaleUpRuleResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyFileSystemAutoScaleUpRule", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyFileSystemAutoScaleUpRuleResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ScaleUpFileSystem(self, request):
+        """该接口用于对turbo 文件系统扩容使用
+
+        :param request: Request instance for ScaleUpFileSystem.
+        :type request: :class:`tencentcloud.cfs.v20190719.models.ScaleUpFileSystemRequest`
+        :rtype: :class:`tencentcloud.cfs.v20190719.models.ScaleUpFileSystemResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ScaleUpFileSystem", params, headers=headers)
+            response = json.loads(body)
+            model = models.ScaleUpFileSystemResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def SetUserQuota(self, request):
         """设置文件系统配额，提供UID/GID的配额设置的接口
 
         :param request: Request instance for SetUserQuota.
         :type request: :class:`tencentcloud.cfs.v20190719.models.SetUserQuotaRequest`
         :rtype: :class:`tencentcloud.cfs.v20190719.models.SetUserQuotaResponse`
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.879/tencentcloud/cfs/v20190719/models.py` & `tencentcloud-sdk-python-cfs-3.0.881/tencentcloud/cfs/v20190719/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2370,14 +2370,84 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ModifyFileSystemAutoScaleUpRuleRequest(AbstractModel):
+    """ModifyFileSystemAutoScaleUpRule请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FileSystemId: 文件系统id
+        :type FileSystemId: str
+        :param ScaleUpThreshold: 扩容阈值，范围[10-90]
+        :type ScaleUpThreshold: int
+        :param TargetThreshold: 扩容后目标阈值,范围[10-90],该值要小于ScaleUpThreshold
+        :type TargetThreshold: int
+        :param Status: 规则状态0:关闭，1 开启
+
+        :type Status: int
+        """
+        self.FileSystemId = None
+        self.ScaleUpThreshold = None
+        self.TargetThreshold = None
+        self.Status = None
+
+
+    def _deserialize(self, params):
+        self.FileSystemId = params.get("FileSystemId")
+        self.ScaleUpThreshold = params.get("ScaleUpThreshold")
+        self.TargetThreshold = params.get("TargetThreshold")
+        self.Status = params.get("Status")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyFileSystemAutoScaleUpRuleResponse(AbstractModel):
+    """ModifyFileSystemAutoScaleUpRule返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FileSystemId: 文件系统id
+        :type FileSystemId: str
+        :param Status: 规则状态0:关闭，1 开启
+        :type Status: int
+        :param ScaleUpThreshold: 扩容阈值,范围[10-90]
+        :type ScaleUpThreshold: int
+        :param TargetThreshold: 扩容后达到阈值,范围[10-90]
+        :type TargetThreshold: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.FileSystemId = None
+        self.Status = None
+        self.ScaleUpThreshold = None
+        self.TargetThreshold = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.FileSystemId = params.get("FileSystemId")
+        self.Status = params.get("Status")
+        self.ScaleUpThreshold = params.get("ScaleUpThreshold")
+        self.TargetThreshold = params.get("TargetThreshold")
+        self.RequestId = params.get("RequestId")
+
+
 class MountInfo(AbstractModel):
     """挂载点信息
 
     """
 
     def __init__(self):
         r"""
@@ -2546,14 +2616,67 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ScaleUpFileSystemRequest(AbstractModel):
+    """ScaleUpFileSystem请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FileSystemId: 文件系统Id
+        :type FileSystemId: str
+        :param TargetCapacity: 扩容的目标容量
+        :type TargetCapacity: int
+        """
+        self.FileSystemId = None
+        self.TargetCapacity = None
+
+
+    def _deserialize(self, params):
+        self.FileSystemId = params.get("FileSystemId")
+        self.TargetCapacity = params.get("TargetCapacity")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ScaleUpFileSystemResponse(AbstractModel):
+    """ScaleUpFileSystem返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FileSystemId: 文件系统Id
+        :type FileSystemId: str
+        :param TargetCapacity: 扩容的目标容量
+        :type TargetCapacity: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.FileSystemId = None
+        self.TargetCapacity = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.FileSystemId = params.get("FileSystemId")
+        self.TargetCapacity = params.get("TargetCapacity")
+        self.RequestId = params.get("RequestId")
+
+
 class SetUserQuotaRequest(AbstractModel):
     """SetUserQuota请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfs-3.0.881/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfs-3.0.879/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.881/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.879
+Version: 3.0.881
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.881/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.879
+Version: 3.0.881
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.879/setup.py` & `tencentcloud-sdk-python-cfs-3.0.881/setup.py`

 * *Files identical despite different names*

