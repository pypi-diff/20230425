# Comparing `tmp/django_mongoengine_rql-0.2.0.tar.gz` & `tmp/django_mongoengine_rql-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_mongoengine_rql-0.2.0.tar", max compression
+gzip compressed data, was "django_mongoengine_rql-0.2.1.tar", max compression
```

## Comparing `django_mongoengine_rql-0.2.0.tar` & `django_mongoengine_rql-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-04-12 09:06:50.797084 django_mongoengine_rql-0.2.0/LICENSE
--rw-r--r--   0        0        0     3874 2023-04-12 09:06:50.797084 django_mongoengine_rql-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-12 09:06:50.797084 django_mongoengine_rql-0.2.0/dj_mongoengine_rql/__init__.py
--rw-r--r--   0        0        0      552 2023-04-12 09:06:50.797084 django_mongoengine_rql-0.2.0/dj_mongoengine_rql/constants.py
--rw-r--r--   0        0        0     1654 2023-04-12 09:06:50.797084 django_mongoengine_rql-0.2.0/dj_mongoengine_rql/filter_cls.py
--rw-r--r--   0        0        0      322 2023-04-12 09:06:50.797084 django_mongoengine_rql-0.2.0/dj_mongoengine_rql/q.py
--rw-r--r--   0        0        0     1965 2023-04-12 09:07:32.109243 django_mongoengine_rql-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5124 1970-01-01 00:00:00.000000 django_mongoengine_rql-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-25 09:32:36.317736 django_mongoengine_rql-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3874 2023-04-25 09:32:36.317736 django_mongoengine_rql-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 09:32:36.317736 django_mongoengine_rql-0.2.1/dj_mongoengine_rql/__init__.py
+-rw-r--r--   0        0        0      552 2023-04-25 09:32:36.317736 django_mongoengine_rql-0.2.1/dj_mongoengine_rql/constants.py
+-rw-r--r--   0        0        0     1752 2023-04-25 09:32:36.317736 django_mongoengine_rql-0.2.1/dj_mongoengine_rql/filter_cls.py
+-rw-r--r--   0        0        0      322 2023-04-25 09:32:36.317736 django_mongoengine_rql-0.2.1/dj_mongoengine_rql/q.py
+-rw-r--r--   0        0        0     1965 2023-04-25 09:33:15.985961 django_mongoengine_rql-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5124 1970-01-01 00:00:00.000000 django_mongoengine_rql-0.2.1/PKG-INFO
```

### Comparing `django_mongoengine_rql-0.2.0/LICENSE` & `django_mongoengine_rql-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_mongoengine_rql-0.2.0/README.md` & `django_mongoengine_rql-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django_mongoengine_rql-0.2.0/dj_mongoengine_rql/constants.py` & `django_mongoengine_rql-0.2.1/dj_mongoengine_rql/constants.py`

 * *Files identical despite different names*

### Comparing `django_mongoengine_rql-0.2.0/dj_mongoengine_rql/filter_cls.py` & `django_mongoengine_rql-0.2.1/dj_mongoengine_rql/filter_cls.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-#  Copyright © 2022 Ingram Micro. All rights reserved.
+#  Copyright © 2023 Ingram Micro. All rights reserved.
 #
 
 from dj_rql.constants import DjangoLookups
 from dj_rql.filter_cls import RQLFilterClass
 from django_mongoengine.fields.djangoflavor import DjangoField
 from py_rql.constants import FilterLookups
 
@@ -36,16 +36,17 @@
         return field.document_type
 
     @classmethod
     def _get_decimal_field_precision(cls, field):
         return field.precision
 
     def _build_django_q(self, filter_item, django_lookup, filter_lookup, typed_value):
-        if django_lookup == DjangoLookups.NULL:
-            q = self.Q_CLS(**{filter_item['orm_route']: None})
+        if django_lookup in (DjangoLookups.EXACT, DjangoLookups.NULL):
+            v = typed_value if django_lookup == DjangoLookups.EXACT else None
+            q = self.Q_CLS(**{filter_item['orm_route']: v})
             return ~q if filter_lookup == FilterLookups.NE else q
 
         if filter_lookup != FilterLookups.NE:
             kwargs = {'{0}__{1}'.format(filter_item['orm_route'], django_lookup): typed_value}
         else:
             kwargs = {'{0}__not__{1}'.format(filter_item['orm_route'], django_lookup): typed_value}
```

### Comparing `django_mongoengine_rql-0.2.0/pyproject.toml` & `django_mongoengine_rql-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-mongoengine-rql"
-version = "0.2.0"
+version = "0.2.1"
 description = "Django Mongoengine RQL Filtering"
 authors = ["Ingram Micro"]
 license = "Apache-2.0"
 packages = [
     { include = "dj_mongoengine_rql" }
 ]
 readme = "./README.md"
```

### Comparing `django_mongoengine_rql-0.2.0/PKG-INFO` & `django_mongoengine_rql-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mongoengine-rql
-Version: 0.2.0
+Version: 0.2.1
 Summary: Django Mongoengine RQL Filtering
 Home-page: https://connect.cloudblue.com/community/api/rql/
 License: Apache-2.0
 Keywords: rql,filter,django,mongo,mongoengine
 Author: Ingram Micro
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

