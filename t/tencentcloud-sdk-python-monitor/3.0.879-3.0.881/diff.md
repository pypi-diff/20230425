# Comparing `tmp/tencentcloud-sdk-python-monitor-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-monitor-3.0.881.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-monitor-3.0.879.tar", last modified: Fri Apr 21 00:53:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-monitor-3.0.881.tar", last modified: Tue Apr 25 00:45:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-monitor-3.0.879.tar` & `tencentcloud-sdk-python-monitor-3.0.881.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:53:02.000000 tencentcloud-sdk-python-monitor-3.0.879/
--rw-r--r--   0 root         (0) root         (0)      749 2023-04-21 00:53:02.000000 tencentcloud-sdk-python-monitor-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:53:02.000000 tencentcloud-sdk-python-monitor-3.0.879/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:53:02.000000 tencentcloud-sdk-python-monitor-3.0.879/tencentcloud/monitor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:53:02.000000 tencentcloud-sdk-python-monitor-3.0.879/tencentcloud/monitor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:53:02.000000 tencentcloud-sdk-python-monitor-3.0.879/tencentcloud/monitor/v20180724/
--rw-r--r--   0 root         (0) root         (0)    10246 2023-04-21 00:53:02.000000 tencentcloud-sdk-python-monitor-3.0.879/tencentcloud/monitor/v20180724/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   143620 2023-04-21 00:53:02.000000 tencentcloud-sdk-python-monitor-3.0.879/tencentcloud/monitor/v20180724/monitor_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:53:02.000000 tencentcloud-sdk-python-monitor-3.0.879/tencentcloud/monitor/v20180724/__init__.py
--rw-r--r--   0 root         (0) root         (0)   551751 2023-04-21 00:53:02.000000 tencentcloud-sdk-python-monitor-3.0.879/tencentcloud/monitor/v20180724/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:53:02.000000 tencentcloud-sdk-python-monitor-3.0.879/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-21 00:53:02.000000 tencentcloud-sdk-python-monitor-3.0.879/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:53:02.000000 tencentcloud-sdk-python-monitor-3.0.879/tencentcloud_sdk_python_monitor.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:53:02.000000 tencentcloud-sdk-python-monitor-3.0.879/tencentcloud_sdk_python_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-21 00:53:02.000000 tencentcloud-sdk-python-monitor-3.0.879/tencentcloud_sdk_python_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-21 00:53:02.000000 tencentcloud-sdk-python-monitor-3.0.879/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:53:02.000000 tencentcloud-sdk-python-monitor-3.0.879/tencentcloud_sdk_python_monitor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-21 00:53:02.000000 tencentcloud-sdk-python-monitor-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:53:02.000000 tencentcloud-sdk-python-monitor-3.0.879/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:45:27.000000 tencentcloud-sdk-python-monitor-3.0.881/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-04-25 00:45:27.000000 tencentcloud-sdk-python-monitor-3.0.881/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:45:27.000000 tencentcloud-sdk-python-monitor-3.0.881/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:45:27.000000 tencentcloud-sdk-python-monitor-3.0.881/tencentcloud/monitor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:45:27.000000 tencentcloud-sdk-python-monitor-3.0.881/tencentcloud/monitor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:45:27.000000 tencentcloud-sdk-python-monitor-3.0.881/tencentcloud/monitor/v20180724/
+-rw-r--r--   0 root         (0) root         (0)    10348 2023-04-25 00:45:27.000000 tencentcloud-sdk-python-monitor-3.0.881/tencentcloud/monitor/v20180724/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   143620 2023-04-25 00:45:27.000000 tencentcloud-sdk-python-monitor-3.0.881/tencentcloud/monitor/v20180724/monitor_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:45:27.000000 tencentcloud-sdk-python-monitor-3.0.881/tencentcloud/monitor/v20180724/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   551751 2023-04-25 00:45:27.000000 tencentcloud-sdk-python-monitor-3.0.881/tencentcloud/monitor/v20180724/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:45:27.000000 tencentcloud-sdk-python-monitor-3.0.881/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-25 00:45:27.000000 tencentcloud-sdk-python-monitor-3.0.881/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:45:27.000000 tencentcloud-sdk-python-monitor-3.0.881/tencentcloud_sdk_python_monitor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:45:27.000000 tencentcloud-sdk-python-monitor-3.0.881/tencentcloud_sdk_python_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-25 00:45:27.000000 tencentcloud-sdk-python-monitor-3.0.881/tencentcloud_sdk_python_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-25 00:45:27.000000 tencentcloud-sdk-python-monitor-3.0.881/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:45:27.000000 tencentcloud-sdk-python-monitor-3.0.881/tencentcloud_sdk_python_monitor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-25 00:45:27.000000 tencentcloud-sdk-python-monitor-3.0.881/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:45:27.000000 tencentcloud-sdk-python-monitor-3.0.881/setup.cfg
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.879/README.rst` & `tencentcloud-sdk-python-monitor-3.0.881/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.879/tencentcloud/monitor/v20180724/errorcodes.py` & `tencentcloud-sdk-python-monitor-3.0.881/tencentcloud/monitor/v20180724/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,14 +121,17 @@
 
 # 被除数为0。
 FAILEDOPERATION_DIVISIONBYZERO = 'FailedOperation.DivisionByZero'
 
 # 后端服务超时
 FAILEDOPERATION_DOHTTPTRANSFERFAILED = 'FailedOperation.DoHTTPTransferFailed'
 
+# DoTRPCTransferFailed
+FAILEDOPERATION_DOTRPCTRANSFERFAILED = 'FailedOperation.DoTRPCTransferFailed'
+
 # 查询分析数据失败。
 FAILEDOPERATION_DRUIDQUERYFAILED = 'FailedOperation.DruidQueryFailed'
 
 # druid表不存在。
 FAILEDOPERATION_DRUIDTABLENOTFOUND = 'FailedOperation.DruidTableNotFound'
 
 # 名字重复。
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.879/tencentcloud/monitor/v20180724/monitor_client.py` & `tencentcloud-sdk-python-monitor-3.0.881/tencentcloud/monitor/v20180724/monitor_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.879/tencentcloud/monitor/v20180724/models.py` & `tencentcloud-sdk-python-monitor-3.0.881/tencentcloud/monitor/v20180724/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -11048,15 +11048,15 @@
         :type EventCondition: :class:`tencentcloud.monitor.v20180724.models.AlarmPolicyEventCondition`
         :param Filter: 全局过滤条件
         :type Filter: :class:`tencentcloud.monitor.v20180724.models.AlarmPolicyFilter`
         :param GroupBy: 聚合维度列表，指定按哪些维度 key 来做 group by
         :type GroupBy: list of str
         :param LogAlarmReqInfo: 日志告警创建请求参数信息
         :type LogAlarmReqInfo: :class:`tencentcloud.monitor.v20180724.models.LogAlarmReq`
-        :param NoticeIds: 模版id，专供prom使用
+        :param NoticeIds: 模板id，专供prom使用
         :type NoticeIds: list of str
         :param Enable: 启停状态，0=停用，1=启用
         :type Enable: int
         :param PolicyName: 专供prom策略名称
         :type PolicyName: str
         :param EbSubject: 事件配置的告警
         :type EbSubject: str
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-monitor-3.0.881/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.879'
+__version__ = '3.0.881'
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-monitor-3.0.881/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-monitor
-Version: 3.0.879
+Version: 3.0.881
 Summary: Tencent Cloud Monitor SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.879/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO` & `tencentcloud-sdk-python-monitor-3.0.881/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-monitor
-Version: 3.0.879
+Version: 3.0.881
 Summary: Tencent Cloud Monitor SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.879/setup.py` & `tencentcloud-sdk-python-monitor-3.0.881/setup.py`

 * *Files identical despite different names*

