# Comparing `tmp/tencentcloud-sdk-python-keewidb-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-keewidb-3.0.880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-keewidb-3.0.879.tar", last modified: Fri Apr 21 00:48:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-keewidb-3.0.880.tar", last modified: Mon Apr 24 03:12:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-keewidb-3.0.879.tar` & `tencentcloud-sdk-python-keewidb-3.0.880.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:48:22.000000 tencentcloud-sdk-python-keewidb-3.0.879/
--rw-r--r--   0 root         (0) root         (0)      749 2023-04-21 00:48:21.000000 tencentcloud-sdk-python-keewidb-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:48:22.000000 tencentcloud-sdk-python-keewidb-3.0.879/tencentcloud_sdk_python_keewidb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:48:22.000000 tencentcloud-sdk-python-keewidb-3.0.879/tencentcloud_sdk_python_keewidb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-21 00:48:22.000000 tencentcloud-sdk-python-keewidb-3.0.879/tencentcloud_sdk_python_keewidb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-21 00:48:22.000000 tencentcloud-sdk-python-keewidb-3.0.879/tencentcloud_sdk_python_keewidb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:48:22.000000 tencentcloud-sdk-python-keewidb-3.0.879/tencentcloud_sdk_python_keewidb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:48:22.000000 tencentcloud-sdk-python-keewidb-3.0.879/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:48:22.000000 tencentcloud-sdk-python-keewidb-3.0.879/tencentcloud/keewidb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:48:22.000000 tencentcloud-sdk-python-keewidb-3.0.879/tencentcloud/keewidb/v20220308/
--rw-r--r--   0 root         (0) root         (0)     5675 2023-04-21 00:48:21.000000 tencentcloud-sdk-python-keewidb-3.0.879/tencentcloud/keewidb/v20220308/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    36254 2023-04-21 00:48:21.000000 tencentcloud-sdk-python-keewidb-3.0.879/tencentcloud/keewidb/v20220308/keewidb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:48:21.000000 tencentcloud-sdk-python-keewidb-3.0.879/tencentcloud/keewidb/v20220308/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135668 2023-04-21 00:48:21.000000 tencentcloud-sdk-python-keewidb-3.0.879/tencentcloud/keewidb/v20220308/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:48:21.000000 tencentcloud-sdk-python-keewidb-3.0.879/tencentcloud/keewidb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:48:21.000000 tencentcloud-sdk-python-keewidb-3.0.879/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-21 00:48:22.000000 tencentcloud-sdk-python-keewidb-3.0.879/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-21 00:48:21.000000 tencentcloud-sdk-python-keewidb-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:48:22.000000 tencentcloud-sdk-python-keewidb-3.0.879/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:12:42.000000 tencentcloud-sdk-python-keewidb-3.0.880/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-04-24 03:12:42.000000 tencentcloud-sdk-python-keewidb-3.0.880/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:12:42.000000 tencentcloud-sdk-python-keewidb-3.0.880/tencentcloud_sdk_python_keewidb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:12:42.000000 tencentcloud-sdk-python-keewidb-3.0.880/tencentcloud_sdk_python_keewidb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-24 03:12:42.000000 tencentcloud-sdk-python-keewidb-3.0.880/tencentcloud_sdk_python_keewidb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-24 03:12:42.000000 tencentcloud-sdk-python-keewidb-3.0.880/tencentcloud_sdk_python_keewidb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:12:42.000000 tencentcloud-sdk-python-keewidb-3.0.880/tencentcloud_sdk_python_keewidb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:12:42.000000 tencentcloud-sdk-python-keewidb-3.0.880/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:12:42.000000 tencentcloud-sdk-python-keewidb-3.0.880/tencentcloud/keewidb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:12:42.000000 tencentcloud-sdk-python-keewidb-3.0.880/tencentcloud/keewidb/v20220308/
+-rw-r--r--   0 root         (0) root         (0)     5675 2023-04-24 03:12:42.000000 tencentcloud-sdk-python-keewidb-3.0.880/tencentcloud/keewidb/v20220308/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    37283 2023-04-24 03:12:42.000000 tencentcloud-sdk-python-keewidb-3.0.880/tencentcloud/keewidb/v20220308/keewidb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:12:42.000000 tencentcloud-sdk-python-keewidb-3.0.880/tencentcloud/keewidb/v20220308/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   137323 2023-04-24 03:12:42.000000 tencentcloud-sdk-python-keewidb-3.0.880/tencentcloud/keewidb/v20220308/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:12:42.000000 tencentcloud-sdk-python-keewidb-3.0.880/tencentcloud/keewidb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:12:42.000000 tencentcloud-sdk-python-keewidb-3.0.880/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-24 03:12:42.000000 tencentcloud-sdk-python-keewidb-3.0.880/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-24 03:12:42.000000 tencentcloud-sdk-python-keewidb-3.0.880/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:12:42.000000 tencentcloud-sdk-python-keewidb-3.0.880/setup.cfg
```

### Comparing `tencentcloud-sdk-python-keewidb-3.0.879/README.rst` & `tencentcloud-sdk-python-keewidb-3.0.880/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-keewidb-3.0.879/tencentcloud_sdk_python_keewidb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-keewidb-3.0.880/tencentcloud_sdk_python_keewidb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-keewidb
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Keewidb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-keewidb-3.0.879/tencentcloud/keewidb/v20220308/errorcodes.py` & `tencentcloud-sdk-python-keewidb-3.0.880/tencentcloud/keewidb/v20220308/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-keewidb-3.0.879/tencentcloud/keewidb/v20220308/keewidb_client.py` & `tencentcloud-sdk-python-keewidb-3.0.880/tencentcloud/keewidb/v20220308/keewidb_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,14 +183,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeConnectionConfig(self, request):
+        """本接口（DescribeConnectionConfig）用于查询实例连接配置，包括出流量和入流量带宽、最大连接数限制。
+
+        :param request: Request instance for DescribeConnectionConfig.
+        :type request: :class:`tencentcloud.keewidb.v20220308.models.DescribeConnectionConfigRequest`
+        :rtype: :class:`tencentcloud.keewidb.v20220308.models.DescribeConnectionConfigResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeConnectionConfig", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeConnectionConfigResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeDBSecurityGroups(self, request):
         """本接口(DescribeDBSecurityGroups)用于查询实例的安全组详情。
 
         :param request: Request instance for DescribeDBSecurityGroups.
         :type request: :class:`tencentcloud.keewidb.v20220308.models.DescribeDBSecurityGroupsRequest`
         :rtype: :class:`tencentcloud.keewidb.v20220308.models.DescribeDBSecurityGroupsResponse`
```

### Comparing `tencentcloud-sdk-python-keewidb-3.0.879/tencentcloud/keewidb/v20220308/models.py` & `tencentcloud-sdk-python-keewidb-3.0.880/tencentcloud/keewidb/v20220308/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -548,14 +548,67 @@
         self.WeekDays = params.get("WeekDays")
         self.TimePeriod = params.get("TimePeriod")
         self.BackupStorageDays = params.get("BackupStorageDays")
         self.BinlogStorageDays = params.get("BinlogStorageDays")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeConnectionConfigRequest(AbstractModel):
+    """DescribeConnectionConfig请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 实例 ID，如：kee-6ubh****。
+        :type InstanceId: str
+        """
+        self.InstanceId = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeConnectionConfigResponse(AbstractModel):
+    """DescribeConnectionConfig返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InNetLimit: 单分片入流量带宽限制，单位：MB。
+        :type InNetLimit: int
+        :param OutNetLimit: 单分片出流量带宽限制，单位：MB。
+        :type OutNetLimit: int
+        :param ClientLimit: 单分片连接数限制。
+        :type ClientLimit: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.InNetLimit = None
+        self.OutNetLimit = None
+        self.ClientLimit = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.InNetLimit = params.get("InNetLimit")
+        self.OutNetLimit = params.get("OutNetLimit")
+        self.ClientLimit = params.get("ClientLimit")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeDBSecurityGroupsRequest(AbstractModel):
     """DescribeDBSecurityGroups请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-keewidb-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-keewidb-3.0.880/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-keewidb-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-keewidb-3.0.880/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-keewidb
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Keewidb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-keewidb-3.0.879/setup.py` & `tencentcloud-sdk-python-keewidb-3.0.880/setup.py`

 * *Files identical despite different names*

