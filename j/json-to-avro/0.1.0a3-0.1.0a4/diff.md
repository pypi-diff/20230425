# Comparing `tmp/json_to_avro-0.1.0a3.tar.gz` & `tmp/json_to_avro-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_to_avro-0.1.0a3.tar", max compression
+gzip compressed data, was "json_to_avro-0.1.0a4.tar", max compression
```

## Comparing `json_to_avro-0.1.0a3.tar` & `json_to_avro-0.1.0a4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-04-04 02:26:42.522535 json_to_avro-0.1.0a3/LICENSE
--rw-r--r--   0        0        0      164 2023-04-04 02:26:42.522747 json_to_avro-0.1.0a3/README.md
--rw-r--r--   0        0        0      194 2023-04-13 03:08:27.218434 json_to_avro-0.1.0a3/json_to_avro/__init__.py
--rw-r--r--   0        0        0      319 2023-04-21 00:04:25.942111 json_to_avro-0.1.0a3/json_to_avro/avro_schema/__init__.py
--rw-r--r--   0        0        0      369 2023-04-13 10:47:53.464735 json_to_avro-0.1.0a3/json_to_avro/avro_schema/avro_schema_candidate.py
--rw-r--r--   0        0        0    21973 2023-04-16 04:07:57.682016 json_to_avro-0.1.0a3/json_to_avro/avro_schema/mergeable_avro_schema.py
--rw-r--r--   0        0        0      627 2023-04-13 03:07:50.323202 json_to_avro-0.1.0a3/json_to_avro/avro_schema/registered_avro_schema.py
--rw-r--r--   0        0        0      236 2023-04-13 03:07:50.323401 json_to_avro-0.1.0a3/json_to_avro/avroable_data.py
--rw-r--r--   0        0        0     2385 2023-04-13 03:07:50.323603 json_to_avro-0.1.0a3/json_to_avro/json_to_avro.py
--rw-r--r--   0        0        0     2816 2023-04-21 00:30:05.218588 json_to_avro-0.1.0a3/json_to_avro/schema_provider.py
--rw-r--r--   0        0        0      733 2023-04-21 00:31:11.857365 json_to_avro-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0      831 1970-01-01 00:00:00.000000 json_to_avro-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-04 02:26:42.522535 json_to_avro-0.1.0a4/LICENSE
+-rw-r--r--   0        0        0      164 2023-04-04 02:26:42.522747 json_to_avro-0.1.0a4/README.md
+-rw-r--r--   0        0        0      181 2023-04-21 02:50:16.396050 json_to_avro-0.1.0a4/json_to_avro/__init__.py
+-rw-r--r--   0        0        0      318 2023-04-21 02:50:16.396070 json_to_avro-0.1.0a4/json_to_avro/avro_schema/__init__.py
+-rw-r--r--   0        0        0      370 2023-04-21 02:50:16.396112 json_to_avro-0.1.0a4/json_to_avro/avro_schema/avro_schema_candidate.py
+-rw-r--r--   0        0        0    22313 2023-04-21 02:52:56.851824 json_to_avro-0.1.0a4/json_to_avro/avro_schema/mergeable_avro_schema.py
+-rw-r--r--   0        0        0      628 2023-04-21 02:50:16.396129 json_to_avro-0.1.0a4/json_to_avro/avro_schema/registered_avro_schema.py
+-rw-r--r--   0        0        0      237 2023-04-21 02:50:16.396127 json_to_avro-0.1.0a4/json_to_avro/avroable_data.py
+-rw-r--r--   0        0        0     2356 2023-04-21 02:50:16.414581 json_to_avro-0.1.0a4/json_to_avro/json_to_avro.py
+-rw-r--r--   0        0        0     2902 2023-04-25 01:38:47.080110 json_to_avro-0.1.0a4/json_to_avro/schema_provider.py
+-rw-r--r--   0        0        0      733 2023-04-25 01:38:59.271163 json_to_avro-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0      831 1970-01-01 00:00:00.000000 json_to_avro-0.1.0a4/PKG-INFO
```

### Comparing `json_to_avro-0.1.0a3/LICENSE` & `json_to_avro-0.1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `json_to_avro-0.1.0a3/json_to_avro/avro_schema/mergeable_avro_schema.py` & `json_to_avro-0.1.0a4/json_to_avro/avro_schema/mergeable_avro_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,25 +11,24 @@
     int: "long",
     float: "double",
     bool: "boolean",
     list: "array",
     dict: "record",
 }
 
+
 @dataclasses.dataclass
 class MergeableAvroSchema:
     schema_dict: dict
 
     def __add__(self, other: "MergeableAvroSchema") -> "MergeableAvroSchema":
         return self.merge_schemas(self.schema_dict, other.schema_dict)
 
     @classmethod
-    def merge_schemas(
-        cls, self_data: dict, other_data: dict
-    ) -> "MergeableAvroSchema":
+    def merge_schemas(cls, self_data: dict, other_data: dict) -> "MergeableAvroSchema":
         return cls(cls._merge_schemas(self_data, other_data))
 
     @classmethod
     def _merge_schemas(
         cls,
         self_data: Any,
         other_data: Any,
@@ -175,29 +174,38 @@
                 ) if t not in types:
                     updated_fields[name] = {
                         **updated_fields[name],
                         "type": [*types, t],
                     }
                 case (
                     {"name": name, "type": list(types1)},
-                    {"name": _, "type": list(types2), "default": None}
+                    {"name": _, "type": list(types2), "default": None},
                 ) if types1 == types2 and "default" not in updated_fields[name]:
                     updated_fields[name] = {
                         **updated_fields[name],
                         "type": types1,
-                        "default": None
+                        "default": None,
                     }
                 case (
                     {"name": _, "type": list(types1), "default": None},
                     {"name": name, "type": list(types2)},
                 ) if types1 == types2 and "default" not in field:
                     updated_fields[name] = {
                         **updated_fields[name],
                         "type": types1,
-                        "default": None
+                        "default": None,
+                    }
+                case (
+                    {"name": name, "type": ["null", dict(_) as type1] as type},
+                    {"name": _, "type": dict(_) as type2},
+                ) if type1 == type2:
+                    updated_fields[name] = {
+                        **updated_fields[name],
+                        "type": type,
+                        "default": None,
                     }
                 case (
                     {
                         "name": _,
                         "type": ("string" | "boolean" | "long" | "double") as t,
                     },
                     {"name": name, "type": list(types)},
@@ -465,23 +473,19 @@
     @property
     def schema_str(self) -> str:
         return json.dumps(self.schema_dict)
 
     @classmethod
     def from_avroable_data(cls, msg: AvroableData) -> "MergeableAvroSchema":
         return cls(
-            schema_dict=cls.convert_json_to_avro_schema(
-                msg.data, msg.record_name
-            ),
+            schema_dict=cls.convert_json_to_avro_schema(msg.data, msg.record_name),
         )
 
     @staticmethod
-    def convert_json_to_avro_schema(
-        json_data: Any, name: str
-    ) -> dict:
+    def convert_json_to_avro_schema(json_data: Any, name: str) -> dict:
         avro_schema: dict = {"type": "record", "name": name, "fields": []}
 
         for key, value in json_data.items():
             match value:
                 case dict(_):
                     avro_schema["fields"].append(
                         {
@@ -534,8 +538,8 @@
     @classmethod
     def sum_schemas(cls, items, name):
         item_iter = items.__iter__()
         schema = cls(cls.convert_json_to_avro_schema(next(item_iter), name))
         for item in item_iter:
             schema += cls(cls.convert_json_to_avro_schema(item, name))
 
-        return schema.schema_dict
+        return schema.schema_dict
```

### Comparing `json_to_avro-0.1.0a3/json_to_avro/avro_schema/registered_avro_schema.py` & `json_to_avro-0.1.0a4/json_to_avro/avro_schema/registered_avro_schema.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
     @classmethod
     def from_schema_version(
         cls, schema_version: SchemaVersion
     ) -> "RegisteredAvroSchema":
         return cls(
             MergeableAvroSchema(schema_version.schema.flat_schema),
             RegisteredAvroSchemaId(schema_version.schema_id),
-        )
+        )
```

### Comparing `json_to_avro-0.1.0a3/json_to_avro/json_to_avro.py` & `json_to_avro-0.1.0a4/json_to_avro/json_to_avro.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,29 +18,30 @@
     def __init__(self, provider: SchemaProvider, serializer: AvroMessageSerializer):
         self.provider = provider
         self.serializer = serializer
 
     @classmethod
     def from_config(cls, config: JsonToAvroConfig):
         schema_registry = SchemaRegistryClient(url=config.schema_registry_url)
-        return cls(SchemaProvider({}, schema_registry), AvroMessageSerializer(schema_registry))
+        return cls(
+            SchemaProvider({}, schema_registry), AvroMessageSerializer(schema_registry)
+        )
 
     def serialize_as_avro(
         self,
         msg: AvroableData,
     ) -> bytes:
         schema_candidate = AvroSchemaCandidate.from_avroable_data(msg)
         maybe_existing_registered_schema = self.provider.get(msg.subject_name)
         logger.debug("Existing Schema: %s" % maybe_existing_registered_schema)
         schema_id: RegisteredAvroSchemaId = (
             maybe_existing_registered_schema.schema_id
             if maybe_existing_registered_schema is not None
             else self.provider.register_and_set(msg.subject_name, schema_candidate)
         )
-        logger.debug("Registered Schema: %s", self.provider[msg.subject_name])
 
         try:
             return self.serializer.encode_record_with_schema_id(schema_id, msg.data)
         except (ValueError, KeyError, TypeError, AttributeError) as e:
             logger.debug(f"Schema mismatch: {e}")
             logger.debug(
                 "existing schema: %s" % maybe_existing_registered_schema.schema
@@ -48,12 +49,12 @@
                 else None,
             )
             logger.debug("Message data: %s" % msg.data)
             new_schema_candidate = AvroSchemaCandidate(
                 self.provider[msg.subject_name].schema + schema_candidate.schema
             )
             logger.debug("New Schema Candidate: %s" % new_schema_candidate)
-            schema_id = self.provider.register_and_set(msg.subject_name, new_schema_candidate)
+            schema_id = self.provider.register_and_set(
+                msg.subject_name, new_schema_candidate
+            )
 
             return self.serializer.encode_record_with_schema_id(schema_id, msg.data)
-
-
```

### Comparing `json_to_avro-0.1.0a3/json_to_avro/schema_provider.py` & `json_to_avro-0.1.0a4/json_to_avro/schema_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,60 @@
 import functools
 from typing import Callable, Optional
 
 from schema_registry.client import AsyncSchemaRegistryClient, SchemaRegistryClient
 from schema_registry.client.utils import SchemaVersion
 
 from json_to_avro.avro_schema.avro_schema_candidate import AvroSchemaCandidate
-from json_to_avro.avro_schema.registered_avro_schema import RegisteredAvroSchema, RegisteredAvroSchemaId
+from json_to_avro.avro_schema.registered_avro_schema import (
+    RegisteredAvroSchema,
+    RegisteredAvroSchemaId,
+)
 from loguru import logger
 
 
-def ensure_backwards_transitive_compatibility(func: Callable) -> Callable:
+def ensure_backward_transitive_compatibility(func: Callable) -> Callable:
     @functools.wraps(func)
     def wraps(*args):
         self, subject, *_ = args
         if subject not in self.current_schema_table:
-            logger.debug("Setting compatibility to BACKWARD_TRANSITIVE for %s" % subject)
-            self.schema_registry_client.update_compatibility("BACKWARD_TRANSITIVE", subject)
+            logger.debug(
+                "Setting compatibility to BACKWARD_TRANSITIVE for %s" % subject
+            )
+            self.schema_registry_client.update_compatibility(
+                "BACKWARD_TRANSITIVE", subject
+            )
         return func(*args)
+
     return wraps
 
 
 class SchemaProvider:
     def __init__(
         self,
         current_schema_table: dict[str, RegisteredAvroSchema],
         schema_registry_client: SchemaRegistryClient,
     ):
         self.current_schema_table = current_schema_table
         self.schema_registry_client = schema_registry_client
 
     @classmethod
-    def from_schema_registry_client(cls, client: SchemaRegistryClient | AsyncSchemaRegistryClient):
+    def from_schema_registry_client(
+        cls, client: SchemaRegistryClient | AsyncSchemaRegistryClient
+    ):
         current_schema_table: dict[str, RegisteredAvroSchema] = {}
         return cls(current_schema_table, client)
 
     def __getitem__(self, subject: str) -> RegisteredAvroSchema:
         """Unsafe version of `get`
         :raises KeyError
         """
         return self.current_schema_table[subject]
 
-    @ensure_backwards_transitive_compatibility
+    @ensure_backward_transitive_compatibility
     def get(self, subject_name: str) -> RegisteredAvroSchema | None:
         if subject_name in self.current_schema_table:
             return self.current_schema_table[subject_name]
 
         schema_version: SchemaVersion | None = self.schema_registry_client.get_schema(
             subject_name, version="latest"
         )
```

### Comparing `json_to_avro-0.1.0a3/pyproject.toml` & `json_to_avro-0.1.0a4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "json-to-avro"
-version = "0.1.0a3"
+version = "0.1.0a4"
 description = "Convert arbitrary JSON data to avro serialized data, registering transitively backwards compatible schemas with Kafka Schema Registry along the way."
 authors = ["Brad Boggs <bboggs@streambit.software>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "json_to_avro"}]
 
 [tool.poetry.dependencies]
```

### Comparing `json_to_avro-0.1.0a3/PKG-INFO` & `json_to_avro-0.1.0a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-to-avro
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: Convert arbitrary JSON data to avro serialized data, registering transitively backwards compatible schemas with Kafka Schema Registry along the way.
 License: MIT
 Author: Brad Boggs
 Author-email: bboggs@streambit.software
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

