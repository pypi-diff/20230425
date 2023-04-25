# Comparing `tmp/htseq-clip-2.8.0b0.tar.gz` & `tmp/htseq-clip-2.9.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/htseq-clip-2.8.0b0.tar", last modified: Fri Sep  3 08:01:07 2021, max compression
+gzip compressed data, was "dist/htseq-clip-2.9.0b0.tar", last modified: Mon Dec  6 13:58:39 2021, max compression
```

## Comparing `htseq-clip-2.8.0b0.tar` & `htseq-clip-2.9.0b0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 sahadeva (21993) hentze     (453)        0 2021-09-03 08:01:07.000000 htseq-clip-2.8.0b0/
--rw-r--r--   0 sahadeva (21993) hentze     (453)     2000 2021-09-03 08:01:07.000000 htseq-clip-2.8.0b0/PKG-INFO
--rw-r--r--   0 sahadeva (21993) hentze     (453)     1088 2020-06-19 09:20:08.000000 htseq-clip-2.8.0b0/README.md
-drwxr-xr-x   0 sahadeva (21993) hentze     (453)        0 2021-09-03 08:01:07.000000 htseq-clip-2.8.0b0/clip/
--rw-r--r--   0 sahadeva (21993) hentze     (453)     5420 2020-01-24 09:01:03.000000 htseq-clip-2.8.0b0/clip/GTxFeature.py
--rw-r--r--   0 sahadeva (21993) hentze     (453)    15256 2020-01-24 09:01:03.000000 htseq-clip-2.8.0b0/clip/Gene.py
--rw-r--r--   0 sahadeva (21993) hentze     (453)     1796 2020-01-24 09:01:03.000000 htseq-clip-2.8.0b0/clip/GeneLengthSummary.py
--rw-r--r--   0 sahadeva (21993) hentze     (453)     4071 2020-01-24 09:01:03.000000 htseq-clip-2.8.0b0/clip/GeneRegion.py
--rwxr-xr-x   0 sahadeva (21993) hentze     (453)        0 2019-04-08 13:18:24.000000 htseq-clip-2.8.0b0/clip/__init__.py
--rw-r--r--   0 sahadeva (21993) hentze     (453)    20634 2021-07-12 07:58:21.000000 htseq-clip-2.8.0b0/clip/bamCLIP.py
--rwxr-xr-x   0 sahadeva (21993) hentze     (453)    33911 2020-01-24 09:01:03.000000 htseq-clip-2.8.0b0/clip/bedCLIP.py
--rw-r--r--   0 sahadeva (21993) hentze     (453)    16695 2021-09-03 07:44:18.000000 htseq-clip-2.8.0b0/clip/clip.py
--rw-r--r--   0 sahadeva (21993) hentze     (453)       47 2020-01-24 09:01:03.000000 htseq-clip-2.8.0b0/clip/command_line.py
--rw-r--r--   0 sahadeva (21993) hentze     (453)    13156 2020-01-24 09:01:03.000000 htseq-clip-2.8.0b0/clip/countCLIP.py
--rwxr-xr-x   0 sahadeva (21993) hentze     (453)     4150 2021-09-03 07:58:47.000000 htseq-clip-2.8.0b0/clip/createMatrix.py
--rw-r--r--   0 sahadeva (21993) hentze     (453)    12555 2021-07-13 07:40:53.000000 htseq-clip-2.8.0b0/clip/gffCLIP.py
--rw-r--r--   0 sahadeva (21993) hentze     (453)     1182 2021-07-08 10:22:40.000000 htseq-clip-2.8.0b0/clip/output.py
-drwxr-xr-x   0 sahadeva (21993) hentze     (453)        0 2021-09-03 08:01:07.000000 htseq-clip-2.8.0b0/htseq_clip.egg-info/
--rw-r--r--   0 sahadeva (21993) hentze     (453)     2000 2021-09-03 08:01:04.000000 htseq-clip-2.8.0b0/htseq_clip.egg-info/PKG-INFO
--rw-r--r--   0 sahadeva (21993) hentze     (453)      610 2021-09-03 08:01:05.000000 htseq-clip-2.8.0b0/htseq_clip.egg-info/SOURCES.txt
--rw-r--r--   0 sahadeva (21993) hentze     (453)        1 2021-09-03 08:01:04.000000 htseq-clip-2.8.0b0/htseq_clip.egg-info/dependency_links.txt
--rw-r--r--   0 sahadeva (21993) hentze     (453)       55 2021-09-03 08:01:04.000000 htseq-clip-2.8.0b0/htseq_clip.egg-info/entry_points.txt
--rw-r--r--   0 sahadeva (21993) hentze     (453)        1 2020-02-24 13:56:56.000000 htseq-clip-2.8.0b0/htseq_clip.egg-info/not-zip-safe
--rw-r--r--   0 sahadeva (21993) hentze     (453)       12 2021-09-03 08:01:04.000000 htseq-clip-2.8.0b0/htseq_clip.egg-info/requires.txt
--rw-r--r--   0 sahadeva (21993) hentze     (453)       11 2021-09-03 08:01:04.000000 htseq-clip-2.8.0b0/htseq_clip.egg-info/top_level.txt
--rwxr-xr-x   0 sahadeva (21993) hentze     (453)       67 2021-09-03 08:01:07.000000 htseq-clip-2.8.0b0/setup.cfg
--rwxr-xr-x   0 sahadeva (21993) hentze     (453)     2141 2021-09-03 07:59:32.000000 htseq-clip-2.8.0b0/setup.py
-drwxr-xr-x   0 sahadeva (21993) hentze     (453)        0 2021-09-03 08:01:07.000000 htseq-clip-2.8.0b0/tests/
--rwxr-xr-x   0 sahadeva (21993) hentze     (453)        0 2020-01-24 09:01:03.000000 htseq-clip-2.8.0b0/tests/__init__.py
--rw-r--r--   0 sahadeva (21993) hentze     (453)     6984 2021-07-12 08:23:09.000000 htseq-clip-2.8.0b0/tests/bamCLIP_test.py
--rw-r--r--   0 sahadeva (21993) hentze     (453)     2525 2020-01-24 09:01:03.000000 htseq-clip-2.8.0b0/tests/countCLIP_test.py
--rw-r--r--   0 sahadeva (21993) hentze     (453)     1092 2020-01-24 09:01:03.000000 htseq-clip-2.8.0b0/tests/createMatrix_test.py
--rw-r--r--   0 sahadeva (21993) hentze     (453)     4354 2020-01-24 09:01:03.000000 htseq-clip-2.8.0b0/tests/gffCLIP_test.py
+drwxr-xr-x   0 sahadeva (21993) hentze     (453)        0 2021-12-06 13:58:39.000000 htseq-clip-2.9.0b0/
+-rw-r--r--   0 sahadeva (21993) hentze     (453)     2000 2021-12-06 13:58:39.000000 htseq-clip-2.9.0b0/PKG-INFO
+-rw-r--r--   0 sahadeva (21993) hentze     (453)     1088 2020-06-19 09:20:08.000000 htseq-clip-2.9.0b0/README.md
+drwxr-xr-x   0 sahadeva (21993) hentze     (453)        0 2021-12-06 13:58:39.000000 htseq-clip-2.9.0b0/clip/
+-rw-r--r--   0 sahadeva (21993) hentze     (453)     5420 2020-01-24 09:01:03.000000 htseq-clip-2.9.0b0/clip/GTxFeature.py
+-rw-r--r--   0 sahadeva (21993) hentze     (453)    15256 2020-01-24 09:01:03.000000 htseq-clip-2.9.0b0/clip/Gene.py
+-rw-r--r--   0 sahadeva (21993) hentze     (453)     1796 2020-01-24 09:01:03.000000 htseq-clip-2.9.0b0/clip/GeneLengthSummary.py
+-rw-r--r--   0 sahadeva (21993) hentze     (453)     4071 2020-01-24 09:01:03.000000 htseq-clip-2.9.0b0/clip/GeneRegion.py
+-rwxr-xr-x   0 sahadeva (21993) hentze     (453)        0 2019-04-08 13:18:24.000000 htseq-clip-2.9.0b0/clip/__init__.py
+-rw-r--r--   0 sahadeva (21993) hentze     (453)    20634 2021-07-12 07:58:21.000000 htseq-clip-2.9.0b0/clip/bamCLIP.py
+-rwxr-xr-x   0 sahadeva (21993) hentze     (453)    33911 2020-01-24 09:01:03.000000 htseq-clip-2.9.0b0/clip/bedCLIP.py
+-rw-r--r--   0 sahadeva (21993) hentze     (453)    16696 2021-11-29 11:52:06.000000 htseq-clip-2.9.0b0/clip/clip.py
+-rw-r--r--   0 sahadeva (21993) hentze     (453)       47 2020-01-24 09:01:03.000000 htseq-clip-2.9.0b0/clip/command_line.py
+-rw-r--r--   0 sahadeva (21993) hentze     (453)    13156 2020-01-24 09:01:03.000000 htseq-clip-2.9.0b0/clip/countCLIP.py
+-rwxr-xr-x   0 sahadeva (21993) hentze     (453)     4150 2021-09-03 07:58:47.000000 htseq-clip-2.9.0b0/clip/createMatrix.py
+-rw-r--r--   0 sahadeva (21993) hentze     (453)    12555 2021-07-13 07:40:53.000000 htseq-clip-2.9.0b0/clip/gffCLIP.py
+-rw-r--r--   0 sahadeva (21993) hentze     (453)     1182 2021-07-08 10:22:40.000000 htseq-clip-2.9.0b0/clip/output.py
+drwxr-xr-x   0 sahadeva (21993) hentze     (453)        0 2021-12-06 13:58:39.000000 htseq-clip-2.9.0b0/htseq_clip.egg-info/
+-rw-r--r--   0 sahadeva (21993) hentze     (453)     2000 2021-12-06 13:58:35.000000 htseq-clip-2.9.0b0/htseq_clip.egg-info/PKG-INFO
+-rw-r--r--   0 sahadeva (21993) hentze     (453)      610 2021-12-06 13:58:36.000000 htseq-clip-2.9.0b0/htseq_clip.egg-info/SOURCES.txt
+-rw-r--r--   0 sahadeva (21993) hentze     (453)        1 2021-12-06 13:58:35.000000 htseq-clip-2.9.0b0/htseq_clip.egg-info/dependency_links.txt
+-rw-r--r--   0 sahadeva (21993) hentze     (453)       55 2021-12-06 13:58:35.000000 htseq-clip-2.9.0b0/htseq_clip.egg-info/entry_points.txt
+-rw-r--r--   0 sahadeva (21993) hentze     (453)        1 2020-02-24 13:56:56.000000 htseq-clip-2.9.0b0/htseq_clip.egg-info/not-zip-safe
+-rw-r--r--   0 sahadeva (21993) hentze     (453)       20 2021-12-06 13:58:35.000000 htseq-clip-2.9.0b0/htseq_clip.egg-info/requires.txt
+-rw-r--r--   0 sahadeva (21993) hentze     (453)       11 2021-12-06 13:58:35.000000 htseq-clip-2.9.0b0/htseq_clip.egg-info/top_level.txt
+-rwxr-xr-x   0 sahadeva (21993) hentze     (453)       67 2021-12-06 13:58:39.000000 htseq-clip-2.9.0b0/setup.cfg
+-rwxr-xr-x   0 sahadeva (21993) hentze     (453)     2149 2021-12-06 13:57:14.000000 htseq-clip-2.9.0b0/setup.py
+drwxr-xr-x   0 sahadeva (21993) hentze     (453)        0 2021-12-06 13:58:39.000000 htseq-clip-2.9.0b0/tests/
+-rwxr-xr-x   0 sahadeva (21993) hentze     (453)        0 2020-01-24 09:01:03.000000 htseq-clip-2.9.0b0/tests/__init__.py
+-rw-r--r--   0 sahadeva (21993) hentze     (453)     6984 2021-07-12 08:23:09.000000 htseq-clip-2.9.0b0/tests/bamCLIP_test.py
+-rw-r--r--   0 sahadeva (21993) hentze     (453)     2525 2020-01-24 09:01:03.000000 htseq-clip-2.9.0b0/tests/countCLIP_test.py
+-rw-r--r--   0 sahadeva (21993) hentze     (453)     1092 2020-01-24 09:01:03.000000 htseq-clip-2.9.0b0/tests/createMatrix_test.py
+-rw-r--r--   0 sahadeva (21993) hentze     (453)     4354 2020-01-24 09:01:03.000000 htseq-clip-2.9.0b0/tests/gffCLIP_test.py
```

### Comparing `htseq-clip-2.8.0b0/PKG-INFO` & `htseq-clip-2.9.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htseq-clip
-Version: 2.8.0b0
+Version: 2.9.0b0
 Summary: htseq-clip: a toolset for the analysis of eCLIP/iCLIP datasets
 Home-page: https://github.com/EMBL-Hentze-group/htseq-clip
 Author: Thomas Schwarzl, Sudeep Sahadevan, Marko Fritz, Nadia Ashraf
 Author-email: schwarzl@embl.de, sudeep.sahadevan@embl.de
 License: MIT
 Description: [![Build Status](https://travis-ci.org/EMBL-Hentze-group/htseq-clip.svg?branch=master)](https://travis-ci.org/EMBL-Hentze-group/htseq-clip)    
         ![GitHub](https://img.shields.io/github/license/EMBL-Hentze-group/htseq-clip)
```

### Comparing `htseq-clip-2.8.0b0/README.md` & `htseq-clip-2.9.0b0/README.md`

 * *Files identical despite different names*

### Comparing `htseq-clip-2.8.0b0/clip/GTxFeature.py` & `htseq-clip-2.9.0b0/clip/GTxFeature.py`

 * *Files identical despite different names*

### Comparing `htseq-clip-2.8.0b0/clip/Gene.py` & `htseq-clip-2.9.0b0/clip/Gene.py`

 * *Files identical despite different names*

### Comparing `htseq-clip-2.8.0b0/clip/GeneLengthSummary.py` & `htseq-clip-2.9.0b0/clip/GeneLengthSummary.py`

 * *Files identical despite different names*

### Comparing `htseq-clip-2.8.0b0/clip/GeneRegion.py` & `htseq-clip-2.9.0b0/clip/GeneRegion.py`

 * *Files identical despite different names*

### Comparing `htseq-clip-2.8.0b0/clip/bamCLIP.py` & `htseq-clip-2.9.0b0/clip/bamCLIP.py`

 * *Files identical despite different names*

### Comparing `htseq-clip-2.8.0b0/clip/bedCLIP.py` & `htseq-clip-2.9.0b0/clip/bedCLIP.py`

 * *Files identical despite different names*

### Comparing `htseq-clip-2.8.0b0/clip/clip.py` & `htseq-clip-2.9.0b0/clip/clip.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 '''
 
 def _annotation(args):
     '''
     Parse annotations from given GFF file
     @TODO use logging module
     '''
-    logging.info('Paring annotations') 
+    logging.info('Parsing annotations') 
     logging.info('GFF file {}, output file {}'.format(args.gff,args.output))
     gffc = gffCLIP(args)
     try:
         gffc.process(args.unsorted)
     except FeatureOrderException as se:
         if args.unsorted:
             raise(se)
```

### Comparing `htseq-clip-2.8.0b0/clip/countCLIP.py` & `htseq-clip-2.9.0b0/clip/countCLIP.py`

 * *Files identical despite different names*

### Comparing `htseq-clip-2.8.0b0/clip/createMatrix.py` & `htseq-clip-2.9.0b0/clip/createMatrix.py`

 * *Files identical despite different names*

### Comparing `htseq-clip-2.8.0b0/clip/gffCLIP.py` & `htseq-clip-2.9.0b0/clip/gffCLIP.py`

 * *Files identical despite different names*

### Comparing `htseq-clip-2.8.0b0/clip/output.py` & `htseq-clip-2.9.0b0/clip/output.py`

 * *Files identical despite different names*

### Comparing `htseq-clip-2.8.0b0/htseq_clip.egg-info/PKG-INFO` & `htseq-clip-2.9.0b0/htseq_clip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htseq-clip
-Version: 2.8.0b0
+Version: 2.9.0b0
 Summary: htseq-clip: a toolset for the analysis of eCLIP/iCLIP datasets
 Home-page: https://github.com/EMBL-Hentze-group/htseq-clip
 Author: Thomas Schwarzl, Sudeep Sahadevan, Marko Fritz, Nadia Ashraf
 Author-email: schwarzl@embl.de, sudeep.sahadevan@embl.de
 License: MIT
 Description: [![Build Status](https://travis-ci.org/EMBL-Hentze-group/htseq-clip.svg?branch=master)](https://travis-ci.org/EMBL-Hentze-group/htseq-clip)    
         ![GitHub](https://img.shields.io/github/license/EMBL-Hentze-group/htseq-clip)
```

### Comparing `htseq-clip-2.8.0b0/htseq_clip.egg-info/SOURCES.txt` & `htseq-clip-2.9.0b0/htseq_clip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `htseq-clip-2.8.0b0/setup.py` & `htseq-clip-2.9.0b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # Get the long description from the README file
 with open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='htseq-clip',
-    version='2.8.0b0',
+    version='2.9.0b0',
     description='htseq-clip: a toolset for the analysis of eCLIP/iCLIP datasets',
 	long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/EMBL-Hentze-group/htseq-clip',
     author='Thomas Schwarzl, Sudeep Sahadevan, Marko Fritz, Nadia Ashraf',
     author_email='schwarzl@embl.de, sudeep.sahadevan@embl.de',
 	zip_safe=False,
@@ -49,14 +49,14 @@
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'License :: OSI Approved :: MIT License',
         'Environment :: Console',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
     ],
-	install_requires=['HTSeq', 'pysam'],
+	install_requires=['HTSeq==0.13.5', 'pysam'],
     packages=['clip','tests'],
     test_suite = 'tests',
 	entry_points = {
         'console_scripts': ['htseq-clip=clip.command_line:main'],
     }
 )
```

### Comparing `htseq-clip-2.8.0b0/tests/bamCLIP_test.py` & `htseq-clip-2.9.0b0/tests/bamCLIP_test.py`

 * *Files identical despite different names*

### Comparing `htseq-clip-2.8.0b0/tests/countCLIP_test.py` & `htseq-clip-2.9.0b0/tests/countCLIP_test.py`

 * *Files identical despite different names*

### Comparing `htseq-clip-2.8.0b0/tests/createMatrix_test.py` & `htseq-clip-2.9.0b0/tests/createMatrix_test.py`

 * *Files identical despite different names*

### Comparing `htseq-clip-2.8.0b0/tests/gffCLIP_test.py` & `htseq-clip-2.9.0b0/tests/gffCLIP_test.py`

 * *Files identical despite different names*

