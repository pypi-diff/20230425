# Comparing `tmp/cleez-0.1.7.tar.gz` & `tmp/cleez-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleez-0.1.7.tar", max compression
+gzip compressed data, was "cleez-0.1.8.tar", max compression
```

## Comparing `cleez-0.1.7.tar` & `cleez-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      583 2023-04-17 08:35:32.159563 cleez-0.1.7/LICENSE
--rw-r--r--   0        0        0      896 2023-04-17 09:52:54.513608 cleez-0.1.7/README.rst
--rw-r--r--   0        0        0     3368 2023-04-25 08:53:10.153514 cleez-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      340 2023-04-17 16:19:10.886202 cleez-0.1.7/src/cleez/__init__.py
--rw-r--r--   0        0        0      553 2023-04-23 08:31:27.115897 cleez-0.1.7/src/cleez/actions.py
--rw-r--r--   0        0        0      522 2023-04-25 05:23:03.518828 cleez-0.1.7/src/cleez/argument.py
--rw-r--r--   0        0        0     5650 2023-04-25 08:52:36.067408 cleez-0.1.7/src/cleez/cleez.py
--rw-r--r--   0        0        0      371 2023-04-16 21:08:33.001276 cleez-0.1.7/src/cleez/colors.py
--rw-r--r--   0        0        0     1765 2023-04-25 08:52:21.338963 cleez-0.1.7/src/cleez/command.py
--rw-r--r--   0        0        0      268 2023-04-17 18:11:58.414950 cleez-0.1.7/src/cleez/exceptions.py
--rw-r--r--   0        0        0     2707 2023-04-24 08:22:54.099009 cleez-0.1.7/src/cleez/help.py
--rw-r--r--   0        0        0    11613 2023-04-25 08:19:46.737002 cleez-0.1.7/src/cleez/testing.py
--rw-r--r--   0        0        0     1758 1970-01-01 00:00:00.000000 cleez-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-04-17 08:35:32.159563 cleez-0.1.8/LICENSE
+-rw-r--r--   0        0        0      896 2023-04-17 09:52:54.513608 cleez-0.1.8/README.rst
+-rw-r--r--   0        0        0     3368 2023-04-25 11:52:09.699984 cleez-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      340 2023-04-17 16:19:10.886202 cleez-0.1.8/src/cleez/__init__.py
+-rw-r--r--   0        0        0      553 2023-04-23 08:31:27.115897 cleez-0.1.8/src/cleez/actions.py
+-rw-r--r--   0        0        0      522 2023-04-25 05:23:03.518828 cleez-0.1.8/src/cleez/argument.py
+-rw-r--r--   0        0        0     5762 2023-04-25 11:51:13.414394 cleez-0.1.8/src/cleez/cleez.py
+-rw-r--r--   0        0        0      371 2023-04-16 21:08:33.001276 cleez-0.1.8/src/cleez/colors.py
+-rw-r--r--   0        0        0     1765 2023-04-25 08:52:21.338963 cleez-0.1.8/src/cleez/command.py
+-rw-r--r--   0        0        0      268 2023-04-17 18:11:58.414950 cleez-0.1.8/src/cleez/exceptions.py
+-rw-r--r--   0        0        0     2707 2023-04-24 08:22:54.099009 cleez-0.1.8/src/cleez/help.py
+-rw-r--r--   0        0        0    11613 2023-04-25 08:19:46.737002 cleez-0.1.8/src/cleez/testing.py
+-rw-r--r--   0        0        0     1758 1970-01-01 00:00:00.000000 cleez-0.1.8/PKG-INFO
```

### Comparing `cleez-0.1.7/LICENSE` & `cleez-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cleez-0.1.7/README.rst` & `cleez-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `cleez-0.1.7/pyproject.toml` & `cleez-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "cleez"
-version = "0.1.7"
+version = "0.1.8"
 homepage = "https://github.com/abilian/cleez"
 description = "Simple class-based CLI framework."
 authors = ["Abilian SAS <sf@abilian.com>"]
 readme = "README.rst"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
```

### Comparing `cleez-0.1.7/src/cleez/actions.py` & `cleez-0.1.8/src/cleez/actions.py`

 * *Files identical despite different names*

### Comparing `cleez-0.1.7/src/cleez/argument.py` & `cleez-0.1.8/src/cleez/argument.py`

 * *Files identical despite different names*

### Comparing `cleez-0.1.7/src/cleez/cleez.py` & `cleez-0.1.8/src/cleez/cleez.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,14 +74,17 @@
                 if isclass(attribute) and issubclass(attribute, Command):
                     command = attribute
                     self.add_command(command)
 
     def add_command(self, command_class: type[Command]):
         if isabstract(command_class):
             return
+        for command in self.commands:
+            if command.name == command_class.name:
+                return
 
         self.commands.append(command_class(self))
 
     def add_option(self, *args, **kwargs):
         if args and isinstance(args[0], Option):
             assert (
                 len(args) == 1
```

### Comparing `cleez-0.1.7/src/cleez/command.py` & `cleez-0.1.8/src/cleez/command.py`

 * *Files identical despite different names*

### Comparing `cleez-0.1.7/src/cleez/help.py` & `cleez-0.1.8/src/cleez/help.py`

 * *Files identical despite different names*

### Comparing `cleez-0.1.7/src/cleez/testing.py` & `cleez-0.1.8/src/cleez/testing.py`

 * *Files identical despite different names*

### Comparing `cleez-0.1.7/PKG-INFO` & `cleez-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleez
-Version: 0.1.7
+Version: 0.1.8
 Summary: Simple class-based CLI framework.
 Home-page: https://github.com/abilian/cleez
 Author: Abilian SAS
 Author-email: sf@abilian.com
 Requires-Python: >=3.9,<4
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

