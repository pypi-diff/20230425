# Comparing `tmp/tencentcloud-sdk-python-lcic-3.0.878.tar.gz` & `tmp/tencentcloud-sdk-python-lcic-3.0.880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.878.tar", last modified: Thu Apr 20 00:36:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.880.tar", last modified: Mon Apr 24 03:12:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lcic-3.0.878.tar` & `tencentcloud-sdk-python-lcic-3.0.880.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/lcic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/lcic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/lcic/v20220817/
--rw-r--r--   0 root         (0) root         (0)     4332 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/lcic/v20220817/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/lcic/v20220817/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135371 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/lcic/v20220817/models.py
--rw-r--r--   0 root         (0) root         (0)    46709 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/lcic/v20220817/lcic_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud_sdk_python_lcic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:36:18.000000 tencentcloud-sdk-python-lcic-3.0.878/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:12:57.000000 tencentcloud-sdk-python-lcic-3.0.880/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-24 03:12:56.000000 tencentcloud-sdk-python-lcic-3.0.880/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:12:57.000000 tencentcloud-sdk-python-lcic-3.0.880/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:12:57.000000 tencentcloud-sdk-python-lcic-3.0.880/tencentcloud/lcic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:12:56.000000 tencentcloud-sdk-python-lcic-3.0.880/tencentcloud/lcic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:12:57.000000 tencentcloud-sdk-python-lcic-3.0.880/tencentcloud/lcic/v20220817/
+-rw-r--r--   0 root         (0) root         (0)     4332 2023-04-24 03:12:56.000000 tencentcloud-sdk-python-lcic-3.0.880/tencentcloud/lcic/v20220817/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:12:56.000000 tencentcloud-sdk-python-lcic-3.0.880/tencentcloud/lcic/v20220817/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   138236 2023-04-24 03:12:56.000000 tencentcloud-sdk-python-lcic-3.0.880/tencentcloud/lcic/v20220817/models.py
+-rw-r--r--   0 root         (0) root         (0)    47779 2023-04-24 03:12:56.000000 tencentcloud-sdk-python-lcic-3.0.880/tencentcloud/lcic/v20220817/lcic_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:12:56.000000 tencentcloud-sdk-python-lcic-3.0.880/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:12:57.000000 tencentcloud-sdk-python-lcic-3.0.880/tencentcloud_sdk_python_lcic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:12:57.000000 tencentcloud-sdk-python-lcic-3.0.880/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-24 03:12:57.000000 tencentcloud-sdk-python-lcic-3.0.880/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-24 03:12:57.000000 tencentcloud-sdk-python-lcic-3.0.880/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:12:57.000000 tencentcloud-sdk-python-lcic-3.0.880/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-24 03:12:57.000000 tencentcloud-sdk-python-lcic-3.0.880/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-24 03:12:56.000000 tencentcloud-sdk-python-lcic-3.0.880/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:12:57.000000 tencentcloud-sdk-python-lcic-3.0.880/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.878/README.rst` & `tencentcloud-sdk-python-lcic-3.0.880/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/lcic/v20220817/errorcodes.py` & `tencentcloud-sdk-python-lcic-3.0.880/tencentcloud/lcic/v20220817/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/lcic/v20220817/models.py` & `tencentcloud-sdk-python-lcic-3.0.880/tencentcloud/lcic/v20220817/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -462,14 +462,93 @@
 
 
     def _deserialize(self, params):
         self.RoomIds = params.get("RoomIds")
         self.RequestId = params.get("RequestId")
 
 
+class BatchDescribeDocumentRequest(AbstractModel):
+    """BatchDescribeDocument请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SdkAppId: 低代码互动课堂的SdkAppId。
+        :type SdkAppId: int
+        :param Page: 分页查询当前页数，从1开始递增
+        :type Page: int
+        :param Limit: 每页数据量，最大1000
+        :type Limit: int
+        :param Permission: 课件权限。[0]：获取owner的私有课件；[1]：获取owner的公开课件; [0,1]：则获取owner的私有课件和公开课件；[2]：获取owner的私有课件和所有人(包括owner)的公开课件
+        :type Permission: list of int non-negative
+        :param Owner: 课件所有者的user_id，不填默认获取SdkAppId下所有课件
+        :type Owner: str
+        :param Keyword: 课件名称搜索词
+        :type Keyword: str
+        :param DocumentId: 课件id列表，从列表中查询，忽略错误的id
+        :type DocumentId: list of str
+        """
+        self.SdkAppId = None
+        self.Page = None
+        self.Limit = None
+        self.Permission = None
+        self.Owner = None
+        self.Keyword = None
+        self.DocumentId = None
+
+
+    def _deserialize(self, params):
+        self.SdkAppId = params.get("SdkAppId")
+        self.Page = params.get("Page")
+        self.Limit = params.get("Limit")
+        self.Permission = params.get("Permission")
+        self.Owner = params.get("Owner")
+        self.Keyword = params.get("Keyword")
+        self.DocumentId = params.get("DocumentId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class BatchDescribeDocumentResponse(AbstractModel):
+    """BatchDescribeDocument返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Total: 符合查询条件文档总数
+        :type Total: int
+        :param Documents: 文档信息列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Documents: list of DocumentInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Total = None
+        self.Documents = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Total = params.get("Total")
+        if params.get("Documents") is not None:
+            self.Documents = []
+            for item in params.get("Documents"):
+                obj = DocumentInfo()
+                obj._deserialize(item)
+                self.Documents.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class BatchRegisterRequest(AbstractModel):
     """BatchRegister请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/lcic/v20220817/lcic_client.py` & `tencentcloud-sdk-python-lcic-3.0.880/tencentcloud/lcic/v20220817/lcic_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,14 +160,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def BatchDescribeDocument(self, request):
+        """批量获取文档详情
+
+        :param request: Request instance for BatchDescribeDocument.
+        :type request: :class:`tencentcloud.lcic.v20220817.models.BatchDescribeDocumentRequest`
+        :rtype: :class:`tencentcloud.lcic.v20220817.models.BatchDescribeDocumentResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("BatchDescribeDocument", params, headers=headers)
+            response = json.loads(body)
+            model = models.BatchDescribeDocumentResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def BatchRegister(self, request):
         """如果批量注册的用户已存在，则会被覆盖。一次最多注册1000个用户。默认请求频率限制：10次/秒
 
         :param request: Request instance for BatchRegister.
         :type request: :class:`tencentcloud.lcic.v20220817.models.BatchRegisterRequest`
         :rtype: :class:`tencentcloud.lcic.v20220817.models.BatchRegisterResponse`
 
@@ -598,15 +621,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeDocuments(self, request):
-        """批量获取文档信息
+        """有新接口替换
+
+        批量获取文档信息（已废弃，替代接口BatchDescribeDocument）
 
         :param request: Request instance for DescribeDocuments.
         :type request: :class:`tencentcloud.lcic.v20220817.models.DescribeDocumentsRequest`
         :rtype: :class:`tencentcloud.lcic.v20220817.models.DescribeDocumentsResponse`
 
         """
         try:
@@ -1173,15 +1198,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def StartRoom(self, request):
-        """开始房间的直播
+        """开始房间的直播。 说明：开始房间接口调用之前需要有用户进入课堂初始化课堂信息。
 
         :param request: Request instance for StartRoom.
         :type request: :class:`tencentcloud.lcic.v20220817.models.StartRoomRequest`
         :rtype: :class:`tencentcloud.lcic.v20220817.models.StartRoomResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.878/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lcic-3.0.880/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.878'
+__version__ = '3.0.880'
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.878/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.880/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.878
+Version: 3.0.880
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.878/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.880/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.878
+Version: 3.0.880
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.878/setup.py` & `tencentcloud-sdk-python-lcic-3.0.880/setup.py`

 * *Files identical despite different names*

