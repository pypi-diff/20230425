# Comparing `tmp/novelcraft_sdk-0.1.0.tar.gz` & `tmp/novelcraft_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novelcraft_sdk-0.1.0.tar", max compression
+gzip compressed data, was "novelcraft_sdk-0.1.1.tar", max compression
```

## Comparing `novelcraft_sdk-0.1.0.tar` & `novelcraft_sdk-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1211 2023-04-24 02:28:54.242174 novelcraft_sdk-0.1.0/LICENSE
--rw-r--r--   0        0        0      806 2023-04-24 02:28:54.242174 novelcraft_sdk-0.1.0/README.md
--rw-r--r--   0        0        0      604 2023-04-24 02:28:54.242174 novelcraft_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       43 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/__init__.py
--rw-r--r--   0        0        0      729 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/__init__.py
--rw-r--r--   0        0        0     5942 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/agent.py
--rw-r--r--   0        0        0     1030 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/block.py
--rw-r--r--   0        0        0     2690 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/block_source.py
--rw-r--r--   0        0        0     3203 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/client.py
--rw-r--r--   0        0        0     1981 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/entity.py
--rw-r--r--   0        0        0     1652 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/entity_source.py
--rw-r--r--   0        0        0     6173 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/inventory.py
--rw-r--r--   0        0        0     1091 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/item_stack.py
--rw-r--r--   0        0        0     2917 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/logger.py
--rw-r--r--   0        0        0     2298 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/message.py
--rw-r--r--   0        0        0      353 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/orientation.py
--rw-r--r--   0        0        0      389 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/position.py
--rw-r--r--   0        0        0    13588 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/sdk.py
--rw-r--r--   0        0        0     1372 2023-04-24 02:28:54.246174 novelcraft_sdk-0.1.0/src/novelcraft/sdk/section.py
--rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 novelcraft_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/LICENSE
+-rw-r--r--   0        0        0      804 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/README.md
+-rw-r--r--   0        0        0      604 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/__init__.py
+-rw-r--r--   0        0        0      729 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/__init__.py
+-rw-r--r--   0        0        0     5917 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/agent.py
+-rw-r--r--   0        0        0     1029 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/block.py
+-rw-r--r--   0        0        0     2680 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/block_source.py
+-rw-r--r--   0        0        0     3189 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/client.py
+-rw-r--r--   0        0        0     1980 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/entity.py
+-rw-r--r--   0        0        0     1646 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/entity_source.py
+-rw-r--r--   0        0        0     6133 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/inventory.py
+-rw-r--r--   0        0        0     1090 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/item_stack.py
+-rw-r--r--   0        0        0     2908 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/logger.py
+-rw-r--r--   0        0        0     2296 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/message.py
+-rw-r--r--   0        0        0      353 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/orientation.py
+-rw-r--r--   0        0        0      389 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/position.py
+-rw-r--r--   0        0        0    14307 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/sdk.py
+-rw-r--r--   0        0        0     1367 2023-04-25 12:14:26.705764 novelcraft_sdk-0.1.1/src/novelcraft/sdk/section.py
+-rw-r--r--   0        0        0     1499 1970-01-01 00:00:00.000000 novelcraft_sdk-0.1.1/PKG-INFO
```

### Comparing `novelcraft_sdk-0.1.0/LICENSE` & `novelcraft_sdk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.1.0/README.md` & `novelcraft_sdk-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 async def main():
     await sdk.initialize()
 
     # Do something
 
-    await ncsdk.finalize()
+    await sdk.finalize()
 
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
 For more information, please start with _placeholder_.
```

### Comparing `novelcraft_sdk-0.1.0/pyproject.toml` & `novelcraft_sdk-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "novelcraft.sdk"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Python library for communicating with NovelCraft Servers and accessing NovelCraft game data"
 authors = ["NovelCraft"]
 license = "Unlicense"
 readme = "README.md"
 packages = [
     { include = "novelcraft", from = "src" }
 ]
```

### Comparing `novelcraft_sdk-0.1.0/src/novelcraft/sdk/__init__.py` & `novelcraft_sdk-0.1.1/src/novelcraft/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `novelcraft_sdk-0.1.0/src/novelcraft/sdk/agent.py` & `novelcraft_sdk-0.1.1/src/novelcraft/sdk/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 information about the agent.
 """
 
 from abc import ABC, abstractmethod
 from enum import Enum
 
 from .entity import IEntity
-from .inventory import IInventory, _Inventory
-from .message import _Message
+from .inventory import IInventory, Inventory
+from .message import Message
 from .orientation import Orientation
 from .position import Position
-from .client import _Client
+from .client import Client
 
 
 class IAgent(IEntity, ABC):
     """The agent interface.
 
     The agent interface is the interface that can be used to control the
     agent and get information about the agent.
@@ -61,152 +61,152 @@
             The movement.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def set_movement(self, movement: MovementKind) -> None:
         """Sets the movement of the agent.
-        
+
         Args:
             movement (MovementKind): The movement.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def attack(self, interaction: InteractionKind) -> None:
         """Attacks.
-        
+
         Args:
             interaction (InteractionKind): The interaction.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def jump(self) -> None:
         """Jumps."""
         raise NotImplementedError()
 
     @abstractmethod
     def look_at(self, position: Position[float]) -> None:
         """Looks at a position.
-        
+
         Args:
             position (Position[float]): The position.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def use(self, interaction: InteractionKind) -> None:
         """Uses.
-        
+
         Args:
             interaction (InteractionKind): The interaction.
         """
         raise NotImplementedError()
 
-class _Agent(IAgent):
-    def __init__(self, client: _Client, token: str, unique_id: int, position: Position[float], orientation: Orientation[float]):
+class Agent(IAgent):
+    def __init__(self, client: Client, token: str, unique_id: int, position: Position[float], orientation: Orientation[float]):
         super().__init__()
 
         self._client = client
         self._health = 0.0
-        self._inventory = _Inventory(client=client, token=token)
+        self._inventory = Inventory(client=client, token=token)
         self._movement = IAgent.MovementKind.STOPPED
         self._orientation = orientation
         self._position = position
         self._token = token
         self._unique_id = unique_id
 
     def get_orientation(self) -> Orientation[float]:
         return self._orientation
-    
+
     def get_position(self) -> Position[float]:
         return self._position
-    
+
     def get_type_id(self) -> int:
         return 0
-    
+
     def get_unique_id(self) -> int:
         return self._unique_id
-    
+
     def set_orientation(self, orientation: Orientation[float]):
         self._orientation = orientation
 
     def set_position(self, position: Position[float]):
         self._position = position
 
     def get_health(self) -> float:
         return self._health
-    
+
     def set_health(self, health: float):
         self._health = health
 
-    def get_inventory(self) -> _Inventory:
+    def get_inventory(self) -> Inventory:
         return self._inventory
 
     def get_movement(self) -> IAgent.MovementKind:
         return self._movement
-    
+
     def set_movement(self, movement: IAgent.MovementKind):
         client = self._client
         if client is None:
             raise RuntimeError("Client is not running")
-        
+
         self._movement = movement
 
-        client.send(_Message({
-            "bound_to": _Message.BoundToKind.SERVER_BOUND,
-            "type": _Message.MessageKind.PERFORM_MOVE,
+        client.send(Message({
+            "bound_to": Message.BoundToKind.SERVER_BOUND.value,
+            "type": Message.MessageKind.PERFORM_MOVE.value,
             "token": self._token,
             "direction": movement.value
         }))
 
     def attack(self, interaction: IAgent.InteractionKind) -> None:
         client = self._client
         if client is None:
             raise RuntimeError("Client is not running")
         
-        client.send(_Message({
-            "bound_to": _Message.BoundToKind.SERVER_BOUND,
-            "type": _Message.MessageKind.PERFORM_ATTACK,
+        client.send(Message({
+            "bound_to": Message.BoundToKind.SERVER_BOUND.value,
+            "type": Message.MessageKind.PERFORM_ATTACK.value,
             "token": self._token,
             "attack_kind": interaction.value
         }))
 
     def jump(self) -> None:
         client = self._client
         if client is None:
             raise RuntimeError("Client is not running")
         
-        client.send(_Message({
-            "bound_to": _Message.BoundToKind.SERVER_BOUND,
-            "type": _Message.MessageKind.PERFORM_JUMP,
+        client.send(Message({
+            "bound_to": Message.BoundToKind.SERVER_BOUND.value,
+            "type": Message.MessageKind.PERFORM_JUMP.value,
             "token": self._token
         }))
 
     def look_at(self, position: Position[float]) -> None:
         client = self._client
         if client is None:
             raise RuntimeError("Client is not running")
         
-        client.send(_Message({
-            "bound_to": _Message.BoundToKind.SERVER_BOUND,
-            "type": _Message.MessageKind.PERFORM_LOOK_AT,
+        client.send(Message({
+            "bound_to": Message.BoundToKind.SERVER_BOUND.value,
+            "type": Message.MessageKind.PERFORM_LOOK_AT.value,
             "token": self._token,
             "look_at_position": {
                 "x": position.x,
                 "y": position.y,
                 "z": position.z
             }
         }))
 
     def use(self, interaction: IAgent.InteractionKind) -> None:
         client = self._client
         if client is None:
             raise RuntimeError("Client is not running")
         
-        client.send(_Message({
-            "bound_to": _Message.BoundToKind.SERVER_BOUND,
-            "type": _Message.MessageKind.PERFORM_USE,
+        client.send(Message({
+            "bound_to": Message.BoundToKind.SERVER_BOUND.value,
+            "type": Message.MessageKind.PERFORM_USE.value,
             "token": self._token,
             "use_kind": interaction.value
-        }))
+        }))
```

### Comparing `novelcraft_sdk-0.1.0/src/novelcraft/sdk/block.py` & `novelcraft_sdk-0.1.1/src/novelcraft/sdk/block.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
         Returns:
             The type ID.
         """
         raise NotImplementedError()
 
 
-class _Block(IBlock):
+class Block(IBlock):
     def __init__(self, type_id: int, position: Position[int]):
         super().__init__()
 
         self._position = position
         self._type_id = type_id
 
     def get_position(self) -> Position[int]:
```

### Comparing `novelcraft_sdk-0.1.0/src/novelcraft/sdk/block_source.py` & `novelcraft_sdk-0.1.1/src/novelcraft/sdk/block_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 """
 from __future__ import annotations
 
 import math
 from abc import ABC, abstractmethod
 from typing import Dict
 
-from .block import IBlock, _Block
+from .block import IBlock, Block
 from .position import Position
-from .section import _Section
+from .section import Section
 
 
 class IBlockSource(ABC):
     """The block source interface.
 
     The block source interface is the interface that can be used to get
     information about blocks.
@@ -29,54 +29,54 @@
 
         Returns:
             The block.
         """
         raise NotImplementedError()
 
 
-class _BlockSource(IBlockSource):
+class BlockSource(IBlockSource):
     _DEFAULT_BLOCK_ID = -1
 
     def __init__(self):
         super().__init__()
 
-        self._section_dictionary: Dict[Position[int], _Section] = {}
+        self._section_dictionary: Dict[Position[int], Section] = {}
 
-    def __getitem__(self, position: Position[int]) -> _Block | None:
+    def __getitem__(self, position: Position[int]) -> Block | None:
         section = self._get_section(position)
         if section is None:
             return None
 
         return section[Position[int](position.x - section.get_position().x,
                                 position.y - section.get_position().y,
                                 position.z - section.get_position().z)]
 
-    def __setitem__(self, position: Position[int], block: _Block) -> None:
+    def __setitem__(self, position: Position[int], block: Block) -> None:
         section = self._get_section(position)
         if section is None:
-            section = _Section(
-                position, [_BlockSource._DEFAULT_BLOCK_ID] * 4096)
+            section = Section(
+                position, [BlockSource._DEFAULT_BLOCK_ID] * 4096)
             self.add_section(section)
 
         section[Position[int](position.x - section.get_position().x,
                          position.y - section.get_position().y,
                          position.z - section.get_position().z)] = block
 
-    def add_section(self, section: _Section) -> None:
+    def add_section(self, section: Section) -> None:
         self._section_dictionary[section.get_position()] = section
 
     def clear(self) -> None:
         self._section_dictionary.clear()
 
     def remove_section(self, position: Position[int]) -> None:
         position = Position[int](16 * int(math.floor(position.x / 16)),
                             16 * int(math.floor(position.y / 16)),
                             16 * int(math.floor(position.z / 16)))
 
         self._section_dictionary.pop(position, None)
 
-    def _get_section(self, position: Position[int]) -> _Section | None:
+    def _get_section(self, position: Position[int]) -> Section | None:
         position = Position[int](16 * int(math.floor(position.x / 16)),
                             16 * int(math.floor(position.y / 16)),
                             16 * int(math.floor(position.z / 16)))
 
         return self._section_dictionary.get(position, None)
```

### Comparing `novelcraft_sdk-0.1.0/src/novelcraft/sdk/client.py` & `novelcraft_sdk-0.1.1/src/novelcraft/sdk/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import asyncio
 import json
 import queue
 from typing import Callable, List
 
 import websockets
 
-from .logger import _Logger
-from .message import _Message
+from .logger import Logger
+from .message import Message
 
 
-class _Client:
+class Client:
     _MESSAGE_TRANSMISSION_INTERVAL = 0.01
     _MESSAGE_QUEUE_CAPACITY = 100
 
     def __init__(self, host: str, port: int):
         self._connection = None
-        self._logger = _Logger("SDK.Client")
-        self._message_handler_list: List[Callable[[_Message], None]] = []
+        self._logger = Logger("SDK.Client")
+        self._message_handler_list: List[Callable[[Message], None]] = []
         self._message_queue = queue.Queue(
-            maxsize=_Client._MESSAGE_QUEUE_CAPACITY)
+            maxsize=Client._MESSAGE_QUEUE_CAPACITY)
         self._task_list: List[asyncio.Task] = []
         self._url = f"ws://{host}:{port}"
 
-    def register_message_handler(self, handler: Callable[[_Message], None]) -> None:
+    def register_message_handler(self, handler: Callable[[Message], None]) -> None:
         self._message_handler_list.append(handler)
 
     async def run(self) -> None:
-        self._connection = await _Client._try_connect(self._url)
+        self._connection = await Client._try_connect(self._url)
         self._logger.info(f"Connected to {self._url}")
 
         self._task_list.append(asyncio.create_task(self._send_loop()))
         self._task_list.append(asyncio.create_task(self._receive_loop()))
 
-    def send(self, message: _Message) -> None:
+    def send(self, message: Message) -> None:
         if self._message_queue.full():
             self._logger.error("Message queue is full, dropping message")
             return
 
         self._message_queue.put(message)
 
     async def stop(self) -> None:
@@ -45,47 +45,47 @@
 
         await self._connection.close() # type: ignore
     
     async def _receive_loop(self) -> None:
         while True:
             try:
                 json_string = await self._connection.recv()  # type: ignore
-                message = _Message(json.loads(json_string))
+                message = Message(json.loads(json_string))
 
                 handler_list = self._message_handler_list.copy()
 
                 for handler in handler_list:
                     handler(message)
 
             except Exception as e:
                 self._logger.error(f"Failed to receive message: {e}")
                 self._logger.info("Trying to reconnect...")
-                self._connection = await _Client._try_connect(self._url)
+                self._connection = await Client._try_connect(self._url)
 
     async def _send_loop(self) -> None:
         while True:
             try:
                 if not self._message_queue.empty():
-                    message: _Message = self._message_queue.get()
+                    message: Message = self._message_queue.get()
                     json_string = json.dumps(message.get_obj())
 
                     try:
                         await self._connection.send(json_string) # type: ignore
 
                     except Exception as e:
                         self._logger.error(f"Failed to send message: {e}")
 
-                await asyncio.sleep(_Client._MESSAGE_TRANSMISSION_INTERVAL)
+                await asyncio.sleep(Client._MESSAGE_TRANSMISSION_INTERVAL)
 
             except Exception as e:
                 self._logger.error(f"Unexpected error occured in send loop: {e}")
 
     @staticmethod
     async def _try_connect(url: str) -> websockets.WebSocketClientProtocol:  # type: ignore
-        logger = _Logger("SDK.Client")
+        logger = Logger("SDK.Client")
         logger.info(f"Trying to connect to {url}")
 
         is_connected = False
         while not is_connected:
             try:
                 return await websockets.connect(url)  # type: ignore
             except:
```

### Comparing `novelcraft_sdk-0.1.0/src/novelcraft/sdk/entity.py` & `novelcraft_sdk-0.1.1/src/novelcraft/sdk/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
         Returns:
             The unique ID.
         """
         raise NotImplementedError()
 
 
-class _Entity(IEntity):
+class Entity(IEntity):
     def __init__(self, type_id: int, unique_id: int, position: Position[float], orientation: Orientation[float]):
         super().__init__()
 
         self._orientation = orientation
         self._position = position
         self._type_id = type_id
         self._unique_id = unique_id
```

### Comparing `novelcraft_sdk-0.1.0/src/novelcraft/sdk/entity_source.py` & `novelcraft_sdk-0.1.1/src/novelcraft/sdk/entity_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import Dict, List
 
-from .entity import IEntity, _Entity
+from .entity import IEntity, Entity
 
 
 class IEntitySource(ABC):
     """The entity source interface.
     
     The entity source API is the API that can be used to get information about
     entities.
@@ -35,30 +35,30 @@
         """Gets all entities.
         
         Returns:
             The entities.
         """
         raise NotImplementedError()
 
-class _EntitySource(IEntitySource):
+class EntitySource(IEntitySource):
     def __init__(self):
         super().__init__()
 
-        self._entity_dictionary: Dict[int, _Entity] = {}
+        self._entity_dictionary: Dict[int, Entity] = {}
 
-    def __getitem__(self, unique_id: int) -> _Entity | None:
+    def __getitem__(self, unique_id: int) -> Entity | None:
         return self._entity_dictionary.get(unique_id, None)
     
     def __iter__(self):
         return iter(self.get_all_entities())
     
-    def add_entity(self, entity: _Entity) -> None:
+    def add_entity(self, entity: Entity) -> None:
         self._entity_dictionary[entity.get_unique_id()] = entity
 
     def clear(self) -> None:
         self._entity_dictionary.clear()
 
-    def get_all_entities(self) -> List[_Entity]:
+    def get_all_entities(self) -> List[Entity]:
         return list(self._entity_dictionary.values())
 
     def remove_entity(self, unique_id: int) -> None:
         self._entity_dictionary.pop(unique_id, None)
```

### Comparing `novelcraft_sdk-0.1.0/src/novelcraft/sdk/inventory.py` & `novelcraft_sdk-0.1.1/src/novelcraft/sdk/inventory.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 The inventory API is the API that can be used to get information about
 inventories."""
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import List
 
-from .item_stack import IItemStack, _ItemStack
-from .message import _Message
-from .client import _Client
+from .item_stack import IItemStack, ItemStack
+from .message import Message
+from .client import Client
 
 
 class IInventory(ABC):
     """The inventory interface.
 
     The inventory interface is the interface that can be used to get
     information about inventories and set items in them.
@@ -84,119 +84,119 @@
         Args:
             slot1 (int): The first slot.
             slot2 (int): The second slot.
         """
         raise NotImplementedError()
 
 
-class _Inventory(IInventory):
+class Inventory(IInventory):
     _HOTBAR_SLOTS = 9
     _SLOTS = 36
 
-    def __init__(self, client: _Client, token: str):
+    def __init__(self, client: Client, token: str):
         super().__init__()
 
         self._client = client
-        self._item_stack_list: List[_ItemStack | None] = [
-            None] * _Inventory._SLOTS
+        self._item_stack_list: List[ItemStack | None] = [
+            None] * Inventory._SLOTS
         self._main_hand_slot: int = 0
         self._token: str = token
 
-    def __getitem__(self, slot: int) -> _ItemStack | None:
-        if slot < 0 or slot >= _Inventory._SLOTS:
+    def __getitem__(self, slot: int) -> ItemStack | None:
+        if slot < 0 or slot >= Inventory._SLOTS:
             raise IndexError("Slot is out of range")
 
         return self._item_stack_list[slot]
 
-    def __setitem__(self, slot: int, item_stack: _ItemStack | None) -> None:
-        if slot < 0 or slot >= _Inventory._SLOTS:
+    def __setitem__(self, slot: int, item_stack: ItemStack | None) -> None:
+        if slot < 0 or slot >= Inventory._SLOTS:
             raise IndexError("Slot is out of range")
 
         # Copy the item stack to prevent the item stack from being modified
-        self._item_stack_list[slot] = _ItemStack(item_stack.get_type_id(), item_stack.get_count()) \
+        self._item_stack_list[slot] = ItemStack(item_stack.get_type_id(), item_stack.get_count()) \
             if item_stack is not None else None
 
     def get_main_hand_slot(self) -> int:
         return self._main_hand_slot
 
     def set_main_hand_slot(self, slot: int) -> None:
         client = self._client
         if client is None:
             raise RuntimeError("Client is not running")
 
-        if slot < 0 or slot >= _Inventory._HOTBAR_SLOTS:
+        if slot < 0 or slot >= Inventory._HOTBAR_SLOTS:
             raise IndexError("Slot is out of range")
 
         self._main_hand_slot = slot
 
-        client.send(_Message({
-            "bound_to": _Message.BoundToKind.SERVER_BOUND.value,
-            "type": _Message.MessageKind.PERFORM_SWITCH_MAIN_HAND_SLOT.value,
+        client.send(Message({
+            "bound_to": Message.BoundToKind.SERVER_BOUND.value,
+            "type": Message.MessageKind.PERFORM_SWITCH_MAIN_HAND_SLOT.value,
             "token": self._token,
             "new_main_hand": slot
         }))
 
     def craft(self, ingredients: List[int | None]) -> None:
         client = self._client
         if client is None:
             raise RuntimeError("Client is not running")
-        
-        client.send(_Message({
-            "bound_to": _Message.BoundToKind.SERVER_BOUND.value,
-            "type": _Message.MessageKind.PERFORM_CRAFT.value,
+
+        client.send(Message({
+            "bound_to": Message.BoundToKind.SERVER_BOUND.value,
+            "type": Message.MessageKind.PERFORM_CRAFT.value,
             "token": self._token,
             "item_id_sequence": ingredients
         }))
 
     def drop_item(self, slot: int, count: int) -> None:
         client = self._client
         if client is None:
             raise RuntimeError("Client is not running")
 
-        if slot < 0 or slot >= _Inventory._SLOTS:
+        if slot < 0 or slot >= Inventory._SLOTS:
             raise IndexError("Slot is out of range")
 
-        client.send(_Message({
-            "bound_to": _Message.BoundToKind.SERVER_BOUND.value,
-            "type": _Message.MessageKind.PERFORM_DROP_ITEM.value,
+        client.send(Message({
+            "bound_to": Message.BoundToKind.SERVER_BOUND.value,
+            "type": Message.MessageKind.PERFORM_DROP_ITEM.value,
             "token": self._token,
             "drop_items": [{
                 "slot": slot,
                 "count": count
             }]
         }))
 
     def merge_slots(self, from_slot: int, to_slot: int) -> None:
         client = self._client
         if client is None:
             raise RuntimeError("Client is not running")
 
-        if from_slot < 0 or from_slot >= _Inventory._SLOTS:
+        if from_slot < 0 or from_slot >= Inventory._SLOTS:
             raise IndexError("From slot is out of range")
-        if to_slot < 0 or to_slot >= _Inventory._SLOTS:
+        if to_slot < 0 or to_slot >= Inventory._SLOTS:
             raise IndexError("To slot is out of range")
 
-        client.send(_Message({
-            "bound_to": _Message.BoundToKind.SERVER_BOUND.value,
-            "type": _Message.MessageKind.PERFORM_MERGE_SLOTS.value,
+        client.send(Message({
+            "bound_to": Message.BoundToKind.SERVER_BOUND.value,
+            "type": Message.MessageKind.PERFORM_MERGE_SLOTS.value,
             "token": self._token,
             "from_slot": from_slot,
             "to_slot": to_slot
         }))
 
     def swap_slots(self, slot1: int, slot2: int) -> None:
         client = self._client
         if client is None:
             raise RuntimeError("Client is not running")
 
-        if slot1 < 0 or slot1 >= _Inventory._SLOTS:
+        if slot1 < 0 or slot1 >= Inventory._SLOTS:
             raise IndexError("Slot 1 is out of range")
-        if slot2 < 0 or slot2 >= _Inventory._SLOTS:
+        if slot2 < 0 or slot2 >= Inventory._SLOTS:
             raise IndexError("Slot 2 is out of range")
 
-        client.send(_Message({
-            "bound_to": _Message.BoundToKind.SERVER_BOUND.value,
-            "type": _Message.MessageKind.PERFORM_SWAP_SLOTS.value,
+        client.send(Message({
+            "bound_to": Message.BoundToKind.SERVER_BOUND.value,
+            "type": Message.MessageKind.PERFORM_SWAP_SLOTS.value,
             "token": self._token,
             "slot_a": slot1,
             "slot_b": slot2
-        }))
+        }))
```

### Comparing `novelcraft_sdk-0.1.0/src/novelcraft/sdk/item_stack.py` & `novelcraft_sdk-0.1.1/src/novelcraft/sdk/item_stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         """Gets the type ID of the item stack.
         
         Returns:
             The type ID.
         """
         raise NotImplementedError()
     
-class _ItemStack(IItemStack):
+class ItemStack(IItemStack):
     def __init__(self, type_id: int, count: int):
         super().__init__()
         
         self._count = count
         self._type_id = type_id
 
     def get_count(self) -> int:
```

### Comparing `novelcraft_sdk-0.1.0/src/novelcraft/sdk/logger.py` & `novelcraft_sdk-0.1.1/src/novelcraft/sdk/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
         Args:
             message (str): The message to log.
         """
         raise NotImplementedError
 
 
-class _Logger(ILogger):
+class Logger(ILogger):
     _FORMAT = ""
 
     _lock = threading.Lock()
 
     def __init__(self, namespace: str) -> None:
         super().__init__()
 
@@ -69,37 +69,37 @@
 
         self._namespace = namespace
 
     def debug(self, message: str) -> None:
         if not self._debug:
             return
         
-        with _Logger._lock:
-            cprint(f'{_Logger._get_current_time_string()} ', color='cyan', end='')
+        with Logger._lock:
+            cprint(f'{Logger._get_current_time_string()} ', color='cyan', end='')
             cprint(f'DEBUG ', color='dark_grey', end='')
             cprint(f'[{self._namespace}] {message}', color='dark_grey', end='')
             print()
 
     def info(self, message: str) -> None:
-        with _Logger._lock:
-            cprint(f'{_Logger._get_current_time_string()} ', color='cyan', end='')
+        with Logger._lock:
+            cprint(f'{Logger._get_current_time_string()} ', color='cyan', end='')
             cprint(f'INFO  ', color='blue', end='')
             cprint(f'[{self._namespace}] {message}', color='white', end='')
             print()
 
     def warn(self, message: str) -> None:
-        with _Logger._lock:
-            cprint(f'{_Logger._get_current_time_string()} ', color='cyan', end='')
+        with Logger._lock:
+            cprint(f'{Logger._get_current_time_string()} ', color='cyan', end='')
             cprint(f'WARN  ', color='yellow', end='')
             cprint(f'[{self._namespace}] {message}', color='yellow', end='')
             print()
 
     def error(self, message: str) -> None:
-        with _Logger._lock:
-            cprint(f'{_Logger._get_current_time_string()} ', color='cyan', end='')
+        with Logger._lock:
+            cprint(f'{Logger._get_current_time_string()} ', color='cyan', end='')
             cprint(f'ERROR ', color='red', end='')
             cprint(f'[{self._namespace}] {message}', color='red', end='')
             print()
 
     @staticmethod
     def _get_current_time_string() -> str:
         return datetime.now().strftime(f'%H:%M:%S')
```

### Comparing `novelcraft_sdk-0.1.0/src/novelcraft/sdk/message.py` & `novelcraft_sdk-0.1.1/src/novelcraft/sdk/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 from typing import Any, Dict
 
 import jsonschema
 
 
-class _Message:
+class Message:
     class BoundToKind(Enum):
         """The bound to kind."""
         SERVER_BOUND = 0
         CLIENT_BOUND = 1
 
     class MessageKind(Enum):
         """The message kind."""
@@ -62,15 +62,15 @@
         "required": [
             "bound_to",
             "type"
         ]
     }
 
     def __init__(self, obj: Dict[str, Any]):
-        validator = jsonschema.Draft7Validator(_Message._JSON_SCHEMA)
+        validator = jsonschema.Draft7Validator(Message._JSON_SCHEMA)
         if not validator.is_valid(obj):
             raise ValueError("The JSON is not valid.")
 
         self._json = obj
 
     def __getitem__(self, key: str) -> Any:
         return self._json[key]
```

### Comparing `novelcraft_sdk-0.1.0/src/novelcraft/sdk/sdk.py` & `novelcraft_sdk-0.1.1/src/novelcraft/sdk/sdk.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,49 +11,49 @@
 from __future__ import annotations
 
 import argparse
 import asyncio
 from dataclasses import dataclass
 from datetime import datetime
 
-from .agent import IAgent, _Agent
-from .block import _Block
-from .block_source import IBlockSource, _BlockSource
-from .client import _Client
-from .entity import _Entity
-from .entity_source import IEntitySource, _EntitySource
-from .item_stack import _ItemStack
-from .logger import ILogger, _Logger
-from .message import _Message
+from .agent import IAgent, Agent
+from .block import Block
+from .block_source import IBlockSource, BlockSource
+from .client import Client
+from .entity import Entity
+from .entity_source import IEntitySource, EntitySource
+from .item_stack import ItemStack
+from .logger import ILogger, Logger
+from .message import Message
 from .orientation import Orientation
 from .position import Position
-from .section import _Section
-from .inventory import _Inventory
+from .section import Section
+from .inventory import Inventory
 
 
 @dataclass
 class _TickInfo:
     """The tick info."""
     tick: int
     time: datetime
 
 
 GET_INFO_INTERVAL = 1
 PING_INVERVAL = 1
 
-_agent: _Agent | None = None
-_block_source: _BlockSource | None = None
-_client: _Client | None = None
-_entity_source: _EntitySource | None = None
+_agent: Agent | None = None
+_block_source: BlockSource | None = None
+_client: Client | None = None
+_entity_source: EntitySource | None = None
 _tick_info: _TickInfo | None = None
 _task_list: list[asyncio.Task] = []
 _token: str | None = None
 _tps: float | None = None
-_sdk_logger: _Logger = _Logger('SDK')
-_user_logger: _Logger = _Logger('User')
+_sdk_logger: Logger = Logger('SDK')
+_user_logger: Logger = Logger('User')
 
 
 async def finalize() -> None:
     """Finalizes the SDK.
 
     This function should be called when the program is about to exit.
     """
@@ -78,15 +78,15 @@
 
         parser = argparse.ArgumentParser()
         parser.add_argument('--host', type=str, default='localhost')
         parser.add_argument('--port', type=int, default=14514)
         parser.add_argument('--token', type=str, default='')
         args = parser.parse_args()
 
-        _client = _Client(args.host, args.port)
+        _client = Client(args.host, args.port)
         _client.register_message_handler(_message_handler)
         await _client.run()
 
         _token = args.token
 
         async def get_info_loop():
             while True:
@@ -163,65 +163,65 @@
 
     Returns:
         The TPS. None if the TPS is not initialized.
     """
     return _tps
 
 
-def _message_handler(message: _Message) -> None:
+def _message_handler(message: Message) -> None:
     try:
         global _block_source, _entity_source, _agent, _tick_info, _tps
 
-        if message.get_bound_to() != _Message.BoundToKind.CLIENT_BOUND.value:
+        if message.get_bound_to() != Message.BoundToKind.CLIENT_BOUND.value:
             return
 
-        if message.get_type() == _Message.MessageKind.ERROR.value:
+        if message.get_type() == Message.MessageKind.ERROR.value:
             _sdk_logger.error(
                 f'The server returned an error: {message.get_obj()["message"]}')
 
-        elif message.get_type() == _Message.MessageKind.AFTER_BLOCK_CHANGE.value:
+        elif message.get_type() == Message.MessageKind.AFTER_BLOCK_CHANGE.value:
             if _block_source is None:
                 return
 
             for block_change in message.get_obj()['change_list']:
                 position = Position[int](block_change['position']['x'],
                                          block_change['position']['y'],
                                          block_change['position']['z'])
-                _block_source[position] = _Block(type_id=block_change['block_type_id'],
+                _block_source[position] = Block(type_id=block_change['block_type_id'],
                                                  position=position)
 
-        elif message.get_type() == _Message.MessageKind.AFTER_ENTITY_CREATE.value:
+        elif message.get_type() == Message.MessageKind.AFTER_ENTITY_CREATE.value:
             if _entity_source is None:
                 return
 
             for creation in message.get_obj()['creation_list']:
-                _entity_source.add_entity(_Entity(type_id=creation['entity_type_id'],
+                _entity_source.add_entity(Entity(type_id=creation['entity_type_id'],
                                                   unique_id=creation['unique_id'],
                                                   position=Position[float](creation['position']['x'],
                                                                            creation['position']['y'],
                                                                            creation['position']['z']),
                                                   orientation=Orientation[float](creation['orientation']['yaw'],
                                                                                  creation['orientation']['pitch'])))
 
-        elif message.get_type() == _Message.MessageKind.AFTER_ENTITY_ORIENTATION_CHANGE.value:
+        elif message.get_type() == Message.MessageKind.AFTER_ENTITY_ORIENTATION_CHANGE.value:
             if _entity_source is None:
                 return
 
             for orientation_change in message.get_obj()['change_list']:
                 entity = _entity_source[orientation_change['unique_id']]
                 if entity is None:
                     continue
 
                 entity.set_orientation(Orientation[float](orientation_change['orientation']['yaw'],
                                                           orientation_change['orientation']['pitch']))
 
                 if _agent is not None and _agent.get_unique_id() == entity.get_unique_id():
                     _agent.set_orientation(entity.get_orientation())
 
-        elif message.get_type() == _Message.MessageKind.AFTER_ENTITY_POSITION_CHANGE.value:
+        elif message.get_type() == Message.MessageKind.AFTER_ENTITY_POSITION_CHANGE.value:
             if _entity_source is None:
                 return
 
             for position_change in message.get_obj()['change_list']:
                 entity = _entity_source[position_change['unique_id']]
                 if entity is None:
                     continue
@@ -229,128 +229,144 @@
                 entity.set_position(Position[float](position_change['position']['x'],
                                                     position_change['position']['y'],
                                                     position_change['position']['z']))
 
                 if _agent is not None and _agent.get_unique_id() == entity.get_unique_id():
                     _agent.set_position(entity.get_position())
 
-        elif message.get_type() == _Message.MessageKind.AFTER_ENTITY_REMOVE.value:
+        elif message.get_type() == Message.MessageKind.AFTER_ENTITY_REMOVE.value:
             if _entity_source is None:
                 return
 
             for removal in message.get_obj()['removal_id_list']:
                 _entity_source.remove_entity(removal)
 
-        elif message.get_type() == _Message.MessageKind.AFTER_PLAYER_INVENTORY_CHANGE.value:
+        elif message.get_type() == Message.MessageKind.AFTER_PLAYER_INVENTORY_CHANGE.value:
             if _agent is None:
                 return
 
             for change in message.get_obj()['change_list']:
                 if change['player_unique_id'] is not _agent.get_unique_id():
                     continue
 
                 for slot_change in change['change_list']:
                     _agent.get_inventory()[slot_change['slot']] = None if slot_change['item_type_id'] is None \
-                        else _ItemStack(type_id=slot_change['item_type_id'],
+                        else ItemStack(type_id=slot_change['item_type_id'],
                                         count=slot_change['count'])
 
-        elif message.get_type() == _Message.MessageKind.GET_BLOCKS_AND_ENTITIES.value:
-            _block_source = _BlockSource()
-            _entity_source = _EntitySource()
+        elif message.get_type() == Message.MessageKind.GET_BLOCKS_AND_ENTITIES.value:
+            _block_source = BlockSource()
+            _entity_source = EntitySource()
 
             for section in message.get_obj()['sections']:
-                _block_source.add_section(_Section(position=Position[int](section['position']['x'],
+                _block_source.add_section(Section(position=Position[int](section['position']['x'],
                                                                           section['position']['y'],
                                                                           section['position']['z']),
                                                    block_id_list=section['blocks']))
 
             for entity in message.get_obj()['entities']:
-                _entity_source.add_entity(_Entity(type_id=entity['type_id'],
+                _entity_source.add_entity(Entity(type_id=entity['type_id'],
                                                   unique_id=entity['unique_id'],
                                                   position=Position[float](entity['position']['x'],
                                                                            entity['position']['y'],
                                                                            entity['position']['z']),
                                                   orientation=Orientation[float](entity['orientation']['yaw'],
                                                                                  entity['orientation']['pitch'])))
 
                 if _agent is not None and _agent.get_unique_id() == entity['unique_id']:
                     _agent.set_position(Position[float](entity['position']['x'],
                                                         entity['position']['y'],
                                                         entity['position']['z']))
                     _agent.set_orientation(Orientation[float](entity['orientation']['yaw'],
                                                               entity['orientation']['pitch']))
 
-        elif message.get_type() == _Message.MessageKind.GET_PLAYER_INFO.value:
+        elif message.get_type() == Message.MessageKind.GET_PLAYER_INFO.value:
             if _client is None:
                 return
             if _token is None:
                 return
 
             player_info = message.get_obj()
             if _agent is None:
                 # Create a new agent
-                _agent = _Agent(client=_client,
+                _agent = Agent(client=_client,
                                 token=_token,
                                 unique_id=player_info["unique_id"],
                                 position=Position[float](
                                     player_info["position"]['x'],
                                     player_info["position"]['y'],
                                     player_info["position"]['z']
                                 ),
                                 orientation=Orientation[float](
                                     player_info['orientation']['yaw'],
                                     player_info['orientation']['pitch']
                                 )
                                 )
 
+                agent_position = _agent.get_position()
+                agent_position = _agent.get_position()
+
+                request_section_list = [{
+                    'x': int(agent_position.x + x*16),
+                    'y': int(agent_position.y + y*16),
+                    'z': int(agent_position.z + z*16)
+                } for x in range(-1, 2) for y in range(-1, 2) for z in range(-1, 2)]
+
+                # Send get blocks and entities message
+                _client.send(Message({
+                    "bound_to": Message.BoundToKind.SERVER_BOUND.value,
+                    "type": Message.MessageKind.GET_BLOCKS_AND_ENTITIES.value,
+                    "token": _token,
+                    "request_section_list": request_section_list})
+                )
+
             # Update Info
             _agent.set_health(player_info['health'])
             _agent.set_position(Position[float](
                 player_info["position"]['x'],
                 player_info["position"]['y'],
                 player_info["position"]['z']
             ))
             _agent.set_orientation(Orientation[float](player_info['orientation']['yaw'],
                                                       player_info['orientation']['pitch']))
             # Main slots
             _agent.get_inventory()._main_hand_slot = int(
                 player_info['main_hand'])
             # inventory
-            for slot in range(_Inventory._SLOTS):
+            for slot in range(Inventory._SLOTS):
                 item_stack = player_info['inventory'][slot]
                 if item_stack is not None:
-                    _agent.get_inventory()[slot] = _ItemStack(
+                    _agent.get_inventory()[slot] = ItemStack(
                         item_stack['type_id'], item_stack['count'])
 
-        elif message.get_type() == _Message.MessageKind.GET_TICK.value:
+        elif message.get_type() == Message.MessageKind.GET_TICK.value:
             tick_message = message.get_obj()
             _tick_info = _TickInfo(tick_message['tick'], datetime.now())
             _tps = tick_message['ticks_per_second']
 
     except Exception as e:
         _sdk_logger.error(f'Error while handling message: {e}')
 
 
 async def _get_info():
     global _client
-
     if _client is None:
         return
 
     # Send get tick message
-    _client.send(_Message({
-        "bound_to": _Message.BoundToKind.SERVER_BOUND.value,
-        "type": _Message.MessageKind.GET_TICK.value,
+    _client.send(Message({
+        "bound_to": Message.BoundToKind.SERVER_BOUND.value,
+        "type": Message.MessageKind.GET_TICK.value,
         "token": _token,
     }))
 
     # Send get player info message
-    _client.send(_Message({
-        "bound_to": _Message.BoundToKind.SERVER_BOUND.value,
-        "type": _Message.MessageKind.GET_PLAYER_INFO.value,
+    _client.send(Message({
+        "bound_to": Message.BoundToKind.SERVER_BOUND.value,
+        "type": Message.MessageKind.GET_PLAYER_INFO.value,
         "token": _token,
     }))
 
     # Compute near section
     if _agent is not None:
         agent_position = _agent.get_position()
         agent_position = _agent.get_position()
@@ -358,13 +374,13 @@
         request_section_list = [{
             'x': int(agent_position.x + x*16),
             'y': int(agent_position.y + y*16),
             'z': int(agent_position.z + z*16)
         } for x in range(-1, 2) for y in range(-1, 2) for z in range(-1, 2)]
 
         # Send get blocks and entities message
-        _client.send(_Message({
-            "bound_to": _Message.BoundToKind.SERVER_BOUND.value,
-            "type": _Message.MessageKind.GET_BLOCKS_AND_ENTITIES.value,
+        _client.send(Message({
+            "bound_to": Message.BoundToKind.SERVER_BOUND.value,
+            "type": Message.MessageKind.GET_BLOCKS_AND_ENTITIES.value,
             "token": _token,
             "request_section_list": request_section_list})
         )
```

### Comparing `novelcraft_sdk-0.1.0/src/novelcraft/sdk/section.py` & `novelcraft_sdk-0.1.1/src/novelcraft/sdk/section.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import List
 
 from .position import Position
-from .block import _Block
+from .block import Block
 
 
-class _Section:
+class Section:
     def __init__(self, position: Position[int], block_id_list: List[int]):
         if position.x % 16 != 0 or position.y % 16 != 0 or position.z % 16 != 0:
             raise ValueError("The position must be a multiple of 16.")
 
         if len(block_id_list) != 4096:
             raise ValueError("The block ID list must have a length of 4096.")
 
         self._block_id_list = block_id_list
         self._position = position
 
-    def __getitem__(self, position: Position[int]) -> _Block:
+    def __getitem__(self, position: Position[int]) -> Block:
         if position.x < 0 or position.x > 15 \
            or position.y < 0 or position.y > 15 \
            or position.z < 0 or position.z > 15:
             raise IndexError("The position is out of range.")
 
-        return _Block(self._block_id_list[position.x * 256 + position.y * 16 + position.z],
+        return Block(self._block_id_list[position.x * 256 + position.y * 16 + position.z],
                       position)
 
-    def __setitem__(self, position: Position[int], block: _Block):
+    def __setitem__(self, position: Position[int], block: Block):
         if position.x < 0 or position.x > 15 \
            or position.y < 0 or position.y > 15 \
            or position.z < 0 or position.z > 15:
             raise IndexError("The position is out of range.")
 
         self._block_id_list[position.x * 256 + position.y * 16 + position.z] = block.get_type_id()
```

### Comparing `novelcraft_sdk-0.1.0/PKG-INFO` & `novelcraft_sdk-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: novelcraft-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library for communicating with NovelCraft Servers and accessing NovelCraft game data
 License: Unlicense
 Author: NovelCraft
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -37,15 +37,15 @@
 
 
 async def main():
     await sdk.initialize()
 
     # Do something
 
-    await ncsdk.finalize()
+    await sdk.finalize()
 
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
 For more information, please start with _placeholder_.
```

