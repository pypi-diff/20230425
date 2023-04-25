# Comparing `tmp/pybio-0.3.2.tar.gz` & `tmp/pybio-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybio-0.3.2.tar", last modified: Thu Apr  6 08:10:20 2023, max compression
+gzip compressed data, was "pybio-0.3.3.tar", last modified: Tue Apr 25 10:50:51 2023, max compression
```

## Comparing `pybio-0.3.2.tar` & `pybio-0.3.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-06 08:10:20.473858 pybio-0.3.2/
--rw-rw-r--   0 rotg     (2023757) games       (20)     9431 2023-04-06 08:10:20.473552 pybio-0.3.2/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) games       (20)     9200 2023-04-03 07:10:50.000000 pybio-0.3.2/README.md
--rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-04-06 08:10:20.473972 pybio-0.3.2/setup.cfg
--rw-rw-r--   0 rotg     (2023757) games       (20)      864 2023-04-06 08:09:27.000000 pybio-0.3.2/setup.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-06 08:10:20.450166 pybio-0.3.2/src/
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-06 08:10:20.455117 pybio-0.3.2/src/pybio/
--rw-rw-r--   0 rotg     (2023757) games       (20)     7599 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-06 08:10:20.459108 pybio-0.3.2/src/pybio/config/
--rw-rw-r--   0 rotg     (2023757) games       (20)     1930 2023-04-03 07:11:00.000000 pybio-0.3.2/src/pybio/config/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-06 08:10:20.459771 pybio-0.3.2/src/pybio/core/
--rw-rw-r--   0 rotg     (2023757) games       (20)       98 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/core/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    25251 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/core/genomes.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-06 08:10:20.466778 pybio-0.3.2/src/pybio/data/
--rw-rw-r--   0 rotg     (2023757) games       (20)      877 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/data/Bam.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    16391 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/data/Bedgraph.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     4675 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/data/Bedgraph2.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1912 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/data/Fasta.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1244 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/data/Fastq.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1591 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/data/Gene.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      177 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/data/GeneFeature.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     3238 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/data/Gff3.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2777 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/data/Gtf.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      186 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/data/Sequence.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      906 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/data/Sissrs.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      956 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/data/TabReader.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2019 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/data/Wig.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2168 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/data/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-06 08:10:20.467109 pybio-0.3.2/src/pybio/expression/
--rw-rw-r--   0 rotg     (2023757) games       (20)     8831 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/expression/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-06 08:10:20.469773 pybio-0.3.2/src/pybio/map/
--rw-rw-r--   0 rotg     (2023757) games       (20)     2257 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/map/STAR.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      131 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/map/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1438 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/map/bowtie.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      580 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/map/nano.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1061 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/map/sege.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-06 08:10:20.470950 pybio-0.3.2/src/pybio/maths/
--rw-rw-r--   0 rotg     (2023757) games       (20)      974 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/maths/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    37335 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/maths/pstat.py
--rw-rw-r--   0 rotg     (2023757) games       (20)   151400 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/maths/stats.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-06 08:10:20.472346 pybio-0.3.2/src/pybio/path/
--rw-rw-r--   0 rotg     (2023757) games       (20)      347 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/path/__init__.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)     3537 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/pybio
--rw-rw-r--   0 rotg     (2023757) games       (20)      101 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/pybio.config.example
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-06 08:10:20.472687 pybio-0.3.2/src/pybio/sequence/
--rw-rw-r--   0 rotg     (2023757) games       (20)     5566 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/sequence/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-06 08:10:20.473052 pybio-0.3.2/src/pybio/utils/
--rw-rw-r--   0 rotg     (2023757) games       (20)    10199 2023-04-03 07:10:50.000000 pybio-0.3.2/src/pybio/utils/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-06 08:10:20.458433 pybio-0.3.2/src/pybio.egg-info/
--rw-rw-r--   0 rotg     (2023757) games       (20)     9431 2023-04-06 08:10:20.455894 pybio-0.3.2/src/pybio.egg-info/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) games       (20)     1030 2023-04-06 08:10:20.456186 pybio-0.3.2/src/pybio.egg-info/SOURCES.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-04-06 08:10:20.457699 pybio-0.3.2/src/pybio.egg-info/dependency_links.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-04-06 07:45:01.000000 pybio-0.3.2/src/pybio.egg-info/not-zip-safe
--rw-rw-r--   0 rotg     (2023757) games       (20)       32 2023-04-06 08:10:20.458239 pybio-0.3.2/src/pybio.egg-info/requires.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-04-06 08:10:20.458554 pybio-0.3.2/src/pybio.egg-info/top_level.txt
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-25 10:50:51.885418 pybio-0.3.3/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     9431 2023-04-25 10:50:51.885120 pybio-0.3.3/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) games       (20)     9200 2023-04-03 07:10:50.000000 pybio-0.3.3/README.md
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-25 10:50:51.866587 pybio-0.3.3/pybio/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     7879 2023-04-21 08:49:23.000000 pybio-0.3.3/pybio/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-25 10:50:51.869228 pybio-0.3.3/pybio/config/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1957 2023-04-18 08:14:24.000000 pybio-0.3.3/pybio/config/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-25 10:50:51.870114 pybio-0.3.3/pybio/core/
+-rw-rw-r--   0 rotg     (2023757) games       (20)       98 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/core/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    25716 2023-04-18 13:19:58.000000 pybio-0.3.3/pybio/core/genomes.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-25 10:50:51.877292 pybio-0.3.3/pybio/data/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      877 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/data/Bam.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    16391 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/data/Bedgraph.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     4675 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/data/Bedgraph2.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1912 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/data/Fasta.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1244 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/data/Fastq.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1591 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/data/Gene.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      177 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/data/GeneFeature.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     3238 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/data/Gff3.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2777 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/data/Gtf.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      186 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/data/Sequence.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      906 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/data/Sissrs.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      956 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/data/TabReader.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2019 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/data/Wig.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2168 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/data/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-25 10:50:51.877737 pybio-0.3.3/pybio/expression/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     8831 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/expression/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-25 10:50:51.880448 pybio-0.3.3/pybio/map/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2257 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/map/STAR.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      131 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/map/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1438 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/map/bowtie.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      580 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/map/nano.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1061 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/map/sege.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-25 10:50:51.882403 pybio-0.3.3/pybio/maths/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      974 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/maths/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    37335 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/maths/pstat.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)   151400 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/maths/stats.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-25 10:50:51.883298 pybio-0.3.3/pybio/path/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      347 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/path/__init__.py
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     4906 2023-04-25 10:49:49.000000 pybio-0.3.3/pybio/pybio
+-rw-rw-r--   0 rotg     (2023757) games       (20)      101 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/pybio.config.example
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-25 10:50:51.883677 pybio-0.3.3/pybio/sequence/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5566 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/sequence/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-25 10:50:51.884304 pybio-0.3.3/pybio/utils/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    10199 2023-04-17 06:24:09.000000 pybio-0.3.3/pybio/utils/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-04-25 10:50:45.000000 pybio-0.3.3/pybio/version
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-25 10:50:51.868875 pybio-0.3.3/pybio.egg-info/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     9431 2023-04-25 10:50:51.867064 pybio-0.3.3/pybio.egg-info/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) games       (20)      892 2023-04-25 10:50:51.867407 pybio-0.3.3/pybio.egg-info/SOURCES.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-04-25 10:50:51.867926 pybio-0.3.3/pybio.egg-info/dependency_links.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-04-18 08:10:15.000000 pybio-0.3.3/pybio.egg-info/not-zip-safe
+-rw-rw-r--   0 rotg     (2023757) games       (20)       32 2023-04-25 10:50:51.868629 pybio-0.3.3/pybio.egg-info/requires.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-04-25 10:50:51.868943 pybio-0.3.3/pybio.egg-info/top_level.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-04-25 10:50:51.885496 pybio-0.3.3/setup.cfg
+-rw-rw-r--   0 rotg     (2023757) games       (20)      949 2023-04-17 08:00:52.000000 pybio-0.3.3/setup.py
```

### Comparing `pybio-0.3.2/PKG-INFO` & `pybio-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybio
-Version: 0.3.2
+Version: 0.3.3
 Summary: pybio genomics
 Home-page: https://github.com/grexor/pybio
 Author: Gregor Rot
 Author-email: gregor.rot@gmail.com
 Keywords: pybio,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pybio-0.3.2/README.md` & `pybio-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/__init__.py` & `pybio-0.3.3/pybio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,22 @@
 import pybio.utils
 import pybio.expression
 import pybio.maths
 import pybio.config
 import pybio.sequence
 import pybio.core
 
+pybio_path = os.path.abspath(__file__)
+pybio_folder = os.path.dirname(pybio_path)
+version = open(os.path.join(pybio_folder, "version"), "rt").readlines()[0].replace("\n", "").replace("\r", "")
+
+print(f"[pybio] v{version}")
+print("Github: https://github.com/grexor/pybio")
+print()
+
 # initialize path module
 pybio.config.init()
 pybio.path.init()
 pybio.core.genomes.init()
 
 def genome_download(species, genome_version, args):
     print(f"[pybio genome_download] species {species} and version {genome_version}")
@@ -115,21 +123,21 @@
         if not genomes_ready.get(species, {}).get(genome_version, {}).get("STAR", False) or not os.path.exists(star_folder):
             return_code = pybio.core.genomes.star_index(species, genome_version)
             if return_code==0:
                 genomes_ready[species][genome_version]["STAR"] = True
             else:
                 genomes_ready[species][genome_version]["STAR"] = False
         else:
-            print(f"[pybio genome] STAR index ready at {pybio.config.genomes_folder}/{species}.annotation.{genome_version}.star")
+            print(f"[pybio genome] STAR index ready at {pybio.config.genomes_folder}/{species}.assembly.{genome_version}.star")
 
     if pybio.utils.is_tool("salmon") and not args.nosalmon:
         salmon_folder = os.path.join(pybio.config.genomes_folder, f"{species}.transcripts.{genome_version}.salmon")
         if not genomes_ready.get(species, {}).get(genome_version, {}).get("salmon", False) or not os.path.exists(salmon_folder):
             return_code = pybio.core.genomes.salmon_index(species, genome_version)
             if return_code==0:
                 genomes_ready[species][genome_version]["salmon"] = True
             else:
                 genomes_ready[species][genome_version]["salmon"] = False
         else:
-            print(f"[pybio genome] salmon index ready at {pybio.config.genomes_folder}/{species}.annotation.{genome_version}.salmon")
+            print(f"[pybio genome] salmon index ready at {pybio.config.genomes_folder}/{species}.transcripts.{genome_version}.salmon")
 
     json.dump(genomes_ready, open(genomes_ready_fname, "wt"))
```

### Comparing `pybio-0.3.2/src/pybio/config/__init__.py` & `pybio-0.3.3/pybio/config/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     config_module = sys.modules[__name__]
     pybio_folder = os.path.abspath(os.path.join(os.path.abspath(__file__), "..", "..")) 
     config_file = os.path.abspath(os.path.join(pybio_folder, "pybio.config"))
     config_example_file = os.path.abspath(os.path.join(pybio_folder, "pybio.config.example"))
     if not os.path.exists(config_file):
         os.system(f"cp {config_example_file} {config_file}")
     config_lines = open(config_file).readlines()
-    print(f"Note: all paths are relative to the pybio home folder {pybio_folder}.")
+    print(f"Note: you can specify absolute or relative paths. Relative paths are relative to: {pybio_folder}")
     print()
     new_config = []
     for cline in config_lines:
         if cline.startswith("#"):
             continue
         k, v = cline.split("=")
         v = v.replace("\n", "").replace("\r", "").replace("\"", "").replace("'", "")
```

### Comparing `pybio-0.3.2/src/pybio/core/genomes.py` & `pybio-0.3.3/pybio/core/genomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         pybio.core.genomes.list_species_ensembl()
     f = open(os.path.join(pybio.config.genomes_folder, "genome_species.tab"), "rt")
     header = f.readline().replace("\r", "").replace("\n", "").split("\t")
     r = f.readline()
     while r:
         r = r.replace("\r", "").replace("\n", "").split("\t")
         data = dict(zip(header, r))
-        species_db[data["species"]] = {"assembly": data["assembly"], "genome_version": data["genome_version"], "provider": data["provider"], "provider_subfolder": data["provider_subfolder"]}
+        species_db[data["species"]] = {"display_name":data["display_name"], "assembly": data["assembly"], "genome_version": data["genome_version"], "provider": data["provider"], "provider_subfolder": data["provider_subfolder"]}
         r = f.readline()
     f.close()
 
 def prepare(species="homo_sapiens", genome_version=None):
     print("[pybio] {species}: processing annotation".format(species=species))
     provider = species_db[species]["provider"]
     if genome_version==None:
@@ -240,15 +240,14 @@
     return r.status_code == requests.codes.ok
 
 def download_assembly(species, genome_version):
     if genome_version==None:
         return False
     species_capital = species.capitalize()
     assembly = species_db[species]["assembly"]
-    print(assembly)
     ensembl_version = genome_version.replace("ensembl", "")
     ensembl_version = ensembl_version.replace("genomes", "")
 
     ftp_address = providers_ftp[species_db[species]["provider"]]
     subfolder = species_db[species]["provider_subfolder"]
     if subfolder!="":
         ftp_address = f"{ftp_address}/{subfolder}"
@@ -369,29 +368,38 @@
     r = requests.get(server+ext, headers={ "Content-Type" : "application/json"})
     if not r.ok:
         r.raise_for_status()
         sys.exit()
     decoded = r.json()
     return str(decoded["version"])
 
+def get_genome_info(genome_id): 
+  server = "https://rest.ensembl.org"
+  ext = f"/info/genomes/{genome_id}?"
+  r = requests.get(server+ext, headers={ "Content-Type" : "application/json"})
+  if not r.ok:
+      return {}
+  decoded = r.json()
+  return decoded
+
 def list_species_ensembl():
     print("[pybio.core.genomes] Species list from Ensembl; done once and takes ~ 1 minute")
     ensembl_version = get_latest_ensembl()
     ensemblgenomes_version = get_latest_ensemblgenomes()
     from bs4 import BeautifulSoup
     import requests
     species_db = {}
     def listFD(url, ext=''):
         page = requests.get(url).text
         soup = BeautifulSoup(page, 'html.parser')
         return [node.get('href')[:-1] for node in soup.find_all('a') if node.get('href').endswith(ext)]
     if not os.path.exists(pybio.config.genomes_folder):
         os.makedirs(pybio.config.genomes_folder)
     f = open(os.path.join(pybio.config.genomes_folder, "genome_species.tab"), "wt")
-    f.write("species\tassembly\tprovider\tprovider_subfolder\tgenome_version\n")
+    f.write("species\tassembly\tprovider\tprovider_subfolder\tgenome_version\tdisplay_name\n")
     for species in listFD(f"https://ftp.ensembl.org/pub/release-{ensembl_version}/fasta/", "/")[1:]:
         print(f"[pybio.core.genomes] Checking {species}" + " "*30, end="\r")
         dna_folder_url = f"https://ftp.ensembl.org/pub/release-{ensembl_version}/fasta/{species}/dna/"
         fasta_file = listFD(dna_folder_url, ext='.dna.primary_assembly.fa.gz')
         if len(fasta_file)==0:
             fasta_file = listFD(dna_folder_url, ext='.dna.toplevel.fa.gz')
         if len(fasta_file)==0:
@@ -400,15 +408,16 @@
             print(f"[pybio.core.genomes] skipping {species}, no fasta file found")
             continue
         fasta_file = fasta_file[0]
         species_assembly = fasta_file.replace(".dna.toplevel.fa.g", "").replace(".dna.primary_assembly.fa.g", "").replace(".dna.nonchromosomal.fa.g", "").split(".")
         species_long = species_assembly[0]
         species_assembly = ".".join(species_assembly[1:])
         species_db[species] = (species, species_assembly)
-        f.write(f"{species}\t{species_assembly}\tensembl\t\tensembl{ensembl_version}\n")
+        genome_data = get_genome_info(species)
+        f.write(f"{species}\t{species_assembly}\tensembl\t\tensembl{ensembl_version}\t{genome_data.get('display_name', '')}\n")
         assert(species.capitalize()==species_long)
 
     for subfolder in ["plants", "fungi", "protists", "metazoa"]:
         print(f"[pybio.core.genomes] Species list from Ensembl Genomes: {subfolder}; done once and takes ~ 1 minute")
         for species in listFD(f"https://ftp.ensemblgenomes.ebi.ac.uk/pub/{subfolder}/release-{ensemblgenomes_version}/fasta/", "/")[1:]:
             print(f"[pybio.core.genomes] Checking {species}" + " "*30, end="\r")
             dna_folder_url = f"https://ftp.ensemblgenomes.ebi.ac.uk/pub/{subfolder}/release-{ensemblgenomes_version}/fasta/{species}/dna/"
@@ -417,15 +426,16 @@
                 print(f"[pybio.core.genomes] Skipping {species}, no fasta file found")
                 continue
             fasta_file = fasta_file[0]
             species_assembly = fasta_file.replace(".dna.toplevel.fa.g", "").split(".")
             species_long = species_assembly[0]
             species_assembly = ".".join(species_assembly[1:])
             species_db[species] = (species, species_assembly)
-            f.write(f"{species}\t{species_assembly}\tensemblgenomes\t{subfolder}\tensemblgenomes{ensemblgenomes_version}\n")
+            genome_data = get_genome_info(species)
+            f.write(f"{species}\t{species_assembly}\tensemblgenomes\t{subfolder}\tensemblgenomes{ensemblgenomes_version}\t{genome_data.get('display_name', '')}\n")
             assert(species.capitalize()==species_long)
 
     f.close()
     print()
     print("[pybio.core.genomes] Complete species list downloaded to:", os.path.join(pybio.config.genomes_folder, "genome_species.tab"))
     print()
     print("[pybio.core.genomes] Example command to download and process homo_sapiens genome:")
```

### Comparing `pybio-0.3.2/src/pybio/data/Bam.py` & `pybio-0.3.3/pybio/data/Bam.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/data/Bedgraph.py` & `pybio-0.3.3/pybio/data/Bedgraph.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/data/Bedgraph2.py` & `pybio-0.3.3/pybio/data/Bedgraph2.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/data/Fasta.py` & `pybio-0.3.3/pybio/data/Fasta.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/data/Fastq.py` & `pybio-0.3.3/pybio/data/Fastq.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/data/Gene.py` & `pybio-0.3.3/pybio/data/Gene.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/data/Gff3.py` & `pybio-0.3.3/pybio/data/Gff3.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/data/Gtf.py` & `pybio-0.3.3/pybio/data/Gtf.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/data/Sissrs.py` & `pybio-0.3.3/pybio/data/Sissrs.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/data/TabReader.py` & `pybio-0.3.3/pybio/data/TabReader.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/data/Wig.py` & `pybio-0.3.3/pybio/data/Wig.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/data/__init__.py` & `pybio-0.3.3/pybio/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/expression/__init__.py` & `pybio-0.3.3/pybio/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/map/STAR.py` & `pybio-0.3.3/pybio/map/STAR.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/map/bowtie.py` & `pybio-0.3.3/pybio/map/bowtie.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/map/nano.py` & `pybio-0.3.3/pybio/map/nano.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/map/sege.py` & `pybio-0.3.3/pybio/map/sege.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/maths/__init__.py` & `pybio-0.3.3/pybio/maths/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/maths/pstat.py` & `pybio-0.3.3/pybio/maths/pstat.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/maths/stats.py` & `pybio-0.3.3/pybio/maths/stats.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/sequence/__init__.py` & `pybio-0.3.3/pybio/sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio/utils/__init__.py` & `pybio-0.3.3/pybio/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.2/src/pybio.egg-info/PKG-INFO` & `pybio-0.3.3/pybio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybio
-Version: 0.3.2
+Version: 0.3.3
 Summary: pybio genomics
 Home-page: https://github.com/grexor/pybio
 Author: Gregor Rot
 Author-email: gregor.rot@gmail.com
 Keywords: pybio,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

