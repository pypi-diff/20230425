# Comparing `tmp/alicebot_adapter_apscheduler-0.6.0.tar.gz` & `tmp/alicebot_adapter_apscheduler-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicebot_adapter_apscheduler-0.6.0.tar", max compression
+gzip compressed data, was "alicebot_adapter_apscheduler-0.6.2.tar", max compression
```

## Comparing `alicebot_adapter_apscheduler-0.6.0.tar` & `alicebot_adapter_apscheduler-0.6.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0      260 2022-08-21 12:26:21.845204 alicebot_adapter_apscheduler-0.6.0/README.md
--rw-r--r--   0        0        0     4684 2022-11-24 16:11:09.367608 alicebot_adapter_apscheduler-0.6.0/alicebot/adapter/apscheduler/__init__.py
--rw-r--r--   0        0        0      380 2022-11-24 15:19:07.995936 alicebot_adapter_apscheduler-0.6.0/alicebot/adapter/apscheduler/config.py
--rw-r--r--   0        0        0      938 2022-11-26 13:42:49.654280 alicebot_adapter_apscheduler-0.6.0/alicebot/adapter/apscheduler/event.py
--rw-r--r--   0        0        0     1362 2022-11-26 15:08:57.866397 alicebot_adapter_apscheduler-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 alicebot_adapter_apscheduler-0.6.0/setup.py
--rw-r--r--   0        0        0     1394 1970-01-01 00:00:00.000000 alicebot_adapter_apscheduler-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      269 2023-04-25 11:14:36.277730 alicebot_adapter_apscheduler-0.6.2/README.md
+-rw-r--r--   0        0        0     4787 2023-04-25 11:14:36.277730 alicebot_adapter_apscheduler-0.6.2/alicebot/adapter/apscheduler/__init__.py
+-rw-r--r--   0        0        0      380 2023-04-25 11:14:36.277730 alicebot_adapter_apscheduler-0.6.2/alicebot/adapter/apscheduler/config.py
+-rw-r--r--   0        0        0      972 2023-04-25 11:14:36.277730 alicebot_adapter_apscheduler-0.6.2/alicebot/adapter/apscheduler/event.py
+-rw-r--r--   0        0        0     1365 2023-04-25 11:14:36.277730 alicebot_adapter_apscheduler-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1405 1970-01-01 00:00:00.000000 alicebot_adapter_apscheduler-0.6.2/PKG-INFO
```

### Comparing `alicebot_adapter_apscheduler-0.6.0/alicebot/adapter/apscheduler/__init__.py` & `alicebot_adapter_apscheduler-0.6.2/alicebot/adapter/apscheduler/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 本适配器用于实现定时任务，适配器将使用 APScheduler 实现定时任务，在设定的时间产生一个事件供插件处理。
 APScheduler 使用方法请参考: [APScheduler](https://apscheduler.readthedocs.io/) 。
 """
 import asyncio
 import inspect
 from functools import wraps
-from typing import Any, Dict, Type
+from typing import Any, Dict, Type, Union, Callable, Awaitable
 
 from apscheduler.job import Job
+from apscheduler.triggers.base import BaseTrigger
 from apscheduler.schedulers.asyncio import AsyncIOScheduler
 
 from alicebot.plugin import Plugin
 from alicebot.adapter import Adapter
 from alicebot.log import logger, error_or_exception
 
 from .config import Config
@@ -42,16 +43,16 @@
             if not hasattr(plugin, "trigger") or not hasattr(plugin, "trigger_args"):
                 logger.error(
                     f"Plugin {plugin.__name__} __schedule__ is True, "
                     f"but did not set trigger or trigger_args"
                 )
                 continue
 
-            trigger = getattr(plugin, "trigger")
-            trigger_args = getattr(plugin, "trigger_args")
+            trigger: Union[str, BaseTrigger] = getattr(plugin, "trigger")
+            trigger_args: Dict[str, Any] = getattr(plugin, "trigger_args")
 
             if not isinstance(trigger, str) or not isinstance(trigger_args, dict):
                 logger.error(
                     f"Plugin {plugin.__name__} trigger or trigger_args type error"
                 )
                 continue
 
@@ -69,68 +70,68 @@
             else:
                 logger.info(f"Plugin {plugin.__name__} has been scheduled to run")
 
         self.scheduler.start()
 
     async def shutdown(self):
         """关闭调度器。"""
-        if self.scheduler is not None:
-            self.scheduler.shutdown()
+        self.scheduler.shutdown()
 
     async def create_event(self, plugin_class: Type[Plugin]):
         """创建 APSchedulerEvent 事件。
 
         Args:
             plugin_class: Plugin 类。
         """
         logger.info(f"APSchedulerEvent set by {plugin_class} is created as scheduled")
         asyncio.create_task(
             self.bot.handle_event(
-                APSchedulerEvent(adapter=self, plugin_class=plugin_class),
+                APSchedulerEvent(
+                    adapter=self, type="apscheduler", plugin_class=plugin_class
+                ),
                 handle_get=False,
                 show_log=False,
             )
         )
 
-    async def send(self, *args, **kwargs):
+    async def send(self, *args: Any, **kwargs: Any):
         raise NotImplementedError
 
 
 def scheduler_decorator(
     trigger: str, trigger_args: Dict[str, Any], override_rule: bool = False
 ):
     """用于为插件类添加计划任务功能的装饰器。
 
     Args:
         trigger: APScheduler 触发器。
         trigger_args: APScheduler 触发器参数。
-        override_rule: 是否重写 rule() 方法，若为 True，则会在 rule() 方法中添加处理本插件定义的计划任务事件的逻辑。
+        override_rule: 是否重写 rule() 方法，若为 True ，则会在 rule() 方法中添加处理本插件定义的计划任务事件的逻辑。
     """
 
-    def _decorator(cls: Type):
+    def _decorator(cls: Type[Plugin]):
         if not inspect.isclass(cls):
             raise TypeError(f"can only decorate class")
         if not issubclass(cls, Plugin):
             raise TypeError(f"can only decorate Plugin class")
         setattr(cls, "__schedule__", True)
         setattr(cls, "trigger", trigger)
         setattr(cls, "trigger_args", trigger_args)
         if override_rule:
 
-            def _rule_decorator(func):
+            def _rule_decorator(func: Callable[[Plugin], Awaitable[bool]]):
                 @wraps(func)
-                async def _wrapper(self, *args, **kwargs):
+                async def _wrapper(self: Plugin):
                     if (
                         self.event.type == "apscheduler"
                         and type(self) == self.event.plugin_class
                     ):
                         return True
                     else:
-                        return await func(self, *args, **kwargs)
+                        return await func(self)
 
                 return _wrapper
 
-            handle_func = getattr(cls, "rule")
-            setattr(cls, "rule", _rule_decorator(handle_func))
+            cls.rule = _rule_decorator(cls.rule)
         return cls
 
     return _decorator
```

### Comparing `alicebot_adapter_apscheduler-0.6.0/alicebot/adapter/apscheduler/event.py` & `alicebot_adapter_apscheduler-0.6.2/alicebot/adapter/apscheduler/event.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """APScheduler 适配器事件。"""
-from typing import TYPE_CHECKING, Any, Dict, Type
+from typing import TYPE_CHECKING, Any, Dict, Type, Union
 
 from alicebot.event import Event
 from alicebot.plugin import Plugin
 
 if TYPE_CHECKING:
     from apscheduler.job import Job
+    from apscheduler.triggers.base import BaseTrigger
 
-    from . import APSchedulerAdapter  # noqa
+    from . import APSchedulerAdapter
 
 
 class APSchedulerEvent(Event["APSchedulerAdapter"]):
     """APSchedulerEvent 事件基类。"""
 
-    type = "apscheduler"
     plugin_class: Type[Plugin]
 
     @property
     def job(self) -> "Job":
         """产生当前事件的 APScheduler Job 对象。"""
-        return self.adapter.plugin_class_to_job.get(self.plugin_class)
+        return self.adapter.plugin_class_to_job[self.plugin_class]
 
     @property
-    def trigger(self) -> str:
+    def trigger(self) -> Union[str, "BaseTrigger"]:
         """当前事件对应的 Plugin 的 trigger。"""
-        return getattr(self.plugin_class, "trigger", None)
+        return getattr(self.plugin_class, "trigger")
 
     @property
     def trigger_args(self) -> Dict[str, Any]:
         """当前事件对应的 Plugin 的 trigger_args。"""
-        return getattr(self.plugin_class, "trigger_args", None)
+        return getattr(self.plugin_class, "trigger_args")
```

### Comparing `alicebot_adapter_apscheduler-0.6.0/pyproject.toml` & `alicebot_adapter_apscheduler-0.6.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 [tool.poetry]
 name = "alicebot-adapter-apscheduler"
-version = "0.6.0"
+version = "0.6.2"
 description = "APScheduler adapter for AliceBot."
 license = "MIT"
 authors = ["st1020 <stone_1020@qq.com>"]
 readme = "README.md"
 homepage = "https://docs.alicebot.dev/"
-repository = "https://github.com/st1020/alicebot"
+repository = "https://github.com/AliceBotProject/alicebot"
 documentation = "https://docs.alicebot.dev/"
 keywords = ["bot", "chatbot", "scheduling", "apscheduler"]
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
 apscheduler = "^3.7"
 
 [tool.poetry.dev-dependencies]
 alicebot = { path = "../../", develop = true }
 
 [tool.pydantic-pycharm-plugin]
 ignore-init-method-arguments = true
```

### Comparing `alicebot_adapter_apscheduler-0.6.0/PKG-INFO` & `alicebot_adapter_apscheduler-0.6.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alicebot-adapter-apscheduler
-Version: 0.6.0
+Version: 0.6.2
 Summary: APScheduler adapter for AliceBot.
 Home-page: https://docs.alicebot.dev/
 License: MIT
 Keywords: bot,chatbot,scheduling,apscheduler
 Author: st1020
 Author-email: stone_1020@qq.com
 Requires-Python: >=3.8,<4.0
@@ -17,22 +17,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Communications :: Chat
-Requires-Dist: alicebot (>=0.6.0,<0.7.0)
+Requires-Dist: alicebot (==0.6.2)
 Requires-Dist: apscheduler (>=3.7,<4.0)
 Project-URL: Documentation, https://docs.alicebot.dev/
-Project-URL: Repository, https://github.com/st1020/alicebot
+Project-URL: Repository, https://github.com/AliceBotProject/alicebot
 Description-Content-Type: text/markdown
 
 <div align="center">
-  <a href="https://docs.alicebot.dev/"><img src="https://raw.githubusercontent.com/st1020/alicebot/master/docs/public/logo.png" width="200" height="200" alt="logo"></a>
+  <a href="https://docs.alicebot.dev/"><img src="https://raw.githubusercontent.com/AliceBotProject/alicebot/master/docs/public/logo.png" width="200" height="200" alt="logo"></a>
 
 # AliceBot-Adapter-APScheduler
 
 **APScheduler 定时任务**
 
 </div>
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: alicebot-adapter-apscheduler Version: 0.6.0
+Metadata-Version: 2.1 Name: alicebot-adapter-apscheduler Version: 0.6.2
 Summary: APScheduler adapter for AliceBot. Home-page: https://
 docs.alicebot.dev/ License: MIT Keywords: bot,chatbot,scheduling,apscheduler
 Author: st1020 Author-email: stone_1020@qq.com Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha Classifier: Framework :: AsyncIO
 Classifier: Framework :: Robot Framework Classifier: Framework :: Robot
 Framework :: Library Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Communications :: Chat
-Requires-Dist: alicebot (>=0.6.0,<0.7.0) Requires-Dist: apscheduler
-(>=3.7,<4.0) Project-URL: Documentation, https://docs.alicebot.dev/ Project-
-URL: Repository, https://github.com/st1020/alicebot Description-Content-Type:
-text/markdown
+Requires-Dist: alicebot (==0.6.2) Requires-Dist: apscheduler (>=3.7,<4.0)
+Project-URL: Documentation, https://docs.alicebot.dev/ Project-URL: Repository,
+https://github.com/AliceBotProject/alicebot Description-Content-Type: text/
+markdown
       [logo] # AliceBot-Adapter-APScheduler **APScheduler å®æ¶ä»»å¡**
```

