# Comparing `tmp/alicebot-0.6.1.tar.gz` & `tmp/alicebot-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicebot-0.6.1.tar", max compression
+gzip compressed data, was "alicebot-0.6.2.tar", max compression
```

## Comparing `alicebot-0.6.1.tar` & `alicebot-0.6.2.tar`

### file list

```diff
@@ -1,19 +1,17 @@
--rw-r--r--   0        0        0     1072 2021-07-24 10:29:46.235810 alicebot-0.6.1/LICENSE
--rw-r--r--   0        0        0     6056 2022-11-26 14:56:24.214652 alicebot-0.6.1/README.md
--rw-r--r--   0        0        0      576 2022-11-25 08:05:51.125434 alicebot-0.6.1/alicebot/__init__.py
--rw-r--r--   0        0        0     4462 2022-11-25 08:04:54.352537 alicebot-0.6.1/alicebot/adapter/__init__.py
--rw-r--r--   0        0        0     1223 2022-11-24 15:50:24.489647 alicebot-0.6.1/alicebot/adapter/http_server_test_adapter.py
--rw-r--r--   0        0        0     1065 2022-11-24 15:51:14.019230 alicebot-0.6.1/alicebot/adapter/test.py
--rw-r--r--   0        0        0     7964 2022-11-24 16:11:27.882361 alicebot-0.6.1/alicebot/adapter/utils.py
--rw-r--r--   0        0        0    34442 2022-12-02 13:33:54.561177 alicebot-0.6.1/alicebot/bot.py
--rw-r--r--   0        0        0     1919 2022-11-26 11:41:42.611663 alicebot-0.6.1/alicebot/config.py
--rw-r--r--   0        0        0     1919 2022-11-15 13:09:44.844629 alicebot-0.6.1/alicebot/event.py
--rw-r--r--   0        0        0     1115 2022-05-31 12:01:12.839144 alicebot-0.6.1/alicebot/exceptions.py
--rw-r--r--   0        0        0      432 2022-08-14 11:24:09.437713 alicebot-0.6.1/alicebot/log.py
--rw-r--r--   0        0        0    13846 2022-06-01 06:54:36.396956 alicebot-0.6.1/alicebot/message.py
--rw-r--r--   0        0        0     3533 2022-11-25 06:50:12.661758 alicebot-0.6.1/alicebot/plugin.py
--rw-r--r--   0        0        0     1141 2022-11-25 08:04:54.352631 alicebot-0.6.1/alicebot/typing.py
--rw-r--r--   0        0        0     5535 2022-11-24 15:15:30.133118 alicebot-0.6.1/alicebot/utils.py
--rw-r--r--   0        0        0     2191 2022-12-03 14:12:33.689294 alicebot-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     7053 1970-01-01 00:00:00.000000 alicebot-0.6.1/setup.py
--rw-r--r--   0        0        0     7481 1970-01-01 00:00:00.000000 alicebot-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-25 11:14:36.273730 alicebot-0.6.2/LICENSE
+-rw-r--r--   0        0        0     6110 2023-04-25 11:14:36.273730 alicebot-0.6.2/README.md
+-rw-r--r--   0        0        0      656 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/__init__.py
+-rw-r--r--   0        0        0     4498 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/adapter/__init__.py
+-rw-r--r--   0        0        0     8043 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/adapter/utils.py
+-rw-r--r--   0        0        0    34806 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/bot.py
+-rw-r--r--   0        0        0     1877 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/config.py
+-rw-r--r--   0        0        0     1851 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/event.py
+-rw-r--r--   0        0        0     1116 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/exceptions.py
+-rw-r--r--   0        0        0      432 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/log.py
+-rw-r--r--   0        0        0    14120 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/message.py
+-rw-r--r--   0        0        0     3568 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/plugin.py
+-rw-r--r--   0        0        0        0 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/py.typed
+-rw-r--r--   0        0        0     1034 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/typing.py
+-rw-r--r--   0        0        0     5457 2023-04-25 11:14:36.273730 alicebot-0.6.2/alicebot/utils.py
+-rw-r--r--   0        0        0     2680 2023-04-25 11:14:36.281730 alicebot-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     7545 1970-01-01 00:00:00.000000 alicebot-0.6.2/PKG-INFO
```

### Comparing `alicebot-0.6.1/LICENSE` & `alicebot-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alicebot-0.6.1/README.md` & `alicebot-0.6.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 <div align="center">
-  <a href="https://docs.alicebot.dev/"><img src="https://raw.githubusercontent.com/st1020/alicebot/master/docs/public/logo.png" width="200" height="200" alt="logo"></a>
+  <a href="https://docs.alicebot.dev/"><img src="https://raw.githubusercontent.com/AliceBotProject/alicebot/master/docs/public/logo.png" width="200" height="200" alt="logo"></a>
 
 # AliceBot
 
 **简单的 Python 异步多后端机器人框架**
 
 </div>
 
 <div align="center">
-  <a href="https://raw.githubusercontent.com/st1020/alicebot/master/LICENSE">
-    <img src="https://img.shields.io/github/license/st1020/alicebot" alt="license">
+  <a href="https://raw.githubusercontent.com/AliceBotProject/alicebot/master/LICENSE">
+    <img src="https://img.shields.io/github/license/AliceBotProject/alicebot" alt="license">
   </a>
   <a href="https://pypi.python.org/pypi/alicebot">
     <img src="https://img.shields.io/pypi/v/alicebot" alt="pypi">
   </a>
   <a href="https://pypi.python.org/pypi/alicebot">
     <img src="https://img.shields.io/pypi/pyversions/alicebot" alt="pypi">
   </a>
-  <a href="https://github.com/st1020/alicebot/">
-    <img src="https://img.shields.io/github/stars/st1020/alicebot?style=social" alt="github">
+  <a href="https://github.com/AliceBotProject/alicebot/">
+    <img src="https://img.shields.io/github/stars/AliceBotProject/alicebot?style=social" alt="github">
   </a>
   <br />
   <a href="https://jq.qq.com/?_wv=1027&k=ZbE3p6tq">
     <img src="https://img.shields.io/badge/QQ%E7%BE%A4-674802046-orange" alt="qq-group">
   </a>
 </div>
 
 <p align="center">
   <a href="https://docs.alicebot.dev/">文档</a>
   ·
   <a href="https://docs.alicebot.dev/guide/">指南</a>
   ·
   <a href="https://docs.alicebot.dev/guide/">API 参考</a>
   ·
-  <a href="https://github.com/st1020/alicebot-example">示例</a>
+  <a href="https://github.com/AliceBotProject/alicebot-example">示例</a>
 </p>
 
 ## 简介
 
 AliceBot 是一个简单的 Python 异步多后端机器人框架，支持多种协议适配，可以轻松地编写易于学习和使用的插件来拓展其功能。
 
 本项目受到了 [NoneBot](https://github.com/nonebot/nonebot2/) 项目的启发，您可以在 [对比](#对比) 小节中查看这两个项目的异同，以便您选择更适合自己的机器人框架。
```

### Comparing `alicebot-0.6.1/alicebot/__init__.py` & `alicebot-0.6.2/alicebot/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,12 +4,12 @@
 本模块从子模块导入了以下内容：
 - `Bot` => [`alicebot.bot.Bot`](./bot#Bot)
 - `Event` => [`alicebot.event.Event`](./event#Event)
 - `Plugin` => [`alicebot.plugin.Plugin`](./plugin#Plugin)
 - `Adapter` => [`alicebot.adapter.Adapter`](./adapter/#Adapter)
 - `ConfigModel` => [`alicebot.config.ConfigModel`](./config#ConfigModel)
 """
-from alicebot.bot import Bot
-from alicebot.event import Event
-from alicebot.plugin import Plugin
-from alicebot.adapter import Adapter
-from alicebot.config import ConfigModel
+from alicebot.bot import Bot  # type: ignore
+from alicebot.event import Event  # type: ignore
+from alicebot.plugin import Plugin  # type: ignore
+from alicebot.adapter import Adapter  # type: ignore
+from alicebot.config import ConfigModel  # type: ignore
```

### Comparing `alicebot-0.6.1/alicebot/adapter/__init__.py` & `alicebot-0.6.2/alicebot/adapter/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 """AliceBot 协议适配器。
 
 所有协议适配器都必须继承自 `Adapter` 基类。
 """
 import os
-import asyncio
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Type, Union, Generic, Callable, Optional, Awaitable
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Type,
+    Union,
+    Generic,
+    Callable,
+    Optional,
+    Awaitable,
+    final,
+)
 
-from alicebot.config import ConfigModel
 from alicebot.log import error_or_exception
 from alicebot.typing import T_Event, T_Config
-from alicebot.utils import is_config_class, sync_func_wrapper
+from alicebot.utils import wrap_get_func, is_config_class
 
 if TYPE_CHECKING:
     from alicebot.bot import Bot
+    from alicebot.event import Event
 
 __all__ = ["Adapter"]
 
 if os.getenv("ALICEBOT_DEV") == "1":
     # 当处于开发环境时，使用 pkg_resources 风格的命名空间包
     __import__("pkg_resources").declare_namespace(__name__)
 
@@ -28,30 +37,30 @@
     Attributes:
         name: 适配器的名称。
         bot: 当前的机器人对象。
     """
 
     name: str
     bot: "Bot"
-    Config: Type[ConfigModel]
+    Config: Type[T_Config] = type(None)  # type: ignore
 
     def __init__(self, bot: "Bot"):
         if not hasattr(self, "name"):
             self.name = self.__class__.__name__
         self.bot: "Bot" = bot
         self.handle_event = self.bot.handle_event
 
     @property
-    def config(self) -> Optional[T_Config]:
+    def config(self) -> T_Config:
         """适配器配置。"""
-        config_class: ConfigModel = getattr(self, "Config", None)
-        if is_config_class(config_class):
-            return getattr(self.bot.config.adapter, config_class.__config_name__, None)
-        return None
+        if is_config_class(self.Config):
+            return getattr(self.bot.config.adapter, self.Config.__config_name__, None)  # type: ignore
+        return None  # type: ignore
 
+    @final
     async def safe_run(self):
         """附带有异常处理地安全运行适配器。"""
         try:
             await self.run()
         except Exception as e:
             error_or_exception(
                 f"Run adapter {self.__class__.__name__} failed:",
@@ -59,15 +68,15 @@
                 self.bot.config.bot.log.verbose_exception,
             )
 
     @abstractmethod
     async def run(self):
         """适配器运行方法，适配器开发者必须实现该方法。
 
-        适配器运行过程中保持保持运行，当此方法结束后，AliceBot 不会自动重新启动适配器。
+        适配器运行过程中保持保持运行，当此方法结束后， AliceBot 不会自动重新启动适配器。
         """
         raise NotImplementedError
 
     async def startup(self):
         """在适配器开始运行前运行的方法，用于初始化适配器。
 
         AliceBot 依次运行并等待所有适配器的 `startup()` 方法，待运行完毕后再创建 `run()` 任务。
@@ -78,21 +87,22 @@
         """在适配器结束运行时运行的方法，用于安全地关闭适配器。
 
         AliceBot 在接收到系统的结束信号后依次运行并等待所有适配器的 `shutdown()` 方法。
         当强制退出时此方法可能未被执行。
         """
         pass
 
-    async def send(self, *args, **kwargs):
+    async def send(self, *args: Any, **kwargs: Any):
         """发送消息，需要适配器开发者实现。"""
         raise NotImplementedError
 
+    @final
     async def get(
         self,
-        func: Optional[Callable[[T_Event], Union[bool, Awaitable[bool]]]] = None,
+        func: Optional[Callable[["Event"], Union[bool, Awaitable[bool]]]] = None,
         *,
         max_try_times: Optional[int] = None,
         timeout: Optional[Union[int, float]] = None,
     ) -> T_Event:
         """获取满足指定条件的的事件，协程会等待直到适配器接收到满足条件的事件、超过最大事件数或超时。
 
         类似 Bot 类的 get() 方法，但是隐含了判断产生 event 的适配器是本适配器。
@@ -108,22 +118,22 @@
         Returns:
             返回满足 func 条件的事件。
 
         Raises:
             GetEventTimeout: 超过最大事件数或超时。
         """
 
-        def func_wrapper(_func):
-            async def _wrapper(_event: T_Event):
+        def func_wrapper(
+            _func: Callable[["Event"], Awaitable[bool]]
+        ) -> Callable[["Event"], Awaitable[bool]]:
+            async def _wrapper(_event: "Event") -> bool:
                 if _event.adapter is not self:
                     return False
                 return await _func(_event)
 
             return _wrapper
 
-        if func is None:
-            func = sync_func_wrapper(lambda x: True)
-        elif not asyncio.iscoroutinefunction(func):
-            func = sync_func_wrapper(func)
-        func = func_wrapper(func)
-
-        return await self.bot.get(func, max_try_times=max_try_times, timeout=timeout)
+        return await self.bot.get(
+            func_wrapper(wrap_get_func(func)),
+            max_try_times=max_try_times,
+            timeout=timeout,
+        )  # type: ignore
```

### Comparing `alicebot-0.6.1/alicebot/adapter/utils.py` & `alicebot-0.6.2/alicebot/adapter/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """适配器实用工具。
 
 这里定义了一些在编写适配器时常用的基类，适配器开发者可以直接继承自这里的类或者用作参考。
 """
 import asyncio
-from typing import Union, Literal
 from abc import ABCMeta, abstractmethod
+from typing import Union, Literal, Optional
 
 import aiohttp
 from aiohttp import web
 
 from alicebot.adapter import Adapter
 from alicebot.typing import T_Event, T_Config
 from alicebot.log import logger, error_or_exception
 
 
 class PollingAdapter(Adapter[T_Event, T_Config], metaclass=ABCMeta):
     """轮询式适配器示例。"""
 
-    delay: Union[int, float] = 0.1
+    delay: float = 0.1
     create_task: bool = False
 
     async def run(self):
         while not self.bot.should_exit.is_set():
             await asyncio.sleep(self.delay)
             if self.create_task:
                 asyncio.create_task(self.on_tick())
@@ -62,15 +62,15 @@
                     if self.bot.should_exit.is_set():
                         break
                     if msg.type == aiohttp.WSMsgType.ERROR:
                         break
                     await self.handle_response(msg)
 
     @abstractmethod
-    def handle_response(self, msg: aiohttp.WSMessage):
+    async def handle_response(self, msg: aiohttp.WSMessage):
         pass
 
 
 class HttpServerAdapter(Adapter[T_Event, T_Config], metaclass=ABCMeta):
     """HTTP 服务端适配器示例。"""
 
     app: web.Application
@@ -96,25 +96,25 @@
         self.site = web.TCPSite(self.runner, self.host, self.port)
         await self.site.start()
 
     async def shutdown(self):
         await self.runner.cleanup()
 
     @abstractmethod
-    async def handle_response(self, request: web.Request):
+    async def handle_response(self, request: web.Request) -> web.StreamResponse:
         pass
 
 
 class WebSocketServerAdapter(Adapter[T_Event, T_Config], metaclass=ABCMeta):
     """WebSocket 服务端适配器示例。"""
 
-    app: web.Application = None
-    runner: web.AppRunner = None
-    site: web.TCPSite = None
-    websocket: web.WebSocketResponse = None
+    app: web.Application
+    runner: web.AppRunner
+    site: web.TCPSite
+    websocket: web.WebSocketResponse
     host: str
     port: int
     url: str
 
     async def startup(self):
         self.app = web.Application()
         self.app.add_routes([web.get(self.url, self.handle_response)])
@@ -122,22 +122,19 @@
     async def run(self):
         self.runner = web.AppRunner(self.app)
         await self.runner.setup()
         self.site = web.TCPSite(self.runner, self.host, self.port)
         await self.site.start()
 
     async def shutdown(self):
-        if self.websocket is not None:
-            await self.websocket.close()
-        if self.site is not None:
-            await self.site.stop()
-        if self.runner is not None:
-            await self.runner.cleanup()
+        await self.websocket.close()
+        await self.site.stop()
+        await self.runner.cleanup()
 
-    async def handle_response(self, request: web.Request):
+    async def handle_response(self, request: web.Request) -> web.WebSocketResponse:
         ws = web.WebSocketResponse()
         await ws.prepare(request)
         self.websocket = ws
 
         msg: aiohttp.WSMessage
         async for msg in ws:
             if msg.type == aiohttp.WSMsgType.TEXT:
@@ -154,23 +151,25 @@
 
 class WebSocketAdapter(Adapter[T_Event, T_Config], metaclass=ABCMeta):
     """WebSocket 适配器示例。
 
     同时支持 WebSocket 客户端和服务端。
     """
 
-    websocket: Union[web.WebSocketResponse, aiohttp.ClientWebSocketResponse] = None
+    websocket: Union[
+        web.WebSocketResponse, aiohttp.ClientWebSocketResponse, None
+    ] = None
 
     # ws
-    session: aiohttp.ClientSession = None
+    session: Optional[aiohttp.ClientSession]
 
     # reverse-ws
-    app: web.Application = None
-    runner: web.AppRunner = None
-    site: web.TCPSite = None
+    app: Optional[web.Application]
+    runner: Optional[web.AppRunner]
+    site: Optional[web.TCPSite]
 
     # config
     adapter_type: Literal["ws", "reverse-ws"]
     host: str
     port: int
     url: str
     reconnect_interval: int = 3
@@ -200,14 +199,15 @@
                         e,
                         self.bot.config.bot.log.verbose_exception,
                     )
                 if self.bot.should_exit.is_set():
                     break
                 await asyncio.sleep(self.reconnect_interval)
         elif self.adapter_type == "reverse-ws":
+            assert self.app is not None
             self.runner = web.AppRunner(self.app)
             await self.runner.setup()
             self.site = web.TCPSite(self.runner, self.host, self.port)
             await self.site.start()
 
     async def shutdown(self):
         """关闭并清理连接。"""
@@ -218,37 +218,40 @@
                 await self.session.close()
         elif self.adapter_type == "reverse-ws":
             if self.site is not None:
                 await self.site.stop()
             if self.runner is not None:
                 await self.runner.cleanup()
 
-    async def handle_reverse_ws_response(self, request: web.Request):
+    async def handle_reverse_ws_response(
+        self, request: web.Request
+    ) -> web.WebSocketResponse:
         """处理 aiohttp WebSocket 服务器的接收。"""
         self.websocket = web.WebSocketResponse()
         await self.websocket.prepare(request)
         await self.reverse_ws_connection_hook()
         await self.handle_websocket()
         return self.websocket
 
     async def reverse_ws_connection_hook(self):
         """反向 WebSocket 连接建立时的钩子函数。"""
         logger.info(f"WebSocket connected!")
 
     async def websocket_connect(self):
         """创建正向 WebSocket 连接。"""
+        assert self.session is not None
         logger.info("Tying to connect to WebSocket server...")
         async with self.session.ws_connect(
             f"ws://{self.host}:{self.port}{self.url}"
         ) as self.websocket:
             await self.handle_websocket()
 
     async def handle_websocket(self):
         """处理 WebSocket。"""
-        if self.websocket.closed:
+        if self.websocket is None or self.websocket.closed:
             return
         async for msg in self.websocket:
             msg: aiohttp.WSMessage
             await self.handle_websocket_msg(msg)
         if not self.bot.should_exit.is_set():
             logger.warning("WebSocket connection closed!")
```

### Comparing `alicebot-0.6.1/alicebot/bot.py` & `alicebot-0.6.2/alicebot/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,52 +4,48 @@
 """
 import os
 import sys
 import json
 import time
 import signal
 import asyncio
+import pkgutil
 import threading
 from pathlib import Path
 from itertools import chain
 from collections import defaultdict
 from typing import Any, Dict, List, Type, Union, Callable, Optional, Awaitable
 
 from pydantic import ValidationError, create_model
 
+from alicebot.event import Event
 from alicebot.adapter import Adapter
 from alicebot.plugin import Plugin, PluginLoadType
 from alicebot.log import logger, error_or_exception
+from alicebot.typing import T_Adapter, T_BotHook, T_EventHook, T_AdapterHook
 from alicebot.config import MainConfig, ConfigModel, PluginConfig, AdapterConfig
-from alicebot.typing import (
-    T_Event,
-    T_BotHook,
-    T_EventHook,
-    T_AdapterHook,
-    T_BotExitHook,
-)
 from alicebot.exceptions import (
     SkipException,
     StopException,
     GetEventTimeout,
     LoadModuleError,
 )
 from alicebot.utils import (
     ModulePathFinder,
     samefile,
+    wrap_get_func,
     is_config_class,
-    sync_func_wrapper,
-    get_classes_from_dir,
     get_classes_from_module_name,
 )
 
 try:
-    import tomllib  # noqa
+    import tomllib  # type: ignore
 except ModuleNotFoundError:
-    import tomli as tomllib
+    import tomli as tomllib  # type: ignore
+
 
 __all__ = ["Bot"]
 
 HANDLED_SIGNALS = (
     signal.SIGINT,  # Unix signal 2. Sent by Ctrl+C.
     signal.SIGTERM,  # Unix signal 15. Sent by `kill <pid>`.
 )
@@ -72,58 +68,58 @@
     should_exit: asyncio.Event
     adapters: List[Adapter]
     plugins_priority_dict: Dict[int, List[Type[Plugin]]]
     plugin_state: Dict[str, Any]
     global_state: Dict[Any, Any]
 
     _condition: asyncio.Condition  # 用于处理 get 的 Condition
-    _current_event: T_Event  # 当前待处理的 Event
+    _current_event: Event  # 当前待处理的 Event
 
     _restart_flag: bool  # 重新启动标志
     _module_path_finder: ModulePathFinder  # 用于查找 plugins 的模块元路径查找器
     _raw_config_dict: Dict[str, Any]  # 原始配置字典
 
     # 以下属性不会在重启时清除
     _config_file: Optional[str]  # 配置文件
     _config_dict: Optional[Dict[str, Any]]  # 配置字典
     _hot_reload: bool  # 热重载
 
     _extend_plugins: List[
         Union[Type[Plugin], str, Path]
     ]  # 使用 load_plugins() 方法程序化加载的插件列表
     _extend_plugin_dirs: List[Path]  # 使用 load_plugins_from_dirs() 方法程序化加载的插件路径列表
-    _extend_adapters: List[str]  # 使用 load_adapter() 方法程序化加载的适配器列表
+    _extend_adapters: List[Union[Type[Adapter], str]]  # 使用 load_adapter() 方法程序化加载的适配器列表
     _bot_run_hooks: List[T_BotHook]
-    _bot_exit_hooks: List[T_BotExitHook]
+    _bot_exit_hooks: List[T_BotHook]
     _adapter_startup_hooks: List[T_AdapterHook]
     _adapter_run_hooks: List[T_AdapterHook]
     _adapter_shutdown_hooks: List[T_AdapterHook]
     _event_preprocessor_hooks: List[T_EventHook]
     _event_postprocessor_hooks: List[T_EventHook]
 
     def __init__(
         self,
         *,
         config_file: Optional[str] = "config.toml",
-        config_dict: Optional[Dict] = None,
+        config_dict: Optional[Dict[str, Any]] = None,
         hot_reload: bool = False,
     ):
         """初始化 AliceBot ，读取配置文件，创建配置，加载适配器和插件。
 
         Args:
             config_file: 配置文件，如不指定则使用默认的 `config.toml`。
-                若指定为 None，则不加载配置文件。
+                若指定为 None ，则不加载配置文件。
             config_dict: 配置字典，默认为 None。
                 若指定字典，则会忽略 config_file 配置，不再读取配置文件。
             hot_reload: 热重载。
                 启用后将自动检查 `plugin_dir` 中的插件文件更新，并在更新时自动重新加载。
         """
         self.config = MainConfig()
         self.plugins_priority_dict = defaultdict(list)
-        self.plugin_state = defaultdict(type(None))
+        self.plugin_state = defaultdict(lambda: type(None)())
         self.global_state = {}
 
         self.adapters = []
         self._restart_flag = False
         self._module_path_finder = ModulePathFinder()
         self._raw_config_dict = {}
 
@@ -146,15 +142,15 @@
 
     @property
     def plugins(self) -> List[Type[Plugin]]:
         """当前已经加载的插件的列表。"""
         return list(chain(*self.plugins_priority_dict.values()))
 
     def run(self):
-        """运行 AliceBot，监听并拦截系统退出信号，更新机器人配置。"""
+        """运行 AliceBot ，监听并拦截系统退出信号，更新机器人配置。"""
         self._restart_flag = True
         while self._restart_flag:
             self._restart_flag = False
             asyncio.run(self._run())
             if self._restart_flag:
                 self._load_plugins_from_dirs(*self._extend_plugin_dirs)
                 self._load_plugins(*self._extend_plugins)
@@ -226,15 +222,15 @@
                 await hot_reload_task
         finally:
             for _adapter in self.adapters:
                 for _hook_func in self._adapter_shutdown_hooks:
                     await _hook_func(_adapter)
                 await _adapter.shutdown()
             for _hook_func in self._bot_exit_hooks:
-                _hook_func(self)
+                await _hook_func(self)
 
             self.adapters.clear()
             self.plugins_priority_dict.clear()
             self._module_path_finder.path.clear()
 
     def _remove_plugin_by_path(self, file: str) -> List[Type[Plugin]]:
         """根据路径删除已加载的插件。"""
@@ -256,15 +252,15 @@
                     f'"{plugin_.__name__}" from file "{file}"'
                 )
         return removed_plugins
 
     async def _run_hot_reload(self):
         """热重载。"""
         try:
-            from watchfiles import Change, PythonFilter, DefaultFilter, awatch
+            from watchfiles import Change, awatch
         except ImportError:
             logger.warning(
                 'Hot reload needs to install "watchfiles", '
                 'try "pip install watchfiles"'
             )
             return
 
@@ -283,21 +279,25 @@
             stop_event=self.should_exit,
         ):
             # 按照 Change.deleted, Change.modified, Change.added 的顺序处理
             # 以确保发生重命名时先处理删除再处理新增
             for change_type, file in sorted(changes, key=lambda x: x[0], reverse=True):
                 # 更改配置文件
                 if (
-                    samefile(self._config_file, file)
+                    self._config_file is not None
+                    and samefile(self._config_file, file)
                     and change_type == change_type.modified
                 ):
                     logger.info(f'Reload config file "{self._config_file}"')
                     old_config = self.config
                     self._reload_config_dict()
-                    if self.config.bot != old_config.bot:
+                    if (
+                        self.config.bot != old_config.bot
+                        or self.config.adapter != old_config.adapter
+                    ):
                         self.restart()
                     continue
 
                 # 更改插件文件夹
                 if change_type == Change.deleted:
                     # 针对删除操作特殊处理
                     if not file.endswith(".py"):
@@ -324,15 +324,15 @@
                 elif change_type == Change.modified:
                     logger.info(f"Hot reload: Modified file: {file}")
                     self._remove_plugin_by_path(file)
                     self._load_plugins(Path(file), plugin_load_type=PluginLoadType.DIR)
                     self._update_config()
 
     def _update_config(self):
-        """更新 config，合并入来自 Plugin 和 Adapter 的 Config。"""
+        """更新 config ，合并入来自 Plugin 和 Adapter 的 Config。"""
 
         def update_config(
             source: List, name: str, base: Type[ConfigModel]
         ) -> ConfigModel:
             config_update_dict = {}
             for i in source:
                 config_class = getattr(i, "Config", None)
@@ -398,25 +398,29 @@
         self.plugins_priority_dict.clear()
         self._load_plugins(*self.config.bot.plugins)
         self._load_plugins_from_dirs(*self.config.bot.plugin_dirs)
         self._load_plugins(*self._extend_plugins)
         self._load_plugins_from_dirs(*self._extend_plugin_dirs)
         self._update_config()
 
-    def _handle_exit(self, *args):  # noqa
+    def _handle_exit(self, *args: Any):
         """当机器人收到退出信号时，根据情况进行处理。"""
         logger.info("Stopping AliceBot...")
         if self.should_exit.is_set():
             logger.warning("Force Exit AliceBot...")
             sys.exit()
         else:
             self.should_exit.set()
 
     async def handle_event(
-        self, current_event: T_Event, *, handle_get: bool = True, show_log: bool = True
+        self,
+        current_event: Event,
+        *,
+        handle_get: bool = True,
+        show_log: bool = True,
     ):
         """被适配器对象调用，根据优先级分发事件给所有插件，并处理插件的 `stop` 、 `skip` 等信号。
 
         此方法不应该被用户手动调用。
 
         Args:
             current_event: 当前待处理的 `Event`。
@@ -433,15 +437,15 @@
             await asyncio.sleep(0)
             async with self._condition:
                 self._current_event = current_event
                 self._condition.notify_all()
         else:
             asyncio.create_task(self._handle_event(current_event))
 
-    async def _handle_event(self, current_event: Optional[T_Event] = None):
+    async def _handle_event(self, current_event: Optional[Event] = None):
         if current_event is None:
             async with self._condition:
                 await self._condition.wait()
                 current_event = self._current_event
             if current_event.__handled__:
                 return
 
@@ -488,19 +492,19 @@
         for _hook_func in self._event_postprocessor_hooks:
             await _hook_func(current_event)
 
         logger.info("Event Finished")
 
     async def get(
         self,
-        func: Optional[Callable[[T_Event], Union[bool, Awaitable[bool]]]] = None,
+        func: Optional[Callable[[Event], Union[bool, Awaitable[bool]]]] = None,
         *,
         max_try_times: Optional[int] = None,
         timeout: Optional[Union[int, float]] = None,
-    ) -> T_Event:
+    ) -> Event:
         """获取满足指定条件的的事件，协程会等待直到适配器接收到满足条件的事件、超过最大事件数或超时。
 
         Args:
             func: 协程或者函数，函数会被自动包装为协程执行。
                 要求接受一个事件作为参数，返回布尔值。当协程返回 `True` 时返回当前事件。
                 当为 `None` 时相当于输入对于任何事件均返回真的协程，即返回适配器接收到的下一个事件。
             max_try_times: 最大事件数。
@@ -508,18 +512,15 @@
 
         Returns:
             返回满足 func 条件的事件。
 
         Raises:
             GetEventTimeout: 超过最大事件数或超时。
         """
-        if func is None:
-            func = sync_func_wrapper(lambda x: True)
-        elif not asyncio.iscoroutinefunction(func):
-            func = sync_func_wrapper(func)
+        _func = wrap_get_func(func)
 
         try_times = 0
         start_time = time.time()
         while not self.should_exit.is_set():
             if max_try_times is not None and try_times > max_try_times:
                 break
             if timeout is not None and time.time() - start_time > timeout:
@@ -534,22 +535,21 @@
                             self._condition.wait(),
                             timeout=start_time + timeout - time.time(),
                         )
                     except asyncio.TimeoutError:
                         break
 
                 if not self._current_event.__handled__:
-                    if await func(self._current_event):
+                    if await _func(self._current_event):
                         self._current_event.__handled__ = True
                         return self._current_event
 
                 try_times += 1
 
-        if not self.should_exit.is_set():
-            raise GetEventTimeout
+        raise GetEventTimeout
 
     def _load_plugin_class(
         self,
         plugin_class: Type[Plugin],
         plugin_load_type: PluginLoadType,
         plugin_file_path: Optional[str],
     ):
@@ -681,19 +681,22 @@
     def _load_plugins_from_dirs(self, *dirs: Path):
         """从目录中加载插件，以 `_` 开头的模块中的插件不会被导入。路径可以是相对路径或绝对路径。
 
         Args:
             *dirs: 储存包含插件的模块的模块路径。
                 例如：`pathlib.Path("path/of/plugins/")` 。
         """
-        dirs = list(map(lambda x: str(x.resolve()), dirs))
-        logger.info(f'Loading plugins from dirs "{", ".join(map(str, dirs))}"')
-        self._module_path_finder.path.extend(dirs)
-        for plugin_class, module in get_classes_from_dir(dirs, Plugin):
-            self._load_plugin_class(plugin_class, PluginLoadType.DIR, module.__file__)
+        dir_list = list(map(lambda x: str(x.resolve()), dirs))
+        logger.info(f'Loading plugins from dirs "{", ".join(map(str, dir_list))}"')
+        self._module_path_finder.path.extend(dir_list)
+        for module_info in pkgutil.iter_modules(dir_list):
+            if not module_info.name.startswith("_"):
+                self._load_plugins_from_module_name(
+                    module_info.name, PluginLoadType.DIR
+                )
 
     def load_plugins_from_dirs(self, *dirs: Path):
         """从目录中加载插件，以 `_` 开头的模块中的插件不会被导入。路径可以是相对路径或绝对路径。
 
         Args:
             *dirs: 储存包含插件的模块的模块路径。
                 例如：`pathlib.Path("path/of/plugins/")` 。
@@ -726,15 +729,15 @@
                         raise LoadModuleError(
                             f"Can not find Adapter class in the {adapter_} module"
                         )
                     elif len(adapter_classes) > 1:
                         raise LoadModuleError(
                             f"More then one Adapter class in the {adapter_} module"
                         )
-                    adapter_object = adapter_classes[0][0](self)
+                    adapter_object = adapter_classes[0][0](self)  # type: ignore
                 else:
                     raise LoadModuleError(
                         f"Type error: {adapter_} can not be loaded as adapter"
                     )
             except Exception as e:
                 error_or_exception(
                     f'Load adapter "{adapter_}" failed:',
@@ -756,45 +759,50 @@
                 如果为 `Type[Adapter]` 类型时，将作为适配器类进行加载。
                 如果为 `str` 类型时，将作为适配器模块名称进行加载，格式和 Python `import` 语句相同。
                     例如：`path.of.adapter`。
         """
         self._extend_adapters.extend(adapters)
         return self._load_adapters(*adapters)
 
-    def get_adapter(self, name: str) -> Adapter:
-        """按照名称获取已经加载的适配器。
+    def get_adapter(
+        self, adapter: Union[str, Type[T_Adapter]]
+    ) -> Union[Adapter, T_Adapter]:
+        """按照名称或适配器类获取已经加载的适配器。
 
         Args:
-            name: 适配器名称。
+            adapter: 适配器名称或适配器类。
 
         Returns:
             获取到的适配器对象。
 
         Raises:
             LookupError: 找不到此名称的适配器对象。
         """
         for _adapter in self.adapters:
-            if _adapter.name == name:
+            if isinstance(adapter, str):
+                if _adapter.name == adapter:
+                    return _adapter
+            elif isinstance(_adapter, adapter):
                 return _adapter
-        raise LookupError(f'Can not find adapter named "{name}"')
+        raise LookupError(f'Can not find adapter named "{adapter}"')
 
     def get_plugin(self, name: str) -> Type[Plugin]:
         """按照名称获取已经加载的插件类。
 
         Args:
             name: 插件名称
 
         Returns:
             获取到的插件类。
 
         Raises:
             LookupError: 找不到此名称的插件类。
         """
         for _plugin in self.plugins:
-            if _plugin.name == name:
+            if _plugin.__name__ == name:
                 return _plugin
         raise LookupError(f'Can not find plugin named "{name}"')
 
     def bot_run_hook(self, func: T_BotHook) -> T_BotHook:
         """注册一个 Bot 启动时的函数。
 
         Args:
@@ -802,15 +810,15 @@
 
         Returns:
             被注册的函数。
         """
         self._bot_run_hooks.append(func)
         return func
 
-    def bot_exit_hook(self, func: T_BotExitHook) -> T_BotExitHook:
+    def bot_exit_hook(self, func: T_BotHook) -> T_BotHook:
         """注册一个 Bot 退出时的函数。
 
         Args:
             func: 被注册的函数。
 
         Returns:
             被注册的函数。
```

### Comparing `alicebot-0.6.1/alicebot/config.py` & `alicebot-0.6.2/alicebot/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 class ConfigModel(BaseModel):
     """AliceBot 配置模型。
 
     Attributes:
         __config_name__: 配置名称。
     """
 
-    __config_name__: str
+    __config_name__: str = ""
 
     class Config:
         extra = Extra.allow
 
 
 class LogConfig(ConfigModel):
     """AliceBot 日志相关设置。
@@ -71,10 +71,7 @@
     Attributes:
         bot: AliceBot 的主要配置。
     """
 
     bot: BotConfig = BotConfig()
     plugin: PluginConfig = PluginConfig()
     adapter: AdapterConfig = AdapterConfig()
-
-    class Config:
-        extra = Extra.allow
```

### Comparing `alicebot-0.6.1/alicebot/event.py` & `alicebot-0.6.2/alicebot/event.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """AliceBot 事件。
 
 事件类的基类。适配器开发者应实现此事件类基类的子类。
 """
 from abc import ABC
-from typing import Any, Generic, Optional
+from typing import Any, Generic, Optional, final
 
 from pydantic import BaseModel, PrivateAttr
 
 from alicebot.message import Message
 from alicebot.typing import T_Adapter
 from alicebot.utils import DataclassEncoder
 
@@ -20,34 +20,32 @@
     Attributes:
         adapter: 产生当前事件的适配器对象。
         type: 事件类型。
         __handled__: 表示事件是否被处理过了，用于适配器处理。
             警告：请勿手动更改此属性的值。
     """
 
-    adapter: Any
+    adapter: T_Adapter  # type: ignore
     # 这里的 adapter 类型定义只是为了 IDE 的类型检查工具能够正常工作，这个字段将永远不会被实际使用
     # IDE 对 BaseModel 实例化时的提示会将 BaseModel 视为 dataclasses，而忽略 __init__ 定义
     # 因此需要此定义防止类型提示出错
     # 参考：
     # https://pydantic-docs.helpmanual.io/visual_studio_code/#technical-details
     # https://koxudaxi.github.io/pydantic-pycharm-plugin/ignore-init-arguments/
 
     type: Optional[str]
 
-    _adapter: Optional[T_Adapter] = PrivateAttr()  # adapter 实际上放在这里
+    _adapter: T_Adapter = PrivateAttr()  # adapter 实际上放在这里
     __handled__: bool = PrivateAttr(default=False)
 
-    def __init__(self, **data):
-        if "adapter" in data:
-            self._adapter = data.pop("adapter")
-        else:
-            raise ValueError('"adapter" argument must be set')
+    def __init__(self, adapter: T_Adapter, **data: Any):
+        self._adapter = adapter
         super().__init__(**data)
 
+    @final
     @property
     def adapter(self) -> T_Adapter:
         """产生当前事件的适配器对象。"""
         return self._adapter
 
     def __str__(self) -> str:
         return f"Event<{self.type}>"
```

### Comparing `alicebot-0.6.1/alicebot/exceptions.py` & `alicebot-0.6.2/alicebot/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """AliceBot 异常。
 
-下列是 AliceBot 运行过程中可能会抛出的异常。这些异常大部分不需要用户处理，AliceBot 会自动捕获并处理。
+下列是 AliceBot 运行过程中可能会抛出的异常。这些异常大部分不需要用户处理， AliceBot 会自动捕获并处理。
 对于适配器开发者，所有适配器抛出的异常都应该继承自 `AdapterException` 。
 """
 
 
 class EventException(BaseException):
     """事件处理过程中由插件抛出的异常，用于控制事件的传播，会被 AliceBot 自动捕获并处理。"""
```

### Comparing `alicebot-0.6.1/alicebot/message.py` & `alicebot-0.6.2/alicebot/message.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,78 +1,79 @@
 """AliceBot 消息。
 
 实现了常用的基本消息 `Message` 和消息字段 `MessageSegment` 模型供适配器使用。
 适配器开发者可以根据需要实现此模块中消息类的子类或定义与此不同的消息类型，但建议若可行的话应尽量使用此模块中消息类的子类。
 """
 import dataclasses
 from copy import copy, deepcopy
+from typing_extensions import Self
 from dataclasses import field, dataclass
 from typing import (
     Any,
     Dict,
     List,
     Type,
     Union,
     Generic,
     Mapping,
     TypeVar,
     Iterable,
     Iterator,
+    Optional,
+    SupportsIndex,
 )
 
 __all__ = ["T_Message", "T_MessageSegment", "T_MS", "Message", "MessageSegment"]
 
 T_Message = TypeVar("T_Message", bound="Message")
 T_MessageSegment = TypeVar("T_MessageSegment", bound="MessageSegment")
 
 # 可以转化为 MessageSegment 的类型
-T_MS = Union[T_MessageSegment, str, Mapping]
+T_MS = Union[T_MessageSegment, str, Mapping[str, Any]]
 
 
 class Message(List[T_MessageSegment]):
     """消息。
 
     本类是 `List` 的子类，并重写了 `__init__()` 方法，
-    可以直接处理 str, Mapping, Iterable[Mapping], T_MessageSegment, T_Message。
+    可以直接处理 str, Mapping, Iterable[Mapping], MessageSegment, Message。
     其中 str 的支持需要适配器开发者重写 `_str_to_message_segment()` 方法实现。
     本类重写了 `+` 和 `+=` 运算符，可以直接和 Message, MessageSegment 等类型的对象执行取和运算。
     若开发者实现了 MessageSegment 的子类则需要重写 `_message_segment_class()` 方法，
     并在 MessageSegment 的子类中重写 `_message_class()` 方法。
     """
 
     def __init__(
         self,
-        message: Union[None, T_Message, T_MS, Iterable[T_MS]] = None,
-        *args,
-        **kwargs,
+        message: Union[Self, T_MS, Iterable[T_MS]] = None,
+        *args: Any,
+        **kwargs: Any,
     ):
         super().__init__(*args, **kwargs)
-        if message is None:
-            return
-        elif isinstance(message, self.__class__):
-            self.extend(message)
+        if isinstance(message, self.__class__):
+            self.extend(message)  # type: ignore
         else:
             self.extend(self._construct(message))
 
     @property
     def _message_segment_class(self) -> Type[T_MessageSegment]:
         """若开发者实现了 MessageSegment 的子类则需要重写此方法。
 
         Returns:
             MessageSegment 类。
         """
-        return MessageSegment
+        return MessageSegment  # type: ignore
 
     @classmethod
     def __get_validators__(cls):
         """pydantic 自定义校验器。"""
         yield cls._validate
 
     @classmethod
-    def _validate(cls, value):
+    def _validate(cls, value: Mapping[str, Any]):
         return cls(value)
 
     def _construct(
         self, msg: Union[T_MS, Iterable[T_MS]]
     ) -> Iterator[T_MessageSegment]:
         """用于将 str, Mapping, Iterable[Mapping] 等类型转换为 MessageSegment。
         用于 pydantic 数据解析和方便用户使用。
@@ -82,35 +83,35 @@
 
         Returns:
             MessageSegment 生成器。
         """
         if isinstance(msg, self._message_segment_class):
             yield msg
         elif isinstance(msg, Mapping):
-            yield self._mapping_to_message_segment(msg)
+            yield self._mapping_to_message_segment(msg)  # type: ignore
         elif isinstance(msg, str):
             yield self._str_to_message_segment(msg)
-        elif isinstance(msg, Iterable):
+        else:
             for seg in msg:
                 for i in self._construct(seg):
                     yield i
 
-    def _mapping_to_message_segment(self, msg: Mapping) -> T_MessageSegment:
-        """用于将 Mapping 转换为 MessageSegment，如有需要，子类可重写此方法以更改对 Mapping 的默认行为。
+    def _mapping_to_message_segment(self, msg: Mapping[str, Any]) -> T_MessageSegment:
+        """用于将 Mapping 转换为 MessageSegment ，如有需要，子类可重写此方法以更改对 Mapping 的默认行为。
 
         Args:
             msg: 要解析为 MessageSegment 的数据。
 
         Returns:
             由 Mapping 转换的 MessageSegment。
         """
         return self._message_segment_class(**msg)
 
     def _str_to_message_segment(self, msg: str) -> T_MessageSegment:
-        """用于将 str 转换为 MessageSegment，子类应重写此方法以支持 str 及支持新的消息字段类。
+        """用于将 str 转换为 MessageSegment ，子类应重写此方法以支持 str 及支持新的消息字段类。
 
         Args:
             msg: 要解析为 MessageSegment 的数据。
 
         Returns:
             由 str 转换的 MessageSegment。
         """
@@ -118,15 +119,15 @@
 
     def __repr__(self) -> str:
         return "Message:[{}]".format(",".join(map(lambda x: repr(x), self)))
 
     def __str__(self) -> str:
         return "".join(map(lambda x: str(x), self))
 
-    def __contains__(self, item) -> bool:
+    def __contains__(self, item: object) -> bool:
         if isinstance(item, str):
             return item in str(self)
         return super().__contains__(item)
 
     def __add__(
         self: T_Message, other: Union[T_Message, T_MessageSegment, str]
     ) -> T_Message:
@@ -149,51 +150,51 @@
         else:
             raise TypeError(
                 f"unsupported operand type(s) for +: '{type(self)}' and '{type(other)}'"
             )
         return self
 
     def is_text(self) -> bool:
-        """
-        Returns:
-            是否是纯文本消息。
-        """
+        """是否是纯文本消息。"""
         return all(map(lambda x: x.is_text(), self))
 
     def get_plain_text(self) -> str:
         """获取消息中的纯文本部分。
 
         Returns:
             消息中的纯文本部分。
         """
         return "".join(map(lambda x: str(x), filter(lambda x: x.is_text(), self)))
 
-    def copy(self) -> T_Message:
+    def copy(self) -> Self:
         """返回自身的浅复制。
 
         Returns:
             自身的浅复制。
         """
         return self.__class__(self)
 
-    def deepcopy(self) -> T_Message:
+    def deepcopy(self) -> Self:
         """返回自身的深复制。
 
         Returns:
             自身的深复制。
         """
         return deepcopy(self)
 
     def startswith(
-        self, prefix: Union[str, T_MessageSegment], start=None, end=None
+        self,
+        prefix: Union[str, T_MessageSegment],
+        start: Optional[SupportsIndex] = None,
+        end: Optional[SupportsIndex] = None,
     ) -> bool:
         """实现类似字符串的 `startswith()` 方法。
 
         当 `prefix` 类型是 str 时，会将自身转换为 str 类型，再调用 str 类型的 `startswith()` 方法。
-        当 `prefix` 类型是 T_MessageSegment 时，`start` 和 `end` 参数将不其作用，
+        当 `prefix` 类型是 MessageSegment 时，`start` 和 `end` 参数将不其作用，
             会判断列表的第一个消息字段是否和 `prefix` 相等。
 
         Args:
             prefix: 前缀。
             start: 开始检查位置。
             end: 停止检查位置。
 
@@ -203,24 +204,27 @@
         if isinstance(prefix, str):
             return str(self).startswith(prefix, start, end)
         elif isinstance(prefix, self._message_segment_class):
             if len(self) == 0:
                 return False
             return self[0] == prefix
         raise TypeError(
-            f"first arg must be str or {self._message_segment_class}，not {type(prefix)}"
+            f"first arg must be str or {self._message_segment_class}, not {type(prefix)}"
         )
 
     def endswith(
-        self, suffix: Union[str, T_MessageSegment], start=None, end=None
+        self,
+        suffix: Union[str, T_MessageSegment],
+        start: Optional[SupportsIndex] = None,
+        end: Optional[SupportsIndex] = None,
     ) -> bool:
         """实现类似字符串的 `endswith()` 方法。
 
         当 `suffix` 类型是 str 时，会将自身转换为 str 类型，再调用 str 类型的 `endswith()` 方法。
-        当 `suffix` 类型是 T_MessageSegment 时，`start` 和 `end` 参数将不其作用，
+        当 `suffix` 类型是 MessageSegment 时，`start` 和 `end` 参数将不其作用，
             会判断列表的最后一个消息字段是否和 `suffix` 相等。
 
         Args:
             suffix: 后缀。
             start: 开始检查位置。
             end: 停止检查位置。
 
@@ -230,61 +234,61 @@
         if isinstance(suffix, str):
             return str(self).endswith(suffix, start, end)
         elif isinstance(suffix, self._message_segment_class):
             if len(self) == 0:
                 return False
             return self[-1] == suffix
         raise TypeError(
-            f"first arg must be str or {self._message_segment_class}，not {type(suffix)}"
+            f"first arg must be str or {self._message_segment_class}, not {type(suffix)}"
         )
 
     def replace(
         self,
         old: Union[str, T_MessageSegment],
-        new: Union[str, T_MessageSegment, None],
+        new: Optional[Union[str, T_MessageSegment]],
         count: int = -1,
-    ) -> T_Message:
+    ) -> Self:
         """实现类似字符串的 `replace()` 方法。
 
         当 `old` 为 str 类型时，`new` 也必须是 str ，本方法将仅对 `is_text()` 为 True 的消息字段进行处理。
-        当 `old` 为 MessageSegment 类型时，`new` 可以是 MessageSegment 或 None，本方法将对所有消息字段进行处理，
+        当 `old` 为 MessageSegment 类型时，`new` 可以是 MessageSegment 或 None ，本方法将对所有消息字段进行处理，
             并替换符合条件的消息字段。None 表示删除匹配到的消息字段。
 
         Args:
             old: 被匹配的字符串或消息字段。
             new: 被替换为的字符串或消息字段。
             count: 替换的次数。
 
         Returns:
             替换后的消息对象。
         """
-        if type(old) == str:
-            if type(new) != str:
+        if type(old) is str:
+            if type(new) is not str:
                 raise TypeError("when type of old is str, type of new must be str.")
             return self._replace_str(old, new, count)
         elif isinstance(old, self._message_segment_class):
             if not (isinstance(new, self._message_segment_class) or new is None):
                 raise TypeError(
                     "when type of old is MessageSegment, "
                     "type of new must be MessageSegment or None."
                 )
             temp_msg = self.deepcopy()
             for index, item in enumerate(temp_msg):
                 if count == 0:
                     break
                 if item == old:
-                    temp_msg[index] = new
+                    temp_msg[index] = new  # type: ignore
                     count -= 1
             if new is None:
-                temp_msg = self.__class__(filter(lambda x: x is not None, self))
+                temp_msg = self.__class__(filter(lambda x: x is not None, self))  # type: ignore
             return temp_msg
         else:
             raise TypeError("type of old must be str or MessageSegment")
 
-    def _replace_str(self, old: str, new: str, count: int = -1) -> T_Message:
+    def _replace_str(self, old: str, new: str, count: int = -1) -> Self:
         """实现类似字符串的 `replace()` 方法。
 
         本方法将被 `replace()` 方法调用以处理 str 类型的替换，
         默认将 MessageSegment 对象的 data['text'] 视为存放纯文本的位置。
         适配器开发者可自行重写此方法以适配其他情况。
 
         Args:
@@ -293,15 +297,15 @@
             count: 替换的次数。
 
         Returns:
             替换后的消息对象。
         """
         temp_msg = self.deepcopy()
         for index, item in enumerate(temp_msg):
-            item: MessageSegment
+            item: T_MessageSegment
             if count == 0:
                 break
             if item.is_text() and old in item.data["text"]:
                 if count == -1:
                     temp_msg[index].data["text"] = item.data["text"].replace(old, new)
                 else:
                     replace_times = min(count, item.data["text"].count(old))
@@ -309,15 +313,15 @@
                         old, new, replace_times
                     )
                     count -= replace_times
         return temp_msg
 
 
 @dataclass
-class MessageSegment(Mapping, Generic[T_Message]):
+class MessageSegment(Mapping[str, Any], Generic[T_Message]):
     """消息字段。
 
     本类实现了所有映射类型的方法，这些方法全部是对 `data` 属性的操作。
     本类重写了 `+` 和 `+=` 运算符，可以直接和 Message, MessageSegment 等类型的对象执行取和运算，返回 Message 对象。
     若开发者实现了 Message 和 MessageSegment 的子类则需要重写 `_message_class()` 方法。
 
     Attributes:
@@ -331,15 +335,15 @@
     @property
     def _message_class(self) -> Type[T_Message]:
         """若开发者实现了 Message 和 MessageSegment 的子类则需要重写此方法。
 
         Returns:
             Message 类。
         """
-        return Message
+        return Message  # type: ignore
 
     def as_dict(self) -> Dict[str, Any]:
         """将当前对象解析为 Dict 对象，开发者可重写本方法以适配特殊的解析方式。
 
         Returns:
             Dict 对象。
         """
@@ -347,45 +351,45 @@
 
     def __str__(self) -> str:
         return str(self.data)
 
     def __repr__(self) -> str:
         return f"MessageSegment<{self.type}>:{str(self)}"
 
-    def __getitem__(self, key) -> Any:
+    def __getitem__(self, key: str) -> Any:
         return self.data[key]
 
-    def __setitem__(self, key, value):
+    def __setitem__(self, key: str, value: Any):
         self.data[key] = value
 
-    def __delitem__(self, key):
+    def __delitem__(self, key: str):
         del self.data[key]
 
     def __len__(self) -> int:
         return len(self.data)
 
     def __iter__(self):
         yield from self.data.__iter__()
 
-    def __contains__(self, key) -> bool:
+    def __contains__(self, key: object) -> bool:
         return key in self.data
 
-    def __eq__(self, other: T_MessageSegment) -> bool:
+    def __eq__(self, other: Self) -> bool:
         return self.type == other.type and self.data == other.data
 
-    def __ne__(self, other: T_MessageSegment) -> bool:
+    def __ne__(self, other: Self) -> bool:
         return not self.__eq__(other)
 
-    def __add__(self, other) -> T_Message:
+    def __add__(self, other: Any) -> T_Message:
         return self._message_class(self) + other
 
-    def __radd__(self, other) -> T_Message:
+    def __radd__(self, other: Any) -> T_Message:
         return self._message_class(other) + self
 
-    def get(self, key: str, default=None):
+    def get(self, key: str, default: Any = None):
         return self.data.get(key, default)
 
     def keys(self):
         return self.data.keys()
 
     def values(self):
         return self.data.values()
@@ -396,22 +400,23 @@
     def is_text(self) -> bool:
         """
         Returns:
             是否是纯文本消息字段。
         """
         return self.type == "text"
 
-    def copy(self) -> T_MessageSegment:
+    def copy(self) -> Self:
         """返回自身的浅复制。
 
         Returns:
             自身的浅复制。
         """
         return copy(self)
 
-    def deepcopy(self) -> T_MessageSegment:
+    def deepcopy(self) -> Self:
         """返回自身的深复制。
 
         Returns:
             自身的深复制。
         """
         return deepcopy(self)
+        return deepcopy(self)
```

### Comparing `alicebot-0.6.1/alicebot/plugin.py` & `alicebot-0.6.2/alicebot/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """AliceBot 插件。
 
 所有 AliceBot 插件的基类。所有用户编写的插件必须继承自 `Plugin` 类。
 """
 from enum import Enum
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Type, Generic, NoReturn, Optional
+from typing import TYPE_CHECKING, Type, Generic, NoReturn, Optional, final
 
-from alicebot.config import ConfigModel
 from alicebot.utils import is_config_class
 from alicebot.typing import T_Event, T_State, T_Config
 from alicebot.exceptions import SkipException, StopException
 
 if TYPE_CHECKING:
     from alicebot.bot import Bot
 
@@ -37,19 +36,20 @@
         __plugin_file_path__: 当插件加载类型为 `PluginLoadType.CLASS` 时为 `None`，
             否则为定义插件在的 Python 模块的位置。
     """
 
     event: T_Event
     priority: int = 0
     block: bool = False
-    Config: Type[ConfigModel]
+    Config: Type[T_Config] = type(None)  # type: ignore
 
     __plugin_load_type__: PluginLoadType
     __plugin_file_path__: Optional[str]
 
+    @final
     def __init__(self, event: T_Event):
         self.event = event
 
         if not hasattr(self, "priority"):
             self.priority = 0
         if not hasattr(self, "block"):
             self.block = False
@@ -58,45 +58,51 @@
 
         self.__post_init__()
 
     def __post_init__(self):
         """用于初始化后处理，被 `__init__()` 方法调用。"""
         pass
 
+    @final
     @property
     def name(self) -> str:
         """插件类名称。"""
         return self.__class__.__name__
 
+    @final
     @property
     def bot(self) -> "Bot":
         """机器人对象。"""
         return self.event.adapter.bot
 
+    @final
     @property
-    def config(self) -> Optional[T_Config]:
+    def config(self) -> T_Config:
         """插件配置。"""
-        config_class: ConfigModel = getattr(self, "Config", None)
-        if is_config_class(config_class):
-            return getattr(self.bot.config.plugin, config_class.__config_name__, None)
-        return None
+        if is_config_class(self.Config):
+            return getattr(self.bot.config.plugin, self.Config.__config_name__, None)  # type: ignore
+        return None  # type: ignore
 
+    @final
     def stop(self) -> NoReturn:
         """停止当前事件传播。"""
         raise StopException()
 
+    @final
     def skip(self) -> NoReturn:
         """跳过自身继续当前事件传播。"""
         raise SkipException()
 
+    @final
     @property
     def state(self) -> T_State:
         """插件状态。"""
         return self.bot.plugin_state[self.name]
 
+    @final
     @state.setter
     def state(self, value: T_State):
         self.bot.plugin_state[self.name] = value
 
     @abstractmethod
     async def handle(self) -> None:
         """处理事件的方法。当 `rule()` 方法返回 `True` 时 AliceBot 会调用此方法。每个插件必须实现此方法。"""
```

### Comparing `alicebot-0.6.1/alicebot/utils.py` & `alicebot-0.6.2/alicebot/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,74 @@
 import os
 import json
 import asyncio
 import inspect
 import os.path
-import pkgutil
 import importlib
 import traceback
 import dataclasses
 from abc import ABC
 from types import ModuleType
 from functools import partial
-from typing_extensions import ParamSpec
 from importlib.abc import MetaPathFinder
 from importlib.machinery import PathFinder
-from typing import Any, List, Type, Tuple, TypeVar, Callable, Iterable, Coroutine
+from typing_extensions import ParamSpec, TypeGuard
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    List,
+    Type,
+    Tuple,
+    Union,
+    TypeVar,
+    Callable,
+    Optional,
+    Sequence,
+    Awaitable,
+    Coroutine,
+)
 
 from alicebot.config import ConfigModel
 
+if TYPE_CHECKING:
+    from alicebot.event import Event
+
 __all__ = [
     "ModulePathFinder",
     "is_config_class",
     "get_classes_from_module",
     "get_classes_from_module_name",
-    "get_classes_from_dir",
     "DataclassEncoder",
     "samefile",
     "sync_func_wrapper",
+    "wrap_get_func",
 ]
 
 _T = TypeVar("_T")
 _P = ParamSpec("_P")
 _R = TypeVar("_R")
 
 
 class ModulePathFinder(MetaPathFinder):
     """用于查找 AliceBot 组件的元路径查找器。"""
 
     path: List[str] = []
 
-    def find_spec(self, fullname, path=None, target=None):
+    def find_spec(
+        self,
+        fullname: str,
+        path: Optional[Sequence[str]] = None,
+        target: Optional[ModuleType] = None,
+    ):
         if path is None:
             path = []
         return PathFinder.find_spec(fullname, self.path + list(path), target)
 
 
-def is_config_class(config_class: Any) -> bool:
+def is_config_class(config_class: Any) -> TypeGuard[Type[ConfigModel]]:
     """判断一个对象是否是配置类。
 
     Args:
         config_class: 待判断的对象。
 
     Returns:
         返回是否是配置类。
@@ -114,42 +134,18 @@
         # 不捕获 KeyboardInterrupt
         # 捕获 KeyboardInterrupt 会阻止用户关闭 Python 当正在导入的模块陷入死循环时
         if isinstance(e, KeyboardInterrupt):
             raise e
         raise ImportError(e, traceback.format_exc()) from e
 
 
-def get_classes_from_dir(
-    dirs: Iterable[str], super_class: Type[_T]
-) -> List[Tuple[Type[_T], ModuleType]]:
-    """从指定路径列表中的所有模块中查找指定类型的类，以 `_` 开头的插件不会被导入。路径可以是相对路径或绝对路径。
-
-    Args:
-        dirs: 储存模块的路径的列表。
-        super_class: 要查找的类的超类。
-
-    Returns:
-        返回由符合条件的类和模块组成的元组的列表。
-    """
-    classes: List[Tuple[Type[_T], ModuleType]] = []
-    for module_info in pkgutil.iter_modules(dirs):
-        if not module_info.name.startswith("_"):
-            try:
-                classes.extend(
-                    get_classes_from_module_name(module_info.name, super_class)
-                )
-            except ImportError:
-                continue
-    return classes
-
-
 class DataclassEncoder(json.JSONEncoder):
     """用于解析 MessageSegment 的 JSONEncoder 类。"""
 
-    def default(self, o):
+    def default(self, o: Any):
         if dataclasses.is_dataclass(o):
             return o.as_dict()
         return super().default(o)
 
 
 def samefile(path1: str, path2: str) -> bool:
     """一个 `os.path.samefile` 的简单包装。
@@ -188,7 +184,26 @@
 
     else:
 
         async def _wrapper(*args: _P.args, **kwargs: _P.kwargs):
             return func(*args, **kwargs)
 
     return _wrapper
+
+
+def wrap_get_func(
+    func: Optional[Callable[["Event"], Union[bool, Awaitable[bool]]]]
+) -> Callable[["Event"], Awaitable[bool]]:
+    """将 `get()` 函数接受的参数包装为一个异步函数。
+
+    Args:
+        func: `get()` 函数接受的参数。
+
+    Returns:
+        异步函数。
+    """
+    if func is None:
+        return sync_func_wrapper(lambda _: True)
+    elif not asyncio.iscoroutinefunction(func):
+        return sync_func_wrapper(func)  # type: ignore
+    else:
+        return func
```

### Comparing `alicebot-0.6.1/pyproject.toml` & `alicebot-0.6.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,90 @@
 [tool.poetry]
 name = "alicebot"
-version = "0.6.1"
+version = "0.6.2"
 description = "A simply asynchronous python chatbot framework."
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
-  "Topic :: Communications :: Chat"
+  "Topic :: Communications :: Chat",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 tomli = { version = "^2.0.0", python = "<3.11" }
 pydantic = "^1.10.0"
 aiohttp = "^3.8.0"
-loguru = "^0.6.0"
-typing-extensions = "^4.4.0"
+loguru = "^0.7.0"
+typing-extensions = "^4.5.0"
 
-[tool.poetry.dev-dependencies]
-watchfiles = "^0.18.0"
+[tool.poetry.group.dev.dependencies]
+watchfiles = "^0.19.0"
 sophia-doc = "^0.1.0"
 alicebot-adapter-cqhttp = { path = "./packages/alicebot-adapter-cqhttp", develop = true }
 alicebot-adapter-mirai = { path = "./packages/alicebot-adapter-mirai", develop = true }
 alicebot-adapter-dingtalk = { path = "./packages/alicebot-adapter-dingtalk", develop = true }
 alicebot-adapter-apscheduler = { path = "./packages/alicebot-adapter-apscheduler", develop = true }
-black = "^22.10.0"
-isort = "^5.10.0"
-pre-commit = "^2.19.0"
+black = "^23.1.0"
+isort = "^5.12.0"
+pre-commit = "^3.1.0"
 pre-commit-hooks = "^4.4.0"
+tomlkit = "^0.11.7"
 
 [tool.poetry.extras]
 cqhttp = ["alicebot-adapter-cqhttp"]
 mirai = ["alicebot-adapter-mirai"]
 dingtalk = ["alicebot-adapter-dingtalk"]
 apscheduler = ["alicebot-adapter-apscheduler"]
 hot_reload = ["watchfiles"]
 all = [
   "alicebot-adapter-cqhttp",
   "alicebot-adapter-mirai",
   "alicebot-adapter-dingtalk",
   "alicebot-adapter-apscheduler",
-  "watchfiles"
+  "watchfiles",
 ]
 
-[tool.pydantic-pycharm-plugin]
-ignore-init-method-arguments = true
-
 [tool.black]
-target-version = ["py38", "py39", "py310"]
+target-version = ["py38", "py39", "py310", "py311"]
 
 [tool.isort]
 profile = "black"
 length_sort = true
 skip_gitignore = true
 force_sort_within_sections = true
 src_paths = ["alicebot", "tests"]
 extra_standard_library = ["typing_extensions"]
 
+[tool.pyright]
+exclude = ["tests"]
+pythonVersion = "3.8"
+pythonPlatform = "All"
+typeCheckingMode = "strict"
+reportImportCycles = false
+reportIncompatibleMethodOverride = false
+reportMissingTypeArgument = false
+reportMissingTypeStubs = false
+reportUnknownArgumentType = false
+reportUnknownLambdaType = false
+reportUnknownMemberType = false
+reportUnknownParameterType = false
+reportUnknownVariableType = false
+reportUnnecessaryIsInstance = false
+
+[tool.pydantic-pycharm-plugin]
+ignore-init-method-arguments = true
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `alicebot-0.6.1/setup.py` & `alicebot-0.6.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,164 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: alicebot
+Version: 0.6.2
+Summary: A simply asynchronous python chatbot framework.
+Home-page: https://docs.alicebot.dev/
+License: MIT
+Keywords: bot,chatbot,qq,qqbot,cqhttp,coolq
+Author: st1020
+Author-email: stone_1020@qq.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Framework :: AsyncIO
+Classifier: Framework :: Robot Framework
+Classifier: Framework :: Robot Framework :: Library
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Communications :: Chat
+Provides-Extra: all
+Provides-Extra: apscheduler
+Provides-Extra: cqhttp
+Provides-Extra: dingtalk
+Provides-Extra: hot-reload
+Provides-Extra: mirai
+Requires-Dist: aiohttp (>=3.8.0,<4.0.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Requires-Dist: tomli (>=2.0.0,<3.0.0) ; python_version < "3.11"
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Project-URL: Documentation, https://docs.alicebot.dev/
+Project-URL: Repository, https://github.com/AliceBotProject/alicebot
+Description-Content-Type: text/markdown
+
+<div align="center">
+  <a href="https://docs.alicebot.dev/"><img src="https://raw.githubusercontent.com/AliceBotProject/alicebot/master/docs/public/logo.png" width="200" height="200" alt="logo"></a>
+
+# AliceBot
+
+**简单的 Python 异步多后端机器人框架**
+
+</div>
+
+<div align="center">
+  <a href="https://raw.githubusercontent.com/AliceBotProject/alicebot/master/LICENSE">
+    <img src="https://img.shields.io/github/license/AliceBotProject/alicebot" alt="license">
+  </a>
+  <a href="https://pypi.python.org/pypi/alicebot">
+    <img src="https://img.shields.io/pypi/v/alicebot" alt="pypi">
+  </a>
+  <a href="https://pypi.python.org/pypi/alicebot">
+    <img src="https://img.shields.io/pypi/pyversions/alicebot" alt="pypi">
+  </a>
+  <a href="https://github.com/AliceBotProject/alicebot/">
+    <img src="https://img.shields.io/github/stars/AliceBotProject/alicebot?style=social" alt="github">
+  </a>
+  <br />
+  <a href="https://jq.qq.com/?_wv=1027&k=ZbE3p6tq">
+    <img src="https://img.shields.io/badge/QQ%E7%BE%A4-674802046-orange" alt="qq-group">
+  </a>
+</div>
+
+<p align="center">
+  <a href="https://docs.alicebot.dev/">文档</a>
+  ·
+  <a href="https://docs.alicebot.dev/guide/">指南</a>
+  ·
+  <a href="https://docs.alicebot.dev/guide/">API 参考</a>
+  ·
+  <a href="https://github.com/AliceBotProject/alicebot-example">示例</a>
+</p>
+
+## 简介
+
+AliceBot 是一个简单的 Python 异步多后端机器人框架，支持多种协议适配，可以轻松地编写易于学习和使用的插件来拓展其功能。
+
+本项目受到了 [NoneBot](https://github.com/nonebot/nonebot2/) 项目的启发，您可以在 [对比](#对比) 小节中查看这两个项目的异同，以便您选择更适合自己的机器人框架。
+
+## 特点
+
+AliceBot 使用了非常灵活且易于使用的插件编写方式，您只需要编写两个方法即可实现一个功能强大的插件。
+
+AliceBot 的适配协议并不与任何一种库或网络协议绑定，您可以自由选择或编写适合您的适配器。
+
+目前 AliceBot 官方维护了以下协议适配：
+
+- [OneBot (CQHTTP) 协议](https://github.com/botuniverse/onebot) （支持QQ等）[ws](https://github.com/botuniverse/onebot-11/blob/master/communication/ws.md) 和 [ws-reverse](https://github.com/botuniverse/onebot-11/blob/master/communication/ws-reverse.md) 连接方式
+- [mirai-api-http 协议](https://github.com/project-mirai/mirai-api-http) 2.0+ [ws](https://github.com/project-mirai/mirai-api-http/blob/master/docs/adapter/WebsocketAdapter.md) 和 [reverse-ws](https://github.com/project-mirai/mirai-api-http/blob/master/docs/adapter/ReverseWebsocketAdapter.md) 连接方式
+- [钉钉](https://developers.dingtalk.com/document/robots/robot-overview) 企业机器人的 outgoing （回调）连接方式
+
+更多协议正在适配中 ...
+
+## 即刻开始
+
+1. 安装：
+
+   ```bash
+   pip install alicebot[all]
+   ```
+
+2. 第一个 AliceBot 项目：
+
+   ```python
+   from alicebot import Bot
+   
+   bot = Bot()
+   bot.load_adapters("alicebot.adapter.cqhttp")
+   
+   bot.run()
+   ```
+
+3. 第一个 AliceBot 插件：
+
+   ```python
+   from alicebot import Plugin
+   
+   
+   class Echo(Plugin):
+       async def handle(self) -> None:
+           await self.event.reply(self.event.message.replace("echo ", ""))
+   
+       async def rule(self) -> bool:
+           if self.event.adapter.name != "cqhttp":
+               return False
+           if self.event.type != "message":
+               return False
+           return self.event.message.startswith("echo ")
+   ```
+
+更多信息请参阅 AliceBot [文档](https://docs.alicebot.dev/)。
+
+## 对比
+
+本项目受到了 [NoneBot](https://github.com/nonebot/nonebot2/) 项目的启发，以下简单介绍两者的异同。
+
+相同点：
+
+- 两者都是使用 Python 编写的，使用了协程异步的高性能机器人框架。
+- 两者都支持多种协议。
+- 两者都会对机器人收到的事件进行解析和处理，并按优先级分发给插件（事件响应器）来完成具体的功能。
+- 两者都基于 MIT 协议开源，这意味着您可以在遵循协议的前提下任意使用本项目。
+
+不同点：
+
+- 总的来说，NoneBot 是一个较为全面的机器人框架，而 AliceBot 是一个小巧简洁的机器人框架，它不包含一些复杂的高级特性，但更加灵活且易于学习。
+- NoneBot 在实现上与 WebSocket 通讯协议深度绑定，它需要一个支持 ASGI 服务器协议的驱动框架，而 AliceBot 并不与任何协议绑定，它甚至可以用来驱动您的树莓派智能音箱。当然，如果您只需要一个支持常见网络聊天工具的机器人框架的话，它们并没有什么区别。
+- NoneBot 提供了很多预设规则和权限控制机制，而 AliceBot 则没有提供，由于插件编写方式的不同，AliceBot 选择给您最大的自由，您需要自行编写插件在何时运行的方法（`rule()` 方法），这在绝大部份情况下并不会造成您编写更多的代码或是影响插件的可读性，自行实现也不会非常困难，但如果您真的需要这些高级功能又不想自己实现的话，NoneBot 提供了更好的选择。
+- NoneBot 拥有相对庞大的用户基数和社区规模，也拥有数量众多的插件，而 AliceBot 则是一个新生项目，这意味着如果您使用 NoneBot 您可能会更加容易找到已经编写完毕的您感兴趣的插件，并且您当您遇到问题时也能够更快地查找到相关资料或者获得解答。
+- NoneBot 相对较为庞大，封装相对较多，完全学习理解需要一定时间，而 AliceBot 小巧简洁，封装较少，很容易掌握。
+
+总而言之，两者有着各自的特点，您可以根据需要选用。
 
-packages = \
-['alicebot', 'alicebot.adapter']
+作者就是在使用 NoneBot 时觉得插件编写不是很易用，于是萌发了编写一个新的机器人框架的想法，AliceBot 就这样诞生了。
 
-package_data = \
-{'': ['*']}
+## 许可证
 
-install_requires = \
-['aiohttp>=3.8.0,<4.0.0',
- 'loguru>=0.6.0,<0.7.0',
- 'pydantic>=1.10.0,<2.0.0',
- 'typing-extensions>=4.4.0,<5.0.0']
-
-extras_require = \
-{':python_version < "3.11"': ['tomli>=2.0.0,<3.0.0']}
-
-setup_kwargs = {
-    'name': 'alicebot',
-    'version': '0.6.1',
-    'description': 'A simply asynchronous python chatbot framework.',
-    'long_description': '<div align="center">\n  <a href="https://docs.alicebot.dev/"><img src="https://raw.githubusercontent.com/st1020/alicebot/master/docs/public/logo.png" width="200" height="200" alt="logo"></a>\n\n# AliceBot\n\n**简单的 Python 异步多后端机器人框架**\n\n</div>\n\n<div align="center">\n  <a href="https://raw.githubusercontent.com/st1020/alicebot/master/LICENSE">\n    <img src="https://img.shields.io/github/license/st1020/alicebot" alt="license">\n  </a>\n  <a href="https://pypi.python.org/pypi/alicebot">\n    <img src="https://img.shields.io/pypi/v/alicebot" alt="pypi">\n  </a>\n  <a href="https://pypi.python.org/pypi/alicebot">\n    <img src="https://img.shields.io/pypi/pyversions/alicebot" alt="pypi">\n  </a>\n  <a href="https://github.com/st1020/alicebot/">\n    <img src="https://img.shields.io/github/stars/st1020/alicebot?style=social" alt="github">\n  </a>\n  <br />\n  <a href="https://jq.qq.com/?_wv=1027&k=ZbE3p6tq">\n    <img src="https://img.shields.io/badge/QQ%E7%BE%A4-674802046-orange" alt="qq-group">\n  </a>\n</div>\n\n<p align="center">\n  <a href="https://docs.alicebot.dev/">文档</a>\n  ·\n  <a href="https://docs.alicebot.dev/guide/">指南</a>\n  ·\n  <a href="https://docs.alicebot.dev/guide/">API 参考</a>\n  ·\n  <a href="https://github.com/st1020/alicebot-example">示例</a>\n</p>\n\n## 简介\n\nAliceBot 是一个简单的 Python 异步多后端机器人框架，支持多种协议适配，可以轻松地编写易于学习和使用的插件来拓展其功能。\n\n本项目受到了 [NoneBot](https://github.com/nonebot/nonebot2/) 项目的启发，您可以在 [对比](#对比) 小节中查看这两个项目的异同，以便您选择更适合自己的机器人框架。\n\n## 特点\n\nAliceBot 使用了非常灵活且易于使用的插件编写方式，您只需要编写两个方法即可实现一个功能强大的插件。\n\nAliceBot 的适配协议并不与任何一种库或网络协议绑定，您可以自由选择或编写适合您的适配器。\n\n目前 AliceBot 官方维护了以下协议适配：\n\n- [OneBot (CQHTTP) 协议](https://github.com/botuniverse/onebot) （支持QQ等）[ws](https://github.com/botuniverse/onebot-11/blob/master/communication/ws.md) 和 [ws-reverse](https://github.com/botuniverse/onebot-11/blob/master/communication/ws-reverse.md) 连接方式\n- [mirai-api-http 协议](https://github.com/project-mirai/mirai-api-http) 2.0+ [ws](https://github.com/project-mirai/mirai-api-http/blob/master/docs/adapter/WebsocketAdapter.md) 和 [reverse-ws](https://github.com/project-mirai/mirai-api-http/blob/master/docs/adapter/ReverseWebsocketAdapter.md) 连接方式\n- [钉钉](https://developers.dingtalk.com/document/robots/robot-overview) 企业机器人的 outgoing （回调）连接方式\n\n更多协议正在适配中 ...\n\n## 即刻开始\n\n1. 安装：\n\n   ```bash\n   pip install alicebot[all]\n   ```\n\n2. 第一个 AliceBot 项目：\n\n   ```python\n   from alicebot import Bot\n   \n   bot = Bot()\n   bot.load_adapters("alicebot.adapter.cqhttp")\n   \n   bot.run()\n   ```\n\n3. 第一个 AliceBot 插件：\n\n   ```python\n   from alicebot import Plugin\n   \n   \n   class Echo(Plugin):\n       async def handle(self) -> None:\n           await self.event.reply(self.event.message.replace("echo ", ""))\n   \n       async def rule(self) -> bool:\n           if self.event.adapter.name != "cqhttp":\n               return False\n           if self.event.type != "message":\n               return False\n           return self.event.message.startswith("echo ")\n   ```\n\n更多信息请参阅 AliceBot [文档](https://docs.alicebot.dev/)。\n\n## 对比\n\n本项目受到了 [NoneBot](https://github.com/nonebot/nonebot2/) 项目的启发，以下简单介绍两者的异同。\n\n相同点：\n\n- 两者都是使用 Python 编写的，使用了协程异步的高性能机器人框架。\n- 两者都支持多种协议。\n- 两者都会对机器人收到的事件进行解析和处理，并按优先级分发给插件（事件响应器）来完成具体的功能。\n- 两者都基于 MIT 协议开源，这意味着您可以在遵循协议的前提下任意使用本项目。\n\n不同点：\n\n- 总的来说，NoneBot 是一个较为全面的机器人框架，而 AliceBot 是一个小巧简洁的机器人框架，它不包含一些复杂的高级特性，但更加灵活且易于学习。\n- NoneBot 在实现上与 WebSocket 通讯协议深度绑定，它需要一个支持 ASGI 服务器协议的驱动框架，而 AliceBot 并不与任何协议绑定，它甚至可以用来驱动您的树莓派智能音箱。当然，如果您只需要一个支持常见网络聊天工具的机器人框架的话，它们并没有什么区别。\n- NoneBot 提供了很多预设规则和权限控制机制，而 AliceBot 则没有提供，由于插件编写方式的不同，AliceBot 选择给您最大的自由，您需要自行编写插件在何时运行的方法（`rule()` 方法），这在绝大部份情况下并不会造成您编写更多的代码或是影响插件的可读性，自行实现也不会非常困难，但如果您真的需要这些高级功能又不想自己实现的话，NoneBot 提供了更好的选择。\n- NoneBot 拥有相对庞大的用户基数和社区规模，也拥有数量众多的插件，而 AliceBot 则是一个新生项目，这意味着如果您使用 NoneBot 您可能会更加容易找到已经编写完毕的您感兴趣的插件，并且您当您遇到问题时也能够更快地查找到相关资料或者获得解答。\n- NoneBot 相对较为庞大，封装相对较多，完全学习理解需要一定时间，而 AliceBot 小巧简洁，封装较少，很容易掌握。\n\n总而言之，两者有着各自的特点，您可以根据需要选用。\n\n作者就是在使用 NoneBot 时觉得插件编写不是很易用，于是萌发了编写一个新的机器人框架的想法，AliceBot 就这样诞生了。\n\n## 许可证\n\nAliceBot 采用 MIT 许可证开放源代码。\n\n本项目的图标由 迷糊小梦神 绘制，作为本项目的一部分，使用与本项目相同的许可证开放使用。\n',
-    'author': 'st1020',
-    'author_email': 'stone_1020@qq.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://docs.alicebot.dev/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
+AliceBot 采用 MIT 许可证开放源代码。
 
+本项目的图标由 迷糊小梦神 绘制，作为本项目的一部分，使用与本项目相同的许可证开放使用。
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,80 +1,85 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['alicebot',
-'alicebot.adapter'] package_data = \ {'': ['*']} install_requires = \
-['aiohttp>=3.8.0,<4.0.0', 'loguru>=0.6.0,<0.7.0', 'pydantic>=1.10.0,<2.0.0',
-'typing-extensions>=4.4.0,<5.0.0'] extras_require = \ {':python_version <
-"3.11"': ['tomli>=2.0.0,<3.0.0']} setup_kwargs = { 'name': 'alicebot',
-'version': '0.6.1', 'description': 'A simply asynchronous python chatbot
-framework.', 'long_description': '
-                 \n [logo]\n\n# AliceBot\n\n**ç®åç Python
-                     å¼æ­¥å¤åç«¯æºå¨äººæ¡æ¶**\n\n
-\n\n
-       \n \n_[license]\n\n \n_[pypi]\n\n \n_[pypi]\n\n \n_[github]\n\n
-                             \n \n_[qq-group]\n\n
-\n\n
-           \n ææ¡£\n Â·\n æå\n Â·\n API_åè\n Â·\n ç¤ºä¾\n
-\n\n## ç®ä»\n\nAliceBot æ¯ä¸ä¸ªç®åç Python
-å¼æ­¥å¤åç«¯æºå¨äººæ¡æ¶ï¼æ¯æå¤ç§åè®®ééï¼å¯ä»¥è½»æ¾å°ç¼åæäºå­¦ä¹ åä½¿ç¨çæä»¶æ¥æå±å¶åè½ã\n\næ¬é¡¹ç®åå°äº
-[NoneBot](https://github.com/nonebot/nonebot2/) é¡¹ç®çå¯åï¼æ¨å¯ä»¥å¨
-[å¯¹æ¯](#å¯¹æ¯)
-å°èä¸­æ¥çè¿ä¸¤ä¸ªé¡¹ç®çå¼åï¼ä»¥ä¾¿æ¨éæ©æ´éåèªå·±çæºå¨äººæ¡æ¶ã\n\n##
-ç¹ç¹\n\nAliceBot
-ä½¿ç¨äºéå¸¸çµæ´»ä¸æäºä½¿ç¨çæä»¶ç¼åæ¹å¼ï¼æ¨åªéè¦ç¼åä¸¤ä¸ªæ¹æ³å³å¯å®ç°ä¸ä¸ªåè½å¼ºå¤§çæä»¶ã\n\nAliceBot
-çééåè®®å¹¶ä¸ä¸ä»»ä½ä¸ç§åºæç½ç»åè®®ç»å®ï¼æ¨å¯ä»¥èªç±éæ©æç¼åéåæ¨çééå¨ã\n\nç®å
-AliceBot å®æ¹ç»´æ¤äºä»¥ä¸åè®®ééï¼\n\n- [OneBot (CQHTTP) åè®®]
+Metadata-Version: 2.1 Name: alicebot Version: 0.6.2 Summary: A simply
+asynchronous python chatbot framework. Home-page: https://docs.alicebot.dev/
+License: MIT Keywords: bot,chatbot,qq,qqbot,cqhttp,coolq Author: st1020 Author-
+email: stone_1020@qq.com Requires-Python: >=3.8,<4.0 Classifier: Development
+Status :: 3 - Alpha Classifier: Framework :: AsyncIO Classifier: Framework ::
+Robot Framework Classifier: Framework :: Robot Framework :: Library Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3 Classifier: Topic :: Communications :: Chat Provides-Extra: all
+Provides-Extra: apscheduler Provides-Extra: cqhttp Provides-Extra: dingtalk
+Provides-Extra: hot-reload Provides-Extra: mirai Requires-Dist: aiohttp
+(>=3.8.0,<4.0.0) Requires-Dist: loguru (>=0.7.0,<0.8.0) Requires-Dist: pydantic
+(>=1.10.0,<2.0.0) Requires-Dist: tomli (>=2.0.0,<3.0.0) ; python_version <
+"3.11" Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) Project-URL:
+Documentation, https://docs.alicebot.dev/ Project-URL: Repository, https://
+github.com/AliceBotProject/alicebot Description-Content-Type: text/markdown
+     [logo] # AliceBot **ç®åç Python å¼æ­¥å¤åç«¯æºå¨äººæ¡æ¶**
+                       [license] [pypi] [pypi] [github]
+                                  [qq-group]
+                   ææ¡£ Â· æå Â· API_åè Â· ç¤ºä¾
+## ç®ä» AliceBot æ¯ä¸ä¸ªç®åç Python
+å¼æ­¥å¤åç«¯æºå¨äººæ¡æ¶ï¼æ¯æå¤ç§åè®®ééï¼å¯ä»¥è½»æ¾å°ç¼åæäºå­¦ä¹ åä½¿ç¨çæä»¶æ¥æå±å¶åè½ã
+æ¬é¡¹ç®åå°äº [NoneBot](https://github.com/nonebot/nonebot2/
+) é¡¹ç®çå¯åï¼æ¨å¯ä»¥å¨ [å¯¹æ¯](#å¯¹æ¯)
+å°èä¸­æ¥çè¿ä¸¤ä¸ªé¡¹ç®çå¼åï¼ä»¥ä¾¿æ¨éæ©æ´éåèªå·±çæºå¨äººæ¡æ¶ã
+## ç¹ç¹ AliceBot
+ä½¿ç¨äºéå¸¸çµæ´»ä¸æäºä½¿ç¨çæä»¶ç¼åæ¹å¼ï¼æ¨åªéè¦ç¼åä¸¤ä¸ªæ¹æ³å³å¯å®ç°ä¸ä¸ªåè½å¼ºå¤§çæä»¶ã
+AliceBot
+çééåè®®å¹¶ä¸ä¸ä»»ä½ä¸ç§åºæç½ç»åè®®ç»å®ï¼æ¨å¯ä»¥èªç±éæ©æç¼åéåæ¨çééå¨ã
+ç®å AliceBot å®æ¹ç»´æ¤äºä»¥ä¸åè®®ééï¼ - [OneBot (CQHTTP) åè®®]
 (https://github.com/botuniverse/onebot) ï¼æ¯æQQç­ï¼[ws](https://
 github.com/botuniverse/onebot-11/blob/master/communication/ws.md) å [ws-
 reverse](https://github.com/botuniverse/onebot-11/blob/master/communication/ws-
-reverse.md) è¿æ¥æ¹å¼\n- [mirai-api-http åè®®](https://github.com/project-
+reverse.md) è¿æ¥æ¹å¼ - [mirai-api-http åè®®](https://github.com/project-
 mirai/mirai-api-http) 2.0+ [ws](https://github.com/project-mirai/mirai-api-
 http/blob/master/docs/adapter/WebsocketAdapter.md) å [reverse-ws](https://
 github.com/project-mirai/mirai-api-http/blob/master/docs/adapter/
-ReverseWebsocketAdapter.md) è¿æ¥æ¹å¼\n- [éé](https://
+ReverseWebsocketAdapter.md) è¿æ¥æ¹å¼ - [éé](https://
 developers.dingtalk.com/document/robots/robot-overview) ä¼ä¸æºå¨äººç
-outgoing ï¼åè°ï¼è¿æ¥æ¹å¼\n\næ´å¤åè®®æ­£å¨ééä¸­ ...\n\n##
-å³å»å¼å§\n\n1. å®è£ï¼\n\n ```bash\n pip install alicebot[all]\n
-```\n\n2. ç¬¬ä¸ä¸ª AliceBot é¡¹ç®ï¼\n\n ```python\n from alicebot import
-Bot\n \n bot = Bot()\n bot.load_adapters("alicebot.adapter.cqhttp")\n \n
-bot.run()\n ```\n\n3. ç¬¬ä¸ä¸ª AliceBot æä»¶ï¼\n\n ```python\n from
-alicebot import Plugin\n \n \n class Echo(Plugin):\n async def handle(self) -
-> None:\n await self.event.reply(self.event.message.replace("echo ", ""))\n \n
-async def rule(self) -> bool:\n if self.event.adapter.name != "cqhttp":\n
-return False\n if self.event.type != "message":\n return False\n return
-self.event.message.startswith("echo ")\n ```\n\næ´å¤ä¿¡æ¯è¯·åé AliceBot
-[ææ¡£](https://docs.alicebot.dev/)ã\n\n## å¯¹æ¯\n\næ¬é¡¹ç®åå°äº
-[NoneBot](https://github.com/nonebot/nonebot2/
-) é¡¹ç®çå¯åï¼ä»¥ä¸ç®åä»ç»ä¸¤èçå¼åã\n\nç¸åç¹ï¼\n\n-
+outgoing ï¼åè°ï¼è¿æ¥æ¹å¼ æ´å¤åè®®æ­£å¨ééä¸­ ... ##
+å³å»å¼å§ 1. å®è£ï¼ ```bash pip install alicebot[all] ``` 2. ç¬¬ä¸ä¸ª
+AliceBot é¡¹ç®ï¼ ```python from alicebot import Bot bot = Bot()
+bot.load_adapters("alicebot.adapter.cqhttp") bot.run() ``` 3. ç¬¬ä¸ä¸ª
+AliceBot æä»¶ï¼ ```python from alicebot import Plugin class Echo(Plugin):
+async def handle(self) -> None: await self.event.reply
+(self.event.message.replace("echo ", "")) async def rule(self) -> bool: if
+self.event.adapter.name != "cqhttp": return False if self.event.type !=
+"message": return False return self.event.message.startswith("echo ") ```
+æ´å¤ä¿¡æ¯è¯·åé AliceBot [ææ¡£](https://docs.alicebot.dev/)ã ##
+å¯¹æ¯ æ¬é¡¹ç®åå°äº [NoneBot](https://github.com/nonebot/nonebot2/
+) é¡¹ç®çå¯åï¼ä»¥ä¸ç®åä»ç»ä¸¤èçå¼åã ç¸åç¹ï¼ -
 ä¸¤èé½æ¯ä½¿ç¨ Python
-ç¼åçï¼ä½¿ç¨äºåç¨å¼æ­¥çé«æ§è½æºå¨äººæ¡æ¶ã\n-
-ä¸¤èé½æ¯æå¤ç§åè®®ã\n-
-ä¸¤èé½ä¼å¯¹æºå¨äººæ¶å°çäºä»¶è¿è¡è§£æåå¤çï¼å¹¶æä¼åçº§ååç»æä»¶ï¼äºä»¶ååºå¨ï¼æ¥å®æå·ä½çåè½ã\n-
-ä¸¤èé½åºäº MIT
-åè®®å¼æºï¼è¿æå³çæ¨å¯ä»¥å¨éµå¾ªåè®®çåæä¸ä»»æä½¿ç¨æ¬é¡¹ç®ã\n\nä¸åç¹ï¼\n\n-
-æ»çæ¥è¯´ï¼NoneBot æ¯ä¸ä¸ªè¾ä¸ºå¨é¢çæºå¨äººæ¡æ¶ï¼è AliceBot
-æ¯ä¸ä¸ªå°å·§ç®æ´çæºå¨äººæ¡æ¶ï¼å®ä¸åå«ä¸äºå¤æçé«çº§ç¹æ§ï¼ä½æ´å çµæ´»ä¸æäºå­¦ä¹ ã\n-
-NoneBot å¨å®ç°ä¸ä¸ WebSocket
+ç¼åçï¼ä½¿ç¨äºåç¨å¼æ­¥çé«æ§è½æºå¨äººæ¡æ¶ã -
+ä¸¤èé½æ¯æå¤ç§åè®®ã -
+ä¸¤èé½ä¼å¯¹æºå¨äººæ¶å°çäºä»¶è¿è¡è§£æåå¤çï¼å¹¶æä¼åçº§ååç»æä»¶ï¼äºä»¶ååºå¨ï¼æ¥å®æå·ä½çåè½ã
+- ä¸¤èé½åºäº MIT
+åè®®å¼æºï¼è¿æå³çæ¨å¯ä»¥å¨éµå¾ªåè®®çåæä¸ä»»æä½¿ç¨æ¬é¡¹ç®ã
+ä¸åç¹ï¼ - æ»çæ¥è¯´ï¼NoneBot
+æ¯ä¸ä¸ªè¾ä¸ºå¨é¢çæºå¨äººæ¡æ¶ï¼è AliceBot
+æ¯ä¸ä¸ªå°å·§ç®æ´çæºå¨äººæ¡æ¶ï¼å®ä¸åå«ä¸äºå¤æçé«çº§ç¹æ§ï¼ä½æ´å çµæ´»ä¸æäºå­¦ä¹ ã
+- NoneBot å¨å®ç°ä¸ä¸ WebSocket
 éè®¯åè®®æ·±åº¦ç»å®ï¼å®éè¦ä¸ä¸ªæ¯æ ASGI
 æå¡å¨åè®®çé©±å¨æ¡æ¶ï¼è AliceBot
-å¹¶ä¸ä¸ä»»ä½åè®®ç»å®ï¼å®çè³å¯ä»¥ç¨æ¥é©±å¨æ¨çæ èæ´¾æºè½é³ç®±ãå½ç¶ï¼å¦ææ¨åªéè¦ä¸ä¸ªæ¯æå¸¸è§ç½ç»èå¤©å·¥å·çæºå¨äººæ¡æ¶çè¯ï¼å®ä»¬å¹¶æ²¡æä»ä¹åºå«ã\n-
-NoneBot æä¾äºå¾å¤é¢è®¾è§ååæéæ§å¶æºå¶ï¼è AliceBot
+å¹¶ä¸ä¸ä»»ä½åè®®ç»å®ï¼å®çè³å¯ä»¥ç¨æ¥é©±å¨æ¨çæ èæ´¾æºè½é³ç®±ãå½ç¶ï¼å¦ææ¨åªéè¦ä¸ä¸ªæ¯æå¸¸è§ç½ç»èå¤©å·¥å·çæºå¨äººæ¡æ¶çè¯ï¼å®ä»¬å¹¶æ²¡æä»ä¹åºå«ã
+- NoneBot æä¾äºå¾å¤é¢è®¾è§ååæéæ§å¶æºå¶ï¼è AliceBot
 åæ²¡ææä¾ï¼ç±äºæä»¶ç¼åæ¹å¼çä¸åï¼AliceBot
 éæ©ç»æ¨æå¤§çèªç±ï¼æ¨éè¦èªè¡ç¼åæä»¶å¨ä½æ¶è¿è¡çæ¹æ³ï¼`rule
 ()`
 æ¹æ³ï¼ï¼è¿å¨ç»å¤§é¨ä»½æåµä¸å¹¶ä¸ä¼é ææ¨ç¼åæ´å¤çä»£ç ææ¯å½±åæä»¶çå¯è¯»æ§ï¼èªè¡å®ç°ä¹ä¸ä¼éå¸¸å°é¾ï¼ä½å¦ææ¨ççéè¦è¿äºé«çº§åè½åä¸æ³èªå·±å®ç°çè¯ï¼NoneBot
-æä¾äºæ´å¥½çéæ©ã\n- NoneBot
+æä¾äºæ´å¥½çéæ©ã - NoneBot
 æ¥æç¸å¯¹åºå¤§çç¨æ·åºæ°åç¤¾åºè§æ¨¡ï¼ä¹æ¥ææ°éä¼å¤çæä»¶ï¼è
 AliceBot åæ¯ä¸ä¸ªæ°çé¡¹ç®ï¼è¿æå³çå¦ææ¨ä½¿ç¨ NoneBot
-æ¨å¯è½ä¼æ´å å®¹ææ¾å°å·²ç»ç¼åå®æ¯çæ¨æå´è¶£çæä»¶ï¼å¹¶ä¸æ¨å½æ¨éå°é®é¢æ¶ä¹è½å¤æ´å¿«å°æ¥æ¾å°ç¸å³èµææèè·å¾è§£ç­ã\n-
-NoneBot
+æ¨å¯è½ä¼æ´å å®¹ææ¾å°å·²ç»ç¼åå®æ¯çæ¨æå´è¶£çæä»¶ï¼å¹¶ä¸æ¨å½æ¨éå°é®é¢æ¶ä¹è½å¤æ´å¿«å°æ¥æ¾å°ç¸å³èµææèè·å¾è§£ç­ã
+- NoneBot
 ç¸å¯¹è¾ä¸ºåºå¤§ï¼å°è£ç¸å¯¹è¾å¤ï¼å®å¨å­¦ä¹ çè§£éè¦ä¸å®æ¶é´ï¼è
-AliceBot
-å°å·§ç®æ´ï¼å°è£è¾å°ï¼å¾å®¹æææ¡ã\n\næ»èè¨ä¹ï¼ä¸¤èæçåèªçç¹ç¹ï¼æ¨å¯ä»¥æ ¹æ®éè¦éç¨ã\n\nä½èå°±æ¯å¨ä½¿ç¨
-NoneBot
+AliceBot å°å·§ç®æ´ï¼å°è£è¾å°ï¼å¾å®¹æææ¡ã
+æ»èè¨ä¹ï¼ä¸¤èæçåèªçç¹ç¹ï¼æ¨å¯ä»¥æ ¹æ®éè¦éç¨ã
+ä½èå°±æ¯å¨ä½¿ç¨ NoneBot
 æ¶è§å¾æä»¶ç¼åä¸æ¯å¾æç¨ï¼äºæ¯èåäºç¼åä¸ä¸ªæ°çæºå¨äººæ¡æ¶çæ³æ³ï¼AliceBot
-å°±è¿æ ·è¯çäºã\n\n## è®¸å¯è¯\n\nAliceBot éç¨ MIT
-è®¸å¯è¯å¼æ¾æºä»£ç ã\n\næ¬é¡¹ç®çå¾æ ç± è¿·ç³å°æ¢¦ç¥
-ç»å¶ï¼ä½ä¸ºæ¬é¡¹ç®çä¸é¨åï¼ä½¿ç¨ä¸æ¬é¡¹ç®ç¸åçè®¸å¯è¯å¼æ¾ä½¿ç¨ã\n',
-'author': 'st1020', 'author_email': 'stone_1020@qq.com', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://docs.alicebot.dev/', 'packages':
-packages, 'package_data': package_data, 'install_requires': install_requires,
-'extras_require': extras_require, 'python_requires': '>=3.8,<4.0', } setup
-(**setup_kwargs)
+å°±è¿æ ·è¯çäºã ## è®¸å¯è¯ AliceBot éç¨ MIT
+è®¸å¯è¯å¼æ¾æºä»£ç ã æ¬é¡¹ç®çå¾æ ç± è¿·ç³å°æ¢¦ç¥
+ç»å¶ï¼ä½ä¸ºæ¬é¡¹ç®çä¸é¨åï¼ä½¿ç¨ä¸æ¬é¡¹ç®ç¸åçè®¸å¯è¯å¼æ¾ä½¿ç¨ã
```

