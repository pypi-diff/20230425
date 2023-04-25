# Comparing `tmp/tencentcloud-sdk-python-tke-3.0.880.tar.gz` & `tmp/tencentcloud-sdk-python-tke-3.0.881.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.880.tar", last modified: Mon Apr 24 03:46:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tke-3.0.881.tar", last modified: Tue Apr 25 00:58:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tke-3.0.880.tar` & `tencentcloud-sdk-python-tke-3.0.881.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:46:47.000000 tencentcloud-sdk-python-tke-3.0.880/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 03:46:47.000000 tencentcloud-sdk-python-tke-3.0.880/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:46:47.000000 tencentcloud-sdk-python-tke-3.0.880/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:46:47.000000 tencentcloud-sdk-python-tke-3.0.880/tencentcloud/tke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:46:47.000000 tencentcloud-sdk-python-tke-3.0.880/tencentcloud/tke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:46:47.000000 tencentcloud-sdk-python-tke-3.0.880/tencentcloud/tke/v20180525/
--rw-r--r--   0 root         (0) root         (0)   180345 2023-04-24 03:46:47.000000 tencentcloud-sdk-python-tke-3.0.880/tencentcloud/tke/v20180525/tke_client.py
--rw-r--r--   0 root         (0) root         (0)    19361 2023-04-24 03:46:47.000000 tencentcloud-sdk-python-tke-3.0.880/tencentcloud/tke/v20180525/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:46:47.000000 tencentcloud-sdk-python-tke-3.0.880/tencentcloud/tke/v20180525/__init__.py
--rw-r--r--   0 root         (0) root         (0)   649069 2023-04-24 03:46:47.000000 tencentcloud-sdk-python-tke-3.0.880/tencentcloud/tke/v20180525/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:46:47.000000 tencentcloud-sdk-python-tke-3.0.880/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:46:47.000000 tencentcloud-sdk-python-tke-3.0.880/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:46:47.000000 tencentcloud-sdk-python-tke-3.0.880/tencentcloud_sdk_python_tke.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:46:47.000000 tencentcloud-sdk-python-tke-3.0.880/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-24 03:46:47.000000 tencentcloud-sdk-python-tke-3.0.880/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:46:47.000000 tencentcloud-sdk-python-tke-3.0.880/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:46:47.000000 tencentcloud-sdk-python-tke-3.0.880/tencentcloud_sdk_python_tke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 03:46:47.000000 tencentcloud-sdk-python-tke-3.0.880/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:46:47.000000 tencentcloud-sdk-python-tke-3.0.880/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud/tke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud/tke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud/tke/v20180525/
+-rw-r--r--   0 root         (0) root         (0)   180345 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud/tke/v20180525/tke_client.py
+-rw-r--r--   0 root         (0) root         (0)    19455 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud/tke/v20180525/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud/tke/v20180525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   649069 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud/tke/v20180525/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud_sdk_python_tke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud_sdk_python_tke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud_sdk_python_tke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud_sdk_python_tke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/tencentcloud_sdk_python_tke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:58:34.000000 tencentcloud-sdk-python-tke-3.0.881/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tke-3.0.880/README.rst` & `tencentcloud-sdk-python-tke-3.0.881/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.880/tencentcloud/tke/v20180525/tke_client.py` & `tencentcloud-sdk-python-tke-3.0.881/tencentcloud/tke/v20180525/tke_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.880/tencentcloud/tke/v20180525/errorcodes.py` & `tencentcloud-sdk-python-tke-3.0.881/tencentcloud/tke/v20180525/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,17 @@
 
 # 查询主题集失败。
 FAILEDOPERATION_GETCLSLOGSET = 'FailedOperation.GetClsLogSet'
 
 # 获取CLS机器组失败。
 FAILEDOPERATION_GETCLSMACHINEGROUP = 'FailedOperation.GetClsMachineGroup'
 
+# 获取CLS日志主题失败。
+FAILEDOPERATION_GETCLSTOPIC = 'FailedOperation.GetClsTopic'
+
 # 通过配置文件创建集群Client错误。
 FAILEDOPERATION_KUBECLIENTCONF = 'FailedOperation.KubeClientConf'
 
 # 连接用户Kubernetes集群失败。
 FAILEDOPERATION_KUBECLIENTCONNECTION = 'FailedOperation.KubeClientConnection'
 
 # KubernetesAPI错误。
```

### Comparing `tencentcloud-sdk-python-tke-3.0.880/tencentcloud/tke/v20180525/models.py` & `tencentcloud-sdk-python-tke-3.0.881/tencentcloud/tke/v20180525/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tke-3.0.880/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tke-3.0.881/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tke-3.0.880/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.881/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.880/tencentcloud_sdk_python_tke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tke-3.0.881/tencentcloud_sdk_python_tke.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tke
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Tke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tke-3.0.880/setup.py` & `tencentcloud-sdk-python-tke-3.0.881/setup.py`

 * *Files identical despite different names*

