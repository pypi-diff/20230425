# Comparing `tmp/tencentcloud-sdk-python-clb-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-clb-3.0.880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.879.tar", last modified: Fri Apr 21 00:40:24 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.880.tar", last modified: Mon Apr 24 02:55:39 2023, max compression
```

## Comparing `tencentcloud-sdk-python-clb-3.0.879.tar` & `tencentcloud-sdk-python-clb-3.0.880.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:40:24.000000 tencentcloud-sdk-python-clb-3.0.879/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 00:40:24.000000 tencentcloud-sdk-python-clb-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:40:24.000000 tencentcloud-sdk-python-clb-3.0.879/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:40:24.000000 tencentcloud-sdk-python-clb-3.0.879/tencentcloud/clb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:40:24.000000 tencentcloud-sdk-python-clb-3.0.879/tencentcloud/clb/v20180317/
--rw-r--r--   0 root         (0) root         (0)     3269 2023-04-21 00:40:24.000000 tencentcloud-sdk-python-clb-3.0.879/tencentcloud/clb/v20180317/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    89842 2023-04-21 00:40:24.000000 tencentcloud-sdk-python-clb-3.0.879/tencentcloud/clb/v20180317/clb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:40:24.000000 tencentcloud-sdk-python-clb-3.0.879/tencentcloud/clb/v20180317/__init__.py
--rw-r--r--   0 root         (0) root         (0)   328056 2023-04-21 00:40:24.000000 tencentcloud-sdk-python-clb-3.0.879/tencentcloud/clb/v20180317/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:40:24.000000 tencentcloud-sdk-python-clb-3.0.879/tencentcloud/clb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:40:24.000000 tencentcloud-sdk-python-clb-3.0.879/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:40:24.000000 tencentcloud-sdk-python-clb-3.0.879/tencentcloud_sdk_python_clb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:40:24.000000 tencentcloud-sdk-python-clb-3.0.879/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 00:40:24.000000 tencentcloud-sdk-python-clb-3.0.879/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:40:24.000000 tencentcloud-sdk-python-clb-3.0.879/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:40:24.000000 tencentcloud-sdk-python-clb-3.0.879/tencentcloud_sdk_python_clb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:40:24.000000 tencentcloud-sdk-python-clb-3.0.879/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 00:40:24.000000 tencentcloud-sdk-python-clb-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:40:24.000000 tencentcloud-sdk-python-clb-3.0.879/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:55:39.000000 tencentcloud-sdk-python-clb-3.0.880/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 02:55:39.000000 tencentcloud-sdk-python-clb-3.0.880/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:55:39.000000 tencentcloud-sdk-python-clb-3.0.880/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:55:39.000000 tencentcloud-sdk-python-clb-3.0.880/tencentcloud/clb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:55:39.000000 tencentcloud-sdk-python-clb-3.0.880/tencentcloud/clb/v20180317/
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-04-24 02:55:39.000000 tencentcloud-sdk-python-clb-3.0.880/tencentcloud/clb/v20180317/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    89842 2023-04-24 02:55:39.000000 tencentcloud-sdk-python-clb-3.0.880/tencentcloud/clb/v20180317/clb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 02:55:39.000000 tencentcloud-sdk-python-clb-3.0.880/tencentcloud/clb/v20180317/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   328368 2023-04-24 02:55:39.000000 tencentcloud-sdk-python-clb-3.0.880/tencentcloud/clb/v20180317/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 02:55:39.000000 tencentcloud-sdk-python-clb-3.0.880/tencentcloud/clb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 02:55:39.000000 tencentcloud-sdk-python-clb-3.0.880/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:55:39.000000 tencentcloud-sdk-python-clb-3.0.880/tencentcloud_sdk_python_clb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 02:55:39.000000 tencentcloud-sdk-python-clb-3.0.880/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-24 02:55:39.000000 tencentcloud-sdk-python-clb-3.0.880/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 02:55:39.000000 tencentcloud-sdk-python-clb-3.0.880/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 02:55:39.000000 tencentcloud-sdk-python-clb-3.0.880/tencentcloud_sdk_python_clb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 02:55:39.000000 tencentcloud-sdk-python-clb-3.0.880/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 02:55:39.000000 tencentcloud-sdk-python-clb-3.0.880/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 02:55:39.000000 tencentcloud-sdk-python-clb-3.0.880/setup.cfg
```

### Comparing `tencentcloud-sdk-python-clb-3.0.879/README.rst` & `tencentcloud-sdk-python-clb-3.0.880/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.879/tencentcloud/clb/v20180317/errorcodes.py` & `tencentcloud-sdk-python-clb-3.0.880/tencentcloud/clb/v20180317/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.879/tencentcloud/clb/v20180317/clb_client.py` & `tencentcloud-sdk-python-clb-3.0.880/tencentcloud/clb/v20180317/clb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.879/tencentcloud/clb/v20180317/models.py` & `tencentcloud-sdk-python-clb-3.0.880/tencentcloud/clb/v20180317/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6410,36 +6410,40 @@
         :type InternetChargeInfo: :class:`tencentcloud.clb.v20180317.models.InternetAccessible`
         :param LoadBalancerPassToTarget: Target是否放通来自CLB的流量。开启放通（true）：只验证CLB上的安全组；不开启放通（false）：需同时验证CLB和后端实例上的安全组。
         :type LoadBalancerPassToTarget: bool
         :param SnatPro: 是否开启跨地域绑定2.0功能
         :type SnatPro: bool
         :param DeleteProtect: 是否开启删除保护
         :type DeleteProtect: bool
+        :param ModifyClassicDomain: 将负载均衡二级域名由mycloud.com改为tencentclb.com，子域名也会变换。修改后mycloud.com域名将失效。
+        :type ModifyClassicDomain: bool
         """
         self.LoadBalancerId = None
         self.LoadBalancerName = None
         self.TargetRegionInfo = None
         self.InternetChargeInfo = None
         self.LoadBalancerPassToTarget = None
         self.SnatPro = None
         self.DeleteProtect = None
+        self.ModifyClassicDomain = None
 
 
     def _deserialize(self, params):
         self.LoadBalancerId = params.get("LoadBalancerId")
         self.LoadBalancerName = params.get("LoadBalancerName")
         if params.get("TargetRegionInfo") is not None:
             self.TargetRegionInfo = TargetRegionInfo()
             self.TargetRegionInfo._deserialize(params.get("TargetRegionInfo"))
         if params.get("InternetChargeInfo") is not None:
             self.InternetChargeInfo = InternetAccessible()
             self.InternetChargeInfo._deserialize(params.get("InternetChargeInfo"))
         self.LoadBalancerPassToTarget = params.get("LoadBalancerPassToTarget")
         self.SnatPro = params.get("SnatPro")
         self.DeleteProtect = params.get("DeleteProtect")
+        self.ModifyClassicDomain = params.get("ModifyClassicDomain")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-clb-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-clb-3.0.880/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-clb-3.0.879/tencentcloud_sdk_python_clb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.880/tencentcloud_sdk_python_clb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.880/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.879/setup.py` & `tencentcloud-sdk-python-clb-3.0.880/setup.py`

 * *Files identical despite different names*

