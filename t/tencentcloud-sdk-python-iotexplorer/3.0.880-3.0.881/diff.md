# Comparing `tmp/tencentcloud-sdk-python-iotexplorer-3.0.880.tar.gz` & `tmp/tencentcloud-sdk-python-iotexplorer-3.0.881.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iotexplorer-3.0.880.tar", last modified: Mon Apr 24 03:11:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iotexplorer-3.0.881.tar", last modified: Tue Apr 25 00:43:13 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iotexplorer-3.0.880.tar` & `tencentcloud-sdk-python-iotexplorer-3.0.881.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:11:52.000000 tencentcloud-sdk-python-iotexplorer-3.0.880/
--rw-r--r--   0 root         (0) root         (0)      761 2023-04-24 03:11:51.000000 tencentcloud-sdk-python-iotexplorer-3.0.880/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:11:52.000000 tencentcloud-sdk-python-iotexplorer-3.0.880/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:11:52.000000 tencentcloud-sdk-python-iotexplorer-3.0.880/tencentcloud/iotexplorer/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:11:51.000000 tencentcloud-sdk-python-iotexplorer-3.0.880/tencentcloud/iotexplorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:11:52.000000 tencentcloud-sdk-python-iotexplorer-3.0.880/tencentcloud/iotexplorer/v20190423/
--rw-r--r--   0 root         (0) root         (0)    20392 2023-04-24 03:11:51.000000 tencentcloud-sdk-python-iotexplorer-3.0.880/tencentcloud/iotexplorer/v20190423/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:11:51.000000 tencentcloud-sdk-python-iotexplorer-3.0.880/tencentcloud/iotexplorer/v20190423/__init__.py
--rw-r--r--   0 root         (0) root         (0)   224109 2023-04-24 03:11:51.000000 tencentcloud-sdk-python-iotexplorer-3.0.880/tencentcloud/iotexplorer/v20190423/models.py
--rw-r--r--   0 root         (0) root         (0)    82835 2023-04-24 03:11:51.000000 tencentcloud-sdk-python-iotexplorer-3.0.880/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:11:51.000000 tencentcloud-sdk-python-iotexplorer-3.0.880/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1699 2023-04-24 03:11:52.000000 tencentcloud-sdk-python-iotexplorer-3.0.880/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:11:52.000000 tencentcloud-sdk-python-iotexplorer-3.0.880/tencentcloud_sdk_python_iotexplorer.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:11:52.000000 tencentcloud-sdk-python-iotexplorer-3.0.880/tencentcloud_sdk_python_iotexplorer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      525 2023-04-24 03:11:52.000000 tencentcloud-sdk-python-iotexplorer-3.0.880/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1699 2023-04-24 03:11:52.000000 tencentcloud-sdk-python-iotexplorer-3.0.880/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:11:52.000000 tencentcloud-sdk-python-iotexplorer-3.0.880/tencentcloud_sdk_python_iotexplorer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1022 2023-04-24 03:11:51.000000 tencentcloud-sdk-python-iotexplorer-3.0.880/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:11:52.000000 tencentcloud-sdk-python-iotexplorer-3.0.880/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:43:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.881/
+-rw-r--r--   0 root         (0) root         (0)      761 2023-04-25 00:43:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.881/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:43:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.881/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:43:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.881/tencentcloud/iotexplorer/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:43:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.881/tencentcloud/iotexplorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:43:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.881/tencentcloud/iotexplorer/v20190423/
+-rw-r--r--   0 root         (0) root         (0)    20510 2023-04-25 00:43:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.881/tencentcloud/iotexplorer/v20190423/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:43:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.881/tencentcloud/iotexplorer/v20190423/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   224364 2023-04-25 00:43:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.881/tencentcloud/iotexplorer/v20190423/models.py
+-rw-r--r--   0 root         (0) root         (0)    82835 2023-04-25 00:43:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.881/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:43:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.881/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-04-25 00:43:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.881/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:43:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.881/tencentcloud_sdk_python_iotexplorer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:43:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.881/tencentcloud_sdk_python_iotexplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      525 2023-04-25 00:43:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.881/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-04-25 00:43:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.881/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:43:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.881/tencentcloud_sdk_python_iotexplorer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-04-25 00:43:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.881/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:43:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.881/setup.cfg
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.880/README.rst` & `tencentcloud-sdk-python-iotexplorer-3.0.881/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.880/tencentcloud/iotexplorer/v20190423/errorcodes.py` & `tencentcloud-sdk-python-iotexplorer-3.0.881/tencentcloud/iotexplorer/v20190423/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -445,14 +445,17 @@
 
 # 操作不支持。
 UNSUPPORTEDOPERATION = 'UnsupportedOperation'
 
 # 围栏下还存在绑定的设备。
 UNSUPPORTEDOPERATION_BINDSEXISTUNDERFENCE = 'UnsupportedOperation.BindsExistUnderFence'
 
+# 存在重复的绑定关系。
+UNSUPPORTEDOPERATION_CANNOTREBINDFAMILY = 'UnsupportedOperation.CannotReBindFamily'
+
 # 创建的设备已经存在。
 UNSUPPORTEDOPERATION_DEVICEDUPKEYEXIST = 'UnsupportedOperation.DeviceDupKeyExist'
 
 # 设备数量超出实例限制。
 UNSUPPORTEDOPERATION_DEVICEEXCEEDLIMIT = 'UnsupportedOperation.DeviceExceedLimit'
 
 # 设备ota升级中。
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.880/tencentcloud/iotexplorer/v20190423/models.py` & `tencentcloud-sdk-python-iotexplorer-3.0.881/tencentcloud/iotexplorer/v20190423/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6080,40 +6080,45 @@
         :type InstanceId: str
         :param ApplicationCount: 应用数量
 注意：此字段可能返回 null，表示取不到有效值。
         :type ApplicationCount: int
         :param DeviceCount: 设备注册总数
 注意：此字段可能返回 null，表示取不到有效值。
         :type DeviceCount: int
+        :param EnableOpenState: 是否开通物联使能
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EnableOpenState: int
         """
         self.ProjectId = None
         self.ProjectName = None
         self.ProjectDesc = None
         self.CreateTime = None
         self.UpdateTime = None
         self.ProductCount = None
         self.NativeAppCount = None
         self.WebAppCount = None
         self.InstanceId = None
         self.ApplicationCount = None
         self.DeviceCount = None
+        self.EnableOpenState = None
 
 
     def _deserialize(self, params):
         self.ProjectId = params.get("ProjectId")
         self.ProjectName = params.get("ProjectName")
         self.ProjectDesc = params.get("ProjectDesc")
         self.CreateTime = params.get("CreateTime")
         self.UpdateTime = params.get("UpdateTime")
         self.ProductCount = params.get("ProductCount")
         self.NativeAppCount = params.get("NativeAppCount")
         self.WebAppCount = params.get("WebAppCount")
         self.InstanceId = params.get("InstanceId")
         self.ApplicationCount = params.get("ApplicationCount")
         self.DeviceCount = params.get("DeviceCount")
+        self.EnableOpenState = params.get("EnableOpenState")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.880/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py` & `tencentcloud-sdk-python-iotexplorer-3.0.881/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.880/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iotexplorer-3.0.881/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.880/PKG-INFO` & `tencentcloud-sdk-python-iotexplorer-3.0.881/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotexplorer
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Iotexplorer SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.880/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-iotexplorer-3.0.881/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.880/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iotexplorer-3.0.881/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotexplorer
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Iotexplorer SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.880/setup.py` & `tencentcloud-sdk-python-iotexplorer-3.0.881/setup.py`

 * *Files identical despite different names*

