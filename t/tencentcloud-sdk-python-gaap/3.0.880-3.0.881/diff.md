# Comparing `tmp/tencentcloud-sdk-python-gaap-3.0.880.tar.gz` & `tmp/tencentcloud-sdk-python-gaap-3.0.881.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-gaap-3.0.880.tar", last modified: Mon Apr 24 03:08:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-gaap-3.0.881.tar", last modified: Tue Apr 25 00:41:09 2023, max compression
```

## Comparing `tencentcloud-sdk-python-gaap-3.0.880.tar` & `tencentcloud-sdk-python-gaap-3.0.881.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:08:25.000000 tencentcloud-sdk-python-gaap-3.0.880/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-24 03:08:24.000000 tencentcloud-sdk-python-gaap-3.0.880/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:08:25.000000 tencentcloud-sdk-python-gaap-3.0.880/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:08:24.000000 tencentcloud-sdk-python-gaap-3.0.880/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:08:25.000000 tencentcloud-sdk-python-gaap-3.0.880/tencentcloud/gaap/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:08:25.000000 tencentcloud-sdk-python-gaap-3.0.880/tencentcloud/gaap/v20180529/
--rw-r--r--   0 root         (0) root         (0)    11791 2023-04-24 03:08:24.000000 tencentcloud-sdk-python-gaap-3.0.880/tencentcloud/gaap/v20180529/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:08:24.000000 tencentcloud-sdk-python-gaap-3.0.880/tencentcloud/gaap/v20180529/__init__.py
--rw-r--r--   0 root         (0) root         (0)   326300 2023-04-24 03:08:24.000000 tencentcloud-sdk-python-gaap-3.0.880/tencentcloud/gaap/v20180529/models.py
--rw-r--r--   0 root         (0) root         (0)   100035 2023-04-24 03:08:24.000000 tencentcloud-sdk-python-gaap-3.0.880/tencentcloud/gaap/v20180529/gaap_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:08:24.000000 tencentcloud-sdk-python-gaap-3.0.880/tencentcloud/gaap/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-24 03:08:25.000000 tencentcloud-sdk-python-gaap-3.0.880/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-24 03:08:24.000000 tencentcloud-sdk-python-gaap-3.0.880/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:08:25.000000 tencentcloud-sdk-python-gaap-3.0.880/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:08:25.000000 tencentcloud-sdk-python-gaap-3.0.880/tencentcloud_sdk_python_gaap.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:08:24.000000 tencentcloud-sdk-python-gaap-3.0.880/tencentcloud_sdk_python_gaap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-24 03:08:25.000000 tencentcloud-sdk-python-gaap-3.0.880/tencentcloud_sdk_python_gaap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-24 03:08:24.000000 tencentcloud-sdk-python-gaap-3.0.880/tencentcloud_sdk_python_gaap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:08:24.000000 tencentcloud-sdk-python-gaap-3.0.880/tencentcloud_sdk_python_gaap.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:41:09.000000 tencentcloud-sdk-python-gaap-3.0.881/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-25 00:41:09.000000 tencentcloud-sdk-python-gaap-3.0.881/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:41:09.000000 tencentcloud-sdk-python-gaap-3.0.881/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:41:09.000000 tencentcloud-sdk-python-gaap-3.0.881/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:41:09.000000 tencentcloud-sdk-python-gaap-3.0.881/tencentcloud/gaap/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:41:09.000000 tencentcloud-sdk-python-gaap-3.0.881/tencentcloud/gaap/v20180529/
+-rw-r--r--   0 root         (0) root         (0)    11791 2023-04-25 00:41:09.000000 tencentcloud-sdk-python-gaap-3.0.881/tencentcloud/gaap/v20180529/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:41:09.000000 tencentcloud-sdk-python-gaap-3.0.881/tencentcloud/gaap/v20180529/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   327522 2023-04-25 00:41:09.000000 tencentcloud-sdk-python-gaap-3.0.881/tencentcloud/gaap/v20180529/models.py
+-rw-r--r--   0 root         (0) root         (0)   100035 2023-04-25 00:41:09.000000 tencentcloud-sdk-python-gaap-3.0.881/tencentcloud/gaap/v20180529/gaap_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:41:09.000000 tencentcloud-sdk-python-gaap-3.0.881/tencentcloud/gaap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-25 00:41:09.000000 tencentcloud-sdk-python-gaap-3.0.881/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-25 00:41:09.000000 tencentcloud-sdk-python-gaap-3.0.881/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:41:09.000000 tencentcloud-sdk-python-gaap-3.0.881/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:41:09.000000 tencentcloud-sdk-python-gaap-3.0.881/tencentcloud_sdk_python_gaap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:41:09.000000 tencentcloud-sdk-python-gaap-3.0.881/tencentcloud_sdk_python_gaap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-25 00:41:09.000000 tencentcloud-sdk-python-gaap-3.0.881/tencentcloud_sdk_python_gaap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-25 00:41:09.000000 tencentcloud-sdk-python-gaap-3.0.881/tencentcloud_sdk_python_gaap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:41:09.000000 tencentcloud-sdk-python-gaap-3.0.881/tencentcloud_sdk_python_gaap.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-gaap-3.0.880/README.rst` & `tencentcloud-sdk-python-gaap-3.0.881/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gaap-3.0.880/tencentcloud/__init__.py` & `tencentcloud-sdk-python-gaap-3.0.881/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-gaap-3.0.880/tencentcloud/gaap/v20180529/errorcodes.py` & `tencentcloud-sdk-python-gaap-3.0.881/tencentcloud/gaap/v20180529/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gaap-3.0.880/tencentcloud/gaap/v20180529/models.py` & `tencentcloud-sdk-python-gaap-3.0.881/tencentcloud/gaap/v20180529/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -8284,30 +8284,37 @@
 第3个bit，支持Http3接入；
 第4个bit，支持IPv6；
 第5个bit，支持精品BGP接入；
 第6个bit，支持三网接入；
 第7个bit，支持接入段Qos加速。
 注意：此字段可能返回 null，表示取不到有效值。
         :type FeatureBitmap: int
+        :param SupportFeature: 接入区域支持的能力
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SupportFeature: :class:`tencentcloud.gaap.v20180529.models.SupportFeature`
         """
         self.RegionId = None
         self.RegionName = None
         self.RegionArea = None
         self.RegionAreaName = None
         self.IDCType = None
         self.FeatureBitmap = None
+        self.SupportFeature = None
 
 
     def _deserialize(self, params):
         self.RegionId = params.get("RegionId")
         self.RegionName = params.get("RegionName")
         self.RegionArea = params.get("RegionArea")
         self.RegionAreaName = params.get("RegionAreaName")
         self.IDCType = params.get("IDCType")
         self.FeatureBitmap = params.get("FeatureBitmap")
+        if params.get("SupportFeature") is not None:
+            self.SupportFeature = SupportFeature()
+            self.SupportFeature._deserialize(params.get("SupportFeature"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -8741,14 +8748,38 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class SupportFeature(AbstractModel):
+    """加速区域支持的能力，包括支持的网络类型等等。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param NetworkType: 接入区域支持的网络类型列表，normal表示支持常规BGP，cn2表示精品BGP，triple表示三网，secure_eip表示定制安全eip。
+        :type NetworkType: list of str
+        """
+        self.NetworkType = None
+
+
+    def _deserialize(self, params):
+        self.NetworkType = params.get("NetworkType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class TCPListener(AbstractModel):
     """TCP类型监听器信息
 
     """
```

### Comparing `tencentcloud-sdk-python-gaap-3.0.880/tencentcloud/gaap/v20180529/gaap_client.py` & `tencentcloud-sdk-python-gaap-3.0.881/tencentcloud/gaap/v20180529/gaap_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gaap-3.0.880/PKG-INFO` & `tencentcloud-sdk-python-gaap-3.0.881/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gaap
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Gaap SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-gaap-3.0.880/setup.py` & `tencentcloud-sdk-python-gaap-3.0.881/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-gaap-3.0.880/tencentcloud_sdk_python_gaap.egg-info/PKG-INFO` & `tencentcloud-sdk-python-gaap-3.0.881/tencentcloud_sdk_python_gaap.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-gaap
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Gaap SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

