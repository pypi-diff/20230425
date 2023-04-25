# Comparing `tmp/slot_machine_serializers-0.2.0.tar.gz` & `tmp/slot_machine_serializers-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slot_machine_serializers-0.2.0.tar", last modified: Tue Apr 25 08:48:47 2023, max compression
+gzip compressed data, was "slot_machine_serializers-0.2.1.tar", last modified: Tue Apr 25 08:53:42 2023, max compression
```

## Comparing `slot_machine_serializers-0.2.0.tar` & `slot_machine_serializers-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-25 08:48:47.252698 slot_machine_serializers-0.2.0/
--rw-r--r--   0 ochsner    (502) staff       (20)     1921 2023-04-25 08:48:47.252802 slot_machine_serializers-0.2.0/PKG-INFO
--rw-r--r--   0 ochsner    (502) staff       (20)     1663 2023-04-25 08:39:28.000000 slot_machine_serializers-0.2.0/README.md
--rw-r--r--   0 ochsner    (502) staff       (20)       90 2023-04-06 15:49:44.000000 slot_machine_serializers-0.2.0/pyproject.toml
--rw-r--r--   0 ochsner    (502) staff       (20)      595 2023-04-25 08:48:47.253162 slot_machine_serializers-0.2.0/setup.cfg
-drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-25 08:48:47.250955 slot_machine_serializers-0.2.0/slot_machine/
--rw-r--r--   0 ochsner    (502) staff       (20)       51 2023-04-06 16:45:57.000000 slot_machine_serializers-0.2.0/slot_machine/__init__.py
--rw-r--r--   0 ochsner    (502) staff       (20)     2759 2023-04-25 08:32:50.000000 slot_machine_serializers-0.2.0/slot_machine/samplers.py
--rw-r--r--   0 ochsner    (502) staff       (20)     4317 2023-04-25 07:58:13.000000 slot_machine_serializers-0.2.0/slot_machine/serializers.py
-drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-25 08:48:47.251942 slot_machine_serializers-0.2.0/slot_machine_serializers.egg-info/
--rw-r--r--   0 ochsner    (502) staff       (20)     1921 2023-04-25 08:48:47.000000 slot_machine_serializers-0.2.0/slot_machine_serializers.egg-info/PKG-INFO
--rw-r--r--   0 ochsner    (502) staff       (20)      400 2023-04-25 08:48:47.000000 slot_machine_serializers-0.2.0/slot_machine_serializers.egg-info/SOURCES.txt
--rw-r--r--   0 ochsner    (502) staff       (20)        1 2023-04-25 08:48:47.000000 slot_machine_serializers-0.2.0/slot_machine_serializers.egg-info/dependency_links.txt
--rw-r--r--   0 ochsner    (502) staff       (20)       49 2023-04-25 08:48:47.000000 slot_machine_serializers-0.2.0/slot_machine_serializers.egg-info/requires.txt
--rw-r--r--   0 ochsner    (502) staff       (20)       13 2023-04-25 08:48:47.000000 slot_machine_serializers-0.2.0/slot_machine_serializers.egg-info/top_level.txt
-drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-25 08:48:47.252421 slot_machine_serializers-0.2.0/tests/
--rw-r--r--   0 ochsner    (502) staff       (20)      601 2023-04-06 16:44:42.000000 slot_machine_serializers-0.2.0/tests/test_samplers.py
--rw-r--r--   0 ochsner    (502) staff       (20)     2517 2023-04-06 16:29:21.000000 slot_machine_serializers-0.2.0/tests/test_serializers.py
+drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-25 08:53:42.851522 slot_machine_serializers-0.2.1/
+-rw-r--r--   0 ochsner    (502) staff       (20)     1921 2023-04-25 08:53:42.851627 slot_machine_serializers-0.2.1/PKG-INFO
+-rw-r--r--   0 ochsner    (502) staff       (20)     1663 2023-04-25 08:39:28.000000 slot_machine_serializers-0.2.1/README.md
+-rw-r--r--   0 ochsner    (502) staff       (20)       90 2023-04-06 15:49:44.000000 slot_machine_serializers-0.2.1/pyproject.toml
+-rw-r--r--   0 ochsner    (502) staff       (20)      595 2023-04-25 08:53:42.852010 slot_machine_serializers-0.2.1/setup.cfg
+drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-25 08:53:42.849525 slot_machine_serializers-0.2.1/slot_machine/
+-rw-r--r--   0 ochsner    (502) staff       (20)       51 2023-04-06 16:45:57.000000 slot_machine_serializers-0.2.1/slot_machine/__init__.py
+-rw-r--r--   0 ochsner    (502) staff       (20)     2763 2023-04-25 08:52:11.000000 slot_machine_serializers-0.2.1/slot_machine/samplers.py
+-rw-r--r--   0 ochsner    (502) staff       (20)     4317 2023-04-25 07:58:13.000000 slot_machine_serializers-0.2.1/slot_machine/serializers.py
+drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-25 08:53:42.850795 slot_machine_serializers-0.2.1/slot_machine_serializers.egg-info/
+-rw-r--r--   0 ochsner    (502) staff       (20)     1921 2023-04-25 08:53:42.000000 slot_machine_serializers-0.2.1/slot_machine_serializers.egg-info/PKG-INFO
+-rw-r--r--   0 ochsner    (502) staff       (20)      400 2023-04-25 08:53:42.000000 slot_machine_serializers-0.2.1/slot_machine_serializers.egg-info/SOURCES.txt
+-rw-r--r--   0 ochsner    (502) staff       (20)        1 2023-04-25 08:53:42.000000 slot_machine_serializers-0.2.1/slot_machine_serializers.egg-info/dependency_links.txt
+-rw-r--r--   0 ochsner    (502) staff       (20)       49 2023-04-25 08:53:42.000000 slot_machine_serializers-0.2.1/slot_machine_serializers.egg-info/requires.txt
+-rw-r--r--   0 ochsner    (502) staff       (20)       13 2023-04-25 08:53:42.000000 slot_machine_serializers-0.2.1/slot_machine_serializers.egg-info/top_level.txt
+drwxr-xr-x   0 ochsner    (502) staff       (20)        0 2023-04-25 08:53:42.851169 slot_machine_serializers-0.2.1/tests/
+-rw-r--r--   0 ochsner    (502) staff       (20)      599 2023-04-25 08:51:02.000000 slot_machine_serializers-0.2.1/tests/test_samplers.py
+-rw-r--r--   0 ochsner    (502) staff       (20)     2517 2023-04-06 16:29:21.000000 slot_machine_serializers-0.2.1/tests/test_serializers.py
```

### Comparing `slot_machine_serializers-0.2.0/PKG-INFO` & `slot_machine_serializers-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slot_machine_serializers
-Version: 0.2.0
+Version: 0.2.1
 Summary: Ordered dataclass serializer mixin for sloted dataclasses
 Home-page: https://github.com/sirno/slot_machine
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # Slot Machine
```

### Comparing `slot_machine_serializers-0.2.0/README.md` & `slot_machine_serializers-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `slot_machine_serializers-0.2.0/setup.cfg` & `slot_machine_serializers-0.2.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = slot_machine_serializers
-version = 0.2.0
+version = 0.2.1
 description = Ordered dataclass serializer mixin for sloted dataclasses
 long_description = file: README.md, LICENSE.md
 long_description_content_type = text/markdown
 url = https://github.com/sirno/slot_machine
 license = MIT
 python_requires = ">=3.10"
```

### Comparing `slot_machine_serializers-0.2.0/slot_machine/samplers.py` & `slot_machine_serializers-0.2.1/slot_machine/samplers.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     """Sample from range distribution."""
 
     @classmethod
     def get_sample(cls, value: str) -> int:
         """Get the sample."""
         split = value.split("..")
 
-        if 1 < len(split) <= 3:
+        if not 1 < len(split) <= 3:
             raise ValueError(f"Invalid range: {value}")
 
         return random.randrange(*map(int, split))
 
 
 class ChoiceSampler(ScalarSampler):
     """Sample from choices."""
```

### Comparing `slot_machine_serializers-0.2.0/slot_machine/serializers.py` & `slot_machine_serializers-0.2.1/slot_machine/serializers.py`

 * *Files identical despite different names*

### Comparing `slot_machine_serializers-0.2.0/slot_machine_serializers.egg-info/PKG-INFO` & `slot_machine_serializers-0.2.1/slot_machine_serializers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slot-machine-serializers
-Version: 0.2.0
+Version: 0.2.1
 Summary: Ordered dataclass serializer mixin for sloted dataclasses
 Home-page: https://github.com/sirno/slot_machine
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # Slot Machine
```

### Comparing `slot_machine_serializers-0.2.0/tests/test_samplers.py` & `slot_machine_serializers-0.2.1/tests/test_samplers.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     chicken_nuggets: int
     price: float
 
 
 def test_sample_basket():
     basket_distribution = """
-chicken_nuggets: !IntegerSampler 10..20
+chicken_nuggets: !RangeSampler 10..20
 price: !UniformSampler 9.99..20.0
 """
     basket = Basket.from_yaml(basket_distribution)
     assert isinstance(basket.chicken_nuggets, int)
     assert isinstance(basket.price, float)
     assert 10 <= basket.chicken_nuggets <= 20
     assert 9.99 <= basket.price <= 20.0
```

### Comparing `slot_machine_serializers-0.2.0/tests/test_serializers.py` & `slot_machine_serializers-0.2.1/tests/test_serializers.py`

 * *Files identical despite different names*

