# Comparing `tmp/marshmallow-recipe-0.0.8.tar.gz` & `tmp/marshmallow-recipe-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marshmallow-recipe-0.0.8.tar", last modified: Sat Mar 26 10:17:49 2022, max compression
+gzip compressed data, was "marshmallow-recipe-0.0.9.tar", last modified: Tue Apr 26 14:25:41 2022, max compression
```

## Comparing `marshmallow-recipe-0.0.8.tar` & `marshmallow-recipe-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 10:17:49.394435 marshmallow-recipe-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-03-26 10:17:37.000000 marshmallow-recipe-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2662 2022-03-26 10:17:49.394435 marshmallow-recipe-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-03-26 10:17:37.000000 marshmallow-recipe-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 10:17:49.394435 marshmallow-recipe-0.0.8/marshmallow_recipe/
--rw-r--r--   0 runner    (1001) docker     (121)     1722 2022-03-26 10:17:37.000000 marshmallow-recipe-0.0.8/marshmallow_recipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5677 2022-03-26 10:17:37.000000 marshmallow-recipe-0.0.8/marshmallow_recipe/bake.py
--rw-r--r--   0 runner    (1001) docker     (121)    19230 2022-03-26 10:17:37.000000 marshmallow-recipe-0.0.8/marshmallow_recipe/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)      936 2022-03-26 10:17:37.000000 marshmallow-recipe-0.0.8/marshmallow_recipe/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-03-26 10:17:37.000000 marshmallow-recipe-0.0.8/marshmallow_recipe/missing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1397 2022-03-26 10:17:37.000000 marshmallow-recipe-0.0.8/marshmallow_recipe/naming_case.py
--rw-r--r--   0 runner    (1001) docker     (121)     3518 2022-03-26 10:17:37.000000 marshmallow-recipe-0.0.8/marshmallow_recipe/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-26 10:17:49.394435 marshmallow-recipe-0.0.8/marshmallow_recipe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2662 2022-03-26 10:17:49.000000 marshmallow-recipe-0.0.8/marshmallow_recipe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-03-26 10:17:49.000000 marshmallow-recipe-0.0.8/marshmallow_recipe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-26 10:17:49.000000 marshmallow-recipe-0.0.8/marshmallow_recipe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-03-26 10:17:49.000000 marshmallow-recipe-0.0.8/marshmallow_recipe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-03-26 10:17:49.000000 marshmallow-recipe-0.0.8/marshmallow_recipe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-26 10:17:49.394435 marshmallow-recipe-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1937 2022-03-26 10:17:37.000000 marshmallow-recipe-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 14:25:41.168740 marshmallow-recipe-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-04-26 14:25:21.000000 marshmallow-recipe-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3710 2022-04-26 14:25:41.168740 marshmallow-recipe-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      974 2022-04-26 14:25:21.000000 marshmallow-recipe-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 14:25:41.168740 marshmallow-recipe-0.0.9/marshmallow_recipe/
+-rw-r--r--   0 runner    (1001) docker     (121)     1722 2022-04-26 14:25:21.000000 marshmallow-recipe-0.0.9/marshmallow_recipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5750 2022-04-26 14:25:21.000000 marshmallow-recipe-0.0.9/marshmallow_recipe/bake.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19596 2022-04-26 14:25:21.000000 marshmallow-recipe-0.0.9/marshmallow_recipe/fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)      936 2022-04-26 14:25:21.000000 marshmallow-recipe-0.0.9/marshmallow_recipe/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-04-26 14:25:21.000000 marshmallow-recipe-0.0.9/marshmallow_recipe/missing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1397 2022-04-26 14:25:21.000000 marshmallow-recipe-0.0.9/marshmallow_recipe/naming_case.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3518 2022-04-26 14:25:21.000000 marshmallow-recipe-0.0.9/marshmallow_recipe/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 14:25:41.168740 marshmallow-recipe-0.0.9/marshmallow_recipe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3710 2022-04-26 14:25:41.000000 marshmallow-recipe-0.0.9/marshmallow_recipe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2022-04-26 14:25:41.000000 marshmallow-recipe-0.0.9/marshmallow_recipe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-26 14:25:41.000000 marshmallow-recipe-0.0.9/marshmallow_recipe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-04-26 14:25:41.000000 marshmallow-recipe-0.0.9/marshmallow_recipe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-04-26 14:25:41.000000 marshmallow-recipe-0.0.9/marshmallow_recipe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-26 14:25:41.168740 marshmallow-recipe-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1937 2022-04-26 14:25:21.000000 marshmallow-recipe-0.0.9/setup.py
```

### Comparing `marshmallow-recipe-0.0.8/LICENSE` & `marshmallow-recipe-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `marshmallow-recipe-0.0.8/marshmallow_recipe/__init__.py` & `marshmallow-recipe-0.0.9/marshmallow_recipe/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "dump_many",
     "schema",
     "EmptySchema",
     "metadata",
     "decimal_metadata",
 )
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 version = f"{__version__}, Python {sys.version}"
 
 VersionInfo = collections.namedtuple("VersionInfo", "major minor micro release_level serial")
 
 
 def _parse_version(v: str) -> VersionInfo:
```

### Comparing `marshmallow-recipe-0.0.8/marshmallow_recipe/bake.py` & `marshmallow-recipe-0.0.9/marshmallow_recipe/bake.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     decimal_field,
     dict_field,
     enum_field,
     float_field,
     int_field,
     list_field,
     nested_field,
+    raw_field,
     str_field,
     uuid_field,
 )
 from .missing import MISSING, Missing
 from .naming_case import DEFAULT_CASE, NamingCase
 
 _T = TypeVar("_T")
@@ -58,14 +59,17 @@
 
 def get_field_for(
     type: Type[_T],
     metadata: Mapping[str, Any],
     *,
     naming_case: NamingCase,
 ) -> m.fields.Field:
+    if type is Any:
+        return raw_field(**metadata)
+
     type = _substitute_any_to_open_generic(type)
 
     if typing_inspect.is_union_type(type):
         type_args = list(set(typing_inspect.get_args(type, True)))
         if types.NoneType not in type_args or len(type_args) != 2:
             raise ValueError(f"Unsupported {type=}")
         required = False
```

### Comparing `marshmallow-recipe-0.0.8/marshmallow_recipe/fields.py` & `marshmallow-recipe-0.0.9/marshmallow_recipe/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,14 +294,29 @@
         enum_type=enum_type,
         allow_none=True,
         **default_fields(None if default is MISSING else default),
         **data_key_fields(name),
     )
 
 
+def raw_field(
+    *,
+    default: Any | None | Missing = MISSING,
+    name: str | None = None,
+    validate: Callable[[Any], Any] | None = None,
+    **_: Any,
+) -> m.fields.Field:
+    return m.fields.Raw(
+        allow_none=True,
+        validate=validate,
+        **default_fields(None if default is MISSING else default),
+        **data_key_fields(name),
+    )
+
+
 DateTimeField: Type[m.fields.DateTime]
 EnumField: Type[m.fields.String]
 
 if _MARSHMALLOW_VERSION_MAJOR >= 3:
 
     def data_key_fields(name: str | None) -> dict[str, Any]:
         if name is None:
```

### Comparing `marshmallow-recipe-0.0.8/marshmallow_recipe/metadata.py` & `marshmallow-recipe-0.0.9/marshmallow_recipe/metadata.py`

 * *Files identical despite different names*

### Comparing `marshmallow-recipe-0.0.8/marshmallow_recipe/naming_case.py` & `marshmallow-recipe-0.0.9/marshmallow_recipe/naming_case.py`

 * *Files identical despite different names*

### Comparing `marshmallow-recipe-0.0.8/marshmallow_recipe/serialization.py` & `marshmallow-recipe-0.0.9/marshmallow_recipe/serialization.py`

 * *Files identical despite different names*

### Comparing `marshmallow-recipe-0.0.8/setup.py` & `marshmallow-recipe-0.0.9/setup.py`

 * *Files identical despite different names*

