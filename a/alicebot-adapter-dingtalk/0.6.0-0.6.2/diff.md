# Comparing `tmp/alicebot_adapter_dingtalk-0.6.0.tar.gz` & `tmp/alicebot_adapter_dingtalk-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicebot_adapter_dingtalk-0.6.0.tar", max compression
+gzip compressed data, was "alicebot_adapter_dingtalk-0.6.2.tar", max compression
```

## Comparing `alicebot_adapter_dingtalk-0.6.0.tar` & `alicebot_adapter_dingtalk-0.6.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0      251 2022-08-21 12:26:14.504649 alicebot_adapter_dingtalk-0.6.0/README.md
--rw-r--r--   0        0        0     5446 2022-11-24 16:11:40.904703 alicebot_adapter_dingtalk-0.6.0/alicebot/adapter/dingtalk/__init__.py
--rw-r--r--   0        0        0      593 2022-11-24 15:20:58.934024 alicebot_adapter_dingtalk-0.6.0/alicebot/adapter/dingtalk/config.py
--rw-r--r--   0        0        0     2366 2022-06-01 07:07:36.302562 alicebot_adapter_dingtalk-0.6.0/alicebot/adapter/dingtalk/event.py
--rw-r--r--   0        0        0      390 2022-06-01 07:10:20.339932 alicebot_adapter_dingtalk-0.6.0/alicebot/adapter/dingtalk/exceptions.py
--rw-r--r--   0        0        0     3203 2022-06-01 07:07:36.321745 alicebot_adapter_dingtalk-0.6.0/alicebot/adapter/dingtalk/message.py
--rw-r--r--   0        0        0     1318 2022-11-26 15:09:44.082092 alicebot_adapter_dingtalk-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 alicebot_adapter_dingtalk-0.6.0/setup.py
--rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 alicebot_adapter_dingtalk-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      260 2023-04-25 11:14:36.281730 alicebot_adapter_dingtalk-0.6.2/README.md
+-rw-r--r--   0        0        0     5287 2023-04-25 11:14:36.281730 alicebot_adapter_dingtalk-0.6.2/alicebot/adapter/dingtalk/__init__.py
+-rw-r--r--   0        0        0      593 2023-04-25 11:14:36.281730 alicebot_adapter_dingtalk-0.6.2/alicebot/adapter/dingtalk/config.py
+-rw-r--r--   0        0        0     2368 2023-04-25 11:14:36.281730 alicebot_adapter_dingtalk-0.6.2/alicebot/adapter/dingtalk/event.py
+-rw-r--r--   0        0        0      315 2023-04-25 11:14:36.281730 alicebot_adapter_dingtalk-0.6.2/alicebot/adapter/dingtalk/exceptions.py
+-rw-r--r--   0        0        0     3197 2023-04-25 11:14:36.281730 alicebot_adapter_dingtalk-0.6.2/alicebot/adapter/dingtalk/message.py
+-rw-r--r--   0        0        0     1321 2023-04-25 11:14:36.281730 alicebot_adapter_dingtalk-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1336 1970-01-01 00:00:00.000000 alicebot_adapter_dingtalk-0.6.2/PKG-INFO
```

### Comparing `alicebot_adapter_dingtalk-0.6.0/alicebot/adapter/dingtalk/__init__.py` & `alicebot_adapter_dingtalk-0.6.2/alicebot/adapter/dingtalk/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 from aiohttp import web
 
 from alicebot.adapter import Adapter
 from alicebot.log import logger, error_or_exception
 
 from .config import Config
 from .event import DingTalkEvent
+from .exceptions import NetworkError
 from .message import DingTalkMessage
-from .exceptions import ApiTimeout, NetworkError
 
 __all__ = ["DingTalkAdapter"]
 
 
 class DingTalkAdapter(Adapter[DingTalkEvent, Config]):
     """钉钉协议适配器。"""
 
     name: str = "dingtalk"
     Config = Config
 
-    app: web.Application = None
-    runner: web.AppRunner = None
-    site: web.TCPSite = None
+    app: web.Application
+    runner: web.AppRunner
+    site: web.TCPSite
 
-    session: aiohttp.ClientSession = None
+    session: aiohttp.ClientSession
 
     async def startup(self):
         """创建 aiohttp Application。"""
         self.app = web.Application()
         self.app.add_routes([web.post(self.config.url, self.handler)])
 
         self.session = aiohttp.ClientSession()
@@ -47,20 +47,17 @@
         self.runner = web.AppRunner(self.app)
         await self.runner.setup()
         self.site = web.TCPSite(self.runner, self.config.host, self.config.port)
         await self.site.start()
 
     async def shutdown(self):
         """清理 aiohttp AppRunner。"""
-        if self.session is not None:
-            await self.session.close()
-        if self.site is not None:
-            await self.site.stop()
-        if self.runner is not None:
-            await self.runner.cleanup()
+        await self.session.close()
+        await self.site.stop()
+        await self.runner.cleanup()
 
     async def handler(self, request: web.Request):
         """处理 aiohttp 服务器的接收。
 
         Args:
             request: aiohttp 服务器的 Request 对象。
         """
```

### Comparing `alicebot_adapter_dingtalk-0.6.0/alicebot/adapter/dingtalk/config.py` & `alicebot_adapter_dingtalk-0.6.2/alicebot/adapter/dingtalk/config.py`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_dingtalk-0.6.0/alicebot/adapter/dingtalk/event.py` & `alicebot_adapter_dingtalk-0.6.2/alicebot/adapter/dingtalk/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from alicebot.event import Event
 
 from .message import DingTalkMessage
 from .exceptions import WebhookExpiredError
 
 if TYPE_CHECKING:
-    from . import DingTalkAdapter  # noqa
+    from . import DingTalkAdapter
 
 
 class UserInfo(BaseModel):
     dingtalkId: str
     staffId: Optional[str]
 
 
@@ -47,27 +47,27 @@
     text: Text
 
     message: Optional[DingTalkMessage]
     response_msg: Union[None, str, Dict, DingTalkMessage] = None
     response_at: Union[None, Dict, DingTalkMessage] = None
 
     @validator("message", always=True)
-    def set_ts_now(cls, v, values, **kwargs):  # noqa
+    def set_message(cls, v, values, **kwargs):  # type: ignore
         return DingTalkMessage.text(values["text"].content)
 
     async def reply(
         self,
         msg: Union[str, Dict, DingTalkMessage],
         at: Union[None, Dict, DingTalkMessage] = None,
     ) -> Dict[str, Any]:
         """回复消息。
 
         Args:
             msg: 回复消息的内容，可以是 str, Dict 或 DingTalkMessage。
-            at: 回复消息时 At 的对象，必须时 at 类型的 DingTalkMessage，或者符合标准的 Dict。
+            at: 回复消息时 At 的对象，必须时 at 类型的 DingTalkMessage ，或者符合标准的 Dict。
 
         Returns:
             调用 Webhook 地址后钉钉服务器的响应。
 
         Raises:
             WebhookExpiredError: 当前事件的 Webhook 地址已经过期。
             ...: 同 `DingTalkAdapter.send()` 方法。
```

### Comparing `alicebot_adapter_dingtalk-0.6.0/alicebot/adapter/dingtalk/message.py` & `alicebot_adapter_dingtalk-0.6.2/alicebot/adapter/dingtalk/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, List, Optional
 
 from alicebot.message import MessageSegment
 
 __all__ = ["DingTalkMessage"]
 
 
-class DingTalkMessage(MessageSegment[None]):
+class DingTalkMessage(MessageSegment):
     """DingTalk 消息"""
 
     @property
     def _message_class(self) -> None:
         return None
 
     def __str__(self):
```

### Comparing `alicebot_adapter_dingtalk-0.6.0/pyproject.toml` & `alicebot_adapter_dingtalk-0.6.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 [tool.poetry]
 name = "alicebot-adapter-dingtalk"
-version = "0.6.0"
+version = "0.6.2"
 description = "DingTalk adapter for AliceBot."
 license = "MIT"
 authors = ["st1020 <stone_1020@qq.com>"]
 readme = "README.md"
 homepage = "https://docs.alicebot.dev/"
-repository = "https://github.com/st1020/alicebot"
+repository = "https://github.com/AliceBotProject/alicebot"
 documentation = "https://docs.alicebot.dev/"
 keywords = ["bot", "chatbot", "dingtalk"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: AsyncIO",
     "Framework :: Robot Framework",
     "Framework :: Robot Framework :: Library",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Topic :: Communications :: Chat"
-]
-packages = [
-    { include = "alicebot" }
+    "Topic :: Communications :: Chat",
 ]
+packages = [{ include = "alicebot" }]
 exclude = ["alicebot/__init__.py", "alicebot/adapter/__init__.py"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-alicebot = "^0.6.0"
+alicebot = "0.6.2"
 
 [tool.poetry.dev-dependencies]
 alicebot = { path = "../../", develop = true }
 
 [tool.pydantic-pycharm-plugin]
 ignore-init-method-arguments = true
```

### Comparing `alicebot_adapter_dingtalk-0.6.0/PKG-INFO` & `alicebot_adapter_dingtalk-0.6.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alicebot-adapter-dingtalk
-Version: 0.6.0
+Version: 0.6.2
 Summary: DingTalk adapter for AliceBot.
 Home-page: https://docs.alicebot.dev/
 License: MIT
 Keywords: bot,chatbot,dingtalk
 Author: st1020
 Author-email: stone_1020@qq.com
 Requires-Python: >=3.8,<4.0
@@ -17,21 +17,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Communications :: Chat
-Requires-Dist: alicebot (>=0.6.0,<0.7.0)
+Requires-Dist: alicebot (==0.6.2)
 Project-URL: Documentation, https://docs.alicebot.dev/
-Project-URL: Repository, https://github.com/st1020/alicebot
+Project-URL: Repository, https://github.com/AliceBotProject/alicebot
 Description-Content-Type: text/markdown
 
 <div align="center">
-  <a href="https://docs.alicebot.dev/"><img src="https://raw.githubusercontent.com/st1020/alicebot/master/docs/public/logo.png" width="200" height="200" alt="logo"></a>
+  <a href="https://docs.alicebot.dev/"><img src="https://raw.githubusercontent.com/AliceBotProject/alicebot/master/docs/public/logo.png" width="200" height="200" alt="logo"></a>
 
 # AliceBot-Adapter-DingTalk
 
 **钉钉协议适配**
 
 </div>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: alicebot-adapter-dingtalk Version: 0.6.0 Summary:
+Metadata-Version: 2.1 Name: alicebot-adapter-dingtalk Version: 0.6.2 Summary:
 DingTalk adapter for AliceBot. Home-page: https://docs.alicebot.dev/ License:
 MIT Keywords: bot,chatbot,dingtalk Author: st1020 Author-email:
 stone_1020@qq.com Requires-Python: >=3.8,<4.0 Classifier: Development Status ::
 3 - Alpha Classifier: Framework :: AsyncIO Classifier: Framework :: Robot
 Framework Classifier: Framework :: Robot Framework :: Library Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3 Classifier: Topic :: Communications :: Chat Requires-Dist: alicebot
-(>=0.6.0,<0.7.0) Project-URL: Documentation, https://docs.alicebot.dev/
-Project-URL: Repository, https://github.com/st1020/alicebot Description-
-Content-Type: text/markdown
+(==0.6.2) Project-URL: Documentation, https://docs.alicebot.dev/ Project-URL:
+Repository, https://github.com/AliceBotProject/alicebot Description-Content-
+Type: text/markdown
            [logo] # AliceBot-Adapter-DingTalk **ééåè®®éé**
```

