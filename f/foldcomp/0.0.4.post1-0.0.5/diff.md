# Comparing `tmp/foldcomp-0.0.4.post1.tar.gz` & `tmp/foldcomp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foldcomp-0.0.4.post1.tar", last modified: Wed Mar 29 13:37:52 2023, max compression
+gzip compressed data, was "foldcomp-0.0.5.tar", last modified: Tue Apr 25 10:56:14 2023, max compression
```

## Comparing `foldcomp-0.0.4.post1.tar` & `foldcomp-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:37:52.215109 foldcomp-0.0.4.post1/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-29 13:37:40.000000 foldcomp-0.0.4.post1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-03-29 13:37:40.000000 foldcomp-0.0.4.post1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-03-29 13:37:40.000000 foldcomp-0.0.4.post1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-29 13:37:40.000000 foldcomp-0.0.4.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-03-29 13:37:52.215109 foldcomp-0.0.4.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-03-29 13:37:40.000000 foldcomp-0.0.4.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:37:52.215109 foldcomp-0.0.4.post1/foldcomp/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-29 13:37:40.000000 foldcomp-0.0.4.post1/foldcomp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 13:37:40.000000 foldcomp-0.0.4.post1/foldcomp/foldcomp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-03-29 13:37:40.000000 foldcomp-0.0.4.post1/foldcomp/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:37:52.215109 foldcomp-0.0.4.post1/foldcomp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-03-29 13:37:52.000000 foldcomp-0.0.4.post1/foldcomp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-29 13:37:52.000000 foldcomp-0.0.4.post1/foldcomp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 13:37:52.000000 foldcomp-0.0.4.post1/foldcomp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-29 13:37:52.000000 foldcomp-0.0.4.post1/foldcomp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-29 13:37:52.000000 foldcomp-0.0.4.post1/foldcomp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-29 13:37:40.000000 foldcomp-0.0.4.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 13:37:52.215109 foldcomp-0.0.4.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-29 13:37:40.000000 foldcomp-0.0.4.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 13:37:52.215109 foldcomp-0.0.4.post1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-29 13:37:40.000000 foldcomp-0.0.4.post1/test/test_foldcomp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:56:14.500622 foldcomp-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-25 10:56:01.000000 foldcomp-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-25 10:56:01.000000 foldcomp-0.0.5/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-04-25 10:56:01.000000 foldcomp-0.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-25 10:56:01.000000 foldcomp-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-04-25 10:56:14.500622 foldcomp-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-04-25 10:56:01.000000 foldcomp-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:56:14.496622 foldcomp-0.0.5/foldcomp/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-25 10:56:01.000000 foldcomp-0.0.5/foldcomp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 10:56:01.000000 foldcomp-0.0.5/foldcomp/foldcomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-04-25 10:56:01.000000 foldcomp-0.0.5/foldcomp/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-25 10:56:01.000000 foldcomp-0.0.5/foldcomp/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:56:14.500622 foldcomp-0.0.5/foldcomp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-04-25 10:56:14.000000 foldcomp-0.0.5/foldcomp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-25 10:56:14.000000 foldcomp-0.0.5/foldcomp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:56:14.000000 foldcomp-0.0.5/foldcomp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-25 10:56:14.000000 foldcomp-0.0.5/foldcomp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 10:56:14.000000 foldcomp-0.0.5/foldcomp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-25 10:56:01.000000 foldcomp-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 10:56:14.500622 foldcomp-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-25 10:56:01.000000 foldcomp-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:56:14.500622 foldcomp-0.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-25 10:56:01.000000 foldcomp-0.0.5/test/test_foldcomp.py
```

### Comparing `foldcomp-0.0.4.post1/CMakeLists.txt` & `foldcomp-0.0.5/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `foldcomp-0.0.4.post1/LICENSE.txt` & `foldcomp-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foldcomp-0.0.4.post1/PKG-INFO` & `foldcomp-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foldcomp
-Version: 0.0.4.post1
+Version: 0.0.5
 Summary: Foldcomp compresses protein structures with torsion angles effectively. It compresses the backbone atoms to 8 bytes and the side chain to additionally 4-5 byes per residue, an averaged-sized protein of 350 residues requires ~4.2kb. Foldcomp is a C++ library with Python bindings.
 Author: Milot Mirdita <milot@mirdita.de>, Hyunbin Kim <khb7840@gmail.com>, Martin Steinegger <themartinsteinegger@gmail.com>
 License: GPLv3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.txt
@@ -26,15 +26,15 @@
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/steineggerlab/foldcomp/master/.github/img/format_benchmark_dark.png">
   <img src="https://raw.githubusercontent.com/steineggerlab/foldcomp/master/.github/img/format_benchmark_light.png" alt="Left panel: Foldcomp data format, saving amino acid residue in 13 byte. Top right panel:  Foldcomp decompression is as fast as gzip. Bottom right panel: Foldcomp compression ratio is higher than pulchra and gzip." max-width="720px" max-height="400px" width="auto" height="auto">
 </picture>
 </p>
 
 ## Publications
 
-[Hyunbin Kim, Milot Mirdita, and Martin Steinegger. Foldcomp: a library and format for compressing and indexing large protein structure sets. bioRxiv, doi:10.1101/2022.12.09.519715  (2022)](https://www.biorxiv.org/content/10.1101/2022.12.09.519715v1)
+[Hyunbin Kim, Milot Mirdita, Martin Steinegger, Foldcomp: a library and format for compressing and indexing large protein structure sets, Bioinformatics, 2023;, btad153,](https://doi.org/10.1093/bioinformatics/btad153)
 
 ## Usage
 
 ### Installing Foldcomp
 
 ```
 # Install Foldcomp Python package
```

### Comparing `foldcomp-0.0.4.post1/README.md` & `foldcomp-0.0.5/foldcomp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: foldcomp
+Version: 0.0.5
+Summary: Foldcomp compresses protein structures with torsion angles effectively. It compresses the backbone atoms to 8 bytes and the side chain to additionally 4-5 byes per residue, an averaged-sized protein of 350 residues requires ~4.2kb. Foldcomp is a C++ library with Python bindings.
+Author: Milot Mirdita <milot@mirdita.de>, Hyunbin Kim <khb7840@gmail.com>, Martin Steinegger <themartinsteinegger@gmail.com>
+License: GPLv3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE.txt
+
 # Foldcomp
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/steineggerlab/foldcomp/master/.github/img/foldcomp_strong_marv.png" max-height="300px" height="300" display="block" margin-left="auto" margin-right="auto" display="block"/>
 </p>
 Foldcomp compresses protein structures with torsion angles effectively. It compresses the backbone atoms to 8 bytes and the side chain to additionally 4-5 byes per residue, thus an averaged-sized protein of 350 residues requires ~6kb.
 
@@ -15,15 +26,15 @@
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/steineggerlab/foldcomp/master/.github/img/format_benchmark_dark.png">
   <img src="https://raw.githubusercontent.com/steineggerlab/foldcomp/master/.github/img/format_benchmark_light.png" alt="Left panel: Foldcomp data format, saving amino acid residue in 13 byte. Top right panel:  Foldcomp decompression is as fast as gzip. Bottom right panel: Foldcomp compression ratio is higher than pulchra and gzip." max-width="720px" max-height="400px" width="auto" height="auto">
 </picture>
 </p>
 
 ## Publications
 
-[Hyunbin Kim, Milot Mirdita, and Martin Steinegger. Foldcomp: a library and format for compressing and indexing large protein structure sets. bioRxiv, doi:10.1101/2022.12.09.519715  (2022)](https://www.biorxiv.org/content/10.1101/2022.12.09.519715v1)
+[Hyunbin Kim, Milot Mirdita, Martin Steinegger, Foldcomp: a library and format for compressing and indexing large protein structure sets, Bioinformatics, 2023;, btad153,](https://doi.org/10.1093/bioinformatics/btad153)
 
 ## Usage
 
 ### Installing Foldcomp
 
 ```
 # Install Foldcomp Python package
```

### Comparing `foldcomp-0.0.4.post1/foldcomp/setup.py` & `foldcomp-0.0.5/foldcomp/setup.py`

 * *Files identical despite different names*

### Comparing `foldcomp-0.0.4.post1/foldcomp.egg-info/PKG-INFO` & `foldcomp-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: foldcomp
-Version: 0.0.4.post1
-Summary: Foldcomp compresses protein structures with torsion angles effectively. It compresses the backbone atoms to 8 bytes and the side chain to additionally 4-5 byes per residue, an averaged-sized protein of 350 residues requires ~4.2kb. Foldcomp is a C++ library with Python bindings.
-Author: Milot Mirdita <milot@mirdita.de>, Hyunbin Kim <khb7840@gmail.com>, Martin Steinegger <themartinsteinegger@gmail.com>
-License: GPLv3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE.txt
-
 # Foldcomp
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/steineggerlab/foldcomp/master/.github/img/foldcomp_strong_marv.png" max-height="300px" height="300" display="block" margin-left="auto" margin-right="auto" display="block"/>
 </p>
 Foldcomp compresses protein structures with torsion angles effectively. It compresses the backbone atoms to 8 bytes and the side chain to additionally 4-5 byes per residue, thus an averaged-sized protein of 350 residues requires ~6kb.
 
@@ -26,15 +15,15 @@
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/steineggerlab/foldcomp/master/.github/img/format_benchmark_dark.png">
   <img src="https://raw.githubusercontent.com/steineggerlab/foldcomp/master/.github/img/format_benchmark_light.png" alt="Left panel: Foldcomp data format, saving amino acid residue in 13 byte. Top right panel:  Foldcomp decompression is as fast as gzip. Bottom right panel: Foldcomp compression ratio is higher than pulchra and gzip." max-width="720px" max-height="400px" width="auto" height="auto">
 </picture>
 </p>
 
 ## Publications
 
-[Hyunbin Kim, Milot Mirdita, and Martin Steinegger. Foldcomp: a library and format for compressing and indexing large protein structure sets. bioRxiv, doi:10.1101/2022.12.09.519715  (2022)](https://www.biorxiv.org/content/10.1101/2022.12.09.519715v1)
+[Hyunbin Kim, Milot Mirdita, Martin Steinegger, Foldcomp: a library and format for compressing and indexing large protein structure sets, Bioinformatics, 2023;, btad153,](https://doi.org/10.1093/bioinformatics/btad153)
 
 ## Usage
 
 ### Installing Foldcomp
 
 ```
 # Install Foldcomp Python package
```

### Comparing `foldcomp-0.0.4.post1/setup.py` & `foldcomp-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from skbuild import setup
 
 setup(
     name="foldcomp",
-    version="0.0.4-1",
+    version="0.0.5",
     description="Foldcomp compresses protein structures with torsion angles effectively. It compresses the backbone atoms to 8 bytes and the side chain to additionally 4-5 byes per residue, an averaged-sized protein of 350 residues requires ~4.2kb. Foldcomp is a C++ library with Python bindings.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Milot Mirdita <milot@mirdita.de>, Hyunbin Kim <khb7840@gmail.com>, Martin Steinegger <themartinsteinegger@gmail.com>",
     license="GPLv3",
     cmake_args=["-DBUILD_PYTHON:BOOL=ON"],
     python_requires=">=3.7",
```

### Comparing `foldcomp-0.0.4.post1/test/test_foldcomp.py` & `foldcomp-0.0.5/test/test_foldcomp.py`

 * *Files identical despite different names*

