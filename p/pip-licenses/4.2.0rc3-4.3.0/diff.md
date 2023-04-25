# Comparing `tmp/pip-licenses-4.2.0rc3.tar.gz` & `tmp/pip-licenses-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pip-licenses-4.2.0rc3.tar", last modified: Wed Apr 12 10:00:41 2023, max compression
+gzip compressed data, was "dist/pip-licenses-4.3.0.tar", last modified: Tue Apr 25 08:14:50 2023, max compression
```

## Comparing `pip-licenses-4.2.0rc3.tar` & `pip-licenses-4.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-04-12 10:00:41.622574 pip-licenses-4.2.0rc3/
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)     5294 2023-04-12 09:58:29.000000 pip-licenses-4.2.0rc3/CHANGELOG.md
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)     1063 2020-12-06 15:11:59.000000 pip-licenses-4.2.0rc3/LICENSE
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)      129 2022-12-04 03:57:54.000000 pip-licenses-4.2.0rc3/MANIFEST.in
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)    30589 2023-04-12 10:00:41.622574 pip-licenses-4.2.0rc3/PKG-INFO
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)    21411 2023-04-12 09:58:26.000000 pip-licenses-4.2.0rc3/README.md
-drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-04-12 10:00:41.622574 pip-licenses-4.2.0rc3/pip_licenses.egg-info/
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)    30589 2023-04-12 10:00:41.000000 pip-licenses-4.2.0rc3/pip_licenses.egg-info/PKG-INFO
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)      361 2023-04-12 10:00:41.000000 pip-licenses-4.2.0rc3/pip_licenses.egg-info/SOURCES.txt
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)        1 2023-04-12 10:00:41.000000 pip-licenses-4.2.0rc3/pip_licenses.egg-info/dependency_links.txt
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)       51 2023-04-12 10:00:41.000000 pip-licenses-4.2.0rc3/pip_licenses.egg-info/entry_points.txt
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)       85 2023-04-12 10:00:41.000000 pip-licenses-4.2.0rc3/pip_licenses.egg-info/requires.txt
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)       12 2023-04-12 10:00:41.000000 pip-licenses-4.2.0rc3/pip_licenses.egg-info/top_level.txt
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)    32432 2023-04-12 09:58:40.000000 pip-licenses-4.2.0rc3/piplicenses.py
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)        0 2022-12-04 03:57:54.000000 pip-licenses-4.2.0rc3/py.typed
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)     1367 2023-04-12 10:00:41.622574 pip-licenses-4.2.0rc3/setup.cfg
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)     2347 2022-12-04 03:57:54.000000 pip-licenses-4.2.0rc3/setup.py
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)    34122 2023-04-12 09:58:29.000000 pip-licenses-4.2.0rc3/test_piplicenses.py
-drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-04-12 10:00:41.622574 pip-licenses-4.2.0rc3/tests/
-drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-04-12 10:00:41.622574 pip-licenses-4.2.0rc3/tests/fixtures/
--rw-r--r--   0 raimon49  (1000) raimon49  (1000)       16 2020-12-06 15:11:59.000000 pip-licenses-4.2.0rc3/tests/fixtures/unicode_characters.txt
+drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-04-25 08:14:50.275305 pip-licenses-4.3.0/
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)     5344 2023-04-25 08:08:23.000000 pip-licenses-4.3.0/CHANGELOG.md
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)     1063 2020-12-06 15:11:59.000000 pip-licenses-4.3.0/LICENSE
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)      129 2022-12-04 03:57:54.000000 pip-licenses-4.3.0/MANIFEST.in
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)    30934 2023-04-25 08:14:50.275305 pip-licenses-4.3.0/PKG-INFO
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)    21661 2023-04-25 08:07:16.000000 pip-licenses-4.3.0/README.md
+drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-04-25 08:14:50.275305 pip-licenses-4.3.0/pip_licenses.egg-info/
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)    30934 2023-04-25 08:14:50.000000 pip-licenses-4.3.0/pip_licenses.egg-info/PKG-INFO
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)      361 2023-04-25 08:14:50.000000 pip-licenses-4.3.0/pip_licenses.egg-info/SOURCES.txt
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)        1 2023-04-25 08:14:50.000000 pip-licenses-4.3.0/pip_licenses.egg-info/dependency_links.txt
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)       51 2023-04-25 08:14:50.000000 pip-licenses-4.3.0/pip_licenses.egg-info/entry_points.txt
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)       85 2023-04-25 08:14:50.000000 pip-licenses-4.3.0/pip_licenses.egg-info/requires.txt
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)       12 2023-04-25 08:14:50.000000 pip-licenses-4.3.0/pip_licenses.egg-info/top_level.txt
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)    32669 2023-04-25 08:07:52.000000 pip-licenses-4.3.0/piplicenses.py
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)        0 2022-12-04 03:57:54.000000 pip-licenses-4.3.0/py.typed
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)     1367 2023-04-25 08:14:50.275305 pip-licenses-4.3.0/setup.cfg
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)     2347 2022-12-04 03:57:54.000000 pip-licenses-4.3.0/setup.py
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)    34555 2023-04-25 08:07:16.000000 pip-licenses-4.3.0/test_piplicenses.py
+drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-04-25 08:14:50.265305 pip-licenses-4.3.0/tests/
+drwxr-xr-x   0 raimon49  (1000) raimon49  (1000)        0 2023-04-25 08:14:50.275305 pip-licenses-4.3.0/tests/fixtures/
+-rw-r--r--   0 raimon49  (1000) raimon49  (1000)       16 2020-12-06 15:11:59.000000 pip-licenses-4.3.0/tests/fixtures/unicode_characters.txt
```

### Comparing `pip-licenses-4.2.0rc3/CHANGELOG.md` & `pip-licenses-4.3.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 ## CHANGELOG
 
+### 4.3.0
+
+* Implement new option `--no-version`
+
 ### 4.2.0
 
 * Implement new option `--with-maintainers`
 * Implement new option `--python`
 * Allow version spec in `--ignore-packages` parameters
 * When the `Author` field is `UNKNOWN`, the output is automatically completed from `Author-email`
 * When the `home-page` field is `UNKNOWN`, the output is automatically completed from `Project-URL`
```

### Comparing `pip-licenses-4.2.0rc3/LICENSE` & `pip-licenses-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pip-licenses-4.2.0rc3/PKG-INFO` & `pip-licenses-4.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-licenses
-Version: 4.2.0rc3
+Version: 4.3.0
 Summary: Dump the software license list of Python packages installed with pip.
 Home-page: https://github.com/raimon49/pip-licenses
 Author: raimon
 Author-email: raimon49@hotmail.com
 License: MIT
 Project-URL: Releases, https://github.com/raimon49/pip-licenses/releases
 Project-URL: Issues, https://github.com/raimon49/pip-licenses/issues
@@ -66,14 +66,15 @@
    -  `Format options <#format-options>`__
 
       -  `Option: with-system <#option-with-system>`__
       -  `Option: with-authors <#option-with-authors>`__
       -  `Option: with-maintainers <#option-with-maintainers>`__
       -  `Option: with-urls <#option-with-urls>`__
       -  `Option: with-description <#option-with-description>`__
+      -  `Option: no-version <#option-no-version>`__
       -  `Option: with-license-file <#option-with-license-file>`__
       -  `Option: filter-strings <#option-filter-strings>`__
       -  `Option: filter-code-page <#option-filter-code-page>`__
 
    -  `Verify options <#verify-options>`__
 
       -  `Option: fail-on <#option-fail-on>`__
@@ -586,14 +587,27 @@
 .. code:: bash
 
    (venv) $ pip-licenses --with-description
     Name    Version  License  Description
     Django  2.0.2    BSD      A high-level Python Web framework that encourages rapid development and clean, pragmatic design.
     pytz    2017.3   MIT      World timezone definitions, modern and historical
 
+Option: no-version
+^^^^^^^^^^^^^^^^^^
+
+When executed with the ``--no-version`` option, output without the
+version number.
+
+.. code:: bash
+
+   (venv) $ pip-licenses --no-version
+    Name    License
+    Django  BSD
+    pytz    MIT
+
 Option: with-license-file
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 
 When executed with the ``--with-license-file`` option, output the
 location of the package's license file on disk and the full contents of
 that file. Due to the length of these fields, this option is best paired
 with ``--format=json``.
@@ -811,14 +825,21 @@
 .. |PyPI - Downloads| image:: https://img.shields.io/pypi/dm/pip-licenses
    :target: https://pypistats.org/packages/pip-licenses
 
 
 CHANGELOG
 ---------
 
+.. _430:
+
+4.3.0
+~~~~~
+
+-  Implement new option ``--no-version``
+
 .. _420:
 
 4.2.0
 ~~~~~
 
 -  Implement new option ``--with-maintainers``
 -  Implement new option ``--python``
```

### Comparing `pip-licenses-4.2.0rc3/README.md` & `pip-licenses-4.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         * [Option: packages](#option-packages)
     * [Format options](#format-options)
         * [Option: with\-system](#option-with-system)
         * [Option: with\-authors](#option-with-authors)
         * [Option: with\-maintainers](#option-with-maintainers)
         * [Option: with\-urls](#option-with-urls)
         * [Option: with\-description](#option-with-description)
+        * [Option: no\-version](#option-no-version)
         * [Option: with\-license\-file](#option-with-license-file)
         * [Option: filter\-strings](#option-filter-strings)
         * [Option: filter\-code\-page](#option-filter-code-page)
     * [Verify options](#verify-options)
         * [Option: fail\-on](#option-fail-on)
         * [Option: allow\-only](#option-allow-only)
     * [More Information](#more-information)
@@ -454,14 +455,25 @@
 ```bash
 (venv) $ pip-licenses --with-description
  Name    Version  License  Description
  Django  2.0.2    BSD      A high-level Python Web framework that encourages rapid development and clean, pragmatic design.
  pytz    2017.3   MIT      World timezone definitions, modern and historical
 ```
 
+#### Option: no-version
+
+When executed with the `--no-version` option, output without the version number.
+
+```bash
+(venv) $ pip-licenses --no-version
+ Name    License
+ Django  BSD
+ pytz    MIT
+```
+
 #### Option: with-license-file
 
 When executed with the `--with-license-file` option, output the location of the package's license file on disk and the full contents of that file. Due to the length of these fields, this option is best paired with `--format=json`.
 
 If you also want to output the file `NOTICE` distributed under Apache License etc., specify the `--with-notice-file` option additionally.
 
 **Note:** If you want to keep the license file path secret, specify `--no-license-path` option together.
```

### Comparing `pip-licenses-4.2.0rc3/pip_licenses.egg-info/PKG-INFO` & `pip-licenses-4.3.0/pip_licenses.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-licenses
-Version: 4.2.0rc3
+Version: 4.3.0
 Summary: Dump the software license list of Python packages installed with pip.
 Home-page: https://github.com/raimon49/pip-licenses
 Author: raimon
 Author-email: raimon49@hotmail.com
 License: MIT
 Project-URL: Releases, https://github.com/raimon49/pip-licenses/releases
 Project-URL: Issues, https://github.com/raimon49/pip-licenses/issues
@@ -66,14 +66,15 @@
    -  `Format options <#format-options>`__
 
       -  `Option: with-system <#option-with-system>`__
       -  `Option: with-authors <#option-with-authors>`__
       -  `Option: with-maintainers <#option-with-maintainers>`__
       -  `Option: with-urls <#option-with-urls>`__
       -  `Option: with-description <#option-with-description>`__
+      -  `Option: no-version <#option-no-version>`__
       -  `Option: with-license-file <#option-with-license-file>`__
       -  `Option: filter-strings <#option-filter-strings>`__
       -  `Option: filter-code-page <#option-filter-code-page>`__
 
    -  `Verify options <#verify-options>`__
 
       -  `Option: fail-on <#option-fail-on>`__
@@ -586,14 +587,27 @@
 .. code:: bash
 
    (venv) $ pip-licenses --with-description
     Name    Version  License  Description
     Django  2.0.2    BSD      A high-level Python Web framework that encourages rapid development and clean, pragmatic design.
     pytz    2017.3   MIT      World timezone definitions, modern and historical
 
+Option: no-version
+^^^^^^^^^^^^^^^^^^
+
+When executed with the ``--no-version`` option, output without the
+version number.
+
+.. code:: bash
+
+   (venv) $ pip-licenses --no-version
+    Name    License
+    Django  BSD
+    pytz    MIT
+
 Option: with-license-file
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 
 When executed with the ``--with-license-file`` option, output the
 location of the package's license file on disk and the full contents of
 that file. Due to the length of these fields, this option is best paired
 with ``--format=json``.
@@ -811,14 +825,21 @@
 .. |PyPI - Downloads| image:: https://img.shields.io/pypi/dm/pip-licenses
    :target: https://pypistats.org/packages/pip-licenses
 
 
 CHANGELOG
 ---------
 
+.. _430:
+
+4.3.0
+~~~~~
+
+-  Implement new option ``--no-version``
+
 .. _420:
 
 4.2.0
 ~~~~~
 
 -  Implement new option ``--with-maintainers``
 -  Implement new option ``--python``
```

### Comparing `pip-licenses-4.2.0rc3/piplicenses.py` & `pip-licenses-4.3.0/piplicenses.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     from email.message import Message
     from typing import Callable, Dict, Iterator, Optional, Sequence
 
 
 open = open  # allow monkey patching
 
 __pkgname__ = "pip-licenses"
-__version__ = "4.2.0rc3"
+__version__ = "4.3.0"
 __author__ = "raimon"
 __license__ = "MIT"
 __summary__ = (
     "Dump the software license list of Python packages installed with pip."
 )
 __url__ = "https://github.com/raimon49/pip-licenses"
 
@@ -590,14 +590,17 @@
 
     if args.with_urls:
         output_fields.append("URL")
 
     if args.with_description:
         output_fields.append("Description")
 
+    if args.no_version:
+        output_fields.remove("Version")
+
     if args.with_license_file:
         if not args.no_license_path:
             output_fields.append("LicenseFile")
 
         output_fields.append("LicenseText")
 
         if args.with_notice_file:
@@ -963,14 +966,21 @@
         "-d",
         "--with-description",
         action="store_true",
         default=False,
         help="dump with short package description",
     )
     format_options.add_argument(
+        "-nv",
+        "--no-version",
+        action="store_true",
+        default=False,
+        help="dump without package version",
+    )
+    format_options.add_argument(
         "-l",
         "--with-license-file",
         action="store_true",
         default=False,
         help="dump with location of license file and "
         "contents, most useful with JSON output",
     )
```

### Comparing `pip-licenses-4.2.0rc3/setup.cfg` & `pip-licenses-4.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pip-licenses-4.2.0rc3/setup.py` & `pip-licenses-4.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `pip-licenses-4.2.0rc3/test_piplicenses.py` & `pip-licenses-4.3.0/test_piplicenses.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,14 +340,25 @@
         output_fields = get_output_fields(args)
         self.assertNotEqual(output_fields, list(DEFAULT_OUTPUT_FIELDS))
         self.assertIn("Description", output_fields)
 
         output_string = create_output_string(args)
         self.assertIn("Description", output_string)
 
+    def test_without_version(self) -> None:
+        without_version_args = ["--no-version"]
+        args = self.parser.parse_args(without_version_args)
+
+        output_fields = get_output_fields(args)
+        self.assertNotEqual(output_fields, list(DEFAULT_OUTPUT_FIELDS))
+        self.assertNotIn("Version", output_fields)
+
+        output_string = create_output_string(args)
+        self.assertNotIn("Version", output_string)
+
     def test_with_license_file(self) -> None:
         with_license_file_args = ["--with-license-file"]
         args = self.parser.parse_args(with_license_file_args)
 
         output_fields = get_output_fields(args)
         self.assertNotEqual(output_fields, list(DEFAULT_OUTPUT_FIELDS))
         self.assertIn("LicenseFile", output_fields)
@@ -826,15 +837,15 @@
     with tempfile.TemporaryDirectory() as target_dir_path:
         venv_builder = TempEnvBuild(with_pip=True)
         venv_builder.create(str(target_dir_path))
         python_exec = venv_builder.context.env_exe
         python_arg = f"--python={python_exec}"
         args = create_parser().parse_args([python_arg, "-s", "-f=json"])
         pkgs = get_packages(args)
-        package_names = sorted(p["name"] for p in pkgs)
+        package_names = sorted(set(p["name"] for p in pkgs))
         print(package_names)
 
     assert package_names == ["pip", "setuptools"]
 
 
 def test_fail_on(monkeypatch) -> None:
     licenses = ("MIT license",)
```

