# Comparing `tmp/gb-0.1.1.tar.gz` & `tmp/gb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gb-0.1.1.tar", max compression
+gzip compressed data, was "gb-0.1.2.tar", max compression
```

## Comparing `gb-0.1.1.tar` & `gb-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1075 2022-07-15 23:24:03.752873 gb-0.1.1/LICENSE
--rw-r--r--   0        0        0     2008 2023-04-25 11:55:09.016556 gb-0.1.1/README.md
--rw-r--r--   0        0        0        0 2022-07-15 23:24:03.756873 gb-0.1.1/gb/__init__.py
--rw-r--r--   0        0        0       78 2022-07-15 23:24:03.756873 gb-0.1.1/gb/__main__.py
--rw-r--r--   0        0        0     2143 2023-04-25 12:02:59.154436 gb-0.1.1/gb/command.py
--rw-r--r--   0        0        0      643 2022-07-15 23:24:03.756873 gb-0.1.1/gb/document.py
--rw-r--r--   0        0        0     1290 2022-07-15 23:24:03.756873 gb-0.1.1/gb/entry.py
--rw-r--r--   0        0        0      413 2022-07-15 23:24:03.757873 gb-0.1.1/gb/magic.py
--rw-r--r--   0        0        0     2127 2022-07-15 23:24:03.757873 gb-0.1.1/gb/mode.py
--rw-r--r--   0        0        0      669 2022-07-15 23:24:03.757873 gb-0.1.1/gb/protocol.py
--rw-r--r--   0        0        0      818 2022-07-15 23:24:03.757873 gb-0.1.1/gb/safe.py
--rw-r--r--   0        0        0     3489 2022-07-15 23:24:03.757873 gb-0.1.1/gb/server.py
--rw-r--r--   0        0        0     1069 2023-04-25 12:09:53.126534 gb-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 gb-0.1.1/setup.py
--rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 gb-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2022-07-15 23:24:03.752873 gb-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2008 2023-04-25 11:55:09.016556 gb-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2022-07-15 23:24:03.756873 gb-0.1.2/gb/__init__.py
+-rw-r--r--   0        0        0       78 2022-07-15 23:24:03.756873 gb-0.1.2/gb/__main__.py
+-rw-r--r--   0        0        0     2143 2023-04-25 12:02:59.154436 gb-0.1.2/gb/command.py
+-rw-r--r--   0        0        0      643 2022-07-15 23:24:03.756873 gb-0.1.2/gb/document.py
+-rw-r--r--   0        0        0     1290 2022-07-15 23:24:03.756873 gb-0.1.2/gb/entry.py
+-rw-r--r--   0        0        0      413 2022-07-15 23:24:03.757873 gb-0.1.2/gb/magic.py
+-rw-r--r--   0        0        0     2127 2022-07-15 23:24:03.757873 gb-0.1.2/gb/mode.py
+-rw-r--r--   0        0        0      669 2022-07-15 23:24:03.757873 gb-0.1.2/gb/protocol.py
+-rw-r--r--   0        0        0      818 2022-07-15 23:24:03.757873 gb-0.1.2/gb/safe.py
+-rw-r--r--   0        0        0     3489 2022-07-15 23:24:03.757873 gb-0.1.2/gb/server.py
+-rw-r--r--   0        0        0     1080 2023-04-25 12:17:06.881206 gb-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 gb-0.1.2/setup.py
+-rw-r--r--   0        0        0     2807 1970-01-01 00:00:00.000000 gb-0.1.2/PKG-INFO
```

### Comparing `gb-0.1.1/LICENSE` & `gb-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gb-0.1.1/README.md` & `gb-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gb-0.1.1/gb/command.py` & `gb-0.1.2/gb/command.py`

 * *Files identical despite different names*

### Comparing `gb-0.1.1/gb/document.py` & `gb-0.1.2/gb/document.py`

 * *Files identical despite different names*

### Comparing `gb-0.1.1/gb/entry.py` & `gb-0.1.2/gb/entry.py`

 * *Files identical despite different names*

### Comparing `gb-0.1.1/gb/mode.py` & `gb-0.1.2/gb/mode.py`

 * *Files identical despite different names*

### Comparing `gb-0.1.1/gb/protocol.py` & `gb-0.1.2/gb/protocol.py`

 * *Files identical despite different names*

### Comparing `gb-0.1.1/gb/safe.py` & `gb-0.1.2/gb/safe.py`

 * *Files identical despite different names*

### Comparing `gb-0.1.1/gb/server.py` & `gb-0.1.2/gb/server.py`

 * *Files identical despite different names*

### Comparing `gb-0.1.1/pyproject.toml` & `gb-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "gb"
-version = "0.1.1"
+version = "0.1.2"
 description = "A Python gopher server."
-authors = ["supakeen <cmdr@supakeen.com>"]
+authors = ["Simon de Vlieger <cmdr@supakeen.com>"]
 license = "MIT"
 readme = "README.md"
-keywords = ["pastebin"]
-repository = "https://github.com/supakeen/pinnwand"
+keywords = ["gopher", "server"]
+repository = "https://src.tty.cat/supakeen/gb"
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `gb-0.1.1/setup.py` & `gb-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 ['click>=8.0,<9.0', 'python-magic>=0.4.27,<0.5.0', 'tornado>=6.0,<7.0']
 
 entry_points = \
 {'console_scripts': ['gb = gb.__main__:main']}
 
 setup_kwargs = {
     'name': 'gb',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A Python gopher server.',
     'long_description': '![gb logo, a gopher in a ball](https://src.tty.cat/supakeen/gb/raw/branch/master/doc/_static/logo-doc.png)\n\n# gb\n\n![rtd badge](https://readthedocs.org/projects/gb/badge/?version=latest) ![license badge](https://gb.readthedocs.io/en/latest/_static/license.svg) ![black badge](https://img.shields.io/badge/code%20style-black-000000.svg)\n\n## About\n\n`gb` or gopherball is a gopher server written in Python with the main goals of\nease of use and integration. The name gopherball is inspired by a recurring\ntheme in the Calvin & Hobbes comicbooks and a tongue in cheek reference of an\nalternative to the World Wide Web as we know it today.\n\n## Examples\nQuick examples to get you running.\n\n`gb --mode=implicit .` will start a gopher server on `127.0.0.1` port `7070` serving\na recursive index of files starting from the current directory.\n\n`gb --mode=implicit --magic .` will start `gb` in magic-mode on `127.0.0.1` port\n`7070`. Magic mode will make `gb` guess at filetypes.\n\n`gb --mode=implicit --host="127.1.1.1" --port 1025 .` will start `gb` in implicit\nmode on the chosen ip and port. Note that using ports under 1024 requires\nsuperuser permissions!\n\n## Technology\n`gb` is written with the help of Python 3.9 and higher and the Tornado\nframework for its networking.\n\n## Modes\n`gb` has one main mode of operation that is commonly used. More modes are\nplanned for the future.\n\n### implicit\nImplicit mode serves a directory recursively. Indexes are automatically\ngenerated and text files are served to the client. Data files are also\nsupported.\n\n## Magic\n`gb` will serve all non-directories as type 9 files, these are non-readable\nfiles and most clients will prompt for download. Turning on magic with\n`--magic` will let `gb` try to determine the correct filetypes.\n\n## Contributing\nThe source code for `gb` lives on my Gitea where you can also submit issues and\npull requests. It mostly needs help by people with the ability to test in\nvarious clients and libraries that might still support the gopher protocol.\n',
-    'author': 'supakeen',
+    'author': 'Simon de Vlieger',
     'author_email': 'cmdr@supakeen.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://github.com/supakeen/pinnwand',
+    'url': 'https://src.tty.cat/supakeen/gb',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.9,<4',
 }
```

### Comparing `gb-0.1.1/PKG-INFO` & `gb-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: gb
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python gopher server.
-Home-page: https://github.com/supakeen/pinnwand
+Home-page: https://src.tty.cat/supakeen/gb
 License: MIT
-Keywords: pastebin
-Author: supakeen
+Keywords: gopher,server
+Author: Simon de Vlieger
 Author-email: cmdr@supakeen.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: click (>=8.0,<9.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0)
 Requires-Dist: tornado (>=6.0,<7.0)
-Project-URL: Repository, https://github.com/supakeen/pinnwand
+Project-URL: Repository, https://src.tty.cat/supakeen/gb
 Description-Content-Type: text/markdown
 
 ![gb logo, a gopher in a ball](https://src.tty.cat/supakeen/gb/raw/branch/master/doc/_static/logo-doc.png)
 
 # gb
 
 ![rtd badge](https://readthedocs.org/projects/gb/badge/?version=latest) ![license badge](https://gb.readthedocs.io/en/latest/_static/license.svg) ![black badge](https://img.shields.io/badge/code%20style-black-000000.svg)
```

