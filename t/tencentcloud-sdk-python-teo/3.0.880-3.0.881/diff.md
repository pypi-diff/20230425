# Comparing `tmp/tencentcloud-sdk-python-teo-3.0.880.tar.gz` & `tmp/tencentcloud-sdk-python-teo-3.0.881.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.880.tar", last modified: Mon Apr 24 03:39:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.881.tar", last modified: Tue Apr 25 00:57:25 2023, max compression
```

## Comparing `tencentcloud-sdk-python-teo-3.0.880.tar` & `tencentcloud-sdk-python-teo-3.0.881.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/tencentcloud/teo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/tencentcloud/teo/v20220106/
--rw-r--r--   0 root         (0) root         (0)     2192 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/tencentcloud/teo/v20220106/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/tencentcloud/teo/v20220106/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24724 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/tencentcloud/teo/v20220106/models.py
--rw-r--r--   0 root         (0) root         (0)     5379 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/tencentcloud/teo/v20220106/teo_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/tencentcloud/teo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/tencentcloud/teo/v20220901/
--rw-r--r--   0 root         (0) root         (0)    21320 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/tencentcloud/teo/v20220901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/tencentcloud/teo/v20220901/__init__.py
--rw-r--r--   0 root         (0) root         (0)   504807 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/tencentcloud/teo/v20220901/models.py
--rw-r--r--   0 root         (0) root         (0)    81864 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/tencentcloud/teo/v20220901/teo_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/tencentcloud_sdk_python_teo.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/tencentcloud_sdk_python_teo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:39:39.000000 tencentcloud-sdk-python-teo-3.0.880/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220106/
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220106/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24724 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220106/models.py
+-rw-r--r--   0 root         (0) root         (0)     5379 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220106/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220901/
+-rw-r--r--   0 root         (0) root         (0)    21701 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   504804 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220901/models.py
+-rw-r--r--   0 root         (0) root         (0)    81864 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220901/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud_sdk_python_teo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/tencentcloud_sdk_python_teo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-25 00:57:24.000000 tencentcloud-sdk-python-teo-3.0.881/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:57:25.000000 tencentcloud-sdk-python-teo-3.0.881/setup.cfg
```

### Comparing `tencentcloud-sdk-python-teo-3.0.880/README.rst` & `tencentcloud-sdk-python-teo-3.0.881/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.880/tencentcloud/teo/v20220106/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.880/tencentcloud/teo/v20220106/models.py` & `tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.880/tencentcloud/teo/v20220106/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220106/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.880/tencentcloud/teo/v20220901/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220901/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,17 +109,23 @@
 
 # 证书错误。
 INVALIDPARAMETER_CERTTOOSHORTKEYSIZE = 'InvalidParameter.CertTooShortKeySize'
 
 # 证书错误。
 INVALIDPARAMETER_CERTUNSUPPORTEDTYPE = 'InvalidParameter.CertUnsupportedType'
 
+# IPv6 访问与客户端 IP 地理位置功能冲突。
+INVALIDPARAMETER_CLIENTIPCOUNTRYCONFLICTSWITHIPV6 = 'InvalidParameter.ClientIpCountryConflictsWithIpv6'
+
 # CNAME模式下无法申请泛域名证书。
 INVALIDPARAMETER_CNAMEWILDHOSTNOTALLOWAPPLYCERTIFICATE = 'InvalidParameter.CnameWildHostNotAllowApplyCertificate'
 
+# 源站不能和域名一致。
+INVALIDPARAMETER_CONFLICTHOSTORIGIN = 'InvalidParameter.ConflictHostOrigin'
+
 # 域名不存在或不属于该账号。
 INVALIDPARAMETER_DOMAINNOTFOUND = 'InvalidParameter.DomainNotFound'
 
 # 当前域名已开启流量调度功能。
 INVALIDPARAMETER_DOMAINONTRAFFICSCHEDULING = 'InvalidParameter.DomainOnTrafficScheduling'
 
 # 操作不支持条件。
@@ -245,14 +251,17 @@
 # 无效的智能加速。
 INVALIDPARAMETER_INVALIDDYNAMICROUTINE = 'InvalidParameter.InvalidDynamicRoutine'
 
 # 套餐包不支持智能加速配置。
 INVALIDPARAMETER_INVALIDDYNAMICROUTINEBILLING = 'InvalidParameter.InvalidDynamicRoutineBilling'
 
 # 无效的自定义错误页面。
+INVALIDPARAMETER_INVALIDERRORPAGE = 'InvalidParameter.InvalidErrorPage'
+
+# 无效的自定义错误页面。
 INVALIDPARAMETER_INVALIDERRORPAGEREDIRECTURL = 'InvalidParameter.InvalidErrorPageRedirectUrl'
 
 # 无效的HTTPS。
 INVALIDPARAMETER_INVALIDHTTPS = 'InvalidParameter.InvalidHttps'
 
 # 无效的HTTPS证书。
 INVALIDPARAMETER_INVALIDHTTPSCERTINFO = 'InvalidParameter.InvalidHttpsCertInfo'
```

### Comparing `tencentcloud-sdk-python-teo-3.0.880/tencentcloud/teo/v20220901/models.py` & `tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220901/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5442,15 +5442,15 @@
         :param MetricNames: 指标列表，取值有:
 <li>l7Flow_outFlux_hy: Edgeone请求流量；</li>
 <li>l7Flow_outBandwidth_hy: Edgeone请求带宽；</li>
 <li>l7Flow_inFlux_hy: 源站响应流量；</li>
 <li>l7Flow_inBandwidth_hy: 源站响应带宽；</li>
 <li>l7Flow_request_hy: 回源请求数；</li>
         :type MetricNames: list of str
-        :param ZoneIds: 站点集合，不填默认选择全部站点。
+        :param ZoneIds: 待查询的站点列表，此参数必填。
         :type ZoneIds: list of str
         :param Interval: 查询时间粒度，取值有：
 <li>min: 1分钟；</li>
 <li>5min: 5分钟；</li>
 <li>hour: 1小时；</li>
 <li>day: 1天。</li>不填将根据开始时间跟结束时间的间距自动推算粒度，具体为：一小时范围内以min粒度查询，两天范围内以5min粒度查询，七天范围内以hour粒度查询，超过七天以day粒度查询。
         :type Interval: str
```

### Comparing `tencentcloud-sdk-python-teo-3.0.880/tencentcloud/teo/v20220901/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.881/tencentcloud/teo/v20220901/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.880/tencentcloud/__init__.py` & `tencentcloud-sdk-python-teo-3.0.881/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-teo-3.0.880/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.881/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.880/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-teo-3.0.881/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.880/tencentcloud_sdk_python_teo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.881/tencentcloud_sdk_python_teo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.880/setup.py` & `tencentcloud-sdk-python-teo-3.0.881/setup.py`

 * *Files identical despite different names*

