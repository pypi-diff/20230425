# Comparing `tmp/pynamer-0.2.0.tar.gz` & `tmp/pynamer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamer-0.2.0.tar", last modified: Fri Apr 21 20:37:15 2023, max compression
+gzip compressed data, was "pynamer-0.3.0.tar", last modified: Tue Apr 25 12:44:42 2023, max compression
```

## Comparing `pynamer-0.2.0.tar` & `pynamer-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 20:37:15.010111 pynamer-0.2.0/
--rw-rw-rw-   0        0        0      161 2023-04-21 18:16:39.000000 pynamer-0.2.0/AUTHORS.md
--rw-rw-rw-   0        0        0      466 2023-04-21 20:36:59.000000 pynamer-0.2.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1095 2023-04-21 17:08:24.000000 pynamer-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      237 2023-04-21 17:08:24.000000 pynamer-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7484 2023-04-21 20:37:15.010111 pynamer-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     6279 2023-04-21 18:16:39.000000 pynamer-0.2.0/README.md
--rw-rw-rw-   0        0        0     2344 2023-04-21 17:08:24.000000 pynamer-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0     1662 2023-04-21 20:37:15.010111 pynamer-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      109 2023-04-21 17:08:24.000000 pynamer-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 20:37:14.925446 pynamer-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 20:37:14.980935 pynamer-0.2.0/src/pynamer/
--rw-rw-rw-   0        0        0     1172 2023-04-21 20:37:00.000000 pynamer-0.2.0/src/pynamer/__init__.py
--rw-rw-rw-   0        0        0     1459 2023-04-21 20:34:11.000000 pynamer-0.2.0/src/pynamer/pynamer.py
-drwxrwxrwx   0        0        0        0 2023-04-21 20:37:14.980935 pynamer-0.2.0/src/pynamer/resources/
--rw-rw-rw-   0        0        0        0 2023-04-21 17:08:24.000000 pynamer-0.2.0/src/pynamer/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 20:37:14.980935 pynamer-0.2.0/src/pynamer.egg-info/
--rw-rw-rw-   0        0        0     7484 2023-04-21 20:37:14.000000 pynamer-0.2.0/src/pynamer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2023-04-21 20:37:14.000000 pynamer-0.2.0/src/pynamer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 20:37:14.000000 pynamer-0.2.0/src/pynamer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-21 20:37:14.000000 pynamer-0.2.0/src/pynamer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-04-21 20:37:14.000000 pynamer-0.2.0/src/pynamer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-21 20:37:14.000000 pynamer-0.2.0/src/pynamer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-21 20:37:14.994467 pynamer-0.2.0/tests/
--rw-rw-rw-   0        0        0      781 2023-04-21 18:16:35.000000 pynamer-0.2.0/tests/test_pynamer.py
--rw-rw-rw-   0        0        0     1165 2023-04-21 18:15:58.000000 pynamer-0.2.0/tests/test_pynamer_cli.py
+drwxrwxrwx   0        0        0        0 2023-04-25 12:44:42.000337 pynamer-0.3.0/
+-rw-rw-rw-   0        0        0      161 2023-04-21 18:16:39.000000 pynamer-0.3.0/AUTHORS.md
+-rw-rw-rw-   0        0        0     2395 2023-04-25 12:44:30.000000 pynamer-0.3.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1095 2023-04-21 17:08:24.000000 pynamer-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      237 2023-04-25 12:30:17.000000 pynamer-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    10951 2023-04-25 12:44:42.001337 pynamer-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9886 2023-04-24 17:58:35.000000 pynamer-0.3.0/README.md
+-rw-rw-rw-   0        0        0     2344 2023-04-21 17:08:24.000000 pynamer-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1713 2023-04-25 12:44:42.003334 pynamer-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      109 2023-04-21 17:08:24.000000 pynamer-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 12:44:41.912338 pynamer-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 12:44:41.974335 pynamer-0.3.0/src/pynamer/
+-rw-rw-rw-   0        0        0       10 2023-04-25 12:29:58.000000 pynamer-0.3.0/src/pynamer/README.md
+-rw-rw-rw-   0        0        0     1185 2023-04-25 12:44:30.000000 pynamer-0.3.0/src/pynamer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 12:44:41.993334 pynamer-0.3.0/src/pynamer/project_name/
+-rw-rw-rw-   0        0        0       37 2023-04-14 21:59:18.000000 pynamer-0.3.0/src/pynamer/project_name/__init__.py
+-rw-rw-rw-   0        0        0     9854 2023-04-25 12:41:44.000000 pynamer-0.3.0/src/pynamer/pynamer.py
+-rw-rw-rw-   0        0        0      395 2023-04-16 15:45:19.000000 pynamer-0.3.0/src/pynamer/setup.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 12:44:41.991336 pynamer-0.3.0/src/pynamer.egg-info/
+-rw-rw-rw-   0        0        0    10951 2023-04-25 12:44:41.000000 pynamer-0.3.0/src/pynamer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      475 2023-04-25 12:44:41.000000 pynamer-0.3.0/src/pynamer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 12:44:41.000000 pynamer-0.3.0/src/pynamer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-04-25 12:44:41.000000 pynamer-0.3.0/src/pynamer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       23 2023-04-25 12:44:41.000000 pynamer-0.3.0/src/pynamer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-25 12:44:41.000000 pynamer-0.3.0/src/pynamer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 12:44:41.997335 pynamer-0.3.0/tests/
+-rw-rw-rw-   0        0        0      781 2023-04-21 18:16:35.000000 pynamer-0.3.0/tests/test_pynamer.py
+-rw-rw-rw-   0        0        0     1165 2023-04-21 18:15:58.000000 pynamer-0.3.0/tests/test_pynamer_cli.py
```

### Comparing `pynamer-0.2.0/LICENSE` & `pynamer-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamer-0.2.0/pyproject.toml` & `pynamer-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynamer-0.2.0/setup.cfg` & `pynamer-0.3.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -63,42 +63,46 @@
 000003e0: 630d 0a70 6163 6b61 6765 7320 3d20 6669  c..packages = fi
 000003f0: 6e64 3a0d 0a70 726f 6a65 6374 5f75 726c  nd:..project_url
 00000400: 7320 3d20 0d0a 696e 636c 7564 655f 7061  s = ..include_pa
 00000410: 636b 6167 655f 6461 7461 203d 2054 7275  ckage_data = Tru
 00000420: 650d 0a70 7974 686f 6e5f 7265 7175 6972  e..python_requir
 00000430: 6573 203d 203e 3d33 2e38 0d0a 696e 7374  es = >=3.8..inst
 00000440: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
-00000450: 0a09 636c 6963 6b0d 0a09 7079 7961 6d6c  ..click...pyyaml
-00000460: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-00000470: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
-00000480: 7265 203d 2073 7263 0d0a 0d0a 5b6f 7074  re = src....[opt
-00000490: 696f 6e73 2e70 6163 6b61 6765 5f64 6174  ions.package_dat
-000004a0: 615d 0d0a 7079 6e61 6d65 7220 3d20 0d0a  a]..pynamer = ..
-000004b0: 0972 6573 6f75 7263 6573 2f63 6f6e 6669  .resources/confi
-000004c0: 672e 7961 6d6c 0d0a 0d0a 5b6f 7074 696f  g.yaml....[optio
-000004d0: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
-000004e0: 0d0a 636f 6e73 6f6c 655f 7363 7269 7074  ..console_script
-000004f0: 7320 3d20 0d0a 0970 796e 616d 6572 203d  s = ...pynamer =
-00000500: 2070 796e 616d 6572 2e70 796e 616d 6572   pynamer.pynamer
-00000510: 5f63 6c69 3a63 6c69 0d0a 0d0a 5b66 6c61  _cli:cli....[fla
-00000520: 6b65 385d 0d0a 646f 6373 7472 696e 672d  ke8]..docstring-
-00000530: 636f 6e76 656e 7469 6f6e 203d 206e 756d  convention = num
-00000540: 7079 0d0a 6d61 782d 636f 6d70 6c65 7869  py..max-complexi
-00000550: 7479 203d 2031 380d 0a6d 6178 2d6c 696e  ty = 18..max-lin
-00000560: 652d 6c65 6e67 7468 203d 2038 380d 0a73  e-length = 88..s
-00000570: 656c 6563 7420 3d20 422c 2042 392c 2043  elect = B, B9, C
-00000580: 2c20 442c 2045 2c20 462c 204e 2c20 570d  , D, E, F, N, W.
-00000590: 0a65 7863 6c75 6465 203d 2074 6573 7473  .exclude = tests
-000005a0: 2f2a 2c2e 746f 782f 2a2c 2e6e 6f78 2f2a  /*,.tox/*,.nox/*
-000005b0: 2c64 6f63 732f 2a2c 2e67 6974 2f2a 2c2e  ,docs/*,.git/*,.
-000005c0: 6769 7468 7562 2f2a 0d0a 6967 6e6f 7265  github/*..ignore
-000005d0: 203d 200d 0a09 4532 3033 2c0d 0a09 5735   = ...E203,...W5
-000005e0: 3033 2c0d 0a09 4634 3031 2c0d 0a70 6572  03,...F401,..per
-000005f0: 2d66 696c 652d 6967 6e6f 7265 7320 3d20  -file-ignores = 
-00000600: 0d0a 095f 5f69 6e69 745f 5f2e 7079 3a46  ...__init__.py:F
-00000610: 3430 310d 0a09 7061 7468 6d61 6769 632e  401...pathmagic.
-00000620: 7079 3a46 3430 310d 0a09 7465 7374 5f70  py:F401...test_p
-00000630: 796e 616d 6572 2e70 793a 4634 3031 0d0a  ynamer.py:F401..
-00000640: 0970 796e 616d 6572 2e70 793a 4634 3031  .pynamer.py:F401
-00000650: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-00000660: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000670: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000450: 0a09 7079 7961 6d6c 0d0a 0972 6571 7565  ..pyyaml...reque
+00000460: 7374 730d 0a09 6a69 6e6a 6132 0d0a 0d0a  sts...jinja2....
+00000470: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+00000480: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
+00000490: 2073 7263 0d0a 0d0a 5b6f 7074 696f 6e73   src....[options
+000004a0: 2e70 6163 6b61 6765 5f64 6174 615d 0d0a  .package_data]..
+000004b0: 7079 6e61 6d65 7220 3d20 0d0a 0973 6574  pynamer = ...set
+000004c0: 7570 2e74 7874 0d0a 0952 4541 444d 452e  up.txt...README.
+000004d0: 6d64 0d0a 0970 726f 6a65 6374 5f6e 616d  md...project_nam
+000004e0: 650d 0a09 7072 6f6a 6563 745f 6e61 6d65  e...project_name
+000004f0: 2f5f 5f69 6e69 745f 5f2e 7079 0d0a 0d0a  /__init__.py....
+00000500: 5b6f 7074 696f 6e73 2e65 6e74 7279 5f70  [options.entry_p
+00000510: 6f69 6e74 735d 0d0a 636f 6e73 6f6c 655f  oints]..console_
+00000520: 7363 7269 7074 7320 3d20 0d0a 0970 796e  scripts = ...pyn
+00000530: 616d 6572 203d 2070 796e 616d 6572 2e70  amer = pynamer.p
+00000540: 796e 616d 6572 3a6d 6169 6e0d 0a0d 0a5b  ynamer:main....[
+00000550: 666c 616b 6538 5d0d 0a64 6f63 7374 7269  flake8]..docstri
+00000560: 6e67 2d63 6f6e 7665 6e74 696f 6e20 3d20  ng-convention = 
+00000570: 6e75 6d70 790d 0a6d 6178 2d63 6f6d 706c  numpy..max-compl
+00000580: 6578 6974 7920 3d20 3138 0d0a 6d61 782d  exity = 18..max-
+00000590: 6c69 6e65 2d6c 656e 6774 6820 3d20 3838  line-length = 88
+000005a0: 0d0a 7365 6c65 6374 203d 2042 2c20 4239  ..select = B, B9
+000005b0: 2c20 432c 2044 2c20 452c 2046 2c20 4e2c  , C, D, E, F, N,
+000005c0: 2057 0d0a 6578 636c 7564 6520 3d20 7465   W..exclude = te
+000005d0: 7374 732f 2a2c 2e74 6f78 2f2a 2c2e 6e6f  sts/*,.tox/*,.no
+000005e0: 782f 2a2c 646f 6373 2f2a 2c2e 6769 742f  x/*,docs/*,.git/
+000005f0: 2a2c 2e67 6974 6875 622f 2a0d 0a69 676e  *,.github/*..ign
+00000600: 6f72 6520 3d20 0d0a 0945 3230 332c 0d0a  ore = ...E203,..
+00000610: 0957 3530 332c 0d0a 0946 3430 312c 0d0a  .W503,...F401,..
+00000620: 7065 722d 6669 6c65 2d69 676e 6f72 6573  per-file-ignores
+00000630: 203d 200d 0a09 5f5f 696e 6974 5f5f 2e70   = ...__init__.p
+00000640: 793a 4634 3031 0d0a 0970 6174 686d 6167  y:F401...pathmag
+00000650: 6963 2e70 793a 4634 3031 0d0a 0974 6573  ic.py:F401...tes
+00000660: 745f 7079 6e61 6d65 722e 7079 3a46 3430  t_pynamer.py:F40
+00000670: 310d 0a09 7079 6e61 6d65 722e 7079 3a46  1...pynamer.py:F
+00000680: 3430 310d 0a0d 0a5b 6567 675f 696e 666f  401....[egg_info
+00000690: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+000006a0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+000006b0: 0a                                       .
```

### Comparing `pynamer-0.2.0/src/pynamer/__init__.py` & `pynamer-0.3.0/src/pynamer/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Core Library modules
 import logging.config
 
 # Third party modules
 import yaml  # type: ignore
 
 __title__ = "pynamer"
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 __author__ = "Stephen R A King"
 __description__ = (
     "Utility to find an available package name on the PyPI repository and register it "
 )
 __email__ = "sking.github@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Stephen R A King"
@@ -26,14 +26,15 @@
     level: INFO
     stream: ext://sys.stdout
     formatter: basic
   file:
     class: logging.FileHandler
     level: DEBUG
     filename: pynamer.log
+    mode: w
     encoding: utf-8
     formatter: timestamp
 
 formatters:
   basic:
     style: "{"
     format: "{levelname:s}:{name:s}:{message:s}"
```

### Comparing `pynamer-0.2.0/tests/test_pynamer.py` & `pynamer-0.3.0/tests/test_pynamer.py`

 * *Files identical despite different names*

### Comparing `pynamer-0.2.0/tests/test_pynamer_cli.py` & `pynamer-0.3.0/tests/test_pynamer_cli.py`

 * *Files identical despite different names*

