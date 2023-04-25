# Comparing `tmp/tencentcloud-sdk-python-ecm-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-ecm-3.0.880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ecm-3.0.879.tar", last modified: Fri Apr 21 00:44:09 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ecm-3.0.880.tar", last modified: Mon Apr 24 03:04:00 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ecm-3.0.879.tar` & `tencentcloud-sdk-python-ecm-3.0.880.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:09.000000 tencentcloud-sdk-python-ecm-3.0.879/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 00:44:08.000000 tencentcloud-sdk-python-ecm-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:09.000000 tencentcloud-sdk-python-ecm-3.0.879/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:09.000000 tencentcloud-sdk-python-ecm-3.0.879/tencentcloud/ecm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:09.000000 tencentcloud-sdk-python-ecm-3.0.879/tencentcloud/ecm/v20190719/
--rw-r--r--   0 root         (0) root         (0)   126245 2023-04-21 00:44:08.000000 tencentcloud-sdk-python-ecm-3.0.879/tencentcloud/ecm/v20190719/ecm_client.py
--rw-r--r--   0 root         (0) root         (0)    23407 2023-04-21 00:44:08.000000 tencentcloud-sdk-python-ecm-3.0.879/tencentcloud/ecm/v20190719/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:44:08.000000 tencentcloud-sdk-python-ecm-3.0.879/tencentcloud/ecm/v20190719/__init__.py
--rw-r--r--   0 root         (0) root         (0)   455283 2023-04-21 00:44:08.000000 tencentcloud-sdk-python-ecm-3.0.879/tencentcloud/ecm/v20190719/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:44:08.000000 tencentcloud-sdk-python-ecm-3.0.879/tencentcloud/ecm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:44:08.000000 tencentcloud-sdk-python-ecm-3.0.879/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:44:09.000000 tencentcloud-sdk-python-ecm-3.0.879/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 00:44:08.000000 tencentcloud-sdk-python-ecm-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:44:09.000000 tencentcloud-sdk-python-ecm-3.0.879/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:44:09.000000 tencentcloud-sdk-python-ecm-3.0.879/tencentcloud_sdk_python_ecm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:44:09.000000 tencentcloud-sdk-python-ecm-3.0.879/tencentcloud_sdk_python_ecm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 00:44:09.000000 tencentcloud-sdk-python-ecm-3.0.879/tencentcloud_sdk_python_ecm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:44:09.000000 tencentcloud-sdk-python-ecm-3.0.879/tencentcloud_sdk_python_ecm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:44:09.000000 tencentcloud-sdk-python-ecm-3.0.879/tencentcloud_sdk_python_ecm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:00.000000 tencentcloud-sdk-python-ecm-3.0.880/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 03:04:00.000000 tencentcloud-sdk-python-ecm-3.0.880/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:00.000000 tencentcloud-sdk-python-ecm-3.0.880/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:00.000000 tencentcloud-sdk-python-ecm-3.0.880/tencentcloud/ecm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:00.000000 tencentcloud-sdk-python-ecm-3.0.880/tencentcloud/ecm/v20190719/
+-rw-r--r--   0 root         (0) root         (0)   126245 2023-04-24 03:04:00.000000 tencentcloud-sdk-python-ecm-3.0.880/tencentcloud/ecm/v20190719/ecm_client.py
+-rw-r--r--   0 root         (0) root         (0)    23407 2023-04-24 03:04:00.000000 tencentcloud-sdk-python-ecm-3.0.880/tencentcloud/ecm/v20190719/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:04:00.000000 tencentcloud-sdk-python-ecm-3.0.880/tencentcloud/ecm/v20190719/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   455477 2023-04-24 03:04:00.000000 tencentcloud-sdk-python-ecm-3.0.880/tencentcloud/ecm/v20190719/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:04:00.000000 tencentcloud-sdk-python-ecm-3.0.880/tencentcloud/ecm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:04:00.000000 tencentcloud-sdk-python-ecm-3.0.880/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:04:00.000000 tencentcloud-sdk-python-ecm-3.0.880/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 03:04:00.000000 tencentcloud-sdk-python-ecm-3.0.880/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:04:00.000000 tencentcloud-sdk-python-ecm-3.0.880/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:00.000000 tencentcloud-sdk-python-ecm-3.0.880/tencentcloud_sdk_python_ecm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:04:00.000000 tencentcloud-sdk-python-ecm-3.0.880/tencentcloud_sdk_python_ecm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-24 03:04:00.000000 tencentcloud-sdk-python-ecm-3.0.880/tencentcloud_sdk_python_ecm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:04:00.000000 tencentcloud-sdk-python-ecm-3.0.880/tencentcloud_sdk_python_ecm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:04:00.000000 tencentcloud-sdk-python-ecm-3.0.880/tencentcloud_sdk_python_ecm.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-ecm-3.0.879/README.rst` & `tencentcloud-sdk-python-ecm-3.0.880/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecm-3.0.879/tencentcloud/ecm/v20190719/ecm_client.py` & `tencentcloud-sdk-python-ecm-3.0.880/tencentcloud/ecm/v20190719/ecm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecm-3.0.879/tencentcloud/ecm/v20190719/errorcodes.py` & `tencentcloud-sdk-python-ecm-3.0.880/tencentcloud/ecm/v20190719/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecm-3.0.879/tencentcloud/ecm/v20190719/models.py` & `tencentcloud-sdk-python-ecm-3.0.880/tencentcloud/ecm/v20190719/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10643,34 +10643,38 @@
 USER：用户路由；
 NETD：网络探测路由，创建网络探测实例时，系统默认下发，不可编辑与删除；
 CCN：云联网路由，系统默认下发，不可编辑与删除。
 用户只能添加和操作 USER 类型的路由。
         :type RouteType: str
         :param RouteId: 路由策略ID。IPv4路由策略ID是有意义的值，IPv6路由策略是无意义的值0。后续建议完全使用字符串唯一ID `RouteItemId`操作路由策略
         :type RouteId: int
+        :param RouteTableId: 路由表实例ID，例如：rtb-azd4dt1c。
+        :type RouteTableId: str
         """
         self.DestinationCidrBlock = None
         self.GatewayType = None
         self.GatewayId = None
         self.RouteItemId = None
         self.RouteDescription = None
         self.Enabled = None
         self.RouteType = None
         self.RouteId = None
+        self.RouteTableId = None
 
 
     def _deserialize(self, params):
         self.DestinationCidrBlock = params.get("DestinationCidrBlock")
         self.GatewayType = params.get("GatewayType")
         self.GatewayId = params.get("GatewayId")
         self.RouteItemId = params.get("RouteItemId")
         self.RouteDescription = params.get("RouteDescription")
         self.Enabled = params.get("Enabled")
         self.RouteType = params.get("RouteType")
         self.RouteId = params.get("RouteId")
+        self.RouteTableId = params.get("RouteTableId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ecm-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ecm-3.0.880/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ecm-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-ecm-3.0.880/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ecm
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Ecm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ecm-3.0.879/setup.py` & `tencentcloud-sdk-python-ecm-3.0.880/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ecm-3.0.879/tencentcloud_sdk_python_ecm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ecm-3.0.880/tencentcloud_sdk_python_ecm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ecm
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Ecm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

