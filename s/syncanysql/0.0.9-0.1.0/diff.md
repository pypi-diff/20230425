# Comparing `tmp/syncanysql-0.0.9.tar.gz` & `tmp/syncanysql-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncanysql-0.0.9.tar", last modified: Thu Apr 20 10:16:18 2023, max compression
+gzip compressed data, was "syncanysql-0.1.0.tar", last modified: Tue Apr 25 10:06:27 2023, max compression
```

## Comparing `syncanysql-0.0.9.tar` & `syncanysql-0.1.0.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 10:16:18.409983 syncanysql-0.0.9/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2023-02-07 08:27:23.000000 syncanysql-0.0.9/LICENSE
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4234 2023-04-20 10:16:18.410984 syncanysql-0.0.9/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2955 2023-04-20 10:10:41.000000 syncanysql-0.0.9/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-04-20 10:16:18.420008 syncanysql-0.0.9/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2011 2023-04-20 10:04:48.000000 syncanysql-0.0.9/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 10:16:17.231680 syncanysql-0.0.9/syncanysql/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8404 2023-03-29 07:10:45.000000 syncanysql-0.0.9/syncanysql/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 10:16:17.686006 syncanysql-0.0.9/syncanysql/calculaters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1050 2023-03-25 04:42:07.000000 syncanysql-0.0.9/syncanysql/calculaters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6152 2023-03-25 11:43:14.000000 syncanysql-0.0.9/syncanysql/calculaters/aggregate_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1045 2023-04-20 03:00:29.000000 syncanysql-0.0.9/syncanysql/calculaters/mysql_calculater.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 10:16:17.951983 syncanysql-0.0.9/syncanysql/calculaters/mysql_funcs/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      320 2023-03-14 09:33:57.000000 syncanysql-0.0.9/syncanysql/calculaters/mysql_funcs/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    10157 2023-04-20 04:07:01.000000 syncanysql-0.0.9/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6002 2023-04-20 03:57:39.000000 syncanysql-0.0.9/syncanysql/calculaters/mysql_funcs/json_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6201 2023-04-20 03:05:35.000000 syncanysql-0.0.9/syncanysql/calculaters/mysql_funcs/number_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6413 2023-04-20 03:54:47.000000 syncanysql-0.0.9/syncanysql/calculaters/mysql_funcs/string_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)   120732 2023-04-20 09:54:00.000000 syncanysql-0.0.9/syncanysql/compiler.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12011 2023-03-27 03:03:08.000000 syncanysql-0.0.9/syncanysql/config.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      229 2023-02-08 10:09:29.000000 syncanysql-0.0.9/syncanysql/errors.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7245 2023-03-29 02:06:08.000000 syncanysql-0.0.9/syncanysql/executor.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3590 2023-03-25 04:39:43.000000 syncanysql-0.0.9/syncanysql/main.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.0.9/syncanysql/parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7259 2023-04-19 08:39:44.000000 syncanysql-0.0.9/syncanysql/prompt.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 10:16:18.367013 syncanysql-0.0.9/syncanysql/taskers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.0.9/syncanysql/taskers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.0.9/syncanysql/taskers/delete.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1513 2023-03-29 02:06:08.000000 syncanysql-0.0.9/syncanysql/taskers/execute.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1394 2023-03-29 02:07:07.000000 syncanysql-0.0.9/syncanysql/taskers/explain.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3519 2023-03-29 02:07:07.000000 syncanysql-0.0.9/syncanysql/taskers/into.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    18357 2023-03-29 02:07:07.000000 syncanysql-0.0.9/syncanysql/taskers/query.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2744 2023-03-29 02:07:49.000000 syncanysql-0.0.9/syncanysql/taskers/set.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2143 2023-03-29 02:06:08.000000 syncanysql-0.0.9/syncanysql/taskers/show.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1173 2023-03-29 02:06:08.000000 syncanysql-0.0.9/syncanysql/taskers/use.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      641 2023-02-19 14:49:39.000000 syncanysql-0.0.9/syncanysql/utils.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-04-20 10:04:48.000000 syncanysql-0.0.9/syncanysql/version.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 10:16:17.518855 syncanysql-0.0.9/syncanysql.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4234 2023-04-20 10:16:16.000000 syncanysql-0.0.9/syncanysql.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1119 2023-04-20 10:16:16.000000 syncanysql-0.0.9/syncanysql.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-20 10:16:16.000000 syncanysql-0.0.9/syncanysql.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-04-20 10:16:16.000000 syncanysql-0.0.9/syncanysql.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-02-25 12:53:08.000000 syncanysql-0.0.9/syncanysql.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      407 2023-04-20 10:16:16.000000 syncanysql-0.0.9/syncanysql.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-04-20 10:16:16.000000 syncanysql-0.0.9/syncanysql.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 10:06:27.902526 syncanysql-0.1.0/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4234 2023-04-25 10:06:27.903523 syncanysql-0.1.0/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2955 2023-04-20 10:10:41.000000 syncanysql-0.1.0/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-04-25 10:06:27.912524 syncanysql-0.1.0/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2030 2023-04-25 10:05:48.000000 syncanysql-0.1.0/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 10:06:26.678746 syncanysql-0.1.0/syncanysql/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     9128 2023-04-25 02:06:38.000000 syncanysql-0.1.0/syncanysql/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 10:06:27.078749 syncanysql-0.1.0/syncanysql/calculaters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1130 2023-04-23 06:35:38.000000 syncanysql-0.1.0/syncanysql/calculaters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6152 2023-03-25 11:43:14.000000 syncanysql-0.1.0/syncanysql/calculaters/aggregate_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1207 2023-04-23 06:39:00.000000 syncanysql-0.1.0/syncanysql/calculaters/mysql_calculater.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 10:06:27.379523 syncanysql-0.1.0/syncanysql/calculaters/mysql_funcs/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      320 2023-03-14 09:33:57.000000 syncanysql-0.1.0/syncanysql/calculaters/mysql_funcs/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    10157 2023-04-20 04:07:01.000000 syncanysql-0.1.0/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6002 2023-04-20 03:57:39.000000 syncanysql-0.1.0/syncanysql/calculaters/mysql_funcs/json_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6193 2023-04-24 06:11:11.000000 syncanysql-0.1.0/syncanysql/calculaters/mysql_funcs/number_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6461 2023-04-24 07:12:16.000000 syncanysql-0.1.0/syncanysql/calculaters/mysql_funcs/string_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)   125161 2023-04-25 03:25:46.000000 syncanysql-0.1.0/syncanysql/compiler.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12017 2023-04-21 07:43:33.000000 syncanysql-0.1.0/syncanysql/config.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      229 2023-02-08 10:09:29.000000 syncanysql-0.1.0/syncanysql/errors.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7641 2023-04-25 01:49:10.000000 syncanysql-0.1.0/syncanysql/executor.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3709 2023-04-24 02:09:57.000000 syncanysql-0.1.0/syncanysql/main.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.1.0/syncanysql/parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7259 2023-04-19 08:39:44.000000 syncanysql-0.1.0/syncanysql/prompt.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 10:06:27.858524 syncanysql-0.1.0/syncanysql/taskers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.1.0/syncanysql/taskers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.1.0/syncanysql/taskers/delete.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1603 2023-04-24 02:15:57.000000 syncanysql-0.1.0/syncanysql/taskers/execute.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1126 2023-04-24 01:38:19.000000 syncanysql-0.1.0/syncanysql/taskers/explain.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3796 2023-04-25 09:19:43.000000 syncanysql-0.1.0/syncanysql/taskers/into.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    18357 2023-03-29 02:07:07.000000 syncanysql-0.1.0/syncanysql/taskers/query.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2744 2023-03-29 02:07:49.000000 syncanysql-0.1.0/syncanysql/taskers/set.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2143 2023-03-29 02:06:08.000000 syncanysql-0.1.0/syncanysql/taskers/show.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1221 2023-04-25 04:04:01.000000 syncanysql-0.1.0/syncanysql/taskers/use.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      641 2023-02-19 14:49:39.000000 syncanysql-0.1.0/syncanysql/utils.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-04-21 10:34:47.000000 syncanysql-0.1.0/syncanysql/version.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 10:06:26.940746 syncanysql-0.1.0/syncanysql.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4234 2023-04-25 10:06:25.000000 syncanysql-0.1.0/syncanysql.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1111 2023-04-25 10:06:26.000000 syncanysql-0.1.0/syncanysql.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 10:06:25.000000 syncanysql-0.1.0/syncanysql.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-04-25 10:06:25.000000 syncanysql-0.1.0/syncanysql.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 10:06:25.000000 syncanysql-0.1.0/syncanysql.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      407 2023-04-25 10:06:25.000000 syncanysql-0.1.0/syncanysql.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-04-25 10:06:25.000000 syncanysql-0.1.0/syncanysql.egg-info/top_level.txt
```

### Comparing `syncanysql-0.0.9/PKG-INFO` & `syncanysql-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.0.9
+Version: 0.1.0
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
         [![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
```

### Comparing `syncanysql-0.0.9/README.md` & `syncanysql-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.9/setup.py` & `syncanysql-0.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 23/02/07
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.0.9"
+version = "0.1.0"
 
 if os.path.exists("README.md"):
     if sys.version_info[0] >= 3:
         try:
             with open("README.md", encoding="utf-8") as fp:
                 long_description = fp.read()
         except Exception as e:
@@ -29,20 +29,20 @@
 setup(
     name='syncanysql',
     version=version,
     url='https://github.com/snower/syncany-sql',
     author='snower',
     author_email='sujian199@gmail.com',
     license='MIT',
-    packages=find_packages(),
+    packages=find_packages(exclude=['*tests*']),
     zip_safe=False,
     install_requires=[
         "pyyaml>=5.1.2",
         "sqlglot>=10.6.2",
-        "syncany>=0.2.5",
+        "syncany>=0.2.6",
         'Pygments>=2.14.0',
         'Pygments>=2.14.0',
         'prompt-toolkit>=3.0.36',
         "rich>=9.11.1",
     ],
     extras_require={
         "pymongo": ['pymongo>=3.6.1'],
```

### Comparing `syncanysql-0.0.9/syncanysql/__init__.py` & `syncanysql-0.1.0/syncanysql/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from syncany.filters import Filter, register_filter
 from syncany.database import DataBase, register_database
 from syncany.calculaters import Calculater, TypeFormatCalculater, TypingCalculater, MathematicalCalculater, \
     TransformCalculater, register_calculater
 from syncany.taskers.config import Parser, ConfigReader, register_parser, register_reader
 from syncany.taskers.tasker import current_tasker
 from syncany.taskers.manager import TaskerManager
-from syncany.database.database import DatabaseManager
-from syncany.database.memory import MemoryDBFactory, MemoryDBCollection
+from syncany.database import DatabaseManager, find_database
+from syncany.errors import DatabaseUnknownException
 from .version import version, version_info
 from .parser import SqlParser, SqlSegment
 from .config import GlobalConfig
 from .executor import Executor
 from .calculaters import AggregateCalculater, StateAggregateCalculater
 
 
@@ -50,78 +50,88 @@
 
     def set_variable(self, name, value):
         if name and name[0] != "@":
             name = "@" + name
         self.executor.env_variables[name] = value
 
     def use(self, name, func_or_module):
-        if "imports" not in self.executor.session_config:
+        if "imports" not in self.executor.session_config.config:
             self.executor.session_config.config["imports"] = {}
         self.executor.session_config.config["imports"][name] = func_or_module
 
     def execute(self, sql):
-        self.__class__._thread_local.current_executer_context = self
-        try:
-            sql_parser = SqlParser(sql)
-            sqls = sql_parser.split()
-            self.__class__._execute_index += 1
-            self.executor.run("execute[%d]" % self._execute_index, sqls)
-            exit_code = self.executor.execute()
+        sql_parser = SqlParser(sql)
+        sqls = sql_parser.split()
+        self.__class__._execute_index += 1
+        with self.executor as executor:
+            executor.run("execute[%d]" % self._execute_index, sqls)
+            exit_code = executor.execute()
             if exit_code is not None and exit_code != 0:
                 raise ExecuterError(exit_code)
-            return 0
-        finally:
-            self.__class__._thread_local.current_executer_context = None
+        return 0
+
+    def get_database(self, db=None):
+        return self.engine.get_database(db)
+
+    def get_memory_datas(self, name):
+        return self.engine.get_memory_datas(name)
 
-    def get_memory_datas(self, name, db=None):
-        return self.engine.get_memory_datas(name, db)
+    def pop_memory_datas(self, name):
+        return self.engine.pop_memory_datas(name)
 
-    def pop_memory_datas(self, name, db=None):
-        return self.engine.pop_memory_datas(name, db)
+    def push_memory_datas(self, name, datas):
+        return self.engine.push_datas(name, datas)
 
     def terminal(self):
         if not self.executor:
             return
         self.executor.terminate()
 
     def __enter__(self):
+        self._thread_local.current_executer_context = self
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        pass
+        self._thread_local.current_executer_context = None
 
 
 class ScriptEngine(object):
     default_instance = None
 
     @classmethod
     def instance(cls, config=None):
         if cls.default_instance is None:
             cls.default_instance = ScriptEngine(config)
         return cls.default_instance
 
+    @classmethod
+    def current_context(cls):
+        return ExecuterContext.current()
+
     def __init__(self, config=None):
         self.config = GlobalConfig()
         self.config.load(config)
         self.manager = None
+        self.databases = {}
         self.executor = None
 
     def setup(self):
         if self.manager is not None:
             return
         init_execute_files = self.config.load()
         self.config.config_logging()
         self.manager = TaskerManager(DatabaseManager())
         self.executor = Executor(self.manager, self.config.session())
         if init_execute_files:
             self.executor.run("init", [SqlSegment("execute `%s`" % init_execute_files[i], i + 1) for i in
                                        range(len(init_execute_files))])
-            exit_code = self.executor.execute()
-            if exit_code is not None and exit_code != 0:
-                raise ExecuterError(exit_code)
+            with self.executor as executor:
+                exit_code = executor.execute()
+                if exit_code is not None and exit_code != 0:
+                    raise ExecuterError(exit_code)
         return 0
 
     def get_variable(self, name, default=None):
         if self.executor is None:
             self.setup()
         if name and name[0] != "@":
             name = "@" + name
@@ -147,59 +157,70 @@
         return ExecuterContext(self, Executor(self.manager, self.executor.session_config.session(), self.executor))
 
     def execute(self, sql):
         if self.executor is None:
             self.setup()
         return ExecuterContext(self, self.executor).execute(sql)
 
-    def get_memory_datas(self, name, db=None):
+    def get_database(self, db=None):
+        if self.manager is None:
+            self.setup()
+        db = db if db else "--"
+        if db in self.databases:
+            return self.databases[db]
+        try:
+            database_config = dict(**[database for database in self.executor.session_config.get()["databases"]
+                                      if database["name"] == db][0])
+        except Exception:
+            raise DatabaseUnknownException("%s is unknown" % db)
+        database_cls = find_database(database_config.pop("driver"))
+        if not database_cls:
+            raise DatabaseUnknownException(database_config["name"] + " is unknown")
+        self.databases[db] = database_cls(self.manager.database_manager, database_config).build()
+        return self.databases[db]
+
+    def get_memory_datas(self, name):
         if self.manager is None:
             return []
-        collection_key = ("--." + name) if not db else (db + "." + name)
-        for config_key, factory in self.manager.database_manager.factorys.items():
-            if not isinstance(factory, MemoryDBFactory):
-                continue
-            for driver in factory.drivers:
-                if not isinstance(driver.instance, MemoryDBCollection):
-                    continue
-                for key in list(driver.instance.keys()):
-                    if collection_key == key:
-                        return driver.instance[key]
-        return []
+        database = self.get_database("--")
+        query = database.query("--." + name, ["id"])
+        return query.commit()
 
-    def pop_memory_datas(self, name, db=None):
+    def pop_memory_datas(self, name):
         if self.manager is None:
             return []
-        collection_key = ("--." + name) if not db else (db + "." + name)
-        for config_key, factory in self.manager.database_manager.factorys.items():
-            if not isinstance(factory, MemoryDBFactory):
-                continue
-            for driver in factory.drivers:
-                if not isinstance(driver.instance, MemoryDBCollection):
-                    continue
-                for key in list(driver.instance.keys()):
-                    if collection_key == key:
-                        collection_datas = driver.instance[key]
-                        driver.instance.remove(key)
-                        return collection_datas
-        return []
+        database = self.get_database("--")
+        query = database.query("--." + name, ["id"])
+        datas = query.commit()
+        delete = database.delete("--." + name, ["id"])
+        delete.commit()
+        return datas
+
+    def push_memory_datas(self, name, datas):
+        database = self.get_database("--")
+        insert = database.insert("--." + name, ["id"], datas=datas if isinstance(datas, list) else [datas])
+        insert.commit()
 
     def terminal(self):
         executer_context = ExecuterContext.current()
         if not executer_context:
             if not self.executor:
                 return
             self.executor.terminate()
             return
         executer_context.terminate()
 
     def close(self):
         if self.manager:
             self.manager.close()
             self.manager = None
+        if self.databases:
+            for name, database in self.databases.items():
+                database.close()
+            self.databases = {}
         self.executor = None
         self.config = None
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
@@ -225,20 +246,28 @@
     ScriptEngine.instance().use(name, func_or_module)
 
 
 def execute(sql):
     return ScriptEngine.instance().execute(sql)
 
 
-def get_memory_datas(name, db=None):
-    return ScriptEngine.instance().get_memory_datas(name, db)
+def get_database(db=None):
+    return ScriptEngine.instance().get_database(db)
+
+
+def get_memory_datas(name):
+    return ScriptEngine.instance().get_memory_datas(name)
+
+
+def pop_memory_datas(name):
+    return ScriptEngine.instance().pop_memory_datas(name)
 
 
-def pop_memory_datas(name, db=None):
-    return ScriptEngine.instance().pop_memory_datas(name, db)
+def push_memory_datas(name, datas):
+    return ScriptEngine.instance().push_datas(name, datas)
 
 
 def terminal():
     return ScriptEngine.instance().terminal()
 
 
 def close():
```

### Comparing `syncanysql-0.0.9/syncanysql/calculaters/__init__.py` & `syncanysql-0.1.0/syncanysql/calculaters/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     "aggregate_min": AggregateMinCalculater,
     "aggregate_avg": AggregateAvgCalculater,
 }
 CALCULATERS.update(SQL_CALCULATERS)
 
 
 def is_mysql_func(name):
+    if MysqlCalculater.funcs is None:
+        MysqlCalculater.find_func(name)
     return name in MysqlCalculater.funcs
 
 
 def find_aggregate_calculater(name):
     calculater = find_calculater(name)
     if not issubclass(calculater, AggregateCalculater):
         raise CalculaterUnknownException("%s is unknown calculater" % name)
```

### Comparing `syncanysql-0.0.9/syncanysql/calculaters/aggregate_calculater.py` & `syncanysql-0.1.0/syncanysql/calculaters/aggregate_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.9/syncanysql/calculaters/mysql_calculater.py` & `syncanysql-0.1.0/syncanysql/calculaters/mysql_calculater.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 # -*- coding: utf-8 -*-
 # 2023/3/2
 # create by: snower
 
 import traceback
 from syncany.logger import get_logger
 from syncany.calculaters.calculater import Calculater
-from . import mysql_funcs
 
 
 class MysqlCalculater(Calculater):
-    funcs = mysql_funcs.funcs
+    funcs = None
+
+    @classmethod
+    def find_func(cls, name):
+        if cls.funcs is None:
+            from . import mysql_funcs
+            cls.funcs = mysql_funcs.funcs
+        return cls.funcs.get(name)
 
     def __init__(self, *args, **kwargs):
         super(MysqlCalculater, self).__init__(*args, **kwargs)
 
-        self.func = self.funcs.get(self.name[7:])
+        self.func = self.find_func(self.name[7:])
 
     def calculate(self, *args):
         try:
             if len(args) == 1 and isinstance(args[0], list) and args[0] and isinstance(args[0][0], dict):
                 try:
                     self.func(*tuple(args[0]))
                 except TypeError:
                     pass
             return self.func(*args)
         except (ValueError, KeyError) as e:
             return None
         except Exception as e:
             get_logger().warning("mysql calculater execute %s(%s) error: %s\n%s", self.name[7:], args, e,
                                  traceback.format_exc())
-            return None
+            return None
```

### Comparing `syncanysql-0.0.9/syncanysql/calculaters/mysql_funcs/datetime_funcs.py` & `syncanysql-0.1.0/syncanysql/calculaters/mysql_funcs/datetime_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.9/syncanysql/calculaters/mysql_funcs/json_funcs.py` & `syncanysql-0.1.0/syncanysql/calculaters/mysql_funcs/json_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.9/syncanysql/calculaters/mysql_funcs/number_funcs.py` & `syncanysql-0.1.0/syncanysql/calculaters/mysql_funcs/number_funcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         return 0
     if x is True:
         return 1
     if isinstance(x, datetime.date):
         if isinstance(x, datetime.datetime):
             return int(x.strftime("%Y%m%d%H%M%S"))
         return int(x.strftime("%Y%m%d"))
-    if isinstance(x, datetime.datetime):
+    if isinstance(x, datetime.time):
         return int(x.strftime("%H%M%S"))
     if isinstance(x, str):
         try:
             return int(x)
         except:
             return parse_number(x, False)
     return int(x)
@@ -52,15 +52,15 @@
         return 0
     if x is True:
         return 1
     if isinstance(x, datetime.date):
         if isinstance(x, datetime.datetime):
             return float(x.strftime("%Y%m%d%H%M%S")) + x.microsecond / 1000
         return float(x.strftime("%Y%m%d"))
-    if isinstance(x, datetime.datetime):
+    if isinstance(x, datetime.time):
         return float(x.strftime("%H%M%S")) + x.microsecond / 1000
     if isinstance(x, str):
         try:
             return float(x)
         except:
             return parse_number(x, True)
     return float(x)
```

### Comparing `syncanysql-0.0.9/syncanysql/calculaters/mysql_funcs/string_funcs.py` & `syncanysql-0.1.0/syncanysql/calculaters/mysql_funcs/string_funcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -195,30 +195,30 @@
     s1, s2 = ensure_str(s1), ensure_str(s2)
     return 0 if s1 == s2 else (-1 if s1 < s2 else 1)
 
 def mysql_startswith(s1, s2):
     if s1 is None or s2 is None:
         return None
     s1, s2 = ensure_str(s1), ensure_str(s2)
-    return s1.startswith(s2)
+    return 1 if s1.startswith(s2) else 0
 
 def mysql_endswith(s1, s2):
     if s1 is None or s2 is None:
         return None
     s1, s2 = ensure_str(s1), ensure_str(s2)
-    return s1.endswith(s2)
+    return 1 if s1.endswith(s2) else 0
 
 def mysql_contains(s1, s2):
     if s1 is None or s2 is None:
         return None
     try:
-        return s2 in s1
+        return 1 if s2 in s1 else 0
     except:
         s1, s2 = ensure_str(s1), ensure_str(s2)
-        return s2 in s1
+        return 1 if s2 in s1 else 0
 
 def mysql_crc32(s):
     if s is None:
         return None
     import zlib
     return zlib.crc32(s)
```

### Comparing `syncanysql-0.0.9/syncanysql/compiler.py` & `syncanysql-0.1.0/syncanysql/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,23 +114,25 @@
             use_info = expression.args["this"].args["this"].name
             if use_info in self.mapping:
                 use_info = self.mapping[use_info]
             return UseCommandTasker({"use": use_info})
         elif isinstance(expression, sqlglot.expressions.Set) and expression.args.get("expressions") and len(expression.args.get("expressions")) == 1:
             set_item_expression = expression.args.get("expressions")[0]
             if isinstance(set_item_expression, sqlglot_expressions.SetItem) and isinstance(set_item_expression.args["this"], sqlglot_expressions.EQ):
-                value = str(set_item_expression.args["this"]).split("=")
+                value = str(set_item_expression).split("=")
                 config = {"key": value[0].strip(), "value": "=".join(value[1:]).strip()}
                 return SetCommandTasker(config)
         raise SyncanySqlCompileException('unknown sql "%s"' % self.to_sql(expression))
 
     def compile_delete(self, expression, arguments):
         config = copy.deepcopy(self.config)
         config.update({
-            "input": "&.--.__subquery_null_" + str(uuid.uuid1().int) + "::id",
+            "input": "&.--.--::id",
+            "loader": "const_loader",
+            "loader_arguments":  {"datas": [{}]},
             "output": "&.-.&1::id",
             "querys": {},
             "schema": "$.*",
         })
 
         table_info = self.parse_table(expression.args["this"], config, arguments)
         where_expression = expression.args.get("where")
@@ -236,15 +238,15 @@
                     value = self.parse_const(value_expression, config, arguments)["value"]
                     if columns[i][1] is None:
                         columns[i][1] = str(type(value).__name__) if isinstance(value, (int, float, bool)) else None
                     data[columns[i][0]] = value
                 datas.append(data)
             config["schema"] = {column_name: "$." + column_name + (("|" + column_type) if column_type else "")
                                 for column_name, column_type in columns}
-            config["input"] = "&.-.-::" + columns[0][0]
+            config["input"] = "&.--.--::" + columns[0][0]
             config["loader"] = "const_loader"
             config["loader_arguments"] = {"datas": datas}
         else:
             raise SyncanySqlCompileException('unkonw insert into, related sql "%s"' % self.to_sql(expression))
 
     def compile_union(self, expression, config, arguments):
         select_expressions = []
@@ -285,14 +287,16 @@
 
         from_expression = expression.args.get("from")
         if not from_expression:
             primary_table["db"] = "--"
             primary_table["name"] = "--"
             primary_table["table_alias"] = "--"
             primary_table["table_name"] = "--"
+            config["loader"] = "const_loader"
+            config["loader_arguments"] = {"datas": [{}]}
             arguments["@limit"] = 1
             arguments["@batch"] = 0
         else:
             if not isinstance(from_expression, sqlglot_expressions.From) or not from_expression.expressions:
                 raise SyncanySqlCompileException('unknown select table, related sql "%s"' % self.to_sql(expression))
             if len(from_expression.expressions) > 1:
                 raise SyncanySqlCompileException('error select table, only select from one table, related sql "%s"'
@@ -378,43 +382,25 @@
                                                  % self.to_sql(expression))
             if column_expression:
                 self.compile_select_column(column_expression, config, arguments, primary_table, column_alias,
                                            self.parse_column(column_expression, config, arguments), join_tables)
                 continue
             if aggregate_expression:
                 self.compile_aggregate_column(aggregate_expression, config, arguments, primary_table, column_alias,
-                                              group_expression, join_tables)
+                                              group_expression, [aggregate_expression], join_tables)
                 continue
 
-            calculate_fields = []
-            self.parse_calculate(calculate_expression, config, arguments, primary_table, calculate_fields)
-            calculate_table_names = set([])
-            for calculate_field in calculate_fields:
-                if not calculate_field["table_name"] or calculate_field["table_name"] == primary_table["table_name"]:
-                    continue
-                if calculate_field["table_name"] not in join_tables:
-                    raise SyncanySqlCompileException('error select column, join table %s is unknown, related sql "%s"'
-                                                     % (calculate_field["table_name"], self.to_sql(expression)))
-                calculate_table_names.add(calculate_field["table_name"])
-            if calculate_table_names:
-                column_join_tables = []
-                self.compile_join_column_tables(calculate_expression, config, arguments, primary_table,
-                                                [join_tables[calculate_table_name] for calculate_table_name in calculate_table_names],
-                                                join_tables, column_join_tables)
-                calculate_column = self.compile_calculate(calculate_expression, config, arguments, primary_table, column_join_tables)
-                config["schema"][column_alias] = self.compile_join_column(calculate_expression, config, arguments, primary_table, 
-                                                                          calculate_column, column_join_tables)
-            else:
-                config["schema"][column_alias] = self.compile_calculate(calculate_expression, config, arguments, primary_table, [])
-            if not primary_table["seted_primary_keys"] and not primary_table["outputer_primary_keys"] and column_alias.isidentifier():
-                loader_primary_keys = [calculate_field["column_name"] for calculate_field in calculate_fields
-                                       if calculate_field["column_name"].isidentifier() and
-                                       (not calculate_field["table_name"] or calculate_field["table_name"] == primary_table["table_name"])]
-                if loader_primary_keys:
-                    primary_table["loader_primary_keys"], primary_table["outputer_primary_keys"] = loader_primary_keys, [column_alias]
+            aggregate_expressions = []
+            self.parse_aggregate(calculate_expression, config, arguments, aggregate_expressions)
+            if aggregate_expressions:
+                self.compile_aggregate_column(calculate_expression, config, arguments, primary_table, column_alias,
+                                              group_expression, aggregate_expressions, join_tables)
+                continue
+            self.compile_select_calculate_column(calculate_expression, config, arguments, primary_table, column_alias,
+                                                 join_tables)
 
         distinct_expression = expression.args.get("distinct")
         if distinct_expression and not config.get("aggregate", {}).get("distinct_keys"):
             if not isinstance(config["schema"], dict):
                 raise SyncanySqlCompileException('error distinct, select columns is unknown, related sql "%s"' % self.to_sql(expression))
             if "aggregate" not in config:
                 config["aggregate"] = copy.deepcopy(DEAULT_AGGREGATE)
@@ -556,14 +542,42 @@
                 primary_table["loader_primary_keys"], primary_table["outputer_primary_keys"], primary_table["seted_primary_keys"] = [], [], True
             primary_table["loader_primary_keys"].append(column_info["column_name"])
             primary_table["outputer_primary_keys"].append(column_alias)
         elif not primary_table["seted_primary_keys"] and not primary_table["outputer_primary_keys"]:
             if not column_info["table_name"] or column_info["table_name"] == primary_table["table_name"]:
                 primary_table["loader_primary_keys"], primary_table["outputer_primary_keys"] = [column_info["column_name"]], [column_alias]
 
+    def compile_select_calculate_column(self, expression, config, arguments, primary_table, column_alias, join_tables):
+        calculate_fields = []
+        self.parse_calculate(expression, config, arguments, primary_table, calculate_fields)
+        calculate_table_names = set([])
+        for calculate_field in calculate_fields:
+            if not calculate_field["table_name"] or calculate_field["table_name"] == primary_table["table_name"]:
+                continue
+            if calculate_field["table_name"] not in join_tables:
+                raise SyncanySqlCompileException('error select column, join table %s is unknown, related sql "%s"'
+                                                 % (calculate_field["table_name"], self.to_sql(expression)))
+            calculate_table_names.add(calculate_field["table_name"])
+        if calculate_table_names:
+            column_join_tables = []
+            self.compile_join_column_tables(expression, config, arguments, primary_table,
+                                            [join_tables[calculate_table_name] for calculate_table_name in calculate_table_names],
+                                            join_tables, column_join_tables)
+            calculate_column = self.compile_calculate(expression, config, arguments, primary_table, column_join_tables)
+            config["schema"][column_alias] = self.compile_join_column(expression, config, arguments, primary_table,
+                                                                      calculate_column, column_join_tables)
+        else:
+            config["schema"][column_alias] = self.compile_calculate(expression, config, arguments, primary_table, [])
+        if not primary_table["seted_primary_keys"] and not primary_table["outputer_primary_keys"] and column_alias.isidentifier():
+            loader_primary_keys = [calculate_field["column_name"] for calculate_field in calculate_fields
+                                   if calculate_field["column_name"].isidentifier() and
+                                   (not calculate_field["table_name"] or calculate_field["table_name"] == primary_table["table_name"])]
+            if loader_primary_keys:
+                primary_table["loader_primary_keys"], primary_table["outputer_primary_keys"] = loader_primary_keys, [column_alias]
+
     def compile_join_column_tables(self, expression, config, arguments, primary_table, current_join_tables, join_tables,
                                    column_join_tables):
         if not current_join_tables:
             return
         current_join_table_names = {current_join_table["name"] for current_join_table in current_join_tables}
         dup_column_join_tables = []
         for column_join_table in column_join_tables:
@@ -681,15 +695,17 @@
         else:
             raise SyncanySqlCompileException('error where condition, only "=,!=,>,>=,<,<=,in" operations are supported, related sql "%s"'
                                              % self.to_sql(expression))
 
     def compile_query_condition(self, expression, config, arguments, primary_table, typing_filters):
         if isinstance(expression, sqlglot_expressions.Select):
             select_expressions = expression.args.get("expressions")
-            if not select_expressions or len(select_expressions) != 1 or not self.is_column(select_expressions[0], config, arguments):
+            if not select_expressions or len(select_expressions) != 1 or \
+                    (not isinstance(select_expressions[0], sqlglot_expressions.Alias) and
+                     not self.is_column(select_expressions[0], config, arguments)):
                 raise SyncanySqlCompileException('error subquery, there must be only one query field, related sql "%s"'
                                                  % self.to_sql(expression))
             if expression.args.get("group") or expression.args.get("having") \
                     or expression.args.get("order") or expression.args.get("limit") or expression.args.get("distinct"):
                 is_subquery = True
             else:
                 is_subquery = False
@@ -723,15 +739,18 @@
         if not isinstance(from_expression, sqlglot_expressions.From) or not from_expression.expressions:
             raise SyncanySqlCompileException('error subquery, unknown select from table, related sql "%s"'
                                              % self.to_sql(expression))
         if len(from_expression.expressions) > 1:
             raise SyncanySqlCompileException('error subquery, there must be only one select from table, related sql "%s"'
                                              % self.to_sql(expression))
         table_info = self.parse_table(from_expression.expressions[0], config, arguments)
-        column_info = self.parse_column(select_expressions[0], config, arguments)
+        if isinstance(select_expressions[0], sqlglot_expressions.Alias):
+            column_info = self.parse_column(select_expressions[0].args["this"], config, arguments)
+        else:
+            column_info = self.parse_column(select_expressions[0], config, arguments)
         if column_info["typing_filters"] and typing_filters:
             column_info["typing_filters"] = typing_filters
         querys = {"querys": {}}
         where_expression = expression.args.get("where")
         if where_expression and isinstance(where_expression, sqlglot_expressions.Where):
             self.compile_where_condition(where_expression.args["this"], querys, arguments, primary_table)
             self.parse_condition_typing_filter(expression, querys, arguments)
@@ -764,44 +783,102 @@
         config["schema"][column_alias] = ["#make", {
             "key": copy.deepcopy(group_column),
             "value": copy.deepcopy(config["schema"][column_alias])
         }, [":#aggregate", "$.key", "$$.value"]]
         config["aggregate"]["key"] = copy.deepcopy(group_column)
         config["aggregate"]["schema"][column_alias] = aggregate_column
 
-    def compile_aggregate_column(self, expression, config, arguments, primary_table, column_alias, group_expression, join_tables):
+    def compile_aggregate_column(self, expression, config, arguments, primary_table, column_alias, group_expression,
+                                 aggregate_expressions, join_tables):
         group_column = self.compile_aggregate_key(group_expression, config, arguments, primary_table, join_tables)
-        is_distinct = False
-        if isinstance(expression, sqlglot_expressions.Anonymous):
-            if expression.args.get("expressions") and isinstance(expression.args["expressions"][0], sqlglot_expressions.Distinct):
-                is_distinct = True
-                value_expressions = expression.args["expressions"][0].args.get("expressions")
+        aggregate_value_expressions, distinct_column_index = [], -1
+        for i in range(len(aggregate_expressions)):
+            aggregate_expression = aggregate_expressions[i]
+            if isinstance(aggregate_expression, sqlglot_expressions.Anonymous):
+                if aggregate_expression.args.get("expressions") and isinstance(aggregate_expression.args["expressions"][0],
+                                                                               sqlglot_expressions.Distinct):
+                    if distinct_column_index >= 0:
+                        raise SyncanySqlCompileException('error aggregate distinct, only one distinct calculation is allowed, related sql "%s"' %
+                                                         self.to_sql(expression))
+                    distinct_column_index = i
+                    value_expressions = aggregate_expression.args["expressions"][0].args.get("expressions")
+                else:
+                    value_expressions = aggregate_expression.args.get("expressions")
             else:
-                value_expressions = expression.args.get("expressions")
-        else:
-            if isinstance(expression.args["this"], sqlglot_expressions.Distinct):
-                is_distinct = True
-                value_expressions = expression.args.get("this").args.get("expressions")
-            else:
-                value_expressions = [expression.args.get("this")]
-        value_column = self.compile_aggregate_value(expression, config, arguments, primary_table, join_tables,
-                                                    value_expressions)
+                if isinstance(aggregate_expression.args["this"], sqlglot_expressions.Distinct):
+                    if distinct_column_index >= 0:
+                        raise SyncanySqlCompileException('error aggregate distinct, only one distinct calculation is allowed, related sql "%s"' %
+                                                         self.to_sql(expression))
+                    distinct_column_index = i
+                    value_expressions = aggregate_expression.args.get("this").args.get("expressions")
+                else:
+                    value_expressions = [aggregate_expression.args.get("this")]
+            aggregate_value_expressions.append(value_expressions)
 
         if "aggregate" not in config:
             config["aggregate"] = copy.deepcopy(DEAULT_AGGREGATE)
-        if is_distinct and value_column:
-            if len(value_column) == 2:
-                config["aggregate"]["distinct_keys"].append(copy.deepcopy(value_column[1]))
-            else:
-                config["aggregate"]["distinct_keys"].extend(copy.deepcopy(value_column[1:]))
-            config["aggregate"]["distinct_aggregates"].add(column_alias)
-        if value_column and len(value_column) == 2:
-            value_column = value_column[1]
+        if len(aggregate_expressions) == 1 and aggregate_expressions[0] is expression:
+            value_column = self.compile_aggregate_value(aggregate_expressions[0], config, arguments, primary_table, join_tables,
+                                                        aggregate_value_expressions[0])
+            if distinct_column_index == 0 and value_column:
+                aggregate_distinct_keys = [copy.deepcopy(value_column[1])] if len(value_column) == 2 else copy.deepcopy(value_column[1:])
+                if not config["aggregate"]["distinct_keys"]:
+                    config["aggregate"]["distinct_keys"].extend(aggregate_distinct_keys)
+                elif config["aggregate"]["distinct_keys"] != aggregate_distinct_keys:
+                    raise SyncanySqlCompileException(
+                        'error aggregate distinct, only one distinct calculation is allowed, related sql "%s"' % self.to_sql(expression))
+                config["aggregate"]["distinct_aggregates"].add(column_alias)
+            if value_column and len(value_column) == 2:
+                value_column = value_column[1]
+            aggregate_calculate, reduce_calculate, final_calculate = self.compile_aggregate_calculate(aggregate_expressions[0])
+            aggregate_column = {
+                "key": group_column,
+                "value": value_column,
+                "calculate": [aggregate_calculate, "$." + column_alias, "$$.value"],
+                "aggregate": [":#aggregate", "$.key", [aggregate_calculate, "$." + column_alias, "$$.value"]],
+                "reduce": [reduce_calculate, "$." + column_alias, "$$." + column_alias],
+                "final_value": [final_calculate, "$." + column_alias] if final_calculate else None
+            }
+        else:
+            value_column, calculate_column, reduce_column = ["#make", {}], ["#make", {}], ["#make", {}]
+            for i in range(len(aggregate_expressions)):
+                aggregate_value_key = "value_%d" % id(aggregate_expressions[i])
+                aggregate_value_column = self.compile_aggregate_value(aggregate_expressions[i], config, arguments, primary_table,
+                                                                                 join_tables, aggregate_value_expressions[i])
+                if distinct_column_index == i and aggregate_value_column:
+                    aggregate_distinct_keys = [copy.deepcopy(aggregate_value_column[1])] if len(aggregate_value_column) == 2 \
+                        else copy.deepcopy(aggregate_value_column[1:])
+                    if not config["aggregate"]["distinct_keys"]:
+                        config["aggregate"]["distinct_keys"].extend(aggregate_distinct_keys)
+                    elif config["aggregate"]["distinct_keys"] != aggregate_distinct_keys:
+                        raise SyncanySqlCompileException(
+                            'error aggregate distinct, only one distinct calculation is allowed, related sql "%s"' % self.to_sql(expression))
+                    config["aggregate"]["distinct_aggregates"].add(column_alias)
+                if aggregate_value_column and len(aggregate_value_column) == 2:
+                    aggregate_value_column = aggregate_value_column[1]
+                aggregate_calculate, reduce_calculate, final_calculate = self.compile_aggregate_calculate(aggregate_expressions[i])
+                value_column[1][aggregate_value_key] = aggregate_value_column
+                calculate_column[1][aggregate_value_key] = [aggregate_calculate, "$." + column_alias + "." + aggregate_value_key,
+                                                                      "$$.value." + aggregate_value_key]
+                reduce_column[1][aggregate_value_key] = [reduce_calculate,
+                                                                   "$." + column_alias + "." + aggregate_value_key,
+                                                                   "$$." + column_alias + "." + aggregate_value_key]
+                setattr(aggregate_expressions[i], "final_column",
+                        [final_calculate, "$." + column_alias + "." + aggregate_value_key]
+                        if final_calculate else ("$." + column_alias + "." + aggregate_value_key))
+            self.compile_select_calculate_column(expression, config, arguments, primary_table, column_alias, join_tables)
+            aggregate_column = {
+                "key": group_column,
+                "value": value_column,
+                "calculate": calculate_column,
+                "aggregate": [":#aggregate", "$.key", copy.deepcopy(calculate_column)],
+                "reduce": reduce_column,
+                "final_value": config["schema"][column_alias]
+            }
 
-        aggregate_column = self.compile_aggregate(expression, config, arguments, column_alias, group_column, value_column)
         config["schema"][column_alias] = ["#make", {
             "key": copy.deepcopy(group_column),
             "value": copy.deepcopy(value_column),
         }, copy.deepcopy(aggregate_column["aggregate"])]
         config["aggregate"]["key"] = copy.deepcopy(aggregate_column["key"])
         config["aggregate"]["schema"][column_alias] = aggregate_column
 
@@ -864,85 +941,40 @@
                                              calculate_table_names], join_tables, column_join_tables)
             calculate_column = self.compile_calculate(value_expression, config, arguments, primary_table,
                                                       column_join_tables)
             value_column.append(self.compile_join_column(value_expression, config, arguments, primary_table,
                                                          calculate_column, column_join_tables))
         return value_column
 
-    def compile_aggregate(self, expression, config, arguments, column_alias, key_column, value_column):
+    def compile_aggregate_calculate(self, expression):
         if isinstance(expression, sqlglot_expressions.Count):
-            calculate = ["@aggregate_count::aggregate", "$." + column_alias, "$$.value"]
-            return {
-                "key": key_column,
-                "value": value_column,
-                "calculate": calculate,
-                "aggregate": [":#aggregate", "$.key", copy.deepcopy(calculate)],
-                "reduce": ["@aggregate_count::reduce", "$." + column_alias, "$$." + column_alias],
-                "final_value": None
-            }
+            return "@aggregate_count::aggregate", "@aggregate_count::reduce", None
         elif isinstance(expression, sqlglot_expressions.Sum):
-            calculate = ["@aggregate_sum::aggregate", "$." + column_alias, "$$.value"]
-            return {
-                "key": key_column,
-                "value": value_column,
-                "calculate": calculate,
-                "aggregate": [":#aggregate", "$.key", copy.deepcopy(calculate)],
-                "reduce": ["@aggregate_sum::reduce", "$." + column_alias, "$$." + column_alias],
-                "final_value": None
-            }
+            return "@aggregate_sum::aggregate", "@aggregate_sum::reduce", None
         elif isinstance(expression, sqlglot_expressions.Min):
-            calculate = ["@aggregate_min::aggregate", "$." + column_alias, "$$.value"]
-            return {
-                "key": key_column,
-                "value": value_column,
-                "calculate": calculate,
-                "aggregate": [":#aggregate", "$.key", copy.deepcopy(calculate)],
-                "reduce": ["@aggregate_min::reduce", "$." + column_alias, "$$." + column_alias],
-                "final_value": None
-            }
+            return "@aggregate_min::aggregate", "@aggregate_min::reduce", None
         elif isinstance(expression, sqlglot_expressions.Max):
-            calculate = ["@aggregate_max::aggregate", "$." + column_alias, "$$.value"]
-            return {
-                "key": key_column,
-                "value": value_column,
-                "calculate": calculate,
-                "aggregate": [":#aggregate", "$.key", copy.deepcopy(calculate)],
-                "reduce": ["@aggregate_max::reduce", "$." + column_alias, "$$." + column_alias],
-                "final_value": None
-            }
+            return "@aggregate_max::aggregate", "@aggregate_max::reduce", None
         elif isinstance(expression, sqlglot_expressions.Avg):
-            calculate = ["@aggregate_avg::aggregate", "$." + column_alias, "$$.value"]
-            return {
-                "key": key_column,
-                "value": value_column,
-                "calculate": calculate,
-                "aggregate": [":#aggregate", "$.key", copy.deepcopy(calculate)],
-                "reduce": ["@aggregate_avg::reduce", "$." + column_alias, "$$." + column_alias],
-                "final_value": ["@aggregate_avg::final_value", "$." + column_alias]
-            }
+            return "@aggregate_avg::aggregate", "@aggregate_avg::reduce", "@aggregate_avg::final_value"
         elif isinstance(expression, sqlglot_expressions.Anonymous):
             calculater_name = expression.args["this"].lower()
             try:
                 aggregate_calculater = find_aggregate_calculater(calculater_name)
-                calculate = ["@" + calculater_name + "::aggregate", "$." + column_alias, "$$.value"]
-                return {
-                    "key": key_column,
-                    "value": value_column,
-                    "calculate": calculate,
-                    "aggregate": [":#aggregate", "$.key", copy.deepcopy(calculate)],
-                    "reduce": ["@" + calculater_name + "::reduce", "$." + column_alias, "$$." + column_alias],
-                    "final_value": ["@" + calculater_name + "::final_value", "$." + column_alias]
-                                    if hasattr(aggregate_calculater, "final_value") else None
-                }
+                return ("@" + calculater_name + "::aggregate",
+                        "@" + calculater_name + "::reduce",
+                        ("@" + calculater_name + "::final_value" if hasattr(aggregate_calculater, "final_value") else None))
             except CalculaterUnknownException:
                 raise SyncanySqlCompileException('unknown aggregate calculate, related sql "%s"' % self.to_sql(expression))
         else:
             raise SyncanySqlCompileException('unknown aggregate calculate, related sql "%s"' % self.to_sql(expression))
         
     def compile_calculate(self, expression, config, arguments, primary_table, column_join_tables, join_index=-1):
+        if self.is_aggregate(expression, config, arguments) and hasattr(expression, "final_column"):
+            return expression.final_column
         if isinstance(expression, sqlglot_expressions.Neg):
             return ["@neg", self.compile_calculate(expression.args["this"], config, arguments, primary_table, 
                                                    column_join_tables, join_index)]
         elif isinstance(expression, sqlglot_expressions.Anonymous):
             calculater_name = expression.args["this"].lower()
             if calculater_name == "get_value":
                 get_value_expressions = expression.args.get("expressions")
@@ -1458,14 +1490,16 @@
                 join_table["querys"][condition_column["typing_name"]] = {}
             join_table["querys"][condition_column["typing_name"]]["in"] = value_column
         else:
             raise SyncanySqlCompileException('error join on condition, only "=,!=,>,>=,<,<=,in" operations are supported, related sql "%s"'
                                              % self.to_sql(expression))
 
     def parse_calculate(self, expression, config, arguments, primary_table, calculate_fields):
+        if self.is_aggregate(expression, config, arguments) and hasattr(expression, "final_column"):
+            return
         if isinstance(expression, sqlglot_expressions.Anonymous):
             for arg_expression in expression.args.get("expressions", []):
                 self.parse_calculate(arg_expression, config, arguments, primary_table, calculate_fields)
         elif isinstance(expression, sqlglot_expressions.Cast):
             self.parse_calculate(expression.args["this"], config, arguments, primary_table, calculate_fields)
         elif isinstance(expression, sqlglot_expressions.If):
             self.parse_calculate(expression.args["this"], config, arguments, primary_table, calculate_fields)
@@ -1508,14 +1542,22 @@
                     continue
                 if isinstance(expression.args[arg_type], list):
                     for arg_expression in expression.args.get(arg_type, []):
                         self.parse_calculate(arg_expression, config, arguments, primary_table, calculate_fields)
                 else:
                     self.parse_calculate(expression.args[arg_type], config, arguments, primary_table, calculate_fields)
 
+    def parse_aggregate(self, expression, config, arguments, aggregate_expressions):
+        if self.is_aggregate(expression, config, arguments):
+            aggregate_expressions.append(expression)
+        if not self.is_calculate(expression, config, arguments):
+            return
+        for _, child_expression in expression.args.items():
+            self.parse_aggregate(child_expression, config, arguments, aggregate_expressions)
+
     def parse_table(self, expression, config, arguments):
         db_name = expression.args["db"].name if "db" in expression.args and expression.args["db"] else None
         if isinstance(expression.args["this"], sqlglot_expressions.Dot):
             def parse(expression):
                 return (parse(expression.args["this"]) if isinstance(expression.args["this"],
                                                                      sqlglot_expressions.Dot) else expression.args["this"].name) \
                        + "." + (parse(expression.args["expression"]) if isinstance(expression.args["expression"],
```

### Comparing `syncanysql-0.0.9/syncanysql/config.py` & `syncanysql-0.1.0/syncanysql/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             if not os.path.exists(filename):
                 continue
             if "extends" not in self.config or not isinstance(self.config["extends"], list):
                 self.config["extends"] = []
             if filename not in self.config["extends"]:
                 self.config["extends"].append(filename)
         self.load_config()
-        if custom_config and isinstance(custom_config):
+        if custom_config and isinstance(custom_config, dict):
             self.merge_config(custom_config)
 
         if "timezone" in self.config:
             timezone = self.config.pop("timezone")
             set_timezone(pytz.timezone(timezone))
         if "databases" not in self.config:
             self.config["databases"] = []
```

### Comparing `syncanysql-0.0.9/syncanysql/executor.py` & `syncanysql-0.1.0/syncanysql/executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 # 2023/2/13
 # create by: snower
 
 import os
 import sys
 import re
 import copy
+import threading
 from collections import deque
 from syncany.filters import StringFilter
 from syncany.calculaters import find_calculater
-from syncany.database.memory import MemoryDBFactory, MemoryDBCollection
+from syncany.database import find_database
 from .errors import SyncanySqlCompileException
 from .utils import parse_value
 from .compiler import Compiler
 
 ENV_VARIABLE_RE = re.compile("(\$\{\w+?(:.*?){0,1}\})", re.DOTALL | re.M)
 RAW_SQL_RE = re.compile("(\/\*\s*raw\(([\w\.]+?)\)\s*(\*\/\s*\()?\s*(.*?)\s*(\)\s*\/\*)?\s*endraw\s*\*\/)", re.DOTALL | re.M)
 FUNC_RE = re.compile("^(\w+?)\(((.+),{0,1})*\)$", re.DOTALL)
@@ -59,25 +60,30 @@
             return self[key[1:]]
         if self.parent is None:
             return default
         return self.parent.get(key, default)
 
 
 class Executor(object):
+    _thread_local = threading.local()
     global_env_variables = None
 
+    @classmethod
+    def current(cls):
+        return cls._thread_local.current_executor
+
     def __init__(self, manager, session_config, parent_executor=None):
         self.manager = manager
         self.session_config = session_config
         self.parent_executor = parent_executor
         self.runners = deque()
         self.tasker = None
         if self.global_env_variables is None:
             self.__class__.global_env_variables = EnvVariables.build_global()
-        self.env_variables = parent_executor.env_variables if parent_executor else EnvVariables(self.global_env_variables)
+        self.env_variables = EnvVariables(parent_executor.env_variables if parent_executor else self.global_env_variables)
 
     def compile_variable(self, sql):
         variables = ENV_VARIABLE_RE.findall(sql)
         for variable, default_value in variables:
             variable_name = variable[2:-1].split(":")[0]
             try:
                 variable_value = self.env_variables.get_value(variable_name.lower())
@@ -141,19 +147,31 @@
             return
         self.tasker.terminate()
 
     def add_runner(self, tasker):
         self.runners.append(tasker)
 
     def clear_temporary_memory_collection(self, names):
-        for config_key, factory in self.manager.database_manager.factorys.items():
-            if not isinstance(factory, MemoryDBFactory):
-                continue
-            for driver in factory.drivers:
-                if not isinstance(driver.instance, MemoryDBCollection):
+        try:
+            database_config = dict(**[database for database in self.session_config.get()["databases"]
+                                      if database["name"] == "--"][0])
+        except (TypeError, KeyError, IndexError):
+            return
+        database_cls = find_database(database_config.pop("driver"))
+        if not database_cls:
+            return
+        database = database_cls(self.manager.database_manager, database_config).build()
+        try:
+            for name in names:
+                if self.runners and database.is_streaming(name):
                     continue
-                for key in list(driver.instance.keys()):
-                    if key not in names or (self.runners and
-                                            self.manager.database_manager.get_state(
-                                                config_key + "::" + key, "is_streaming")):
-                        continue
-                    driver.instance.remove(key)
+                delete = database.delete(name, ["id"])
+                delete.commit()
+        finally:
+            database.close()
+
+    def __enter__(self):
+        self._thread_local.current_executor = self
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self._thread_local.current_executor = self.parent_executor
```

### Comparing `syncanysql-0.0.9/syncanysql/main.py` & `syncanysql-0.1.0/syncanysql/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,44 +35,44 @@
                 len(sys.argv) >= 2 and not sys.argv[1].endswith(".sqlx") and not sys.argv[1].endswith(".sql"))):
             global_config.config_logging(False)
         else:
             global_config.config_logging(True)
         manager = TaskerManager(DatabaseManager())
 
         try:
-            executor = Executor(manager, global_config.session())
-            if init_execute_files:
-                executor.run("init", [SqlSegment("execute `%s`" % init_execute_files[i], i + 1) for i in range(len(init_execute_files))])
-                exit_code = executor.execute()
-                if exit_code is not None and exit_code != 0:
-                    return exit_code
+            with Executor(manager, global_config.session()) as executor:
+                if init_execute_files:
+                    executor.run("init", [SqlSegment("execute `%s`" % init_execute_files[i], i + 1) for i in range(len(init_execute_files))])
+                    exit_code = executor.execute()
+                    if exit_code is not None and exit_code != 0:
+                        return exit_code
 
-            if not sys.stdin.isatty() and (len(sys.argv) == 1 or (
-                    len(sys.argv) >= 2 and not sys.argv[1].endswith(".sqlx") and not sys.argv[1].endswith(".sql"))):
-                start_time = time.time()
-                content = sys.stdin.read().strip()
-                if not content:
-                    exit(0)
-                sql_parser = SqlParser(content[1:-1] if content[0] in ('"', "'") and content[-1] in ('"', "'") else content)
-                sqls = sql_parser.split()
-                executor.run("pipe", sqls)
-                exit_code = executor.execute()
-                get_logger().info("execute pipe sql finish with code %d %.2fms", exit_code, (time.time() - start_time) * 1000)
-                exit(exit_code)
-            elif len(sys.argv) >= 2:
-                start_time = time.time()
-                file_parser = FileParser(sys.argv[1])
-                sqls = file_parser.load()
-                executor.run(sys.argv[1], sqls)
-                exit_code = executor.execute()
-                get_logger().info("execute file %s finish with code %d %.2fms", sys.argv[1], exit_code, (time.time() - start_time) * 1000)
-                exit(exit_code)
-            else:
-                cli_prompt = CliPrompt(manager, global_config.session(), executor)
-                exit(cli_prompt.run())
+                if not sys.stdin.isatty() and (len(sys.argv) == 1 or (
+                        len(sys.argv) >= 2 and not sys.argv[1].endswith(".sqlx") and not sys.argv[1].endswith(".sql"))):
+                    start_time = time.time()
+                    content = sys.stdin.read().strip()
+                    if not content:
+                        exit(0)
+                    sql_parser = SqlParser(content[1:-1] if content[0] in ('"', "'") and content[-1] in ('"', "'") else content)
+                    sqls = sql_parser.split()
+                    executor.run("pipe", sqls)
+                    exit_code = executor.execute()
+                    get_logger().info("execute pipe sql finish with code %d %.2fms", exit_code, (time.time() - start_time) * 1000)
+                    exit(exit_code)
+                elif len(sys.argv) >= 2:
+                    start_time = time.time()
+                    file_parser = FileParser(sys.argv[1])
+                    sqls = file_parser.load()
+                    executor.run(sys.argv[1], sqls)
+                    exit_code = executor.execute()
+                    get_logger().info("execute file %s finish with code %d %.2fms", sys.argv[1], exit_code, (time.time() - start_time) * 1000)
+                    exit(exit_code)
+                else:
+                    cli_prompt = CliPrompt(manager, global_config.session(), executor)
+                    exit(cli_prompt.run())
         finally:
             manager.close()
     except SystemError:
         get_logger().error("signal exited")
         exit(130)
     except KeyboardInterrupt:
         get_logger().error("Crtl+C exited")
```

### Comparing `syncanysql-0.0.9/syncanysql/parser.py` & `syncanysql-0.1.0/syncanysql/parser.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.9/syncanysql/prompt.py` & `syncanysql-0.1.0/syncanysql/prompt.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.9/syncanysql/taskers/delete.py` & `syncanysql-0.1.0/syncanysql/taskers/delete.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.9/syncanysql/taskers/execute.py` & `syncanysql-0.1.0/syncanysql/taskers/execute.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # create by: snower
 
 import os
 import time
 from syncany.logger import get_logger
 from ..parser import FileParser
 
+
 class ExecuteTasker(object):
     def __init__(self, config):
         self.config = config
         self.executor = None
 
     def start(self, name, executor, session_config, manager, arguments):
         if self.config["filename"].endswith("sql") or self.config["filename"].endswith("sqlx"):
@@ -19,25 +20,27 @@
                 self.executor = Executor(manager, session_config.session(), executor)
 
             start_time = time.time()
             get_logger().info("execute file %s", self.config["filename"])
             try:
                 file_parser = FileParser(self.config["filename"])
                 sqls = file_parser.load()
-                self.executor.run(self.config["filename"], sqls)
+                with self.executor as executor:
+                    executor.run(self.config["filename"], sqls)
             finally:
                 session_config.merge()
                 get_logger().info("execute file %s finish %.2fms", self.config["filename"], (time.time() - start_time) * 1000)
         else:
             os.system(self.config["filename"])
         return [self]
 
     def run(self, executor, session_config, manager):
         if not self.executor:
             return 0
-        return self.executor.execute()
+        with self.executor as executor:
+            return executor.execute()
 
     def terminate(self):
         if not self.executor:
             return
         self.executor.terminate()
         self.executor = None
```

### Comparing `syncanysql-0.0.9/syncanysql/taskers/explain.py` & `syncanysql-0.1.0/syncanysql/taskers/explain.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,20 +14,16 @@
     def start(self, name, executor, session_config, manager, arguments):
         self.config = copy.deepcopy(self.tasker.config)
         beautify_print("%s tasker %s compiled config:" % (datetime.datetime.now(), self.config["name"]))
         beautify_print(self.config)
         print()
 
         for key in list(arguments.keys()):
-            if key.endswith("@limit"):
-                arguments[key] = 1
-            elif key.endswith("@verbose"):
+            if key.endswith("@verbose"):
                 arguments[key] = True
-        self.tasker.config["output"] = "&.-.&1::" + self.tasker.config["output"].split("::")[-1].split(" ")[0]
-        self.tasker.config["name"] = self.tasker.config["name"] + "#explain"
         self.tasker.start(name, executor, session_config, manager, arguments)
         return [self]
 
     def run(self, executor, session_config, manager):
         try:
             return self.tasker.run(executor, session_config, manager)
         finally:
```

### Comparing `syncanysql-0.0.9/syncanysql/taskers/query.py` & `syncanysql-0.1.0/syncanysql/taskers/query.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.9/syncanysql/taskers/set.py` & `syncanysql-0.1.0/syncanysql/taskers/set.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.9/syncanysql/taskers/show.py` & `syncanysql-0.1.0/syncanysql/taskers/show.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.9/syncanysql/taskers/use.py` & `syncanysql-0.1.0/syncanysql/taskers/use.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self.config = config
 
     def start(self, name, executor, session_config, manager, arguments):
         use_info = [s.strip() for s in self.config["use"].split(" as ")]
         if not use_info[0] or isinstance(use_info[0], (bool, int, float, list, tuple, set, dict)):
             return []
         if isinstance(use_info[0], str):
-            __import__(use_info[0], {}, {})
+            __import__(use_info[0], globals(), locals(), [use_info[0].rpartition(".")[-1]])
         if len(use_info) >= 2:
             if os.path.exists(use_info[0]):
                 session_config.set("sources." + use_info[1], use_info[0])
             else:
                 session_config.set("imports." + use_info[1], use_info[0])
         else:
             if os.path.exists(use_info[0]):
```

### Comparing `syncanysql-0.0.9/syncanysql/utils.py` & `syncanysql-0.1.0/syncanysql/utils.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.9/syncanysql.egg-info/PKG-INFO` & `syncanysql-0.1.0/syncanysql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.0.9
+Version: 0.1.0
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
         [![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
```

### Comparing `syncanysql-0.0.9/syncanysql.egg-info/SOURCES.txt` & `syncanysql-0.1.0/syncanysql.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.cfg
 setup.py
 syncanysql/__init__.py
 syncanysql/compiler.py
 syncanysql/config.py
 syncanysql/errors.py
```

