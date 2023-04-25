# Comparing `tmp/machkit-0.1.0.tar.gz` & `tmp/machkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "machkit-0.1.0.tar", last modified: Mon Apr 24 10:12:01 2023, max compression
+gzip compressed data, was "machkit-0.1.1.tar", last modified: Tue Apr 25 03:01:18 2023, max compression
```

## Comparing `machkit-0.1.0.tar` & `machkit-0.1.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 garry      (501) staff       (20)        0 2023-04-24 10:12:01.165161 machkit-0.1.0/
--rw-r--r--   0 garry      (501) staff       (20)      292 2023-04-24 10:12:01.165327 machkit-0.1.0/PKG-INFO
--rw-r--r--   0 garry      (501) staff       (20)     1922 2023-04-24 10:07:54.000000 machkit-0.1.0/README.md
-drwxr-xr-x   0 garry      (501) staff       (20)        0 2023-04-24 10:12:01.122298 machkit-0.1.0/datappkit/
--rw-r--r--   0 garry      (501) staff       (20)       35 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/__init__.py
-drwxr-xr-x   0 garry      (501) staff       (20)        0 2023-04-24 10:12:01.126258 machkit-0.1.0/datappkit/common/
--rw-r--r--   0 garry      (501) staff       (20)       64 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/common/__init__.py
--rw-r--r--   0 garry      (501) staff       (20)      557 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/common/config.py
--rw-r--r--   0 garry      (501) staff       (20)     1955 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/common/datapp_response.py
--rw-r--r--   0 garry      (501) staff       (20)        0 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/common/quota_manager.py
--rw-r--r--   0 garry      (501) staff       (20)        0 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/common/user_manager.py
-drwxr-xr-x   0 garry      (501) staff       (20)        0 2023-04-24 10:12:01.137365 machkit-0.1.0/datappkit/controller/
--rw-r--r--   0 garry      (501) staff       (20)      139 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/controller/__init__.py
--rw-r--r--   0 garry      (501) staff       (20)      692 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/controller/batches_controller.py
--rw-r--r--   0 garry      (501) staff       (20)      258 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/controller/file_controller.py
--rw-r--r--   0 garry      (501) staff       (20)      316 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/controller/label_controller.py
--rw-r--r--   0 garry      (501) staff       (20)      493 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/controller/requirement_controller.py
--rw-r--r--   0 garry      (501) staff       (20)      404 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/controller/user_controller.py
--rw-r--r--   0 garry      (501) staff       (20)     4115 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/datapp.py
-drwxr-xr-x   0 garry      (501) staff       (20)        0 2023-04-24 10:12:01.144653 machkit-0.1.0/datappkit/services/
--rw-r--r--   0 garry      (501) staff       (20)      144 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/services/__init__.py
--rw-r--r--   0 garry      (501) staff       (20)     4548 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/services/base_request.py
--rw-r--r--   0 garry      (501) staff       (20)     2065 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/services/batches_service.py
--rw-r--r--   0 garry      (501) staff       (20)     1795 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/services/file_service.py
--rw-r--r--   0 garry      (501) staff       (20)     1047 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/services/label_service.py
--rw-r--r--   0 garry      (501) staff       (20)     4825 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/services/requirement_service.py
--rw-r--r--   0 garry      (501) staff       (20)     2503 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/services/user_service.py
-drwxr-xr-x   0 garry      (501) staff       (20)        0 2023-04-24 10:12:01.146121 machkit-0.1.0/datappkit/utils/
--rw-r--r--   0 garry      (501) staff       (20)        0 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/utils/__init__.py
--rw-r--r--   0 garry      (501) staff       (20)     1567 2023-04-24 10:07:54.000000 machkit-0.1.0/datappkit/utils/file_utils.py
-drwxr-xr-x   0 garry      (501) staff       (20)        0 2023-04-24 10:12:01.154487 machkit-0.1.0/machkit.egg-info/
--rw-r--r--   0 garry      (501) staff       (20)      292 2023-04-24 10:12:00.000000 machkit-0.1.0/machkit.egg-info/PKG-INFO
--rw-r--r--   0 garry      (501) staff       (20)     1137 2023-04-24 10:12:01.000000 machkit-0.1.0/machkit.egg-info/SOURCES.txt
--rw-r--r--   0 garry      (501) staff       (20)        1 2023-04-24 10:12:00.000000 machkit-0.1.0/machkit.egg-info/dependency_links.txt
--rw-r--r--   0 garry      (501) staff       (20)       17 2023-04-24 10:12:00.000000 machkit-0.1.0/machkit.egg-info/requires.txt
--rw-r--r--   0 garry      (501) staff       (20)       16 2023-04-24 10:12:00.000000 machkit-0.1.0/machkit.egg-info/top_level.txt
--rw-r--r--   0 garry      (501) staff       (20)       78 2023-04-24 10:12:01.169592 machkit-0.1.0/setup.cfg
--rw-r--r--   0 garry      (501) staff       (20)      721 2023-04-24 10:07:54.000000 machkit-0.1.0/setup.py
-drwxr-xr-x   0 garry      (501) staff       (20)        0 2023-04-24 10:12:01.164540 machkit-0.1.0/tests/
--rw-r--r--   0 garry      (501) staff       (20)       55 2023-04-24 10:07:54.000000 machkit-0.1.0/tests/__init__.py
--rw-r--r--   0 garry      (501) staff       (20)        0 2023-04-24 10:07:54.000000 machkit-0.1.0/tests/test_basic.py
--rw-r--r--   0 garry      (501) staff       (20)     3998 2023-04-24 10:07:54.000000 machkit-0.1.0/tests/test_batch.py
--rw-r--r--   0 garry      (501) staff       (20)      260 2023-04-24 10:07:54.000000 machkit-0.1.0/tests/test_file.py
--rw-r--r--   0 garry      (501) staff       (20)     1499 2023-04-24 10:07:54.000000 machkit-0.1.0/tests/test_label.py
--rw-r--r--   0 garry      (501) staff       (20)      449 2023-04-24 10:07:54.000000 machkit-0.1.0/tests/test_login.py
--rw-r--r--   0 garry      (501) staff       (20)      220 2023-04-24 10:07:54.000000 machkit-0.1.0/tests/test_otp.py
--rw-r--r--   0 garry      (501) staff       (20)     2427 2023-04-24 10:07:54.000000 machkit-0.1.0/tests/test_requirement.py
--rw-r--r--   0 garry      (501) staff       (20)     1416 2023-04-24 10:07:54.000000 machkit-0.1.0/tests/test_token.py
--rw-r--r--   0 garry      (501) staff       (20)     1565 2023-04-24 10:07:54.000000 machkit-0.1.0/tests/test_user.py
+drwxr-xr-x   0 garry      (501) staff       (20)        0 2023-04-25 03:01:18.582151 machkit-0.1.1/
+-rw-r--r--   0 garry      (501) staff       (20)      292 2023-04-25 03:01:18.582384 machkit-0.1.1/PKG-INFO
+-rw-r--r--   0 garry      (501) staff       (20)     1910 2023-04-25 02:55:57.000000 machkit-0.1.1/README.md
+drwxr-xr-x   0 garry      (501) staff       (20)        0 2023-04-25 03:01:18.543132 machkit-0.1.1/machkit/
+-rw-r--r--   0 garry      (501) staff       (20)       34 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/__init__.py
+drwxr-xr-x   0 garry      (501) staff       (20)        0 2023-04-25 03:01:18.551450 machkit-0.1.1/machkit/common/
+-rw-r--r--   0 garry      (501) staff       (20)       62 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/common/__init__.py
+-rw-r--r--   0 garry      (501) staff       (20)      555 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/common/config.py
+-rw-r--r--   0 garry      (501) staff       (20)     1955 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/common/datapp_response.py
+-rw-r--r--   0 garry      (501) staff       (20)        0 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/common/quota_manager.py
+-rw-r--r--   0 garry      (501) staff       (20)        0 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/common/user_manager.py
+drwxr-xr-x   0 garry      (501) staff       (20)        0 2023-04-25 03:01:18.556128 machkit-0.1.1/machkit/controller/
+-rw-r--r--   0 garry      (501) staff       (20)      139 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/controller/__init__.py
+-rw-r--r--   0 garry      (501) staff       (20)      690 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/controller/batches_controller.py
+-rw-r--r--   0 garry      (501) staff       (20)      256 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/controller/file_controller.py
+-rw-r--r--   0 garry      (501) staff       (20)      314 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/controller/label_controller.py
+-rw-r--r--   0 garry      (501) staff       (20)      491 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/controller/requirement_controller.py
+-rw-r--r--   0 garry      (501) staff       (20)      402 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/controller/user_controller.py
+-rw-r--r--   0 garry      (501) staff       (20)     4105 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/machkit.py
+drwxr-xr-x   0 garry      (501) staff       (20)        0 2023-04-25 03:01:18.563302 machkit-0.1.1/machkit/services/
+-rw-r--r--   0 garry      (501) staff       (20)      144 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/services/__init__.py
+-rw-r--r--   0 garry      (501) staff       (20)     4544 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/services/base_request.py
+-rw-r--r--   0 garry      (501) staff       (20)     2063 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/services/batches_service.py
+-rw-r--r--   0 garry      (501) staff       (20)     1795 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/services/file_service.py
+-rw-r--r--   0 garry      (501) staff       (20)     1045 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/services/label_service.py
+-rw-r--r--   0 garry      (501) staff       (20)     4823 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/services/requirement_service.py
+-rw-r--r--   0 garry      (501) staff       (20)     2497 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/services/user_service.py
+drwxr-xr-x   0 garry      (501) staff       (20)        0 2023-04-25 03:01:18.564663 machkit-0.1.1/machkit/utils/
+-rw-r--r--   0 garry      (501) staff       (20)        0 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/utils/__init__.py
+-rw-r--r--   0 garry      (501) staff       (20)     1567 2023-04-25 02:55:57.000000 machkit-0.1.1/machkit/utils/file_utils.py
+drwxr-xr-x   0 garry      (501) staff       (20)        0 2023-04-25 03:01:18.547848 machkit-0.1.1/machkit.egg-info/
+-rw-r--r--   0 garry      (501) staff       (20)      292 2023-04-25 03:01:18.000000 machkit-0.1.1/machkit.egg-info/PKG-INFO
+-rw-r--r--   0 garry      (501) staff       (20)     1094 2023-04-25 03:01:18.000000 machkit-0.1.1/machkit.egg-info/SOURCES.txt
+-rw-r--r--   0 garry      (501) staff       (20)        1 2023-04-25 03:01:18.000000 machkit-0.1.1/machkit.egg-info/dependency_links.txt
+-rw-r--r--   0 garry      (501) staff       (20)       17 2023-04-25 03:01:18.000000 machkit-0.1.1/machkit.egg-info/requires.txt
+-rw-r--r--   0 garry      (501) staff       (20)       14 2023-04-25 03:01:18.000000 machkit-0.1.1/machkit.egg-info/top_level.txt
+-rw-r--r--   0 garry      (501) staff       (20)       78 2023-04-25 03:01:18.583582 machkit-0.1.1/setup.cfg
+-rw-r--r--   0 garry      (501) staff       (20)      721 2023-04-25 03:01:08.000000 machkit-0.1.1/setup.py
+drwxr-xr-x   0 garry      (501) staff       (20)        0 2023-04-25 03:01:18.577096 machkit-0.1.1/tests/
+-rw-r--r--   0 garry      (501) staff       (20)       55 2023-04-24 10:07:54.000000 machkit-0.1.1/tests/__init__.py
+-rw-r--r--   0 garry      (501) staff       (20)        0 2023-04-24 10:07:54.000000 machkit-0.1.1/tests/test_basic.py
+-rw-r--r--   0 garry      (501) staff       (20)     3995 2023-04-25 02:55:57.000000 machkit-0.1.1/tests/test_batch.py
+-rw-r--r--   0 garry      (501) staff       (20)      258 2023-04-25 02:55:57.000000 machkit-0.1.1/tests/test_file.py
+-rw-r--r--   0 garry      (501) staff       (20)     1495 2023-04-25 02:55:57.000000 machkit-0.1.1/tests/test_label.py
+-rw-r--r--   0 garry      (501) staff       (20)      575 2023-04-25 02:55:57.000000 machkit-0.1.1/tests/test_login.py
+-rw-r--r--   0 garry      (501) staff       (20)      220 2023-04-24 10:07:54.000000 machkit-0.1.1/tests/test_otp.py
+-rw-r--r--   0 garry      (501) staff       (20)     2542 2023-04-25 02:55:57.000000 machkit-0.1.1/tests/test_requirement.py
+-rw-r--r--   0 garry      (501) staff       (20)     1416 2023-04-24 10:07:54.000000 machkit-0.1.1/tests/test_token.py
+-rw-r--r--   0 garry      (501) staff       (20)     1561 2023-04-25 02:55:57.000000 machkit-0.1.1/tests/test_user.py
```

### Comparing `machkit-0.1.0/README.md` & `machkit-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,55 @@
-# datappkit
+# machkit
 
 ## 简介
 
-datappkit 是一个对数据操作的SDK，为接入方提供对标注和统计等平台沟通的接口
+machkit 是一个对数据操作的 SDK，为接入方提供对标注和统计等平台沟通的接口
 
 ## 安装
 
 普通用户安装：
 
-``` shell
-pip install datappkit
+```shell
+pip install machkit
 ```
 
 开发者：
 
-``` shell
-git clone git@git-core.megvii-inc.com:brain/label/infrastructure/data-service-sdk.git
+```shell
+git clone git@git-core.megvii-inc.com:transformer/yueying/data-service-sdk.git
 cd data-service-sdk
 pip install -r requirements.txt
 pip install -r requirements-dev.txt
 ```
 
 ## 使用
 
-Debug模式
+Debug 模式
+
 ```
 执行export DATAPP_KIT_DEBUG=on 可开启测试环境，所有接口会打到平台的dev环境
 ```
 
 代码调用
+
 ```python
-from datappkit.datapp import Datapp
+from machkit.machkit import Datapp
 
 datapp = Datapp()
 datapp.login("account", "pwd")
 datapp.get_requirement(1079)
 # 其他功能见datapp模块提供的注释 或接口文档：https://wiki.megvii-inc.com/pages/viewpage.action?pageId=346934255
 ```
 
 ## 工程结构：
+
 ```
 .
 ├── README.md
-├── datappkit #核心代码包
+├── machkit #核心代码包
 │   ├── __init__.py
 │   ├── common #通用基础包
 │   │   ├── __init__.py
 │   │   └── quota_manager.py #配额管理
 │   │   └── ...
 │   ├── controller #控制层，接收事件并转发给service
 │   │   ├── __init__.py
@@ -68,8 +71,8 @@
 ├── requirements.txt #开发依赖
 ├── setup.py #打包和发布管理模块
 ├── tests
 │   ├── __init__.py
 │   └── test_basic.py
 │   └── ...
 └── venv
-```
+```
```

### Comparing `machkit-0.1.0/datappkit/common/config.py` & `machkit-0.1.1/machkit/common/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from datappkit.utils import file_utils
+from machkit.utils import file_utils
 
 
 _t_filename = os.environ['HOME'] + os.sep + ".datapp-kit.session"
 _token = ''
 
 
 def debug():
```

### Comparing `machkit-0.1.0/datappkit/common/datapp_response.py` & `machkit-0.1.1/machkit/common/datapp_response.py`

 * *Files identical despite different names*

### Comparing `machkit-0.1.0/datappkit/controller/batches_controller.py` & `machkit-0.1.1/machkit/controller/batches_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datappkit.services.batches_service import BatchesService
+from machkit.services.batches_service import BatchesService
 
 
 class BatchesController:
 
     def __init__(self):
         self.service = BatchesService()
```

### Comparing `machkit-0.1.0/datappkit/datapp.py` & `machkit-0.1.1/machkit/machkit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from datappkit.controller.batches_controller import BatchesController
-from datappkit.controller.file_controller import FileController
-from datappkit.controller.label_controller import LabelController
-from datappkit.controller.requirement_controller import RequirementController
-from datappkit.controller.user_controller import UserController
+from machkit.controller.batches_controller import BatchesController
+from machkit.controller.file_controller import FileController
+from machkit.controller.label_controller import LabelController
+from machkit.controller.requirement_controller import RequirementController
+from machkit.controller.user_controller import UserController
 
 
 class Datapp:
     """
     datapp工具入口
     """
```

### Comparing `machkit-0.1.0/datappkit/services/base_request.py` & `machkit-0.1.1/machkit/services/base_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 from collections import OrderedDict
 from typing import Any, Dict, Optional, Tuple
 
 import requests
 from requests import Response
 from requests.models import RequestEncodingMixin
-import datappkit.common.config as config
-from datappkit.common.datapp_response import DatappResponse
+import machkit.common.config as config
+from machkit.common.datapp_response import DatappResponse
 
 YUEYING_HOST_DEV = "https://galaxy-api-test.mach-drive.com"
 YUEYING_HOST_PROD = "https://api.mach-drive.com"
 
 # 登录
 YUEYING_LOGIN_URI = "/guc/v1/login?type=1&platform_id=20"
 # 获取当前用户信息
```

### Comparing `machkit-0.1.0/datappkit/services/batches_service.py` & `machkit-0.1.1/machkit/services/batches_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datappkit.services.base_request import BaseRequest, GET_BATCHES, POST_BATCHES_PUBLISH, GET_BATCHES_CONFIG, \
+from machkit.services.base_request import BaseRequest, GET_BATCHES, POST_BATCHES_PUBLISH, GET_BATCHES_CONFIG, \
     GET_BATCH, POST_BATCHES_CONFIGS
 
 
 class BatchesService:
 
     def get_batch(self, batch_id):
         uri = GET_BATCH.format(batchId=batch_id)
```

### Comparing `machkit-0.1.0/datappkit/services/file_service.py` & `machkit-0.1.1/machkit/services/file_service.py`

 * *Files identical despite different names*

### Comparing `machkit-0.1.0/datappkit/services/label_service.py` & `machkit-0.1.1/machkit/services/label_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datappkit.services.base_request import BaseRequest, GET_LABEL_TYPE_URI, GET_LABEL_TASK
+from machkit.services.base_request import BaseRequest, GET_LABEL_TYPE_URI, GET_LABEL_TASK
 
 
 class LabelService:
 
     def get_label_type(self):
         res, data = BaseRequest('GET', GET_LABEL_TYPE_URI, {}).request()
         type_list = []
```

### Comparing `machkit-0.1.0/datappkit/services/requirement_service.py` & `machkit-0.1.1/machkit/services/requirement_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datappkit.services.base_request import BaseRequest, GET_REQUIREMENT_DETAIL_URI, POST_REQUIREMENT_URI, GET_REQUIREMENT_URI, \
+from machkit.services.base_request import BaseRequest, GET_REQUIREMENT_DETAIL_URI, POST_REQUIREMENT_URI, GET_REQUIREMENT_URI, \
     PATCH_REQUIREMENT_URI
 
 
 class RequirementService:
 
     def create(self, data):
         body = {
```

### Comparing `machkit-0.1.0/datappkit/services/user_service.py` & `machkit-0.1.1/machkit/services/user_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from datappkit.common import config
-from datappkit.common.datapp_response import DatappResponse
-from datappkit.services.base_request import BaseRequest, CURRENT_YUEYING_USER_URI, YUEYING_LOGIN_URI, SEARCH_EMPLOYEE, \
+from machkit.common import config
+from machkit.common.datapp_response import DatappResponse
+from machkit.services.base_request import BaseRequest, CURRENT_YUEYING_USER_URI, YUEYING_LOGIN_URI, SEARCH_EMPLOYEE, \
     SEARCH_GUC_COMPANY_USER, SEARCH_PROJECT_USER, SEARCH_COMPANY_USER
 
 
 class UserService:
 
     def login(self, account, password):
         body = {'account': account, 'password': password}
```

### Comparing `machkit-0.1.0/datappkit/utils/file_utils.py` & `machkit-0.1.1/machkit/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `machkit-0.1.0/setup.py` & `machkit-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 requirements = load_requirements("requirements.txt")
 test_requirements = load_requirements("requirements-dev.txt")
 
 
 setup(
     name="machkit",
     description="mach team kit wrapper library",
-    version="0.1.0",
+    version="0.1.1",
     author="datapp",
     author_email="baojiarui@megvii.com",
     url="https://git-core.megvii-inc.com/transformer/yueying/data-service-sdk",
     packages=find_packages(exclude=("tests")),
     classifiers=[
         "License :: Other/Proprietary License",
     ],
```

### Comparing `machkit-0.1.0/tests/test_batch.py` & `machkit-0.1.1/tests/test_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 sys.path.append("/Users/garry/PycharmProjects/data-service-sdk")
 
-from datappkit.common import config
-from datappkit.datapp import Datapp
+from machkit.common import config
+from machkit.machkit import Datapp
 
 def create_configs_data():
     return {
         'batch_ids': [1421, 1420],
         'task_config': {
             'attr_config': [
                 {
```

### Comparing `machkit-0.1.0/tests/test_label.py` & `machkit-0.1.1/tests/test_label.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import sys
 sys.path.append("/Users/garry/PycharmProjects/data-service-sdk")
 
-from datappkit.common import config
-from datappkit.datapp import Datapp
-
+from machkit.common import config
+from machkit.machkit import Datapp
 
 if __name__ == '__main__':
     datapp = Datapp()
     # test jwt
     # config.set_authorization('JWT eyJ0eXBlIjoiSldUIiwiYWxnIjoiUlMyNTYifQ.eyJ1c2VyX2lkIjozNywiaWF0IjoxNjQ5MjE1MjU0LCJleHBpcmVfYXQiOjE2NjczNTkyNTQsImRvbWFpbiI6Im1lZ3l1ZXlpbmcuY29tIiwicGxhdGZvcm1faWQiOjIxfQ.fQXfDbwvpg4N8U_2xoZaLKasi_zmH6uMvSILsEyhhz32tj5mxtlsJvueHZ5fYWbKT5OozLDEe-lHUEUsde8U8iE6nfL1XBFM4HvCbjDskFJt-G6yC2AgV6XEYZAMsOne9ni9kVlKwIG9_mqm1oiv0wE-LLhm732ySYfTf7s9DiDLEV-TLOjLPIkGYKHUN-Oi1XiLOf_gkNlGy4DVWLCh4CRsLZngD5ysz9ZkHj1cE8hqvk1IphwJ4D9a7H_nharumisS2SI4nVpQDr8Za_goIZmJ6KED3oS9WlX3cQPweQ0oX5oSFIyIEd7VVDcusoMp0ykFZYUjH9R_GbLQKaSYoA')
     # config.set_authorization('JWT eyJhbGciOiJSUzI1NiIsInR5cGUiOiJKV1QifQ.eyJ1c2VyX2lkIjoxOCwiaWF0IjoxNjQ5NDE2MjQ4LCJleHBpcmVfYXQiOjE2Njc1NjAyNDgsImRvbWFpbiI6Im1lZ3l1ZXlpbmcuY29tIiwicGxhdGZvcm1faWQiOjIxfQ.uUnPaEO4OLg83GxKSP3kJYyN-pmp_WGsd7lCA5RBo9N7rsB1tnrtoiC5fTfuAp2lrhT6DtYBZxuAfdDheUK6UOACZSXhENDosGhATGd-Su82xWG8bBBi0xjlIRJDaXtL_0TiTUuwwl9VGTz9hLm16t_WDexvFv2rWmwG-9NHWWvUANBGEl4nBVMfkI0APvhyD7kHemOh9rvb7IWFgRcevBF9CoS9qqahmuN7JELmgBMB8KLHo_LFz40Fnl8BnzNvFu_eM5aRPVRVKu9Nhzk7irQd2xsQQglZwYxKFrBbXsQnmOIaNqW39ddknW8x-pqJskfDuzVl6jnMj0Ar-JXvbw')
```

### Comparing `machkit-0.1.0/tests/test_requirement.py` & `machkit-0.1.1/tests/test_requirement.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import sys
+import sys,os
 sys.path.append("/Users/garry/PycharmProjects/data-service-sdk")
-
-from datappkit.common import config
-from datappkit.datapp import Datapp
-
+data_serice_sdk = os.path.abspath(".")
+sys.path.append(data_serice_sdk)
+os.environ.setdefault("HOME",data_serice_sdk)
+from machkit.common import config
+from machkit.machkit import Datapp
 
 def create():
     """
     test 创建需求
     """
     body = {
         "name": "sdk_test_0720a",
@@ -65,19 +66,19 @@
 if __name__ == '__main__':
     datapp = Datapp()
     # test jwt
     # config.set_authorization('JWT eyJ0eXBlIjoiSldUIiwiYWxnIjoiUlMyNTYifQ.eyJ1c2VyX2lkIjozNywiaWF0IjoxNjQ5MjE1MjU0LCJleHBpcmVfYXQiOjE2NjczNTkyNTQsImRvbWFpbiI6Im1lZ3l1ZXlpbmcuY29tIiwicGxhdGZvcm1faWQiOjIxfQ.fQXfDbwvpg4N8U_2xoZaLKasi_zmH6uMvSILsEyhhz32tj5mxtlsJvueHZ5fYWbKT5OozLDEe-lHUEUsde8U8iE6nfL1XBFM4HvCbjDskFJt-G6yC2AgV6XEYZAMsOne9ni9kVlKwIG9_mqm1oiv0wE-LLhm732ySYfTf7s9DiDLEV-TLOjLPIkGYKHUN-Oi1XiLOf_gkNlGy4DVWLCh4CRsLZngD5ysz9ZkHj1cE8hqvk1IphwJ4D9a7H_nharumisS2SI4nVpQDr8Za_goIZmJ6KED3oS9WlX3cQPweQ0oX5oSFIyIEd7VVDcusoMp0ykFZYUjH9R_GbLQKaSYoA')
     # datapp.login("13333330003", "test123")
 
     # 创建需求
-    create()
+    # create()
 
     # 获取需求详情
     # res, data = datapp.get_requirement(1079)
     # print(res, data)
 
     # 修改需求
     # patch()
 
     # 获取需求list
-    # res, data = datapp.get_requirements(1, 1)
-    # print(res, data)
+    res, data = datapp.get_requirements(1, 10)
+    print(res, data)
```

### Comparing `machkit-0.1.0/tests/test_token.py` & `machkit-0.1.1/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `machkit-0.1.0/tests/test_user.py` & `machkit-0.1.1/tests/test_user.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import sys
 sys.path.append("/Users/garry/PycharmProjects/data-service-sdk")
 
-from datappkit.common import config
-from datappkit.datapp import Datapp
-
+from machkit.common import config
+from machkit.machkit import Datapp
 
 if __name__ == '__main__':
     datapp = Datapp()
     # test jwt
     # config.set_authorization('JWT eyJ0eXBlIjoiSldUIiwiYWxnIjoiUlMyNTYifQ.eyJ1c2VyX2lkIjozNywiaWF0IjoxNjQ5MjE1MjU0LCJleHBpcmVfYXQiOjE2NjczNTkyNTQsImRvbWFpbiI6Im1lZ3l1ZXlpbmcuY29tIiwicGxhdGZvcm1faWQiOjIxfQ.fQXfDbwvpg4N8U_2xoZaLKasi_zmH6uMvSILsEyhhz32tj5mxtlsJvueHZ5fYWbKT5OozLDEe-lHUEUsde8U8iE6nfL1XBFM4HvCbjDskFJt-G6yC2AgV6XEYZAMsOne9ni9kVlKwIG9_mqm1oiv0wE-LLhm732ySYfTf7s9DiDLEV-TLOjLPIkGYKHUN-Oi1XiLOf_gkNlGy4DVWLCh4CRsLZngD5ysz9ZkHj1cE8hqvk1IphwJ4D9a7H_nharumisS2SI4nVpQDr8Za_goIZmJ6KED3oS9WlX3cQPweQ0oX5oSFIyIEd7VVDcusoMp0ykFZYUjH9R_GbLQKaSYoA')
     # config.set_authorization('JWT eyJhbGciOiJSUzI1NiIsInR5cGUiOiJKV1QifQ.eyJ1c2VyX2lkIjoxOCwiaWF0IjoxNjQ5NDE2MjQ4LCJleHBpcmVfYXQiOjE2Njc1NjAyNDgsImRvbWFpbiI6Im1lZ3l1ZXlpbmcuY29tIiwicGxhdGZvcm1faWQiOjIxfQ.uUnPaEO4OLg83GxKSP3kJYyN-pmp_WGsd7lCA5RBo9N7rsB1tnrtoiC5fTfuAp2lrhT6DtYBZxuAfdDheUK6UOACZSXhENDosGhATGd-Su82xWG8bBBi0xjlIRJDaXtL_0TiTUuwwl9VGTz9hLm16t_WDexvFv2rWmwG-9NHWWvUANBGEl4nBVMfkI0APvhyD7kHemOh9rvb7IWFgRcevBF9CoS9qqahmuN7JELmgBMB8KLHo_LFz40Fnl8BnzNvFu_eM5aRPVRVKu9Nhzk7irQd2xsQQglZwYxKFrBbXsQnmOIaNqW39ddknW8x-pqJskfDuzVl6jnMj0Ar-JXvbw')
```

