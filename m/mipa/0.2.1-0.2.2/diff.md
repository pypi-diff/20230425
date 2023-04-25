# Comparing `tmp/mipa-0.2.1.tar.gz` & `tmp/mipa-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mipa-0.2.1.tar", last modified: Tue Mar 21 19:22:12 2023, max compression
+gzip compressed data, was "mipa-0.2.2.tar", last modified: Tue Apr 25 08:53:03 2023, max compression
```

## Comparing `mipa-0.2.1.tar` & `mipa-0.2.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:22:12.750432 mipa-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-21 19:22:01.000000 mipa-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-21 19:22:01.000000 mipa-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-03-21 19:22:12.750432 mipa-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-03-21 19:22:01.000000 mipa-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:22:12.750432 mipa-0.2.1/mipa/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-21 19:22:01.000000 mipa-0.2.1/mipa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-21 19:22:12.750432 mipa-0.2.1/mipa/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-03-21 19:22:01.000000 mipa-0.2.1/mipa/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-21 19:22:01.000000 mipa-0.2.1/mipa/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:22:12.750432 mipa-0.2.1/mipa/ext/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-21 19:22:01.000000 mipa-0.2.1/mipa/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:22:12.750432 mipa-0.2.1/mipa/ext/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-21 19:22:01.000000 mipa-0.2.1/mipa/ext/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-03-21 19:22:01.000000 mipa-0.2.1/mipa/ext/commands/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-03-21 19:22:01.000000 mipa-0.2.1/mipa/ext/commands/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-03-21 19:22:01.000000 mipa-0.2.1/mipa/ext/commands/cog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-03-21 19:22:01.000000 mipa-0.2.1/mipa/ext/commands/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-03-21 19:22:01.000000 mipa-0.2.1/mipa/ext/commands/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:22:12.750432 mipa-0.2.1/mipa/ext/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-03-21 19:22:01.000000 mipa-0.2.1/mipa/ext/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-03-21 19:22:01.000000 mipa-0.2.1/mipa/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-03-21 19:22:01.000000 mipa-0.2.1/mipa/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-03-21 19:22:01.000000 mipa-0.2.1/mipa/router.py
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-03-21 19:22:01.000000 mipa-0.2.1/mipa/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-03-21 19:22:01.000000 mipa-0.2.1/mipa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:22:12.750432 mipa-0.2.1/mipa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-03-21 19:22:12.000000 mipa-0.2.1/mipa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-21 19:22:12.000000 mipa-0.2.1/mipa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 19:22:12.000000 mipa-0.2.1/mipa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-21 19:22:12.000000 mipa-0.2.1/mipa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-21 19:22:12.000000 mipa-0.2.1/mipa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-21 19:22:01.000000 mipa-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-21 19:22:01.000000 mipa-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-21 19:22:12.750432 mipa-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-21 19:22:01.000000 mipa-0.2.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-03-21 19:22:01.000000 mipa-0.2.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:53:03.218676 mipa-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-25 08:52:51.000000 mipa-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-25 08:52:51.000000 mipa-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-25 08:53:03.218676 mipa-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-25 08:52:51.000000 mipa-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:53:03.218676 mipa-0.2.2/mipa/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 08:53:03.218676 mipa-0.2.2/mipa/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:53:03.218676 mipa-0.2.2/mipa/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:53:03.218676 mipa-0.2.2/mipa/ext/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/ext/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/ext/commands/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/ext/commands/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/ext/commands/cog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/ext/commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/ext/commands/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:53:03.218676 mipa-0.2.2/mipa/ext/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/ext/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-25 08:52:51.000000 mipa-0.2.2/mipa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:53:03.218676 mipa-0.2.2/mipa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-25 08:53:03.000000 mipa-0.2.2/mipa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-25 08:53:03.000000 mipa-0.2.2/mipa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:53:03.000000 mipa-0.2.2/mipa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-25 08:53:03.000000 mipa-0.2.2/mipa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-25 08:53:03.000000 mipa-0.2.2/mipa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-25 08:52:51.000000 mipa-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-25 08:52:51.000000 mipa-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-25 08:53:03.218676 mipa-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-25 08:52:51.000000 mipa-0.2.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-25 08:52:51.000000 mipa-0.2.2/versioneer.py
```

### Comparing `mipa-0.2.1/LICENSE` & `mipa-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mipa-0.2.1/PKG-INFO` & `mipa-0.2.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mipa
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python wrapper for the Misskey API
 Home-page: https://github.com/yupix/MiPA
 Author: yupix
 Author-email: yupi0982@outlook.jp
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
@@ -25,14 +25,18 @@
 ## 概要
 
 MiPA は[Discord.py](https://github.com/Rapptz/discord.py)
 ライクな書き方ができるように作っている MisskeyApi wrapper です
 
 ## 注意
 
+### MiPACとの関係性について
+
+MiPAはMiPACというライブラリに依存しています。これはMiPAのCore部分をまとめた物であり、基本的にはApiへのアクセス用メソッドなどを提供します。MiPAではMiPACのメソッド群をそのまま公開している為、MiPAC側で大きな変更が入るとMiPAを使用しているプロジェクトでもその影響を受ける可能性があります。そのため、[CHANGELOG.md](./CHANGELOG.md) で MiPACのバージョンが変更された際はそのリリースノートへのリンクを添付しています。予めMiPAC側での変更を確認したうえでアップデートをお願いします。
+
 - このプロジェクトは開発中です。仕様が定まっていないため、破壊的変更が多いです。
 - `master` ブランチで使用しているmipacは`GitHub`にあるmipacの`develop`ブランチの物です。
 
 ## サポートしているMisskey
 
 - [Misskey Official v12](https://github.com/misskey-dev/misskey)
 - [Ayuskey latest](https://github.com/teamblackcrystal/misskey)
@@ -73,14 +77,25 @@
     asyncio.run(bot.start('wss://example.com/streaming', 'your token here'))
 ```
 
 Want more examples? Go to the [examples folder](examples)! Want to know how to use a feature that isn't even here?
 Submit a request in an Issue!
 
 
+### 使用者の方へ
+
+MiPAで作ったBotなどをGitHubなどで公開している場合は、Issueなどに送信してくだされば、MiPAで作られている物に追加します。また、良ければBotのプロフィールなどにこのBotはMiPAで作成されているとの旨を記載してくださると嬉しいです。
+
+### MiPAで作られているもの
+
+#### Bot
+
+- [akari](https://github.com/teamblackcrystal/akari)
+    - 作者の yupix が作成しているBotです。クリーンアーキテクチャを用いているため、部分的に分かりにくい所があるかもしれません。
+
 ### 開発者向け情報
 
 このプロジェクトでは [black](https://github.com/psf/black)のforkである、[axblack](https://github.com/axiros/axblack)を利用しています。主な違いはダブルクォートがデフォルトではなく、シングルクォートになっている点です
 
 ## LICENSE
 
 このプロジェクトは [MIT LICENSE](./LICENSE) で提供されます。
```

### Comparing `mipa-0.2.1/README.md` & `mipa-0.2.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 ## 概要
 
 MiPA は[Discord.py](https://github.com/Rapptz/discord.py)
 ライクな書き方ができるように作っている MisskeyApi wrapper です
 
 ## 注意
 
+### MiPACとの関係性について
+
+MiPAはMiPACというライブラリに依存しています。これはMiPAのCore部分をまとめた物であり、基本的にはApiへのアクセス用メソッドなどを提供します。MiPAではMiPACのメソッド群をそのまま公開している為、MiPAC側で大きな変更が入るとMiPAを使用しているプロジェクトでもその影響を受ける可能性があります。そのため、[CHANGELOG.md](./CHANGELOG.md) で MiPACのバージョンが変更された際はそのリリースノートへのリンクを添付しています。予めMiPAC側での変更を確認したうえでアップデートをお願いします。
+
 - このプロジェクトは開発中です。仕様が定まっていないため、破壊的変更が多いです。
 - `master` ブランチで使用しているmipacは`GitHub`にあるmipacの`develop`ブランチの物です。
 
 ## サポートしているMisskey
 
 - [Misskey Official v12](https://github.com/misskey-dev/misskey)
 - [Ayuskey latest](https://github.com/teamblackcrystal/misskey)
@@ -55,14 +59,25 @@
     asyncio.run(bot.start('wss://example.com/streaming', 'your token here'))
 ```
 
 Want more examples? Go to the [examples folder](examples)! Want to know how to use a feature that isn't even here?
 Submit a request in an Issue!
 
 
+### 使用者の方へ
+
+MiPAで作ったBotなどをGitHubなどで公開している場合は、Issueなどに送信してくだされば、MiPAで作られている物に追加します。また、良ければBotのプロフィールなどにこのBotはMiPAで作成されているとの旨を記載してくださると嬉しいです。
+
+### MiPAで作られているもの
+
+#### Bot
+
+- [akari](https://github.com/teamblackcrystal/akari)
+    - 作者の yupix が作成しているBotです。クリーンアーキテクチャを用いているため、部分的に分かりにくい所があるかもしれません。
+
 ### 開発者向け情報
 
 このプロジェクトでは [black](https://github.com/psf/black)のforkである、[axblack](https://github.com/axiros/axblack)を利用しています。主な違いはダブルクォートがデフォルトではなく、シングルクォートになっている点です
 
 ## LICENSE
 
 このプロジェクトは [MIT LICENSE](./LICENSE) で提供されます。
```

### Comparing `mipa-0.2.1/mipa/client.py` & `mipa-0.2.2/mipa/client.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.1/mipa/exception.py` & `mipa-0.2.2/mipa/exception.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.1/mipa/ext/commands/_types.py` & `mipa-0.2.2/mipa/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.1/mipa/ext/commands/bot.py` & `mipa-0.2.2/mipa/ext/commands/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     List,
     Optional,
     Tuple,
     Union,
 )
 
 from mipac.models.chat import ChatMessage
+from mipac.models.emoji import CustomEmoji
 from mipac.models.user import UserDetailed
 
 from mipa import Client
 from mipa.exception import (
     CogNameDuplicate,
     ExtensionAlreadyLoaded,
     ExtensionFailed,
@@ -445,10 +446,30 @@
         When you earn an achievement
 
         Parameters
         ----------
         notice : NotificationAchievement
         """
 
+    async def on_emoji_deleted(self, emojis: list[CustomEmoji]):
+        """
+        カスタム絵文字が削除された
+
+        Parameters
+        ----------
+        emojis : list[CustomEmoji]
+            削除された絵文字のリスト
+        """
+
+    async def on_emoji_updated(self, emojis: list[CustomEmoji]):
+        """
+        カスタム絵文字が更新された
+
+        Parameters
+        ----------
+        emojis : list[CustomEmoji]
+            更新された絵文字のリスト
+        """
+
 
 class Bot(BotBase, Client):
     pass
```

### Comparing `mipa-0.2.1/mipa/ext/commands/cog.py` & `mipa-0.2.2/mipa/ext/commands/cog.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,22 +24,34 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 from __future__ import annotations
 
 import inspect
-from typing import TYPE_CHECKING, Any, ClassVar, Dict, List, Optional, Tuple
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    ClassVar,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    TypeVar,
+)
 
 from mipa.ext.commands._types import _BaseCommand
 from mipa.ext.commands.core import Command
 
 if TYPE_CHECKING:
     from mipa.ext.commands.bot import BotBase
 
+FuncT = TypeVar('FuncT', bound=Callable[..., Any])
+
 
 class CogMeta(type):
     __cog_name__: str
 
     def __new__(cls, *args: Tuple[Any], **kwargs: Dict[str, Any]):
         name, bases, attrs = args
         attrs['__cog_name__'] = kwargs.pop('name', name)
@@ -100,16 +112,16 @@
 
     def __new__(cls, *args: Any, **kwargs: Any):
         self = super().__new__(cls)
         self.__cog_commands__ = tuple(cls.__cog_commands__)
         return self
 
     @classmethod
-    def listener(cls, name: Optional[str] = None):
-        def decorator(func: Cog):
+    def listener(cls, name: Optional[str] = None) -> Callable[[FuncT], FuncT]:
+        def decorator(func: FuncT):
             actual = func
             if isinstance(actual, staticmethod):
                 actual = actual.__func__
             if not inspect.iscoroutinefunction(actual):
                 raise TypeError(
                     'Listener function must be a coroutine function.'
                 )
```

### Comparing `mipa-0.2.1/mipa/ext/commands/context.py` & `mipa-0.2.2/mipa/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.1/mipa/ext/commands/core.py` & `mipa-0.2.2/mipa/ext/commands/core.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.1/mipa/ext/tasks/__init__.py` & `mipa-0.2.2/mipa/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.1/mipa/gateway.py` & `mipa-0.2.2/mipa/gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 import asyncio
 import json
 from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, TypeVar
 
 import aiohttp
 from aiohttp import ClientError
-from mipac.util import str_lower
+from mipac.utils.format import str_lower
 
 from mipa.exception import ClientConnectorError, WebSocketReconnect
 from mipa.router import Router
 
 if TYPE_CHECKING:
     from .client import Client
```

### Comparing `mipa-0.2.1/mipa/http.py` & `mipa-0.2.2/mipa/http.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.1/mipa/router.py` & `mipa-0.2.2/mipa/router.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.1/mipa/state.py` & `mipa-0.2.2/mipa/state.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,23 @@
 DEALINGS IN THE SOFTWARE.
 """
 from __future__ import annotations
 
 import asyncio
 import inspect
 import logging
-from typing import TYPE_CHECKING, Any, Callable, Dict
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    Generic,
+    TypedDict,
+    TypeVar,
+)
 
 from mipac.models import Note
 from mipac.models.chat import ChatMessage
 from mipac.models.emoji import CustomEmoji
 from mipac.models.note import NoteDeleted
 from mipac.models.notification import (
     NotificationAchievement,
@@ -45,29 +53,37 @@
     NotificationPollEnd,
     NotificationReaction,
 )
 from mipac.models.reaction import PartialReaction
 from mipac.models.user import UserDetailed
 from mipac.types import INote
 from mipac.types.chat import IChatMessage
+from mipac.types.emoji import ICustomEmoji
 from mipac.types.note import (
     INoteUpdated,
     INoteUpdatedDelete,
     INoteUpdatedReaction,
 )
-from mipac.util import str_lower, upper_to_lower
+from mipac.utils.format import str_lower, upper_to_lower
 
 if TYPE_CHECKING:
     from mipac.types.notification import INotification
     from mipac.types.user import IUserDetailed
 
     from mipa.client import Client
 
 _log = logging.getLogger(__name__)
 
+T = TypeVar('T')
+
+
+class IMessage(TypedDict, Generic[T]):
+    type: str
+    body: dict[str, T]
+
 
 class ConnectionState:
     def __init__(
         self,
         dispatch: Callable[..., Any],
         loop: asyncio.AbstractEventLoop,
         client: Client,
@@ -82,14 +98,32 @@
                 parsers[attr[6:].upper()] = func
 
     async def parse_emoji_added(self, message: Dict[str, Any]):
         self.__dispatch(
             'emoji_add', CustomEmoji(message['body']['emoji'], client=self.api)
         )
 
+    async def parse_emoji_deleted(self, message: IMessage[list[ICustomEmoji]]):
+        self.__dispatch(
+            'emoji_deleted',
+            [
+                CustomEmoji(emoji, client=self.api)
+                for emoji in message['body']['emojis']
+            ],
+        )
+
+    async def parse_emoji_updated(self, message: IMessage[list[ICustomEmoji]]):
+        self.__dispatch(
+            'emoji_updated',
+            [
+                CustomEmoji(emoji, client=self.api)
+                for emoji in message['body']['emojis']
+            ],
+        )
+
     async def parse_channel(self, message: Dict[str, Any]) -> None:
         """parse_channel is a function to parse channel event
 
         チャンネルタイプのデータを解析後適切なパーサーに移動させます
 
         Parameters
         ----------
@@ -124,35 +158,37 @@
         self.__dispatch('user_unfollow', user)
 
     async def parse_signin(self, message: Dict[str, Any]):
         """
         ログインが発生した際のイベント
         """
 
-    async def parse_note_updated(self, message: INoteUpdated[Any]):
-        message: Dict[str, Any] = upper_to_lower(message)
+    async def parse_note_updated(self, note_data: INoteUpdated[Any]):
+        message: Dict[str, Any] = upper_to_lower(note_data)
         if func := getattr(self, f'parse_{message["body"]["type"]}', None):
             await func(message)
         else:
             _log.debug(
                 f'Unknown note_updated event type: {message["body"]["type"]}'
             )
 
     async def parse_deleted(self, note: INoteUpdated[INoteUpdatedDelete]):
         self.__dispatch('note_deleted', NoteDeleted(note))
 
     async def parse_unreacted(
         self, reaction: INoteUpdated[INoteUpdatedReaction]
     ):
-        self.__dispatch('unreacted', PartialReaction(reaction))
+        self.__dispatch(
+            'unreacted', PartialReaction(reaction, client=self.api)
+        )
 
     async def parse_reacted(
         self, reaction: INoteUpdated[INoteUpdatedReaction]
     ):
-        self.__dispatch('reacted', PartialReaction(reaction))
+        self.__dispatch('reacted', PartialReaction(reaction, client=self.api))
 
     async def parse_me_updated(self, user: IUserDetailed):
         self.__dispatch('me_updated', UserDetailed(user, client=self.api))
 
     async def parse_read_all_announcements(
         self, message: Dict[str, Any]
     ) -> None:
@@ -209,24 +245,26 @@
         """
         チャットが既読になっていない場合のデータを処理する関数
         """
         self.__dispatch(
             'chat_unread_message', ChatMessage(message, client=self.api),
         )
 
-    async def parse_notification(self, message: Dict[str, Any]) -> None:
+    async def parse_notification(
+        self, notification_data: Dict[str, Any]
+    ) -> None:
         """
         Parse notification event
 
         Parameters
         ----------
         message: Dict[str, Any]
             Received message
         """
-        message: INotification = upper_to_lower(message)
+        message: INotification = upper_to_lower(notification_data)
         notification_map: dict[
             str,
             tuple[
                 str,
                 [
                     NotificationFollow
                     | NotificationNote
@@ -256,15 +294,15 @@
                 'achievement_earned',
                 NotificationAchievement,
             ),
         }
         dispatch_path, parse_class = notification_map.get(
             str_lower(message['type']), (None, None)
         )
-        if dispatch_path:
+        if dispatch_path and parse_class:
             self.__dispatch(
                 dispatch_path, parse_class(message, client=self.api)
             )
 
     async def parse_unread_notification(self, message: Dict[str, Any]) -> None:
         """
         未読の通知を解析する関数
```

### Comparing `mipa-0.2.1/mipa/utils.py` & `mipa-0.2.2/mipa/utils.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.1/mipa.egg-info/PKG-INFO` & `mipa-0.2.2/mipa.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mipa
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python wrapper for the Misskey API
 Home-page: https://github.com/yupix/MiPA
 Author: yupix
 Author-email: yupi0982@outlook.jp
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
@@ -25,14 +25,18 @@
 ## 概要
 
 MiPA は[Discord.py](https://github.com/Rapptz/discord.py)
 ライクな書き方ができるように作っている MisskeyApi wrapper です
 
 ## 注意
 
+### MiPACとの関係性について
+
+MiPAはMiPACというライブラリに依存しています。これはMiPAのCore部分をまとめた物であり、基本的にはApiへのアクセス用メソッドなどを提供します。MiPAではMiPACのメソッド群をそのまま公開している為、MiPAC側で大きな変更が入るとMiPAを使用しているプロジェクトでもその影響を受ける可能性があります。そのため、[CHANGELOG.md](./CHANGELOG.md) で MiPACのバージョンが変更された際はそのリリースノートへのリンクを添付しています。予めMiPAC側での変更を確認したうえでアップデートをお願いします。
+
 - このプロジェクトは開発中です。仕様が定まっていないため、破壊的変更が多いです。
 - `master` ブランチで使用しているmipacは`GitHub`にあるmipacの`develop`ブランチの物です。
 
 ## サポートしているMisskey
 
 - [Misskey Official v12](https://github.com/misskey-dev/misskey)
 - [Ayuskey latest](https://github.com/teamblackcrystal/misskey)
@@ -73,14 +77,25 @@
     asyncio.run(bot.start('wss://example.com/streaming', 'your token here'))
 ```
 
 Want more examples? Go to the [examples folder](examples)! Want to know how to use a feature that isn't even here?
 Submit a request in an Issue!
 
 
+### 使用者の方へ
+
+MiPAで作ったBotなどをGitHubなどで公開している場合は、Issueなどに送信してくだされば、MiPAで作られている物に追加します。また、良ければBotのプロフィールなどにこのBotはMiPAで作成されているとの旨を記載してくださると嬉しいです。
+
+### MiPAで作られているもの
+
+#### Bot
+
+- [akari](https://github.com/teamblackcrystal/akari)
+    - 作者の yupix が作成しているBotです。クリーンアーキテクチャを用いているため、部分的に分かりにくい所があるかもしれません。
+
 ### 開発者向け情報
 
 このプロジェクトでは [black](https://github.com/psf/black)のforkである、[axblack](https://github.com/axiros/axblack)を利用しています。主な違いはダブルクォートがデフォルトではなく、シングルクォートになっている点です
 
 ## LICENSE
 
 このプロジェクトは [MIT LICENSE](./LICENSE) で提供されます。
```

### Comparing `mipa-0.2.1/mipa.egg-info/SOURCES.txt` & `mipa-0.2.2/mipa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mipa-0.2.1/setup.py` & `mipa-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.1/versioneer.py` & `mipa-0.2.2/versioneer.py`

 * *Files identical despite different names*

