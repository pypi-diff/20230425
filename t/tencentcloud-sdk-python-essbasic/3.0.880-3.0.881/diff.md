# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.880.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.881.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.880.tar", last modified: Mon Apr 24 03:04:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.881.tar", last modified: Tue Apr 25 00:40:33 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.880.tar` & `tencentcloud-sdk-python-essbasic-3.0.881.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    15377 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    50151 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   229475 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:04:45.000000 tencentcloud-sdk-python-essbasic-3.0.880/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    15673 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    50151 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   229707 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:40:33.000000 tencentcloud-sdk-python-essbasic-3.0.881/setup.cfg
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.880/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.881/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,14 +361,17 @@
 
 # 签署人未达到合法年龄。
 OPERATIONDENIED_INVALIDAPPROVERAGE = 'OperationDenied.InvalidApproverAge'
 
 # 没有API权限。
 OPERATIONDENIED_NOAPIAUTH = 'OperationDenied.NoApiAuth'
 
+# 企业暂未开通手机号验证身份的服务，请在企业中心开通再使用
+OPERATIONDENIED_NOAPPROVERMOBILECHECKPERMISSION = 'OperationDenied.NoApproverMobileCheckPermission'
+
 # 无权操作合同。
 OPERATIONDENIED_NOFLOWPERMISSION = 'OperationDenied.NoFlowPermission'
 
 # 未通过个人实名。
 OPERATIONDENIED_NOIDENTITYVERIFY = 'OperationDenied.NoIdentityVerify'
 
 # 流程配额不足。
@@ -388,14 +391,17 @@
 
 # 当前企业员工没有开通境外签署能力。
 OPERATIONDENIED_OVERSEAABILITYNOTOPEN = 'OperationDenied.OverseaAbilityNotOpen'
 
 # 出证计费额度不足。
 OPERATIONDENIED_PROVENOQUOTA = 'OperationDenied.ProveNoQuota'
 
+# 必填控件未填
+OPERATIONDENIED_REQUIREDCOMPONENTNOTFILL = 'OperationDenied.RequiredComponentNotFill'
+
 # 用户不归属于当前企业，无法操作，请检查后重试。
 OPERATIONDENIED_USERNOTINORGANIZATION = 'OperationDenied.UserNotInOrganization'
 
 # 接口功能暂未开放，请联系客户经理申请白名单使用
 OPERATIONDENIED_WHITELISTFORBID = 'OperationDenied.WhiteListForbid'
 
 # 资源不存在。
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2491,14 +2491,17 @@
         :type KeywordOrder: str
         :param KeywordPage: 指定关键字页码，可选参数，指定页码后，将只在指定的页码内查找关键字，非该页码的关键字将不会查询出来
         :type KeywordPage: int
         :param RelativeLocation: 关键字位置模式，Middle-居中，Below-正下方，Right-正右方，LowerRight-右上角，UpperRight-右下角。示例：如果设置Middle的关键字盖章，则印章的中心会和关键字的中心重合，如果设置Below，则印章在关键字的正下方
         :type RelativeLocation: str
         :param KeywordIndexes: 关键字索引，可选参数，如果一个关键字在PDF文件中存在多个，可以通过关键字索引指定使用第几个关键字作为最后的结果，可指定多个索引。示例[0,2]，说明使用PDF文件内第1个和第3个关键字位置。
         :type KeywordIndexes: list of int
+        :param Placeholder: 填写提示的内容
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Placeholder: str
         """
         self.ComponentId = None
         self.ComponentType = None
         self.ComponentName = None
         self.ComponentRequired = None
         self.ComponentRecipientId = None
         self.FileIndex = None
@@ -2516,14 +2519,15 @@
         self.OffsetX = None
         self.OffsetY = None
         self.ChannelComponentId = None
         self.KeywordOrder = None
         self.KeywordPage = None
         self.RelativeLocation = None
         self.KeywordIndexes = None
+        self.Placeholder = None
 
 
     def _deserialize(self, params):
         self.ComponentId = params.get("ComponentId")
         self.ComponentType = params.get("ComponentType")
         self.ComponentName = params.get("ComponentName")
         self.ComponentRequired = params.get("ComponentRequired")
@@ -2543,14 +2547,15 @@
         self.OffsetX = params.get("OffsetX")
         self.OffsetY = params.get("OffsetY")
         self.ChannelComponentId = params.get("ChannelComponentId")
         self.KeywordOrder = params.get("KeywordOrder")
         self.KeywordPage = params.get("KeywordPage")
         self.RelativeLocation = params.get("RelativeLocation")
         self.KeywordIndexes = params.get("KeywordIndexes")
+        self.Placeholder = params.get("Placeholder")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.880/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.881/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.880/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.881/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.880/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.881/setup.py`

 * *Files identical despite different names*

