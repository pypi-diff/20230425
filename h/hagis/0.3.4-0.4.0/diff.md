# Comparing `tmp/hagis-0.3.4.tar.gz` & `tmp/hagis-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.3.4.tar", last modified: Mon Apr 24 11:59:46 2023, max compression
+gzip compressed data, was "hagis-0.4.0.tar", last modified: Tue Apr 25 13:26:31 2023, max compression
```

## Comparing `hagis-0.3.4.tar` & `hagis-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 11:59:46.708927 hagis-0.3.4/
--rw-rw-rw-   0        0        0      923 2023-04-24 11:59:46.707913 hagis-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-04-22 02:10:21.000000 hagis-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 11:59:46.693738 hagis-0.3.4/hagis/
--rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.3.4/hagis/__init__.py
--rw-rw-rw-   0        0        0    13373 2023-04-24 11:56:52.000000 hagis-0.3.4/hagis/hagis.py
-drwxrwxrwx   0        0        0        0 2023-04-24 11:59:46.705802 hagis-0.3.4/hagis.egg-info/
--rw-rw-rw-   0        0        0      923 2023-04-24 11:59:46.000000 hagis-0.3.4/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-04-24 11:59:46.000000 hagis-0.3.4/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 11:59:46.000000 hagis-0.3.4/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-24 11:59:46.000000 hagis-0.3.4/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      589 2023-04-24 11:57:16.000000 hagis-0.3.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 11:59:46.708927 hagis-0.3.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 13:26:31.790752 hagis-0.4.0/
+-rw-rw-rw-   0        0        0      923 2023-04-25 13:26:31.789752 hagis-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-04-22 02:10:21.000000 hagis-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 13:26:31.778759 hagis-0.4.0/hagis/
+-rw-rw-rw-   0        0        0       22 2023-04-13 14:53:13.000000 hagis-0.4.0/hagis/__init__.py
+-rw-rw-rw-   0        0        0    13836 2023-04-25 13:21:44.000000 hagis-0.4.0/hagis/hagis.py
+drwxrwxrwx   0        0        0        0 2023-04-25 13:26:31.787752 hagis-0.4.0/hagis.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-04-25 13:26:31.000000 hagis-0.4.0/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-04-25 13:26:31.000000 hagis-0.4.0/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 13:26:31.000000 hagis-0.4.0/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-25 13:26:31.000000 hagis-0.4.0/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      589 2023-04-25 13:22:09.000000 hagis-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 13:26:31.790752 hagis-0.4.0/setup.cfg
```

### Comparing `hagis-0.3.4/PKG-INFO` & `hagis-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.3.4
+Version: 0.4.0
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.3.4/hagis/hagis.py` & `hagis-0.4.0/hagis/hagis.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from time import time
 from types import SimpleNamespace
 from typing import Any, Callable, Dict, Generic, Iterable, List, Optional, Tuple, Type, TypeVar, Union
 from requests import post
 
 T = TypeVar("T")
 
-class Layer(Generic[T]): # pylint: disable=too-many-instance-attributes
+
+class Layer(Generic[T]):  # pylint: disable=too-many-instance-attributes
     """ Layer class.
 
     Args:
         Generic (T): Type argument.
     """
     def __init__(self, layer_url: str, model: Type[T] = SimpleNamespace,
                  oid_field: str = "objectid", shape_property_name: str = "shape", **mapping: str) -> None:
@@ -59,14 +60,17 @@
                     else:
                         self._fields[key] = property_name
 
                     if key == shape_property_name.lower():
                         self._shape_property_name = property_name
                         self._shape_property_type = property_type
 
+        self._is_arcgis_gemetry = hasattr(self._shape_property_type, "__module__")\
+            and self._shape_property_type.__module__.startswith("arcgis.geometry.")
+
         # Add custom properties that have not been handled as dynamically handled propeties.
         for property_name, field in mapping.items():
             if property_name not in mapped:
                 self._fields[property_name.lower()] = field
 
     _token_cache: Dict[Tuple[str, str], Tuple[str, int]] = {}
 
@@ -243,15 +247,18 @@
 
         dictionary["attributes"] = attributes
 
         for key, value in item.__dict__.items():
             lower_property_name = key.lower()
             field = self._fields[lower_property_name]
             if lower_property_name == self._shape_property_name.lower():
-                dictionary["geometry"] = value.__dict__
+                if self._is_arcgis_gemetry:
+                    dictionary["geometry"] = loads(value.JSON)
+                else:
+                    dictionary["geometry"] = value.__dict__
             elif isinstance(value, datetime):
                 attributes[field] = int((value - datetime.utcfromtimestamp(0)).total_seconds() * 1000)
             else:
                 attributes[field] = value
 
         return dictionary
 
@@ -288,16 +295,19 @@
     def _map(self, row: SimpleNamespace) -> SimpleNamespace:
         if not hasattr(row, "geometry"):
             return row.attributes
 
         if self._shape_property_type is None or self._shape_property_type in self._unknown_shape_types:
             shape = row.geometry
         else:
-            shape = self._shape_property_type()
-            shape.__dict__ = row.geometry.__dict__
+            if self._is_arcgis_gemetry:
+                shape = self._shape_property_type(row.geometry.__dict__)
+            else:
+                shape = self._shape_property_type()
+                shape.__dict__ = row.geometry.__dict__
 
         return SimpleNamespace(**row.attributes.__dict__, **{self._shape_property_name: shape})
 
     def _query(self, where_clause: str, fields: str, keep_querying: bool, **kwargs: Any) -> Iterable[SimpleNamespace]:
         def get_rows(where_clause: str):
             return self._get_rows(where_clause, fields, **kwargs)
 
@@ -312,27 +322,30 @@
             for number in range(size, len(oids), size):
                 more_where_clause = f"{self._oid_field} IN ({','.join(map(str, oids[number:number+size]))})"
                 more_rows, _ = get_rows(more_where_clause)
                 for row in more_rows:
                     yield self._map(row)
 
 
-class Point: # pylint: disable=too-few-public-methods
+class Point:  # pylint: disable=too-few-public-methods
     """ Point class.
     """
     x: float
     y: float
 
-class Multipoint: # pylint: disable=too-few-public-methods
+
+class Multipoint:  # pylint: disable=too-few-public-methods
     """ Multipoint class.
     """
     points: List[List[float]]
 
-class Polyline: # pylint: disable=too-few-public-methods
+
+class Polyline:  # pylint: disable=too-few-public-methods
     """ Polyline class.
     """
     paths: List[List[List[float]]]
 
-class Polygon: # pylint: disable=too-few-public-methods
+
+class Polygon:  # pylint: disable=too-few-public-methods
     """ Polygon class.
     """
     rings: List[List[List[float]]]
```

### Comparing `hagis-0.3.4/hagis.egg-info/PKG-INFO` & `hagis-0.4.0/hagis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.3.4
+Version: 0.4.0
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.3.4/pyproject.toml` & `hagis-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.3.4"
+version = "0.4.0"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

