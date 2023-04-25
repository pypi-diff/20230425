# Comparing `tmp/alicebot_adapter_mirai-0.6.0.post2.tar.gz` & `tmp/alicebot_adapter_mirai-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicebot_adapter_mirai-0.6.0.post2.tar", max compression
+gzip compressed data, was "alicebot_adapter_mirai-0.6.2.tar", max compression
```

## Comparing `alicebot_adapter_mirai-0.6.0.post2.tar` & `alicebot_adapter_mirai-0.6.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34522 2021-08-21 10:41:03.751593 alicebot_adapter_mirai-0.6.0.post2/LICENSE
--rw-r--r--   0        0        0      249 2022-08-21 12:26:07.263645 alicebot_adapter_mirai-0.6.0.post2/README.md
--rw-r--r--   0        0        0     8997 2023-03-02 13:46:00.613797 alicebot_adapter_mirai-0.6.0.post2/alicebot/adapter/mirai/__init__.py
--rw-r--r--   0        0        0     1032 2022-11-24 16:03:49.202552 alicebot_adapter_mirai-0.6.0.post2/alicebot/adapter/mirai/config.py
--rw-r--r--   0        0        0      660 2022-06-01 07:07:36.279865 alicebot_adapter_mirai-0.6.0.post2/alicebot/adapter/mirai/event/__init__.py
--rw-r--r--   0        0        0      902 2022-06-01 07:07:36.293099 alicebot_adapter_mirai-0.6.0.post2/alicebot/adapter/mirai/event/base.py
--rw-r--r--   0        0        0     1042 2022-06-01 07:07:36.298178 alicebot_adapter_mirai-0.6.0.post2/alicebot/adapter/mirai/event/mate.py
--rw-r--r--   0        0        0     3586 2022-06-01 07:07:36.333284 alicebot_adapter_mirai-0.6.0.post2/alicebot/adapter/mirai/event/message.py
--rw-r--r--   0        0        0     5392 2022-06-01 07:07:36.354929 alicebot_adapter_mirai-0.6.0.post2/alicebot/adapter/mirai/event/notice.py
--rw-r--r--   0        0        0     4264 2022-06-01 07:07:36.336702 alicebot_adapter_mirai-0.6.0.post2/alicebot/adapter/mirai/event/request.py
--rw-r--r--   0        0        0      596 2022-06-01 07:13:07.979393 alicebot_adapter_mirai-0.6.0.post2/alicebot/adapter/mirai/exceptions.py
--rw-r--r--   0        0        0     4391 2023-03-02 13:51:48.216073 alicebot_adapter_mirai-0.6.0.post2/alicebot/adapter/mirai/message.py
--rw-r--r--   0        0        0     1344 2023-03-02 13:57:26.549524 alicebot_adapter_mirai-0.6.0.post2/pyproject.toml
--rw-r--r--   0        0        0     1438 1970-01-01 00:00:00.000000 alicebot_adapter_mirai-0.6.0.post2/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/LICENSE
+-rw-r--r--   0        0        0      258 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/README.md
+-rw-r--r--   0        0        0     9718 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/__init__.py
+-rw-r--r--   0        0        0     1032 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/config.py
+-rw-r--r--   0        0        0      119 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/__init__.py
+-rw-r--r--   0        0        0      825 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/base.py
+-rw-r--r--   0        0        0     1042 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/mate.py
+-rw-r--r--   0        0        0     3650 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/message.py
+-rw-r--r--   0        0        0     5492 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/notice.py
+-rw-r--r--   0        0        0     4264 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/request.py
+-rw-r--r--   0        0        0      647 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/exceptions.py
+-rw-r--r--   0        0        0     4425 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/message.py
+-rw-r--r--   0        0        0     1341 2023-04-25 11:14:36.281730 alicebot_adapter_mirai-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1443 1970-01-01 00:00:00.000000 alicebot_adapter_mirai-0.6.2/PKG-INFO
```

### Comparing `alicebot_adapter_mirai-0.6.0.post2/LICENSE` & `alicebot_adapter_mirai-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_mirai-0.6.0.post2/alicebot/adapter/mirai/__init__.py` & `alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,55 +4,67 @@
 本适配器支持 mirai-api-http 的 Websocket Adapter 模式和 Reverse Websocket Adapter 模式。
 协议详情请参考: [mirai-api-http](https://github.com/project-mirai/mirai-api-http) 。
 """
 import sys
 import json
 import time
 import asyncio
+import inspect
 from functools import partial
-from typing import TYPE_CHECKING, Any, Dict, Literal, Optional
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    Type,
+    Literal,
+    Callable,
+    ClassVar,
+    Optional,
+    Awaitable,
+)
 
 import aiohttp
 
 from alicebot.utils import DataclassEncoder
 from alicebot.adapter.utils import WebSocketAdapter
 from alicebot.log import logger, error_or_exception
 
+from . import event
 from .config import Config
 from .message import MiraiMessage
 from .exceptions import ApiTimeout, ActionFailed, NetworkError
-from .event import (
-    BotEvent,
-    MateEvent,
-    MiraiEvent,
-    CommandExecutedEvent,
-    get_event_class,
-)
+from .event import BotEvent, MateEvent, MiraiEvent, CommandExecutedEvent
 
 if TYPE_CHECKING:
     from .message import T_MiraiMSG
 
 __all__ = ["MiraiAdapter"]
 
 
 class MiraiAdapter(WebSocketAdapter[MiraiEvent, Config]):
     """Mirai 协议适配器。
 
-    在插件中可以直接使用 `self.adapter.xxx_api(**params)` 调用名称为 `xxx_api` 的 API，
+    在插件中可以直接使用 `self.adapter.xxx_api(**params)` 调用名称为 `xxx_api` 的 API ，
     和调用 `call_api()` 方法相同。
     """
 
     name: str = "mirai"
     Config = Config
 
-    _api_response: Any
-    _api_response_cond: asyncio.Condition = None
+    event_models: ClassVar[Dict[str, Type[MiraiEvent]]] = {
+        name: model
+        for name, model in inspect.getmembers(event, inspect.isclass)
+        if issubclass(model, MiraiEvent)
+    }
+
+    _api_response: Dict[str, Any]
+    _api_response_cond: asyncio.Condition
     _sync_id: int = 0
 
-    def __getattr__(self, item):
+    def __getattr__(self, item: str) -> Callable[..., Awaitable[Any]]:
         return partial(self.call_api, item)
 
     async def startup(self):
         """初始化适配器。"""
         self.adapter_type = self.config.adapter_type
         self.host = self.config.host
         self.port = self.config.port
@@ -64,23 +76,25 @@
     async def reverse_ws_connection_hook(self):
         """反向 WebSocket 连接建立时的钩子函数。"""
         logger.info(f"WebSocket connected!")
         asyncio.create_task(self.verify_identity())
 
     async def websocket_connect(self):
         """创建正向 WebSocket 连接。"""
+        assert self.session is not None
         logger.info("Trying to verify identity and create connection...")
         async with self.session.ws_connect(
             f"ws://{self.host}:{self.port}/all?"
             f"verifyKey={self.config.verify_key}&qq={self.config.qq}"
         ) as self.websocket:
             await self.handle_websocket()
 
     async def handle_websocket_msg(self, msg: aiohttp.WSMessage):
         """处理 WebSocket 消息。"""
+        assert self.websocket is not None
         if msg.type == aiohttp.WSMsgType.TEXT:
             try:
                 msg_dict = msg.json()
             except json.JSONDecodeError as e:
                 error_or_exception(
                     "WebSocket message parsing error, not json:",
                     e,
@@ -113,21 +127,33 @@
                 f"with exception {self.websocket.exception()!r}"
             )
 
     def _get_sync_id(self) -> int:
         self._sync_id = (self._sync_id + 1) % sys.maxsize
         return self._sync_id
 
+    @classmethod
+    def get_event_model(cls, event_type: str) -> Type[MiraiEvent]:
+        """根据接收到的消息类型返回对应的事件类。
+
+        Args:
+            event_type: 事件类型。
+
+        Returns:
+            对应的事件类。
+        """
+        return cls.event_models[event_type]
+
     async def handle_mirai_event(self, msg: Dict[str, Any]):
         """处理 Mirai 事件。
 
         Args:
             msg: 接收到的信息。
         """
-        mirai_event = get_event_class(msg.get("type"))(adapter=self, **msg)
+        mirai_event = self.get_event_model(msg["type"])(adapter=self, **msg)
 
         if isinstance(mirai_event, MateEvent):
             # meta_event 不交由插件处理
             if isinstance(mirai_event, BotEvent):
                 logger.info(f"Bot {mirai_event.qq}: {mirai_event.type}")
             elif isinstance(mirai_event, CommandExecutedEvent):
                 logger.info(
@@ -153,31 +179,32 @@
             except ActionFailed as e:
                 logger.warning(f"Verify failed with code {e.code}, retrying...")
             else:
                 logger.info("Verify success!")
                 return
 
     async def call_api(
-        self, command: str, sub_command: Optional[str] = None, **content
-    ) -> Dict[str, Any]:
-        """调用 Mirai API，协程会等待直到获得 API 响应。
+        self, command: str, sub_command: Optional[str] = None, **content: Dict[str, Any]
+    ) -> Any:
+        """调用 Mirai API ，协程会等待直到获得 API 响应。
 
         Args:
             command: 命令字。
             sub_command: 子命令字。
             **content: 请求内容。
 
         Returns:
             API 响应中的 data 字段，即 Mirai-api-http API 通用接口中的内容。
 
         Raises:
             NetworkError: 网络错误。
             ActionFailed: API 操作失败。
             ApiTimeout: API 请求响应超时。
         """
+        assert self.websocket is not None
         sync_id = str(self._get_sync_id())
         try:
             await self.websocket.send_str(
                 json.dumps(
                     {
                         "syncId": sync_id,
                         "command": command,
@@ -204,32 +231,31 @@
                     break
                 if self._api_response.get("syncId") == sync_id:
                     status_code = self._api_response.get("data", {}).get("code")
                     if status_code is not None and status_code != 0:
                         raise ActionFailed(code=status_code, resp=self._api_response)
                     return self._api_response.get("data")
 
-        if not self.bot.should_exit.is_set():
-            raise ApiTimeout
+        raise ApiTimeout
 
     async def send(
         self,
         message_: "T_MiraiMSG",
         message_type: Literal["private", "friend", "group"],
         target: int,
-        quote: int = None,
+        quote: Optional[int] = None,
     ) -> Any:
         """调用 Mirai API 发送消息。
 
         Args:
             message_: 消息内容，可以是 str, Mapping, Iterable[Mapping],
                 'MiraiMessageSegment', 'MiraiMessage'。
                 将使用 `MiraiMessage` 进行封装。
             message_type: 消息类型。应该是 private, friend 或者 group。其中 private 和 friend 相同。
-            target: 发送对象的 ID ，QQ 号码或者群号码。
+            target: 发送对象的 ID ， QQ 号码或者群号码。
             quote: 引用的消息的 messageId。默认为 `None` ，不引用任何消息。
 
         Returns:
             API 响应。
 
         Raises:
             TypeError: message_type 非法。
```

### Comparing `alicebot_adapter_mirai-0.6.0.post2/alicebot/adapter/mirai/config.py` & `alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/config.py`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_mirai-0.6.0.post2/alicebot/adapter/mirai/event/base.py` & `alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from typing import TYPE_CHECKING, Literal, TypeVar
+from typing import TYPE_CHECKING, Literal
 
 from pydantic import BaseModel
 
 from alicebot.event import Event
 
 if TYPE_CHECKING:
-    from .. import MiraiAdapter  # noqa
-
-T_MiraiEvent = TypeVar("T_MiraiEvent", bound="MiraiEvent")
+    from .. import MiraiAdapter
 
 Permission = Literal["OWNER", "ADMINISTRATOR", "MEMBER"]
 
 
 class Subject(BaseModel):
     id: int
     kind: Literal["Friend", "Group"]
```

### Comparing `alicebot_adapter_mirai-0.6.0.post2/alicebot/adapter/mirai/event/mate.py` & `alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/mate.py`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_mirai-0.6.0.post2/alicebot/adapter/mirai/event/message.py` & `alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/message.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     async def reply(self, msg: "T_MiraiMSG", quote: bool = False) -> Dict[str, Any]:
         if quote:
             return await self.adapter.send(
                 msg,
                 message_type="friend",
                 target=self.sender.id,
-                quote=self.messageChain[0].id,
+                quote=self.messageChain[0].id,  # type: ignore
             )
         else:
             return await self.adapter.send(
                 msg, message_type="friend", target=self.sender.id
             )
 
 
@@ -67,15 +67,15 @@
 
     async def reply(self, msg: "T_MiraiMSG", quote: bool = False) -> Dict[str, Any]:
         if quote:
             return await self.adapter.send(
                 msg,
                 message_type="group",
                 target=self.sender.group.id,
-                quote=self.messageChain[0].id,
+                quote=self.messageChain[0].id,  # type: ignore
             )
         else:
             return await self.adapter.send(
                 msg, message_type="group", target=self.sender.group.id
             )
 
 
@@ -87,15 +87,15 @@
 
     async def reply(self, msg: "T_MiraiMSG", quote: bool = False) -> Dict[str, Any]:
         if quote:
             return await self.adapter.sendTempMessage(
                 qq=self.sender.id,
                 group=self.sender.group.id,
                 messageChain=msg,
-                quote=self.messageChain[0].id,
+                quote=self.messageChain[0].id,  # type: ignore
             )
         else:
             return await self.adapter.sendTempMessage(
                 qq=self.sender.id, group=self.sender.group.id, messageChain=msg
             )
 
 
@@ -107,15 +107,15 @@
 
     async def reply(self, msg: "T_MiraiMSG", quote: bool = False) -> Dict[str, Any]:
         if quote:
             return await self.adapter.send(
                 msg,
                 message_type="friend",
                 target=self.sender.id,
-                quote=self.messageChain[0].id,
+                quote=self.messageChain[0].id,  # type: ignore
             )
         else:
             return await self.adapter.send(
                 msg, message_type="friend", target=self.sender.id
             )
```

### Comparing `alicebot_adapter_mirai-0.6.0.post2/alicebot/adapter/mirai/event/notice.py` & `alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/notice.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal
+from typing import Literal, Optional
 
 from pydantic import create_model
 
 from .base import (
     Subject,
     GroupInfo,
     FriendInfo,
@@ -123,55 +123,55 @@
     """群消息撤回"""
 
     type: Literal["GroupRecallEvent"]
     authorId: int
     messageId: int
     time: int
     group: GroupInfo
-    operator: GroupMemberInfo
+    operator: Optional[GroupMemberInfo]
 
 
 class GroupNameChangeEvent(GroupNoticeEvent):
     """某个群名改变"""
 
     type: Literal["GroupNameChangeEvent"]
     origin: str
     current: str
     group: GroupInfo
-    operator: GroupMemberInfo
+    operator: Optional[GroupMemberInfo]
 
 
 class GroupEntranceAnnouncementChangeEvent(GroupNoticeEvent):
     """某群入群公告改变"""
 
     type: Literal["GroupEntranceAnnouncementChangeEvent"]
     origin: str
     current: str
     group: GroupInfo
-    operator: GroupMemberInfo
+    operator: Optional[GroupMemberInfo]
 
 
 class GroupMuteAllEvent(GroupNoticeEvent):
     """全员禁言"""
 
     type: Literal["GroupMuteAllEvent"]
     origin: bool
     current: bool
     group: GroupInfo
-    operator: GroupMemberInfo
+    operator: Optional[GroupMemberInfo]
 
 
 class GroupAllowAnonymousChatEvent(GroupNoticeEvent):
     """匿名聊天"""
 
     type: Literal["GroupAllowAnonymousChatEvent"]
     origin: bool
     current: bool
     group: GroupInfo
-    operator: GroupMemberInfo
+    operator: Optional[GroupMemberInfo]
 
 
 class GroupAllowConfessTalkEvent(GroupNoticeEvent):
     """坦白说"""
 
     type: Literal["GroupAllowAnonymousChatEvent"]
     origin: bool
@@ -183,15 +183,15 @@
 class GroupAllowMemberInviteEvent(GroupNoticeEvent):
     """允许群员邀请好友加群"""
 
     type: Literal["GroupAllowMemberInviteEvent"]
     origin: bool
     current: bool
     group: GroupInfo
-    operator: GroupMemberInfo
+    operator: Optional[GroupMemberInfo]
 
 
 class GroupMemberEvent(GroupEvent):
     """群成员相关事件"""
 
     member: GroupMemberInfo
 
@@ -202,15 +202,15 @@
     type: Literal["MemberJoinEvent"]
 
 
 class MemberLeaveEventKick(GroupMemberEvent):
     """成员被踢出群（该成员不是Bot）"""
 
     type: Literal["MemberLeaveEventKick"]
-    operator: GroupMemberInfo
+    operator: Optional[GroupMemberInfo]
 
 
 class MemberLeaveEventQuit(GroupMemberEvent):
     """成员主动离群（该成员不是Bot）"""
 
     type: Literal["MemberLeaveEventQuit"]
 
@@ -240,22 +240,22 @@
 
 
 class MemberMuteEvent(GroupMemberEvent):
     """群成员被禁言事件（该成员不是Bot）"""
 
     type: Literal["MemberMuteEvent"]
     durationSeconds: int
-    operator: GroupMemberInfo
+    operator: Optional[GroupMemberInfo]
 
 
 class MemberUnmuteEvent(GroupMemberEvent):
     """群成员被取消禁言事件（该成员不是Bot）"""
 
     type: Literal["MemberUnmuteEvent"]
-    operator: GroupMemberInfo
+    operator: Optional[GroupMemberInfo]
 
 
 class MemberHonorChangeEvent(GroupMemberEvent):
     """群员称号改变"""
 
     type: Literal["MemberHonorChangeEvent"]
     action: Literal["achieve", "lose"]
```

### Comparing `alicebot_adapter_mirai-0.6.0.post2/alicebot/adapter/mirai/event/request.py` & `alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/event/request.py`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_mirai-0.6.0.post2/alicebot/adapter/mirai/message.py` & `alicebot_adapter_mirai-0.6.2/alicebot/adapter/mirai/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 
 from alicebot.utils import DataclassEncoder
 from alicebot.message import Message, MessageSegment
 
 __all__ = ["T_MiraiMSG", "MiraiMessage", "MiraiMessageSegment"]
 
 T_MiraiMSG = Union[
-    str, Mapping, Iterable[Mapping], "MiraiMessageSegment", "MiraiMessage"
+    str,
+    Mapping[str, Any],
+    Iterable[Mapping[str, Any]],
+    "MiraiMessageSegment",
+    "MiraiMessage",
 ]
 
 
 class MiraiMessage(Message["MiraiMessageSegment"]):
     @property
     def _message_segment_class(self) -> Type["MiraiMessageSegment"]:
         return MiraiMessageSegment
@@ -26,15 +30,15 @@
         Returns:
             messageChain 数组。
         """
         return list(map(lambda x: x.as_dict(), self))
 
 
 class MiraiMessageSegment(MessageSegment["MiraiMessage"]):
-    def __init__(self, type: str, **data):  # noqa
+    def __init__(self, type: str, **data: Any):
         super().__init__(
             type=type, data={k: v for k, v in data.items() if v is not None}
         )
 
     @property
     def _message_class(self) -> Type["MiraiMessage"]:
         return MiraiMessage
```

### Comparing `alicebot_adapter_mirai-0.6.0.post2/pyproject.toml` & `alicebot_adapter_mirai-0.6.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 [tool.poetry]
 name = "alicebot-adapter-mirai"
-version = "0.6.0.post2"
+version = "0.6.2"
 description = "Mirai adapter for AliceBot."
 license = "AGPL-3.0-or-later"
 authors = ["st1020 <stone_1020@qq.com>"]
 readme = "README.md"
 homepage = "https://docs.alicebot.dev/"
-repository = "https://github.com/st1020/alicebot"
+repository = "https://github.com/AliceBotProject/alicebot"
 documentation = "https://docs.alicebot.dev/"
 keywords = ["bot", "chatbot", "qq", "qqbot", "mirai"]
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

### Comparing `alicebot_adapter_mirai-0.6.0.post2/PKG-INFO` & `alicebot_adapter_mirai-0.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alicebot-adapter-mirai
-Version: 0.6.0.post2
+Version: 0.6.2
 Summary: Mirai adapter for AliceBot.
 Home-page: https://docs.alicebot.dev/
 License: AGPL-3.0-or-later
 Keywords: bot,chatbot,qq,qqbot,mirai
 Author: st1020
 Author-email: stone_1020@qq.com
 Requires-Python: >=3.8,<4.0
@@ -18,21 +18,21 @@
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
 
 # AliceBot-Adapter-CQHTTP
 
 **Mirai 协议适配**
 
 </div>
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: alicebot-adapter-mirai Version: 0.6.0.post2
-Summary: Mirai adapter for AliceBot. Home-page: https://docs.alicebot.dev/
-License: AGPL-3.0-or-later Keywords: bot,chatbot,qq,qqbot,mirai Author: st1020
-Author-email: stone_1020@qq.com Requires-Python: >=3.8,<4.0 Classifier:
-Development Status :: 3 - Alpha Classifier: Framework :: AsyncIO Classifier:
-Framework :: Robot Framework Classifier: Framework :: Robot Framework ::
-Library Classifier: License :: OSI Approved :: GNU Affero General Public
-License v3 or later (AGPLv3+) Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
-Communications :: Chat Requires-Dist: alicebot (>=0.6.0,<0.7.0) Project-URL:
-Documentation, https://docs.alicebot.dev/ Project-URL: Repository, https://
-github.com/st1020/alicebot Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: alicebot-adapter-mirai Version: 0.6.2 Summary:
+Mirai adapter for AliceBot. Home-page: https://docs.alicebot.dev/ License:
+AGPL-3.0-or-later Keywords: bot,chatbot,qq,qqbot,mirai Author: st1020 Author-
+email: stone_1020@qq.com Requires-Python: >=3.8,<4.0 Classifier: Development
+Status :: 3 - Alpha Classifier: Framework :: AsyncIO Classifier: Framework ::
+Robot Framework Classifier: Framework :: Robot Framework :: Library Classifier:
+License :: OSI Approved :: GNU Affero General Public License v3 or later
+(AGPLv3+) Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3 Classifier: Topic :: Communications :: Chat Requires-
+Dist: alicebot (==0.6.2) Project-URL: Documentation, https://docs.alicebot.dev/
+Project-URL: Repository, https://github.com/AliceBotProject/alicebot
+Description-Content-Type: text/markdown
             [logo] # AliceBot-Adapter-CQHTTP **Mirai åè®®éé**
```

