# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.879.tar", last modified: Fri Apr 21 00:57:05 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.880.tar", last modified: Mon Apr 24 03:18:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.879.tar` & `tencentcloud-sdk-python-ocr-3.0.880.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:57:05.000000 tencentcloud-sdk-python-ocr-3.0.879/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:57:05.000000 tencentcloud-sdk-python-ocr-3.0.879/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:57:05.000000 tencentcloud-sdk-python-ocr-3.0.879/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 00:57:05.000000 tencentcloud-sdk-python-ocr-3.0.879/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:57:05.000000 tencentcloud-sdk-python-ocr-3.0.879/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:57:05.000000 tencentcloud-sdk-python-ocr-3.0.879/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 00:57:05.000000 tencentcloud-sdk-python-ocr-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:57:05.000000 tencentcloud-sdk-python-ocr-3.0.879/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:57:05.000000 tencentcloud-sdk-python-ocr-3.0.879/tencentcloud/ocr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:57:05.000000 tencentcloud-sdk-python-ocr-3.0.879/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)   107564 2023-04-21 00:57:05.000000 tencentcloud-sdk-python-ocr-3.0.879/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)     5764 2023-04-21 00:57:05.000000 tencentcloud-sdk-python-ocr-3.0.879/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:57:05.000000 tencentcloud-sdk-python-ocr-3.0.879/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)   413744 2023-04-21 00:57:05.000000 tencentcloud-sdk-python-ocr-3.0.879/tencentcloud/ocr/v20181119/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:57:05.000000 tencentcloud-sdk-python-ocr-3.0.879/tencentcloud/ocr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:57:05.000000 tencentcloud-sdk-python-ocr-3.0.879/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:57:05.000000 tencentcloud-sdk-python-ocr-3.0.879/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 00:57:05.000000 tencentcloud-sdk-python-ocr-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:57:05.000000 tencentcloud-sdk-python-ocr-3.0.879/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:18:42.000000 tencentcloud-sdk-python-ocr-3.0.880/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:18:42.000000 tencentcloud-sdk-python-ocr-3.0.880/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:18:42.000000 tencentcloud-sdk-python-ocr-3.0.880/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-24 03:18:42.000000 tencentcloud-sdk-python-ocr-3.0.880/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:18:42.000000 tencentcloud-sdk-python-ocr-3.0.880/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:18:42.000000 tencentcloud-sdk-python-ocr-3.0.880/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 03:18:42.000000 tencentcloud-sdk-python-ocr-3.0.880/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:18:42.000000 tencentcloud-sdk-python-ocr-3.0.880/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:18:42.000000 tencentcloud-sdk-python-ocr-3.0.880/tencentcloud/ocr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:18:42.000000 tencentcloud-sdk-python-ocr-3.0.880/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)   107564 2023-04-24 03:18:42.000000 tencentcloud-sdk-python-ocr-3.0.880/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2023-04-24 03:18:42.000000 tencentcloud-sdk-python-ocr-3.0.880/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:18:42.000000 tencentcloud-sdk-python-ocr-3.0.880/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   415162 2023-04-24 03:18:42.000000 tencentcloud-sdk-python-ocr-3.0.880/tencentcloud/ocr/v20181119/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:18:42.000000 tencentcloud-sdk-python-ocr-3.0.880/tencentcloud/ocr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:18:42.000000 tencentcloud-sdk-python-ocr-3.0.880/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:18:42.000000 tencentcloud-sdk-python-ocr-3.0.880/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 03:18:42.000000 tencentcloud-sdk-python-ocr-3.0.880/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:18:42.000000 tencentcloud-sdk-python-ocr-3.0.880/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.879/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.880/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.879/README.rst` & `tencentcloud-sdk-python-ocr-3.0.880/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.879/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.880/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.879/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.880/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.879/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.880/tencentcloud/ocr/v20181119/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7241,28 +7241,32 @@
         :type IsPdf: bool
         :param PdfPageNumber: 需要识别的PDF页面的对应页码，仅支持PDF单页识别，当上传文件为PDF且IsPdf参数值为true时有效，默认值为1。
         :type PdfPageNumber: int
         :param ItemNames: 自定义结构化功能需返回的字段名称，例：
 若客户只想返回姓名、性别两个字段的识别结果，则输入
 ItemNames=["姓名","性别"]
         :type ItemNames: list of str
+        :param ReturnFullText: 是否开启全文字段识别
+        :type ReturnFullText: bool
         """
         self.ImageUrl = None
         self.ImageBase64 = None
         self.IsPdf = None
         self.PdfPageNumber = None
         self.ItemNames = None
+        self.ReturnFullText = None
 
 
     def _deserialize(self, params):
         self.ImageUrl = params.get("ImageUrl")
         self.ImageBase64 = params.get("ImageBase64")
         self.IsPdf = params.get("IsPdf")
         self.PdfPageNumber = params.get("PdfPageNumber")
         self.ItemNames = params.get("ItemNames")
+        self.ReturnFullText = params.get("ReturnFullText")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -7276,30 +7280,39 @@
     def __init__(self):
         r"""
         :param Angle: 图片旋转角度(角度制)，文本的水平方向
 为 0；顺时针为正，逆时针为负
         :type Angle: float
         :param StructuralList: 配置结构化文本信息
         :type StructuralList: list of GroupInfo
+        :param WordList: 还原文本信息
+        :type WordList: list of WordItem
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Angle = None
         self.StructuralList = None
+        self.WordList = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.Angle = params.get("Angle")
         if params.get("StructuralList") is not None:
             self.StructuralList = []
             for item in params.get("StructuralList"):
                 obj = GroupInfo()
                 obj._deserialize(item)
                 self.StructuralList.append(obj)
+        if params.get("WordList") is not None:
+            self.WordList = []
+            for item in params.get("WordList"):
+                obj = WordItem()
+                obj._deserialize(item)
+                self.WordList.append(obj)
         self.RequestId = params.get("RequestId")
 
 
 class StructuralItem(AbstractModel):
     """智能结构化识别
 
     """
@@ -10555,14 +10568,44 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class WordItem(AbstractModel):
+    """还原文本信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DetectedText: 文本块内容
+        :type DetectedText: str
+        :param Coord: 四点坐标
+        :type Coord: :class:`tencentcloud.ocr.v20181119.models.Polygon`
+        """
+        self.DetectedText = None
+        self.Coord = None
+
+
+    def _deserialize(self, params):
+        self.DetectedText = params.get("DetectedText")
+        if params.get("Coord") is not None:
+            self.Coord = Polygon()
+            self.Coord._deserialize(params.get("Coord"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class Words(AbstractModel):
     """识别出来的单词信息包括单词（包括单词Character和单词置信度confidence）
 
     """
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.880/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.880/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.879/setup.py` & `tencentcloud-sdk-python-ocr-3.0.880/setup.py`

 * *Files identical despite different names*

