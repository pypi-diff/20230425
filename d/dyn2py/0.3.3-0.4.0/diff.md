# Comparing `tmp/dyn2py-0.3.3.tar.gz` & `tmp/dyn2py-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyn2py-0.3.3.tar", last modified: Mon Mar 27 23:07:21 2023, max compression
+gzip compressed data, was "dyn2py-0.4.0.tar", last modified: Mon Apr 24 22:49:45 2023, max compression
```

## Comparing `dyn2py-0.3.3.tar` & `dyn2py-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:07:21.970013 dyn2py-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-27 23:07:09.000000 dyn2py-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    48020 2023-03-27 23:07:21.970013 dyn2py-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-03-27 23:07:09.000000 dyn2py-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:07:21.970013 dyn2py-0.3.3/dyn2py/
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-03-27 23:07:09.000000 dyn2py-0.3.3/dyn2py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-27 23:07:09.000000 dyn2py-0.3.3/dyn2py/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-27 23:07:09.000000 dyn2py-0.3.3/dyn2py/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22285 2023-03-27 23:07:09.000000 dyn2py-0.3.3/dyn2py/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-03-27 23:07:09.000000 dyn2py-0.3.3/dyn2py/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:07:21.970013 dyn2py-0.3.3/dyn2py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    48020 2023-03-27 23:07:21.000000 dyn2py-0.3.3/dyn2py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-27 23:07:21.000000 dyn2py-0.3.3/dyn2py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 23:07:21.000000 dyn2py-0.3.3/dyn2py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-27 23:07:21.000000 dyn2py-0.3.3/dyn2py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-27 23:07:21.000000 dyn2py-0.3.3/dyn2py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-27 23:07:21.000000 dyn2py-0.3.3/dyn2py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-27 23:07:09.000000 dyn2py-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 23:07:21.970013 dyn2py-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:07:21.970013 dyn2py-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-03-27 23:07:09.000000 dyn2py-0.3.3/tests/test_CommandLine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-03-27 23:07:09.000000 dyn2py-0.3.3/tests/test_DynamoFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-03-27 23:07:09.000000 dyn2py-0.3.3/tests/test_File.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-03-27 23:07:09.000000 dyn2py-0.3.3/tests/test_PythonFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-03-27 23:07:09.000000 dyn2py-0.3.3/tests/test_PythonNode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:49:45.209891 dyn2py-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 22:49:34.000000 dyn2py-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    48731 2023-04-24 22:49:45.209891 dyn2py-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-04-24 22:49:34.000000 dyn2py-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:49:45.205891 dyn2py-0.4.0/dyn2py/
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-04-24 22:49:34.000000 dyn2py-0.4.0/dyn2py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-24 22:49:34.000000 dyn2py-0.4.0/dyn2py/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26475 2023-04-24 22:49:34.000000 dyn2py-0.4.0/dyn2py/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-24 22:49:34.000000 dyn2py-0.4.0/dyn2py/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:49:45.209891 dyn2py-0.4.0/dyn2py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    48731 2023-04-24 22:49:45.000000 dyn2py-0.4.0/dyn2py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-24 22:49:45.000000 dyn2py-0.4.0/dyn2py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 22:49:45.000000 dyn2py-0.4.0/dyn2py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 22:49:45.000000 dyn2py-0.4.0/dyn2py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-24 22:49:45.000000 dyn2py-0.4.0/dyn2py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 22:49:45.000000 dyn2py-0.4.0/dyn2py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-24 22:49:34.000000 dyn2py-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 22:49:45.209891 dyn2py-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:49:45.209891 dyn2py-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-04-24 22:49:34.000000 dyn2py-0.4.0/tests/test_CommandLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-24 22:49:34.000000 dyn2py-0.4.0/tests/test_DynamoFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-24 22:49:34.000000 dyn2py-0.4.0/tests/test_File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-24 22:49:34.000000 dyn2py-0.4.0/tests/test_PythonFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-24 22:49:34.000000 dyn2py-0.4.0/tests/test_PythonNode.py
```

### Comparing `dyn2py-0.3.3/LICENSE` & `dyn2py-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dyn2py-0.3.3/PKG-INFO` & `dyn2py-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyn2py
-Version: 0.3.3
+Version: 0.4.0
 Summary: Extract python code from Dynamo graphs
 Author-email: infeeeee <gyetpet@mailbox.org>
 Maintainer-email: infeeeee <gyetpet@mailbox.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -743,91 +743,112 @@
 positional arguments:
   source                path to a Dynamo graph, a python script or a folder containing them
 
 options:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
   -l LOGLEVEL, --loglevel LOGLEVEL
-                        set log level, possible options: CRITICAL, ERROR, WARNING, INFO, DEBUG
+                        set log level, possible options: HEADLESS, CRITICAL, ERROR, WARNING, INFO, DEBUG
   -n, --dry-run         do not modify files, only show log
   -F, --force           overwrite even if the files are older
   -b, --backup          create a backup for updated files
   -f {py,dyn}, --filter {py,dyn}
                         only check python or Dynamo graphs, skip the others, useful for folders
 
 dynamo options, only for processing Dynamo graphs:
   -u, --update          update Dynamo graph from python scripts in the same folder
   -p path/to/folder, --python-folder path/to/folder
                         extract python scripts to this folder, read python scripts from here with --update
 
 The script by default overwrites older files with newer files.
 Do not move the source Dynamo graphs, or update won't work with them later.
 Multiple sources are supported, separate them by spaces.
+HEADLESS loglevel only prints modified filenames.
 ```
 
 #### Examples
 
 *Notes: In Windows cmd use backward slashes as path separators, in any other shells use forward slashes. Powershell accepts both of them. Wrap paths with spaces in double quotes.*
 
-Extract all nodes next to a Dynamo file:
-
-```
+```shell
+# Extract all nodes next to a Dynamo file:
 dyn2py path/to/dynamofile.dyn
-```
-
-Update a Dynamo file from previously exported and modified python files:
 
-```
+# Update a Dynamo file from previously exported and modified python files:
 dyn2py --update path/to/dynamofile.dyn
-```
 
-Extract python nodes to a specific folder, process multiple Dynamo files:
-
-```
+# Extract python nodes to a specific folder, process multiple Dynamo files:
 dyn2py --python-folder path/to/pythonfiles path/to/dynamofile1.dyn path/to/dynamofile2.dyn
-```
-
-Update Dynamo files from python files from a folder. Only check python files, create backups:
 
-```
+# Update Dynamo files from python files from a folder. Only check python files, create backups:
 dyn2py --filter py --backup path/to/pythonfiles
 ```
 
+#### Git hooks
+
+Git hooks are a built-in feature of Git that allow developers to automate tasks throughout the Git workflow. Read more here: https://githooks.com/
+
+With the `pre-commit` hook it's possible to add more files to the currently initialized commit.
+
+You can find an example pre-commit hook here: [pre-commit](pre-commit). Copy this file to the `.git/hooks` folder of your repo of Dynamo graphs. This folder is hidden by default, but it should exist in all initialized git repo. Do not rename this file.
+
+This script will go through staged `.dyn` files and export python scripts from them, and add them to the current commit. Now you can check changed lines in a diff tool, you can see changed python code in a PR!
+
 ### As a python module
 
 Full API documentation available here: https://infeeeee.github.io/dyn2py
 
-Most basic example to extract all nodes next to a Dynamo file:
+#### Examples
+
+Extract all nodes from python nodes next to a Dynamo file:
 
 ```python
 import dyn2py
 
+# Open a Dynamo graph:
 dynamo_file = dyn2py.DynamoFile("path/to/dynamofile.dyn")
-python_files = dynamo_file.extract_python()
-[python_file.write() for python_file in python_files]
+
+# Extract python nodes:
+dynamo_file.extract_python()
+
+# Save all python nodes as separate files:
+dyn2py.PythonFile.write_open_files()
 ```
 
-Change options like with the command line switches with the `Options` class:
+Update python node from a python file:
 
 ```python
 import dyn2py
 
-# Create a backup on overwrite, read python files from a different folder:
-options = dyn2py.Options(
-    backup=True,
-    python_folder="path/to/pythonfiles")
+# Open a python file:
+python_file = dyn2py.PythonFile("path/to/pythonfile.py")
+
+# Update the node in the graph:
+python_file.update_dynamo()
+
+# Save modified Dynamo graph:
+dyn2py.DynamoFile.write_open_files()
+```
 
+Update all python nodes of a Dynamo grapg from a different folder, save backups:
+
+```python
+import dyn2py
+
+# open a Dynamo graph:
 dynamo_file = dyn2py.DynamoFile("path/to/dynamofile.dyn")
-python_files = dynamo_file.get_related_python_files(options)
+
+# Get python files from a dofferent folder:
+python_files = dynamo_file.get_related_python_files(python_folder="path/to/pythonfiles")
 
 # Read python files and update the graph:
-[python_file.update_dynamo(options) for python_file in python_files]
+[python_file.update_dynamo() for python_file in python_files]
 
-# Don't forget to save at the end:
-dynamo_file.write(options)
+# Save open Dynamo graphs:
+dyn2py.DynamoFile.write_open_files(backup=True)
 ```
 
 For more examples check tests in the [tests folder on Github](https://github.com/infeeeee/dyn2py/tree/main/tests)
 
 They should work in Dynamo, inside CPython3 nodes.
 
 ## Troubleshooting
@@ -838,14 +859,16 @@
 
 ## Limitations
 
 Only supports Dynamo 2 files, Dynamo 1 files are reported and ignored. Please update them to Dynamo 2 by opening them in Dynamo 2.
 
 Both IronPython2 and CPython3 nodes are supported! IronPython2 nodes won't be updated to CPython3, they will be imported as-is.
 
+Cannot create new python nodes, only existing ones can be updated.
+
 ## Development
 
 ### Installation
 
 Requirements: git, python, pip
 
 ```
@@ -855,40 +878,32 @@
 ```
 
 With venv:
 
 ```
 git clone https://github.com/infeeeee/dyn2py
 cd dyn2py
-venv .venv
+python -m venv .venv
 . ./.venv/bin/activate
 pip install -e .
 ```
 
 ### Build for Windows
 
 ```
 pip install -e .[build]
 pyinstaller dyn2py.spec
 ```
 
 ### Create installer for Windows
 
 - Install Inno Setup: https://jrsoftware.org/isdl.php
-- The already built exe should be in the root folder
-- Run this in powershell:
+- Build an exe
+- Run `dyn2py-installer.ps1` in powershell
 
-```powershell
-# Read version number from pyproject.toml and update in innosetup:
-$regex = Select-String -Path pyproject.toml -Pattern '^version = "((?:\d\.){2}\d)"$'
-$version = $regex.Matches.Groups[1].Value
-(Get-Content dyn2py-installer.iss).Replace("x.x.x",$version) | Set-Content dyn2py-installer.iss
-# Build:
-& "C:\Program Files (x86)\Inno Setup 6\ISCC.exe" -Qp $(Join-Path $PWD.Path dyn2py-installer.iss)
-```
 ### Live module documentation
 
 ```
 pip install -e .[doc]
 pdoc -d google dyn2py
 ```
 
@@ -901,13 +916,13 @@
 ```
 python -m unittest discover -v -s ./tests -p "test_*.py"
 ```
 
 ### New release
 
 1. Update version number in `pyproject.toml`
-2. Create a publish a git tag with that number
+2. Create and publish a git tag with that number
 
 ## License
 
 GPL-3.0
```

### Comparing `dyn2py-0.3.3/README.md` & `dyn2py-0.4.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -49,91 +49,112 @@
 positional arguments:
   source                path to a Dynamo graph, a python script or a folder containing them
 
 options:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
   -l LOGLEVEL, --loglevel LOGLEVEL
-                        set log level, possible options: CRITICAL, ERROR, WARNING, INFO, DEBUG
+                        set log level, possible options: HEADLESS, CRITICAL, ERROR, WARNING, INFO, DEBUG
   -n, --dry-run         do not modify files, only show log
   -F, --force           overwrite even if the files are older
   -b, --backup          create a backup for updated files
   -f {py,dyn}, --filter {py,dyn}
                         only check python or Dynamo graphs, skip the others, useful for folders
 
 dynamo options, only for processing Dynamo graphs:
   -u, --update          update Dynamo graph from python scripts in the same folder
   -p path/to/folder, --python-folder path/to/folder
                         extract python scripts to this folder, read python scripts from here with --update
 
 The script by default overwrites older files with newer files.
 Do not move the source Dynamo graphs, or update won't work with them later.
 Multiple sources are supported, separate them by spaces.
+HEADLESS loglevel only prints modified filenames.
 ```
 
 #### Examples
 
 *Notes: In Windows cmd use backward slashes as path separators, in any other shells use forward slashes. Powershell accepts both of them. Wrap paths with spaces in double quotes.*
 
-Extract all nodes next to a Dynamo file:
-
-```
+```shell
+# Extract all nodes next to a Dynamo file:
 dyn2py path/to/dynamofile.dyn
-```
-
-Update a Dynamo file from previously exported and modified python files:
 
-```
+# Update a Dynamo file from previously exported and modified python files:
 dyn2py --update path/to/dynamofile.dyn
-```
 
-Extract python nodes to a specific folder, process multiple Dynamo files:
-
-```
+# Extract python nodes to a specific folder, process multiple Dynamo files:
 dyn2py --python-folder path/to/pythonfiles path/to/dynamofile1.dyn path/to/dynamofile2.dyn
-```
-
-Update Dynamo files from python files from a folder. Only check python files, create backups:
 
-```
+# Update Dynamo files from python files from a folder. Only check python files, create backups:
 dyn2py --filter py --backup path/to/pythonfiles
 ```
 
+#### Git hooks
+
+Git hooks are a built-in feature of Git that allow developers to automate tasks throughout the Git workflow. Read more here: https://githooks.com/
+
+With the `pre-commit` hook it's possible to add more files to the currently initialized commit.
+
+You can find an example pre-commit hook here: [pre-commit](pre-commit). Copy this file to the `.git/hooks` folder of your repo of Dynamo graphs. This folder is hidden by default, but it should exist in all initialized git repo. Do not rename this file.
+
+This script will go through staged `.dyn` files and export python scripts from them, and add them to the current commit. Now you can check changed lines in a diff tool, you can see changed python code in a PR!
+
 ### As a python module
 
 Full API documentation available here: https://infeeeee.github.io/dyn2py
 
-Most basic example to extract all nodes next to a Dynamo file:
+#### Examples
+
+Extract all nodes from python nodes next to a Dynamo file:
 
 ```python
 import dyn2py
 
+# Open a Dynamo graph:
 dynamo_file = dyn2py.DynamoFile("path/to/dynamofile.dyn")
-python_files = dynamo_file.extract_python()
-[python_file.write() for python_file in python_files]
+
+# Extract python nodes:
+dynamo_file.extract_python()
+
+# Save all python nodes as separate files:
+dyn2py.PythonFile.write_open_files()
 ```
 
-Change options like with the command line switches with the `Options` class:
+Update python node from a python file:
 
 ```python
 import dyn2py
 
-# Create a backup on overwrite, read python files from a different folder:
-options = dyn2py.Options(
-    backup=True,
-    python_folder="path/to/pythonfiles")
+# Open a python file:
+python_file = dyn2py.PythonFile("path/to/pythonfile.py")
+
+# Update the node in the graph:
+python_file.update_dynamo()
+
+# Save modified Dynamo graph:
+dyn2py.DynamoFile.write_open_files()
+```
 
+Update all python nodes of a Dynamo grapg from a different folder, save backups:
+
+```python
+import dyn2py
+
+# open a Dynamo graph:
 dynamo_file = dyn2py.DynamoFile("path/to/dynamofile.dyn")
-python_files = dynamo_file.get_related_python_files(options)
+
+# Get python files from a dofferent folder:
+python_files = dynamo_file.get_related_python_files(python_folder="path/to/pythonfiles")
 
 # Read python files and update the graph:
-[python_file.update_dynamo(options) for python_file in python_files]
+[python_file.update_dynamo() for python_file in python_files]
 
-# Don't forget to save at the end:
-dynamo_file.write(options)
+# Save open Dynamo graphs:
+dyn2py.DynamoFile.write_open_files(backup=True)
 ```
 
 For more examples check tests in the [tests folder on Github](https://github.com/infeeeee/dyn2py/tree/main/tests)
 
 They should work in Dynamo, inside CPython3 nodes.
 
 ## Troubleshooting
@@ -144,14 +165,16 @@
 
 ## Limitations
 
 Only supports Dynamo 2 files, Dynamo 1 files are reported and ignored. Please update them to Dynamo 2 by opening them in Dynamo 2.
 
 Both IronPython2 and CPython3 nodes are supported! IronPython2 nodes won't be updated to CPython3, they will be imported as-is.
 
+Cannot create new python nodes, only existing ones can be updated.
+
 ## Development
 
 ### Installation
 
 Requirements: git, python, pip
 
 ```
@@ -161,40 +184,32 @@
 ```
 
 With venv:
 
 ```
 git clone https://github.com/infeeeee/dyn2py
 cd dyn2py
-venv .venv
+python -m venv .venv
 . ./.venv/bin/activate
 pip install -e .
 ```
 
 ### Build for Windows
 
 ```
 pip install -e .[build]
 pyinstaller dyn2py.spec
 ```
 
 ### Create installer for Windows
 
 - Install Inno Setup: https://jrsoftware.org/isdl.php
-- The already built exe should be in the root folder
-- Run this in powershell:
+- Build an exe
+- Run `dyn2py-installer.ps1` in powershell
 
-```powershell
-# Read version number from pyproject.toml and update in innosetup:
-$regex = Select-String -Path pyproject.toml -Pattern '^version = "((?:\d\.){2}\d)"$'
-$version = $regex.Matches.Groups[1].Value
-(Get-Content dyn2py-installer.iss).Replace("x.x.x",$version) | Set-Content dyn2py-installer.iss
-# Build:
-& "C:\Program Files (x86)\Inno Setup 6\ISCC.exe" -Qp $(Join-Path $PWD.Path dyn2py-installer.iss)
-```
 ### Live module documentation
 
 ```
 pip install -e .[doc]
 pdoc -d google dyn2py
 ```
 
@@ -207,13 +222,13 @@
 ```
 python -m unittest discover -v -s ./tests -p "test_*.py"
 ```
 
 ### New release
 
 1. Update version number in `pyproject.toml`
-2. Create a publish a git tag with that number
+2. Create and publish a git tag with that number
 
 ## License
 
 GPL-3.0
```

### Comparing `dyn2py-0.3.3/dyn2py/__init__.py` & `dyn2py-0.4.0/dyn2py/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,19 +18,15 @@
 __version__ = METADATA["Version"]
 __all__ = [
     "run",
     "Options",
     "File",
     "DynamoFile",
     "PythonFile",
-    "PythonNode",
-    "DynamoFileException",
-    "PythonNodeNotFoundException",
-    "PythonNodeException",
-    "PythonFileException"
+    "PythonNode"
 ]
 
 
 def __dir__():
     return __all__
 
 
@@ -41,14 +37,15 @@
         prog=METADATA["Name"],
         description=METADATA["Summary"],
         formatter_class=argparse.RawDescriptionHelpFormatter,
         epilog=textwrap.dedent("""\
             The script by default overwrites older files with newer files.
             Do not move the source Dynamo graphs, or update won't work with them later.
             Multiple sources are supported, separate them by spaces.
+            HEADLESS loglevel only prints modified filenames.
             """)
     )
 
     parser.add_argument("-v", "--version",
                         action="version",
                         version=f'{METADATA["Name"]} {METADATA["Version"]}'
                         )
@@ -113,16 +110,21 @@
 
     if not isinstance(options, Options):
         raise TypeError("Options have to be a dyn2py.Options() object!")
 
     from_command_line = bool(inspect.stack()[1].function == "__command_line")
 
     # Set up logging:
+    if options.loglevel == "HEADLESS":
+        loglevel = "CRITICAL"
+    else:
+        loglevel = options.loglevel
+
     logging.basicConfig(format='%(levelname)s: %(message)s',
-                        level=options.loglevel)
+                        level=loglevel)
     logging.debug(f"Run options: {vars(options)}")
 
     # Set up sources:
     source_files = []
     for source in options.source:
 
         if not source.exists():
@@ -145,21 +147,21 @@
             source_files.append(source)
 
     # Create file objects
     files = []
     for f in source_files:
         try:
             files.append(File(f))
-        except DynamoFileException as e:
+        except DynamoFile.Error as e:
             # It's a dynamo1 file
-            logging.warning(e)
+            logging.warning(f"This is a Dynamo 1 file! {e.file.filepath}")
             continue
-        except PythonNodeNotFoundException as e:
-            # No python node in this file
-            logging.warning(e)
+        except DynamoFile.PythonNodeNotFound as e:
+            # No python nodes in this file
+            logging.warning(f"This file has no Python nodes! {e.file.filepath} ")
             continue
 
     # Dynamo files come first, sort sources:
     files.sort(key=lambda f: f.extension)
 
     # Filters:
     if options.filter == "py":
@@ -189,12 +191,17 @@
 
         if f.is_dynamo_file():
             logging.debug("Source is a Dynamo file")
             f.extract_python(options)
 
         elif f.is_python_file():
             logging.debug("Source is a Python file")
-            f.update_dynamo(options)
+            try:
+                f.update_dynamo(options)
+            except FileNotFoundError:
+                logging.error(f"{f.filepath} Source Dynamo file not found! ")
 
     # Write files at the end:
-    for f in DynamoFile.open_files | PythonFile.open_files:
-        f.write(options)
+    try:
+        File.write_open_files(options)
+    except File.Error as e:
+        logging.error(f"Cannot save file! {e.file.filepath}")
```

### Comparing `dyn2py-0.3.3/dyn2py/files.py` & `dyn2py-0.4.0/dyn2py/files.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 import logging
 import os
 from datetime import datetime
 from decimal import Decimal
 from pathvalidate import sanitize_filename
 from importlib_metadata import metadata
 
-from dyn2py.exceptions import *
 from dyn2py.options import Options
 
 
 METADATA = metadata("dyn2py")
 HEADER_SEPARATOR = "*" * 60
 
 
 class File():
     """Base class for managing files"""
 
+    open_files: set[File] = set()
+    """A set of open files."""
+
     def __init__(self, filepath: pathlib.Path | str, read_from_disk: bool = True) -> None:
         """Generate a file object. If the path is correct it will become a DynamoFile or PythonFile object.
             Calls DynamoFile.read_file() and PythonFile.read_file()
 
         Args:
             filepath (pathlib.Path | str): Path to the python file or Dynamo graph
             read_from_disk (bool, optional): Read the file from disk. False to get only metadata. Defaults to True.
@@ -106,90 +108,153 @@
         """Check if this is a python file
 
         Returns:
             bool: True if it's python file
         """
         return bool(self.extension == ".py")
 
-    def write(self, options: Options | None = None) -> None:
+    def write(self, options: Options | None = None, **option_args) -> None:
         """Prepare writing file to the disk:
             create backup, process dry-run, call filetype specific write_file() methods
             Should be called on subclasses!
 
         Args:
             options (Options | None, optional): Run options. Defaults to None.
+            **option_args: Options() arguments
 
         Raises:
+            ValueError: Both options and other arguments given
             TypeError: If called on a File object
+            File.Error: Target folder does not exist
         """
 
         if not options:
-            options = Options()
+            options = Options.from_kwargs(kwargs=option_args)
+        elif option_args:
+            # Should not give both options and arguments:
+            raise ValueError("Options object and extra arguments!")
 
         # This should only work on subclasses:
         if type(self).__name__ == "File":
             raise TypeError("This method shouldn't be called on File objects!")
 
         if not self.modified:
             logging.debug("File not modified, not saving")
             return
 
         # Create backup:
         if not options.dry_run and self.filepath.exists() and options.backup:
             backup_filename = sanitize_filename(
-                f"{self.basename}_{self.mtimeiso}{self.extension}")
+                filename=f"{self.basename}_{self.mtimeiso}{self.extension}")
             backup_path = self.dirpath.joinpath(backup_filename)
             logging.info(f"Creating backup to {backup_path}")
             self.filepath.rename(backup_path)
+            if options.loglevel == "HEADLESS":
+                print(backup_path)
 
         # Call filetype specific methods:
         if options.dry_run:
             logging.info(
                 f"Should write file, but it's a dry-run: {self.filepath}")
         else:
+            if not self.dirpath.exists():
+                raise File.Error("File dir does not exist!", self)
             logging.info(f"Writing file: {self.filepath}")
             self._write_file()
+            if options.loglevel == "HEADLESS":
+                print(self.filepath)
 
     def _write_file(self):
         """Should be implemented in subclasses
 
         Raises:
             NotImplementedError: If called on a File object
         """
         raise NotImplementedError(
             "Should be called only on DynamoFile and PythonFile objects!")
 
+    @classmethod
+    def get_open_files(cls) -> set:
+        """Get open files of this class and subclasses
+
+        Returns:
+            set: A set of open files
+        """
+        return {f for f in File.open_files if
+                isinstance(f, cls)}
+
+    @classmethod
+    def write_open_files(cls, options: Options | None = None, **option_args) -> None:
+        """Write open files of this class and subclasses
+
+        Args:
+            options (Options | None, optional): Run options. Defaults to None.
+            **option_args: Options() arguments
+
+        Raises:
+            ValueError: Both options and other arguments given
+
+        """
+        if not options:
+            options = Options.from_kwargs(kwargs=option_args)
+        elif option_args:
+            # Should not give both options and arguments:
+            raise ValueError("Options object and extra arguments!")
+
+        for f in cls.get_open_files():
+            f.write(options)
+
+    @classmethod
+    def close_open_files(cls) -> None:
+        """Close open files of this class and subclasses"""
+        File.open_files = File.open_files - cls.get_open_files()
+
+    class Error(Exception):
+        def __init__(self, message: str, file: File) -> None:
+            """There is some problem with this file
+
+            Args:
+                message (str): The message to display
+                file (File): The problem File
+            """
+            super().__init__(message)
+            self.file = file
+
 
 class DynamoFile(File):
     """A Dynamo file, subclass of File()"""
 
     full_dict: dict
     """The contents of the Dynamo file, as dict."""
     uuid: str
     """The uuid of the graph."""
     name: str
     """The name of the graph, read from the file, not the filename"""
     python_nodes: set[PythonNode]
     """Python node objects, read from this file."""
 
-    open_files: set[DynamoFile] = set()
-    """A set of open Dynamo files, before saving. Self added by read()"""
-
-    def extract_python(self, options: Options | None = None) -> list[PythonFile]:
+    def extract_python(self, options: Options | None = None, **option_args) -> list[PythonFile]:
         """Extract python files from Dynamo graphs, add them to open_files
 
         Args:
             options (Options | None, optional): Run options. Defaults to None.
+            **option_args: Options() arguments
+
+        Raises:
+            ValueError: Both options and other arguments given
 
         Returns:
             list[PythonFile]: List of PythonFile objects extracted from this DynamoFile
         """
 
         if not options:
-            options = Options()
+            options = Options.from_kwargs(kwargs=option_args)
+        elif option_args:
+            # Should not give both options and arguments:
+            raise ValueError("Options object and extra arguments!")
 
         logging.info(f"Extracting from file: {self.filepath}")
         python_files = []
 
         # Go through nodes in the file:
         for python_node in self.python_nodes:
             if options.python_folder:
@@ -218,17 +283,17 @@
         """Read Dynamo graph to parameters. Automatically called by __init__()
 
         Args:
             reread (bool, optional): Reread the file, even if it was read already. Defaults to False.
 
         Raises:
             FileNotFoundError: The file does not exist
-            DynamoFileException: If the file is a Dynamo 1 file
+            DynamoFile.Error: If the file is a Dynamo 1 file
             json.JSONDecodeError: If there are any other problem with the file
-            PythonNodeNotFoundException: No python nodes in the file
+            DynamoFile.PythonNodeNotFound: No python nodes in the file
         """
 
         if not self.exists:
             raise FileNotFoundError
 
         if not self in self.open_files or reread:
 
@@ -238,31 +303,31 @@
                 with open(self.filepath, "r", encoding="utf-8") as input_json:
                     self.full_dict = json.load(input_json,
                                                use_decimal=True)
 
             except json.JSONDecodeError as e:
                 with open(self.filepath, "r", encoding="utf-8") as input_json:
                     if input_json.readline().startswith("<Workspace Version="):
-                        raise DynamoFileException("This is a Dynamo 1 file!")
+                        raise self.Error("This is a Dynamo 1 file!", self)
                     else:
                         raise e
 
             # Parameters:
             self.uuid = self.full_dict["Uuid"]
             self.name = self.full_dict["Name"]
             self.open_files.add(self)
 
             full_python_nodes = [n for n in self.full_dict["Nodes"]
                                  if n["NodeType"] == "PythonScriptNode"]
             # The name of the node is stored here:
             node_views = self.full_dict["View"]["NodeViews"]
 
             if not full_python_nodes:
-                raise PythonNodeNotFoundException(
-                    "No python nodes in this file!")
+                raise self.PythonNodeNotFound(
+                    "No python nodes in this file!", self, "")
 
             self.python_nodes = set()
 
             # Create PythonNodes from the dict:
             for p_node in full_python_nodes:
                 python_node = PythonNode(
                     node_dict_from_dyn=p_node,
@@ -275,46 +340,47 @@
         Args:
             node_id (str): The id of the python node as string
 
         Returns:
             PythonNode: The PythonNode with the given id
 
         Raises:
-            PythonNodeNotFoundException: No python node with this id
+            DynamoFile.PythonNodeNotFound: No python node with this id
         """
 
         python_node = next((
             p for p in self.python_nodes if p.id == node_id
         ), None)
 
         if not python_node:
-            raise PythonNodeNotFoundException(
-                f"Node not found with id {node_id}")
+            raise self.PythonNodeNotFound(
+                "Node not found", self, node_id)
 
         return python_node
 
     def update_python_node(self, python_node: PythonNode) -> None:
         """Update the code of a PythonNode in this file
 
         Args:
             python_node (PythonNode): The new node
 
         Raises:
-            PythonNodeNotFoundException: Existing node not found
+            DynamoFile.PythonNodeNotFound: Existing node not found
         """
 
         # Find the old node:
         python_node_in_file = self.get_python_node_by_id(python_node.id)
 
         node_dict = next((
             n for n in self.full_dict["Nodes"] if n["Id"] == python_node.id
         ), {})
 
-        if not node_dict or not python_node_in_file:
-            raise PythonNodeNotFoundException()
+        if not node_dict:
+            raise self.PythonNodeNotFound(
+                "Existing node not found in file", self, python_node.id)
 
         # Remove the old and add the new:
         self.python_nodes.remove(python_node_in_file)
         self.python_nodes.add(python_node)
 
         # Update the dict, Dyn files are always CRLF:
         node_dict["Code"] = "\r\n".join(python_node.code)
@@ -322,25 +388,32 @@
         self.modified = True
 
     def _write_file(self) -> None:
         """Write this file to the disk. Should be called only from File.write()"""
         with open(self.filepath, "w", encoding="utf-8", newline="") as output_file:
             json.dump(self.full_dict, output_file, indent=2,  use_decimal=True)
 
-    def get_related_python_files(self, options: Options | None = None) -> list[PythonFile]:
+    def get_related_python_files(self, options: Options | None = None, **option_args) -> list[PythonFile]:
         """Get python files exported from this Dynamo file
 
         Args:
             options (Options | None, optional): Run options. Defaults to None.
+            **option_args: Options() arguments
+
+        Raises:
+            ValueError: Both options and other arguments given
 
         Returns:
             list[PythonFile]: A list of PythonFile objects
         """
         if not options:
-            options = Options()
+            options = Options.from_kwargs(kwargs=option_args)
+        elif option_args:
+            # Should not give both options and arguments:
+            raise ValueError("Options object and extra arguments!")
 
         # Find the folder of the python files
         if options.python_folder:
             python_folder = options.python_folder
         else:
             python_folder = self.dirpath
 
@@ -357,33 +430,43 @@
         """Get an open Dynamo graph by its uuid
 
         Args:
             uuid (str): Uuid of the file
         Returns:
             DynamoFile: The file. None if not found
         """
-        f = next((d for d in DynamoFile.open_files if d.uuid == uuid), None)
+        f = next((d for d in DynamoFile.get_open_files() if d.uuid == uuid), None)
         if f:
             logging.debug(f"Found open file {f.uuid}")
         return f
 
+    class PythonNodeNotFound(Exception):
+        def __init__(self, message: str, file: DynamoFile, node_id: str) -> None:
+            """Python node not found with this id
+
+            Args:
+                message (str): The message to display
+                file (DynamoFile): The problem DynamoFile
+                node_id (str): The missing id
+            """
+            super().__init__(message)
+            self.file = file
+            self.node_id = node_id
+
 
 class PythonFile(File):
     """A Python file, subclass of File()"""
 
     code: list[str]
     """The python code. Lines as list items, without newlines."""
     header_data: dict
     """Parsed dict from the header of a python file."""
     text: str
     """Full contents of the file."""
 
-    open_files: set[PythonFile] = set()
-    """A set of open Python files."""
-
     def __init__(self,
                  filepath: pathlib.Path | str,
                  dynamo_file: DynamoFile | None = None,
                  python_node: PythonNode | None = None
                  ) -> None:
         """Generate a PythonFile. If both dynamo_file and python_node given, generate the text of the file, do not read from disk
 
@@ -399,18 +482,19 @@
             super().__init__(filepath, read_from_disk=False)
 
             header_notice = os.linesep.join([
                 "This file was generated with dyn2py from a Dynamo graph.",
                 "Do not edit this section, if you want to update the Dynamo graph!"
             ])
 
-            # Double escape path:
-            dyn_path_string = str(dynamo_file.realpath)
+            # Calculate relative path, change to forward slash
+            dyn_path_string = os.path.relpath(
+                dynamo_file.filepath, self.dirpath)
             if "\\" in dyn_path_string:
-                dyn_path_string = dyn_path_string.replace("\\", "\\\\")
+                dyn_path_string = dyn_path_string.replace("\\", "/")
 
             self.header_data = {
                 "dyn2py_version": METADATA["Version"],
                 "dyn2py_extracted": datetime.now().isoformat(),
                 "dyn_uuid": dynamo_file.uuid,
                 "dyn_name": dynamo_file.name,
                 "dyn_path": dyn_path_string,
@@ -447,15 +531,15 @@
         """Read python script to parameters
 
         Args:
             reread (bool, optional): Reread the file, even if it was read already. Defaults to False.
 
         Raises:
             FileNotFoundError: The file does not exist
-            PythonFileException: Some error reading the file
+            PythonFile.Error: Some error reading the file
         """
         if not self.exists:
             raise FileNotFoundError
 
         # Only read if it's not already open:
         if not self in self.open_files or reread:
 
@@ -482,32 +566,40 @@
                     code_start_line = i+2
                     break
 
                 else:
                     # Find the location of the separator
                     sl = line.find(":")
                     if sl == -1:
-                        raise PythonFileException("Error reading header!")
+                        raise self.Error("Error reading header!", self)
                     self.header_data[line[0:sl]] = line[sl+1:]
 
             self.code = python_lines[code_start_line:]
             self.open_files.add(self)
 
             logging.debug(f"Header data from python file: {self.header_data}")
             # logging.debug(f"Code from python file: {self.code}")
 
-    def update_dynamo(self, options: Options | None = None) -> None:
+    def update_dynamo(self, options: Options | None = None, **option_args) -> None:
         """Update a the source Dynamo graph from this python script
 
         Args:
             options (Options | None, optional): Run options. Defaults to None.
+            **option_args: Options() arguments
+
+        Raises:
+            ValueError: Both options and other arguments given
+
         """
 
         if not options:
-            options = Options()
+            options = Options.from_kwargs(kwargs=option_args)
+        elif option_args:
+            # Should not give both options and arguments:
+            raise ValueError("Options object and extra arguments!")
 
         dynamo_file = self.get_source_dynamo_file()
 
         new_python_node = PythonNode(python_file=self)
 
         old_python_node = dynamo_file.get_python_node_by_id(
             self.header_data["py_id"])
@@ -524,33 +616,42 @@
         logging.info(f"Dynamo graph will be updated: {dynamo_file.filepath}")
         dynamo_file.update_python_node(new_python_node)
 
     def get_source_dynamo_file(self) -> DynamoFile:
         """Get the source Dynamo file of this PythonFile
 
         Raises:
-            DynamoFileException: The uuid of the dynamo file changed
+            DynamoFile.Error: The uuid of the dynamo file changed
 
         Returns:
             DynamoFile: The DynamoFile
         """
 
         # Check if it was already opened:
         dynamo_file = DynamoFile.get_open_file_by_uuid(
             self.header_data["dyn_uuid"])
 
         # Open if it's the first time:
         if not dynamo_file:
 
-            dynamo_file = DynamoFile(
-                pathlib.Path(self.header_data["dyn_path"]))
+            cwd = pathlib.Path(os.getcwd()).resolve()
+            # Change to pythonfiles' dir:
+            os.chdir(self.dirpath)
+
+            dynpath = os.path.realpath(self.header_data["dyn_path"])
+            logging.debug(f"Resolved path: {dynpath}")
+
+            # Change back to the original path:
+            os.chdir(cwd)
+            dynamo_file = DynamoFile(pathlib.Path(dynpath))
 
             # Check if uuid is ok:
             if not dynamo_file.uuid == self.header_data["dyn_uuid"]:
-                raise DynamoFileException(f"Dynamo graph uuid changed!")
+                raise DynamoFile.Error(
+                    "Dynamo graph uuid changed!", dynamo_file)
 
         return dynamo_file
 
     def _write_file(self) -> None:
         """Write this file to the disk. Should be called only from File.write()"""
         with open(self.filepath, "w", encoding="utf-8", newline="") as output_file:
             output_file.write(self.text)
@@ -583,15 +684,15 @@
 
         Args:
             node_dict_from_dyn (dict, optional): The dict of the node from a dyn file. Defaults to {}.
             dynamo_file (DynamoFile, optional): The file the node is from. Defaults to None.
             python_file (PythonFile, optional): The python file to be converted to node. Defaults to None.
 
         Raises:
-            PythonNodeException: Wrong arguments were given
+            PythonNode.Error: Wrong arguments were given
         """
         # Initialize from dynamo file:
         if node_dict_from_dyn and dynamo_file and not python_file:
             self.id = node_dict_from_dyn["Id"]
 
             # Older dynamo files doesn't have "Engine" property, fall back to IronPython2
             if "Engine" in node_dict_from_dyn:
@@ -623,13 +724,23 @@
         elif python_file and not node_dict_from_dyn and not dynamo_file:
             self.id = python_file.header_data["py_id"]
             self.engine = python_file.header_data["py_engine"]
             self.code = python_file.code
             self.filename = python_file.basename + ".py"
             self.filepath = python_file.filepath
 
+        elif python_file and node_dict_from_dyn and dynamo_file:
+            raise self.Error("Too much arguments given!")
+
+        elif not python_file and not node_dict_from_dyn and not dynamo_file:
+            raise self.Error("No arguments given!")
+
         else:
-            raise PythonNodeException
+            raise self.Error("Something wrong!")
 
         # Calculate checksum:
         checksums = [hashlib.md5(l.encode()).hexdigest() for l in self.code]
         self.checksum = hashlib.md5("".join(checksums).encode()).hexdigest()
+
+    class Error(Exception):
+        """Something wrong with this node"""
+        pass
```

### Comparing `dyn2py-0.3.3/dyn2py.egg-info/PKG-INFO` & `dyn2py-0.4.0/dyn2py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyn2py
-Version: 0.3.3
+Version: 0.4.0
 Summary: Extract python code from Dynamo graphs
 Author-email: infeeeee <gyetpet@mailbox.org>
 Maintainer-email: infeeeee <gyetpet@mailbox.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -743,91 +743,112 @@
 positional arguments:
   source                path to a Dynamo graph, a python script or a folder containing them
 
 options:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
   -l LOGLEVEL, --loglevel LOGLEVEL
-                        set log level, possible options: CRITICAL, ERROR, WARNING, INFO, DEBUG
+                        set log level, possible options: HEADLESS, CRITICAL, ERROR, WARNING, INFO, DEBUG
   -n, --dry-run         do not modify files, only show log
   -F, --force           overwrite even if the files are older
   -b, --backup          create a backup for updated files
   -f {py,dyn}, --filter {py,dyn}
                         only check python or Dynamo graphs, skip the others, useful for folders
 
 dynamo options, only for processing Dynamo graphs:
   -u, --update          update Dynamo graph from python scripts in the same folder
   -p path/to/folder, --python-folder path/to/folder
                         extract python scripts to this folder, read python scripts from here with --update
 
 The script by default overwrites older files with newer files.
 Do not move the source Dynamo graphs, or update won't work with them later.
 Multiple sources are supported, separate them by spaces.
+HEADLESS loglevel only prints modified filenames.
 ```
 
 #### Examples
 
 *Notes: In Windows cmd use backward slashes as path separators, in any other shells use forward slashes. Powershell accepts both of them. Wrap paths with spaces in double quotes.*
 
-Extract all nodes next to a Dynamo file:
-
-```
+```shell
+# Extract all nodes next to a Dynamo file:
 dyn2py path/to/dynamofile.dyn
-```
-
-Update a Dynamo file from previously exported and modified python files:
 
-```
+# Update a Dynamo file from previously exported and modified python files:
 dyn2py --update path/to/dynamofile.dyn
-```
 
-Extract python nodes to a specific folder, process multiple Dynamo files:
-
-```
+# Extract python nodes to a specific folder, process multiple Dynamo files:
 dyn2py --python-folder path/to/pythonfiles path/to/dynamofile1.dyn path/to/dynamofile2.dyn
-```
-
-Update Dynamo files from python files from a folder. Only check python files, create backups:
 
-```
+# Update Dynamo files from python files from a folder. Only check python files, create backups:
 dyn2py --filter py --backup path/to/pythonfiles
 ```
 
+#### Git hooks
+
+Git hooks are a built-in feature of Git that allow developers to automate tasks throughout the Git workflow. Read more here: https://githooks.com/
+
+With the `pre-commit` hook it's possible to add more files to the currently initialized commit.
+
+You can find an example pre-commit hook here: [pre-commit](pre-commit). Copy this file to the `.git/hooks` folder of your repo of Dynamo graphs. This folder is hidden by default, but it should exist in all initialized git repo. Do not rename this file.
+
+This script will go through staged `.dyn` files and export python scripts from them, and add them to the current commit. Now you can check changed lines in a diff tool, you can see changed python code in a PR!
+
 ### As a python module
 
 Full API documentation available here: https://infeeeee.github.io/dyn2py
 
-Most basic example to extract all nodes next to a Dynamo file:
+#### Examples
+
+Extract all nodes from python nodes next to a Dynamo file:
 
 ```python
 import dyn2py
 
+# Open a Dynamo graph:
 dynamo_file = dyn2py.DynamoFile("path/to/dynamofile.dyn")
-python_files = dynamo_file.extract_python()
-[python_file.write() for python_file in python_files]
+
+# Extract python nodes:
+dynamo_file.extract_python()
+
+# Save all python nodes as separate files:
+dyn2py.PythonFile.write_open_files()
 ```
 
-Change options like with the command line switches with the `Options` class:
+Update python node from a python file:
 
 ```python
 import dyn2py
 
-# Create a backup on overwrite, read python files from a different folder:
-options = dyn2py.Options(
-    backup=True,
-    python_folder="path/to/pythonfiles")
+# Open a python file:
+python_file = dyn2py.PythonFile("path/to/pythonfile.py")
+
+# Update the node in the graph:
+python_file.update_dynamo()
+
+# Save modified Dynamo graph:
+dyn2py.DynamoFile.write_open_files()
+```
 
+Update all python nodes of a Dynamo grapg from a different folder, save backups:
+
+```python
+import dyn2py
+
+# open a Dynamo graph:
 dynamo_file = dyn2py.DynamoFile("path/to/dynamofile.dyn")
-python_files = dynamo_file.get_related_python_files(options)
+
+# Get python files from a dofferent folder:
+python_files = dynamo_file.get_related_python_files(python_folder="path/to/pythonfiles")
 
 # Read python files and update the graph:
-[python_file.update_dynamo(options) for python_file in python_files]
+[python_file.update_dynamo() for python_file in python_files]
 
-# Don't forget to save at the end:
-dynamo_file.write(options)
+# Save open Dynamo graphs:
+dyn2py.DynamoFile.write_open_files(backup=True)
 ```
 
 For more examples check tests in the [tests folder on Github](https://github.com/infeeeee/dyn2py/tree/main/tests)
 
 They should work in Dynamo, inside CPython3 nodes.
 
 ## Troubleshooting
@@ -838,14 +859,16 @@
 
 ## Limitations
 
 Only supports Dynamo 2 files, Dynamo 1 files are reported and ignored. Please update them to Dynamo 2 by opening them in Dynamo 2.
 
 Both IronPython2 and CPython3 nodes are supported! IronPython2 nodes won't be updated to CPython3, they will be imported as-is.
 
+Cannot create new python nodes, only existing ones can be updated.
+
 ## Development
 
 ### Installation
 
 Requirements: git, python, pip
 
 ```
@@ -855,40 +878,32 @@
 ```
 
 With venv:
 
 ```
 git clone https://github.com/infeeeee/dyn2py
 cd dyn2py
-venv .venv
+python -m venv .venv
 . ./.venv/bin/activate
 pip install -e .
 ```
 
 ### Build for Windows
 
 ```
 pip install -e .[build]
 pyinstaller dyn2py.spec
 ```
 
 ### Create installer for Windows
 
 - Install Inno Setup: https://jrsoftware.org/isdl.php
-- The already built exe should be in the root folder
-- Run this in powershell:
+- Build an exe
+- Run `dyn2py-installer.ps1` in powershell
 
-```powershell
-# Read version number from pyproject.toml and update in innosetup:
-$regex = Select-String -Path pyproject.toml -Pattern '^version = "((?:\d\.){2}\d)"$'
-$version = $regex.Matches.Groups[1].Value
-(Get-Content dyn2py-installer.iss).Replace("x.x.x",$version) | Set-Content dyn2py-installer.iss
-# Build:
-& "C:\Program Files (x86)\Inno Setup 6\ISCC.exe" -Qp $(Join-Path $PWD.Path dyn2py-installer.iss)
-```
 ### Live module documentation
 
 ```
 pip install -e .[doc]
 pdoc -d google dyn2py
 ```
 
@@ -901,13 +916,13 @@
 ```
 python -m unittest discover -v -s ./tests -p "test_*.py"
 ```
 
 ### New release
 
 1. Update version number in `pyproject.toml`
-2. Create a publish a git tag with that number
+2. Create and publish a git tag with that number
 
 ## License
 
 GPL-3.0
```

### Comparing `dyn2py-0.3.3/pyproject.toml` & `dyn2py-0.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dyn2py"
-version = "0.3.3"
+version = "0.4.0"
 description = "Extract python code from Dynamo graphs"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["dynamo", "dyn", "visual programming"]
 license = { file = "LICENSE" }
 
 
@@ -30,7 +30,10 @@
 
 [project.scripts]
 dyn2py = "dyn2py:__command_line"
 
 
 [build-system]
 requires = ["setuptools", "wheel"]
+
+[tool.setuptools]
+packages = ["dyn2py"]
```

### Comparing `dyn2py-0.3.3/tests/test_CommandLine.py` & `dyn2py-0.4.0/tests/test_CommandLine.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,24 +32,37 @@
         for arg in args:
             p = subprocess.run(f"dyn2py {arg}",
                                capture_output=True, shell=True)
 
             self.assertFalse(p.stderr)
 
     dyn_sources = [
-        {"filename": "python_nodes.dyn", "py_file_count": 6},
-        {"filename": "single_node.dyn", "py_file_count": 1}
+        {"filename": "python_nodes.dyn", "output_file_count": 6},
+        {"filename": "single_node.dyn", "output_file_count": 1}
+    ]
+
+    py_sources = [
+        {"filename": "single_node_mod.py"},
     ]
 
     dyn_sources_error = ["dynamo1file.dyn",
                          "no_python.dyn",
                          "nonexisting.dyn"]
 
     @staticmethod
     def run_command(args: list = []) -> dict:
+        """_summary_
+
+        Args:
+            args (list, optional): list of arguments to run. Defaults to [].
+
+        Returns:
+            dict["stderr"]: error message
+            dict["python_file_mtimes"]: exported file in the output dir, and modification times
+        """
         argstring = " ".join(args)
         process = subprocess.run(f"dyn2py -l WARNING {argstring}",
                                  capture_output=True, shell=True)
 
         stderr = process.stderr.decode()
 
         python_files = {p: p.stat().st_mtime for p in pathlib.Path(OUTPUT_DIR).iterdir()
@@ -72,30 +85,30 @@
                 for force_arg in ["-F", "--force"]:
                     for pfolder_option in ["", "-p", "--python-folder"]:
 
                         test_dicts = [source_dict.copy()]
 
                         test_dicts[0]["filenames"] = [
                             test_dicts[0]["filename"]]
-                        if i == 0:
+                        if i == 0 and len(source_dict) > 1:
                             # Create a multi file version on the first file:
                             d = {}
                             for key in source_dict:
                                 if key == "filename":
                                     d["filenames"] = [f["filename"]
                                                       for f in source_dicts]
                                 elif isinstance(source_dict[key], (int, float)):
                                     d[key] = sum([f[key]
                                                  for f in source_dicts])
                             test_dicts.append(d)
 
                         for test_dict in test_dicts:
 
                             if pfolder_option:
-                                file_dir = INPUT_DIR
+                                file_dir = TEMP_DIR
                                 pfolder_arg = f"{pfolder_option} {OUTPUT_DIR}"
                             else:
                                 file_dir = OUTPUT_DIR
                                 pfolder_arg = ""
 
                             test_dict["filepath"] = " ".join(
                                 [f"{file_dir}/{f}" for f in test_dict["filenames"]])
@@ -109,15 +122,15 @@
                             tests.append(test_dict)
 
         return tests
 
     def test_dyn_error(self):
         for s in self.dyn_sources_error:
 
-            cleanup_output_dir()
+            cleanup_dirs()
 
             if pathlib.Path(f"{INPUT_DIR}/{s}").exists():
                 shutil.copy(f"{INPUT_DIR}/{s}",
                             f"{OUTPUT_DIR}/{s}")
 
             file_open = self.run_command(
                 [f"{OUTPUT_DIR}/{s}"])
@@ -127,73 +140,120 @@
                 len(file_open["python_file_mtimes"]), 0)
 
     def test_dyn(self):
 
         dyn_tests = self.generate_test_args(self.dyn_sources)
 
         for s in dyn_tests:
-            cleanup_output_dir()
+            cleanup_dirs()
 
+            # if no pythonfolder, everything should be in output ddir
             if not s["pfolder_arg"]:
-                for filename in s["filenames"]:
-                    shutil.copy(f"{INPUT_DIR}/{filename}",
-                                f"{OUTPUT_DIR}/{filename}")
+                source_dir = OUTPUT_DIR
+            else:
+                source_dir = TEMP_DIR
+
+            # copy  source files:
+            for filename in s["filenames"]:
+                shutil.copy(f"{INPUT_DIR}/{filename}",
+                            f"{source_dir}/{filename}")
+            
 
+            # Open files normally
             file_open = self.run_command(
                 [s["pfolder_arg"], s['filepath']])
 
+            # Open without error:
             self.assertFalse(
                 bool(file_open["stderr"]), msg=file_open["stderr"])
             self.assertEqual(
-                len(file_open["python_file_mtimes"]), s["py_file_count"])
+                len(file_open["python_file_mtimes"]), s["output_file_count"])
 
             # Test no overwrite
             file_no_overwrite = self.run_command(
                 [s["pfolder_arg"], s['filepath']])
 
+            # Should give error, because they already exist:
             self.assertTrue(bool(file_no_overwrite["stderr"]))
             self.assertEqual(
-                len(file_no_overwrite["python_file_mtimes"]), s["py_file_count"])
+                len(file_no_overwrite["python_file_mtimes"]), s["output_file_count"])
 
+            # The modify time shouldn't change as they were not overwritten:
             for p in file_no_overwrite["python_file_mtimes"]:
                 self.assertEqual(
                     file_no_overwrite["python_file_mtimes"][p], file_open["python_file_mtimes"][p])
 
             # Test force:
             file_force = self.run_command(
                 [s["pfolder_arg"], s["force_arg"], s['filepath']])
 
+            # Should not have an error:
             self.assertFalse(bool(file_force["stderr"]))
             self.assertEqual(
-                len(file_force["python_file_mtimes"]), s["py_file_count"])
+                len(file_force["python_file_mtimes"]), s["output_file_count"])
 
+            # Modify time should be higher as they were replaced
             for p in file_force["python_file_mtimes"]:
                 self.assertTrue(
                     file_force["python_file_mtimes"][p] > file_open["python_file_mtimes"][p]
                 )
 
             # Test backup
             file_backup = self.run_command(
                 [s["pfolder_arg"], s["force_arg"], s["backup_arg"], s['filepath']])
 
             self.assertFalse(bool(file_backup["stderr"]))
 
             self.assertEqual(
-                len(file_backup["python_file_mtimes"]), s["py_file_count"] * 2)
+                len(file_backup["python_file_mtimes"]
+                    ), s["output_file_count"] * 2,
+                msg=f""
+            )
 
             for p in file_force["python_file_mtimes"]:
                 self.assertTrue(
                     file_backup["python_file_mtimes"][p] > file_force["python_file_mtimes"][p]
                 )
 
+    # def test_py(self):
+    #     py_tests = self.generate_test_args(self.py_sources)
+
+    #     # TODO add more python files!
+    #     self.assertEqual(len(py_tests), 1)
+
+    #     for s in py_tests:
+    #         cleanup_dirs()
+
+    #         extract_single_node_dyn(modify_py=True)
+
+            
+    #         # if pythonfolder, python should be in the temp folder:
+    #         if s["pfolder_arg"]:
+    #             for filename in s["filenames"]:
+    #                 shutil.move(f"{OUTPUT_DIR}/{filename}",
+    #                             f"{TEMP_DIR}/{filename}")
+
+    #         # Open files normally
+    #         file_open = self.run_command(
+    #             [s["pfolder_arg"], s['filepath']])
+
+
+    #         # Open without error:
+    #         self.assertFalse(
+    #             bool(file_open["stderr"]), msg=file_open["stderr"])
+    #         self.assertEqual(
+    #             len(file_open["python_file_mtimes"]), s["output_file_count"])
+
+                                
+
     def test_single_dyn_dryrun(self):
         for s in self.dyn_sources:
             for arg in ["-n", "--dry-run"]:
 
-                cleanup_output_dir()
+                cleanup_dirs()
 
                 shutil.copy(f"{INPUT_DIR}/{s['filename']}",
                             f"{OUTPUT_DIR}/{s['filename']}")
 
                 file_dryrun = self.run_command(
                     [arg, f"{OUTPUT_DIR}/{s['filename']}"])
```

### Comparing `dyn2py-0.3.3/tests/test_DynamoFile.py` & `dyn2py-0.4.0/tests/test_DynamoFile.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,49 +15,48 @@
         dyn = dyn2py.DynamoFile(f"{INPUT_DIR}/python_nodes.dyn")
 
         self.assertEqual(dyn.uuid, "3c3b4c05-9716-4e93-9360-ca0637cb5486")
         self.assertEqual(dyn.name, "python_nodes")
         self.assertTrue(dyn in dyn2py.DynamoFile.open_files)
 
         # Dynamo 1 file:
-        with self.assertRaises(dyn2py.DynamoFileException):
+        with self.assertRaises(dyn2py.DynamoFile.Error):
             dyn1 = dyn2py.DynamoFile(f"{INPUT_DIR}/dynamo1file.dyn")
 
         # Not existing file:
         with self.assertRaises(FileNotFoundError):
             dyn2 = dyn2py.DynamoFile(f"{INPUT_DIR}/not_existing.dyn")
 
         # No python nodes:
-        with self.assertRaises(dyn2py.PythonNodeNotFoundException):
+        with self.assertRaises(dyn2py.DynamoFile.PythonNodeNotFound):
             dyn2 = dyn2py.DynamoFile(f"{INPUT_DIR}/no_python.dyn")
 
     def test_get_python_nodes(self):
         dyn = dyn2py.DynamoFile(f"{INPUT_DIR}/python_nodes.dyn")
         py_node = dyn.get_python_node_by_id("d7704617c75e4bf1a5c387b7c3f001ea")
 
         self.assertEqual(len(dyn.python_nodes), 6)
         self.assertTrue(py_node)
         self.assertIn(py_node, dyn.python_nodes)
         self.assertEqual(py_node.checksum, "e830a6ae6b395bcfd4e5a40da48f3bfc")
 
-        with self.assertRaises(dyn2py.PythonNodeNotFoundException):
+        with self.assertRaises(dyn2py.DynamoFile.PythonNodeNotFound):
             dyn.get_python_node_by_id("wrongid")
 
     def test_extract_python(self):
-        cleanup_output_dir()
+        cleanup_dirs()
         dyn2py.PythonFile.open_files.clear()
 
         opt = dyn2py.Options(python_folder=OUTPUT_DIR)
         dyn = dyn2py.DynamoFile(f"{INPUT_DIR}/python_nodes.dyn")
         dyn.extract_python(options=opt)
 
-        self.assertEqual(len(dyn2py.PythonFile.open_files), 6)
+        self.assertEqual(len(dyn2py.PythonFile.get_open_files()), 6)
 
-        for f in dyn2py.PythonFile.open_files:
-            f.write()
+        dyn2py.PythonFile.write_open_files()
 
         output_dir = pathlib.Path(OUTPUT_DIR)
         self.assertEqual(len(list(output_dir.iterdir())), 6)
 
     def test_get_open_file_by_uuid(self):
         dyn2py.DynamoFile.open_files.clear()
 
@@ -66,15 +65,15 @@
 
         self.assertEqual(dyn1,
                          dyn2py.DynamoFile.get_open_file_by_uuid("3c3b4c05-9716-4e93-9360-ca0637cb5486"))
         self.assertEqual(dyn2,
                          dyn2py.DynamoFile.get_open_file_by_uuid("76de5c79-17c5-4c74-9f90-ad99a213d339"))
 
     def test_get_related_python_files(self):
-        cleanup_output_dir()
+        cleanup_dirs()
 
         opt = dyn2py.Options(python_folder=OUTPUT_DIR)
         dyn1 = dyn2py.DynamoFile(f"{INPUT_DIR}/python_nodes.dyn")
         dyn2 = dyn2py.DynamoFile(f"{INPUT_DIR}/single_node.dyn")
         for dyn in [dyn1, dyn2]:
             dyn.extract_python(options=opt)
             for f in dyn2py.PythonFile.open_files:
@@ -88,15 +87,15 @@
         self.assertEqual(len(python_files2), 1)
 
         no_python_files = dyn1.get_related_python_files()
 
         self.assertFalse(no_python_files)
 
     def test_write_same(self):
-        cleanup_output_dir()
+        cleanup_dirs()
 
         shutil.copy(f"{INPUT_DIR}/python_nodes.dyn",
                     f"{OUTPUT_DIR}/python_nodes.dyn")
 
         new_dyn = dyn2py.DynamoFile(f"{OUTPUT_DIR}/python_nodes.dyn")
         new_dyn.modified = True
         new_dyn.write()
@@ -135,10 +134,10 @@
         # Check if the node in the copy:
         dyn2 = dyn2py.DynamoFile(f"{OUTPUT_DIR}/single_node2.dyn")
         node2 = dyn2.get_python_node_by_id(node_id=node1.id)
 
         self.assertTrue(node2)
         self.assertEqual(node1.checksum, node2.checksum)
 
-        with self.assertRaises(dyn2py.PythonNodeNotFoundException):
+        with self.assertRaises(dyn2py.DynamoFile.PythonNodeNotFound):
             node2.id = "wrong_id"
             dyn2.update_python_node(node2)
```

### Comparing `dyn2py-0.3.3/tests/test_File.py` & `dyn2py-0.4.0/tests/test_File.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 import platform
 
 from tests.support import *
 
 
 class TestFile(unittest.TestCase):
 
-    # Write methods should be tested in subclasses!
-
     def test_init(self):
         paths = [
             f"{INPUT_DIR}/python_nodes.dyn",
             pathlib.Path(f"{INPUT_DIR}/python_nodes.dyn")
         ]
 
         if platform.system() == "Windows":
@@ -67,15 +65,15 @@
             self.assertEqual(the_file.__class__, dyn2py.PythonFile)
 
     def test_newer(self):
         older_file = dyn2py.File(f"{INPUT_DIR}/single_node.dyn")
         nonexisting_file = dyn2py.File(f"{INPUT_DIR}/new_file.py")
 
         # Extract a python file so it is always newer than the others:
-        cleanup_output_dir()
+        cleanup_dirs()
         opt = dyn2py.Options(python_folder=OUTPUT_DIR)
         older_file.extract_python(options=opt)  # type: ignore
         for f in dyn2py.PythonFile.open_files:
             f.write()
         newer_file = dyn2py.File(
             f"{OUTPUT_DIR}/single_node_1c5d99792882409e97e132b3e9f814b0.py")
 
@@ -99,7 +97,19 @@
         ]
 
         for path, f in paths:
             file = dyn2py.File(path)
 
             self.assertEqual(file.is_dynamo_file(), f == "dyn")
             self.assertEqual(file.is_python_file(), f == "py")
+
+    def test_write(self):
+
+        # new empty file:
+        empty_filepath = pathlib.Path(f"{OUTPUT_DIR}/empty.txt")
+        empty_filepath.touch()
+
+        empty_file = dyn2py.File(f"{OUTPUT_DIR}/empty.txt")
+        
+        self.assertTrue(empty_file.exists)
+        with self.assertRaises(TypeError):
+            empty_file.write()
```

### Comparing `dyn2py-0.3.3/tests/test_PythonFile.py` & `dyn2py-0.4.0/tests/test_PythonFile.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 
 
 class TestPythonFile(unittest.TestCase):
 
     def test_init(self):
         extract_single_node_dyn()
 
-        py1 = dyn2py.PythonFile(f"{OUTPUT_DIR}/single_node_1c5d99792882409e97e132b3e9f814b0.py")
+        dyn2py.File.open_files.clear()
 
-        dyn2py.DynamoFile.open_files.clear()
+        py1 = dyn2py.PythonFile(
+            f"{OUTPUT_DIR}/single_node_1c5d99792882409e97e132b3e9f814b0.py")
         dyn = dyn2py.DynamoFile(f"{INPUT_DIR}/single_node.dyn")
         node = list(dyn.python_nodes)[0]
         py2 = dyn2py.PythonFile(filepath=node.filepath,
                                 dynamo_file=dyn, python_node=node)
 
         for py in [py1, py2]:
 
             self.assertEqual(len(py.code), 17)
-            self.assertEqual(len(py.text.split(os.linesep)), 32, msg=py.filepath)
+            self.assertEqual(len(py.text.split(os.linesep)),
+                             32, msg=py.filepath)
             self.assertIs(type(py.header_data), dict)
-            self.assertTrue(py in dyn2py.PythonFile.open_files)
+            self.assertTrue(py in dyn2py.PythonFile.get_open_files())
 
     def test_update_dynamo(self):
         extract_single_node_dyn(modify_py=True)
 
         dyn2py.DynamoFile.open_files.clear()
         dyn2py.PythonFile.open_files.clear()
 
@@ -64,43 +66,41 @@
         # It should work with force:
         opt = dyn2py.Options(force=True)
         py2.update_dynamo(options=opt)
         self.assertTrue(dyn2.modified)
 
     def test_get_source_dynamo_file(self):
         extract_single_node_dyn()
-        dyn2py.DynamoFile.open_files.clear()
-        dyn2py.PythonFile.open_files.clear()
+        dyn2py.File.open_files.clear()
 
         py1 = dyn2py.PythonFile(
             f"{OUTPUT_DIR}/single_node_1c5d99792882409e97e132b3e9f814b0.py")
 
         dyn1 = py1.get_source_dynamo_file()
-        self.assertEqual(len(dyn2py.DynamoFile.open_files), 1)
+        self.assertEqual(len(dyn2py.DynamoFile.get_open_files()), 1)
         self.assertIn(dyn1, dyn2py.DynamoFile.open_files)
 
         dyn2 = py1.get_source_dynamo_file()
         self.assertIs(dyn1, dyn2)
 
         dyn2py.DynamoFile.open_files.clear()
 
-        with self.assertRaises(dyn2py.DynamoFileException):
+        with self.assertRaises(dyn2py.DynamoFile.Error):
             py1.header_data["dyn_uuid"] = "wrong-uuid"
             py1.get_source_dynamo_file()
 
     def test_write(self):
         extract_single_node_dyn()
-        dyn2py.DynamoFile.open_files.clear()
-        dyn2py.PythonFile.open_files.clear()
+        dyn2py.File.open_files.clear()
 
         py1 = dyn2py.PythonFile(
             f"{OUTPUT_DIR}/single_node_1c5d99792882409e97e132b3e9f814b0.py")
 
         dyn1 = py1.get_source_dynamo_file()
         node = list(dyn1.python_nodes)[0]
         py2 = dyn2py.PythonFile(
-            node.filepath, dynamo_file=dyn1, python_node=node)
+            f"{OUTPUT_DIR}/{node.filename}", dynamo_file=dyn1, python_node=node)
         self.assertIsNot(py1, py2)
         self.assertEqual(py1.code, py2.code)
         for d in py1.header_data:
             if not d == "dyn2py_extracted":
                 self.assertEqual(py1.header_data[d], py2.header_data[d])
```

### Comparing `dyn2py-0.3.3/tests/test_PythonNode.py` & `dyn2py-0.4.0/tests/test_PythonNode.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,15 +44,16 @@
         node_dict = next((n for n in dyn.full_dict["Nodes"]
                           if n["NodeType"] == "PythonScriptNode"), {})
 
         extract_single_node_dyn(modify_py=True)
 
         py = dyn2py.PythonFile(f"{OUTPUT_DIR}/single_node_mod.py")
 
-        with self.assertRaises(dyn2py.PythonNodeException):
+        with self.assertRaises(dyn2py.PythonNode.Error):
             node1 = dyn2py.PythonNode(
                 node_dict_from_dyn=node_dict,
                 dynamo_file=dyn,
                 python_file=py
             )
-
+        
+        with self.assertRaises(dyn2py.PythonNode.Error):
             node2 = dyn2py.PythonNode()
```

