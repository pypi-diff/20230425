# Comparing `tmp/proteinTools-1.3.2.tar.gz` & `tmp/proteinTools-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-1.3.2.tar", last modified: Mon Apr 24 17:32:45 2023, max compression
+gzip compressed data, was "proteinTools-1.3.3.tar", last modified: Tue Apr 25 04:56:05 2023, max compression
```

## Comparing `proteinTools-1.3.2.tar` & `proteinTools-1.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-24 17:32:45.535031 proteinTools-1.3.2/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.3.2/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-24 17:32:45.531756 proteinTools-1.3.2/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.3.2/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-24 17:32:45.466620 proteinTools-1.3.2/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    52956 2023-04-24 17:31:02.000000 proteinTools-1.3.2/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.3.2/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-24 17:32:45.516576 proteinTools-1.3.2/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-24 17:32:45.000000 proteinTools-1.3.2/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-24 17:32:45.000000 proteinTools-1.3.2/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-24 17:32:45.000000 proteinTools-1.3.2/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-24 17:32:45.000000 proteinTools-1.3.2/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-24 17:32:45.000000 proteinTools-1.3.2/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-24 17:32:45.539361 proteinTools-1.3.2/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-24 17:32:26.000000 proteinTools-1.3.2/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-25 04:56:05.948302 proteinTools-1.3.3/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.3.3/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-25 04:56:05.944366 proteinTools-1.3.3/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.3.3/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-25 04:56:05.830642 proteinTools-1.3.3/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    53090 2023-04-25 04:55:56.000000 proteinTools-1.3.3/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.3.3/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-25 04:56:05.924874 proteinTools-1.3.3/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-25 04:56:05.000000 proteinTools-1.3.3/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-25 04:56:05.000000 proteinTools-1.3.3/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-25 04:56:05.000000 proteinTools-1.3.3/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-25 04:56:05.000000 proteinTools-1.3.3/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-25 04:56:05.000000 proteinTools-1.3.3/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-25 04:56:05.953320 proteinTools-1.3.3/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-25 04:55:23.000000 proteinTools-1.3.3/setup.py
```

### Comparing `proteinTools-1.3.2/LICENSE` & `proteinTools-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-1.3.2/proteinTools/PT.py` & `proteinTools-1.3.3/proteinTools/PT.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,15 +452,18 @@
                 sheet, helix, chainkeys = [], [], list(self.chains.keys())
                 for count, line in enumerate(data):
                     if line[0:6] == 'HETATM':
                         ligands = line[17:20]
                         if ligands == 'HOH':
                             break
                         if ligands != curr_lig:
-                            lignum = int(line[22:27])
+                            try:
+                                lignum = int(line[22:27])
+                            except:
+                                lignum = int(line[22:26])
                             if lignum != currnum:
                                 currnum = lignum
                                 lig = ligand(ligands)
                                 self.ligand_list.append(lig)
                                 current_ligand_index += 1
                         element = line[76:80].strip()
                         if element not in atom_keys:
```

### Comparing `proteinTools-1.3.2/setup.py` & `proteinTools-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name = "proteinTools",
-    version = "1.3.2",
+    version = "1.3.3",
     author = "Christian de Frondeville",
     description = "Lightweight, object-oriented bioinformatics package which simplifies interacting with proteins.",
     long_description = long_description,
     packages = ["proteinTools"],
     install_requires=['pandas','urllib3','chembl-webresource-client','mygene', 'pubchempy']
 )
```

