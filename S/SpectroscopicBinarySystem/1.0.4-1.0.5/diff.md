# Comparing `tmp/SpectroscopicBinarySystem-1.0.4.tar.gz` & `tmp/SpectroscopicBinarySystem-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpectroscopicBinarySystem-1.0.4.tar", last modified: Tue Apr 25 12:38:53 2023, max compression
+gzip compressed data, was "SpectroscopicBinarySystem-1.0.5.tar", last modified: Tue Apr 25 12:44:51 2023, max compression
```

## Comparing `SpectroscopicBinarySystem-1.0.4.tar` & `SpectroscopicBinarySystem-1.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 12:38:53.233541 SpectroscopicBinarySystem-1.0.4/
--rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1811 2023-04-25 12:38:53.233541 SpectroscopicBinarySystem-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1421 2023-04-25 12:20:47.000000 SpectroscopicBinarySystem-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 12:38:53.232349 SpectroscopicBinarySystem-1.0.4/SpectroscopicBinarySystem.egg-info/
--rw-rw-rw-   0        0        0     1811 2023-04-25 12:38:53.000000 SpectroscopicBinarySystem-1.0.4/SpectroscopicBinarySystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2023-04-25 12:38:53.000000 SpectroscopicBinarySystem-1.0.4/SpectroscopicBinarySystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 12:38:53.000000 SpectroscopicBinarySystem-1.0.4/SpectroscopicBinarySystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      189 2023-04-25 12:38:53.000000 SpectroscopicBinarySystem-1.0.4/SpectroscopicBinarySystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 12:38:53.000000 SpectroscopicBinarySystem-1.0.4/SpectroscopicBinarySystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-04-25 10:37:13.000000 SpectroscopicBinarySystem-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      846 2023-04-25 12:38:53.235717 SpectroscopicBinarySystem-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 12:44:51.363843 SpectroscopicBinarySystem-1.0.5/
+-rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1811 2023-04-25 12:44:51.364857 SpectroscopicBinarySystem-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1421 2023-04-25 12:20:47.000000 SpectroscopicBinarySystem-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 12:44:51.362815 SpectroscopicBinarySystem-1.0.5/SpectroscopicBinarySystem.egg-info/
+-rw-rw-rw-   0        0        0     1811 2023-04-25 12:44:51.000000 SpectroscopicBinarySystem-1.0.5/SpectroscopicBinarySystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-04-25 12:44:51.000000 SpectroscopicBinarySystem-1.0.5/SpectroscopicBinarySystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 12:44:51.000000 SpectroscopicBinarySystem-1.0.5/SpectroscopicBinarySystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-04-25 12:44:51.000000 SpectroscopicBinarySystem-1.0.5/SpectroscopicBinarySystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 12:44:51.000000 SpectroscopicBinarySystem-1.0.5/SpectroscopicBinarySystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-04-25 10:37:13.000000 SpectroscopicBinarySystem-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      829 2023-04-25 12:44:51.367397 SpectroscopicBinarySystem-1.0.5/setup.cfg
```

### Comparing `SpectroscopicBinarySystem-1.0.4/LICENSE` & `SpectroscopicBinarySystem-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.0.4/PKG-INFO` & `SpectroscopicBinarySystem-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `SpectroscopicBinarySystem-1.0.4/README.md` & `SpectroscopicBinarySystem-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.0.4/SpectroscopicBinarySystem.egg-info/PKG-INFO` & `SpectroscopicBinarySystem-1.0.5/SpectroscopicBinarySystem.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `SpectroscopicBinarySystem-1.0.4/setup.cfg` & `SpectroscopicBinarySystem-1.0.5/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 7065 6374 726f 7363 6f70 6963   = Spectroscopic
 00000020: 4269 6e61 7279 5379 7374 656d 0d0a 7665  BinarySystem..ve
-00000030: 7273 696f 6e20 3d20 312e 302e 340d 0a61  rsion = 1.0.4..a
+00000030: 7273 696f 6e20 3d20 312e 302e 350d 0a61  rsion = 1.0.5..a
 00000040: 7574 686f 7220 3d20 4775 696c 6c61 756d  uthor = Guillaum
 00000050: 6520 4265 7274 7261 6e64 0d0a 6175 7468  e Bertrand..auth
 00000060: 6f72 5f65 6d61 696c 203d 2067 6265 2e69  or_email = gbe.i
 00000070: 6f40 706d 2e6d 650d 0a64 6573 6372 6970  o@pm.me..descrip
 00000080: 7469 6f6e 203d 2050 7974 686f 6e20 6173  tion = Python as
 00000090: 7472 6f6e 6f6d 7920 746f 6f6c 7320 666f  tronomy tools fo
 000000a0: 7220 7370 6563 7472 6f73 636f 7069 6320  r spectroscopic 
@@ -30,24 +30,23 @@
 000001d0: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
 000001e0: 203d 200d 0a09 6173 7472 6f70 793e 3d35   = ...astropy>=5
 000001f0: 2e32 2e32 0d0a 0961 7374 726f 7175 6572  .2.2...astroquer
 00000200: 793e 3d30 2e34 2e36 0d0a 0942 696e 6172  y>=0.4.6...Binar
 00000210: 7953 7461 7253 6f6c 7665 723e 3d31 2e32  yStarSolver>=1.2
 00000220: 2e30 0d0a 096d 6174 706c 6f74 6c69 623e  .0...matplotlib>
 00000230: 3d33 2e37 2e31 0d0a 096e 756d 7079 3e3d  =3.7.1...numpy>=
-00000240: 312e 3234 2e32 0d0a 096f 7262 6974 616c  1.24.2...orbital
-00000250: 3e3d 302e 302e 300d 0a09 4f72 6269 7461  >=0.0.0...Orbita
-00000260: 6c50 793e 3d30 2e37 2e30 0d0a 0950 7959  lPy>=0.7.0...PyY
-00000270: 414d 4c3e 3d36 2e30 0d0a 0973 7065 6375  AML>=6.0...specu
-00000280: 7469 6c73 3e3d 312e 392e 310d 0a09 4269  tils>=1.9.1...Bi
-00000290: 6e61 7279 5374 6172 536f 6c76 6572 3e3d  naryStarSolver>=
-000002a0: 312e 322e 300d 0a09 706c 6f74 6c79 3e3d  1.2.0...plotly>=
-000002b0: 352e 3134 2e31 0d0a 0d0a 5b6f 7074 696f  5.14.1....[optio
-000002c0: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
-000002d0: 5d0d 0a69 6e63 6c75 6465 203d 2073 7065  ]..include = spe
-000002e0: 6374 726f 7363 6f70 6963 6269 6e61 7279  ctroscopicbinary
-000002f0: 7379 7374 656d 2f2a 0d0a 6578 636c 7564  system/*..exclud
-00000300: 6520 3d20 0d0a 0965 7861 6d70 6c65 732a  e = ...examples*
-00000310: 0d0a 0964 6f63 732a 0d0a 0974 6573 742a  ...docs*...test*
-00000320: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-00000330: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000340: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000240: 312e 3234 2e32 0d0a 094f 7262 6974 616c  1.24.2...Orbital
+00000250: 5079 3e3d 302e 372e 300d 0a09 5079 5941  Py>=0.7.0...PyYA
+00000260: 4d4c 3e3d 362e 300d 0a09 7370 6563 7574  ML>=6.0...specut
+00000270: 696c 733e 3d31 2e39 2e31 0d0a 0942 696e  ils>=1.9.1...Bin
+00000280: 6172 7953 7461 7253 6f6c 7665 723e 3d31  aryStarSolver>=1
+00000290: 2e32 2e30 0d0a 0970 6c6f 746c 793e 3d35  .2.0...plotly>=5
+000002a0: 2e31 342e 310d 0a0d 0a5b 6f70 7469 6f6e  .14.1....[option
+000002b0: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+000002c0: 0d0a 696e 636c 7564 6520 3d20 7370 6563  ..include = spec
+000002d0: 7472 6f73 636f 7069 6362 696e 6172 7973  troscopicbinarys
+000002e0: 7973 7465 6d2f 2a0d 0a65 7863 6c75 6465  ystem/*..exclude
+000002f0: 203d 200d 0a09 6578 616d 706c 6573 2a0d   = ...examples*.
+00000300: 0a09 646f 6373 2a0d 0a09 7465 7374 2a0d  ..docs*...test*.
+00000310: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000320: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000330: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

