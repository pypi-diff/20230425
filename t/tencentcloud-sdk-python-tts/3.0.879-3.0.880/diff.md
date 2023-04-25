# Comparing `tmp/tencentcloud-sdk-python-tts-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-tts-3.0.880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tts-3.0.879.tar", last modified: Fri Apr 21 01:08:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tts-3.0.880.tar", last modified: Mon Apr 24 03:48:24 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tts-3.0.879.tar` & `tencentcloud-sdk-python-tts-3.0.880.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud/tts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud/tts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud/tts/v20190823/
--rw-r--r--   0 root         (0) root         (0)     5481 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud/tts/v20190823/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud/tts/v20190823/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20734 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud/tts/v20190823/models.py
--rw-r--r--   0 root         (0) root         (0)     5910 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud/tts/v20190823/tts_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud_sdk_python_tts.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud_sdk_python_tts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud_sdk_python_tts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud_sdk_python_tts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/tencentcloud_sdk_python_tts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 01:08:57.000000 tencentcloud-sdk-python-tts-3.0.879/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:48:24.000000 tencentcloud-sdk-python-tts-3.0.880/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 03:48:24.000000 tencentcloud-sdk-python-tts-3.0.880/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:48:24.000000 tencentcloud-sdk-python-tts-3.0.880/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:48:24.000000 tencentcloud-sdk-python-tts-3.0.880/tencentcloud/tts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:48:24.000000 tencentcloud-sdk-python-tts-3.0.880/tencentcloud/tts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:48:24.000000 tencentcloud-sdk-python-tts-3.0.880/tencentcloud/tts/v20190823/
+-rw-r--r--   0 root         (0) root         (0)     5481 2023-04-24 03:48:24.000000 tencentcloud-sdk-python-tts-3.0.880/tencentcloud/tts/v20190823/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:48:24.000000 tencentcloud-sdk-python-tts-3.0.880/tencentcloud/tts/v20190823/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20710 2023-04-24 03:48:24.000000 tencentcloud-sdk-python-tts-3.0.880/tencentcloud/tts/v20190823/models.py
+-rw-r--r--   0 root         (0) root         (0)     5910 2023-04-24 03:48:24.000000 tencentcloud-sdk-python-tts-3.0.880/tencentcloud/tts/v20190823/tts_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:48:24.000000 tencentcloud-sdk-python-tts-3.0.880/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:48:24.000000 tencentcloud-sdk-python-tts-3.0.880/tencentcloud_sdk_python_tts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:48:24.000000 tencentcloud-sdk-python-tts-3.0.880/tencentcloud_sdk_python_tts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-24 03:48:24.000000 tencentcloud-sdk-python-tts-3.0.880/tencentcloud_sdk_python_tts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:48:24.000000 tencentcloud-sdk-python-tts-3.0.880/tencentcloud_sdk_python_tts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:48:24.000000 tencentcloud-sdk-python-tts-3.0.880/tencentcloud_sdk_python_tts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:48:24.000000 tencentcloud-sdk-python-tts-3.0.880/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 03:48:24.000000 tencentcloud-sdk-python-tts-3.0.880/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:48:24.000000 tencentcloud-sdk-python-tts-3.0.880/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tts-3.0.879/README.rst` & `tencentcloud-sdk-python-tts-3.0.880/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.879/tencentcloud/tts/v20190823/errorcodes.py` & `tencentcloud-sdk-python-tts-3.0.880/tencentcloud/tts/v20190823/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.879/tencentcloud/tts/v20190823/models.py` & `tencentcloud-sdk-python-tts-3.0.880/tencentcloud/tts/v20190823/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,15 +329,15 @@
         :type Codec: str
         :param EnableSubtitle: 是否开启时间戳功能，默认为false。
         :type EnableSubtitle: bool
         :param SegmentRate: 断句敏感阈值，默认值为：0，取值范围：[0,1,2]。该值越大越不容易断句，模型会更倾向于仅按照标点符号断句。此参数建议不要随意调整，可能会影响合成效果。
         :type SegmentRate: int
         :param EmotionCategory: 控制合成音频的情感，仅支持多情感音色使用。取值: neutral(中性)、sad(悲伤)、happy(高兴)、angry(生气)、fear(恐惧)、news(新闻)、story(故事)、radio(广播)、poetry(诗歌)、call(客服)
         :type EmotionCategory: str
-        :param EmotionIntensity: 控制合成音频情感程度，取值范围为[50,200],默认为100，不填写为默认值；只有EmotionCategory不为空时生效；
+        :param EmotionIntensity: 控制合成音频情感程度，取值范围为[50,200],默认为100；只有EmotionCategory不为空时生效；
         :type EmotionIntensity: int
         """
         self.Text = None
         self.SessionId = None
         self.Volume = None
         self.Speed = None
         self.ProjectId = None
```

### Comparing `tencentcloud-sdk-python-tts-3.0.879/tencentcloud/tts/v20190823/tts_client.py` & `tencentcloud-sdk-python-tts-3.0.880/tencentcloud/tts/v20190823/tts_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tts-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tts-3.0.880/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tts-3.0.879/tencentcloud_sdk_python_tts.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tts-3.0.880/tencentcloud_sdk_python_tts.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tts
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Tts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tts-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-tts-3.0.880/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tts
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Tts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tts-3.0.879/setup.py` & `tencentcloud-sdk-python-tts-3.0.880/setup.py`

 * *Files identical despite different names*

