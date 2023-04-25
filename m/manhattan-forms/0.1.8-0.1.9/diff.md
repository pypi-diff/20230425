# Comparing `tmp/manhattan_forms-0.1.8.tar.gz` & `tmp/manhattan_forms-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/manhattan_forms-0.1.8.tar", last modified: Sat Aug 25 21:24:30 2018, max compression
+gzip compressed data, was "dist/manhattan_forms-0.1.9.tar", last modified: Thu Oct 18 21:29:21 2018, max compression
```

## Comparing `manhattan_forms-0.1.8.tar` & `manhattan_forms-0.1.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-08-25 21:24:30.000000 manhattan_forms-0.1.8/
-drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-08-25 21:24:30.000000 manhattan_forms-0.1.8/manhattan_forms/
-drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-08-25 21:24:30.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/
-drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-08-25 21:24:30.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/
-drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-08-25 21:24:30.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/captchas/
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     3408 2018-04-12 16:16:47.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/captchas/google.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)       43 2018-04-12 16:16:47.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/captchas/__init__.py
-drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-08-25 21:24:30.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/tests/
-drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-08-25 21:24:30.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/tests/captchas/
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     1944 2018-04-12 16:16:47.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/tests/captchas/test_google.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)        0 2018-04-12 16:16:47.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/tests/captchas/__init__.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)    14928 2018-05-25 14:12:06.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/tests/test_fields.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     2435 2018-04-12 16:16:47.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/tests/test_form.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     2419 2018-04-12 16:16:47.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/tests/test_csrf.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     1632 2018-04-12 16:16:47.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/tests/test_utils.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)       51 2018-04-12 16:16:47.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/tests/conftest.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     4333 2018-04-12 16:16:47.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/tests/test_validators.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)        0 2018-04-12 16:16:47.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/tests/__init__.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)      812 2018-04-12 16:16:47.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/tests/fixtures.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)      236 2018-04-12 16:16:47.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/tests/frames.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     3477 2018-08-25 21:23:48.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/utils.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)    21957 2018-07-22 22:53:25.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/fields.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     7005 2018-05-25 13:04:47.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/validators.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     7119 2018-08-24 11:00:24.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/__init__.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)       55 2018-04-12 16:16:47.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan/__init__.py
-drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-08-25 21:24:30.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan_forms.egg-info/
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     1284 2018-08-25 21:24:30.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan_forms.egg-info/SOURCES.txt
--rw-rw-r--   0 anthony   (1001) anthony   (1001)       10 2018-08-25 21:24:30.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan_forms.egg-info/top_level.txt
--rw-rw-r--   0 anthony   (1001) anthony   (1001)        1 2018-08-25 21:24:30.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan_forms.egg-info/dependency_links.txt
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     1246 2018-08-25 21:24:30.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan_forms.egg-info/PKG-INFO
--rw-rw-r--   0 anthony   (1001) anthony   (1001)      186 2018-08-25 21:24:30.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan_forms.egg-info/requires.txt
--rw-rw-r--   0 anthony   (1001) anthony   (1001)       10 2018-08-25 21:24:30.000000 manhattan_forms-0.1.8/manhattan_forms/manhattan_forms.egg-info/namespace_packages.txt
--rw-rw-r--   0 anthony   (1001) anthony   (1001)       60 2018-04-12 16:16:47.000000 manhattan_forms-0.1.8/MANIFEST.in
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     1100 2018-04-12 16:16:47.000000 manhattan_forms-0.1.8/LICENSE
--rw-rw-r--   0 anthony   (1001) anthony   (1001)       79 2018-08-25 21:24:30.000000 manhattan_forms-0.1.8/setup.cfg
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     1246 2018-08-25 21:24:30.000000 manhattan_forms-0.1.8/PKG-INFO
--rw-rw-r--   0 anthony   (1001) anthony   (1001)     4185 2018-08-25 21:22:40.000000 manhattan_forms-0.1.8/setup.py
--rw-rw-r--   0 anthony   (1001) anthony   (1001)      237 2018-04-12 16:16:47.000000 manhattan_forms-0.1.8/README.md
+drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-10-18 21:29:21.000000 manhattan_forms-0.1.9/
+drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-10-18 21:29:21.000000 manhattan_forms-0.1.9/manhattan_forms/
+drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-10-18 21:29:21.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/
+drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-10-18 21:29:21.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/
+drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-10-18 21:29:21.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/captchas/
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     3408 2018-04-12 16:16:47.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/captchas/google.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)       43 2018-04-12 16:16:47.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/captchas/__init__.py
+drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-10-18 21:29:21.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/tests/
+drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-10-18 21:29:21.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/tests/captchas/
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     1944 2018-04-12 16:16:47.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/tests/captchas/test_google.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)        0 2018-04-12 16:16:47.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/tests/captchas/__init__.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)    14928 2018-05-25 14:12:06.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/tests/test_fields.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     2435 2018-04-12 16:16:47.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/tests/test_form.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     2419 2018-04-12 16:16:47.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/tests/test_csrf.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     1632 2018-04-12 16:16:47.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/tests/test_utils.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)       51 2018-04-12 16:16:47.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/tests/conftest.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     4333 2018-04-12 16:16:47.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/tests/test_validators.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)        0 2018-04-12 16:16:47.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/tests/__init__.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)      812 2018-04-12 16:16:47.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/tests/fixtures.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)      236 2018-04-12 16:16:47.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/tests/frames.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     3463 2018-08-25 21:30:47.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/utils.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)    21957 2018-10-18 21:19:36.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/fields.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     7340 2018-10-18 21:24:57.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/validators.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     7119 2018-08-24 11:00:24.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/__init__.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)       55 2018-04-12 16:16:47.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan/__init__.py
+drwxrwxr-x   0 anthony   (1001) anthony   (1001)        0 2018-10-18 21:29:21.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan_forms.egg-info/
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     1284 2018-10-18 21:29:21.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan_forms.egg-info/SOURCES.txt
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)       10 2018-10-18 21:29:20.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan_forms.egg-info/top_level.txt
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)        1 2018-10-18 21:29:20.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan_forms.egg-info/dependency_links.txt
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     1246 2018-10-18 21:29:20.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan_forms.egg-info/PKG-INFO
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)      186 2018-10-18 21:29:20.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan_forms.egg-info/requires.txt
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)       10 2018-10-18 21:29:20.000000 manhattan_forms-0.1.9/manhattan_forms/manhattan_forms.egg-info/namespace_packages.txt
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)       60 2018-04-12 16:16:47.000000 manhattan_forms-0.1.9/MANIFEST.in
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     1100 2018-04-12 16:16:47.000000 manhattan_forms-0.1.9/LICENSE
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)       79 2018-10-18 21:29:21.000000 manhattan_forms-0.1.9/setup.cfg
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     1246 2018-10-18 21:29:21.000000 manhattan_forms-0.1.9/PKG-INFO
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)     4185 2018-10-18 21:28:17.000000 manhattan_forms-0.1.9/setup.py
+-rw-rw-r--   0 anthony   (1001) anthony   (1001)      237 2018-04-12 16:16:47.000000 manhattan_forms-0.1.9/README.md
```

### Comparing `manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/captchas/google.py` & `manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/captchas/google.py`

 * *Files identical despite different names*

### Comparing `manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/tests/captchas/test_google.py` & `manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/tests/captchas/test_google.py`

 * *Files identical despite different names*

### Comparing `manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/tests/test_fields.py` & `manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/tests/test_form.py` & `manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/tests/test_csrf.py` & `manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/tests/test_csrf.py`

 * *Files identical despite different names*

### Comparing `manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/tests/test_utils.py` & `manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/tests/test_validators.py` & `manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/tests/fixtures.py` & `manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/utils.py` & `manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,11 +97,11 @@
         return None
 
     if isinstance(value, Frame):
         value = value._id
 
     try:
         return ObjectId(value)
-    except (InvalidObjectId, ValueError):
+    except InvalidObjectId:
         if value == '':
             return ''
         raise ValueError('invalid literal for `ObjectId()`')
```

### Comparing `manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/fields.py` & `manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/fields.py`

 * *Files identical despite different names*

### Comparing `manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/validators.py` & `manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/validators.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import wtforms.validators
 from wtforms.validators import *
 from wtforms.validators import ValidationError
 
 # WTForm validators are passed through to provide a single access point
 __all__ = set(wtforms.validators.__all__)
 __all__.add('ErrorMessage')
+__all__.add('PseudoRequired')
 __all__.add('RequiredIf')
 __all__.add('ValidationError')
 __all__.add('UniqueDocument')
 __all__ = tuple(__all__)
 
 
 class ErrorMessage(str):
@@ -31,14 +32,27 @@
         # Additional error information is add based on the kwargs
         for k, v in kwargs.items():
             setattr(cls, k, v)
 
         return str.__new__(cls, content)
 
 
+class PseudoRequired:
+    """
+    The `PseudoRequired` validator is used when you need a field to appear
+    required even though the field itself isn't. This is a common requirement
+    for tokenizer fields.
+    """
+
+    field_flags = ('required',)
+
+    def __call__(self, form, field):
+        return
+
+
 class RequiredIf:
     """
     The `RequiredIf` validator allows the parent field to be flagged as required
     only if certain conditions are met.
 
     The set of conditions are specified using keywords when initializing the
     validator, for example:
```

### Comparing `manhattan_forms-0.1.8/manhattan_forms/manhattan/forms/__init__.py` & `manhattan_forms-0.1.9/manhattan_forms/manhattan/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `manhattan_forms-0.1.8/manhattan_forms/manhattan_forms.egg-info/SOURCES.txt` & `manhattan_forms-0.1.9/manhattan_forms/manhattan_forms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manhattan_forms-0.1.8/manhattan_forms/manhattan_forms.egg-info/PKG-INFO` & `manhattan_forms-0.1.9/manhattan_forms/manhattan_forms.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manhattan-forms
-Version: 0.1.8
+Version: 0.1.9
 Summary: A set of classes, functions and utilties that extend WTForms for use with manhattan.
 Home-page: https://git.getme.co.uk/manhattan/manhattan_forms
 Author: Anthony Blackshaw
 Author-email: ant@getme.co.uk
 Maintainer: The Getme development team
 Maintainer-email: devs@getme.co.uk
 License: MIT
```

### Comparing `manhattan_forms-0.1.8/LICENSE` & `manhattan_forms-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `manhattan_forms-0.1.8/PKG-INFO` & `manhattan_forms-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manhattan_forms
-Version: 0.1.8
+Version: 0.1.9
 Summary: A set of classes, functions and utilties that extend WTForms for use with manhattan.
 Home-page: https://git.getme.co.uk/manhattan/manhattan_forms
 Author: Anthony Blackshaw
 Author-email: ant@getme.co.uk
 Maintainer: The Getme development team
 Maintainer-email: devs@getme.co.uk
 License: MIT
```

### Comparing `manhattan_forms-0.1.8/setup.py` & `manhattan_forms-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 setup(
     name='manhattan_forms',
     namespace_packages=['manhattan'],
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.1.8',
+    version='0.1.9',
 
     description='A set of classes, functions and utilties that extend WTForms '
                 'for use with manhattan.',
     long_description=long_description,
 
     # The project's main homepage (@@ add github url once public)
     url='https://git.getme.co.uk/manhattan/manhattan_forms',
```

