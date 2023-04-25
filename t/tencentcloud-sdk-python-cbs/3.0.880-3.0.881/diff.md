# Comparing `tmp/tencentcloud-sdk-python-cbs-3.0.880.tar.gz` & `tmp/tencentcloud-sdk-python-cbs-3.0.881.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cbs-3.0.880.tar", last modified: Mon Apr 24 02:50:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cbs-3.0.881.tar", last modified: Tue Apr 25 00:28:19 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cbs-3.0.880.tar` & `tencentcloud-sdk-python-cbs-3.0.881.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:50:47.000000 tencentcloud-sdk-python-cbs-3.0.880/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:50:47.000000 tencentcloud-sdk-python-cbs-3.0.880/tencentcloud_sdk_python_cbs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 02:50:47.000000 tencentcloud-sdk-python-cbs-3.0.880/tencentcloud_sdk_python_cbs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-24 02:50:47.000000 tencentcloud-sdk-python-cbs-3.0.880/tencentcloud_sdk_python_cbs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 02:50:47.000000 tencentcloud-sdk-python-cbs-3.0.880/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 02:50:47.000000 tencentcloud-sdk-python-cbs-3.0.880/tencentcloud_sdk_python_cbs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 02:50:47.000000 tencentcloud-sdk-python-cbs-3.0.880/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:50:47.000000 tencentcloud-sdk-python-cbs-3.0.880/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 02:50:47.000000 tencentcloud-sdk-python-cbs-3.0.880/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:50:47.000000 tencentcloud-sdk-python-cbs-3.0.880/tencentcloud/cbs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:50:47.000000 tencentcloud-sdk-python-cbs-3.0.880/tencentcloud/cbs/v20170312/
--rw-r--r--   0 root         (0) root         (0)     7755 2023-04-24 02:50:47.000000 tencentcloud-sdk-python-cbs-3.0.880/tencentcloud/cbs/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53378 2023-04-24 02:50:47.000000 tencentcloud-sdk-python-cbs-3.0.880/tencentcloud/cbs/v20170312/cbs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 02:50:47.000000 tencentcloud-sdk-python-cbs-3.0.880/tencentcloud/cbs/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   158638 2023-04-24 02:50:47.000000 tencentcloud-sdk-python-cbs-3.0.880/tencentcloud/cbs/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 02:50:47.000000 tencentcloud-sdk-python-cbs-3.0.880/tencentcloud/cbs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 02:50:47.000000 tencentcloud-sdk-python-cbs-3.0.880/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 02:50:47.000000 tencentcloud-sdk-python-cbs-3.0.880/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 02:50:47.000000 tencentcloud-sdk-python-cbs-3.0.880/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:28:19.000000 tencentcloud-sdk-python-cbs-3.0.881/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:28:19.000000 tencentcloud-sdk-python-cbs-3.0.881/tencentcloud_sdk_python_cbs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:28:19.000000 tencentcloud-sdk-python-cbs-3.0.881/tencentcloud_sdk_python_cbs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-25 00:28:19.000000 tencentcloud-sdk-python-cbs-3.0.881/tencentcloud_sdk_python_cbs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:28:19.000000 tencentcloud-sdk-python-cbs-3.0.881/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:28:19.000000 tencentcloud-sdk-python-cbs-3.0.881/tencentcloud_sdk_python_cbs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-25 00:28:19.000000 tencentcloud-sdk-python-cbs-3.0.881/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:28:19.000000 tencentcloud-sdk-python-cbs-3.0.881/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:28:19.000000 tencentcloud-sdk-python-cbs-3.0.881/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:28:19.000000 tencentcloud-sdk-python-cbs-3.0.881/tencentcloud/cbs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:28:19.000000 tencentcloud-sdk-python-cbs-3.0.881/tencentcloud/cbs/v20170312/
+-rw-r--r--   0 root         (0) root         (0)     7755 2023-04-25 00:28:19.000000 tencentcloud-sdk-python-cbs-3.0.881/tencentcloud/cbs/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53378 2023-04-25 00:28:19.000000 tencentcloud-sdk-python-cbs-3.0.881/tencentcloud/cbs/v20170312/cbs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:28:19.000000 tencentcloud-sdk-python-cbs-3.0.881/tencentcloud/cbs/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   158638 2023-04-25 00:28:19.000000 tencentcloud-sdk-python-cbs-3.0.881/tencentcloud/cbs/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:28:19.000000 tencentcloud-sdk-python-cbs-3.0.881/tencentcloud/cbs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:28:19.000000 tencentcloud-sdk-python-cbs-3.0.881/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-25 00:28:19.000000 tencentcloud-sdk-python-cbs-3.0.881/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:28:19.000000 tencentcloud-sdk-python-cbs-3.0.881/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.880/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cbs-3.0.881/tencentcloud_sdk_python_cbs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cbs
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Cbs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.880/README.rst` & `tencentcloud-sdk-python-cbs-3.0.881/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cbs-3.0.880/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cbs-3.0.881/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cbs-3.0.880/tencentcloud/cbs/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cbs-3.0.881/tencentcloud/cbs/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cbs-3.0.880/tencentcloud/cbs/v20170312/cbs_client.py` & `tencentcloud-sdk-python-cbs-3.0.881/tencentcloud/cbs/v20170312/cbs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cbs-3.0.880/tencentcloud/cbs/v20170312/models.py` & `tencentcloud-sdk-python-cbs-3.0.881/tencentcloud/cbs/v20170312/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1705,43 +1705,43 @@
         r"""
         :param SnapshotIds: 要查询快照的ID列表。参数不支持同时指定`SnapshotIds`和`Filters`。
         :type SnapshotIds: list of str
         :param Filters: 过滤条件。参数不支持同时指定`SnapshotIds`和`Filters`。<br><li>snapshot-id - Array of String - 是否必填：否 -（过滤条件）按照快照的ID过滤。快照ID形如：`snap-11112222`。<br><li>snapshot-name - Array of String - 是否必填：否 -（过滤条件）按照快照名称过滤。<br><li>snapshot-state - Array of String - 是否必填：否 -（过滤条件）按照快照状态过滤。 (NORMAL：正常 | CREATING：创建中 | ROLLBACKING：回滚中。)<br><li>disk-usage - Array of String - 是否必填：否 -（过滤条件）按创建快照的云盘类型过滤。 (SYSTEM_DISK：代表系统盘 | DATA_DISK：代表数据盘。)<br><li>project-id  - Array of String - 是否必填：否 -（过滤条件）按云硬盘所属项目ID过滤。<br><li>disk-id  - Array of String - 是否必填：否 -（过滤条件）按照创建快照的云硬盘ID过滤。<br><li>zone - Array of String - 是否必填：否 -（过滤条件）按照[可用区](/document/product/213/15753#ZoneInfo)过滤。<br><li>encrypt - Array of String - 是否必填：否 -（过滤条件）按是否加密盘快照过滤。 (TRUE：表示加密盘快照 | FALSE：表示非加密盘快照。)
 <li>snapshot-type- Array of String - 是否必填：否 -（过滤条件）根据snapshot-type指定的快照类型查询对应的快照。
 (SHARED_SNAPSHOT：表示共享过来的快照 | PRIVATE_SNAPSHOT：表示自己私有快照。)
         :type Filters: list of Filter
-        :param Offset: 偏移量，默认为0。关于`Offset`的更进一步介绍请参考API[简介](/document/product/362/15633)中的相关小节。
-        :type Offset: int
         :param Limit: 返回数量，默认为20，最大值为100。关于`Limit`的更进一步介绍请参考 API [简介](/document/product/362/15633)中的相关小节。
         :type Limit: int
-        :param Order: 输出云盘列表的排列顺序。取值范围：<br><li>ASC：升序排列<br><li>DESC：降序排列。
-        :type Order: str
         :param OrderField: 快照列表排序的依据字段。取值范围：<br><li>CREATE_TIME：依据快照的创建时间排序<br>默认按创建时间排序。
         :type OrderField: str
+        :param Offset: 偏移量，默认为0。关于`Offset`的更进一步介绍请参考API[简介](/document/product/362/15633)中的相关小节。
+        :type Offset: int
+        :param Order: 输出云盘列表的排列顺序。取值范围：<br><li>ASC：升序排列<br><li>DESC：降序排列。
+        :type Order: str
         """
         self.SnapshotIds = None
         self.Filters = None
-        self.Offset = None
         self.Limit = None
-        self.Order = None
         self.OrderField = None
+        self.Offset = None
+        self.Order = None
 
 
     def _deserialize(self, params):
         self.SnapshotIds = params.get("SnapshotIds")
         if params.get("Filters") is not None:
             self.Filters = []
             for item in params.get("Filters"):
                 obj = Filter()
                 obj._deserialize(item)
                 self.Filters.append(obj)
-        self.Offset = params.get("Offset")
         self.Limit = params.get("Limit")
-        self.Order = params.get("Order")
         self.OrderField = params.get("OrderField")
+        self.Offset = params.get("Offset")
+        self.Order = params.get("Order")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.880/PKG-INFO` & `tencentcloud-sdk-python-cbs-3.0.881/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cbs
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Cbs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cbs-3.0.880/setup.py` & `tencentcloud-sdk-python-cbs-3.0.881/setup.py`

 * *Files identical despite different names*

