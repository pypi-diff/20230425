# Comparing `tmp/alicebot_adapter_cqhttp-0.6.0.post1.tar.gz` & `tmp/alicebot_adapter_cqhttp-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicebot_adapter_cqhttp-0.6.0.post1.tar", max compression
+gzip compressed data, was "alicebot_adapter_cqhttp-0.6.2.tar", max compression
```

## Comparing `alicebot_adapter_cqhttp-0.6.0.post1.tar` & `alicebot_adapter_cqhttp-0.6.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      258 2022-08-21 12:25:59.358786 alicebot_adapter_cqhttp-0.6.0.post1/README.md
--rw-r--r--   0        0        0     7713 2023-03-02 13:45:49.447761 alicebot_adapter_cqhttp-0.6.0.post1/alicebot/adapter/cqhttp/__init__.py
--rw-r--r--   0        0        0      875 2022-11-24 16:01:48.887631 alicebot_adapter_cqhttp-0.6.0.post1/alicebot/adapter/cqhttp/config.py
--rw-r--r--   0        0        0     8810 2022-06-01 07:07:16.887728 alicebot_adapter_cqhttp-0.6.0.post1/alicebot/adapter/cqhttp/event.py
--rw-r--r--   0        0        0      659 2022-06-01 07:08:37.244693 alicebot_adapter_cqhttp-0.6.0.post1/alicebot/adapter/cqhttp/exceptions.py
--rw-r--r--   0        0        0     7478 2022-06-01 07:07:36.379345 alicebot_adapter_cqhttp-0.6.0.post1/alicebot/adapter/cqhttp/message.py
--rw-r--r--   0        0        0     1350 2023-03-02 13:57:33.184742 alicebot_adapter_cqhttp-0.6.0.post1/pyproject.toml
--rw-r--r--   0        0        0     1355 1970-01-01 00:00:00.000000 alicebot_adapter_cqhttp-0.6.0.post1/PKG-INFO
+-rw-r--r--   0        0        0      267 2023-04-25 11:14:36.277730 alicebot_adapter_cqhttp-0.6.2/README.md
+-rw-r--r--   0        0        0     9890 2023-04-25 11:14:36.281730 alicebot_adapter_cqhttp-0.6.2/alicebot/adapter/cqhttp/__init__.py
+-rw-r--r--   0        0        0      875 2023-04-25 11:14:36.281730 alicebot_adapter_cqhttp-0.6.2/alicebot/adapter/cqhttp/config.py
+-rw-r--r--   0        0        0     9252 2023-04-25 11:14:36.281730 alicebot_adapter_cqhttp-0.6.2/alicebot/adapter/cqhttp/event.py
+-rw-r--r--   0        0        0      706 2023-04-25 11:14:36.281730 alicebot_adapter_cqhttp-0.6.2/alicebot/adapter/cqhttp/exceptions.py
+-rw-r--r--   0        0        0     7530 2023-04-25 11:14:36.281730 alicebot_adapter_cqhttp-0.6.2/alicebot/adapter/cqhttp/message.py
+-rw-r--r--   0        0        0     1347 2023-04-25 11:14:36.281730 alicebot_adapter_cqhttp-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1360 1970-01-01 00:00:00.000000 alicebot_adapter_cqhttp-0.6.2/PKG-INFO
```

### Comparing `alicebot_adapter_cqhttp-0.6.0.post1/alicebot/adapter/cqhttp/__init__.py` & `alicebot_adapter_cqhttp-0.6.2/alicebot/adapter/cqhttp/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,82 +3,111 @@
 本适配器适配了 OneBot v11 协议。
 协议详情请参考: [OneBot](https://github.com/howmanybots/onebot/blob/master/README.md) 。
 """
 import sys
 import json
 import time
 import asyncio
+import inspect
 from functools import partial
-from typing import TYPE_CHECKING, Any, Dict, Literal
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    Type,
+    Tuple,
+    Literal,
+    Callable,
+    ClassVar,
+    Optional,
+    Awaitable,
+)
 
 import aiohttp
+from aiohttp import web
 
 from alicebot.utils import DataclassEncoder
 from alicebot.adapter.utils import WebSocketAdapter
 from alicebot.log import logger, error_or_exception
 
+from . import event
 from .config import Config
 from .message import CQHTTPMessage
-from .event import CQHTTPEvent, get_event_class
 from .exceptions import ApiTimeout, ActionFailed, NetworkError, ApiNotAvailable
+from .event import MetaEvent, CQHTTPEvent, HeartbeatMetaEvent, LifecycleMetaEvent
 
 if TYPE_CHECKING:
     from .message import T_CQMSG
 
 __all__ = ["CQHTTPAdapter"]
 
+T_EventModels = Dict[
+    Tuple[Optional[str], Optional[str], Optional[str]], Type[CQHTTPEvent]
+]
+
+DEFAULT_EVENT_MODELS: T_EventModels = {}
+for _, model in inspect.getmembers(event, inspect.isclass):
+    if issubclass(model, CQHTTPEvent):
+        DEFAULT_EVENT_MODELS[model.get_event_type()] = model
+
 
 class CQHTTPAdapter(WebSocketAdapter[CQHTTPEvent, Config]):
     """CQHTTP 协议适配器。"""
 
     name = "cqhttp"
     Config = Config
 
-    _api_response: Dict[Any, Any]
-    _api_response_cond: asyncio.Condition = None
+    event_models: ClassVar[T_EventModels] = DEFAULT_EVENT_MODELS
+
+    _api_response: Dict[str, Any]
+    _api_response_cond: asyncio.Condition
     _api_id: int = 0
 
-    def __getattr__(self, item):
+    def __getattr__(self, item: str) -> Callable[..., Awaitable[Any]]:
         return partial(self.call_api, item)
 
     async def startup(self):
         """初始化适配器。"""
-        self.adapter_type = self.config.adapter_type
-        if self.adapter_type == "ws-reverse":
-            self.adapter_type = "reverse-ws"
+        adapter_type = self.config.adapter_type
+        if adapter_type == "ws-reverse":
+            adapter_type = "reverse-ws"
+        self.adapter_type = adapter_type
         self.host = self.config.host
         self.port = self.config.port
         self.url = self.config.url
         self.reconnect_interval = self.config.reconnect_interval
         self._api_response_cond = asyncio.Condition()
         await super().startup()
 
     async def reverse_ws_connection_hook(self):
         """反向 WebSocket 连接建立时的钩子函数。"""
         logger.info(f"WebSocket connected!")
         if self.config.access_token:
+            assert isinstance(self.websocket, web.WebSocketResponse)
             if (
                 self.websocket.headers.get("Authorization", "")
                 != f"Bearer {self.config.access_token}"
             ):
                 await self.websocket.close()
 
     async def websocket_connect(self):
         """创建正向 WebSocket 连接。"""
+        assert self.session is not None
         logger.info("Tying to connect to WebSocket server...")
         async with self.session.ws_connect(
             f"ws://{self.host}:{self.port}/",
             headers={"Authorization": f"Bearer {self.config.access_token}"}
             if self.config.access_token
             else None,
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
@@ -99,63 +128,103 @@
                 f"with exception {self.websocket.exception()!r}"
             )
 
     def _get_api_echo(self) -> int:
         self._api_id = (self._api_id + 1) % sys.maxsize
         return self._api_id
 
+    @classmethod
+    def add_event_model(cls, event_model: Type[CQHTTPEvent]) -> None:
+        """添加自定义事件模型，事件模型类必须继承于 `CQHTTPEvent`。
+
+        Args:
+            event_model: 事件模型类。
+        """
+        cls.event_models[event_model.get_event_type()] = event_model
+
+    @classmethod
+    def get_event_model(
+        cls,
+        post_type: Optional[str],
+        detail_type: Optional[str],
+        sub_type: Optional[str],
+    ) -> Type[CQHTTPEvent]:
+        """根据接收到的消息类型返回对应的事件类。
+
+        Args:
+            post_type: 请求类型。
+            detail_type: 事件类型。
+            sub_type: 子类型。
+
+        Returns:
+            对应的事件类。
+        """
+        return (
+            cls.event_models.get((post_type, detail_type, sub_type), None)
+            or cls.event_models.get((post_type, detail_type, None), None)
+            or cls.event_models.get((post_type, None, None), None)
+            or cls.event_models[(None, None, None)]
+        )
+
     async def handle_cqhttp_event(self, msg: Dict[str, Any]):
         """处理 CQHTTP 事件。
 
         Args:
             msg: 接收到的信息。
         """
-        post_type = msg.get("post_type")
-        event_type = msg.get(post_type + "_type")
-        sub_type = msg.get("sub_type", None)
-        event_class = get_event_class(post_type, event_type, sub_type)
+        post_type = msg.get("post_type", None)
+        if post_type is None:
+            event_class = self.get_event_model(None, None, None)
+        else:
+            event_class = self.get_event_model(
+                post_type,
+                msg.get(post_type + "_type", None),
+                msg.get("sub_type", None),
+            )
 
         cqhttp_event = event_class(adapter=self, **msg)
 
         if cqhttp_event.post_type == "meta_event":
             # meta_event 不交由插件处理
-            if (
-                cqhttp_event.meta_event_type == "lifecycle"
-                and cqhttp_event.sub_type == "connect"
-            ):
-                logger.info(
-                    f"WebSocket connection "
-                    f"from CQHTTP Bot {msg.get('self_id')} accepted!"
-                )
+            assert isinstance(cqhttp_event, MetaEvent)
+            if cqhttp_event.meta_event_type == "lifecycle":
+                assert isinstance(cqhttp_event, LifecycleMetaEvent)
+                if cqhttp_event.sub_type == "connect":
+                    logger.info(
+                        f"WebSocket connection "
+                        f"from CQHTTP Bot {msg.get('self_id')} accepted!"
+                    )
             elif cqhttp_event.meta_event_type == "heartbeat":
+                assert isinstance(cqhttp_event, HeartbeatMetaEvent)
                 if cqhttp_event.status.good and cqhttp_event.status.online:
                     pass
                 else:
                     logger.error(
                         f"CQHTTP Bot status is not good: {cqhttp_event.status.dict()}"
                     )
         else:
             await self.handle_event(cqhttp_event)
 
-    async def call_api(self, api: str, **params) -> Any:
-        """调用 CQHTTP API，协程会等待直到获得 API 响应。
+    async def call_api(self, api: str, **params: Any) -> Any:
+        """调用 CQHTTP API ，协程会等待直到获得 API 响应。
 
         Args:
             api: API 名称。
             **params: API 参数。
 
         Returns:
             API 响应中的 data 字段。
 
         Raises:
             NetworkError: 网络错误。
-            ApiNotAvailable: API 请求响应 404， API 不可用。
-            ActionFailed: API 请求响应 failed， API 操作失败。
+            ApiNotAvailable: API 请求响应 404 ， API 不可用。
+            ActionFailed: API 请求响应 failed ， API 操作失败。
             ApiTimeout: API 请求响应超时。
         """
+        assert self.websocket is not None
         api_echo = self._get_api_echo()
         try:
             await self.websocket.send_str(
                 json.dumps(
                     {"action": api, "params": params, "echo": api_echo},
                     cls=DataclassEncoder,
                 )
@@ -183,23 +252,23 @@
                     return self._api_response.get("data")
 
         if not self.bot.should_exit.is_set():
             raise ApiTimeout
 
     async def send(
         self, message_: "T_CQMSG", message_type: Literal["private", "group"], id_: int
-    ) -> Dict[str, Any]:
+    ) -> Any:
         """发送消息，调用 send_private_msg 或 send_group_msg API 发送消息。
 
         Args:
             message_: 消息内容，可以是 str, Mapping, Iterable[Mapping],
                 'CQHTTPMessageSegment', 'CQHTTPMessage'。
                 将使用 `CQHTTPMessage` 进行封装。
             message_type: 消息类型。应该是 private 或者 group。
-            id_: 发送对象的 ID ，QQ 号码或者群号码。
+            id_: 发送对象的 ID ， QQ 号码或者群号码。
 
         Returns:
             API 响应。
 
         Raises:
             TypeError: message_type 不是 'private' 或 'group'。
             ...: 同 `call_api()` 方法。
```

### Comparing `alicebot_adapter_cqhttp-0.6.0.post1/alicebot/adapter/cqhttp/config.py` & `alicebot_adapter_cqhttp-0.6.2/alicebot/adapter/cqhttp/config.py`

 * *Files identical despite different names*

### Comparing `alicebot_adapter_cqhttp-0.6.0.post1/alicebot/adapter/cqhttp/event.py` & `alicebot_adapter_cqhttp-0.6.2/alicebot/adapter/cqhttp/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """CQHTTP 适配器事件。"""
 import inspect
-from typing import TYPE_CHECKING, Any, Dict, Type, Literal, TypeVar, Optional
+from typing import TYPE_CHECKING, Any, Dict, Tuple, Literal, Optional
 
 from pydantic import Field, BaseModel
+from pydantic.fields import ModelField
+from pydantic.typing import is_literal_type, all_literal_values
 
 from alicebot.event import Event
 
 from .message import CQHTTPMessage
 
 if TYPE_CHECKING:
+    from . import CQHTTPAdapter
     from .message import T_CQMSG
-    from . import CQHTTPAdapter  # noqa
-
-T_CQHTTPEvent = TypeVar("T_CQHTTPEvent", bound="CQHTTPEvent")
 
 
 class Sender(BaseModel):
     user_id: Optional[int]
     nickname: Optional[str]
     card: Optional[str]
     sex: Optional[Literal["male", "female", "unknown"]]
@@ -44,28 +44,54 @@
     online: bool
     good: bool
 
     class Config:
         extra = "allow"
 
 
+def _get_literal_field(field: ModelField) -> Optional[str]:
+    if not is_literal_type(field.outer_type_):
+        return None
+    literal_values = all_literal_values(field.outer_type_)
+    if len(literal_values) != 1:
+        return None
+    return literal_values[0]
+
+
 class CQHTTPEvent(Event["CQHTTPAdapter"]):
     """CQHTTP 事件基类"""
 
     __event__ = ""
     type: Optional[str] = Field(alias="post_type")
     time: int
     self_id: int
-    post_type: Literal["message", "notice", "request", "meta_event"]
+    post_type: str
 
     @property
     def to_me(self) -> bool:
         """当前事件的 user_id 是否等于 self_id。"""
         return getattr(self, "user_id") == self.self_id
 
+    @classmethod
+    def get_event_type(cls) -> Tuple[Optional[str], Optional[str], Optional[str]]:
+        """获取事件类型。
+
+        Returns:
+            事件类型。
+        """
+        post_type_field = cls.__fields__.get("post_type", None)
+        post_type = post_type_field and _get_literal_field(post_type_field)
+        if post_type is None:
+            return (None, None, None)
+        detail_type_field = cls.__fields__.get(post_type + "_type", None)
+        detail_type = detail_type_field and _get_literal_field(detail_type_field)
+        sub_type_field = cls.__fields__.get("sub_type", None)
+        sub_type = sub_type_field and _get_literal_field(sub_type_field)
+        return (post_type, detail_type, sub_type)
+
 
 class MessageEvent(CQHTTPEvent):
     """消息事件"""
 
     __event__ = "message"
     post_type: Literal["message"]
     message_type: Literal["private", "group"]
@@ -220,15 +246,15 @@
 
 class NotifyEvent(NoticeEvent):
     """提醒事件"""
 
     __event__ = "notice.notify"
     notice_type: Literal["notify"]
     sub_type: str
-    group_id: int
+    group_id: Optional[int]
     user_id: int
 
 
 class PokeNotifyEvent(NotifyEvent):
     """戳一戳"""
 
     __event__ = "notice.notify.poke"
@@ -238,22 +264,24 @@
 
 
 class GroupLuckyKingNotifyEvent(NotifyEvent):
     """群红包运气王"""
 
     __event__ = "notice.notify.lucky_king"
     sub_type: Literal["lucky_king"]
+    group_id: int
     target_id: int
 
 
 class GroupHonorNotifyEvent(NotifyEvent):
     """群成员荣誉变更"""
 
     __event__ = "notice.notify.honor"
     sub_type: Literal["honor"]
+    group_id: int
     honor_type: Literal["talkative", "performer", "emotion"]
 
 
 class RequestEvent(CQHTTPEvent):
     """请求事件"""
 
     __event__ = "request"
@@ -359,28 +387,7 @@
 
 
 _cqhttp_events = {
     model.__event__: model
     for model in globals().values()
     if inspect.isclass(model) and issubclass(model, CQHTTPEvent)
 }
-
-
-def get_event_class(
-    post_type: str, event_type: str, sub_type: Optional[str] = None
-) -> Type[T_CQHTTPEvent]:
-    """根据接收到的消息类型返回对应的事件类。
-
-    Args:
-        post_type: 请求类型。
-        event_type: 事件类型。
-        sub_type: 子类型。
-
-    Returns:
-        对应的事件类。
-    """
-    if sub_type is None:
-        return _cqhttp_events[".".join((post_type, event_type))]
-    return (
-        _cqhttp_events.get(".".join((post_type, event_type, sub_type)))
-        or _cqhttp_events[".".join((post_type, event_type))]
-    )
```

### Comparing `alicebot_adapter_cqhttp-0.6.0.post1/alicebot/adapter/cqhttp/exceptions.py` & `alicebot_adapter_cqhttp-0.6.2/alicebot/adapter/cqhttp/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """CQHTTP 适配器异常。"""
+from typing import Any, Dict
+
 from alicebot.exceptions import AdapterException
 
 
 class CQHTTPException(AdapterException):
     """CQHTTP 异常基类。"""
 
 
 class NetworkError(CQHTTPException):
     """网络异常。"""
 
 
 class ActionFailed(CQHTTPException):
     """API 请求成功响应，但响应表示 API 操作失败。"""
 
-    def __init__(self, resp):
+    def __init__(self, resp: Dict[str, Any]):
         """
         Args:
             resp: 返回的响应。
         """
         self.resp = resp
 
 
 class ApiNotAvailable(ActionFailed):
-    """API 请求返回 404，表示当前请求的 API 不可用或不存在。"""
+    """API 请求返回 404 ，表示当前请求的 API 不可用或不存在。"""
 
 
 class ApiTimeout(CQHTTPException):
     """API 请求响应超时。"""
```

### Comparing `alicebot_adapter_cqhttp-0.6.0.post1/alicebot/adapter/cqhttp/message.py` & `alicebot_adapter_cqhttp-0.6.2/alicebot/adapter/cqhttp/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 """CQHTTP 适配器消息。"""
-from typing import Type, Union, Literal, Mapping, Iterable, Optional
+from typing import Any, Type, Union, Literal, Mapping, Iterable, Optional
 
 from alicebot.message import Message, MessageSegment
 
 __all__ = ["T_CQMSG", "CQHTTPMessage", "CQHTTPMessageSegment", "escape"]
 
 T_CQMSG = Union[
-    str, Mapping, Iterable[Mapping], "CQHTTPMessageSegment", "CQHTTPMessage"
+    str,
+    Mapping[str, Any],
+    Iterable[Mapping[str, Any]],
+    "CQHTTPMessageSegment",
+    "CQHTTPMessage",
 ]
 
 
 class CQHTTPMessage(Message["CQHTTPMessageSegment"]):
     """CQHTTP 消息。"""
 
     @property
     def _message_segment_class(self) -> Type["CQHTTPMessageSegment"]:
         return CQHTTPMessageSegment
 
-    def _str_to_message_segment(self, msg) -> "CQHTTPMessageSegment":
+    def _str_to_message_segment(self, msg: str) -> "CQHTTPMessageSegment":
         return CQHTTPMessageSegment.text(msg)
 
 
 class CQHTTPMessageSegment(MessageSegment["CQHTTPMessage"]):
     """CQHTTP 消息字段。"""
 
     @property
@@ -218,15 +222,15 @@
     @classmethod
     def node(cls, id_: int) -> "CQHTTPMessageSegment":
         """合并转发节点"""
         return cls(type="node", data={"id": str(id_)})
 
     @classmethod
     def node_custom(
-        cls, user_id: int, nickname, content: "CQHTTPMessage"
+        cls, user_id: int, nickname: str, content: "CQHTTPMessage"
     ) -> "CQHTTPMessageSegment":
         """合并转发自定义节点"""
         return cls(
             type="node",
             data={
                 "user_id": str(user_id),
                 "nickname": str(nickname),
```

### Comparing `alicebot_adapter_cqhttp-0.6.0.post1/pyproject.toml` & `alicebot_adapter_cqhttp-0.6.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 [tool.poetry]
 name = "alicebot-adapter-cqhttp"
-version = "0.6.0.post1"
+version = "0.6.2"
 description = "OneBot(CQHTTP) adapter for AliceBot."
 license = "MIT"
 authors = ["st1020 <stone_1020@qq.com>"]
 readme = "README.md"
 homepage = "https://docs.alicebot.dev/"
-repository = "https://github.com/st1020/alicebot"
+repository = "https://github.com/AliceBotProject/alicebot"
 documentation = "https://docs.alicebot.dev/"
 keywords = ["bot", "chatbot", "qq", "qqbot", "cqhttp", "coolq"]
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

### Comparing `alicebot_adapter_cqhttp-0.6.0.post1/PKG-INFO` & `alicebot_adapter_cqhttp-0.6.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alicebot-adapter-cqhttp
-Version: 0.6.0.post1
+Version: 0.6.2
 Summary: OneBot(CQHTTP) adapter for AliceBot.
 Home-page: https://docs.alicebot.dev/
 License: MIT
 Keywords: bot,chatbot,qq,qqbot,cqhttp,coolq
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
 
 # AliceBot-Adapter-CQHTTP
 
 **OneBot(CQHTTP) 协议适配**
 
 </div>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: alicebot-adapter-cqhttp Version: 0.6.0.post1
-Summary: OneBot(CQHTTP) adapter for AliceBot. Home-page: https://
-docs.alicebot.dev/ License: MIT Keywords: bot,chatbot,qq,qqbot,cqhttp,coolq
-Author: st1020 Author-email: stone_1020@qq.com Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 3 - Alpha Classifier: Framework :: AsyncIO
-Classifier: Framework :: Robot Framework Classifier: Framework :: Robot
-Framework :: Library Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3 Classifier: Topic :: Communications :: Chat
-Requires-Dist: alicebot (>=0.6.0,<0.7.0) Project-URL: Documentation, https://
-docs.alicebot.dev/ Project-URL: Repository, https://github.com/st1020/alicebot
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: alicebot-adapter-cqhttp Version: 0.6.2 Summary:
+OneBot(CQHTTP) adapter for AliceBot. Home-page: https://docs.alicebot.dev/
+License: MIT Keywords: bot,chatbot,qq,qqbot,cqhttp,coolq Author: st1020 Author-
+email: stone_1020@qq.com Requires-Python: >=3.8,<4.0 Classifier: Development
+Status :: 3 - Alpha Classifier: Framework :: AsyncIO Classifier: Framework ::
+Robot Framework Classifier: Framework :: Robot Framework :: Library Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3 Classifier: Topic :: Communications :: Chat Requires-Dist: alicebot
+(==0.6.2) Project-URL: Documentation, https://docs.alicebot.dev/ Project-URL:
+Repository, https://github.com/AliceBotProject/alicebot Description-Content-
+Type: text/markdown
        [logo] # AliceBot-Adapter-CQHTTP **OneBot(CQHTTP) åè®®éé**
```

