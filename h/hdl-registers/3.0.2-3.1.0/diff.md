# Comparing `tmp/hdl_registers-3.0.2.tar.gz` & `tmp/hdl_registers-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdl_registers-3.0.2.tar", last modified: Sat Mar  4 14:22:55 2023, max compression
+gzip compressed data, was "hdl_registers-3.1.0.tar", last modified: Tue Apr 25 07:27:32 2023, max compression
```

## Comparing `hdl_registers-3.0.2.tar` & `hdl_registers-3.1.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 14:22:55.105303 hdl_registers-3.0.2/
--rw-r--r--   0 root         (0) root         (0)     3423 2023-03-04 14:22:55.105303 hdl_registers-3.0.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 14:22:55.096302 hdl_registers-3.0.2/hdl_registers/
--rw-rw-rw-   0 root         (0) root         (0)      874 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4927 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/about.py
--rw-rw-rw-   0 root         (0) root         (0)     2528 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/bit.py
--rw-rw-rw-   0 root         (0) root         (0)     4214 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/bit_vector.py
--rw-rw-rw-   0 root         (0) root         (0)     1831 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/constant.py
--rw-rw-rw-   0 root         (0) root         (0)     2882 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/html_translator.py
--rw-rw-rw-   0 root         (0) root         (0)    10474 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     6239 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/register.py
--rw-rw-rw-   0 root         (0) root         (0)     3433 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/register_array.py
--rw-rw-rw-   0 root         (0) root         (0)     8233 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/register_c_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/register_code_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    29090 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/register_cpp_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     4446 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/register_field.py
--rw-rw-rw-   0 root         (0) root         (0)    13707 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/register_field_type.py
--rw-rw-rw-   0 root         (0) root         (0)     9540 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/register_html_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    18096 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/register_list.py
--rw-rw-rw-   0 root         (0) root         (0)     2766 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/register_python_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     9546 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/register_vhdl_generator.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/requirements_develop.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 14:22:55.099302 hdl_registers-3.0.2/hdl_registers/test/
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      688 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/test/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 14:22:55.105303 hdl_registers-3.0.2/hdl_registers/test/unit/
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/test/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4215 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/test/unit/test_bit.py
--rw-rw-rw-   0 root         (0) root         (0)    10454 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/test/unit/test_bit_vector.py
--rw-rw-rw-   0 root         (0) root         (0)     2007 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/test/unit/test_constant.py
--rw-rw-rw-   0 root         (0) root         (0)     3924 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/test/unit/test_html_translator.py
--rw-rw-rw-   0 root         (0) root         (0)    16015 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/test/unit/test_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     5549 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/test/unit/test_register.py
--rw-rw-rw-   0 root         (0) root         (0)     4793 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/test/unit/test_register_array.py
--rw-rw-rw-   0 root         (0) root         (0)     3761 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/test/unit/test_register_code_generation.py
--rw-rw-rw-   0 root         (0) root         (0)     1409 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/test/unit/test_register_cpp_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     9368 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/test/unit/test_register_field_type.py
--rw-rw-rw-   0 root         (0) root         (0)     7231 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/test/unit/test_register_html_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    16339 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/test/unit/test_register_list.py
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/test/unit/test_register_python_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     5509 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/hdl_registers/test/unit/test_register_vhdl_generator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 14:22:55.098302 hdl_registers-3.0.2/hdl_registers.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3423 2023-03-04 14:22:55.000000 hdl_registers-3.0.2/hdl_registers.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1669 2023-03-04 14:22:55.000000 hdl_registers-3.0.2/hdl_registers.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-04 14:22:55.000000 hdl_registers-3.0.2/hdl_registers.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-04 14:22:55.000000 hdl_registers-3.0.2/hdl_registers.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      161 2023-03-04 14:22:55.000000 hdl_registers-3.0.2/hdl_registers.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-04 14:22:55.000000 hdl_registers-3.0.2/hdl_registers.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      923 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-04 14:22:55.105303 hdl_registers-3.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4833 2023-03-04 14:22:54.000000 hdl_registers-3.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:27:32.664765 hdl_registers-3.1.0/
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-04-25 07:27:32.664765 hdl_registers-3.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:27:32.656764 hdl_registers-3.1.0/hdl_registers/
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5154 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/about.py
+-rw-rw-rw-   0 root         (0) root         (0)     2528 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/bit.py
+-rw-rw-rw-   0 root         (0) root         (0)     4214 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/bit_vector.py
+-rw-rw-rw-   0 root         (0) root         (0)     1989 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/constant.py
+-rw-rw-rw-   0 root         (0) root         (0)     2882 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/html_translator.py
+-rw-rw-rw-   0 root         (0) root         (0)    10474 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     6239 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/register.py
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/register_array.py
+-rw-rw-rw-   0 root         (0) root         (0)     8782 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/register_c_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/register_code_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    29313 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/register_cpp_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4446 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/register_field.py
+-rw-rw-rw-   0 root         (0) root         (0)    13707 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/register_field_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     9956 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/register_html_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    18096 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/register_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     2766 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/register_python_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     9666 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/register_vhdl_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/requirements_develop.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:27:32.658764 hdl_registers-3.1.0/hdl_registers/test/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      688 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/test/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:27:32.664765 hdl_registers-3.1.0/hdl_registers/test/unit/
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/test/unit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4215 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/test/unit/test_bit.py
+-rw-rw-rw-   0 root         (0) root         (0)    10454 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/test/unit/test_bit_vector.py
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/test/unit/test_constant.py
+-rw-rw-rw-   0 root         (0) root         (0)     3924 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/test/unit/test_html_translator.py
+-rw-rw-rw-   0 root         (0) root         (0)    16349 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/test/unit/test_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     5549 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/test/unit/test_register.py
+-rw-rw-rw-   0 root         (0) root         (0)     4793 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/test/unit/test_register_array.py
+-rw-rw-rw-   0 root         (0) root         (0)     3761 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/test/unit/test_register_code_generation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1409 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/test/unit/test_register_cpp_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     9368 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/test/unit/test_register_field_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     7523 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/test/unit/test_register_html_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    16339 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/test/unit/test_register_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/test/unit/test_register_python_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5734 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/hdl_registers/test/unit/test_register_vhdl_generator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 07:27:32.658764 hdl_registers-3.1.0/hdl_registers.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-04-25 07:27:32.000000 hdl_registers-3.1.0/hdl_registers.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-25 07:27:32.000000 hdl_registers-3.1.0/hdl_registers.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 07:27:32.000000 hdl_registers-3.1.0/hdl_registers.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 07:27:32.000000 hdl_registers-3.1.0/hdl_registers.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      161 2023-04-25 07:27:32.000000 hdl_registers-3.1.0/hdl_registers.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-25 07:27:32.000000 hdl_registers-3.1.0/hdl_registers.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      923 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 07:27:32.664765 hdl_registers-3.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4835 2023-04-25 07:27:31.000000 hdl_registers-3.1.0/setup.py
```

### Comparing `hdl_registers-3.0.2/PKG-INFO` & `hdl_registers-3.1.0/hdl_registers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: hdl_registers
-Version: 3.0.2
-Summary: An open-source HDL register generator fast enough to run in real time.
+Name: hdl-registers
+Version: 3.1.0
+Summary: An open-source HDL register generator fast enough to run in real time
 Home-page: https://hdl-registers.com
 Author: Lukas Vik
 Author-email: 2767848-LukasVik@users.noreply.gitlab.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://hdl-registers.com/
 Project-URL: Changelog, https://hdl-registers.com/release_notes.html
 Project-URL: Source, https://gitlab.com/hdl_registers/hdl_registers
@@ -18,17 +18,14 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 
-About hdl_registers
-===================
-
 |pic_website| |pic_gitlab| |pic_gitter| |pic_pip_install| |pic_license| |pic_python_line_coverage|
 
 .. |pic_website| image:: https://hdl-registers.com/badges/website.svg
   :alt: Website
   :target: https://hdl-registers.com
 
 .. |pic_gitlab| image:: https://hdl-registers.com/badges/gitlab.svg
```

### Comparing `hdl_registers-3.0.2/hdl_registers/__init__.py` & `hdl_registers-3.1.0/hdl_registers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 # https://gitlab.com/hdl_registers/hdl_registers
 # --------------------------------------------------------------------------------------------------
 
 # Standard libraries
 from pathlib import Path
 
 # Local folder libraries
-from .about import get_pypi_slogan
+from .about import get_short_slogan
 
 REPO_ROOT = Path(__file__).parent.parent.resolve()
 
 HDL_REGISTERS_PATH = REPO_ROOT / "hdl_registers"
 HDL_REGISTERS_TEST = HDL_REGISTERS_PATH / "test"
 HDL_REGISTERS_DOC = REPO_ROOT / "doc"
 HDL_REGISTERS_GENERATED = REPO_ROOT / "generated"
 
-__version__ = "3.0.2"
-__doc__ = get_pypi_slogan()  # pylint: disable=redefined-builtin
+__version__ = "3.1.0"
+__doc__ = get_short_slogan()  # pylint: disable=redefined-builtin
```

### Comparing `hdl_registers-3.0.2/hdl_registers/about.py` & `hdl_registers-3.1.0/hdl_registers/about.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,26 +4,25 @@
 # This file is part of the hdl_registers project, a HDL register generator fast enough to run
 # in real time.
 # https://hdl-registers.com
 # https://gitlab.com/hdl_registers/hdl_registers
 # --------------------------------------------------------------------------------------------------
 
 
-def get_pypi_slogan():
+def get_short_slogan():
     """
-    Short slogan used on pypi.org and in Python package.
-    Note that there seems to be an upper limit of 98 characters, so it can't be the same as the one
-    on the website.
-
-    Note that this slogan is also listed (manually duplicated) in license.rst for
-    academic citations.
-    If you change in one place you should change in both.
+    Short slogan used e.g. on pypi.org.
+    Note that there seems to be an upper limit of 98 characters when rendering the slogan
+    on pypi.org.
+
+    Note that this slogan should be the same as the one used in the readme and on the website below.
+    The difference is capitalization and whether the project name is included.
     """
-    rst = "An open-source HDL register generator fast enough to run in real time."
-    return rst
+    result = "An open-source HDL register generator fast enough to run in real time"
+    return result
 
 
 def get_readme_rst(
     include_extra_for_gitlab=False,
     include_extra_for_website=False,
     include_extra_for_pypi=False,
 ):
@@ -40,39 +39,47 @@
             gitlab README.
         include_extra_for_website (bool): Include the extra text that shall be included in the
             website main page.
         include_extra_for_pypi (bool): Include the extra text that shall be included in the
             PyPI release README.
     """
     if include_extra_for_gitlab:
+        readme_rst = ""
         extra_rst = """\
 **See documentation on the website**: https://hdl-registers.com
 
 **See PyPI for installation details**: https://pypi.org/project/hdl-registers/
 """
     elif include_extra_for_website:
+        # The website needs the initial heading, in order for the landing page to get
+        # the correct title.
+        # The others do not need this initial heading, it just makes the gitlab/pypi page
+        # more clunky.
+        readme_rst = """\
+About hdl_registers
+===================
+
+"""
         extra_rst = """\
-This website contains readable documentation for the project.
+To install the Python package, see :ref:`installation`.
 To check out the source code go to the
 `gitlab page <https://gitlab.com/hdl_registers/hdl_registers>`__.
-To install see the `PyPI page <https://pypi.org/project/hdl-registers/>`__.
 """
     elif include_extra_for_pypi:
+        readme_rst = ""
         extra_rst = """\
 **See documentation on the website**: https://hdl-registers.com
 
 **Check out the source code on gitlab**: https://gitlab.com/hdl_registers/hdl_registers
 """
     else:
+        readme_rst = ""
         extra_rst = ""
 
-    readme_rst = f"""\
-About hdl_registers
-===================
-
+    readme_rst += f"""\
 |pic_website| |pic_gitlab| |pic_gitter| |pic_pip_install| |pic_license| |pic_python_line_coverage|
 
 .. |pic_website| image:: https://hdl-registers.com/badges/website.svg
   :alt: Website
   :target: https://hdl-registers.com
 
 .. |pic_gitlab| image:: https://hdl-registers.com/badges/gitlab.svg
@@ -115,10 +122,10 @@
 <https://hdl-modules.com/modules/reg_file/reg_file.html#axi-lite-reg-file-vhd>`_
   in your VHDL code.
 * HTML website with documentation of the registers and constants.
 * C header with constant values, register addresses, and register field information.
 * C++ header and implementation with constant values, and setters/getters for
   registers and fields.
   The header has an abstract interface class which can be used for mocking.
-"""  # noqa: E501
+"""
 
     return readme_rst
```

### Comparing `hdl_registers-3.0.2/hdl_registers/bit.py` & `hdl_registers-3.1.0/hdl_registers/bit.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/bit_vector.py` & `hdl_registers-3.1.0/hdl_registers/bit_vector.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/constant.py` & `hdl_registers-3.1.0/hdl_registers/constant.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 # This file is part of the hdl_registers project, a HDL register generator fast enough to run
 # in real time.
 # https://hdl-registers.com
 # https://gitlab.com/hdl_registers/hdl_registers
 # --------------------------------------------------------------------------------------------------
 
 
-class Constant:
+class Constant:  # pylint: disable=too-many-instance-attributes
     is_boolean = False
     is_integer = False
     is_float = False
+    is_string = False
 
     def __init__(self, name, value, description=None):
         """
         Arguments:
             name (str): The name of the constant.
             value (bool, int, str): The constant value.
             description (str): Textual description for the constant.
@@ -44,15 +45,18 @@
         if isinstance(value, int):
             self.is_boolean = isinstance(value, bool)
             self.is_integer = not self.is_boolean
 
         elif isinstance(value, float):
             self.is_float = True
 
-        if sum([self.is_boolean, self.is_integer, self.is_float]) != 1:
+        elif isinstance(value, str):
+            self.is_string = True
+
+        if sum([self.is_boolean, self.is_integer, self.is_float, self.is_string]) != 1:
             raise ValueError(
                 f'Constant "{self.name}" has invalid data type "{type(value)}". Value: "{value}"'
             )
 
     def __repr__(self):
         return f"""{self.__class__.__name__}(\
 name={self.name},\
```

### Comparing `hdl_registers-3.0.2/hdl_registers/html_translator.py` & `hdl_registers-3.1.0/hdl_registers/html_translator.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/parser.py` & `hdl_registers-3.1.0/hdl_registers/parser.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/register.py` & `hdl_registers-3.1.0/hdl_registers/register.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/register_array.py` & `hdl_registers-3.1.0/hdl_registers/register_array.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/register_c_generator.py` & `hdl_registers-3.1.0/hdl_registers/register_c_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,23 +174,37 @@
         else:
             name = f"{self.module_name}_{register_array.name}_{register.name}"
         return name.upper()
 
     def _constants(self, constants):
         c_code = ""
         for constant in constants:
+            constant_name = f"{self.module_name.upper()}_{constant.name.upper()}"
+
+            # Most of the types are a simple "#define". But some are special, where we explicitly
+            # set the declaration.
+            declaration = ""
+
             if constant.is_boolean:
                 value = str(constant.value).lower()
             elif constant.is_integer:
-                # No suffix -> "int", i.e. signed integer of at least 32 bits
+                # No suffix -> "int", i.e. signed integer of at least 32 bits.
                 value = str(constant.value)
             elif constant.is_float:
-                # "f" suffix -> "float" (as opposed to "double", to match the VHDL type)
+                # "f" suffix -> "float" (as opposed to "double", to match the VHDL type).
                 value = f"{constant.value}f"
+            elif constant.is_string:
+                # C string literal: Raw value enclosed in double quotation marks.
+                declaration = f'char *{constant_name} = "{constant.value}";'
             else:
                 raise ValueError(f"Got unexpected constant type. {constant}")
 
             c_code += self._comment(f'Register constant "{constant.name}".')
             c_code += self._comment_block(constant.description)
-            c_code += f"#define {self.module_name.upper()}_{constant.name.upper()} ({value})\n"
+
+            if declaration:
+                c_code += f"{declaration}\n"
+            else:
+                # Default: simple "#define"
+                c_code += f"#define {constant_name} ({value})\n"
 
         return c_code
```

### Comparing `hdl_registers-3.0.2/hdl_registers/register_code_generator.py` & `hdl_registers-3.1.0/hdl_registers/register_code_generator.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/register_cpp_generator.py` & `hdl_registers-3.1.0/hdl_registers/register_cpp_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,14 +349,18 @@
                 value = str(constant.value)
             elif constant.is_float:
                 # Expand "const" to "constexpr", which is needed for static floats. See
                 # https://stackoverflow.com/questions/9141950/
                 # initializing-const-member-within-class-declaration-in-c
                 type_declaration = "expr float"
                 value = str(constant.value)
+            elif constant.is_string:
+                # Expand "const" to "constexpr", which is needed for static string literals.
+                type_declaration = "expr auto"
+                value = f'"{constant.value}"'
             else:
                 raise ValueError(f"Got unexpected constant type. {constant}")
 
             cpp_code += self._comment("Register constant.", indentation=2)
             cpp_code += f"  static const{type_declaration} {constant.name} = {value};\n"
 
         if constants:
```

### Comparing `hdl_registers-3.0.2/hdl_registers/register_field.py` & `hdl_registers-3.1.0/hdl_registers/register_field.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/register_field_type.py` & `hdl_registers-3.1.0/hdl_registers/register_field_type.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/register_html_generator.py` & `hdl_registers-3.1.0/hdl_registers/register_html_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -277,20 +277,30 @@
 
         html += """
 </tbody>
 </table>"""
 
         return html
 
-    def _format_hex_constant(self, constant):
+    def _format_constant_value(self, constant):
+        if constant.is_string:
+            return f'"{constant.value}"'
+
+        # For others, just cast to string
+        if constant.is_boolean or constant.is_integer or constant.is_float:
+            return str(constant.value)
+
+        raise ValueError(f"Got unexpected constant type. {constant}")
+
+    def _format_hex_constant_value(self, constant):
         if constant.is_integer:
             return self._to_hex_string(value=constant.value, num_nibbles=8)
 
         # No hex formatting available for the other types
-        if constant.is_boolean or constant.is_float:
+        if constant.is_boolean or constant.is_float or constant.is_string:
             return "-"
 
         raise ValueError(f"Got unexpected constant type. {constant}")
 
     def _get_constant_table(self, constants):
         html = """
 <table>
@@ -305,16 +315,16 @@
 <tbody>"""
 
         for constant in constants:
             description = self._html_translator.translate(constant.description)
             html += f"""
   <tr>
     <td><strong>{constant.name}</strong></td>
-    <td>{constant.value}</td>
-    <td>{self._format_hex_constant(constant=constant)}</td>
+    <td>{self._format_constant_value(constant=constant)}</td>
+    <td>{self._format_hex_constant_value(constant=constant)}</td>
     <td>{description}</td>
   </tr>"""
 
         html += """
 </tbody>
 </table>"""
         return html
```

### Comparing `hdl_registers-3.0.2/hdl_registers/register_list.py` & `hdl_registers-3.1.0/hdl_registers/register_list.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/register_python_generator.py` & `hdl_registers-3.1.0/hdl_registers/register_python_generator.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/register_vhdl_generator.py` & `hdl_registers-3.1.0/hdl_registers/register_vhdl_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,14 +207,17 @@
                 value = str(constant.value).lower()
             elif constant.is_integer:
                 type_name = "integer"
                 value = constant.value
             elif constant.is_float:
                 type_name = "real"
                 value = constant.value
+            elif constant.is_string:
+                type_name = "string"
+                value = f'"{constant.value}"'
             else:
                 raise ValueError(f"Got unexpected constant type. {constant}")
 
             vhdl += (
                 "  constant "
                 f"{self.module_name}_constant_{constant.name} : {type_name} := {value};\n"
             )
```

### Comparing `hdl_registers-3.0.2/hdl_registers/test/conftest.py` & `hdl_registers-3.1.0/hdl_registers/test/conftest.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/test/unit/test_bit.py` & `hdl_registers-3.1.0/hdl_registers/test/unit/test_bit.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/test/unit/test_bit_vector.py` & `hdl_registers-3.1.0/hdl_registers/test/unit/test_bit_vector.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/test/unit/test_constant.py` & `hdl_registers-3.1.0/hdl_registers/test/unit/test_constant.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,54 +3,70 @@
 #
 # This file is part of the hdl_registers project, a HDL register generator fast enough to run
 # in real time.
 # https://hdl-registers.com
 # https://gitlab.com/hdl_registers/hdl_registers
 # --------------------------------------------------------------------------------------------------
 
+# Standard libraries
+from pathlib import Path
+
 # Third party libraries
 import pytest
 
 # First party libraries
 from hdl_registers.constant import Constant
 
 
 def test_boolean():
     for value in [True, False]:
         constant = Constant(name="apa", value=value)
 
         assert constant.is_boolean
         assert not constant.is_integer
         assert not constant.is_float
+        assert not constant.is_string
 
 
 def test_integer():
     for value in [123, -9]:
         constant = Constant(name="apa", value=value)
 
-        assert constant.is_integer
         assert not constant.is_boolean
+        assert constant.is_integer
         assert not constant.is_float
+        assert not constant.is_string
 
 
 def test_float():
     for value in [3.14, -9.9]:
         constant = Constant(name="apa", value=value)
 
+        assert not constant.is_boolean
+        assert not constant.is_integer
         assert constant.is_float
+        assert not constant.is_string
+
+
+def test_string():
+    for value in ["", "hello"]:
+        constant = Constant(name="apa", value=value)
+
         assert not constant.is_boolean
         assert not constant.is_integer
+        assert not constant.is_float
+        assert constant.is_string
 
 
 def test_invalid_data_type():
     with pytest.raises(ValueError) as exception_info:
-        Constant(name="apa", value="hest")
+        Constant(name="apa", value=Path())
     assert (
         str(exception_info.value)
-        == 'Constant "apa" has invalid data type "<class \'str\'>". Value: "hest"'
+        == 'Constant "apa" has invalid data type "<class \'pathlib.PosixPath\'>". Value: "."'
     )
 
 
 def test_repr():
     # Check that repr is an actual representation, not just "X object at 0xABCDEF"
     assert "apa" in repr(Constant(name="apa", value=0))
```

### Comparing `hdl_registers-3.0.2/hdl_registers/test/unit/test_html_translator.py` & `hdl_registers-3.1.0/hdl_registers/test/unit/test_html_translator.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/test/unit/test_parser.py` & `hdl_registers-3.1.0/hdl_registers/test/unit/test_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -466,38 +466,53 @@
         assert (
             str(exception_info.value)
             == f'Error while parsing bit vector "dummy_bit_vector" in register "dummy_reg" in '
             f'{self.toml_file}: Unknown key "height"'
         )
 
     def test_constants_in_toml(self):
+        # Test all supported data types
         self.create_toml_file_with_extras(
             """
 [constant.data_width]
 
 value = 0xf
 description = "the width"
 
 [constant.apa]
 
 value = 3.14
+
+[constant.hest]
+
+value = true
+
+[constant.zebra]
+
+value = "foo"
 """
         )
 
         register_list = from_toml(self.module_name, self.toml_file)
-        assert len(register_list.constants) == 2
+        assert len(register_list.constants) == 4
 
         assert register_list.constants[0].name == "data_width"
         assert register_list.constants[0].value == 15
         assert register_list.constants[0].description == "the width"
 
         assert register_list.constants[1].name == "apa"
         assert register_list.constants[1].value == 3.14
         assert register_list.constants[1].description == ""
 
+        assert register_list.constants[2].name == "hest"
+        assert register_list.constants[2].value is True
+
+        assert register_list.constants[3].name == "zebra"
+        assert register_list.constants[3].value == "foo"
+
     def test_constant_without_value_should_raise_exception(self):
         self.create_toml_file_with_extras(
             """
 [constant.data_width]
 
 description = "the width"
 """
```

### Comparing `hdl_registers-3.0.2/hdl_registers/test/unit/test_register.py` & `hdl_registers-3.1.0/hdl_registers/test/unit/test_register.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/test/unit/test_register_array.py` & `hdl_registers-3.1.0/hdl_registers/test/unit/test_register_array.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/test/unit/test_register_code_generation.py` & `hdl_registers-3.1.0/hdl_registers/test/unit/test_register_code_generation.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/test/unit/test_register_cpp_generator.py` & `hdl_registers-3.1.0/hdl_registers/test/unit/test_register_cpp_generator.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/test/unit/test_register_field_type.py` & `hdl_registers-3.1.0/hdl_registers/test/unit/test_register_field_type.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/test/unit/test_register_html_generator.py` & `hdl_registers-3.1.0/hdl_registers/test/unit/test_register_html_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -136,14 +136,18 @@
         assert "Registers" in html, html
         assert "dummy_regs" in html, html
 
         # Check that constants are there
         assert constants_text in html, html
         self._check_constant(name="data_width", value=24, html=html)
         self._check_constant(name="decrement", value=-8, html=html)
+        self._check_constant(name="enabled", value="True", html=html)
+        self._check_constant(name="disabled", value="False", html=html)
+        self._check_constant(name="rate", value="3.5", html=html)
+        self._check_constant(name="paragraph", value='"hello there :)"', html=html)
 
         # Test again with no constants
         self.registers.constants = []
         html = self._create_html_page()
 
         # Registers should still be there
         assert "Registers" in html, html
```

### Comparing `hdl_registers-3.0.2/hdl_registers/test/unit/test_register_list.py` & `hdl_registers-3.1.0/hdl_registers/test/unit/test_register_list.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/test/unit/test_register_python_generator.py` & `hdl_registers-3.1.0/hdl_registers/test/unit/test_register_python_generator.py`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/hdl_registers/test/unit/test_register_vhdl_generator.py` & `hdl_registers-3.1.0/hdl_registers/test/unit/test_register_vhdl_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,32 +29,35 @@
 class RegisterConfiguration:
     def __init__(self, module_name, source_toml_file):
         self.register_list = from_toml(module_name=module_name, toml_file=source_toml_file)
 
         self.register_list.add_constant(name="boolean_constant", value=True)
         self.register_list.add_constant(name="integer_constant", value=3)
         self.register_list.add_constant(name="real_constant", value=3.14)
+        self.register_list.add_constant(name="string_constant", value="apa")
 
     def test_vhdl_package(self, output_path, test_registers, test_constants):
         self.register_list.create_vhdl_package(output_path)
         vhdl = read_file(output_path / "test_regs_pkg.vhd")
 
         if test_registers:
             assert "constant test_reg_map : " in vhdl, vhdl
         else:
             assert "constant test_reg_map : " not in vhdl, vhdl
 
         if test_constants:
             assert "constant test_constant_boolean_constant : boolean := true;" in vhdl, vhdl
             assert "constant test_constant_integer_constant : integer := 3;" in vhdl, vhdl
             assert "constant test_constant_real_constant : real := 3.14;" in vhdl, vhdl
+            assert 'constant test_constant_string_constant : string := "apa";' in vhdl, vhdl
         else:
             assert "boolean_constant" not in vhdl, vhdl
             assert "integer_constant" not in vhdl, vhdl
             assert "real_constant" not in vhdl, vhdl
+            assert "string_constant" not in vhdl, vhdl
 
 
 @pytest.fixture
 def register_configuration():
     return RegisterConfiguration("test", HDL_REGISTERS_TEST / "regs_test.toml")
```

### Comparing `hdl_registers-3.0.2/hdl_registers.egg-info/PKG-INFO` & `hdl_registers-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: hdl-registers
-Version: 3.0.2
-Summary: An open-source HDL register generator fast enough to run in real time.
+Name: hdl_registers
+Version: 3.1.0
+Summary: An open-source HDL register generator fast enough to run in real time
 Home-page: https://hdl-registers.com
 Author: Lukas Vik
 Author-email: 2767848-LukasVik@users.noreply.gitlab.com
 License: BSD 3-Clause License
 Project-URL: Documentation, https://hdl-registers.com/
 Project-URL: Changelog, https://hdl-registers.com/release_notes.html
 Project-URL: Source, https://gitlab.com/hdl_registers/hdl_registers
@@ -18,17 +18,14 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 
-About hdl_registers
-===================
-
 |pic_website| |pic_gitlab| |pic_gitter| |pic_pip_install| |pic_license| |pic_python_line_coverage|
 
 .. |pic_website| image:: https://hdl-registers.com/badges/website.svg
   :alt: Website
   :target: https://hdl-registers.com
 
 .. |pic_gitlab| image:: https://hdl-registers.com/badges/gitlab.svg
```

### Comparing `hdl_registers-3.0.2/hdl_registers.egg-info/SOURCES.txt` & `hdl_registers-3.1.0/hdl_registers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/pyproject.toml` & `hdl_registers-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdl_registers-3.0.2/setup.py` & `hdl_registers-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # Do PYTHONPATH insert() instead of append() to prefer any local repo checkout over any pip install
 REPO_ROOT = Path(__file__).parent.resolve()
 sys.path.insert(0, str(REPO_ROOT))
 
 # First party libraries
 import hdl_registers
-from hdl_registers.about import get_pypi_slogan, get_readme_rst
+from hdl_registers.about import get_readme_rst, get_short_slogan
 
 # Duplicated from tsfpga/__init__.py since setup.py may not depend on tsfpga
 DEFAULT_FILE_ENCODING = "utf-8"
 REQUIREMENTS_TXT = hdl_registers.HDL_REGISTERS_PATH / "requirements.txt"
 REQUIREMENTS_DEVELOP_TXT = hdl_registers.HDL_REGISTERS_PATH / "requirements_develop.txt"
 
 
@@ -47,15 +47,15 @@
     You should see all the files in "/usr/local/lib/python3.8/site-packages/hdl_registers".
     Test to run "python -m pip uninstall hdl_registers" and see that it passes. Check the output to
     see that there are not package files installed in weird locations (such as /usr/local/lib/).
     """
     setup(
         name="hdl_registers",
         version=hdl_registers.__version__,
-        description=get_pypi_slogan(),
+        description=get_short_slogan(),
         long_description=get_readme_rst(include_extra_for_pypi=True),
         long_description_content_type="text/x-rst",
         license="BSD 3-Clause License",
         author="Lukas Vik",
         author_email="2767848-LukasVik@users.noreply.gitlab.com",
         url="https://hdl-registers.com",
         project_urls={
```

