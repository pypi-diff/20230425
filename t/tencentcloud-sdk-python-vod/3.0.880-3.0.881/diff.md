# Comparing `tmp/tencentcloud-sdk-python-vod-3.0.880.tar.gz` & `tmp/tencentcloud-sdk-python-vod-3.0.881.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.880.tar", last modified: Mon Apr 24 03:48:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.881.tar", last modified: Tue Apr 25 01:00:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vod-3.0.880.tar` & `tencentcloud-sdk-python-vod-3.0.881.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 03:48:51.000000 tencentcloud-sdk-python-vod-3.0.880/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud/vod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud/vod/v20180717/
--rw-r--r--   0 root         (0) root         (0)   172410 2023-04-24 03:48:51.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud/vod/v20180717/vod_client.py
--rw-r--r--   0 root         (0) root         (0)    25016 2023-04-24 03:48:51.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud/vod/v20180717/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:48:51.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud/vod/v20180717/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1171666 2023-04-24 03:48:51.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud/vod/v20180717/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:48:51.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud/vod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:48:51.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud_sdk_python_vod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud_sdk_python_vod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 03:48:51.000000 tencentcloud-sdk-python-vod-3.0.880/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 01:00:51.000000 tencentcloud-sdk-python-vod-3.0.881/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-25 01:00:51.000000 tencentcloud-sdk-python-vod-3.0.881/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 01:00:51.000000 tencentcloud-sdk-python-vod-3.0.881/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 01:00:51.000000 tencentcloud-sdk-python-vod-3.0.881/tencentcloud/vod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 01:00:51.000000 tencentcloud-sdk-python-vod-3.0.881/tencentcloud/vod/v20180717/
+-rw-r--r--   0 root         (0) root         (0)   172410 2023-04-25 01:00:51.000000 tencentcloud-sdk-python-vod-3.0.881/tencentcloud/vod/v20180717/vod_client.py
+-rw-r--r--   0 root         (0) root         (0)    25111 2023-04-25 01:00:51.000000 tencentcloud-sdk-python-vod-3.0.881/tencentcloud/vod/v20180717/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 01:00:51.000000 tencentcloud-sdk-python-vod-3.0.881/tencentcloud/vod/v20180717/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1171666 2023-04-25 01:00:51.000000 tencentcloud-sdk-python-vod-3.0.881/tencentcloud/vod/v20180717/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 01:00:51.000000 tencentcloud-sdk-python-vod-3.0.881/tencentcloud/vod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 01:00:51.000000 tencentcloud-sdk-python-vod-3.0.881/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 01:00:51.000000 tencentcloud-sdk-python-vod-3.0.881/tencentcloud_sdk_python_vod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 01:00:51.000000 tencentcloud-sdk-python-vod-3.0.881/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-25 01:00:51.000000 tencentcloud-sdk-python-vod-3.0.881/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 01:00:51.000000 tencentcloud-sdk-python-vod-3.0.881/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 01:00:51.000000 tencentcloud-sdk-python-vod-3.0.881/tencentcloud_sdk_python_vod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 01:00:51.000000 tencentcloud-sdk-python-vod-3.0.881/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-25 01:00:51.000000 tencentcloud-sdk-python-vod-3.0.881/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 01:00:51.000000 tencentcloud-sdk-python-vod-3.0.881/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vod-3.0.880/README.rst` & `tencentcloud-sdk-python-vod-3.0.881/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.880/tencentcloud/vod/v20180717/vod_client.py` & `tencentcloud-sdk-python-vod-3.0.881/tencentcloud/vod/v20180717/vod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.880/tencentcloud/vod/v20180717/errorcodes.py` & `tencentcloud-sdk-python-vod-3.0.881/tencentcloud/vod/v20180717/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 
 # 操作失败：分类不存在。
 FAILEDOPERATION_CLASSNOFOUND = 'FailedOperation.ClassNoFound'
 
 # 操作失败：不支持的封面类型。
 FAILEDOPERATION_COVERTYPE = 'FailedOperation.CoverType'
 
+# 操作失败：数据库操作失败。
+FAILEDOPERATION_DBERROR = 'FailedOperation.DBError'
+
 # 域名部署中，不能变更配置。
 FAILEDOPERATION_DOMAINDEPLOYING = 'FailedOperation.DomainDeploying'
 
 # 用户账户异常。
 FAILEDOPERATION_INVALIDACCOUNT = 'FailedOperation.InvalidAccount'
 
 # 没有开通点播业务。
```

### Comparing `tencentcloud-sdk-python-vod-3.0.880/tencentcloud/vod/v20180717/models.py` & `tencentcloud-sdk-python-vod-3.0.881/tencentcloud/vod/v20180717/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.880/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vod-3.0.881/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vod-3.0.880/tencentcloud_sdk_python_vod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.881/tencentcloud_sdk_python_vod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.880/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.881/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.880/setup.py` & `tencentcloud-sdk-python-vod-3.0.881/setup.py`

 * *Files identical despite different names*

