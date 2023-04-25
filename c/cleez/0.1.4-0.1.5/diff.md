# Comparing `tmp/cleez-0.1.4.tar.gz` & `tmp/cleez-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleez-0.1.4.tar", max compression
+gzip compressed data, was "cleez-0.1.5.tar", max compression
```

## Comparing `cleez-0.1.4.tar` & `cleez-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      583 2023-04-17 08:35:32.159563 cleez-0.1.4/LICENSE
--rw-r--r--   0        0        0      896 2023-04-17 09:52:54.513608 cleez-0.1.4/README.rst
--rw-r--r--   0        0        0     3368 2023-04-24 08:39:56.663490 cleez-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      340 2023-04-17 16:19:10.886202 cleez-0.1.4/src/cleez/__init__.py
--rw-r--r--   0        0        0      553 2023-04-23 08:31:27.115897 cleez-0.1.4/src/cleez/actions.py
--rw-r--r--   0        0        0     4952 2023-04-24 08:31:13.115187 cleez-0.1.4/src/cleez/cleez.py
--rw-r--r--   0        0        0      371 2023-04-16 21:08:33.001276 cleez-0.1.4/src/cleez/colors.py
--rw-r--r--   0        0        0     1752 2023-04-24 08:30:16.438456 cleez-0.1.4/src/cleez/command.py
--rw-r--r--   0        0        0      268 2023-04-17 18:11:58.414950 cleez-0.1.4/src/cleez/exceptions.py
--rw-r--r--   0        0        0     2707 2023-04-24 08:22:54.099009 cleez-0.1.4/src/cleez/help.py
--rw-r--r--   0        0        0    11768 2023-04-24 08:31:38.016892 cleez-0.1.4/src/cleez/testing.py
--rw-r--r--   0        0        0     1758 1970-01-01 00:00:00.000000 cleez-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-04-17 08:35:32.159563 cleez-0.1.5/LICENSE
+-rw-r--r--   0        0        0      896 2023-04-17 09:52:54.513608 cleez-0.1.5/README.rst
+-rw-r--r--   0        0        0     3368 2023-04-24 17:26:41.136412 cleez-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      340 2023-04-17 16:19:10.886202 cleez-0.1.5/src/cleez/__init__.py
+-rw-r--r--   0        0        0      553 2023-04-23 08:31:27.115897 cleez-0.1.5/src/cleez/actions.py
+-rw-r--r--   0        0        0     4985 2023-04-24 17:21:57.536192 cleez-0.1.5/src/cleez/cleez.py
+-rw-r--r--   0        0        0      371 2023-04-16 21:08:33.001276 cleez-0.1.5/src/cleez/colors.py
+-rw-r--r--   0        0        0     1752 2023-04-24 08:30:16.438456 cleez-0.1.5/src/cleez/command.py
+-rw-r--r--   0        0        0      268 2023-04-17 18:11:58.414950 cleez-0.1.5/src/cleez/exceptions.py
+-rw-r--r--   0        0        0     2707 2023-04-24 08:22:54.099009 cleez-0.1.5/src/cleez/help.py
+-rw-r--r--   0        0        0    11768 2023-04-24 08:31:38.016892 cleez-0.1.5/src/cleez/testing.py
+-rw-r--r--   0        0        0     1758 1970-01-01 00:00:00.000000 cleez-0.1.5/PKG-INFO
```

### Comparing `cleez-0.1.4/LICENSE` & `cleez-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cleez-0.1.4/README.rst` & `cleez-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `cleez-0.1.4/pyproject.toml` & `cleez-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "cleez"
-version = "0.1.4"
+version = "0.1.5"
 homepage = "https://github.com/abilian/cleez"
 description = "Simple class-based CLI framework."
 authors = ["Abilian SAS <sf@abilian.com>"]
 readme = "README.rst"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
```

### Comparing `cleez-0.1.4/src/cleez/actions.py` & `cleez-0.1.5/src/cleez/actions.py`

 * *Files identical despite different names*

### Comparing `cleez-0.1.4/src/cleez/cleez.py` & `cleez-0.1.5/src/cleez/cleez.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 __all__ = ["CLI"]
 
 
 @dataclass(frozen=True)
 class CLI:
     name: str = "cleez"
+    version: str = "0.1.0"
 
     commands: list[Command] = field(default_factory=list)
     options: list[Option] = field(default_factory=list)
     help_maker: HelpMaker = field(default_factory=HelpMaker)
 
     #
     # Public API
@@ -141,15 +142,15 @@
             print(self.get_version())
             sys.exit(0)
 
     def print_help(self):
         self.help_maker.print_help(self)
 
     def get_version(self):
-        return "TODO"
+        return self.version
 
     def get_command_name(self):
         return self.name
 
 
 class MyArgParser(argparse.ArgumentParser):
     """Subclass of argparse.ArgumentParser that doesn't exit on error.
```

### Comparing `cleez-0.1.4/src/cleez/command.py` & `cleez-0.1.5/src/cleez/command.py`

 * *Files identical despite different names*

### Comparing `cleez-0.1.4/src/cleez/help.py` & `cleez-0.1.5/src/cleez/help.py`

 * *Files identical despite different names*

### Comparing `cleez-0.1.4/src/cleez/testing.py` & `cleez-0.1.5/src/cleez/testing.py`

 * *Files identical despite different names*

### Comparing `cleez-0.1.4/PKG-INFO` & `cleez-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleez
-Version: 0.1.4
+Version: 0.1.5
 Summary: Simple class-based CLI framework.
 Home-page: https://github.com/abilian/cleez
 Author: Abilian SAS
 Author-email: sf@abilian.com
 Requires-Python: >=3.9,<4
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

