# Comparing `tmp/pyfa_converter-1.0.4.0.tar.gz` & `tmp/pyfa_converter-1.0.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfa_converter-1.0.4.0.tar", max compression
+gzip compressed data, was "pyfa_converter-1.0.4.0a0.tar", max compression
```

## Comparing `pyfa_converter-1.0.4.0.tar` & `pyfa_converter-1.0.4.0a0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1063 2023-04-24 22:35:07.784011 pyfa_converter-1.0.4.0/LICENSE.md
--rw-r--r--   0        0        0     2432 2023-04-24 22:35:07.784011 pyfa_converter-1.0.4.0/README.md
--rw-r--r--   0        0        0      247 2023-04-24 22:35:07.784011 pyfa_converter-1.0.4.0/pyfa_converter/__init__.py
--rw-r--r--   0        0        0     1144 2023-04-24 22:35:07.784011 pyfa_converter-1.0.4.0/pyfa_converter/depends.py
--rw-r--r--   0        0        0     4129 2023-04-24 22:35:07.784011 pyfa_converter-1.0.4.0/pyfa_converter/main.py
--rw-r--r--   0        0        0        0 2023-04-24 22:35:07.784011 pyfa_converter-1.0.4.0/pyfa_converter/utils/__init__.py
--rw-r--r--   0        0        0     5603 2023-04-24 22:35:07.784011 pyfa_converter-1.0.4.0/pyfa_converter/utils/deprecation.py
--rw-r--r--   0        0        0      444 2023-04-24 22:35:07.784011 pyfa_converter-1.0.4.0/pyfa_converter/utils/deprecation_message.py
--rw-r--r--   0        0        0      880 2023-04-24 22:35:19.920290 pyfa_converter-1.0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3198 1970-01-01 00:00:00.000000 pyfa_converter-1.0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2022-12-19 06:26:10.841635 pyfa_converter-1.0.4.0a0/LICENSE.md
+-rw-r--r--   0        0        0     2432 2022-12-19 06:26:10.841635 pyfa_converter-1.0.4.0a0/README.md
+-rw-r--r--   0        0        0      247 2022-12-19 06:26:10.841635 pyfa_converter-1.0.4.0a0/pyfa_converter/__init__.py
+-rw-r--r--   0        0        0     1144 2022-12-19 06:26:10.841635 pyfa_converter-1.0.4.0a0/pyfa_converter/depends.py
+-rw-r--r--   0        0        0     4034 2022-12-19 06:26:10.841635 pyfa_converter-1.0.4.0a0/pyfa_converter/main.py
+-rw-r--r--   0        0        0        0 2022-12-19 06:26:10.841635 pyfa_converter-1.0.4.0a0/pyfa_converter/utils/__init__.py
+-rw-r--r--   0        0        0     5603 2022-12-19 06:26:10.841635 pyfa_converter-1.0.4.0a0/pyfa_converter/utils/deprecation.py
+-rw-r--r--   0        0        0      444 2022-12-19 06:26:10.841635 pyfa_converter-1.0.4.0a0/pyfa_converter/utils/deprecation_message.py
+-rw-r--r--   0        0        0      881 2022-12-19 06:26:32.997966 pyfa_converter-1.0.4.0a0/pyproject.toml
+-rw-r--r--   0        0        0     3240 1970-01-01 00:00:00.000000 pyfa_converter-1.0.4.0a0/setup.py
+-rw-r--r--   0        0        0     3200 1970-01-01 00:00:00.000000 pyfa_converter-1.0.4.0a0/PKG-INFO
```

### Comparing `pyfa_converter-1.0.4.0/LICENSE.md` & `pyfa_converter-1.0.4.0a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyfa_converter-1.0.4.0/README.md` & `pyfa_converter-1.0.4.0a0/README.md`

 * *Files identical despite different names*

### Comparing `pyfa_converter-1.0.4.0/pyfa_converter/depends.py` & `pyfa_converter-1.0.4.0a0/pyfa_converter/depends.py`

 * *Files identical despite different names*

### Comparing `pyfa_converter-1.0.4.0/pyfa_converter/main.py` & `pyfa_converter-1.0.4.0a0/pyfa_converter/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -85,23 +85,21 @@
                 field: The field to convert.
 
             Returns:
                 Either the result of `Query`, if the field is not a sub-model, or
                 the result of `Depends on` if it is.
 
             """
-            field_type = type(field.type_) if not isinstance(field.type_, type) else field.type_
-
-            if issubclass(field_type, BaseModel):
+            if issubclass(field.type_, BaseModel):
                 # This is a sub-model.
-                assert hasattr(field_type, _type_var_name), (
+                assert hasattr(field.type_, _type_var_name), (
                     f"Sub-model class for {field.name} field must be decorated with"
                     f" `as_form` too."
                 )
-                attr = getattr(field_type, _type_var_name)
+                attr = getattr(field.type_, _type_var_name)
                 return Depends(attr)  # noqa
             else:
                 return cls.param_maker(field=field, _type=_type)
 
         new_params = PydanticConverterUtils.override_signature_parameters(
             model=model_cls, param_maker=make_form_parameter
         )
```

### Comparing `pyfa_converter-1.0.4.0/pyfa_converter/utils/deprecation.py` & `pyfa_converter-1.0.4.0a0/pyfa_converter/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `pyfa_converter-1.0.4.0/pyproject.toml` & `pyfa_converter-1.0.4.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfa-converter"
-version = "1.0.4.0"
+version = "1.0.4.0a"
 description = "Pydantic to fastapi model converter."
 authors = ["dotX12 <dev@shitposting.team>"]
 license = "MIT License"
 homepage = "https://github.com/dotX12/pyfa-converter"
 repository = "https://github.com/dotX12/pyfa-converter"
 readme = "README.md"
```

### Comparing `pyfa_converter-1.0.4.0/PKG-INFO` & `pyfa_converter-1.0.4.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfa-converter
-Version: 1.0.4.0
+Version: 1.0.4.0a0
 Summary: Pydantic to fastapi model converter.
 Home-page: https://github.com/dotX12/pyfa-converter
 License: MIT
 Author: dotX12
 Author-email: dev@shitposting.team
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

