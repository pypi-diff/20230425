# Comparing `tmp/tencentcloud-sdk-python-ccc-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-ccc-3.0.880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ccc-3.0.879.tar", last modified: Fri Apr 21 00:38:24 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ccc-3.0.880.tar", last modified: Mon Apr 24 02:50:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ccc-3.0.879.tar` & `tencentcloud-sdk-python-ccc-3.0.880.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:38:24.000000 tencentcloud-sdk-python-ccc-3.0.879/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 00:38:24.000000 tencentcloud-sdk-python-ccc-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:38:24.000000 tencentcloud-sdk-python-ccc-3.0.879/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:38:24.000000 tencentcloud-sdk-python-ccc-3.0.879/tencentcloud/ccc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:38:24.000000 tencentcloud-sdk-python-ccc-3.0.879/tencentcloud/ccc/v20200210/
--rw-r--r--   0 root         (0) root         (0)    36406 2023-04-21 00:38:24.000000 tencentcloud-sdk-python-ccc-3.0.879/tencentcloud/ccc/v20200210/ccc_client.py
--rw-r--r--   0 root         (0) root         (0)     4155 2023-04-21 00:38:24.000000 tencentcloud-sdk-python-ccc-3.0.879/tencentcloud/ccc/v20200210/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:38:24.000000 tencentcloud-sdk-python-ccc-3.0.879/tencentcloud/ccc/v20200210/__init__.py
--rw-r--r--   0 root         (0) root         (0)   139762 2023-04-21 00:38:24.000000 tencentcloud-sdk-python-ccc-3.0.879/tencentcloud/ccc/v20200210/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:38:24.000000 tencentcloud-sdk-python-ccc-3.0.879/tencentcloud/ccc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:38:24.000000 tencentcloud-sdk-python-ccc-3.0.879/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:38:24.000000 tencentcloud-sdk-python-ccc-3.0.879/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:38:24.000000 tencentcloud-sdk-python-ccc-3.0.879/tencentcloud_sdk_python_ccc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:38:24.000000 tencentcloud-sdk-python-ccc-3.0.879/tencentcloud_sdk_python_ccc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 00:38:24.000000 tencentcloud-sdk-python-ccc-3.0.879/tencentcloud_sdk_python_ccc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:38:24.000000 tencentcloud-sdk-python-ccc-3.0.879/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:38:24.000000 tencentcloud-sdk-python-ccc-3.0.879/tencentcloud_sdk_python_ccc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 00:38:24.000000 tencentcloud-sdk-python-ccc-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:38:24.000000 tencentcloud-sdk-python-ccc-3.0.879/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:50:55.000000 tencentcloud-sdk-python-ccc-3.0.880/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 02:50:55.000000 tencentcloud-sdk-python-ccc-3.0.880/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:50:55.000000 tencentcloud-sdk-python-ccc-3.0.880/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:50:55.000000 tencentcloud-sdk-python-ccc-3.0.880/tencentcloud/ccc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:50:55.000000 tencentcloud-sdk-python-ccc-3.0.880/tencentcloud/ccc/v20200210/
+-rw-r--r--   0 root         (0) root         (0)    36406 2023-04-24 02:50:55.000000 tencentcloud-sdk-python-ccc-3.0.880/tencentcloud/ccc/v20200210/ccc_client.py
+-rw-r--r--   0 root         (0) root         (0)     4155 2023-04-24 02:50:55.000000 tencentcloud-sdk-python-ccc-3.0.880/tencentcloud/ccc/v20200210/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 02:50:55.000000 tencentcloud-sdk-python-ccc-3.0.880/tencentcloud/ccc/v20200210/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140284 2023-04-24 02:50:55.000000 tencentcloud-sdk-python-ccc-3.0.880/tencentcloud/ccc/v20200210/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 02:50:55.000000 tencentcloud-sdk-python-ccc-3.0.880/tencentcloud/ccc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 02:50:55.000000 tencentcloud-sdk-python-ccc-3.0.880/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 02:50:55.000000 tencentcloud-sdk-python-ccc-3.0.880/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:50:55.000000 tencentcloud-sdk-python-ccc-3.0.880/tencentcloud_sdk_python_ccc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 02:50:55.000000 tencentcloud-sdk-python-ccc-3.0.880/tencentcloud_sdk_python_ccc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-24 02:50:55.000000 tencentcloud-sdk-python-ccc-3.0.880/tencentcloud_sdk_python_ccc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 02:50:55.000000 tencentcloud-sdk-python-ccc-3.0.880/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 02:50:55.000000 tencentcloud-sdk-python-ccc-3.0.880/tencentcloud_sdk_python_ccc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 02:50:55.000000 tencentcloud-sdk-python-ccc-3.0.880/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 02:50:55.000000 tencentcloud-sdk-python-ccc-3.0.880/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.879/README.rst` & `tencentcloud-sdk-python-ccc-3.0.880/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.879/tencentcloud/ccc/v20200210/ccc_client.py` & `tencentcloud-sdk-python-ccc-3.0.880/tencentcloud/ccc/v20200210/ccc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.879/tencentcloud/ccc/v20200210/errorcodes.py` & `tencentcloud-sdk-python-ccc-3.0.880/tencentcloud/ccc/v20200210/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.879/tencentcloud/ccc/v20200210/models.py` & `tencentcloud-sdk-python-ccc-3.0.880/tencentcloud/ccc/v20200210/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1307,24 +1307,28 @@
         r"""
         :param SdkAppId: 应用 ID（必填），可以查看 https://console.cloud.tencent.com/ccc
         :type SdkAppId: int
         :param EnabledSkillGroup: 是否返回技能组维度信息，默认“是”
         :type EnabledSkillGroup: bool
         :param EnabledNumber: 是否返回线路维度信息，默认“否”
         :type EnabledNumber: bool
+        :param GroupIdList: 筛选技能组列表
+        :type GroupIdList: list of int
         """
         self.SdkAppId = None
         self.EnabledSkillGroup = None
         self.EnabledNumber = None
+        self.GroupIdList = None
 
 
     def _deserialize(self, params):
         self.SdkAppId = params.get("SdkAppId")
         self.EnabledSkillGroup = params.get("EnabledSkillGroup")
         self.EnabledNumber = params.get("EnabledNumber")
+        self.GroupIdList = params.get("GroupIdList")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -2093,22 +2097,30 @@
 
     def __init__(self):
         r"""
         :param SdkAppId: 应用 ID（必填），可以查看 https://console.cloud.tencent.com/ccc
         :type SdkAppId: int
         :param StaffList: 筛选坐席列表，默认不传返回全部坐席信息
         :type StaffList: list of str
+        :param GroupIdList: 筛选技能组ID列表
+        :type GroupIdList: list of int
+        :param StatusList: 筛选坐席状态列表
+        :type StatusList: list of str
         """
         self.SdkAppId = None
         self.StaffList = None
+        self.GroupIdList = None
+        self.StatusList = None
 
 
     def _deserialize(self, params):
         self.SdkAppId = params.get("SdkAppId")
         self.StaffList = params.get("StaffList")
+        self.GroupIdList = params.get("GroupIdList")
+        self.StatusList = params.get("StatusList")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ccc-3.0.880/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ccc-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-ccc-3.0.880/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ccc
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Ccc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.879/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ccc-3.0.880/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ccc
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Ccc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.879/setup.py` & `tencentcloud-sdk-python-ccc-3.0.880/setup.py`

 * *Files identical despite different names*

