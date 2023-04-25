# Comparing `tmp/tencentcloud-sdk-python-tmt-3.0.880.tar.gz` & `tmp/tencentcloud-sdk-python-tmt-3.0.881.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tmt-3.0.880.tar", last modified: Mon Apr 24 03:47:12 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tmt-3.0.881.tar", last modified: Tue Apr 25 00:59:24 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tmt-3.0.880.tar` & `tencentcloud-sdk-python-tmt-3.0.881.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:47:12.000000 tencentcloud-sdk-python-tmt-3.0.880/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-24 03:47:11.000000 tencentcloud-sdk-python-tmt-3.0.880/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:47:12.000000 tencentcloud-sdk-python-tmt-3.0.880/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-24 03:47:11.000000 tencentcloud-sdk-python-tmt-3.0.880/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:47:12.000000 tencentcloud-sdk-python-tmt-3.0.880/tencentcloud/tmt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:47:12.000000 tencentcloud-sdk-python-tmt-3.0.880/tencentcloud/tmt/v20180321/
--rw-r--r--   0 root         (0) root         (0)     3396 2023-04-24 03:47:11.000000 tencentcloud-sdk-python-tmt-3.0.880/tencentcloud/tmt/v20180321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:47:11.000000 tencentcloud-sdk-python-tmt-3.0.880/tencentcloud/tmt/v20180321/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9404 2023-04-24 03:47:11.000000 tencentcloud-sdk-python-tmt-3.0.880/tencentcloud/tmt/v20180321/tmt_client.py
--rw-r--r--   0 root         (0) root         (0)    33822 2023-04-24 03:47:11.000000 tencentcloud-sdk-python-tmt-3.0.880/tencentcloud/tmt/v20180321/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 03:47:11.000000 tencentcloud-sdk-python-tmt-3.0.880/tencentcloud/tmt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 03:47:12.000000 tencentcloud-sdk-python-tmt-3.0.880/tencentcloud_sdk_python_tmt.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 03:47:12.000000 tencentcloud-sdk-python-tmt-3.0.880/tencentcloud_sdk_python_tmt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-24 03:47:12.000000 tencentcloud-sdk-python-tmt-3.0.880/tencentcloud_sdk_python_tmt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:47:12.000000 tencentcloud-sdk-python-tmt-3.0.880/tencentcloud_sdk_python_tmt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-24 03:47:12.000000 tencentcloud-sdk-python-tmt-3.0.880/tencentcloud_sdk_python_tmt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-24 03:47:12.000000 tencentcloud-sdk-python-tmt-3.0.880/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-24 03:47:11.000000 tencentcloud-sdk-python-tmt-3.0.880/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-24 03:47:12.000000 tencentcloud-sdk-python-tmt-3.0.880/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:59:24.000000 tencentcloud-sdk-python-tmt-3.0.881/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-25 00:59:23.000000 tencentcloud-sdk-python-tmt-3.0.881/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:59:24.000000 tencentcloud-sdk-python-tmt-3.0.881/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-25 00:59:23.000000 tencentcloud-sdk-python-tmt-3.0.881/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:59:24.000000 tencentcloud-sdk-python-tmt-3.0.881/tencentcloud/tmt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:59:24.000000 tencentcloud-sdk-python-tmt-3.0.881/tencentcloud/tmt/v20180321/
+-rw-r--r--   0 root         (0) root         (0)     3585 2023-04-25 00:59:23.000000 tencentcloud-sdk-python-tmt-3.0.881/tencentcloud/tmt/v20180321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:59:23.000000 tencentcloud-sdk-python-tmt-3.0.881/tencentcloud/tmt/v20180321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9401 2023-04-25 00:59:23.000000 tencentcloud-sdk-python-tmt-3.0.881/tencentcloud/tmt/v20180321/tmt_client.py
+-rw-r--r--   0 root         (0) root         (0)    33942 2023-04-25 00:59:23.000000 tencentcloud-sdk-python-tmt-3.0.881/tencentcloud/tmt/v20180321/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 00:59:23.000000 tencentcloud-sdk-python-tmt-3.0.881/tencentcloud/tmt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 00:59:24.000000 tencentcloud-sdk-python-tmt-3.0.881/tencentcloud_sdk_python_tmt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 00:59:23.000000 tencentcloud-sdk-python-tmt-3.0.881/tencentcloud_sdk_python_tmt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-25 00:59:24.000000 tencentcloud-sdk-python-tmt-3.0.881/tencentcloud_sdk_python_tmt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:59:23.000000 tencentcloud-sdk-python-tmt-3.0.881/tencentcloud_sdk_python_tmt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 00:59:23.000000 tencentcloud-sdk-python-tmt-3.0.881/tencentcloud_sdk_python_tmt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-25 00:59:24.000000 tencentcloud-sdk-python-tmt-3.0.881/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-25 00:59:23.000000 tencentcloud-sdk-python-tmt-3.0.881/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-25 00:59:24.000000 tencentcloud-sdk-python-tmt-3.0.881/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.880/README.rst` & `tencentcloud-sdk-python-tmt-3.0.881/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tmt-3.0.880/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tmt-3.0.881/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tmt-3.0.880/tencentcloud/tmt/v20180321/errorcodes.py` & `tencentcloud-sdk-python-tmt-3.0.881/tencentcloud/tmt/v20180321/errorcodes.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
 # 操作失败。
 FAILEDOPERATION = 'FailedOperation'
 
 # 数据插入错误。
 FAILEDOPERATION_INSERTERR = 'FailedOperation.InsertErr'
 
+# 暂时无法识别该语种。
+FAILEDOPERATION_LANGUAGERECOGNITIONERR = 'FailedOperation.LanguageRecognitionErr'
+
 # 本月免费额度已用完，如需继续使用您可以在机器翻译控制台升级为付费使用。
 FAILEDOPERATION_NOFREEAMOUNT = 'FailedOperation.NoFreeAmount'
 
 # 内部请求错误。
 FAILEDOPERATION_REQUESTAILABERR = 'FailedOperation.RequestAiLabErr'
 
 # 账号因为欠费停止服务，请在腾讯云账户充值。
@@ -55,14 +58,17 @@
 
 # 参数错误。
 INVALIDPARAMETER_MISSINGPARAMETER = 'InvalidParameter.MissingParameter'
 
 # Seq之间的间隙请不要大于2000。
 INVALIDPARAMETER_SEQINTERVALTOOLARGE = 'InvalidParameter.SeqIntervalTooLarge'
 
+# 参数取值错误。
+INVALIDPARAMETERVALUE = 'InvalidParameterValue'
+
 # 超过配额限制。
 LIMITEXCEEDED = 'LimitExceeded'
 
 # 超出请求频率。
 LIMITEXCEEDED_LIMITEDACCESSFREQUENCY = 'LimitExceeded.LimitedAccessFrequency'
 
 # 缺少参数错误。
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.880/tencentcloud/tmt/v20180321/tmt_client.py` & `tencentcloud-sdk-python-tmt-3.0.881/tencentcloud/tmt/v20180321/tmt_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def GetFileTranslate(self, request):
         """在调用文档翻译请求接口后，有回调和轮询两种方式获取识别结果。
-        •当采用回调方式时，翻译完成后会将结果通过 POST 请求的形式通知到用户在请求时填写的回调 URL，具体请参见文档翻译结果回调 。
+        •当采用回调方式时，翻译完成后会将结果通过 POST 请求的形式通知到用户在请求时填写的回调 URL，具体请参见文档翻译结果回调。
         • 当采用轮询方式时，需要主动提交任务ID来轮询识别结果，共有任务成功、等待、执行中和失败四种结果，具体信息请参见参数说明。
 
         :param request: Request instance for GetFileTranslate.
         :type request: :class:`tencentcloud.tmt.v20180321.models.GetFileTranslateRequest`
         :rtype: :class:`tencentcloud.tmt.v20180321.models.GetFileTranslateResponse`
 
         """
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.880/tencentcloud/tmt/v20180321/models.py` & `tencentcloud-sdk-python-tmt-3.0.881/tencentcloud/tmt/v20180321/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,19 +61,19 @@
 km（高棉语）：zh（简体中文）、zh-HK（繁体中文）、 zh-TW（繁体中文)、zh-TR(繁体中文）
 lo（老挝语）：zh（简体中文）、zh-HK（繁体中文）、 zh-TW（繁体中文)、zh-TR(繁体中文）
         :type Target: str
         :param DocumentType: 文档类型：可支持以下几种(pdf,docx,pptx,xlsx,txt,xml,html,markdown,properties)
         :type DocumentType: str
         :param SourceType: 数据来源，0：url，1：直接传文件编码后数据
         :type SourceType: int
-        :param Url: 需要翻译文件url
+        :param Url: 需要翻译文件url，文件需小于100MB。
         :type Url: str
         :param BasicDocumentType: 原始文档类型
         :type BasicDocumentType: str
-        :param CallbackUrl: 回调url
+        :param CallbackUrl: 回调url，文件大于10MB，建议采用回调方式；回调时，所有内容会放入 Body 中。
         :type CallbackUrl: str
         :param Data: 文件数据，当SourceType 值为1时必须填写，为0可不写。要base64编码(采用python语言时注意读取文件应该为string而不是byte，以byte格式读取后要decode()。编码后的数据不可带有回车换行符)。数据要小于5MB。
         :type Data: str
         """
         self.Source = None
         self.Target = None
         self.DocumentType = None
@@ -611,15 +611,15 @@
 <li>th（泰语）：zh（中文）、en（英语）</li>
 <li>ms（马来语）：zh（中文）、en（英语）</li>
 <li>ar（阿拉伯语）：en（英语）</li>
 <li>hi（印地语）：en（英语）</li>
         :type Target: str
         :param ProjectId: 项目ID，可以根据控制台-账号中心-项目管理中的配置填写，如无配置请填写默认项目ID:0
         :type ProjectId: int
-        :param SourceTextList: 待翻译的文本列表，批量接口可以以数组方式在一次请求中填写多个待翻译文本。文本统一使用utf-8格式编码，非utf-8格式编码字符会翻译失败，请传入有效文本，html标记等非常规翻译文本可能会翻译失败。单次请求的文本长度总和需要低于2000字符。
+        :param SourceTextList: 待翻译的文本列表，批量接口可以以数组方式在一次请求中填写多个待翻译文本。文本统一使用utf-8格式编码，非utf-8格式编码字符会翻译失败，请传入有效文本，html标记等非常规翻译文本可能会翻译失败。单次请求的文本长度总和需要低于6000字符。
         :type SourceTextList: list of str
         """
         self.Source = None
         self.Target = None
         self.ProjectId = None
         self.SourceTextList = None
 
@@ -641,15 +641,15 @@
 class TextTranslateBatchResponse(AbstractModel):
     """TextTranslateBatch返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Source: 源语言，详见入参Target
+        :param Source: 源语言，详见入参Source
         :type Source: str
         :param Target: 目标语言，详见入参Target
         :type Target: str
         :param TargetTextList: 翻译后的文本列表
         :type TargetTextList: list of str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
@@ -670,15 +670,15 @@
 class TextTranslateRequest(AbstractModel):
     """TextTranslate请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param SourceText: 待翻译的文本，文本统一使用utf-8格式编码，非utf-8格式编码字符会翻译失败，请传入有效文本，html标记等非常规翻译文本可能会翻译失败。单次请求的文本长度需要低于2000字符。
+        :param SourceText: 待翻译的文本，文本统一使用utf-8格式编码，非utf-8格式编码字符会翻译失败，请传入有效文本，html标记等非常规翻译文本可能会翻译失败。单次请求的文本长度需要低于6000字符。
         :type SourceText: str
         :param Source: 源语言，支持：
 auto：自动识别（识别为一种语言）
 zh：简体中文
 zh-TW：繁体中文
 en：英语
 ja：日语
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.880/tencentcloud_sdk_python_tmt.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tmt-3.0.881/tencentcloud_sdk_python_tmt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tmt
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Tmt SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.880/PKG-INFO` & `tencentcloud-sdk-python-tmt-3.0.881/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tmt
-Version: 3.0.880
+Version: 3.0.881
 Summary: Tencent Cloud Tmt SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tmt-3.0.880/setup.py` & `tencentcloud-sdk-python-tmt-3.0.881/setup.py`

 * *Files identical despite different names*

