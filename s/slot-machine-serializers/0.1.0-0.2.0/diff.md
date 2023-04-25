# Comparing `tmp/slot_machine_serializers-0.1.0.tar.gz` & `tmp/slot_machine_serializers-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slot_machine_serializers-0.1.0.tar", last modified: Fri Apr 21 09:05:52 2023, max compression
+gzip compressed data, was "slot_machine_serializers-0.2.0.tar", last modified: Tue Apr 25 08:48:47 2023, max compression
```

## Comparing `slot_machine_serializers-0.1.0.tar` & `slot_machine_serializers-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-21 09:05:52.151545 slot_machine_serializers-0.1.0/
--rw-r--r--   0 ochsner    (502) staff       (20)     1924 2023-04-21 09:05:52.151653 slot_machine_serializers-0.1.0/PKG-INFO
--rw-r--r--   0 ochsner    (502) staff       (20)     1666 2023-04-12 13:31:21.000000 slot_machine_serializers-0.1.0/README.md
--rw-r--r--   0 ochsner    (502) staff       (20)       90 2023-04-06 15:49:44.000000 slot_machine_serializers-0.1.0/pyproject.toml
--rw-r--r--   0 ochsner    (502) staff       (20)      595 2023-04-21 09:05:52.152017 slot_machine_serializers-0.1.0/setup.cfg
-drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-21 09:05:52.149580 slot_machine_serializers-0.1.0/slot_machine/
--rw-r--r--   0 ochsner    (502) staff       (20)       51 2023-04-06 16:45:57.000000 slot_machine_serializers-0.1.0/slot_machine/__init__.py
--rw-r--r--   0 ochsner    (502) staff       (20)     2267 2023-04-12 13:20:58.000000 slot_machine_serializers-0.1.0/slot_machine/samplers.py
--rw-r--r--   0 ochsner    (502) staff       (20)     3836 2023-04-06 15:49:44.000000 slot_machine_serializers-0.1.0/slot_machine/serializers.py
-drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-21 09:05:52.150631 slot_machine_serializers-0.1.0/slot_machine_serializers.egg-info/
--rw-r--r--   0 ochsner    (502) staff       (20)     1924 2023-04-21 09:05:52.000000 slot_machine_serializers-0.1.0/slot_machine_serializers.egg-info/PKG-INFO
--rw-r--r--   0 ochsner    (502) staff       (20)      400 2023-04-21 09:05:52.000000 slot_machine_serializers-0.1.0/slot_machine_serializers.egg-info/SOURCES.txt
--rw-r--r--   0 ochsner    (502) staff       (20)        1 2023-04-21 09:05:52.000000 slot_machine_serializers-0.1.0/slot_machine_serializers.egg-info/dependency_links.txt
--rw-r--r--   0 ochsner    (502) staff       (20)       49 2023-04-21 09:05:52.000000 slot_machine_serializers-0.1.0/slot_machine_serializers.egg-info/requires.txt
--rw-r--r--   0 ochsner    (502) staff       (20)       13 2023-04-21 09:05:52.000000 slot_machine_serializers-0.1.0/slot_machine_serializers.egg-info/top_level.txt
-drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-21 09:05:52.151237 slot_machine_serializers-0.1.0/tests/
--rw-r--r--   0 ochsner    (502) staff       (20)      601 2023-04-06 16:44:42.000000 slot_machine_serializers-0.1.0/tests/test_samplers.py
--rw-r--r--   0 ochsner    (502) staff       (20)     2517 2023-04-06 16:29:21.000000 slot_machine_serializers-0.1.0/tests/test_serializers.py
+drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-25 08:48:47.252698 slot_machine_serializers-0.2.0/
+-rw-r--r--   0 ochsner    (502) staff       (20)     1921 2023-04-25 08:48:47.252802 slot_machine_serializers-0.2.0/PKG-INFO
+-rw-r--r--   0 ochsner    (502) staff       (20)     1663 2023-04-25 08:39:28.000000 slot_machine_serializers-0.2.0/README.md
+-rw-r--r--   0 ochsner    (502) staff       (20)       90 2023-04-06 15:49:44.000000 slot_machine_serializers-0.2.0/pyproject.toml
+-rw-r--r--   0 ochsner    (502) staff       (20)      595 2023-04-25 08:48:47.253162 slot_machine_serializers-0.2.0/setup.cfg
+drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-25 08:48:47.250955 slot_machine_serializers-0.2.0/slot_machine/
+-rw-r--r--   0 ochsner    (502) staff       (20)       51 2023-04-06 16:45:57.000000 slot_machine_serializers-0.2.0/slot_machine/__init__.py
+-rw-r--r--   0 ochsner    (502) staff       (20)     2759 2023-04-25 08:32:50.000000 slot_machine_serializers-0.2.0/slot_machine/samplers.py
+-rw-r--r--   0 ochsner    (502) staff       (20)     4317 2023-04-25 07:58:13.000000 slot_machine_serializers-0.2.0/slot_machine/serializers.py
+drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-25 08:48:47.251942 slot_machine_serializers-0.2.0/slot_machine_serializers.egg-info/
+-rw-r--r--   0 ochsner    (502) staff       (20)     1921 2023-04-25 08:48:47.000000 slot_machine_serializers-0.2.0/slot_machine_serializers.egg-info/PKG-INFO
+-rw-r--r--   0 ochsner    (502) staff       (20)      400 2023-04-25 08:48:47.000000 slot_machine_serializers-0.2.0/slot_machine_serializers.egg-info/SOURCES.txt
+-rw-r--r--   0 ochsner    (502) staff       (20)        1 2023-04-25 08:48:47.000000 slot_machine_serializers-0.2.0/slot_machine_serializers.egg-info/dependency_links.txt
+-rw-r--r--   0 ochsner    (502) staff       (20)       49 2023-04-25 08:48:47.000000 slot_machine_serializers-0.2.0/slot_machine_serializers.egg-info/requires.txt
+-rw-r--r--   0 ochsner    (502) staff       (20)       13 2023-04-25 08:48:47.000000 slot_machine_serializers-0.2.0/slot_machine_serializers.egg-info/top_level.txt
+drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-25 08:48:47.252421 slot_machine_serializers-0.2.0/tests/
+-rw-r--r--   0 ochsner    (502) staff       (20)      601 2023-04-06 16:44:42.000000 slot_machine_serializers-0.2.0/tests/test_samplers.py
+-rw-r--r--   0 ochsner    (502) staff       (20)     2517 2023-04-06 16:29:21.000000 slot_machine_serializers-0.2.0/tests/test_serializers.py
```

### Comparing `slot_machine_serializers-0.1.0/PKG-INFO` & `slot_machine_serializers-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slot_machine_serializers
-Version: 0.1.0
+Version: 0.2.0
 Summary: Ordered dataclass serializer mixin for sloted dataclasses
 Home-page: https://github.com/sirno/slot_machine
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # Slot Machine
@@ -28,16 +28,16 @@
 With `slot_machine` your next choice will be one you look forward to.
 
 ## Examples
 
 Simply add your favorite samplers to the configuration:
 
 ```yaml
-chicken_nuggets: !IntegerSampler 5..20
-price: !UniformSampler 9.99..20
+chicken_nuggets: !RangeSampler 5..20
+price: !UniformSampler 9..99..20
 ```
 
 Specify your dataclass and get rolling:
 
 ```python
 from dataclasses import dataclass
 from slot_machine import SlotsSerializer
@@ -45,15 +45,15 @@
 @dataclass(slots=True)
 class Basket(SlotsSerializer):
     chicken_nuggets: int
     price: float
 
 yaml_file = """
 basket:
-  chicken_nuggets: !IntegerSampler 5..10
+  chicken_nuggets: !RangeSampler 5..10
   price: !UniformSampler 9.99..20
 """
 
 surprise_basket = Basket.from_yaml(yaml_file)
 ```
 
 ### Build your own
```

### Comparing `slot_machine_serializers-0.1.0/README.md` & `slot_machine_serializers-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 With `slot_machine` your next choice will be one you look forward to.
 
 ## Examples
 
 Simply add your favorite samplers to the configuration:
 
 ```yaml
-chicken_nuggets: !IntegerSampler 5..20
-price: !UniformSampler 9.99..20
+chicken_nuggets: !RangeSampler 5..20
+price: !UniformSampler 9..99..20
 ```
 
 Specify your dataclass and get rolling:
 
 ```python
 from dataclasses import dataclass
 from slot_machine import SlotsSerializer
@@ -36,15 +36,15 @@
 @dataclass(slots=True)
 class Basket(SlotsSerializer):
     chicken_nuggets: int
     price: float
 
 yaml_file = """
 basket:
-  chicken_nuggets: !IntegerSampler 5..10
+  chicken_nuggets: !RangeSampler 5..10
   price: !UniformSampler 9.99..20
 """
 
 surprise_basket = Basket.from_yaml(yaml_file)
 ```
 
 ### Build your own
```

### Comparing `slot_machine_serializers-0.1.0/setup.cfg` & `slot_machine_serializers-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = slot_machine_serializers
-version = 0.1.0
+version = 0.2.0
 description = Ordered dataclass serializer mixin for sloted dataclasses
 long_description = file: README.md, LICENSE.md
 long_description_content_type = text/markdown
 url = https://github.com/sirno/slot_machine
 license = MIT
 python_requires = ">=3.10"
```

### Comparing `slot_machine_serializers-0.1.0/slot_machine/samplers.py` & `slot_machine_serializers-0.2.0/slot_machine/samplers.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,16 +38,14 @@
         """Get the sample."""
         pass
 
 
 class ScalarSampler(Sampler):
     """Define scalar sampler."""
 
-    _value_type = str
-
     @classmethod
     def _construct_yaml(cls, loader: yaml.Loader, node: yaml.nodes.Node) -> Self:
         value = loader.construct_scalar(node)
         return cls.get_sample(value=value)
 
 
 class MappingSampler(Sampler):
@@ -64,30 +62,53 @@
 
     @classmethod
     def get_sample(cls, value: str) -> float:
         """Get the sample."""
         return random.uniform(*map(float, value.split("..")))
 
 
-class IntegerSampler(ScalarSampler):
-    """Sample from integer distribution."""
+class RangeSampler(ScalarSampler):
+    """Sample from range distribution."""
 
     @classmethod
     def get_sample(cls, value: str) -> int:
         """Get the sample."""
-        return random.randint(*map(int, value.split("..")))
+        split = value.split("..")
 
+        if 1 < len(split) <= 3:
+            raise ValueError(f"Invalid range: {value}")
 
-class RangeSampler(ScalarSampler):
-    """Sample from range distribution."""
+        return random.randrange(*map(int, split))
+
+
+class ChoiceSampler(ScalarSampler):
+    """Sample from choices."""
 
     @classmethod
-    def get_sample(cls, value: str) -> int:
+    def get_sample(cls, values: list) -> int:
+        """Get the sample."""
+        return random.choice(values)
+
+
+class IntegerSampler(ScalarSampler):
+    """Sample from integer choices."""
+
+    @classmethod
+    def get_sample(cls, values: list) -> int:
+        """Get the sample."""
+        return random.choice(map(int, values))
+
+
+class FloatSampler(ScalarSampler):
+    """Sample from float choices."""
+
+    @classmethod
+    def get_sample(cls, values: list) -> float:
         """Get the sample."""
-        return random.randrange(*map(int, value.split("..")))
+        return random.choice(map(float, values))
 
 
 class NormalSampler(ScalarSampler):
     """Sample from normal distribution."""
 
     @classmethod
     def get_sample(cls, **kwargs) -> float:
```

### Comparing `slot_machine_serializers-0.1.0/slot_machine/serializers.py` & `slot_machine_serializers-0.2.0/slot_machine/serializers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Serializer and deserializer mixins for YAML."""
 
 from __future__ import annotations
 
 __all__ = ["SlotsSerializer", "SlotsLoader", "SlotsDumper"]
 
-import yaml
+import inspect
 import typing
+import yaml
 
 from typing_extensions import Self
 
 from collections import OrderedDict
 from typing import Dict
 
 
@@ -21,14 +22,23 @@
     pass
 
 
 class SlotsSerializer:
     """Serialize and deserialize YAML slotted dataclasses in order."""
 
     def __init_subclass__(cls) -> None:
+        # Check that all attributes have valid type hints
+        type_hints = typing.get_type_hints(cls)
+        for key, value in type_hints.items():
+            if not inspect.isclass(value):
+                raise TypeError(
+                    f"Type hint `{value}` for attribute `{key}` in class `{cls.__name__}` is not a class. "
+                    "Maybe you are trying to use a type alias from the typing module?"
+                )
+
         # Add constructor to the yaml decoder
         def construct_yaml(loader: SlotsSerializer, node: yaml.nodes.Node) -> cls:
             type_hints = typing.get_type_hints(cls)
             mapping = {}
             for key_node, value_node in node.value:
                 key = loader.construct_object(key_node, deep=False)
                 value_type = type_hints[key]
@@ -119,7 +129,8 @@
         with open(path, "r") as f:
             return cls.from_yaml(f.read())
 
     @classmethod
     def show_tag(cls, subclass) -> Self:
         """Decorator to show tag in yaml output."""
         subclass._show_tag = True
+        return subclass
```

### Comparing `slot_machine_serializers-0.1.0/slot_machine_serializers.egg-info/PKG-INFO` & `slot_machine_serializers-0.2.0/slot_machine_serializers.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slot-machine-serializers
-Version: 0.1.0
+Version: 0.2.0
 Summary: Ordered dataclass serializer mixin for sloted dataclasses
 Home-page: https://github.com/sirno/slot_machine
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # Slot Machine
@@ -28,16 +28,16 @@
 With `slot_machine` your next choice will be one you look forward to.
 
 ## Examples
 
 Simply add your favorite samplers to the configuration:
 
 ```yaml
-chicken_nuggets: !IntegerSampler 5..20
-price: !UniformSampler 9.99..20
+chicken_nuggets: !RangeSampler 5..20
+price: !UniformSampler 9..99..20
 ```
 
 Specify your dataclass and get rolling:
 
 ```python
 from dataclasses import dataclass
 from slot_machine import SlotsSerializer
@@ -45,15 +45,15 @@
 @dataclass(slots=True)
 class Basket(SlotsSerializer):
     chicken_nuggets: int
     price: float
 
 yaml_file = """
 basket:
-  chicken_nuggets: !IntegerSampler 5..10
+  chicken_nuggets: !RangeSampler 5..10
   price: !UniformSampler 9.99..20
 """
 
 surprise_basket = Basket.from_yaml(yaml_file)
 ```
 
 ### Build your own
```

### Comparing `slot_machine_serializers-0.1.0/tests/test_samplers.py` & `slot_machine_serializers-0.2.0/tests/test_samplers.py`

 * *Files identical despite different names*

### Comparing `slot_machine_serializers-0.1.0/tests/test_serializers.py` & `slot_machine_serializers-0.2.0/tests/test_serializers.py`

 * *Files identical despite different names*

