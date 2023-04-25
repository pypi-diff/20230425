# Comparing `tmp/SAPsim-1.0.0.tar.gz` & `tmp/SAPsim-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAPsim-1.0.0.tar", last modified: Sun Apr 23 03:30:44 2023, max compression
+gzip compressed data, was "SAPsim-1.0.1.tar", last modified: Tue Apr 25 11:20:59 2023, max compression
```

## Comparing `SAPsim-1.0.0.tar` & `SAPsim-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:30:44.286396 SAPsim-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-23 03:30:35.000000 SAPsim-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-23 03:30:44.286396 SAPsim-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-23 03:30:35.000000 SAPsim-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-23 03:30:35.000000 SAPsim-1.0.0/README_PyPI.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:30:44.282396 SAPsim-1.0.0/SAPsim/
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-04-23 03:30:35.000000 SAPsim-1.0.0/SAPsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:30:44.282396 SAPsim-1.0.0/SAPsim/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 03:30:35.000000 SAPsim-1.0.0/SAPsim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-04-23 03:30:35.000000 SAPsim-1.0.0/SAPsim/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-23 03:30:35.000000 SAPsim-1.0.0/SAPsim/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-23 03:30:35.000000 SAPsim-1.0.0/SAPsim/utils/globs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-04-23 03:30:35.000000 SAPsim-1.0.0/SAPsim/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-23 03:30:35.000000 SAPsim-1.0.0/SAPsim/utils/instructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-23 03:30:35.000000 SAPsim-1.0.0/SAPsim/utils/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:30:44.282396 SAPsim-1.0.0/SAPsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-23 03:30:44.000000 SAPsim-1.0.0/SAPsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-23 03:30:44.000000 SAPsim-1.0.0/SAPsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 03:30:44.000000 SAPsim-1.0.0/SAPsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 03:30:44.000000 SAPsim-1.0.0/SAPsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 03:30:44.000000 SAPsim-1.0.0/SAPsim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-23 03:30:35.000000 SAPsim-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 03:30:44.286396 SAPsim-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-23 03:30:35.000000 SAPsim-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 03:30:44.286396 SAPsim-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-23 03:30:35.000000 SAPsim-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-23 03:30:35.000000 SAPsim-1.0.0/tests/test_example_progs.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-23 03:30:35.000000 SAPsim-1.0.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-23 03:30:35.000000 SAPsim-1.0.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-04-23 03:30:35.000000 SAPsim-1.0.0/tests/test_instructions.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-25 11:20:59.517633 SAPsim-1.0.1/
+-rw-r--r--   0 jesse      (501) staff       (20)     1066 2023-02-23 19:54:52.000000 SAPsim-1.0.1/LICENSE
+-rw-r--r--   0 jesse      (501) staff       (20)     2621 2023-04-25 11:20:59.517478 SAPsim-1.0.1/PKG-INFO
+-rw-r--r--   0 jesse      (501) staff       (20)     1766 2023-04-25 11:20:34.000000 SAPsim-1.0.1/README.md
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-25 11:20:59.511919 SAPsim-1.0.1/SAPsim/
+-rw-r--r--   0 jesse      (501) staff       (20)      685 2023-04-25 11:20:18.000000 SAPsim-1.0.1/SAPsim/__init__.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-25 11:20:59.515590 SAPsim-1.0.1/SAPsim/utils/
+-rw-r--r--   0 jesse      (501) staff       (20)        0 2023-04-23 03:19:25.000000 SAPsim-1.0.1/SAPsim/utils/__init__.py
+-rw-r--r--   0 jesse      (501) staff       (20)     7470 2023-04-23 03:19:25.000000 SAPsim-1.0.1/SAPsim/utils/exceptions.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5593 2023-04-25 11:20:18.000000 SAPsim-1.0.1/SAPsim/utils/execute.py
+-rw-r--r--   0 jesse      (501) staff       (20)     2110 2023-04-23 03:19:25.000000 SAPsim-1.0.1/SAPsim/utils/globs.py
+-rw-r--r--   0 jesse      (501) staff       (20)     7692 2023-04-25 11:20:18.000000 SAPsim-1.0.1/SAPsim/utils/helpers.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5936 2023-04-23 03:19:25.000000 SAPsim-1.0.1/SAPsim/utils/instructions.py
+-rw-r--r--   0 jesse      (501) staff       (20)     3749 2023-04-25 11:20:18.000000 SAPsim-1.0.1/SAPsim/utils/parser.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-25 11:20:59.512779 SAPsim-1.0.1/SAPsim.egg-info/
+-rw-r--r--   0 jesse      (501) staff       (20)     2621 2023-04-25 11:20:59.000000 SAPsim-1.0.1/SAPsim.egg-info/PKG-INFO
+-rw-r--r--   0 jesse      (501) staff       (20)      521 2023-04-25 11:20:59.000000 SAPsim-1.0.1/SAPsim.egg-info/SOURCES.txt
+-rw-r--r--   0 jesse      (501) staff       (20)        1 2023-04-25 11:20:59.000000 SAPsim-1.0.1/SAPsim.egg-info/dependency_links.txt
+-rw-r--r--   0 jesse      (501) staff       (20)       20 2023-04-25 11:20:59.000000 SAPsim-1.0.1/SAPsim.egg-info/requires.txt
+-rw-r--r--   0 jesse      (501) staff       (20)       13 2023-04-25 11:20:59.000000 SAPsim-1.0.1/SAPsim.egg-info/top_level.txt
+-rw-r--r--   0 jesse      (501) staff       (20)      903 2023-04-25 11:20:18.000000 SAPsim-1.0.1/pyproject.toml
+-rw-r--r--   0 jesse      (501) staff       (20)       38 2023-04-25 11:20:59.517676 SAPsim-1.0.1/setup.cfg
+-rw-r--r--   0 jesse      (501) staff       (20)     1393 2023-04-25 11:20:18.000000 SAPsim-1.0.1/setup.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-25 11:20:59.517136 SAPsim-1.0.1/tests/
+-rw-r--r--   0 jesse      (501) staff       (20)      121 2023-02-23 20:02:21.000000 SAPsim-1.0.1/tests/__init__.py
+-rw-r--r--   0 jesse      (501) staff       (20)     3029 2023-04-23 03:19:25.000000 SAPsim-1.0.1/tests/test_example_progs.py
+-rw-r--r--   0 jesse      (501) staff       (20)      524 2023-04-23 03:19:25.000000 SAPsim-1.0.1/tests/test_exceptions.py
+-rw-r--r--   0 jesse      (501) staff       (20)     1389 2023-04-23 03:19:25.000000 SAPsim-1.0.1/tests/test_helpers.py
+-rw-r--r--   0 jesse      (501) staff       (20)     4765 2023-04-23 03:19:25.000000 SAPsim-1.0.1/tests/test_instructions.py
+-rw-r--r--   0 jesse      (501) staff       (20)     2620 2023-04-25 11:20:18.000000 SAPsim-1.0.1/tests/test_run.py
```

### Comparing `SAPsim-1.0.0/LICENSE` & `SAPsim-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.0/README.md` & `SAPsim-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # SAPsim
 
-> Simulation of [SAP (Simple As Possible) computer](https://jessewei.dev/img/sap.jpg) programs from COMP311 (Computer Organization) @ [UNC](https://unc.edu)
+![Test badge](https://github.com/jesse-wei/SAPsim/actions/workflows/test.yml/badge.svg)
+![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
+![Python](https://img.shields.io/badge/python-3670A0?style=plastic&logo=python&logoColor=ffdd54)
 
-![Tests](https://github.com/jesse-wei/SAPsim/actions/workflows/tests.yml/badge.svg)
+> Simulation of [SAP (Simple As Possible) computer](https://jessewei.dev/img/sap.jpg) programs from COMP311 (Computer Organization) @ [UNC](https://unc.edu)
 
 ## Install
 
 Your Python version needs to be 3.9+. Check with `python --version` or `python3 --version`, if `python` doesn't work.
 
 Next, install SAPsim.
 
@@ -14,29 +16,29 @@
 pip install SAPsim
 ```
 
 If `pip` doesn't work, try `pip3`.
 
 ## Usage
 
-Write a SAP program in the format shown in [`ex2.csv`](tests/public_prog/ex2.csv). See [`template.csv`](template.csv) for a blank template. You may edit the `.csv` files in Microsoft Excel.
+Write a SAP program in the format shown in [ex2.csv](https://github.com/jesse-wei/SAPsim/blob/main/tests/public_prog/ex2.csv). See [template.csv](https://github.com/jesse-wei/SAPsim/blob/main/template.csv) for a blank template. You may edit the `.csv` files in Microsoft Excel.
 
 Now, open a Python terminal or file. You'll pass the path to your SAP program as an argument.
 
 ```py
 from SAPsim import run
-run("path/to/your/SAP/program.csv")             # run at full speed (default)
-run("path/to/your/SAP/program.csv", debug=True) # run in debug (step) mode
+run("path/to/your/SAP/program.csv")                 # run at full speed (default)
+run("path/to/your/SAP/program.csv", debug=True)     # run in debug (step) mode
 ```
 
-For additional settings, see the [documentation](https://SAPsim.readthedocs.io/en/latest/#installation-and-usage).
+Additional settings are described [here](https://SAPsim.readthedocs.io/en/latest/#settings).
 
 ## Rules
 
-It's easiest to just copy the example programs [above](#how-to-program).
+It's easiest to just mimic the example programs [above](#usage).
 
 But if you need it, the list of rules for SAP programs is [here](https://SAPsim.readthedocs.io/en/latest/rules.html).
 
 ## SAP instruction set
 
 ![SAP instruction set](https://user-images.githubusercontent.com/55986131/220041985-da3060d2-18c3-4158-8d30-a5d88e08acc4.png)
```

### Comparing `SAPsim-1.0.0/SAPsim/__init__.py` & `SAPsim-1.0.1/SAPsim/utils/execute.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,124 +1,149 @@
+"""Execute instructions in RAM."""
+
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
 from pathlib import Path
 from typing import Any
-from SAPsim.utils.parser import parse_csv
-import SAPsim.utils.helpers as helpers
 import SAPsim.utils.globs as globs
-import SAPsim.utils.execute as execute
+import SAPsim.utils.instructions as instructions
+import SAPsim.utils.helpers as helpers
+from SAPsim.utils.helpers import is_documented_by
+import SAPsim.utils.exceptions as exceptions
+import SAPsim.utils.parser as parser
+
+
+def execute_full_speed() -> None:
+    """Execute instructions in ``RAM`` at full speed until ``EXECUTING`` is ``False`` or ``PC > max addr``."""
+    max_addr: int = 0
+    if globs.RAM.keys():
+        max_addr = max(globs.RAM.keys())
+    while globs.EXECUTING:
+        # Check that RAM is non-empty.
+        if globs.RAM.keys() and globs.PC > max_addr:
+            globs.EXECUTING = False
+            raise exceptions.DroppedOffBottom
+
+        # If we're executing an empty address but it's not a DroppedOffBottom, just skip and don't execute
+        if globs.PC not in globs.RAM:
+            globs.PC += 1
+            continue
+
+        instructions.OPCODE_TO_INSTR_PROCEDURE[
+            helpers.parse_opcode(globs.RAM[globs.PC])
+        ](helpers.parse_arg(globs.RAM[globs.PC]))
+
+
+def execute_next() -> None:
+    """Execute a single instruction at the current ``PC`` value if ``EXECUTING``. If attempting to execute an empty address, ``PC += 1`` (i.e., doesn't skip to next filled address)."""
+    if globs.EXECUTING:
+        if globs.RAM.keys() and globs.PC > max(globs.RAM.keys()):
+            globs.EXECUTING = False
+            raise exceptions.DroppedOffBottom
+
+        # If executing an empty address, just skip and don't execute
+        if globs.PC not in globs.RAM:
+            globs.PC += 1
+        else:
+            instructions.OPCODE_TO_INSTR_PROCEDURE[
+                helpers.parse_opcode(globs.RAM[globs.PC])
+            ](helpers.parse_arg(globs.RAM[globs.PC]))
 
 
 def run(prog_path: str, **kwargs) -> None:
-    r"""Run given .csv program.
+    r"""Run given .csv program in SAPsim format.
 
     :param prog_path:
         .csv file in SAPsim format.
     :type prog_path: ``str``
     :param \**kwargs:
         See below
 
     :Keyword Arguments:
         * *debug* (``bool``) --
             * Whether to run in debug mode (True) or at full speed (False)
             * Default is full speed
         * *change* (``str``) --
             * Comma-separated list of changes to RAM
+            * Format: <addr>:<base-10 value>,<addr>:<base-10 value>,...
+            * The value at each address will be overwritten to that base-10 value
             * Useful for debugging programs (edit a value without changing CSV)
             * Also useful for autograding programs (overwrite a reserved instruction/data value)
-            * Format: <addr>:<base-10 value>,<addr>:<base-10 value>, ...
-        * *format* (``str``) --
+        * *table_fmt* (``str``) --
             * Table format
             * Options: https://github.com/astanin/python-tabulate#table-format
+            * Default value is "simple_outline"
         * *bits* (``int``) --
             * Number of bits in unsigned registers
             * Default 8
-    :return: ``dict`` containing all final values in globs.py, used for autograding
-    :rtype: ``dict``
+    :return: ``None``
     """
     path: Path = Path(prog_path)
     assert path.suffix == ".csv"
     helpers.setup_8bit()
-    parse_csv(path)
+    parser.parse_csv(path)
     if "bits" in kwargs:
         assert int(kwargs["bits"]) > 1
         globs.NUM_BITS_IN_REGISTERS = int(kwargs["bits"])
         globs.MAX_UNSIGNED_VAL_IN_REGISTERS = 2**globs.NUM_BITS_IN_REGISTERS - 1
     if "change" in kwargs:
         changes = kwargs["change"].split(",")
         for change in changes:
             if change.count(":") != 1:
                 print(
                     "Invalid syntax for --c option, correct format is <addr>:<base-10 value>,<addr>:<base-10 value>, ..."
                 )
                 exit(1)
+            change = change.strip()
             colon_position = change.find(":")
             addr = int(change[:colon_position])
             if addr not in globs.RAM:
                 print(
                     f"You can apply a change only to an address that's already mapped (not skipped). Address {addr} is not mapped."
                 )
                 exit(1)
             value = int(change[colon_position + 1 :])
             if value < 0 or value > globs.MAX_UNSIGNED_VAL_IN_REGISTERS:
                 print(
                     f"Invalid base-10 value for change: {value}. Negative or overflows registers."
                 )
                 exit(1)
             globs.RAM[addr] = value
-    if "format" in kwargs:
-        globs.table_fmt = kwargs["format"]
+    if "table_fmt" in kwargs:
+        globs.table_fmt = kwargs["table_fmt"]
     if "debug" in kwargs and kwargs["debug"]:
-        print("Initial state of simulation.")
+        print(f"Initial state of simulation of {prog_path}")
         helpers.print_RAM(dispPC=True)
         helpers.print_info()
         print("Debug mode: press Enter to execute next instruction ( > ).")
         input()
         while globs.EXECUTING:
             # Special case so that you don't have to press Enter twice to halt on a HLT instruction
             if (
                 globs.PC in globs.RAM
                 and helpers.parse_opcode(globs.RAM[globs.PC]) == 0xF
             ):
-                execute.execute_next()
+                execute_next()
                 break
-            execute.execute_next()
+            execute_next()
             helpers.print_RAM(dispPC=True)
             helpers.print_info()
             input()
         print("Program halted.")
     else:
-        execute.execute_full_speed()
+        execute_full_speed()
         helpers.print_RAM(dispPC=True)
         helpers.print_info()
         print("Program halted.")
 
 
+@is_documented_by(
+    run,
+    2,
+    r"""
+    :return: ``dict`` containing program state (see ``helpers.get_state``)
+    :rtype: ``dict[str, Any]``
+    """,
+)
 def run_and_return_state(prog_path: str, **kwargs) -> dict[str, Any]:
-    r"""Run given .csv program and return final state. Just a wrapper around ``run()`` that can be used for autograding.
-
-    The rest of the docstring is identical to that of run().
-
-    :param prog_path:
-        .csv file in SAPsim format.
-    :type prog_path: ``str``
-    :param \**kwargs:
-        See below
-
-    :Keyword Arguments:
-        * *debug* (``bool``) --
-            * Whether to run in debug mode (True) or at full speed (False)
-        * *change* (``str``) --
-            * Comma-separated list of changes to RAM
-            * Useful for debugging programs (edit a value without changing CSV)
-            * Also useful for autograding programs (overwrite a reserved instruction/data value)
-            * Format: <addr>:<base-10 value>,<addr>:<base-10 value>, ...
-        * *format* (``str``) --
-            * Table format
-            * Options: https://github.com/astanin/python-tabulate#table-format
-        * *bits* (``int``) --
-            * Number of bits in unsigned registers
-    :return: ``dict`` containing all final values in globs.py, used for autograding
-    :rtype: ``dict``
-    """
     run(prog_path, **kwargs)
     return helpers.get_state()
```

### Comparing `SAPsim-1.0.0/SAPsim/utils/exceptions.py` & `SAPsim-1.0.1/SAPsim/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.0/SAPsim/utils/globs.py` & `SAPsim-1.0.1/SAPsim/utils/globs.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.0/SAPsim/utils/helpers.py` & `SAPsim-1.0.1/SAPsim/utils/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         table_row = []
         if "dispPC" in kwargs and kwargs["dispPC"]:
             table_row.append(">" if globs.PC == addr else "")
         table_row.extend([addr, instruction_str, byte, pad_hex(hex(byte), 2)])
         table.append(table_row)
     headers = []
     if "dispPC" in kwargs and kwargs["dispPC"]:
-        headers.append("")
+        headers.append("PC")
     headers.extend(["Addr", "Instruction", "Dec", "Hex"])
     print(tabulate(table, headers=headers, tablefmt=globs.table_fmt))
 
 
 def print_info(**kwargs):
     """Print the values of everything in global_vars.py except RAM. Set optional parameter ``bool=True`` to print flags as ``bool`` instead of ``int``. Set ``format=`` for tabulate pretty-print format."""
     table = [
@@ -204,7 +204,28 @@
         assert kwargs["B"] == globs.B
     if "FLAG_C" in kwargs:
         assert kwargs["FLAG_C"] == globs.FLAG_C
     if "FLAG_Z" in kwargs:
         assert kwargs["FLAG_Z"] == globs.FLAG_Z
     if "EXECUTING" in kwargs:
         assert kwargs["EXECUTING"] == globs.EXECUTING
+
+
+def is_documented_by(original, lines_to_remove: int = 0, append: str = ""):
+    r"""Use for wrapper functions that should have the original function's docstring.
+
+    :param original: The original function
+    :param lines_to_remove: How many lines to remove from the end of the docstring (i.e., to remove old return)
+    :type lines_to_remove: ``int``
+    :param append: What to append to docstring. Pass in a docstring (i.e., triple quotation marks), and there should be a leading newline
+    :type append: ``str``"""
+
+    def wrapper(target):
+        original_doc = original.__doc__.rstrip("\n")
+        target.__doc__ = "\n".join(original_doc.split("\n")[:-lines_to_remove])
+        # append_with_newline = append
+        # if append_with_newline and append_with_newline[0] != "\n":
+        #     append_with_newline = "\n" + append_with_newline
+        target.__doc__ += f"{append}"
+        return target
+
+    return wrapper
```

### Comparing `SAPsim-1.0.0/SAPsim/utils/instructions.py` & `SAPsim-1.0.1/SAPsim/utils/instructions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.0/SAPsim/utils/parser.py` & `SAPsim-1.0.1/SAPsim/utils/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Parses a SAP program in the CSV format given in ``template.csv`` into ``globs.RAM``."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
 from csv import DictReader
+from pathlib import Path
 import SAPsim.utils.exceptions as exceptions
 import SAPsim.utils.globs as globs
 
 
-def parse_csv(file_path):
+def parse_csv(file_path: Path):
     """Takes a ``.csv`` file path in ``template.csv`` format and parses it into ``RAM``."""
     prog = DictReader(open(file_path))
     num_rows = 1
     addresses = set()
 
     for row in prog:
         if not row["Address"]:
```

### Comparing `SAPsim-1.0.0/SAPsim.egg-info/SOURCES.txt` & `SAPsim-1.0.1/SAPsim.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENSE
 README.md
-README_PyPI.md
 pyproject.toml
 setup.py
 SAPsim/__init__.py
 SAPsim.egg-info/PKG-INFO
 SAPsim.egg-info/SOURCES.txt
 SAPsim.egg-info/dependency_links.txt
 SAPsim.egg-info/requires.txt
@@ -16,8 +15,9 @@
 SAPsim/utils/helpers.py
 SAPsim/utils/instructions.py
 SAPsim/utils/parser.py
 tests/__init__.py
 tests/test_example_progs.py
 tests/test_exceptions.py
 tests/test_helpers.py
-tests/test_instructions.py
+tests/test_instructions.py
+tests/test_run.py
```

### Comparing `SAPsim-1.0.0/pyproject.toml` & `SAPsim-1.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "SAPsim"
 authors = [
     { name="Jesse Wei", email="jesse@cs.unc.edu" },
 ]
 description = "Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC"
-readme = "README_PyPI.md"
+readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `SAPsim-1.0.0/setup.py` & `SAPsim-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 """All required (i.e., for functionality) dependencies that are installed when running `pip install SAPsim`.
 
 Non-functional (e.g., formatting, documentation) dependencies listed in requirements.txt."""
 
 setup(
     name="SAPsim",
     # Version number that appears on PyPI and Test PyPI
-    version="1.0.0",
+    version="1.0.1",
     description="Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC",
     author="Jesse Wei",
     author_email="jesse@cs.unc.edu",
-    url="https://github.com/jesse-wei/sapsim",
+    url="https://github.com/jesse-wei/SAPsim",
     download_url="https://github.com/jesse-wei/SAPsim/releases",
     keywords=[
         "SAP",
         "SAPsim",
         "simple as possible",
         "UNC",
         "COMP311",
```

### Comparing `SAPsim-1.0.0/tests/test_example_progs.py` & `SAPsim-1.0.1/tests/test_example_progs.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.0/tests/test_exceptions.py` & `SAPsim-1.0.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.0/tests/test_helpers.py` & `SAPsim-1.0.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.0/tests/test_instructions.py` & `SAPsim-1.0.1/tests/test_instructions.py`

 * *Files identical despite different names*

