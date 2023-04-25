# Comparing `tmp/highrise_bot_sdk-23.1.0b6.tar.gz` & `tmp/highrise_bot_sdk-23.1.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highrise_bot_sdk-23.1.0b6.tar", max compression
+gzip compressed data, was "highrise_bot_sdk-23.1.0b8.tar", max compression
```

## Comparing `highrise_bot_sdk-23.1.0b6.tar` & `highrise_bot_sdk-23.1.0b8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2281 2023-04-17 15:53:00.038558 highrise_bot_sdk-23.1.0b6/README.md
--rw-r--r--   0        0        0      992 2023-04-17 15:53:00.038518 highrise_bot_sdk-23.1.0b6/pyproject.toml
--rw-r--r--   0        0        0     7982 2023-04-17 14:59:33.153106 highrise_bot_sdk-23.1.0b6/src/highrise/__init__.py
--rw-r--r--   0        0        0     7172 2023-04-17 14:59:33.153149 highrise_bot_sdk-23.1.0b6/src/highrise/__main__.py
--rw-r--r--   0        0        0     3064 2023-03-31 11:07:05.693250 highrise_bot_sdk-23.1.0b6/src/highrise/_unions.py
--rw-r--r--   0        0        0     7386 2023-04-11 15:27:49.521650 highrise_bot_sdk-23.1.0b6/src/highrise/models.py
--rw-r--r--   0        0        0        0 2023-03-30 13:16:17.585454 highrise_bot_sdk-23.1.0b6/src/highrise/py.typed
--rw-r--r--   0        0        0     3257 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.1.0b6/setup.py
--rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.1.0b6/PKG-INFO
+-rw-r--r--   0        0        0     2673 2023-04-25 12:36:05.294701 highrise_bot_sdk-23.1.0b8/README.md
+-rw-r--r--   0        0        0      992 2023-04-25 12:36:05.291545 highrise_bot_sdk-23.1.0b8/pyproject.toml
+-rw-r--r--   0        0        0     8524 2023-04-25 12:23:39.561597 highrise_bot_sdk-23.1.0b8/src/highrise/__init__.py
+-rw-r--r--   0        0        0     7907 2023-04-25 12:23:39.561633 highrise_bot_sdk-23.1.0b8/src/highrise/__main__.py
+-rw-r--r--   0        0        0     3064 2023-03-31 11:07:05.693250 highrise_bot_sdk-23.1.0b8/src/highrise/_unions.py
+-rw-r--r--   0        0        0     8531 2023-04-25 12:23:39.561662 highrise_bot_sdk-23.1.0b8/src/highrise/models.py
+-rw-r--r--   0        0        0        0 2023-03-30 13:16:17.585454 highrise_bot_sdk-23.1.0b8/src/highrise/py.typed
+-rw-r--r--   0        0        0     3656 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.1.0b8/setup.py
+-rw-r--r--   0        0        0     3305 1970-01-01 00:00:00.000000 highrise_bot_sdk-23.1.0b8/PKG-INFO
```

### Comparing `highrise_bot_sdk-23.1.0b6/README.md` & `highrise_bot_sdk-23.1.0b8/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ---
 
 The Highrise Python Bot SDK is a python library for writing and running Highrise bots.
 
 First, install the library (preferably in a virtual environment):
 
 ```shell
-$ pip install highrise-bot-sdk==23.1.0b6
+$ pip install highrise-bot-sdk==23.1.0b8
 ```
 
 In the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You'll need the token to start your bot later.
 You will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.
 
 Open a new file, and paste the following to get started (into `mybot.py` for example):
 
@@ -28,14 +28,21 @@
 
 ```
 $ highrise mybot:Bot <room ID> <API token>
 ```
 
 ## Changelog
 
+### 23.1.0b8 (2023-04-25)
+
+- Add support for moving users to another room (`self.highrise.move_user_to_room(user_id, room_id)`).
+- Add handler that is triggered when user moves inside a room  (`self.on_user_move(user_id, position)`).) 
+- Expand session_metadata information with information about client rates
+- Expand session_metadata with information about sdk versions if client uses skd
+
 ### 23.1.0b6 (2023-04-17)
 
 - Add Python 3.10 support
 
 ### 23.1.0b5 (2023-04-11)
 
 - Add support for getting room permissions for users (`self.highrise.get_room_privilege(user_id)`).
```

### Comparing `highrise_bot_sdk-23.1.0b6/pyproject.toml` & `highrise_bot_sdk-23.1.0b8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "highrise-bot-sdk"
-version = "23.1.0.b6"
+version = "23.1.0.b8"
 description = "The Highrise Bot SDK, for running Highrise bots written in Python."
 authors = ["Pocket Worlds Inc <server@high.rs>"]
 license = "proprietary"
 readme = "README.md"
 packages = [{include = "highrise", from = "src"}]
```

### Comparing `highrise_bot_sdk-23.1.0b6/src/highrise/__init__.py` & `highrise_bot_sdk-23.1.0b8/src/highrise/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,25 +25,27 @@
     GetRoomPrivilegeRequest,
     GetRoomUsersRequest,
     GetWalletRequest,
     IndicatorRequest,
     Item,
     KeepaliveRequest,
     ModerateRoomRequest,
+    MoveUserToRoomRequest,
     Position,
     Reaction,
     ReactionEvent,
     ReactionRequest,
     RoomPermissions,
     SessionMetadata,
     TeleportRequest,
     TipReactionEvent,
     User,
     UserJoinedEvent,
     UserLeftEvent,
+    UserMovedEvent,
 )
 
 if TYPE_CHECKING:
     from attrs import AttrsInstance
 else:
 
     class AttrsInstance(Protocol):
@@ -112,14 +114,18 @@
         """On a tip received in the room."""
         pass
 
     async def on_channel(self, sender_id: str, message: str, tags: set[str]) -> None:
         """On a hidden channel message."""
         pass
 
+    async def on_user_move(self, user: User, pos: Position) -> None:
+        """On a user moving in the room."""
+        pass
+
 
 class Highrise:
     ws: ClientWebSocketResponse
     tg: TaskGroup
     _req_id = count()
     _req_id_registry: dict[str, Queue[Any]] = {}
 
@@ -198,14 +204,21 @@
         """Change the room privilege for given user_id.
 
         example: self.highrise.change_room_privilege(user_id, RoomPermissions(moderator=True))
 
         """
         await _do_req_no_resp(self, ChangeRoomPrivilegeRequest(user_id, permissions))
 
+    async def move_user_to_room(self, user_id: str, room_id: str) -> None:
+        """Attempt to move user to a different room.
+
+        This will only work if the bot belongs to owner of target room, or has designer privileges.
+        """
+        await _do_req_no_resp(self, MoveUserToRoomRequest(user_id, room_id))
+
     def call_in(self, callback: Callable, delay: float) -> None:
         self.tg.create_task(_delayed_callback(callback, delay))
 
 
 class ResponseError(Exception):
     """An API response error."""
 
@@ -260,24 +273,26 @@
     | TeleportRequest
     | GetRoomUsersRequest
     | GetWalletRequest
     | GetRoomPrivilegeRequest
     | ChangeRoomPrivilegeRequest
     | ModerateRoomRequest
     | KeepaliveRequest
+    | MoveUserToRoomRequest
 )
 IncomingEvents = (
     Error
     | ChatEvent
     | EmoteEvent
     | ReactionEvent
     | UserJoinedEvent
     | UserLeftEvent
     | ChannelEvent
     | TipReactionEvent
+    | UserMovedEvent
 )
 
 
 Incoming = IncomingEvents | Union[tuple(r.Response for r in Outgoing.__args__)]  # type: ignore
 
 
 configure_tagged_union(SessionMetadata | Error, converter)
```

### Comparing `highrise_bot_sdk-23.1.0b6/src/highrise/__main__.py` & `highrise_bot_sdk-23.1.0b8/src/highrise/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,18 +22,21 @@
     EmoteEvent,
     Error,
     ReactionEvent,
     SessionMetadata,
     TipReactionEvent,
     UserJoinedEvent,
     UserLeftEvent,
+    UserMovedEvent,
 )
 
 KEEPALIVE_RATE: Final[int] = 15
 READ_TIMEOUT: Final[int] = 20
+SDK_PACKAGE: Final[str] = "highrise-bot-sdk"
+SDK_NAME: Final[str] = "highrise-python-bot-sdk"
 
 
 @command()
 @argument("bot_path")
 @argument("room_id")
 @argument("api_token")
 def run(bot_path: str, room_id: str, api_token: str) -> None:
@@ -45,24 +48,28 @@
     """
     path.append(getcwd())
     mod, name = bot_path.split(":")
     return arun(main(getattr(import_module(mod), name)(), room_id, api_token))
 
 
 async def main(bot: BaseBot, room_id: str, api_key: str) -> None:
-    version = pkg_resources.get_distribution("highrise-bot-sdk").version
+    version = pkg_resources.get_distribution(SDK_PACKAGE).version
     async with TaskGroup() as tg:
         t = throttler(5, 5)
         while True:
             await anext(t)
             try:
                 async with ClientSession() as session:
                     async with session.ws_connect(
                         environ.get("HR_WEBAPI_URL", "wss://highrise.game/web/webapi"),
-                        headers={"room-id": room_id, "api-token": api_key},
+                        headers={
+                            "room-id": room_id,
+                            "api-token": api_key,
+                            "user-agent": f"{SDK_NAME}/{version}",
+                        },
                     ) as ws:
 
                         async def send_keepalive() -> None:
                             while True:
                                 await sleep(KEEPALIVE_RATE)
                                 try:
                                     await ws.send_json({"_type": "KeepaliveRequest"})
@@ -79,17 +86,22 @@
                             ka_task.cancel()
                             return
                         bot_id = str(session_metadata.user_id)
                         chat = Highrise()
                         chat.ws = ws
                         chat.tg = tg
 
-                        print(
-                            f"Connected using The Highrise Python Bot SDK version: '{version}'."
-                        )
+                        if (
+                            session_metadata.sdk_version is not None
+                            and session_metadata.sdk_version != version
+                        ):
+                            print(
+                                f"WARNING: The Highrise Python Bot SDK version ({version}) "
+                                f"does not match the recommended version for the API ({session_metadata.sdk_version})"
+                            )
 
                         bot.highrise = chat
                         tg.create_task(bot.on_start(session_metadata))
                         while True:
                             frame = await ws.receive(READ_TIMEOUT)
                             if isinstance(frame.data, WebSocketError):
                                 print("Websocket error, exiting.")
@@ -133,14 +145,16 @@
                                     tg.create_task(bot.on_user_join(user))
                                 case UserLeftEvent(user=user):
                                     tg.create_task(bot.on_user_leave(user))
                                 case TipReactionEvent(
                                     sender=sender, receiver=receiver, item=tip
                                 ):
                                     tg.create_task(bot.on_tip(sender, receiver, tip))
+                                case UserMovedEvent(user=user, position=pos):
+                                    tg.create_task(bot.on_user_move(user, pos))
             except (ConnectionResetError, WSServerHandshakeError, TimeoutError):
                 # The throttler should kick in up-code.
                 print("ERROR")
                 pass
 
 
 async def throttler(
```

### Comparing `highrise_bot_sdk-23.1.0b6/src/highrise/_unions.py` & `highrise_bot_sdk-23.1.0b8/src/highrise/_unions.py`

 * *Files identical despite different names*

### Comparing `highrise_bot_sdk-23.1.0b6/src/highrise/models.py` & `highrise_bot_sdk-23.1.0b8/src/highrise/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -336,22 +336,53 @@
 
         rid: str
 
     Response: ClassVar = ChangeRoomPrivilegeResponse
 
 
 @define
+class MoveUserToRoomRequest:
+    """
+    Move user to another room using room_id as a target room id
+    Bot operator must be owner of the target room, or has designer privileges in the target room, this will also work
+    if bot has designer privileges in the target room.
+
+    All other restriction to room movement apply, ie if target room is full this will fail.
+
+    """
+
+    user_id: str
+    room_id: str
+
+    rid: str | None = None
+
+    @define
+    class MoveUserToRoomResponse:
+        rid: str
+
+    Response: ClassVar = MoveUserToRoomResponse
+
+
+@define
 class SessionMetadata:
     """
     Initial session data.
 
     This will be sent once, as the first message when a connection is established.
+    user_id is the bot's user id.
+    rate_limits is a dictionary of rate limits, with the key being the rate limit name and the value being a tuple of
+    (limit, period).
+    sdk_versions is a string containing the SDK versions recommended by the server if user is using SDK.
+
+
     """
 
     user_id: str
+    rate_limits: dict[str, tuple[int, float]]
+    sdk_version: str | None = None
 
 
 @define
 class ChatEvent:
     """
     A chat event, sent by a `user` in the room.
     """
@@ -417,7 +448,19 @@
     """
     The `sender` has sent `receiver` a tip (the `item`) in the current room.
     """
 
     sender: User
     receiver: User
     item: Item | CurrencyItem
+
+
+@define
+class UserMovedEvent:
+    """
+    A user has moved in the room.
+    user: User that moved
+    position: New position of the user or anchor position
+    """
+
+    user: User
+    position: Position | AnchorPosition
```

### Comparing `highrise_bot_sdk-23.1.0b6/setup.py` & `highrise_bot_sdk-23.1.0b8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,17 +17,17 @@
  'quattro>=22.1.0,<23.0.0']
 
 entry_points = \
 {'console_scripts': ['highrise = highrise.__main__:run']}
 
 setup_kwargs = {
     'name': 'highrise-bot-sdk',
-    'version': '23.1.0b6',
+    'version': '23.1.0b8',
     'description': 'The Highrise Bot SDK, for running Highrise bots written in Python.',
-    'long_description': "# The Highrise Python Bot SDK\n\n---\n\nThe Highrise Python Bot SDK is a python library for writing and running Highrise bots.\n\nFirst, install the library (preferably in a virtual environment):\n\n```shell\n$ pip install highrise-bot-sdk==23.1.0b6\n```\n\nIn the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You'll need the token to start your bot later.\nYou will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.\n\nOpen a new file, and paste the following to get started (into `mybot.py` for example):\n\n```python\nfrom highrise import BaseBot\n\nclass Bot(BaseBot):\n    pass\n```\n\nOverride methods from `BaseBot` as needed.\n\nWhen you're ready, run the bot from the terminal using the SDK, giving it the Python path to the Bot class:\n\n```\n$ highrise mybot:Bot <room ID> <API token>\n```\n\n## Changelog\n\n### 23.1.0b6 (2023-04-17)\n\n- Add Python 3.10 support\n\n### 23.1.0b5 (2023-04-11)\n\n- Add support for getting room permissions for users (`self.highrise.get_room_privilege(user_id)`).\n- Add support changing room permissions for users (`self.highrise.set_room_privilege(user_id, privilege)`).\n- Add support for moderating rooms (`self.highrise.moderate_room(user_id, moderate_action, action_length)`). \n- Rework how keepalive is handled\n\n### 23.1.0b4 (2023-04-05)\n\n- Methods mapping to requests with empty responses (`chat`, `send_whisper`, `send_emote`, `react`, `set_indicator`, `send_channel`, `walk_to`, `teleport`) now return `None`, and raise a `highrise.ResponseError` on an error response.\n- Fix the emote API.\n- Internally rework request handling to improve robustness.\n\n### 23.1.0b3 (2023-04-03)\n\n- Fix the chatting API.\n\n### 23.1.0b2 (2023-04-03)\n\n- Add support for receiving and sending reactions.\n- Fix support for hidden channels.\n- Migrate to the new message for avatars leaving.\n- Improve concurrency when awaiting bot methods.\n- Fix issues with teleporting users.\n- Fix issues with user coordinates.\n- Add support for fetching the bot wallet (`self.highrise.get_wallet()`).\n\n### 23.1.0b1 (2023-03-28)\n\n- Add support for emotes and hidden channel messages.\n\n### 23.1.0b0 (2023-03-10)\n\n- Initial beta release.\n",
+    'long_description': "# The Highrise Python Bot SDK\n\n---\n\nThe Highrise Python Bot SDK is a python library for writing and running Highrise bots.\n\nFirst, install the library (preferably in a virtual environment):\n\n```shell\n$ pip install highrise-bot-sdk==23.1.0b8\n```\n\nIn the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You'll need the token to start your bot later.\nYou will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.\n\nOpen a new file, and paste the following to get started (into `mybot.py` for example):\n\n```python\nfrom highrise import BaseBot\n\nclass Bot(BaseBot):\n    pass\n```\n\nOverride methods from `BaseBot` as needed.\n\nWhen you're ready, run the bot from the terminal using the SDK, giving it the Python path to the Bot class:\n\n```\n$ highrise mybot:Bot <room ID> <API token>\n```\n\n## Changelog\n\n### 23.1.0b8 (2023-04-25)\n\n- Add support for moving users to another room (`self.highrise.move_user_to_room(user_id, room_id)`).\n- Add handler that is triggered when user moves inside a room  (`self.on_user_move(user_id, position)`).) \n- Expand session_metadata information with information about client rates\n- Expand session_metadata with information about sdk versions if client uses skd\n\n### 23.1.0b6 (2023-04-17)\n\n- Add Python 3.10 support\n\n### 23.1.0b5 (2023-04-11)\n\n- Add support for getting room permissions for users (`self.highrise.get_room_privilege(user_id)`).\n- Add support changing room permissions for users (`self.highrise.set_room_privilege(user_id, privilege)`).\n- Add support for moderating rooms (`self.highrise.moderate_room(user_id, moderate_action, action_length)`). \n- Rework how keepalive is handled\n\n### 23.1.0b4 (2023-04-05)\n\n- Methods mapping to requests with empty responses (`chat`, `send_whisper`, `send_emote`, `react`, `set_indicator`, `send_channel`, `walk_to`, `teleport`) now return `None`, and raise a `highrise.ResponseError` on an error response.\n- Fix the emote API.\n- Internally rework request handling to improve robustness.\n\n### 23.1.0b3 (2023-04-03)\n\n- Fix the chatting API.\n\n### 23.1.0b2 (2023-04-03)\n\n- Add support for receiving and sending reactions.\n- Fix support for hidden channels.\n- Migrate to the new message for avatars leaving.\n- Improve concurrency when awaiting bot methods.\n- Fix issues with teleporting users.\n- Fix issues with user coordinates.\n- Add support for fetching the bot wallet (`self.highrise.get_wallet()`).\n\n### 23.1.0b1 (2023-03-28)\n\n- Add support for emotes and hidden channel messages.\n\n### 23.1.0b0 (2023-03-10)\n\n- Initial beta release.\n",
     'author': 'Pocket Worlds Inc',
     'author_email': 'server@high.rs',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `highrise_bot_sdk-23.1.0b6/PKG-INFO` & `highrise_bot_sdk-23.1.0b8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highrise-bot-sdk
-Version: 23.1.0b6
+Version: 23.1.0b8
 Summary: The Highrise Bot SDK, for running Highrise bots written in Python.
 License: Proprietary
 Author: Pocket Worlds Inc
 Author-email: server@high.rs
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 ---
 
 The Highrise Python Bot SDK is a python library for writing and running Highrise bots.
 
 First, install the library (preferably in a virtual environment):
 
 ```shell
-$ pip install highrise-bot-sdk==23.1.0b6
+$ pip install highrise-bot-sdk==23.1.0b8
 ```
 
 In the [`Settings` section of the Highrise website](https://highrise.game/account/settings), create a bot and generate the API token. You'll need the token to start your bot later.
 You will also need a room ID for your bot to connect to; the room needs to be owned by you or your bot user needs to have designer rights to enter it.
 
 Open a new file, and paste the following to get started (into `mybot.py` for example):
 
@@ -46,14 +46,21 @@
 
 ```
 $ highrise mybot:Bot <room ID> <API token>
 ```
 
 ## Changelog
 
+### 23.1.0b8 (2023-04-25)
+
+- Add support for moving users to another room (`self.highrise.move_user_to_room(user_id, room_id)`).
+- Add handler that is triggered when user moves inside a room  (`self.on_user_move(user_id, position)`).) 
+- Expand session_metadata information with information about client rates
+- Expand session_metadata with information about sdk versions if client uses skd
+
 ### 23.1.0b6 (2023-04-17)
 
 - Add Python 3.10 support
 
 ### 23.1.0b5 (2023-04-11)
 
 - Add support for getting room permissions for users (`self.highrise.get_room_privilege(user_id)`).
```

