# Comparing `tmp/SpectroscopicBinarySystem-1.0.7.tar.gz` & `tmp/SpectroscopicBinarySystem-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpectroscopicBinarySystem-1.0.7.tar", last modified: Tue Apr 25 13:02:09 2023, max compression
+gzip compressed data, was "SpectroscopicBinarySystem-1.0.8.tar", last modified: Tue Apr 25 13:06:19 2023, max compression
```

## Comparing `SpectroscopicBinarySystem-1.0.7.tar` & `SpectroscopicBinarySystem-1.0.8.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 13:02:09.580186 SpectroscopicBinarySystem-1.0.7/
--rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     1811 2023-04-25 13:02:09.581479 SpectroscopicBinarySystem-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1421 2023-04-25 12:20:47.000000 SpectroscopicBinarySystem-1.0.7/README.md
--rw-rw-rw-   0        0        0       82 2023-04-25 10:37:13.000000 SpectroscopicBinarySystem-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      831 2023-04-25 13:02:09.584487 SpectroscopicBinarySystem-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-25 13:02:09.544034 SpectroscopicBinarySystem-1.0.7/spectroscopicbinarysystem/
-drwxrwxrwx   0        0        0        0 2023-04-25 13:02:09.579023 SpectroscopicBinarySystem-1.0.7/spectroscopicbinarysystem/SpectroscopicBinarySystem.egg-info/
--rw-rw-rw-   0        0        0     1811 2023-04-25 13:02:09.000000 SpectroscopicBinarySystem-1.0.7/spectroscopicbinarysystem/SpectroscopicBinarySystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-04-25 13:02:09.000000 SpectroscopicBinarySystem-1.0.7/spectroscopicbinarysystem/SpectroscopicBinarySystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 13:02:09.000000 SpectroscopicBinarySystem-1.0.7/spectroscopicbinarysystem/SpectroscopicBinarySystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-04-25 13:02:09.000000 SpectroscopicBinarySystem-1.0.7/spectroscopicbinarysystem/SpectroscopicBinarySystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 13:02:09.000000 SpectroscopicBinarySystem-1.0.7/spectroscopicbinarysystem/SpectroscopicBinarySystem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 13:06:19.535533 SpectroscopicBinarySystem-1.0.8/
+-rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1811 2023-04-25 13:06:19.535533 SpectroscopicBinarySystem-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1421 2023-04-25 12:20:47.000000 SpectroscopicBinarySystem-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 13:06:19.531791 SpectroscopicBinarySystem-1.0.8/SpectroscopicBinarySystem.egg-info/
+-rw-rw-rw-   0        0        0     1811 2023-04-25 13:06:19.000000 SpectroscopicBinarySystem-1.0.8/SpectroscopicBinarySystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2023-04-25 13:06:19.000000 SpectroscopicBinarySystem-1.0.8/SpectroscopicBinarySystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 13:06:19.000000 SpectroscopicBinarySystem-1.0.8/SpectroscopicBinarySystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-25 13:06:19.000000 SpectroscopicBinarySystem-1.0.8/SpectroscopicBinarySystem.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0      174 2023-04-25 13:06:19.000000 SpectroscopicBinarySystem-1.0.8/SpectroscopicBinarySystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-04-25 13:06:19.000000 SpectroscopicBinarySystem-1.0.8/SpectroscopicBinarySystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-04-25 10:37:13.000000 SpectroscopicBinarySystem-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      753 2023-04-25 13:06:19.537761 SpectroscopicBinarySystem-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 13:06:19.534023 SpectroscopicBinarySystem-1.0.8/spectroscopicbinarysystem/
+-rw-rw-rw-   0        0        0    23846 2023-04-25 13:05:14.000000 SpectroscopicBinarySystem-1.0.8/spectroscopicbinarysystem/__init__.py
```

### Comparing `SpectroscopicBinarySystem-1.0.7/LICENSE` & `SpectroscopicBinarySystem-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.0.7/PKG-INFO` & `SpectroscopicBinarySystem-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `SpectroscopicBinarySystem-1.0.7/README.md` & `SpectroscopicBinarySystem-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.0.7/setup.cfg` & `SpectroscopicBinarySystem-1.0.8/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 7065 6374 726f 7363 6f70 6963   = Spectroscopic
 00000020: 4269 6e61 7279 5379 7374 656d 0d0a 7665  BinarySystem..ve
-00000030: 7273 696f 6e20 3d20 312e 302e 370d 0a61  rsion = 1.0.7..a
+00000030: 7273 696f 6e20 3d20 312e 302e 380d 0a61  rsion = 1.0.8..a
 00000040: 7574 686f 7220 3d20 4775 696c 6c61 756d  uthor = Guillaum
 00000050: 6520 4265 7274 7261 6e64 0d0a 6175 7468  e Bertrand..auth
 00000060: 6f72 5f65 6d61 696c 203d 2067 6265 2e69  or_email = gbe.i
 00000070: 6f40 706d 2e6d 650d 0a64 6573 6372 6970  o@pm.me..descrip
 00000080: 7469 6f6e 203d 2050 7974 686f 6e20 6173  tion = Python as
 00000090: 7472 6f6e 6f6d 7920 746f 6f6c 7320 666f  tronomy tools fo
 000000a0: 7220 7370 6563 7472 6f73 636f 7069 6320  r spectroscopic 
@@ -20,33 +20,29 @@
 00000130: 655f 6669 6c65 7320 3d20 4c49 4345 4e53  e_files = LICENS
 00000140: 450d 0a6b 6579 776f 7264 7320 3d20 6173  E..keywords = as
 00000150: 7472 6f6e 6f6d 792c 6173 7472 6f70 6879  tronomy,astrophy
 00000160: 7369 6373 2c73 6369 656e 6365 2c66 6974  sics,science,fit
 00000170: 732c 6d6f 6465 6c73 2c66 6974 7469 6e67  s,models,fitting
 00000180: 2c73 7065 6374 726f 7363 6f70 792c 7370  ,spectroscopy,sp
 00000190: 6563 7472 756d 0d0a 0d0a 5b6f 7074 696f  ectrum....[optio
-000001a0: 6e73 5d0d 0a70 6163 6b61 6765 7320 3d20  ns]..packages = 
-000001b0: 6669 6e64 3a0d 0a70 6163 6b61 6765 5f64  find:..package_d
-000001c0: 6972 203d 200d 0a09 3d20 7370 6563 7472  ir = ...= spectr
-000001d0: 6f73 636f 7069 6362 696e 6172 7973 7973  oscopicbinarysys
-000001e0: 7465 6d0d 0a70 7974 686f 6e5f 7265 7175  tem..python_requ
-000001f0: 6972 6573 203d 203e 3d33 2e39 0d0a 696e  ires = >=3.9..in
-00000200: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
-00000210: 200d 0a09 6173 7472 6f70 793e 3d35 2e32   ...astropy>=5.2
-00000220: 2e32 0d0a 0961 7374 726f 7175 6572 793e  .2...astroquery>
-00000230: 3d30 2e34 2e36 0d0a 0942 696e 6172 7953  =0.4.6...BinaryS
-00000240: 7461 7253 6f6c 7665 723e 3d31 2e32 2e30  tarSolver>=1.2.0
-00000250: 0d0a 096d 6174 706c 6f74 6c69 623e 3d33  ...matplotlib>=3
-00000260: 2e37 2e31 0d0a 096e 756d 7079 3e3d 312e  .7.1...numpy>=1.
-00000270: 3234 2e32 0d0a 094f 7262 6974 616c 5079  24.2...OrbitalPy
-00000280: 3e3d 302e 372e 300d 0a09 5079 5941 4d4c  >=0.7.0...PyYAML
-00000290: 3e3d 362e 300d 0a09 7370 6563 7574 696c  >=6.0...specutil
-000002a0: 733e 3d31 2e39 2e31 0d0a 0942 696e 6172  s>=1.9.1...Binar
-000002b0: 7953 7461 7253 6f6c 7665 723e 3d31 2e32  yStarSolver>=1.2
-000002c0: 2e30 0d0a 0970 6c6f 746c 793e 3d35 2e31  .0...plotly>=5.1
-000002d0: 342e 310d 0a0d 0a5b 6f70 7469 6f6e 732e  4.1....[options.
-000002e0: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
-000002f0: 7768 6572 6520 3d20 7370 6563 7472 6f73  where = spectros
-00000300: 636f 7069 6362 696e 6172 7973 7973 7465  copicbinarysyste
-00000310: 6d0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  m....[egg_info].
-00000320: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-00000330: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+000001a0: 6e73 5d0d 0a6e 616d 6573 7061 6365 5f70  ns]..namespace_p
+000001b0: 6163 6b61 6765 7320 3d20 7370 6563 7472  ackages = spectr
+000001c0: 6f73 636f 7069 6362 696e 6172 7973 7973  oscopicbinarysys
+000001d0: 7465 6d0d 0a70 7974 686f 6e5f 7265 7175  tem..python_requ
+000001e0: 6972 6573 203d 203e 3d33 2e39 0d0a 696e  ires = >=3.9..in
+000001f0: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
+00000200: 200d 0a09 6173 7472 6f70 793e 3d35 2e32   ...astropy>=5.2
+00000210: 2e32 0d0a 0961 7374 726f 7175 6572 793e  .2...astroquery>
+00000220: 3d30 2e34 2e36 0d0a 0942 696e 6172 7953  =0.4.6...BinaryS
+00000230: 7461 7253 6f6c 7665 723e 3d31 2e32 2e30  tarSolver>=1.2.0
+00000240: 0d0a 096d 6174 706c 6f74 6c69 623e 3d33  ...matplotlib>=3
+00000250: 2e37 2e31 0d0a 096e 756d 7079 3e3d 312e  .7.1...numpy>=1.
+00000260: 3234 2e32 0d0a 094f 7262 6974 616c 5079  24.2...OrbitalPy
+00000270: 3e3d 302e 372e 300d 0a09 5079 5941 4d4c  >=0.7.0...PyYAML
+00000280: 3e3d 362e 300d 0a09 7370 6563 7574 696c  >=6.0...specutil
+00000290: 733e 3d31 2e39 2e31 0d0a 0942 696e 6172  s>=1.9.1...Binar
+000002a0: 7953 7461 7253 6f6c 7665 723e 3d31 2e32  yStarSolver>=1.2
+000002b0: 2e30 0d0a 0970 6c6f 746c 793e 3d35 2e31  .0...plotly>=5.1
+000002c0: 342e 310d 0a0d 0a5b 6567 675f 696e 666f  4.1....[egg_info
+000002d0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+000002e0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+000002f0: 0a                                       .
```

### Comparing `SpectroscopicBinarySystem-1.0.7/spectroscopicbinarysystem/SpectroscopicBinarySystem.egg-info/PKG-INFO` & `SpectroscopicBinarySystem-1.0.8/SpectroscopicBinarySystem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

