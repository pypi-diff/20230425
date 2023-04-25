# Comparing `tmp/tencentcloud-sdk-python-billing-3.0.880.tar.gz` & `tmp/tencentcloud-sdk-python-billing-3.0.881.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-billing-3.0.880.tar", last modified: Mon Apr 24 02:45:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-billing-3.0.881.tar", last modified: Tue Apr 25 00:22:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-billing-3.0.880.tar` & `tencentcloud-sdk-python-billing-3.0.881.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:45:57.000000 tencentcloud-sdk-python-billing-3.0.880/
--rw-r--r--   0 root         (0) root         (0)      749 2023-04-24 02:45:57.000000 tencentcloud-sdk-python-billing-3.0.880/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:45:57.000000 tencentcloud-sdk-python-billing-3.0.880/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 02:45:57.000000 tencentcloud-sdk-python-billing-3.0.880/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:45:57.000000 tencentcloud-sdk-python-billing-3.0.880/tencentcloud/billing/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:45:57.000000 tencentcloud-sdk-python-billing-3.0.880/tencentcloud/billing/v20180709/
--rw-r--r--   0 root         (0) root         (0)     2904 2023-04-24 02:45:57.000000 tencentcloud-sdk-python-billing-3.0.880/tencentcloud/billing/v20180709/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 02:45:57.000000 tencentcloud-sdk-python-billing-3.0.880/tencentcloud/billing/v20180709/__init__.py
--rw-r--r--   0 root         (0) root         (0)   148244 2023-04-24 02:45:57.000000 tencentcloud-sdk-python-billing-3.0.880/tencentcloud/billing/v20180709/models.py
--rw-r--r--   0 root         (0) root         (0)    19523 2023-04-24 02:45:57.000000 tencentcloud-sdk-python-billing-3.0.880/tencentcloud/billing/v20180709/billing_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 02:45:57.000000 tencentcloud-sdk-python-billing-3.0.880/tencentcloud/billing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 02:45:57.000000 tencentcloud-sdk-python-billing-3.0.880/tencentcloud_sdk_python_billing.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 02:45:57.000000 tencentcloud-sdk-python-billing-3.0.880/tencentcloud_sdk_python_billing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-24 02:45:57.000000 tencentcloud-sdk-python-billing-3.0.880/tencentcloud_sdk_python_billing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-24 02:45:57.000000 tencentcloud-sdk-python-billing-3.0.880/tencentcloud_sdk_python_billing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 02:45:57.000000 tencentcloud-sdk-python-billing-3.0.880/tencentcloud_sdk_python_billing.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-24 02:45:57.000000 tencentcloud-sdk-python-billing-3.0.880/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-24 02:45:57.000000 tencentcloud-sdk-python-billing-3.0.880/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 02:45:57.000000 tencentcloud-sdk-python-billing-3.0.880/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:22:32.000000 tencentcloud-sdk-python-billing-3.0.881/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-04-25 00:22:32.000000 tencentcloud-sdk-python-billing-3.0.881/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:22:32.000000 tencentcloud-sdk-python-billing-3.0.881/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:22:32.000000 tencentcloud-sdk-python-billing-3.0.881/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:22:32.000000 tencentcloud-sdk-python-billing-3.0.881/tencentcloud/billing/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:22:32.000000 tencentcloud-sdk-python-billing-3.0.881/tencentcloud/billing/v20180709/
+-rw-r--r--   0 root         (0) root         (0)     2904 2023-04-25 00:22:32.000000 tencentcloud-sdk-python-billing-3.0.881/tencentcloud/billing/v20180709/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:22:32.000000 tencentcloud-sdk-python-billing-3.0.881/tencentcloud/billing/v20180709/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   148500 2023-04-25 00:22:32.000000 tencentcloud-sdk-python-billing-3.0.881/tencentcloud/billing/v20180709/models.py
+-rw-r--r--   0 root         (0) root         (0)    19523 2023-04-25 00:22:32.000000 tencentcloud-sdk-python-billing-3.0.881/tencentcloud/billing/v20180709/billing_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:22:32.000000 tencentcloud-sdk-python-billing-3.0.881/tencentcloud/billing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:22:32.000000 tencentcloud-sdk-python-billing-3.0.881/tencentcloud_sdk_python_billing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:22:32.000000 tencentcloud-sdk-python-billing-3.0.881/tencentcloud_sdk_python_billing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-25 00:22:32.000000 tencentcloud-sdk-python-billing-3.0.881/tencentcloud_sdk_python_billing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-25 00:22:32.000000 tencentcloud-sdk-python-billing-3.0.881/tencentcloud_sdk_python_billing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:22:32.000000 tencentcloud-sdk-python-billing-3.0.881/tencentcloud_sdk_python_billing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-25 00:22:32.000000 tencentcloud-sdk-python-billing-3.0.881/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-25 00:22:32.000000 tencentcloud-sdk-python-billing-3.0.881/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:22:32.000000 tencentcloud-sdk-python-billing-3.0.881/setup.cfg
```

### Comparing `tencentcloud-sdk-python-billing-3.0.880/README.rst` & `tencentcloud-sdk-python-billing-3.0.881/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.880/tencentcloud/__init__.py` & `tencentcloud-sdk-python-billing-3.0.881/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-billing-3.0.880/tencentcloud/billing/v20180709/errorcodes.py` & `tencentcloud-sdk-python-billing-3.0.881/tencentcloud/billing/v20180709/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.880/tencentcloud/billing/v20180709/models.py` & `tencentcloud-sdk-python-billing-3.0.881/tencentcloud/billing/v20180709/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,36 +39,41 @@
         :type IncentivePayAmount: str
         :param VoucherPayAmount: 代金券金额
         :type VoucherPayAmount: str
         :param BillMonth: 账单月份，格式2019-08
         :type BillMonth: str
         :param TotalCost: 原价，单位为元。TotalCost字段自账单3.0（即2021-05）之后开始生效，账单3.0之前返回"-"。合同价的情况下，TotalCost字段与官网价格存在差异，也返回“-”。
         :type TotalCost: str
+        :param TransferPayAmount: 分成金金额
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TransferPayAmount: str
         """
         self.ActionType = None
         self.ActionTypeName = None
         self.RealTotalCost = None
         self.RealTotalCostRatio = None
         self.CashPayAmount = None
         self.IncentivePayAmount = None
         self.VoucherPayAmount = None
         self.BillMonth = None
         self.TotalCost = None
+        self.TransferPayAmount = None
 
 
     def _deserialize(self, params):
         self.ActionType = params.get("ActionType")
         self.ActionTypeName = params.get("ActionTypeName")
         self.RealTotalCost = params.get("RealTotalCost")
         self.RealTotalCostRatio = params.get("RealTotalCostRatio")
         self.CashPayAmount = params.get("CashPayAmount")
         self.IncentivePayAmount = params.get("IncentivePayAmount")
         self.VoucherPayAmount = params.get("VoucherPayAmount")
         self.BillMonth = params.get("BillMonth")
         self.TotalCost = params.get("TotalCost")
+        self.TransferPayAmount = params.get("TransferPayAmount")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-billing-3.0.880/tencentcloud/billing/v20180709/billing_client.py` & `tencentcloud-sdk-python-billing-3.0.881/tencentcloud/billing/v20180709/billing_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.880/tencentcloud_sdk_python_billing.egg-info/PKG-INFO` & `tencentcloud-sdk-python-billing-3.0.881/tencentcloud_sdk_python_billing.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-billing
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Billing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-billing-3.0.880/PKG-INFO` & `tencentcloud-sdk-python-billing-3.0.881/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-billing
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Billing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-billing-3.0.880/setup.py` & `tencentcloud-sdk-python-billing-3.0.881/setup.py`

 * *Files identical despite different names*

