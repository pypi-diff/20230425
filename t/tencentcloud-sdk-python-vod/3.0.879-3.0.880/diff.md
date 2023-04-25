# Comparing `tmp/tencentcloud-sdk-python-vod-3.0.879.tar.gz` & `tmp/tencentcloud-sdk-python-vod-3.0.880.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.879.tar", last modified: Fri Apr 21 01:09:25 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.880.tar", last modified: Mon Apr 24 03:48:52 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vod-3.0.879.tar` & `tencentcloud-sdk-python-vod-3.0.880.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud/vod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud/vod/v20180717/
--rw-r--r--   0 root         (0) root         (0)   172410 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud/vod/v20180717/vod_client.py
--rw-r--r--   0 root         (0) root         (0)    25016 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud/vod/v20180717/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud/vod/v20180717/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1170904 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud/vod/v20180717/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud/vod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud_sdk_python_vod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/tencentcloud_sdk_python_vod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-21 01:09:25.000000 tencentcloud-sdk-python-vod-3.0.879/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 03:48:51.000000 tencentcloud-sdk-python-vod-3.0.880/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud/vod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud/vod/v20180717/
+-rw-r--r--   0 root         (0) root         (0)   172410 2023-04-24 03:48:51.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud/vod/v20180717/vod_client.py
+-rw-r--r--   0 root         (0) root         (0)    25016 2023-04-24 03:48:51.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud/vod/v20180717/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:48:51.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud/vod/v20180717/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1171666 2023-04-24 03:48:51.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud/vod/v20180717/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:48:51.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud/vod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:48:51.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud_sdk_python_vod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/tencentcloud_sdk_python_vod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 03:48:51.000000 tencentcloud-sdk-python-vod-3.0.880/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:48:52.000000 tencentcloud-sdk-python-vod-3.0.880/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vod-3.0.879/README.rst` & `tencentcloud-sdk-python-vod-3.0.880/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.879/tencentcloud/vod/v20180717/vod_client.py` & `tencentcloud-sdk-python-vod-3.0.880/tencentcloud/vod/v20180717/vod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.879/tencentcloud/vod/v20180717/errorcodes.py` & `tencentcloud-sdk-python-vod-3.0.880/tencentcloud/vod/v20180717/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.879/tencentcloud/vod/v20180717/models.py` & `tencentcloud-sdk-python-vod-3.0.880/tencentcloud/vod/v20180717/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4594,24 +4594,33 @@
 <li>srt：生成 SRT 字幕文件。</li>
         :type SubtitleFormats: list of str
         :param SubtitleFormat: 生成的字幕文件格式，不填或者填空字符串表示不生成字幕文件，可选值：
 <li>vtt：生成 WebVTT 字幕文件；</li>
 <li>srt：生成 SRT 字幕文件。</li>
 <font color='red'>注意：此字段已废弃，建议使用 SubtitleFormats。</font>
         :type SubtitleFormat: str
+        :param SrcLanguage: 媒体源语言，取值范围：
+<li>zh：中文普通话；</li>
+<li>en：英语；</li>
+<li>ja：日语；</li>
+<li>zh-ca：粤语。</li>
+<font color=red>注意：</font> 填空字符串，或者不填该参数，则自动识别（效果较难保证，推荐填写原始媒体对应的语言，以提高识别的准确率）。
+        :type SrcLanguage: str
         """
         self.Switch = None
         self.SubtitleFormats = None
         self.SubtitleFormat = None
+        self.SrcLanguage = None
 
 
     def _deserialize(self, params):
         self.Switch = params.get("Switch")
         self.SubtitleFormats = params.get("SubtitleFormats")
         self.SubtitleFormat = params.get("SubtitleFormat")
+        self.SrcLanguage = params.get("SrcLanguage")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4631,26 +4640,34 @@
         :param SubtitleFormatsOperation: 字幕格式列表操作信息。
         :type SubtitleFormatsOperation: :class:`tencentcloud.vod.v20180717.models.SubtitleFormatsOperation`
         :param SubtitleFormat: 生成的字幕文件格式，<font color='red'>填空字符串</font>表示不生成字幕文件，可选值：
 <li>vtt：生成 WebVTT 字幕文件；</li>
 <li>srt：生成 SRT 字幕文件。</li>
 <font color='red'>注意：此字段已废弃，建议使用 SubtitleFormatsOperation。</font>
         :type SubtitleFormat: str
+        :param SrcLanguage: 媒体源语言，取值范围：
+<li>zh：中文普通话；</li>
+<li>en：英语；</li>
+<li>ja：日语；</li>
+<li>zh-ca：粤语。</li>
+        :type SrcLanguage: str
         """
         self.Switch = None
         self.SubtitleFormatsOperation = None
         self.SubtitleFormat = None
+        self.SrcLanguage = None
 
 
     def _deserialize(self, params):
         self.Switch = params.get("Switch")
         if params.get("SubtitleFormatsOperation") is not None:
             self.SubtitleFormatsOperation = SubtitleFormatsOperation()
             self.SubtitleFormatsOperation._deserialize(params.get("SubtitleFormatsOperation"))
         self.SubtitleFormat = params.get("SubtitleFormat")
+        self.SrcLanguage = params.get("SrcLanguage")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-vod-3.0.879/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vod-3.0.880/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vod-3.0.879/tencentcloud_sdk_python_vod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.880/tencentcloud_sdk_python_vod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.879/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.880/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.879
+Version: 3.0.880
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.879/setup.py` & `tencentcloud-sdk-python-vod-3.0.880/setup.py`

 * *Files identical despite different names*

