# Comparing `tmp/space_rocks-1.7.6.tar.gz` & `tmp/space_rocks-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space_rocks-1.7.6.tar", max compression
+gzip compressed data, was "space_rocks-1.7.7.tar", max compression
```

## Comparing `space_rocks-1.7.6.tar` & `space_rocks-1.7.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1067 2023-04-21 07:53:47.207007 space_rocks-1.7.6/LICENSE
--rw-r--r--   0        0        0     1731 2023-04-21 07:53:47.207007 space_rocks-1.7.6/README.md
--rw-r--r--   0        0        0     1552 2023-04-21 08:05:18.107013 space_rocks-1.7.6/pyproject.toml
--rw-r--r--   0        0        0      450 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/__init__.py
--rw-r--r--   0        0        0     4886 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/cache.py
--rw-r--r--   0        0        0    11459 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/cli.py
--rw-r--r--   0        0        0     7078 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/config.py
--rw-r--r--   0        0        0    39456 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/core.py
--rw-r--r--   0        0        0    32930 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/datacloud.py
--rw-r--r--   0        0        0    13116 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/index.py
--rw-r--r--   0        0        0      982 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/logging.py
--rw-r--r--   0        0        0     3765 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/metadata.py
--rw-r--r--   0        0        0     6300 2023-02-19 15:02:48.465877 space_rocks-1.7.6/rocks/plots.py
--rw-r--r--   0        0        0    12653 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/resolve.py
--rw-r--r--   0        0        0    12231 2023-04-21 07:53:47.215006 space_rocks-1.7.6/rocks/ssodnet.py
--rw-r--r--   0        0        0     3161 1970-01-01 00:00:00.000000 space_rocks-1.7.6/setup.py
--rw-r--r--   0        0        0     3304 1970-01-01 00:00:00.000000 space_rocks-1.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-21 07:53:47.207007 space_rocks-1.7.7/LICENSE
+-rw-r--r--   0        0        0     1731 2023-04-21 07:53:47.207007 space_rocks-1.7.7/README.md
+-rw-r--r--   0        0        0     1419 2023-04-24 10:12:17.117344 space_rocks-1.7.7/pyproject.toml
+-rw-r--r--   0        0        0      450 2023-04-24 08:24:01.013287 space_rocks-1.7.7/rocks/__init__.py
+-rw-r--r--   0        0        0     4886 2023-04-21 07:53:47.215006 space_rocks-1.7.7/rocks/cache.py
+-rw-r--r--   0        0        0    11492 2023-04-24 14:38:10.881484 space_rocks-1.7.7/rocks/cli.py
+-rw-r--r--   0        0        0     7078 2023-04-21 07:53:47.215006 space_rocks-1.7.7/rocks/config.py
+-rw-r--r--   0        0        0    39130 2023-04-24 14:46:13.273488 space_rocks-1.7.7/rocks/core.py
+-rw-r--r--   0        0        0    32930 2023-04-21 07:53:47.215006 space_rocks-1.7.7/rocks/datacloud.py
+-rw-r--r--   0        0        0    13082 2023-04-25 07:26:58.446013 space_rocks-1.7.7/rocks/index.py
+-rw-r--r--   0        0        0      982 2023-04-21 07:53:47.215006 space_rocks-1.7.7/rocks/logging.py
+-rw-r--r--   0        0        0     3765 2023-04-21 07:53:47.215006 space_rocks-1.7.7/rocks/metadata.py
+-rw-r--r--   0        0        0     6300 2023-02-19 15:02:48.465877 space_rocks-1.7.7/rocks/plots.py
+-rw-r--r--   0        0        0    12799 2023-04-24 08:24:01.017288 space_rocks-1.7.7/rocks/resolve.py
+-rw-r--r--   0        0        0    12231 2023-04-21 07:53:47.215006 space_rocks-1.7.7/rocks/ssodnet.py
+-rw-r--r--   0        0        0     3026 1970-01-01 00:00:00.000000 space_rocks-1.7.7/setup.py
+-rw-r--r--   0        0        0     3148 1970-01-01 00:00:00.000000 space_rocks-1.7.7/PKG-INFO
```

### Comparing `space_rocks-1.7.6/LICENSE` & `space_rocks-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.6/README.md` & `space_rocks-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.6/pyproject.toml` & `space_rocks-1.7.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 [tool.poetry]
 name = "space-rocks"
-version = "1.7.6"
+version = "1.7.7"
 description = "Python client for SsODNet data access."
 authors = ["Max Mahlke <max.mahlke@oca.eu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://rocks.readthedocs.io/en/latest/"
 documentation = "https://rocks.readthedocs.io/en/latest/"
 repository = "https://github.com/maxmahlke/rocks.git"
 packages = [{'include' = 'rocks'}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.11"
-sphinx = {version = "^5", optional = true}
-sphinx-hoverxref = {version = "*", optional = true}
-jinja2 = {version = "<3.1", optional = true}
-pydantic = "^1.8.2"
-numpy = "^1.21.2"
-matplotlib = "^3.4.3"
+numpy = ">=1.21"
+matplotlib = ">=3.4.3"
 aiohttp = "^3.7.4"
 cchardet = "^2.1.7"
 aiodns = "^3.0.0"
-pandas = "^1.3.2"
-rich = "^12"
-click = "^8.0.1"
+pandas = ">=1.3.5"
+pydantic = "^1.8.2"
+rich = ">=12.2.0"
+click = ">=8.1.2"
 nest-asyncio = "^1.5.1"
 requests = "^2.26.0"
 Levenshtein = "^0.16.0"
 furo = "^2022.9.15"
 sphinx-copybutton = "^0.5.0"
 sphinx_design = "^0.3.0"
 bs4 = "^0.0.1"
```

### Comparing `space_rocks-1.7.6/rocks/cache.py` & `space_rocks-1.7.7/rocks/cache.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.6/rocks/cli.py` & `space_rocks-1.7.7/rocks/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,15 @@
             choices=["0", "1"],
             show_choices=False,
             default="1",
         )
 
         if decision == "1":
             click.echo()
+            index._build_index()
     if update:
         index._build_index()
 
 
 @cli_rocks.command()
 @click.argument("id_", nargs=-1)
 def who(id_):
```

### Comparing `space_rocks-1.7.6/rocks/config.py` & `space_rocks-1.7.7/rocks/config.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.6/rocks/core.py` & `space_rocks-1.7.7/rocks/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import datetime as dt
 import keyword
 from typing import List, Generator
 
 import numpy as np
 import pandas as pd
 import pydantic
-import rich
 
 from rocks import config
 from rocks import datacloud as dc
 from rocks.logging import logger
 from rocks import metadata
 from rocks import resolve
 from rocks import ssodnet
@@ -915,19 +914,14 @@
                 location_list = error["loc"][:-1]
 
                 if any(
                     property_ in location_list for property_ in ["taxonomy", "spin"]
                 ):
                     for property_ in ["taxonomy", "spin"]:
                         if property_ in location_list:
-                            # these are lists instead of dicts and the indices are flipped
-                            # eg taxonomy bibref 0 becomes taxonomy 0 bibref
-                            idx = location_list.index(property_)
-                            entry, idx_list = location_list[idx + 1 : idx + 3]
-
                             try:
                                 del ssocard["parameters"]["physical"][property_]
                             except KeyError:
                                 pass
                 else:
                     for location in error["loc"][:-1]:
                         offending_part = offending_part[location]
@@ -1062,17 +1056,17 @@
                     if "spin" in error["loc"]:
                         error["loc"] = ("parameters", "physical", "spin")
                         break
                 except TypeError:
                     break
 
             logger.debug(
-                f"object:{id_}[/] Invalid value for {'.'.join([str(e) for e in error['loc']])}"
-                f"\nPassed value: {value}"
+                f"{id_}: Invalid value for {'.'.join([str(e) for e in error['loc']])}"
             )
+            logger.debug(f"Passed value: {value}")
 
 
 def rocks_(ids, datacloud=None, progress=False, on_404="warning"):
     """Create multiple Rock instances.
 
     Parameters
     ----------
```

### Comparing `space_rocks-1.7.6/rocks/datacloud.py` & `space_rocks-1.7.7/rocks/datacloud.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.6/rocks/index.py` & `space_rocks-1.7.7/rocks/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -462,17 +462,16 @@
     | '__/ _ \ / __| |/ / __|
     | | | (_) | (__|   <\__ \
     |_|  \___/ \___|_|\_\___/
 
     version: {__version__}
     cache:   {config.PATH_CACHE}
 
-    It looks like this is the first time you run [green]rocks[/green].
-    Some metadata is required to be present in the cache directory.
-    [green]rocks[/green] will download it now.
+    It looks like this is the first time you run [green]rocks[/green]. Some
+    metadata is required to run. [green]rocks[/green] will download it now.
     """
 
     # Cache directory is missing: first time running rocks
     if not config.PATH_CACHE.is_dir():
         rich.print(GREETING)
         config.PATH_CACHE.mkdir(parents=True)
```

### Comparing `space_rocks-1.7.6/rocks/logging.py` & `space_rocks-1.7.7/rocks/logging.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.6/rocks/metadata.py` & `space_rocks-1.7.7/rocks/metadata.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.6/rocks/plots.py` & `space_rocks-1.7.7/rocks/plots.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.6/rocks/resolve.py` & `space_rocks-1.7.7/rocks/resolve.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,15 +231,19 @@
 
     try:
         id_ = int(float(id_))
         return id_
     except ValueError:
         pass
 
-    # Name or designation
+    # -> Name or designation
+
+    # Strip leading and trailing whitespace
+    id_ = id_.strip()
+
     return id_.replace("_(Asteroid)", "").replace("_", "").replace(" ", "").lower()
 
 
 def _standardize_id_for_quaero(id_):
     """Try to infer id_ type and re-format if necessary to ensure
     successful remote lookup.
 
@@ -253,14 +257,17 @@
     str, int, None
         The standardized name, designation, or number. None if id_ is NaN or None.
     """
     if isinstance(id_, (int, float)):
         return int(id_)
 
     elif isinstance(id_, str):
+        # Strip leading and trailing whitespace
+        id_ = id_.strip()
+
         # String id_. Perform some regex tests to make sure it's well formatted
 
         # Asteroid number
         try:
             id_ = int(float(id_))
             return id_
         except ValueError:
```

### Comparing `space_rocks-1.7.6/rocks/ssodnet.py` & `space_rocks-1.7.7/rocks/ssodnet.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.6/setup.py` & `space_rocks-1.7.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,46 +10,42 @@
 install_requires = \
 ['Levenshtein>=0.16.0,<0.17.0',
  'aiodns>=3.0.0,<4.0.0',
  'aiohttp>=3.7.4,<4.0.0',
  'beautifulsoup4>=4.11.1,<5.0.0',
  'bs4>=0.0.1,<0.0.2',
  'cchardet>=2.1.7,<3.0.0',
- 'click>=8.0.1,<9.0.0',
+ 'click>=8.1.2',
  'furo>=2022.9.15,<2023.0.0',
- 'matplotlib>=3.4.3,<4.0.0',
+ 'matplotlib>=3.4.3',
  'nest-asyncio>=1.5.1,<2.0.0',
- 'numpy>=1.21.2,<2.0.0',
- 'pandas>=1.3.2,<2.0.0',
+ 'numpy>=1.21',
+ 'pandas>=1.3.5',
  'platformdirs>=2.6.2,<3.0.0',
  'pydantic>=1.8.2,<2.0.0',
  'requests>=2.26.0,<3.0.0',
- 'rich>=12,<13',
+ 'rich>=12.2.0',
  'sphinx-copybutton>=0.5.0,<0.6.0',
  'sphinx_design>=0.3.0,<0.4.0']
 
-extras_require = \
-{'docs': ['sphinx>=5,<6', 'sphinx-hoverxref']}
-
 entry_points = \
 {'console_scripts': ['rocks = rocks.cli:cli_rocks']}
 
 setup_kwargs = {
     'name': 'space-rocks',
-    'version': '1.7.6',
+    'version': '1.7.7',
     'description': 'Python client for SsODNet data access.',
     'long_description': '<p align="center">\n  <img width="260" src="https://raw.githubusercontent.com/maxmahlke/rocks/master/docs/_static/logo_rocks.svg">\n</p>\n\n<p align="center">\n  <a href="https://github.com/maxmahlke/rocks#features"> Features </a> - <a href="https://github.com/maxmahlke/rocks#install"> Install </a> - <a href="https://github.com/maxmahlke/rocks#documentation"> Documentation </a>\n</p>\n\n<br>\n\n<div align="center">\n  <a href="https://img.shields.io/pypi/pyversions/space-rocks">\n    <img src="https://img.shields.io/pypi/pyversions/space-rocks"/>\n  </a>\n  <a href="https://img.shields.io/pypi/v/space-rocks">\n    <img src="https://img.shields.io/pypi/v/space-rocks"/>\n  </a>\n  <a href="https://readthedocs.org/projects/rocks/badge/?version=latest">\n    <img src="https://readthedocs.org/projects/rocks/badge/?version=latest"/>\n  </a>\n  <a href="https://arxiv.org/abs/2209.10697">\n    <img src="https://img.shields.io/badge/arXiv-2209.10697-f9f107.svg"/>\n  </a>\n</div>\n\n<br>\n\n## Features\n\nExplore asteroid data on the command-line...\n\n``` sh\n$ rocks id 221\n(221) Eos\n\n$ rocks class Eos\nMB>Outer\n\n$ rocks albedo Eos\n0.136 +- 0.004\n\n$ rocks taxonomy Eos\nK\n\n$ rocks density Eos\n4.559e+03 +- 1.139e+03 kg/m$^3$\n```\n\n... and in a `python` script.\n\n``` python\n>>> import rocks\n>>> rocks.identify("1902ug")\n(\'Fortuna\', 19)\n>>> ceres = rocks.Rock("ceres")\n>>> ceres.diameter.value\n848.4\n>>> ceres.diameter.unit\n\'km\'\n>>> ceres.mass.value\n9.384e+20\n>>> ceres.mass.error\n6.711e+17\n```\n\n## Install\n\nInstall from PyPi using `pip`:\n\n     $ pip install space-rocks\n\nThe minimum required `python` version is 3.7.\n\n\n## Documentation\n\nCheck out the documentation at [rocks.readthedocs.io](https://rocks.readthedocs.io/en/latest/) or run\n\n     $ rocks docs\n',
     'author': 'Max Mahlke',
     'author_email': 'max.mahlke@oca.eu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://rocks.readthedocs.io/en/latest/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'extras_require': extras_require,
     'entry_points': entry_points,
     'python_requires': '>=3.7.1,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['rocks']
 package_data = \ {'': ['*']} install_requires = \
 ['Levenshtein>=0.16.0,<0.17.0', 'aiodns>=3.0.0,<4.0.0',
 'aiohttp>=3.7.4,<4.0.0', 'beautifulsoup4>=4.11.1,<5.0.0', 'bs4>=0.0.1,<0.0.2',
-'cchardet>=2.1.7,<3.0.0', 'click>=8.0.1,<9.0.0', 'furo>=2022.9.15,<2023.0.0',
-'matplotlib>=3.4.3,<4.0.0', 'nest-asyncio>=1.5.1,<2.0.0',
-'numpy>=1.21.2,<2.0.0', 'pandas>=1.3.2,<2.0.0', 'platformdirs>=2.6.2,<3.0.0',
-'pydantic>=1.8.2,<2.0.0', 'requests>=2.26.0,<3.0.0', 'rich>=12,<13', 'sphinx-
-copybutton>=0.5.0,<0.6.0', 'sphinx_design>=0.3.0,<0.4.0'] extras_require = \
-{'docs': ['sphinx>=5,<6', 'sphinx-hoverxref']} entry_points = \
-{'console_scripts': ['rocks = rocks.cli:cli_rocks']} setup_kwargs = { 'name':
-'space-rocks', 'version': '1.7.6', 'description': 'Python client for SsODNet
-data access.', 'long_description': '
+'cchardet>=2.1.7,<3.0.0', 'click>=8.1.2', 'furo>=2022.9.15,<2023.0.0',
+'matplotlib>=3.4.3', 'nest-asyncio>=1.5.1,<2.0.0', 'numpy>=1.21',
+'pandas>=1.3.5', 'platformdirs>=2.6.2,<3.0.0', 'pydantic>=1.8.2,<2.0.0',
+'requests>=2.26.0,<3.0.0', 'rich>=12.2.0', 'sphinx-copybutton>=0.5.0,<0.6.0',
+'sphinx_design>=0.3.0,<0.4.0'] entry_points = \ {'console_scripts': ['rocks =
+rocks.cli:cli_rocks']} setup_kwargs = { 'name': 'space-rocks', 'version':
+'1.7.7', 'description': 'Python client for SsODNet data access.',
+'long_description': '
   \n [https://raw.githubusercontent.com/maxmahlke/rocks/master/docs/_static/
                                logo_rocks.svg]\n
 \n\n
                     \n Features - Install - Documentation\n
 \n\n
 \n\n
   \n \n_[https://img.shields.io/pypi/pyversions/space-rocks]\n\n \n_[https://
@@ -33,9 +32,9 @@
 Install\n\nInstall from PyPi using `pip`:\n\n $ pip install space-rocks\n\nThe
 minimum required `python` version is 3.7.\n\n\n## Documentation\n\nCheck out
 the documentation at [rocks.readthedocs.io](https://rocks.readthedocs.io/en/
 latest/) or run\n\n $ rocks docs\n', 'author': 'Max Mahlke', 'author_email':
 'max.mahlke@oca.eu', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
 'https://rocks.readthedocs.io/en/latest/', 'packages': packages,
 'package_data': package_data, 'install_requires': install_requires,
-'extras_require': extras_require, 'entry_points': entry_points,
-'python_requires': '>=3.7.1,<3.11', } setup(**setup_kwargs)
+'entry_points': entry_points, 'python_requires': '>=3.7.1,<3.11', } setup
+(**setup_kwargs)
```

### Comparing `space_rocks-1.7.6/PKG-INFO` & `space_rocks-1.7.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: space-rocks
-Version: 1.7.6
+Version: 1.7.7
 Summary: Python client for SsODNet data access.
 Home-page: https://rocks.readthedocs.io/en/latest/
 License: MIT
 Author: Max Mahlke
 Author-email: max.mahlke@oca.eu
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -15,28 +15,25 @@
 Provides-Extra: docs
 Requires-Dist: Levenshtein (>=0.16.0,<0.17.0)
 Requires-Dist: aiodns (>=3.0.0,<4.0.0)
 Requires-Dist: aiohttp (>=3.7.4,<4.0.0)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: cchardet (>=2.1.7,<3.0.0)
-Requires-Dist: click (>=8.0.1,<9.0.0)
+Requires-Dist: click (>=8.1.2)
 Requires-Dist: furo (>=2022.9.15,<2023.0.0)
-Requires-Dist: jinja2 (<3.1)
-Requires-Dist: matplotlib (>=3.4.3,<4.0.0)
+Requires-Dist: matplotlib (>=3.4.3)
 Requires-Dist: nest-asyncio (>=1.5.1,<2.0.0)
-Requires-Dist: numpy (>=1.21.2,<2.0.0)
-Requires-Dist: pandas (>=1.3.2,<2.0.0)
+Requires-Dist: numpy (>=1.21)
+Requires-Dist: pandas (>=1.3.5)
 Requires-Dist: platformdirs (>=2.6.2,<3.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
-Requires-Dist: rich (>=12,<13)
-Requires-Dist: sphinx (>=5,<6); extra == "docs"
+Requires-Dist: rich (>=12.2.0)
 Requires-Dist: sphinx-copybutton (>=0.5.0,<0.6.0)
-Requires-Dist: sphinx-hoverxref; extra == "docs"
 Requires-Dist: sphinx_design (>=0.3.0,<0.4.0)
 Project-URL: Documentation, https://rocks.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/maxmahlke/rocks.git
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img width="260" src="https://raw.githubusercontent.com/maxmahlke/rocks/master/docs/_static/logo_rocks.svg">
```

#### html2text {}

```diff
@@ -1,28 +1,26 @@
-Metadata-Version: 2.1 Name: space-rocks Version: 1.7.6 Summary: Python client
+Metadata-Version: 2.1 Name: space-rocks Version: 1.7.7 Summary: Python client
 for SsODNet data access. Home-page: https://rocks.readthedocs.io/en/latest/
 License: MIT Author: Max Mahlke Author-email: max.mahlke@oca.eu Requires-
 Python: >=3.7.1,<3.11 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Provides-Extra: docs
 Requires-Dist: Levenshtein (>=0.16.0,<0.17.0) Requires-Dist: aiodns
 (>=3.0.0,<4.0.0) Requires-Dist: aiohttp (>=3.7.4,<4.0.0) Requires-Dist:
 beautifulsoup4 (>=4.11.1,<5.0.0) Requires-Dist: bs4 (>=0.0.1,<0.0.2) Requires-
-Dist: cchardet (>=2.1.7,<3.0.0) Requires-Dist: click (>=8.0.1,<9.0.0) Requires-
-Dist: furo (>=2022.9.15,<2023.0.0) Requires-Dist: jinja2 (<3.1) Requires-Dist:
-matplotlib (>=3.4.3,<4.0.0) Requires-Dist: nest-asyncio (>=1.5.1,<2.0.0)
-Requires-Dist: numpy (>=1.21.2,<2.0.0) Requires-Dist: pandas (>=1.3.2,<2.0.0)
-Requires-Dist: platformdirs (>=2.6.2,<3.0.0) Requires-Dist: pydantic
-(>=1.8.2,<2.0.0) Requires-Dist: requests (>=2.26.0,<3.0.0) Requires-Dist: rich
-(>=12,<13) Requires-Dist: sphinx (>=5,<6); extra == "docs" Requires-Dist:
-sphinx-copybutton (>=0.5.0,<0.6.0) Requires-Dist: sphinx-hoverxref; extra ==
-"docs" Requires-Dist: sphinx_design (>=0.3.0,<0.4.0) Project-URL:
-Documentation, https://rocks.readthedocs.io/en/latest/ Project-URL: Repository,
-https://github.com/maxmahlke/rocks.git Description-Content-Type: text/markdown
+Dist: cchardet (>=2.1.7,<3.0.0) Requires-Dist: click (>=8.1.2) Requires-Dist:
+furo (>=2022.9.15,<2023.0.0) Requires-Dist: matplotlib (>=3.4.3) Requires-Dist:
+nest-asyncio (>=1.5.1,<2.0.0) Requires-Dist: numpy (>=1.21) Requires-Dist:
+pandas (>=1.3.5) Requires-Dist: platformdirs (>=2.6.2,<3.0.0) Requires-Dist:
+pydantic (>=1.8.2,<2.0.0) Requires-Dist: requests (>=2.26.0,<3.0.0) Requires-
+Dist: rich (>=12.2.0) Requires-Dist: sphinx-copybutton (>=0.5.0,<0.6.0)
+Requires-Dist: sphinx_design (>=0.3.0,<0.4.0) Project-URL: Documentation,
+https://rocks.readthedocs.io/en/latest/ Project-URL: Repository, https://
+github.com/maxmahlke/rocks.git Description-Content-Type: text/markdown
     [https://raw.githubusercontent.com/maxmahlke/rocks/master/docs/_static/
                                 logo_rocks.svg]
                       Features - Install - Documentation
 
  [https://img.shields.io/pypi/pyversions/space-rocks] [https://img.shields.io/
       pypi/v/space-rocks] [https://readthedocs.org/projects/rocks/badge/
   ?version=latest] [https://img.shields.io/badge/arXiv-2209.10697-f9f107.svg]
```

