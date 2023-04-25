# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.880.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.881.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.880.tar", last modified: Mon Apr 24 03:04:34 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.881.tar", last modified: Tue Apr 25 00:40:26 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.880.tar` & `tencentcloud-sdk-python-ess-3.0.881.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    49192 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    23577 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   219487 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:04:34.000000 tencentcloud-sdk-python-ess-3.0.880/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:40:26.000000 tencentcloud-sdk-python-ess-3.0.881/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-25 00:40:26.000000 tencentcloud-sdk-python-ess-3.0.881/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:40:26.000000 tencentcloud-sdk-python-ess-3.0.881/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:40:26.000000 tencentcloud-sdk-python-ess-3.0.881/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:40:26.000000 tencentcloud-sdk-python-ess-3.0.881/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:40:26.000000 tencentcloud-sdk-python-ess-3.0.881/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:40:26.000000 tencentcloud-sdk-python-ess-3.0.881/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    49192 2023-04-25 00:40:26.000000 tencentcloud-sdk-python-ess-3.0.881/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    23727 2023-04-25 00:40:26.000000 tencentcloud-sdk-python-ess-3.0.881/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:40:26.000000 tencentcloud-sdk-python-ess-3.0.881/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   219487 2023-04-25 00:40:26.000000 tencentcloud-sdk-python-ess-3.0.881/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:40:26.000000 tencentcloud-sdk-python-ess-3.0.881/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:40:26.000000 tencentcloud-sdk-python-ess-3.0.881/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-25 00:40:26.000000 tencentcloud-sdk-python-ess-3.0.881/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:40:26.000000 tencentcloud-sdk-python-ess-3.0.881/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:40:26.000000 tencentcloud-sdk-python-ess-3.0.881/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:40:26.000000 tencentcloud-sdk-python-ess-3.0.881/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-25 00:40:26.000000 tencentcloud-sdk-python-ess-3.0.881/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:40:26.000000 tencentcloud-sdk-python-ess-3.0.881/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.880/README.rst` & `tencentcloud-sdk-python-ess-3.0.881/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.880/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.881/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.880/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.881/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.880/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.881/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 
 # 流程未找到关联的电子文件信息，请检查操作步骤，检查参数，并在修改后重试。
 FAILEDOPERATION_FLOWHASNODOCUMENT = 'FailedOperation.FlowHasNoDocument'
 
 # 签署审核未通过，请先完成审核。
 FAILEDOPERATION_NOSIGNREVIEWPASS = 'FailedOperation.NoSignReviewPass'
 
+# 未找到集团子企业相关用户信息，请检查用户相关参数
+FAILEDOPERATION_NOTFOUNDSHADOWUSER = 'FailedOperation.NotFoundShadowUser'
+
 # 企业经营状态与工商局信息不符。
 FAILEDOPERATION_ORGANIZATIONEXPERIENCECHANGE = 'FailedOperation.OrganizationExperienceChange'
 
 # 企业名称与工商局信息不符。
 FAILEDOPERATION_ORGANIZATIONNAMECHANGED = 'FailedOperation.OrganizationNameChanged'
 
 # 企业名称与工商局信息不符,需要超管修改。
```

### Comparing `tencentcloud-sdk-python-ess-3.0.880/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.881/tencentcloud/ess/v20201111/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.880/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.881/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.880/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.881/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.880/setup.py` & `tencentcloud-sdk-python-ess-3.0.881/setup.py`

 * *Files identical despite different names*

