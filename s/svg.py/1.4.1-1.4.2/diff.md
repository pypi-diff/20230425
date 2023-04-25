# Comparing `tmp/svg.py-1.4.1.tar.gz` & `tmp/svg.py-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svg.py-1.4.1.tar", last modified: Tue Nov 22 07:28:16 2022, max compression
+gzip compressed data, was "svg.py-1.4.2.tar", last modified: Tue Apr 25 10:07:21 2023, max compression
```

## Comparing `svg.py-1.4.1.tar` & `svg.py-1.4.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0       30 2022-08-08 07:37:36.583707 svg.py-1.4.1/.gitignore
--rw-r--r--   0        0        0     1048 2022-08-08 07:37:36.583707 svg.py-1.4.1/LICENSE
--rw-r--r--   0        0        0     1457 2022-09-23 11:52:20.854564 svg.py-1.4.1/README.md
--rw-r--r--   0        0        0       81 2022-08-08 07:37:36.583707 svg.py-1.4.1/examples/__init__.py
--rw-r--r--   0        0        0     1007 2022-08-08 07:37:36.583707 svg.py-1.4.1/examples/grid3.py
--rw-r--r--   0        0        0   137547 2022-08-08 07:37:36.583707 svg.py-1.4.1/examples/grid3.svg
--rw-r--r--   0        0        0      789 2022-08-08 07:37:36.583707 svg.py-1.4.1/examples/grid4.py
--rw-r--r--   0        0        0    15297 2022-08-08 07:37:36.583707 svg.py-1.4.1/examples/grid4.svg
--rw-r--r--   0        0        0     2240 2022-08-08 07:37:36.583707 svg.py-1.4.1/examples/shapes.py
--rw-r--r--   0        0        0      887 2022-08-08 07:37:36.583707 svg.py-1.4.1/examples/shapes.svg
--rw-r--r--   0        0        0     1067 2022-08-08 07:37:36.583707 svg.py-1.4.1/examples/text.py
--rw-r--r--   0        0        0      506 2022-08-08 07:37:36.583707 svg.py-1.4.1/examples/text.svg
--rw-r--r--   0        0        0     1229 2022-09-19 08:09:18.255101 svg.py-1.4.1/examples/transform.py
--rw-r--r--   0        0        0      362 2022-08-08 07:37:36.583707 svg.py-1.4.1/examples/transform.svg
--rw-r--r--   0        0        0      734 2022-08-08 07:37:36.583707 svg.py-1.4.1/pyproject.toml
--rw-r--r--   0        0        0      106 2022-08-08 07:37:36.583707 svg.py-1.4.1/reflect/__init__.py
--rw-r--r--   0        0        0      915 2022-08-08 07:37:36.583707 svg.py-1.4.1/reflect/_lib_element.py
--rw-r--r--   0        0        0     2389 2022-08-08 07:37:36.583707 svg.py-1.4.1/reflect/_mdn_attr.py
--rw-r--r--   0        0        0     1109 2022-08-08 07:37:36.583707 svg.py-1.4.1/scripts/actualize_deprecated.py
--rw-r--r--   0        0        0       50 2022-08-08 07:37:36.583707 svg.py-1.4.1/setup.cfg
--rw-r--r--   0        0        0   149217 2022-08-08 07:37:36.587707 svg.py-1.4.1/svg.xsd
--rw-r--r--   0        0        0     3328 2022-11-22 07:28:02.258113 svg.py-1.4.1/svg/__init__.py
--rw-r--r--   0        0        0    13433 2022-11-22 07:27:56.110201 svg.py-1.4.1/svg/_filters.py
--rw-r--r--   0        0        0      539 2022-08-08 07:37:36.587707 svg.py-1.4.1/svg/_helpers.py
--rw-r--r--   0        0        0     4740 2022-11-22 07:27:56.110201 svg.py-1.4.1/svg/_mixins.py
--rw-r--r--   0        0        0     4934 2022-11-22 07:27:56.110201 svg.py-1.4.1/svg/_path.py
--rw-r--r--   0        0        0     1980 2022-11-22 07:27:56.110201 svg.py-1.4.1/svg/_transforms.py
--rw-r--r--   0        0        0     1320 2022-11-22 07:27:56.110201 svg.py-1.4.1/svg/_types.py
--rw-r--r--   0        0        0    28075 2022-11-22 07:27:56.110201 svg.py-1.4.1/svg/elements.py
--rw-r--r--   0        0        0        0 2022-08-08 07:37:36.587707 svg.py-1.4.1/svg/py.typed
--rw-r--r--   0        0        0        0 2022-09-22 12:09:27.525839 svg.py-1.4.1/tests/__init__.py
--rw-r--r--   0        0        0      168 2022-08-08 07:37:36.587707 svg.py-1.4.1/tests/fixtures/deprecated_elements.txt
--rw-r--r--   0        0        0     1463 2022-08-08 07:37:36.587707 svg.py-1.4.1/tests/test_attributes.py
--rw-r--r--   0        0        0      579 2022-08-08 07:37:36.587707 svg.py-1.4.1/tests/test_elements.py
--rw-r--r--   0        0        0      442 2022-08-08 07:37:36.587707 svg.py-1.4.1/tests/test_examples.py
--rw-r--r--   0        0        0     2106 1970-01-01 00:00:00.000000 svg.py-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0       30 2022-08-08 07:37:36.583707 svg.py-1.4.2/.gitignore
+-rw-r--r--   0        0        0     1048 2022-08-08 07:37:36.583707 svg.py-1.4.2/LICENSE
+-rw-r--r--   0        0        0     1457 2022-09-23 11:52:20.854564 svg.py-1.4.2/README.md
+-rw-r--r--   0        0        0       81 2022-08-08 07:37:36.583707 svg.py-1.4.2/examples/__init__.py
+-rw-r--r--   0        0        0     1007 2022-08-08 07:37:36.583707 svg.py-1.4.2/examples/grid3.py
+-rw-r--r--   0        0        0   137547 2022-08-08 07:37:36.583707 svg.py-1.4.2/examples/grid3.svg
+-rw-r--r--   0        0        0      789 2022-08-08 07:37:36.583707 svg.py-1.4.2/examples/grid4.py
+-rw-r--r--   0        0        0    15297 2022-08-08 07:37:36.583707 svg.py-1.4.2/examples/grid4.svg
+-rw-r--r--   0        0        0     2240 2022-08-08 07:37:36.583707 svg.py-1.4.2/examples/shapes.py
+-rw-r--r--   0        0        0      887 2022-08-08 07:37:36.583707 svg.py-1.4.2/examples/shapes.svg
+-rw-r--r--   0        0        0     1067 2022-08-08 07:37:36.583707 svg.py-1.4.2/examples/text.py
+-rw-r--r--   0        0        0      506 2022-08-08 07:37:36.583707 svg.py-1.4.2/examples/text.svg
+-rw-r--r--   0        0        0     1229 2022-09-19 08:09:18.255101 svg.py-1.4.2/examples/transform.py
+-rw-r--r--   0        0        0      362 2022-08-08 07:37:36.583707 svg.py-1.4.2/examples/transform.svg
+-rw-r--r--   0        0        0      734 2022-08-08 07:37:36.583707 svg.py-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0      106 2022-08-08 07:37:36.583707 svg.py-1.4.2/reflect/__init__.py
+-rw-r--r--   0        0        0      915 2022-08-08 07:37:36.583707 svg.py-1.4.2/reflect/_lib_element.py
+-rw-r--r--   0        0        0     2389 2022-08-08 07:37:36.583707 svg.py-1.4.2/reflect/_mdn_attr.py
+-rw-r--r--   0        0        0     1109 2022-08-08 07:37:36.583707 svg.py-1.4.2/scripts/actualize_deprecated.py
+-rw-r--r--   0        0        0       50 2022-08-08 07:37:36.583707 svg.py-1.4.2/setup.cfg
+-rw-r--r--   0        0        0   149217 2022-08-08 07:37:36.587707 svg.py-1.4.2/svg.xsd
+-rw-r--r--   0        0        0     3328 2023-04-25 10:04:58.299461 svg.py-1.4.2/svg/__init__.py
+-rw-r--r--   0        0        0    13433 2022-11-22 07:27:56.110201 svg.py-1.4.2/svg/_filters.py
+-rw-r--r--   0        0        0      539 2022-08-08 07:37:36.587707 svg.py-1.4.2/svg/_helpers.py
+-rw-r--r--   0        0        0     4740 2022-11-22 07:27:56.110201 svg.py-1.4.2/svg/_mixins.py
+-rw-r--r--   0        0        0     4934 2022-11-22 07:27:56.110201 svg.py-1.4.2/svg/_path.py
+-rw-r--r--   0        0        0     1992 2023-04-25 10:04:48.999586 svg.py-1.4.2/svg/_transforms.py
+-rw-r--r--   0        0        0     1320 2022-11-22 07:27:56.110201 svg.py-1.4.2/svg/_types.py
+-rw-r--r--   0        0        0    28075 2022-11-22 07:27:56.110201 svg.py-1.4.2/svg/elements.py
+-rw-r--r--   0        0        0        0 2022-08-08 07:37:36.587707 svg.py-1.4.2/svg/py.typed
+-rw-r--r--   0        0        0        0 2022-09-22 12:09:27.525839 svg.py-1.4.2/tests/__init__.py
+-rw-r--r--   0        0        0      168 2022-08-08 07:37:36.587707 svg.py-1.4.2/tests/fixtures/deprecated_elements.txt
+-rw-r--r--   0        0        0     1463 2022-08-08 07:37:36.587707 svg.py-1.4.2/tests/test_attributes.py
+-rw-r--r--   0        0        0      579 2022-08-08 07:37:36.587707 svg.py-1.4.2/tests/test_elements.py
+-rw-r--r--   0        0        0      442 2022-08-08 07:37:36.587707 svg.py-1.4.2/tests/test_examples.py
+-rw-r--r--   0        0        0     2106 1970-01-01 00:00:00.000000 svg.py-1.4.2/PKG-INFO
```

### Comparing `svg.py-1.4.1/LICENSE` & `svg.py-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/README.md` & `svg.py-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/examples/grid3.py` & `svg.py-1.4.2/examples/grid3.py`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/examples/grid3.svg` & `svg.py-1.4.2/examples/grid3.svg`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/examples/grid4.py` & `svg.py-1.4.2/examples/grid4.py`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/examples/grid4.svg` & `svg.py-1.4.2/examples/grid4.svg`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/examples/shapes.py` & `svg.py-1.4.2/examples/shapes.py`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/examples/shapes.svg` & `svg.py-1.4.2/examples/shapes.svg`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/examples/text.py` & `svg.py-1.4.2/examples/text.py`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/examples/transform.py` & `svg.py-1.4.2/examples/transform.py`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/pyproject.toml` & `svg.py-1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/reflect/_lib_element.py` & `svg.py-1.4.2/reflect/_lib_element.py`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/reflect/_mdn_attr.py` & `svg.py-1.4.2/reflect/_mdn_attr.py`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/scripts/actualize_deprecated.py` & `svg.py-1.4.2/scripts/actualize_deprecated.py`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/svg.xsd` & `svg.py-1.4.2/svg.xsd`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/svg/__init__.py` & `svg.py-1.4.2/svg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     ColorProfile, DefinitionSrc, Defs, Desc, Element, Ellipse, ForeignObject,
     G, Image, Line, LinearGradient, Marker, Mask, Metadata, MPath, Path,
     Pattern, Polygon, Polyline, RadialGradient, Rect, Script, Set, Stop, Style,
     Switch, Symbol, Text, TextPath, Title, TSpan, Use, View,
 )
 
 
-__version__ = '1.4.1'
+__version__ = '1.4.2'
 __all__ = [
     'values',
     'escape',
     'mm',
     'px',
 
     # elements
```

### Comparing `svg.py-1.4.1/svg/_filters.py` & `svg.py-1.4.2/svg/_filters.py`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/svg/_helpers.py` & `svg.py-1.4.2/svg/_helpers.py`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/svg/_mixins.py` & `svg.py-1.4.2/svg/_mixins.py`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/svg/_path.py` & `svg.py-1.4.2/svg/_path.py`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/svg/_transforms.py` & `svg.py-1.4.2/svg/_transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     a: Number
     x: Optional[Number] = None
     y: Optional[Number] = None
 
     def __str__(self):
         if self.x is None:
             return f'rotate({self.a})'
-        assert self.y
+        assert self.y is not None
         return f'rotate({self.a} {self.x} {self.y})'
 
 
 @dataclass
 class SkewX(Transform):
     """
     https://developer.mozilla.org/en-US/docs/Web/SVG/Attribute/transform#skewx
```

### Comparing `svg.py-1.4.1/svg/_types.py` & `svg.py-1.4.2/svg/_types.py`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/svg/elements.py` & `svg.py-1.4.2/svg/elements.py`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/tests/test_attributes.py` & `svg.py-1.4.2/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/tests/test_elements.py` & `svg.py-1.4.2/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `svg.py-1.4.1/PKG-INFO` & `svg.py-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svg.py
-Version: 1.4.1
+Version: 1.4.2
 Summary: SVG drawing library
 Home-page: https://github.com/orsinium-labs/svg
 License: MIT
 Keywords: svg,drawing,vector
 Author: Gram
 Author-email: gram@orsinium.dev
 Requires-Python: >=3.7
```

