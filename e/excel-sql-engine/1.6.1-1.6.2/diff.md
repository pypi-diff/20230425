# Comparing `tmp/excel-sql-engine-1.6.1.tar.gz` & `tmp/excel-sql-engine-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excel-sql-engine-1.6.1.tar", last modified: Sun Apr 23 17:33:33 2023, max compression
+gzip compressed data, was "excel-sql-engine-1.6.2.tar", last modified: Tue Apr 25 06:57:24 2023, max compression
```

## Comparing `excel-sql-engine-1.6.1.tar` & `excel-sql-engine-1.6.2.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 17:33:33.469143 excel-sql-engine-1.6.1/
--rw-rw-rw-   0        0        0    14408 2023-03-13 18:23:44.000000 excel-sql-engine-1.6.1/LICENCE
--rw-rw-rw-   0        0        0     8286 2023-04-23 17:33:33.467110 excel-sql-engine-1.6.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-23 17:33:33.398037 excel-sql-engine-1.6.1/PyxlSql/
--rw-rw-rw-   0        0        0      563 2023-03-13 18:23:44.000000 excel-sql-engine-1.6.1/PyxlSql/__init__.py
--rw-rw-rw-   0        0        0     7165 2023-04-22 19:48:11.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlAbstracts.py
--rw-rw-rw-   0        0        0    15468 2023-04-18 13:41:16.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlArgs.py
--rw-rw-rw-   0        0        0    37421 2023-04-21 17:35:39.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlEngine.py
--rw-rw-rw-   0        0        0     2934 2023-03-13 18:23:44.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlErrors.py
--rw-rw-rw-   0        0        0    26449 2023-04-18 13:02:23.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlGrammar.py
--rw-rw-rw-   0        0        0     9159 2023-04-21 18:05:53.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlPivot.py
--rw-rw-rw-   0        0        0     7231 2023-03-21 21:57:15.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlResults.py
--rw-rw-rw-   0        0        0    14165 2023-04-21 18:17:44.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlSheets.py
--rw-rw-rw-   0        0        0    14107 2023-04-22 19:48:11.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlSql.py
--rw-rw-rw-   0        0        0    14413 2023-03-20 16:49:03.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlStages.py
--rw-rw-rw-   0        0        0    18944 2023-04-21 15:56:11.000000 excel-sql-engine-1.6.1/PyxlSql/pyxlWorkbook.py
--rw-rw-rw-   0        0        0     7585 2023-04-21 09:26:14.000000 excel-sql-engine-1.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 17:33:33.451088 excel-sql-engine-1.6.1/excel_sql_engine.egg-info/
--rw-rw-rw-   0        0        0     8286 2023-04-23 17:33:33.000000 excel-sql-engine-1.6.1/excel_sql_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      574 2023-04-23 17:33:33.000000 excel-sql-engine-1.6.1/excel_sql_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 17:33:33.000000 excel-sql-engine-1.6.1/excel_sql_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-23 17:33:33.000000 excel-sql-engine-1.6.1/excel_sql_engine.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      196 2023-04-20 15:20:18.000000 excel-sql-engine-1.6.1/excel_sql_engine.egg-info/setup.cfg
--rw-rw-rw-   0        0        0        8 2023-04-23 17:33:33.000000 excel-sql-engine-1.6.1/excel_sql_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 17:33:33.470154 excel-sql-engine-1.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1306 2023-04-23 17:27:56.000000 excel-sql-engine-1.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-23 17:33:33.461088 excel-sql-engine-1.6.1/tests/
--rw-rw-rw-   0        0        0     7703 2023-04-17 15:39:30.000000 excel-sql-engine-1.6.1/tests/test_Northwind.py
--rw-rw-rw-   0        0        0     6381 2023-04-18 14:00:43.000000 excel-sql-engine-1.6.1/tests/test_tooling.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:57:24.798802 excel-sql-engine-1.6.2/
+-rw-rw-rw-   0        0        0       83 2023-04-23 21:39:10.000000 excel-sql-engine-1.6.2/LICENCE
+-rw-rw-rw-   0        0        0     8286 2023-04-25 06:57:24.796764 excel-sql-engine-1.6.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-25 06:57:24.765663 excel-sql-engine-1.6.2/PyxlSql/
+-rw-rw-rw-   0        0        0      496 2023-04-24 07:16:16.000000 excel-sql-engine-1.6.2/PyxlSql/__init__.py
+-rw-rw-rw-   0        0        0      481 2023-04-24 15:44:58.000000 excel-sql-engine-1.6.2/PyxlSql/__main__.py
+-rw-rw-rw-   0        0        0     7162 2023-04-24 08:11:45.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlAbstracts.py
+-rw-rw-rw-   0        0        0    15468 2023-04-18 13:41:16.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlArgs.py
+-rw-rw-rw-   0        0        0    37463 2023-04-24 12:07:56.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlEngine.py
+-rw-rw-rw-   0        0        0     3450 2023-04-24 15:42:26.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlErrors.py
+-rw-rw-rw-   0        0        0     9367 2023-04-24 18:03:18.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlFullHelp.py
+-rw-rw-rw-   0        0        0    26457 2023-04-24 17:57:14.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlGrammar.py
+-rw-rw-rw-   0        0        0      115 2023-04-23 21:45:08.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlLicence.py
+-rw-rw-rw-   0        0        0     9159 2023-04-21 18:05:53.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlPivot.py
+-rw-rw-rw-   0        0        0     7231 2023-03-21 21:57:15.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlResults.py
+-rw-rw-rw-   0        0        0    14165 2023-04-21 18:17:44.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlSheets.py
+-rw-rw-rw-   0        0        0    14617 2023-04-24 18:07:21.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlSql.py
+-rw-rw-rw-   0        0        0    14413 2023-03-20 16:49:03.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlStages.py
+-rw-rw-rw-   0        0        0      493 2023-04-25 06:57:23.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlVersion.py
+-rw-rw-rw-   0        0        0    18371 2023-04-24 12:47:48.000000 excel-sql-engine-1.6.2/PyxlSql/pyxlWorkbook.py
+-rw-rw-rw-   0        0        0     7585 2023-04-21 09:26:14.000000 excel-sql-engine-1.6.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 06:57:24.785652 excel-sql-engine-1.6.2/excel_sql_engine.egg-info/
+-rw-rw-rw-   0        0        0     8286 2023-04-25 06:57:24.000000 excel-sql-engine-1.6.2/excel_sql_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      664 2023-04-25 06:57:24.000000 excel-sql-engine-1.6.2/excel_sql_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 06:57:24.000000 excel-sql-engine-1.6.2/excel_sql_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-25 06:57:24.000000 excel-sql-engine-1.6.2/excel_sql_engine.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      196 2023-04-20 15:20:18.000000 excel-sql-engine-1.6.2/excel_sql_engine.egg-info/setup.cfg
+-rw-rw-rw-   0        0        0        8 2023-04-25 06:57:24.000000 excel-sql-engine-1.6.2/excel_sql_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 06:57:24.798802 excel-sql-engine-1.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1306 2023-04-25 06:57:23.000000 excel-sql-engine-1.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:57:24.792764 excel-sql-engine-1.6.2/tests/
+-rw-rw-rw-   0        0        0     7751 2023-04-24 18:02:02.000000 excel-sql-engine-1.6.2/tests/test_Northwind.py
+-rw-rw-rw-   0        0        0     6411 2023-04-24 18:02:02.000000 excel-sql-engine-1.6.2/tests/test_tooling.py
```

### Comparing `excel-sql-engine-1.6.1/PKG-INFO` & `excel-sql-engine-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel-sql-engine
-Version: 1.6.1
+Version: 1.6.2
 Summary: A tiny SQL engine for Excel files, based on Openpyxl
 Home-page: https://gitlab.com/fabien.battini/pyxlsql
 Author: Fabien BATTINI
 Author-email: fabien.battini@gmail.com
 Keywords: excel sql
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
```

### Comparing `excel-sql-engine-1.6.1/PyxlSql/pyxlAbstracts.py` & `excel-sql-engine-1.6.2/PyxlSql/pyxlAbstracts.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 from PyxlSql.pyxlSheets import PyxlSheet
 
 
 class AbstractRunner:
     def __init__(self, arguments=None):
         self.arguments = arguments
 
-    def run_first(self):
-        raise PyxlSqlInternalError(f"AbstractRunner.run_first() on {self.name}")
+    def run(self):
+        raise PyxlSqlInternalError(f"AbstractRunner.run() on {type(self)}")
 
     def build(self, arguments=None):
-        raise PyxlSqlInternalError(f"AbstractRunner.build() on {self.name}")
+        raise PyxlSqlInternalError(f"AbstractRunner.build() on {type(self)}")
 
 # ---------------------------------------------------------------------------------------------------------------
 # Forward declaration of Statement, because used in the Parser code
 # ---------------------------------------------------------------------------------------------------------------
 
 
 class AbstractStatement:
@@ -119,33 +119,33 @@
             self.dst_sheet_arg = None
         else:
             self.dst_sheet_arg = command.dst_sheet_arg
 
         self.specification = specification
 
     def evaluate(self, _inputs: AbstractResult, _outputs: AbstractResult):
-        raise PyxlSqlInternalError(f"Arg.evaluate() on {self.name}")
+        raise PyxlSqlInternalError(f"Arg.evaluate() on {type(self)}")
 
     def get_constant(self):
-        raise PyxlSqlInternalError(f"Arg.get_constant() on {self.name}")
+        raise PyxlSqlInternalError(f"Arg.get_constant() on {type(self)}")
 
     def find_name_and_sheet(self, not_in_src=False):
-        raise PyxlSqlInternalError(f"Arg.find_name_and_sheet() on {self.name}")
+        raise PyxlSqlInternalError(f"Arg.find_name_and_sheet() on {type(self)}")
 
     def set_sheet_number(self, nb: int):
-        raise PyxlSqlInternalError(f"Arg.set_sheet_number() on {self.name}")
+        raise PyxlSqlInternalError(f"Arg.set_sheet_number() on {type(self)}")
 
     def get_sheet_name(self) -> str:
-        raise PyxlSqlInternalError(f"Arg.get_sheet_name() on {self.name}")
+        raise PyxlSqlInternalError(f"Arg.get_sheet_name() on {type(self)}")
 
     def get_sheet(self) -> PyxlSheet:
-        raise PyxlSqlInternalError(f"Arg.get_sheet() on {self.name}")
+        raise PyxlSqlInternalError(f"Arg.get_sheet() on {type(self)}")
 
     def verify_fields(self, not_in_src=False, not_in_dst=False):
-        raise PyxlSqlInternalError(f"Arg.verify_fields() on {self.name}")
+        raise PyxlSqlInternalError(f"Arg.verify_fields() on {type(self)}")
 
 
 # ---------------------------------------------------------------------------------------------------------------
 # Clause
 # ---------------------------------------------------------------------------------------------------------------
 
 class Clause(AbstractStatement):
```

### Comparing `excel-sql-engine-1.6.1/PyxlSql/pyxlArgs.py` & `excel-sql-engine-1.6.2/PyxlSql/pyxlArgs.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6.1/PyxlSql/pyxlEngine.py` & `excel-sql-engine-1.6.2/PyxlSql/pyxlEngine.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,19 +368,19 @@
         self.filename = filename.get_constant()
         self.workbook = dst_wb.get_workbook(workbook.get_constant()) if workbook else dst_wb
         # filename.verify_fields(not_in_src=True)  # useless: never a field
 
     def execute(self):
 
         for sheet in self.workbook.sheets_to_delete:
-            print(f"EXECUTE DELETE {sheet}")
+            print(f"EXECUTE DELETE {sheet}", flush=True)
             self.dst_wb.delete_sheet(sheet)
         self.workbook.sheets_to_delete = []
 
-        print(f"EXECUTE {self.name} {self.filename}")
+        print(f"EXECUTE {self.name} {self.filename}", flush=True)
         self.workbook.save(self.filename)
 
 
 class ExportCmd(Cmd):
     name = 'EXPORT HTML'
     help = "Saves the workbook as an HTML file in 'Filename'"
 
@@ -475,19 +475,19 @@
         """
         LOAD  filename
         """
         super().__init__(runner, dst_wb)
         self.filename = filename.get_constant()
 
     def execute(self):
-        print(f"EXECUTE {self.name} {self.filename}")
+        print(f"EXECUTE {self.name} {self.filename}",flush=True)
 
         runner = self.runner
-        cmdline = runner.build(["-f", "tests/" + self.filename])
-        cmdline.run_first()
+        cmdline = runner.build([self.dst_wb.file_path + '/' + self.filename])
+        cmdline.run()
 
 
 class DatabaseCmd(Cmd):
     """
     Class used to load data from an Excel sheet by specifying non default start and end
     "DATABASE" src_sheet "START" cell "END" cell
     """
```

### Comparing `excel-sql-engine-1.6.1/PyxlSql/pyxlErrors.py` & `excel-sql-engine-1.6.2/PyxlSql/pyxlErrors.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # developed by fabien.battini@gmail.com
 # ---------------------------------------------------------------------------------------------------------------
 
 # ---------------------------------------------------------------------------------------------------------------
 # Management of exceptions for PyxlSql
 # ---------------------------------------------------------------------------------------------------------------
 
-
+import sys
 class PyxlSqlError(Exception):
     """Base class for exceptions in this module."""
     current_line = ""
     error_count = 0
     error_list: list[str] = []
     warning_count = 0
     warning_list: list[str] = []
@@ -36,46 +36,62 @@
         PyxlSqlError.warning_list.append(msg)
 
     @staticmethod
     def info(msg):
         print(f"Info: {msg}")
 
     def print(self, level="ERROR"):
-        print(f"\n{level}: {PyxlSqlError.current_line or ''}")
+        print(f"\n{level}: {PyxlSqlError.current_line or 'not a SQL statement'}")
         print(f"{level}:     {self.message}")
-        print(f"{level}:     {self.context}\n")
+        print(f"{level}:     {self.context}\n", flush=True)
+        sys.stdout.flush()
         PyxlSqlError.error_count += 1
         PyxlSqlError.error_list.append(PyxlSqlError.current_line + " " + self.message + " " + self.context)
         if PyxlSqlError.error_count > 20:
-            print("\nFATAL ERROR: Too much errors, aborting")
+            print("\nFATAL ERROR: Too much errors, aborting", flush=True)
             exit(-1)
 
     @staticmethod
     def set_line(filename, line_number, *items):
         PyxlSqlError.current_line = f"{filename}:{line_number}: "
         for f in items:
             PyxlSqlError.current_line += " '" + str(f) + "'"
 
+class PyxlSqlWarning(PyxlSqlError):
+    def __init__(self, msg, context: str):
+        super().__init__(msg, context)
+        self.warning(msg)
 
 class PyxlSqlInternalError(PyxlSqlError):
     def __init__(self, context: str):
         super().__init__("Internal ", context)
+        self.print()
 
 
 class PyxlSqlColumnError(PyxlSqlError):
     def __init__(self, column, context: str):
         super().__init__(f"unknown column '{column}'", context)
+        self.print()
 
 
 class PyxlSqlSheetError(PyxlSqlError):
     def __init__(self, sheet, context: str):
         super().__init__(f"unknown sheet '{sheet}'", context)
+        self.print()
 
 
 class PyxlSqlParseError(PyxlSqlError):
     def __init__(self, message, context: str):
         super().__init__("SQL SYNTAX : " + message, context)
+        self.print()
 
 
 class PyxlSqlExecutionError(PyxlSqlError):
     def __init__(self, message, context: str):
         super().__init__("PYTHON SYNTAX : " + message, context)
+        self.print()
+
+
+class PyxlSqlCmdlineError(PyxlSqlError):
+    def __init__(self, message, context: str):
+        super().__init__("Arguments : " + message, context)
+        self.print()
```

### Comparing `excel-sql-engine-1.6.1/PyxlSql/pyxlGrammar.py` & `excel-sql-engine-1.6.2/PyxlSql/pyxlGrammar.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,18 +42,20 @@
     """the Abstract class for all items that can be parsed by the Parser"""
 
     def __init__(self, runner: AbstractRunner, sub_tokens=None, sub_clauses=None):
         self.name: str = "INTERNAL ERROR"
         self.sub_tokens: list = sub_tokens if sub_tokens is not None else []
         self.runner = runner
         self.sub_clauses_names = []
+
         if sub_clauses is not None:
             for cl in sub_clauses:
                 self.sub_clauses_names.append(cl.name)
 
+
     def accepts(self, clause_parser):
         """
         :param clause_parser: Token
         :return: True if self accepts 'clause' as a sub item
         """
         name = clause_parser.name
         for cl in self.sub_clauses_names:
@@ -524,14 +526,16 @@
 
         # Dababase_cmd   := "DATABASE" src_sheet "START" cell "END" cell
         self.add(CmdToken(self.runner, DatabaseCmd,
                           sub_tokens=[SheetToken(self.runner, "sheet"),
                                       KeywordToken(self.runner, "START"), StringToken(self.runner, "start"),
                                       KeywordToken(self.runner, "END"), StringToken(self.runner, "end")]))
 
+
+
     def add(self, item: Token):
         """
         :param item: Token
         :return: None
         """
         self.items[item.name] = item
         if self.help is None:
```

### Comparing `excel-sql-engine-1.6.1/PyxlSql/pyxlPivot.py` & `excel-sql-engine-1.6.2/PyxlSql/pyxlPivot.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6.1/PyxlSql/pyxlResults.py` & `excel-sql-engine-1.6.2/PyxlSql/pyxlResults.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6.1/PyxlSql/pyxlSheets.py` & `excel-sql-engine-1.6.2/PyxlSql/pyxlSheets.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6.1/PyxlSql/pyxlSql.py` & `excel-sql-engine-1.6.2/PyxlSql/pyxlSql.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,27 +4,31 @@
 # developed by fabien.battini@gmail.com
 # ---------------------------------------------------------------------------------------------------------------
 
 
 import argparse
 import os
 import re
+import sys
 from typing import Optional
-from PyxlSql.pyxlErrors import PyxlSqlError
+from PyxlSql.pyxlErrors import PyxlSqlError, PyxlSqlCmdlineError
 from PyxlSql.pyxlSheets import PyxlSheet
 from PyxlSql.pyxlWorkbook  import   PyxlWorkbook
 from PyxlSql.pyxlEngine import AbstractStatement
 from PyxlSql.pyxlGrammar import Parser
 from PyxlSql.pyxlAbstracts import AbstractRunner
+from PyxlSql.pyxlVersion import PyxlVersion
+from PyxlSql.pyxlLicence import PyxlLicence
+from PyxlSql.pyxlFullHelp import PyxlFullHelp
 
 # how to get openpyxl, pytest etc.,
 # shell>python -m pip install --upgrade openpyxl pytest setuptools wheel tox pytest-flakes pytest-cov sphinx gitpython
 
 # how to test: (cf tox.ini, which does everything)
-# (venv) PyxlSQL> pyxlSql -f tests/Test_pyxlsql.xlsx  #noqa
+# (venv) PyxlSQL> pyxlSql -f tests/Test_pyxlsql.xlsx  # noqa
 # (venv) PyxlSQL> pytest --cache-clear --ff
 # (venv) PyxlSQL> pytest --flakes
 # (venv) PyxlSQL> pytest --cov --cov-report html --cov-report term
 # (venv) PyxlSQL> sphinx-build source build/html -W -b html
 # or:
 # (venv) PyxlSQL> tox
 
@@ -35,23 +39,24 @@
 # REQ 0002: PyxlSQL statements are stored 'Pyxl SQL' sheet
 # REQ 0003: Sheet are described as 'sheet name' or 'filename.xlsx[sheet name]'
 # REQ 0004: remove start/trailing spaces for Command, Clause, field names, it is a common error, hard to find
 # REQ 0005: Import functools automatically, otherwise MIN/MAX do not work
 # REQ 0006: Requirements and FIX ME should be extracted automatically from the source code and published in doc
 # Req 0007: Use API token to upload on Pypi. see  https://pyptoxi.org/help/#apitoken and https://pypi.org/manage/account/token/
 # REQ 0008: Generate to do.rst through tox, using parse_requirements.py
-# REQ 0009: publish also htmlcov on gitlab.io
+# REQ 0009: publish also htmlcov on gitlab.io  # noqa
 # REQ 0010: create a downloadable executable for windows user : python -m pip install PyInstaller #
 # TODO: REQ 0011: create a doc specific to windows user that do not know python
 # REQ 0012: manage also .ods files from LibreOffice: NO, this is NOT possible, OpenPyxl does NOT read .ods format
 # REQ 0013: LAZY reading of sheets: only sheets that are referred by the SQL commands are read.
 
 # TODO: REQ 0014: 100% coverage: most of not covered lines are defensive code which is unreachable by design
 # DONE: Update current documentation xxx.rst because @ is often replaced by # in examples, due to more strict typing
-
+# TODO: REQ 0015 --max-errors = int, default = 20. Maximum number of errors
+# REQ 0016 --full-help : describes the grammar
 
 # ----------------------- Cmdline arguments
 # REQ 1001: --dir/-d directory: processes all Excel files in the directory
 # REQ 1002: --file/-f file (multiple times): process this file
 # REQ 1003: --filepath/-p dir (multiple times): adds directory to path for included Excel files
 # REQ 1004: the directory of the file being processed is added in the filepath
 # TODO: REQ 1005: --data-only: reads excel file with the data-only flag
@@ -63,15 +68,15 @@
 #             then erases this line
 # REQ 2002: Update_cmd     := "UPDATE" dst_sheet: string
 # REQ 2003: Import_cmd     := "IMPORT" module ("SUBS" sub_modules)
 #           Behavior: allows to use more features in the EXPRESSION clauses by importing python libs
 # REQ 2004: Delete_cmd     := "DELETE" dst_sheet
 #           Behavior : remove a sheet, e.g. the Micro SQL sheet
 # REQ 2005: Save_cmd       := "SAVE" filename ("FROM" Workbook)
-#           Behavior: file saved is writen with the same directory than the original file
+#           Behavior: file saved is writen with the same directory as the original file
 #           If workbook is specified, then this workbook is saved (which has little use)
 # REQ 2006: Rename_cmd      := "RENAME" dst_sheet "AS" new_name
 # REQ 2007: SELECT
 
 # HOW TO do a multiple stages approach
 # ------------------------------------
 #    For instance, to save intermediate stages, or to cut processing into several sheets
@@ -168,16 +173,16 @@
 # ---------------------------------------------------------------------------------------------------
 
 
 class SqlWb(PyxlWorkbook):
     column_names = 'STATEMENT', 'First', 'KEY', 'Second', 'CONDITION', 'Third'
     sql_sheet_name = 'Pyxl SQL'
 
-    def __init__(self, runner: AbstractRunner, file_name, file_path=None):
-        super().__init__(file_name, file_path=file_path)
+    def __init__(self, runner: AbstractRunner, file_name):
+        super().__init__(file_name)
         self.runner = runner
         self.parser = Parser(runner)
         self.parse_commands()
 
     def parse_commands(self):
         current_command: Optional[AbstractStatement] = None
         active_sheet: PyxlSheet
@@ -191,16 +196,17 @@
 
         for row in active_sheet.get_row_range():
             word = active_sheet.get_val(row, self.column_names[0])
             if word is None:
                 if current_command is not None and current_command.is_a_command():
                     try:
                         current_command.execute()
-                    except PyxlSqlError as error:
-                        error.print("Executing")
+                    except PyxlSqlError:
+                        print("Errors during parsing, trying to continue...", flush=True)
+                        sys.stdout.flush()
                 current_command = None
                 continue
 
             values = []
             cells = []
             for param in self.column_names[1:]:
                 val = active_sheet.get_val(row, param)
@@ -210,72 +216,89 @@
                 values.append(val)
                 cells.append(cell)
 
             PyxlSqlError.set_line(self.filename + ':[' + SqlWb.sql_sheet_name + ']', row, [word]+values)
             try:
                 all_vals = [v.strip() if isinstance(v,str) else v for v in [word]+values] # R E Q 0004
                 new_item = self.parser.parse(active_sheet, all_vals, cells)
-            except PyxlSqlError as current_error:
-                current_error.print()
+            except PyxlSqlError:
+                print("Errors during parsing, trying to continue...", flush=True)
+                sys.stdout.flush()
                 continue
 
             if new_item.is_a_command():
                 if current_command is not None and current_command.is_a_command():
-                    current_command.execute()
+                    try:
+                        current_command.execute()
+                    except PyxlSqlError:
+                        print("Errors during execution, trying to continue...", flush=True)
+                        sys.stdout.flush()
+                        continue
                 current_command = new_item
 
         if current_command is not None and current_command.is_a_command():
-            current_command.execute()
+            try:
+                current_command.execute()
+            except PyxlSqlError:
+                print("Errors during execution, trying to continue...", flush=True)
+                sys.stdout.flush()
+
 
 
 # ------------------------------------------------------------
 # Class PyxlSqlRunner
 # ------------------------------------------------------------
 
 
 class PyxlRunner(AbstractRunner):
     def __init__(self, arguments=None):
         super().__init__()
         self.parser = argparse.ArgumentParser(description='execute PyxlSql commands in Excel files')
-        self.parser.add_argument('--filepath', '-p', help="path for included files", type=str, action='append')
-        self.parser.add_argument('--files', '-f', help="(multiple times): process this file",
-                                 type=str, dest='files', action='append')
-        self.parser.add_argument('--dir', '-d', help="process all excel files in the directory",
-                                 type=str, dest='dir', action='store')
+        # -h, --help is implicit
+        self.parser.add_argument('files', help="file to be processed (multiple times)",
+                                 type=str, action='append')
 
-        self.parser.add_argument('--licence', help="prints the LICENCE", action='store_true')
+        self.parser.add_argument('--filepath', '-p', help="path for included files", type=str, action='append')
+        self.parser.add_argument('--licence', '-l', help="prints the LICENCE", action='store_true')
+        self.parser.add_argument('--version', help="prints the version", action='store_true')
         self.parser.add_argument('--full-help', help="prints the complete help, and exits", action='store_true')
-        self.parser.add_argument('--parse-only', help="parse PyxlSql commands, verifies syntax only, and exits",
-                                 action='store_true')
+        # self.parser.add_argument('--parse-only', help="parse PyxlSql commands, verifies syntax only, and exits",
+        #                          action='store_true')
 
         self.args = self.parser.parse_args() if arguments is None else self.parser.parse_args(arguments)
 
-        d = self.args.dir or "."
-        self.dir = d if d[-1] == "/" or d[-1] == '\\' else d+"/"
-        file_path = self.args.filepath or [self.dir]
-        self.file_path = list(map(lambda f: f if f[-1] == "/" or f[-1] == '\\' else f+"/", file_path))
-        self.files = self.args.files or list(map(lambda f: self.dir + f, os.listdir(self.dir)))
+        self.files = self.args.files
+
+
+        if self.args.version:
+            version = PyxlVersion()
+            print(f"pyxlSql {version.version}")
+
+        if self.args.licence:
+            licence = PyxlLicence()
+            licence.print()
+
+        if self.args.full_help:
+            full = PyxlFullHelp()
+            full.print()
+
+
 
     def build(self, arguments=None):
         return PyxlRunner(arguments)
 
     def run(self):
-        for existing_file in self.files:
-            if os.path.isfile(existing_file):
-                if re.match(r".*\.xls(x|m|)$", existing_file):
-                    SqlWb(self, existing_file, file_path=self.file_path)
+        for file in self.files:
+            if os.path.isfile(file):
+                if re.match(r".*\.xls(x|m|)$", file):
+                    return SqlWb(self, file)
+                else:
+                    raise PyxlSqlCmdlineError(f"file '{file}' is not Excel", "command line arguments")
             else:
-                PyxlSqlError("Non existing file", '{' + existing_file + '}')
-
-    def run_first(self):
-        """Used for tests with pytest"""
-        for existing_file in self.files:
-            if os.path.isfile(existing_file) and re.match(r".*\.xls(x|m|)$", existing_file):
-                return SqlWb(self, existing_file, file_path=self.file_path)
-        raise PyxlSqlError("No file to process", '{' + self.files[0] + '}')
+                raise PyxlSqlCmdlineError(f"file '{file}' does not exist", "command line arguments")
 
 def run_pyxl_sql():
     my_runner = PyxlRunner()
     my_runner.run()
 
 if __name__ == "__main__":
-    run_pyxl_sql()
+    run_pyxl_sql()
```

### Comparing `excel-sql-engine-1.6.1/PyxlSql/pyxlStages.py` & `excel-sql-engine-1.6.2/PyxlSql/pyxlStages.py`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6.1/PyxlSql/pyxlWorkbook.py` & `excel-sql-engine-1.6.2/PyxlSql/pyxlWorkbook.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,25 +19,22 @@
 
 
 class PyxlWorkbook:
     """
     class to manage excel workbooks structured as a database
     """
     def __init__(self, file_name, create=False, first_row=1, first_column= 1, last_row=None, last_column=None,
-                 font=None, file_path: list=[]):
-        self.file_path = file_path or []
-        self.filename = self.find_file(file_name)
+                 font=None):
 
-        if self.filename is None:
-            print(f"FATAL ERROR: Cannot find '{file_name}' in path '{self.file_path}', aborting")
-            exit(-1)
 
-        local_path = os.path.dirname(self.filename)
-        if local_path not in self.file_path:
-            self.file_path.append(local_path)
+        if file_name is None:
+            raise PyxlSqlError(f"Call PyxlWorkbook with file '{None}'", "command line arguments")
+
+        self.filename = file_name
+        self.file_path= os.path.dirname(self.filename) or '.'
 
         try:
             self.wb: openpyxl.workbook = openpyxl.load_workbook(filename=self.filename)
         except OSError as error:
             print(f"FATAL ERROR: Cannot open '{file_name}' : {str(error)}, aborting")
             exit(-1)
 
@@ -138,27 +135,14 @@
 
         m = re.search(r'<a:folHlink><a:srgbClr val="([\dABCDEF]*)"/></a:folHlink>', theme_desc)
         if m:
             theme.append(m.group(1))
 
         return theme
 
-    def find_file(self, filename):
-        if filename is None:
-            return None
-        if os.path.exists(filename):
-            return filename
-        for d in self.file_path:
-            if d[-1] != "/":
-                d += "/"
-            f = os.path.realpath(d + filename)
-            if os.path.exists(f):
-                return f
-        return None
-
     def get_sheet(self, sheet_name, first_row=None, first_column=None, last_row=None, last_column=None,
                   raise_exception=True, to_read=True):
         first_row = first_row or self.first_row
 
         if sheet_name is None:
             return None
         if sheet_name in self.sheets:
@@ -208,15 +192,15 @@
         sheet.rename(new_sheet_name)
         self.sheets[new_sheet_name]=sheet
         self.sheets.pop(old_sheet_name)
 
     def save(self, file_name):
         current_dir = os.path.dirname(os.path.realpath(self.filename))
         try:
-            self.wb.save(current_dir + "\\" + file_name)
+            self.wb.save(current_dir + "/" + file_name)
         except OSError as err:
             raise PyxlSqlExecutionError(f" file '{current_dir}\\{file_name}' is read-only", str(err))
 
     @staticmethod
     def local_open(file_name: str, mode: str):
         try:
             ins = open(file_name, mode)
@@ -430,15 +414,15 @@
             outs.write('      </table>\n')
             outs.write('   </div>\n')
         outs.write('</body>\n')
         outs.write('</html>\n')
 
     def get_workbook(self, name):
         if name not in self.wbs:
-            self.wbs[name] = PyxlWorkbook(name, file_path=self.file_path)
+            self.wbs[name] = PyxlWorkbook(self.file_path+'/'+name)
         return self.wbs[name]
 
     def import_module(self, module, sub_modules=None):
         mod = importlib.import_module(module)
         if sub_modules is None:
             self.imported[module] = mod
             return
```

### Comparing `excel-sql-engine-1.6.1/README.md` & `excel-sql-engine-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `excel-sql-engine-1.6.1/excel_sql_engine.egg-info/PKG-INFO` & `excel-sql-engine-1.6.2/excel_sql_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel-sql-engine
-Version: 1.6.1
+Version: 1.6.2
 Summary: A tiny SQL engine for Excel files, based on Openpyxl
 Home-page: https://gitlab.com/fabien.battini/pyxlsql
 Author: Fabien BATTINI
 Author-email: fabien.battini@gmail.com
 Keywords: excel sql
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
```

### Comparing `excel-sql-engine-1.6.1/excel_sql_engine.egg-info/SOURCES.txt` & `excel-sql-engine-1.6.2/excel_sql_engine.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 LICENCE
 README.md
 setup.py
 PyxlSql/__init__.py
+PyxlSql/__main__.py
 PyxlSql/pyxlAbstracts.py
 PyxlSql/pyxlArgs.py
 PyxlSql/pyxlEngine.py
 PyxlSql/pyxlErrors.py
+PyxlSql/pyxlFullHelp.py
 PyxlSql/pyxlGrammar.py
+PyxlSql/pyxlLicence.py
 PyxlSql/pyxlPivot.py
 PyxlSql/pyxlResults.py
 PyxlSql/pyxlSheets.py
 PyxlSql/pyxlSql.py
 PyxlSql/pyxlStages.py
+PyxlSql/pyxlVersion.py
 PyxlSql/pyxlWorkbook.py
 excel_sql_engine.egg-info/PKG-INFO
 excel_sql_engine.egg-info/SOURCES.txt
 excel_sql_engine.egg-info/dependency_links.txt
 excel_sql_engine.egg-info/entry_points.txt
 excel_sql_engine.egg-info/setup.cfg
 excel_sql_engine.egg-info/top_level.txt
```

### Comparing `excel-sql-engine-1.6.1/setup.py` & `excel-sql-engine-1.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # CAVEAT : This file is edited by tests/patch_files.py to setup the version name from the latest tag
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # see https://setuptools.pypa.io/en/latest/references/keywords.html
 setuptools.setup(
     name="excel-sql-engine",
-    version="1.6.1",
+    version="1.6.2",
     author="Fabien BATTINI",
     author_email="fabien.battini@gmail.com",
     description="A tiny SQL engine for Excel files, based on Openpyxl",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/fabien.battini/pyxlsql",
     license_files=["LICENCE"],
```

### Comparing `excel-sql-engine-1.6.1/tests/test_Northwind.py` & `excel-sql-engine-1.6.2/tests/test_Northwind.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 from test_tooling import TestedWb
 from PyxlSql.pyxlErrors import PyxlSqlError
 from PyxlSql.pyxlWorkbook import PyxlWorkbook
 
 
 def test_northwind():
     PyxlSqlError.reset()
-    TestedWb.build("Environemental.xlsx")  # noqa   should not contain any code
+    TestedWb.build(["tests/Environemental.xlsx"])  # noqa   should not contain any code
     TestedWb.assert_warning_start(0, 'file \'tests/Environemental.xlsx\' does not ')  # noqa
     TestedWb.assert_warning_number(1)
     PyxlSqlError.reset()
 
-    tcl = TestedWb.build("Test_pyxlsql.xlsx") # noqa
+    tcl = TestedWb.build(["tests/Test_pyxlsql.xlsx"]) # noqa
 
     TestedWb.assert_line(tcl, "Auto", 2, ["Info 0", "Argentina", 10250, 12300, 14760, "=(C2+D2+E2)/3"], delta=1.0)
     TestedWb.assert_line(tcl, "Auto", 3, ["Info 1", "Austria",   22365, 26838, 32205, "=(C3+D3+E3)/3"], delta=1.0)
     TestedWb.assert_line(tcl, "Auto", 25, ["Info 23", "Venezuela", 35268, 42321, 50785, "=(C25+D25+E25)/3"], delta=1.0)
     TestedWb.assert_line(tcl, "Auto", 26, [None, None, None, None, None, None], delta=1.0)
     # testing propagation of formatting
     TestedWb.assert_format(tcl, "Auto", "2019", 3, "Auto", "2019", 2,
@@ -104,21 +104,21 @@
     TestedWb.assert_line(tcl, "Pivot", 2,
                          ["Medium",	"Y", "USA",	"= E2/$E$25"])
     TestedWb.assert_line(tcl, "Pivot", 3,
                          ["High", "Y", "Canada", "= E3/$E$25"])
     TestedWb.assert_line(tcl, "Pivot", 24,
                         [None,None, "Switzerland",	"= E24/$E$25"])
 
-    step2 = PyxlWorkbook("tests/outputs/northwind-results-stage2.xlsx", file_path=["./"])  # noqa
+    step2 = PyxlWorkbook("tests/outputs/northwind-results-stage2.xlsx")  # noqa
     TestedWb.assert_not_none(step2, "Header", "Value", 2)
     TestedWb.assert_line(step2, "Best", 2, ["Info 9", "Finland", 12228.4586666667], delta = 0.5)
     TestedWb.assert_line(step2, "Best", 24, ["Info 22", "USA", 678008.24], delta = 0.5)
 
     PyxlSqlError.reset()
-    TestedWb.build("test_errors.xlsx")
+    TestedWb.build(["tests/test_errors.xlsx", "--full-help", "--version", "--licence"] )
     TestedWb.assert_error_start(0, 'tests/test_errors.xlsx:[Pyxl SQL]:3:  \'[\'WHERE\',')
     TestedWb.assert_error_start(1, 'tests/test_errors.xlsx:[Pyxl SQL]:5:  \'[\'UPDATE\', ')
     TestedWb.assert_error_start(2, 'tests/test_errors.xlsx:[Pyxl SQL]:6:  \'[\'LEFT JOIN\',')
     TestedWb.assert_error_start(3, 'tests/test_errors.xlsx:[Pyxl SQL]:11:  \'[\'EXAMPLE ERROR\',')
 
     TestedWb.assert_error_number(4)
```

### Comparing `excel-sql-engine-1.6.1/tests/test_tooling.py` & `excel-sql-engine-1.6.2/tests/test_tooling.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 sys.path.append(os.path.dirname(os.path.dirname(os.path.realpath(__file__))))
 from PyxlSql.pyxlSql import  SqlWb, PyxlRunner
 from PyxlSql.pyxlErrors import PyxlSqlError
 
 
 class TestedWb:
     @staticmethod
-    def build(filename):
-        cmdline = PyxlRunner(["-f", "tests/" + filename])
-        sql: SqlWb = cmdline.run_first()
+    def build(args):
+        cmdline = PyxlRunner(args)
+        sql: SqlWb = cmdline.run()
         return sql
 
     @staticmethod
     def get_line(sql: SqlWb, sheet_name: str, row: int):
+        if sql is None:
+            assert sql is not None
         sheet = sql.get_sheet(sheet_name)
         columns = sheet.columns
         res = [sheet.get_val(row, field) for field in columns]
         return res
 
     @staticmethod
     def assert_equal(expected, actual, context: str, delta=0.0):
@@ -120,14 +122,15 @@
     def assert_error_number(err_nb: int):
         msg = f"Line:{str(inspect.currentframe().f_lineno)}: Error[{err_nb}] is not the max[{PyxlSqlError.error_count}]"
         assert PyxlSqlError.error_count == err_nb, msg
 
     @staticmethod
     def assert_warning_start(warning_nb: int, start: str):
         msg = f"Line:{str(inspect.currentframe().f_lineno)}: Warning[{warning_nb}] not reached"
+
         assert PyxlSqlError.warning_count >= warning_nb, msg
         if PyxlSqlError.warning_count < warning_nb:
             return
         warning = PyxlSqlError.warning_list[warning_nb]
         msg = f"Line:{str(inspect.currentframe().f_lineno)}: Warning[{warning_nb}] '{warning[:40]}' != '{start[:40]}' "
         assert PyxlSqlError.warning_list[warning_nb].startswith(start), msg
```

