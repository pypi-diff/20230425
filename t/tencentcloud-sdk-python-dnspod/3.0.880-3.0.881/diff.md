# Comparing `tmp/tencentcloud-sdk-python-dnspod-3.0.880.tar.gz` & `tmp/tencentcloud-sdk-python-dnspod-3.0.881.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.880.tar", last modified: Mon Apr 24 03:02:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.881.tar", last modified: Tue Apr 25 00:35:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dnspod-3.0.880.tar` & `tencentcloud-sdk-python-dnspod-3.0.881.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:02:58.000000 tencentcloud-sdk-python-dnspod-3.0.880/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:02:58.000000 tencentcloud-sdk-python-dnspod-3.0.880/tencentcloud_sdk_python_dnspod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:02:58.000000 tencentcloud-sdk-python-dnspod-3.0.880/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-04-24 03:02:58.000000 tencentcloud-sdk-python-dnspod-3.0.880/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-24 03:02:58.000000 tencentcloud-sdk-python-dnspod-3.0.880/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:02:58.000000 tencentcloud-sdk-python-dnspod-3.0.880/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      746 2023-04-24 03:02:58.000000 tencentcloud-sdk-python-dnspod-3.0.880/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:02:58.000000 tencentcloud-sdk-python-dnspod-3.0.880/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:02:58.000000 tencentcloud-sdk-python-dnspod-3.0.880/tencentcloud/dnspod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:02:58.000000 tencentcloud-sdk-python-dnspod-3.0.880/tencentcloud/dnspod/v20210323/
--rw-r--r--   0 root         (0) root         (0)    23416 2023-04-24 03:02:58.000000 tencentcloud-sdk-python-dnspod-3.0.880/tencentcloud/dnspod/v20210323/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:02:58.000000 tencentcloud-sdk-python-dnspod-3.0.880/tencentcloud/dnspod/v20210323/__init__.py
--rw-r--r--   0 root         (0) root         (0)   201880 2023-04-24 03:02:58.000000 tencentcloud-sdk-python-dnspod-3.0.880/tencentcloud/dnspod/v20210323/models.py
--rw-r--r--   0 root         (0) root         (0)    58917 2023-04-24 03:02:58.000000 tencentcloud-sdk-python-dnspod-3.0.880/tencentcloud/dnspod/v20210323/dnspod_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:02:58.000000 tencentcloud-sdk-python-dnspod-3.0.880/tencentcloud/dnspod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:02:58.000000 tencentcloud-sdk-python-dnspod-3.0.880/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-24 03:02:58.000000 tencentcloud-sdk-python-dnspod-3.0.880/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-04-24 03:02:58.000000 tencentcloud-sdk-python-dnspod-3.0.880/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:02:58.000000 tencentcloud-sdk-python-dnspod-3.0.880/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud_sdk_python_dnspod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      746 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/dnspod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/dnspod/v20210323/
+-rw-r--r--   0 root         (0) root         (0)    23568 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/dnspod/v20210323/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/dnspod/v20210323/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   201880 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/dnspod/v20210323/models.py
+-rw-r--r--   0 root         (0) root         (0)    58917 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/dnspod/v20210323/dnspod_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/dnspod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:35:51.000000 tencentcloud-sdk-python-dnspod-3.0.881/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.880/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.880/README.rst` & `tencentcloud-sdk-python-dnspod-3.0.881/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.880/tencentcloud/dnspod/v20210323/errorcodes.py` & `tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/dnspod/v20210323/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,14 +364,17 @@
 
 # 鉴权失败。
 INVALIDPARAMETER_PERMISSIONDENIED = 'InvalidParameter.PermissionDenied'
 
 # 用户UIN无效。
 INVALIDPARAMETER_QCLOUDUININVALID = 'InvalidParameter.QcloudUinInvalid'
 
+# TXT 记录无法匹配，请确认记录值是否准确，并再次验证。
+INVALIDPARAMETER_QUHUITXTNOTMATCH = 'InvalidParameter.QuhuiTxtNotMatch'
+
 # TXT 记录未设置或暂未生效，请稍后重试。
 INVALIDPARAMETER_QUHUITXTRECORDWAIT = 'InvalidParameter.QuhuiTxtRecordWait'
 
 # 已实名用户。
 INVALIDPARAMETER_REALNAMEUSER = 'InvalidParameter.RealNameUser'
 
 # 记录编号错误。
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.880/tencentcloud/dnspod/v20210323/models.py` & `tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/dnspod/v20210323/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.880/tencentcloud/dnspod/v20210323/dnspod_client.py` & `tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/dnspod/v20210323/dnspod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.880/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dnspod-3.0.881/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dnspod-3.0.880/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.881/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.880/setup.py` & `tencentcloud-sdk-python-dnspod-3.0.881/setup.py`

 * *Files identical despite different names*

