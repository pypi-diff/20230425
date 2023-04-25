# Comparing `tmp/tencentcloud-sdk-python-cdb-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-cdb-3.0.880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.879.tar", last modified: Fri Apr 21 00:38:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.880.tar", last modified: Mon Apr 24 02:51:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdb-3.0.879.tar` & `tencentcloud-sdk-python-cdb-3.0.880.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:38:31.000000 tencentcloud-sdk-python-cdb-3.0.879/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 00:38:31.000000 tencentcloud-sdk-python-cdb-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:38:31.000000 tencentcloud-sdk-python-cdb-3.0.879/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:38:31.000000 tencentcloud-sdk-python-cdb-3.0.879/tencentcloud/cdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:38:31.000000 tencentcloud-sdk-python-cdb-3.0.879/tencentcloud/cdb/v20170320/
--rw-r--r--   0 root         (0) root         (0)   141766 2023-04-21 00:38:31.000000 tencentcloud-sdk-python-cdb-3.0.879/tencentcloud/cdb/v20170320/cdb_client.py
--rw-r--r--   0 root         (0) root         (0)    18041 2023-04-21 00:38:31.000000 tencentcloud-sdk-python-cdb-3.0.879/tencentcloud/cdb/v20170320/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:38:31.000000 tencentcloud-sdk-python-cdb-3.0.879/tencentcloud/cdb/v20170320/__init__.py
--rw-r--r--   0 root         (0) root         (0)   485639 2023-04-21 00:38:31.000000 tencentcloud-sdk-python-cdb-3.0.879/tencentcloud/cdb/v20170320/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 00:38:31.000000 tencentcloud-sdk-python-cdb-3.0.879/tencentcloud/cdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 00:38:31.000000 tencentcloud-sdk-python-cdb-3.0.879/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:38:31.000000 tencentcloud-sdk-python-cdb-3.0.879/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 00:38:31.000000 tencentcloud-sdk-python-cdb-3.0.879/tencentcloud_sdk_python_cdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 00:38:31.000000 tencentcloud-sdk-python-cdb-3.0.879/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 00:38:31.000000 tencentcloud-sdk-python-cdb-3.0.879/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 00:38:31.000000 tencentcloud-sdk-python-cdb-3.0.879/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 00:38:31.000000 tencentcloud-sdk-python-cdb-3.0.879/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 00:38:31.000000 tencentcloud-sdk-python-cdb-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 00:38:31.000000 tencentcloud-sdk-python-cdb-3.0.879/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:51:02.000000 tencentcloud-sdk-python-cdb-3.0.880/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 02:51:01.000000 tencentcloud-sdk-python-cdb-3.0.880/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:51:02.000000 tencentcloud-sdk-python-cdb-3.0.880/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:51:02.000000 tencentcloud-sdk-python-cdb-3.0.880/tencentcloud/cdb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:51:02.000000 tencentcloud-sdk-python-cdb-3.0.880/tencentcloud/cdb/v20170320/
+-rw-r--r--   0 root         (0) root         (0)   141766 2023-04-24 02:51:01.000000 tencentcloud-sdk-python-cdb-3.0.880/tencentcloud/cdb/v20170320/cdb_client.py
+-rw-r--r--   0 root         (0) root         (0)    18041 2023-04-24 02:51:01.000000 tencentcloud-sdk-python-cdb-3.0.880/tencentcloud/cdb/v20170320/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 02:51:01.000000 tencentcloud-sdk-python-cdb-3.0.880/tencentcloud/cdb/v20170320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   489157 2023-04-24 02:51:01.000000 tencentcloud-sdk-python-cdb-3.0.880/tencentcloud/cdb/v20170320/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 02:51:01.000000 tencentcloud-sdk-python-cdb-3.0.880/tencentcloud/cdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 02:51:01.000000 tencentcloud-sdk-python-cdb-3.0.880/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 02:51:02.000000 tencentcloud-sdk-python-cdb-3.0.880/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:51:02.000000 tencentcloud-sdk-python-cdb-3.0.880/tencentcloud_sdk_python_cdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 02:51:02.000000 tencentcloud-sdk-python-cdb-3.0.880/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-24 02:51:02.000000 tencentcloud-sdk-python-cdb-3.0.880/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 02:51:02.000000 tencentcloud-sdk-python-cdb-3.0.880/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 02:51:02.000000 tencentcloud-sdk-python-cdb-3.0.880/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 02:51:01.000000 tencentcloud-sdk-python-cdb-3.0.880/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 02:51:02.000000 tencentcloud-sdk-python-cdb-3.0.880/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.879/README.rst` & `tencentcloud-sdk-python-cdb-3.0.880/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.879/tencentcloud/cdb/v20170320/cdb_client.py` & `tencentcloud-sdk-python-cdb-3.0.880/tencentcloud/cdb/v20170320/cdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.879/tencentcloud/cdb/v20170320/errorcodes.py` & `tencentcloud-sdk-python-cdb-3.0.880/tencentcloud/cdb/v20170320/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.879/tencentcloud/cdb/v20170320/models.py` & `tencentcloud-sdk-python-cdb-3.0.880/tencentcloud/cdb/v20170320/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -533,14 +533,20 @@
         :type ExecTimeSection: str
         :param LockWaitTimeSection: 锁等待时间，格式为M-N，例如：10-200
         :type LockWaitTimeSection: str
         :param IoWaitTimeSection: IO等待时间，格式为M-N，例如：10-200
         :type IoWaitTimeSection: str
         :param TransactionLivingTimeSection: 事务持续时间，格式为M-N，例如：10-200
         :type TransactionLivingTimeSection: str
+        :param ThreadId: 线程ID
+        :type ThreadId: list of str
+        :param SentRows: 返回行数。表示筛选返回行数大于该值的审计日志。
+        :type SentRows: int
+        :param ErrCode: mysql错误码
+        :type ErrCode: list of int
         """
         self.Host = None
         self.User = None
         self.DBName = None
         self.TableName = None
         self.PolicyName = None
         self.Sql = None
@@ -551,14 +557,17 @@
         self.Sqls = None
         self.AffectRowsSection = None
         self.SentRowsSection = None
         self.ExecTimeSection = None
         self.LockWaitTimeSection = None
         self.IoWaitTimeSection = None
         self.TransactionLivingTimeSection = None
+        self.ThreadId = None
+        self.SentRows = None
+        self.ErrCode = None
 
 
     def _deserialize(self, params):
         self.Host = params.get("Host")
         self.User = params.get("User")
         self.DBName = params.get("DBName")
         self.TableName = params.get("TableName")
@@ -571,14 +580,17 @@
         self.Sqls = params.get("Sqls")
         self.AffectRowsSection = params.get("AffectRowsSection")
         self.SentRowsSection = params.get("SentRowsSection")
         self.ExecTimeSection = params.get("ExecTimeSection")
         self.LockWaitTimeSection = params.get("LockWaitTimeSection")
         self.IoWaitTimeSection = params.get("IoWaitTimeSection")
         self.TransactionLivingTimeSection = params.get("TransactionLivingTimeSection")
+        self.ThreadId = params.get("ThreadId")
+        self.SentRows = params.get("SentRows")
+        self.ErrCode = params.get("ErrCode")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -698,14 +710,44 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class AuditRuleFilters(AbstractModel):
+    """审计规则的过滤条件
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RuleFilters: 单条审计规则。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RuleFilters: list of RuleFilters
+        """
+        self.RuleFilters = None
+
+
+    def _deserialize(self, params):
+        if params.get("RuleFilters") is not None:
+            self.RuleFilters = []
+            for item in params.get("RuleFilters"):
+                obj = RuleFilters()
+                obj._deserialize(item)
+                self.RuleFilters.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class BackupConfig(AbstractModel):
     """ECDB第二个从库的配置信息，只有ECDB实例才有这个字段
 
     """
 
     def __init__(self):
         r"""
@@ -2292,15 +2334,15 @@
         :type ProjectId: int
         :param Zone: 可用区信息，该参数缺省时，系统会自动选择一个可用区，请使用 [获取云数据库可售卖规格](https://cloud.tencent.com/document/api/236/17229) 接口获取可创建的可用区。
         :type Zone: str
         :param MasterInstanceId: 实例 ID，购买只读实例或者灾备实例时必填，该字段表示只读实例或者灾备实例的主实例 ID，请使用 [查询实例列表](https://cloud.tencent.com/document/api/236/15872) 接口查询云数据库实例 ID。
         :type MasterInstanceId: str
         :param InstanceRole: 实例类型，默认为 master，支持值包括：master - 表示主实例，dr - 表示灾备实例，ro - 表示只读实例。
         :type InstanceRole: str
-        :param MasterRegion: 主实例的可用区信息，购买灾备、RO实例时必填。
+        :param MasterRegion: 主实例地域信息，购买灾备、RO实例时，该字段必填。
         :type MasterRegion: str
         :param Port: 自定义端口，端口支持范围：[ 1024-65535 ] 。
         :type Port: int
         :param Password: 设置 root 帐号密码，密码规则：8 - 64 个字符，至少包含字母、数字、字符（支持的字符：_+-&=!@#$%^*()）中的两种，购买主实例时可指定该参数，购买只读实例或者灾备实例时指定该参数无意义。
         :type Password: str
         :param ParamList: 参数列表，参数格式如 ParamList.0.Name=auto_increment&ParamList.0.Value=1。可通过 [查询默认的可设置参数列表](https://cloud.tencent.com/document/api/236/32662) 查询支持设置的参数。
         :type ParamList: list of ParamInfo
@@ -10152,37 +10194,47 @@
     def __init__(self):
         r"""
         :param InstanceId: CDB实例ID
         :type InstanceId: str
         :param LogExpireDay: 审计日志保存时长。支持值包括：
 7 - 一周
 30 - 一个月；
+90 - 三个月；
 180 - 六个月；
 365 - 一年；
 1095 - 三年；
 1825 - 五年；
         :type LogExpireDay: int
         :param HighLogExpireDay: 高频审计日志保存时长。支持值包括：
 7 - 一周
 30 - 一个月；
-180 - 六个月；
-365 - 一年；
-1095 - 三年；
-1825 - 五年；
         :type HighLogExpireDay: int
+        :param AuditRuleFilters: 审计规则。同RuleTemplateIds都不填是全审计。
+        :type AuditRuleFilters: list of AuditRuleFilters
+        :param RuleTemplateIds: 规则模版ID。同AuditRuleFilters都不填是全审计。
+        :type RuleTemplateIds: list of str
         """
         self.InstanceId = None
         self.LogExpireDay = None
         self.HighLogExpireDay = None
+        self.AuditRuleFilters = None
+        self.RuleTemplateIds = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.LogExpireDay = params.get("LogExpireDay")
         self.HighLogExpireDay = params.get("HighLogExpireDay")
+        if params.get("AuditRuleFilters") is not None:
+            self.AuditRuleFilters = []
+            for item in params.get("AuditRuleFilters"):
+                obj = AuditRuleFilters()
+                obj._deserialize(item)
+                self.AuditRuleFilters.append(obj)
+        self.RuleTemplateIds = params.get("RuleTemplateIds")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -11873,14 +11925,46 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class RuleFilters(AbstractModel):
+    """审计规则的规则过滤条件
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Type: 审计规则过滤条件的参数名称。可选值：host – 客户端 IP；user – 数据库账户；dbName – 数据库名称；sqlType-SQL类型；sql-sql语句；affectRows -影响行数；sentRows-返回行数；checkRows-扫描行数；execTime-执行时间。
+        :type Type: str
+        :param Compare: 审计规则过滤条件的匹配类型。可选值：INC – 包含；EXC – 不包含；EQS – 等于；NEQ – 不等于；REG-正则；GT-大于；LT-小于。
+        :type Compare: str
+        :param Value: 审计规则过滤条件的匹配值。sqlType条件的Value需在一下选择"alter", "changeuser", "create", "delete", "drop", "execute", "insert", "login", "logout", "other", "replace", "select", "set", "update"。
+        :type Value: list of str
+        """
+        self.Type = None
+        self.Compare = None
+        self.Value = None
+
+
+    def _deserialize(self, params):
+        self.Type = params.get("Type")
+        self.Compare = params.get("Compare")
+        self.Value = params.get("Value")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class SecurityGroup(AbstractModel):
     """安全组详情
 
     """
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdb-3.0.880/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdb-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.880/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.879/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.880/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.879/setup.py` & `tencentcloud-sdk-python-cdb-3.0.880/setup.py`

 * *Files identical despite different names*

