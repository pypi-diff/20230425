# Comparing `tmp/tencentcloud-sdk-python-nlp-3.0.878.tar.gz` & `tmp/tencentcloud-sdk-python-nlp-3.0.880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-nlp-3.0.878.tar", last modified: Thu Apr 20 00:38:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-nlp-3.0.880.tar", last modified: Mon Apr 24 03:18:13 2023, max compression
```

## Comparing `tencentcloud-sdk-python-nlp-3.0.878.tar` & `tencentcloud-sdk-python-nlp-3.0.880.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:38:28.000000 tencentcloud-sdk-python-nlp-3.0.878/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-20 00:38:28.000000 tencentcloud-sdk-python-nlp-3.0.878/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:38:28.000000 tencentcloud-sdk-python-nlp-3.0.878/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:38:28.000000 tencentcloud-sdk-python-nlp-3.0.878/tencentcloud/nlp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:38:28.000000 tencentcloud-sdk-python-nlp-3.0.878/tencentcloud/nlp/v20190408/
--rw-r--r--   0 root         (0) root         (0)     5316 2023-04-20 00:38:28.000000 tencentcloud-sdk-python-nlp-3.0.878/tencentcloud/nlp/v20190408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    29728 2023-04-20 00:38:28.000000 tencentcloud-sdk-python-nlp-3.0.878/tencentcloud/nlp/v20190408/nlp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:38:28.000000 tencentcloud-sdk-python-nlp-3.0.878/tencentcloud/nlp/v20190408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56111 2023-04-20 00:38:28.000000 tencentcloud-sdk-python-nlp-3.0.878/tencentcloud/nlp/v20190408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-20 00:38:28.000000 tencentcloud-sdk-python-nlp-3.0.878/tencentcloud/nlp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-20 00:38:28.000000 tencentcloud-sdk-python-nlp-3.0.878/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 00:38:28.000000 tencentcloud-sdk-python-nlp-3.0.878/tencentcloud_sdk_python_nlp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 00:38:28.000000 tencentcloud-sdk-python-nlp-3.0.878/tencentcloud_sdk_python_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-20 00:38:28.000000 tencentcloud-sdk-python-nlp-3.0.878/tencentcloud_sdk_python_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:38:28.000000 tencentcloud-sdk-python-nlp-3.0.878/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 00:38:28.000000 tencentcloud-sdk-python-nlp-3.0.878/tencentcloud_sdk_python_nlp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-20 00:38:28.000000 tencentcloud-sdk-python-nlp-3.0.878/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-20 00:38:28.000000 tencentcloud-sdk-python-nlp-3.0.878/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-20 00:38:28.000000 tencentcloud-sdk-python-nlp-3.0.878/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:18:13.000000 tencentcloud-sdk-python-nlp-3.0.880/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 03:18:13.000000 tencentcloud-sdk-python-nlp-3.0.880/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:18:13.000000 tencentcloud-sdk-python-nlp-3.0.880/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:18:13.000000 tencentcloud-sdk-python-nlp-3.0.880/tencentcloud/nlp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:18:13.000000 tencentcloud-sdk-python-nlp-3.0.880/tencentcloud/nlp/v20190408/
+-rw-r--r--   0 root         (0) root         (0)     5316 2023-04-24 03:18:13.000000 tencentcloud-sdk-python-nlp-3.0.880/tencentcloud/nlp/v20190408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    29728 2023-04-24 03:18:13.000000 tencentcloud-sdk-python-nlp-3.0.880/tencentcloud/nlp/v20190408/nlp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:18:13.000000 tencentcloud-sdk-python-nlp-3.0.880/tencentcloud/nlp/v20190408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56111 2023-04-24 03:18:13.000000 tencentcloud-sdk-python-nlp-3.0.880/tencentcloud/nlp/v20190408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:18:13.000000 tencentcloud-sdk-python-nlp-3.0.880/tencentcloud/nlp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:18:13.000000 tencentcloud-sdk-python-nlp-3.0.880/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:18:13.000000 tencentcloud-sdk-python-nlp-3.0.880/tencentcloud_sdk_python_nlp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:18:13.000000 tencentcloud-sdk-python-nlp-3.0.880/tencentcloud_sdk_python_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-24 03:18:13.000000 tencentcloud-sdk-python-nlp-3.0.880/tencentcloud_sdk_python_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:18:13.000000 tencentcloud-sdk-python-nlp-3.0.880/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:18:13.000000 tencentcloud-sdk-python-nlp-3.0.880/tencentcloud_sdk_python_nlp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:18:13.000000 tencentcloud-sdk-python-nlp-3.0.880/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 03:18:13.000000 tencentcloud-sdk-python-nlp-3.0.880/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:18:13.000000 tencentcloud-sdk-python-nlp-3.0.880/setup.cfg
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.878/README.rst` & `tencentcloud-sdk-python-nlp-3.0.880/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.878/tencentcloud/nlp/v20190408/errorcodes.py` & `tencentcloud-sdk-python-nlp-3.0.880/tencentcloud/nlp/v20190408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.878/tencentcloud/nlp/v20190408/nlp_client.py` & `tencentcloud-sdk-python-nlp-3.0.880/tencentcloud/nlp/v20190408/nlp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.878/tencentcloud/nlp/v20190408/models.py` & `tencentcloud-sdk-python-nlp-3.0.880/tencentcloud/nlp/v20190408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-nlp-3.0.878/tencentcloud/__init__.py` & `tencentcloud-sdk-python-nlp-3.0.880/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.878'
+__version__ = '3.0.880'
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.878/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-nlp-3.0.880/tencentcloud_sdk_python_nlp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-nlp
-Version: 3.0.878
+Version: 3.0.880
 Summary: Tencent Cloud Nlp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.878/PKG-INFO` & `tencentcloud-sdk-python-nlp-3.0.880/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-nlp
-Version: 3.0.878
+Version: 3.0.880
 Summary: Tencent Cloud Nlp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-nlp-3.0.878/setup.py` & `tencentcloud-sdk-python-nlp-3.0.880/setup.py`

 * *Files identical despite different names*

