# Comparing `tmp/pyham-1.1.8.tar.gz` & `tmp/pyham-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyham-1.1.8.tar", last modified: Tue Jun 16 11:22:48 2020, max compression
+gzip compressed data, was "dist/pyham-1.1.9.tar", last modified: Thu Apr 22 05:51:41 2021, max compression
```

## Comparing `pyham-1.1.8.tar` & `pyham-1.1.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2020-06-16 11:22:48.000000 pyham-1.1.8/
--rw-r--r--   0 admin      (501) staff       (20)     6174 2020-06-16 11:22:48.000000 pyham-1.1.8/PKG-INFO
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2020-06-16 11:22:48.000000 pyham-1.1.8/tests/
--rw-r--r--   0 admin      (501) staff       (20)      139 2020-06-16 09:10:06.000000 pyham-1.1.8/tests/test_utils.py
--rw-r--r--   0 admin      (501) staff       (20)     1335 2020-06-16 09:10:06.000000 pyham-1.1.8/tests/test_conflict.py
--rw-r--r--   0 admin      (501) staff       (20)     7478 2020-06-16 11:13:39.000000 pyham-1.1.8/tests/test_abstractgene.pyc
--rw-r--r--   0 admin      (501) staff       (20)      653 2020-06-16 09:10:06.000000 pyham-1.1.8/tests/test_iham.py
--rw-r--r--   0 admin      (501) staff       (20)     5257 2020-06-16 11:20:03.000000 pyham-1.1.8/tests/test_treeprofile.py
--rw-r--r--   0 admin      (501) staff       (20)     7689 2020-06-16 09:10:06.000000 pyham-1.1.8/tests/functional_test.py
--rw-r--r--   0 admin      (501) staff       (20)    21900 2020-06-16 09:10:06.000000 pyham-1.1.8/tests/test_ham.py
--rw-r--r--   0 admin      (501) staff       (20)     2361 2020-06-16 11:13:38.000000 pyham-1.1.8/tests/test_conflict.pyc
--rw-r--r--   0 admin      (501) staff       (20)     1836 2020-06-16 09:10:06.000000 pyham-1.1.8/tests/test_genome.py
--rw-r--r--   0 admin      (501) staff       (20)    23223 2020-06-16 09:10:06.000000 pyham-1.1.8/tests/test_orthoxmlparser.py
--rw-r--r--   0 admin      (501) staff       (20)      775 2020-06-16 11:13:38.000000 pyham-1.1.8/tests/test_utils.pyc
--rw-r--r--   0 admin      (501) staff       (20)     7734 2020-06-16 11:13:39.000000 pyham-1.1.8/tests/test_taxonomy.pyc
--rw-r--r--   0 admin      (501) staff       (20)     5776 2020-06-16 11:13:39.000000 pyham-1.1.8/tests/test_treeprofile.pyc
--rw-r--r--   0 admin      (501) staff       (20)     5994 2020-06-16 09:10:06.000000 pyham-1.1.8/tests/test_abstractgene.py
--rw-r--r--   0 admin      (501) staff       (20)    22169 2020-06-16 11:13:39.000000 pyham-1.1.8/tests/test_orthoxmlparser.pyc
--rw-r--r--   0 admin      (501) staff       (20)    14023 2020-06-16 09:10:06.000000 pyham-1.1.8/tests/test_mapper.py
--rw-r--r--   0 admin      (501) staff       (20)     6789 2020-06-16 09:10:06.000000 pyham-1.1.8/tests/test_taxonomy.py
--rw-r--r--   0 admin      (501) staff       (20)    15556 2020-06-16 11:13:39.000000 pyham-1.1.8/tests/test_mapper.pyc
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2020-06-16 11:22:48.000000 pyham-1.1.8/tests/data/
--rw-r--r--   0 admin      (501) staff       (20)     7059 2020-06-16 09:10:06.000000 pyham-1.1.8/tests/data/simpleEx_complexParalogs.orthoxml
--rw-r--r--   0 admin      (501) staff       (20)     7732 2020-06-16 09:10:06.000000 pyham-1.1.8/tests/data/SimpleEx_complexParalogGetHOGS3format.xml
--rw-r--r--   0 admin      (501) staff       (20)     2106 2020-06-16 09:10:06.000000 pyham-1.1.8/tests/data/simpleExNoCladeName.phyloxml
--rw-r--r--   0 admin      (501) staff       (20)      100 2020-06-16 09:10:06.000000 pyham-1.1.8/tests/data/simpleEx.nwk
--rw-r--r--   0 admin      (501) staff       (20)       48 2020-06-16 09:10:06.000000 pyham-1.1.8/tests/data/simpleExNoName.nwk
--rw-r--r--   0 admin      (501) staff       (20)     3235 2020-06-16 09:10:06.000000 pyham-1.1.8/tests/data/simpleEx.phyloxml
--rw-r--r--   0 admin      (501) staff       (20)     2373 2020-06-16 09:10:06.000000 pyham-1.1.8/tests/data/simpleExNoName.phyloxml
--rw-r--r--   0 admin      (501) staff       (20)     2400 2020-06-16 09:10:06.000000 pyham-1.1.8/tests/data/hogvisEx.orthoxml
--rw-r--r--   0 admin      (501) staff       (20)     4278 2020-06-16 09:10:06.000000 pyham-1.1.8/tests/data/simpleEx.orthoxml
--rw-r--r--   0 admin      (501) staff       (20)     1408 2020-06-16 11:13:39.000000 pyham-1.1.8/tests/test_iham.pyc
--rw-r--r--   0 admin      (501) staff       (20)     2307 2020-06-16 11:13:39.000000 pyham-1.1.8/tests/test_genome.pyc
--rw-r--r--   0 admin      (501) staff       (20)    18843 2020-06-16 11:13:39.000000 pyham-1.1.8/tests/test_ham.pyc
--rw-r--r--   0 admin      (501) staff       (20)      116 2020-06-16 09:10:06.000000 pyham-1.1.8/MANIFEST.in
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2020-06-16 11:22:48.000000 pyham-1.1.8/docs/
--rw-r--r--   0 admin      (501) staff       (20)     6819 2020-06-16 09:10:06.000000 pyham-1.1.8/docs/index.rst
--rw-r--r--   0 admin      (501) staff       (20)       69 2020-06-16 09:10:06.000000 pyham-1.1.8/docs/taxonomy.rst
--rw-r--r--   0 admin      (501) staff       (20)      600 2020-06-16 09:10:06.000000 pyham-1.1.8/docs/Makefile
--rw-r--r--   0 admin      (501) staff       (20)       76 2020-06-16 09:10:06.000000 pyham-1.1.8/docs/treeprofile.rst
--rw-r--r--   0 admin      (501) staff       (20)       50 2020-06-16 09:10:06.000000 pyham-1.1.8/docs/iHam.rst
--rw-r--r--   0 admin      (501) staff       (20)       71 2020-06-16 09:10:06.000000 pyham-1.1.8/docs/filter.rst
--rw-r--r--   0 admin      (501) staff       (20)      283 2020-06-16 09:10:06.000000 pyham-1.1.8/docs/gene.rst
--rw-r--r--   0 admin      (501) staff       (20)      182 2020-06-16 09:10:06.000000 pyham-1.1.8/docs/ham.rst
--rw-r--r--   0 admin      (501) staff       (20)      373 2020-06-16 09:10:06.000000 pyham-1.1.8/docs/genome.rst
--rw-r--r--   0 admin      (501) staff       (20)       63 2020-06-16 09:10:06.000000 pyham-1.1.8/docs/utils.rst
--rw-r--r--   0 admin      (501) staff       (20)      271 2020-06-16 09:10:06.000000 pyham-1.1.8/docs/mapper.rst
--rw-r--r--   0 admin      (501) staff       (20)      203 2020-06-16 09:10:06.000000 pyham-1.1.8/docs/api.rst
--rw-r--r--   0 admin      (501) staff       (20)     1890 2020-06-16 09:10:06.000000 pyham-1.1.8/setup.py
--rw-r--r--   0 admin      (501) staff       (20)       67 2020-06-16 11:22:48.000000 pyham-1.1.8/setup.cfg
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2020-06-16 11:22:48.000000 pyham-1.1.8/pyham.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     6174 2020-06-16 11:22:48.000000 pyham-1.1.8/pyham.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     1355 2020-06-16 11:22:48.000000 pyham-1.1.8/pyham.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)       96 2020-06-16 11:22:48.000000 pyham-1.1.8/pyham.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)        6 2020-06-16 11:22:48.000000 pyham-1.1.8/pyham.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2020-06-16 11:22:48.000000 pyham-1.1.8/pyham.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)     4359 2020-06-16 09:10:06.000000 pyham-1.1.8/README.rst
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2020-06-16 11:22:48.000000 pyham-1.1.8/pyham/
--rw-r--r--   0 admin      (501) staff       (20)    36048 2020-06-16 09:10:06.000000 pyham-1.1.8/pyham/ham.py
--rw-r--r--   0 admin      (501) staff       (20)    19166 2020-06-16 09:47:53.000000 pyham-1.1.8/pyham/TreeProfile.py
--rw-r--r--   0 admin      (501) staff       (20)    14459 2020-06-16 09:10:06.000000 pyham-1.1.8/pyham/mapper.py
--rw-r--r--   0 admin      (501) staff       (20)      449 2020-06-16 11:21:56.000000 pyham-1.1.8/pyham/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    18604 2020-06-16 09:10:06.000000 pyham-1.1.8/pyham/abstractgene.py
--rw-r--r--   0 admin      (501) staff       (20)    13608 2020-06-16 09:10:06.000000 pyham-1.1.8/pyham/parsers.py
--rw-r--r--   0 admin      (501) staff       (20)    12372 2020-06-16 09:10:06.000000 pyham-1.1.8/pyham/iham.py
--rw-r--r--   0 admin      (501) staff       (20)     1200 2020-06-16 09:10:06.000000 pyham-1.1.8/pyham/utils.py
--rw-r--r--   0 admin      (501) staff       (20)    11883 2020-06-16 09:10:06.000000 pyham-1.1.8/pyham/taxonomy.py
--rw-r--r--   0 admin      (501) staff       (20)     4764 2020-06-16 09:10:06.000000 pyham-1.1.8/pyham/genome.py
--rw-r--r--   0 admin      (501) staff       (20)     1105 2020-06-16 09:10:06.000000 pyham-1.1.8/LICENSE.txt
+drwxr-xr-x   0 adriaal    (501) staff       (20)        0 2021-04-22 05:51:41.972032 pyham-1.1.9/
+-rw-r--r--   0 adriaal    (501) staff       (20)     1105 2017-05-12 09:32:36.000000 pyham-1.1.9/LICENSE.txt
+-rw-r--r--   0 adriaal    (501) staff       (20)      116 2018-05-09 08:36:28.000000 pyham-1.1.9/MANIFEST.in
+-rw-r--r--   0 adriaal    (501) staff       (20)     6274 2021-04-22 05:51:41.974123 pyham-1.1.9/PKG-INFO
+-rw-r--r--   0 adriaal    (501) staff       (20)     4359 2019-06-19 15:35:54.000000 pyham-1.1.9/README.rst
+drwxr-xr-x   0 adriaal    (501) staff       (20)        0 2021-04-22 05:51:41.912690 pyham-1.1.9/docs/
+-rw-r--r--   0 adriaal    (501) staff       (20)      600 2017-05-17 09:51:19.000000 pyham-1.1.9/docs/Makefile
+-rw-r--r--   0 adriaal    (501) staff       (20)      203 2018-06-15 07:30:48.000000 pyham-1.1.9/docs/api.rst
+-rw-r--r--   0 adriaal    (501) staff       (20)       71 2017-05-17 09:51:19.000000 pyham-1.1.9/docs/filter.rst
+-rw-r--r--   0 adriaal    (501) staff       (20)      283 2017-05-17 09:51:19.000000 pyham-1.1.9/docs/gene.rst
+-rw-r--r--   0 adriaal    (501) staff       (20)      373 2017-05-17 09:51:19.000000 pyham-1.1.9/docs/genome.rst
+-rw-r--r--   0 adriaal    (501) staff       (20)      182 2017-05-17 09:51:19.000000 pyham-1.1.9/docs/ham.rst
+-rw-r--r--   0 adriaal    (501) staff       (20)       50 2018-06-15 07:30:48.000000 pyham-1.1.9/docs/iHam.rst
+-rw-r--r--   0 adriaal    (501) staff       (20)     6819 2018-09-05 12:11:55.000000 pyham-1.1.9/docs/index.rst
+-rw-r--r--   0 adriaal    (501) staff       (20)      271 2017-05-17 09:51:19.000000 pyham-1.1.9/docs/mapper.rst
+-rw-r--r--   0 adriaal    (501) staff       (20)       69 2017-05-17 09:51:19.000000 pyham-1.1.9/docs/taxonomy.rst
+-rw-r--r--   0 adriaal    (501) staff       (20)       76 2017-05-17 09:51:19.000000 pyham-1.1.9/docs/treeprofile.rst
+-rw-r--r--   0 adriaal    (501) staff       (20)       63 2017-05-17 09:51:19.000000 pyham-1.1.9/docs/utils.rst
+drwxr-xr-x   0 adriaal    (501) staff       (20)        0 2021-04-22 05:51:41.932953 pyham-1.1.9/pyham/
+-rw-r--r--   0 adriaal    (501) staff       (20)    19103 2020-08-14 15:07:17.000000 pyham-1.1.9/pyham/TreeProfile.py
+-rw-r--r--   0 adriaal    (501) staff       (20)      449 2021-04-22 05:49:11.000000 pyham-1.1.9/pyham/__init__.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    18787 2021-04-22 05:48:00.000000 pyham-1.1.9/pyham/abstractgene.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     4764 2018-08-16 09:24:46.000000 pyham-1.1.9/pyham/genome.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    36453 2021-04-21 21:34:27.000000 pyham-1.1.9/pyham/ham.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    12372 2018-11-16 14:15:05.000000 pyham-1.1.9/pyham/iham.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    14459 2018-09-05 12:11:55.000000 pyham-1.1.9/pyham/mapper.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    14786 2021-04-21 21:04:54.000000 pyham-1.1.9/pyham/parsers.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    11931 2020-08-14 16:21:54.000000 pyham-1.1.9/pyham/taxonomy.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     1200 2018-09-05 12:11:55.000000 pyham-1.1.9/pyham/utils.py
+drwxr-xr-x   0 adriaal    (501) staff       (20)        0 2021-04-22 05:51:41.936859 pyham-1.1.9/pyham.egg-info/
+-rw-r--r--   0 adriaal    (501) staff       (20)     6274 2021-04-22 05:51:41.000000 pyham-1.1.9/pyham.egg-info/PKG-INFO
+-rw-r--r--   0 adriaal    (501) staff       (20)     1355 2021-04-22 05:51:41.000000 pyham-1.1.9/pyham.egg-info/SOURCES.txt
+-rw-r--r--   0 adriaal    (501) staff       (20)        1 2021-04-22 05:51:41.000000 pyham-1.1.9/pyham.egg-info/dependency_links.txt
+-rw-r--r--   0 adriaal    (501) staff       (20)       91 2021-04-22 05:51:41.000000 pyham-1.1.9/pyham.egg-info/requires.txt
+-rw-r--r--   0 adriaal    (501) staff       (20)        6 2021-04-22 05:51:41.000000 pyham-1.1.9/pyham.egg-info/top_level.txt
+-rw-r--r--   0 adriaal    (501) staff       (20)       67 2021-04-22 05:51:41.977668 pyham-1.1.9/setup.cfg
+-rw-r--r--   0 adriaal    (501) staff       (20)     1985 2021-04-21 21:40:19.000000 pyham-1.1.9/setup.py
+drwxr-xr-x   0 adriaal    (501) staff       (20)        0 2021-04-22 05:51:41.963107 pyham-1.1.9/tests/
+drwxr-xr-x   0 adriaal    (501) staff       (20)        0 2021-04-22 05:51:41.971271 pyham-1.1.9/tests/data/
+-rw-r--r--   0 adriaal    (501) staff       (20)     7732 2018-06-15 07:30:48.000000 pyham-1.1.9/tests/data/SimpleEx_complexParalogGetHOGS3format.xml
+-rw-r--r--   0 adriaal    (501) staff       (20)     2400 2017-04-19 07:03:46.000000 pyham-1.1.9/tests/data/hogvisEx.orthoxml
+-rw-r--r--   0 adriaal    (501) staff       (20)      100 2017-04-19 07:03:46.000000 pyham-1.1.9/tests/data/simpleEx.nwk
+-rw-r--r--   0 adriaal    (501) staff       (20)     4278 2017-04-19 07:03:46.000000 pyham-1.1.9/tests/data/simpleEx.orthoxml
+-rw-r--r--   0 adriaal    (501) staff       (20)     3235 2018-09-05 12:11:55.000000 pyham-1.1.9/tests/data/simpleEx.phyloxml
+-rw-r--r--   0 adriaal    (501) staff       (20)     2106 2018-09-05 12:11:55.000000 pyham-1.1.9/tests/data/simpleExNoCladeName.phyloxml
+-rw-r--r--   0 adriaal    (501) staff       (20)       48 2017-04-19 07:03:46.000000 pyham-1.1.9/tests/data/simpleExNoName.nwk
+-rw-r--r--   0 adriaal    (501) staff       (20)     2373 2018-09-05 12:11:55.000000 pyham-1.1.9/tests/data/simpleExNoName.phyloxml
+-rw-r--r--   0 adriaal    (501) staff       (20)     7059 2018-05-09 08:36:28.000000 pyham-1.1.9/tests/data/simpleEx_complexParalogs.orthoxml
+-rw-r--r--   0 adriaal    (501) staff       (20)     7401 2021-04-21 21:11:00.000000 pyham-1.1.9/tests/functional_test.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     5994 2018-05-11 08:55:07.000000 pyham-1.1.9/tests/test_abstractgene.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     7136 2018-11-09 15:44:12.000000 pyham-1.1.9/tests/test_abstractgene.pyc
+-rw-r--r--   0 adriaal    (501) staff       (20)     1335 2018-09-05 12:11:55.000000 pyham-1.1.9/tests/test_conflict.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     2247 2018-11-09 15:44:12.000000 pyham-1.1.9/tests/test_conflict.pyc
+-rw-r--r--   0 adriaal    (501) staff       (20)     1836 2018-08-16 09:24:46.000000 pyham-1.1.9/tests/test_genome.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     2212 2018-11-09 15:44:12.000000 pyham-1.1.9/tests/test_genome.pyc
+-rw-r--r--   0 adriaal    (501) staff       (20)    21751 2021-04-21 21:13:00.000000 pyham-1.1.9/tests/test_ham.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    18197 2018-11-09 15:44:12.000000 pyham-1.1.9/tests/test_ham.pyc
+-rw-r--r--   0 adriaal    (501) staff       (20)      653 2018-09-05 12:11:55.000000 pyham-1.1.9/tests/test_iham.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     1332 2018-11-09 15:44:12.000000 pyham-1.1.9/tests/test_iham.pyc
+-rw-r--r--   0 adriaal    (501) staff       (20)    13745 2021-04-21 21:17:49.000000 pyham-1.1.9/tests/test_mapper.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    14853 2018-11-09 15:44:12.000000 pyham-1.1.9/tests/test_mapper.pyc
+-rw-r--r--   0 adriaal    (501) staff       (20)    23223 2018-11-16 14:15:05.000000 pyham-1.1.9/tests/test_orthoxmlparser.py
+-rw-r--r--   0 adriaal    (501) staff       (20)    19600 2018-11-09 15:44:12.000000 pyham-1.1.9/tests/test_orthoxmlparser.pyc
+-rw-r--r--   0 adriaal    (501) staff       (20)     6789 2018-09-05 12:11:55.000000 pyham-1.1.9/tests/test_taxonomy.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     7354 2018-11-09 15:44:12.000000 pyham-1.1.9/tests/test_taxonomy.pyc
+-rw-r--r--   0 adriaal    (501) staff       (20)     5317 2020-08-14 16:03:08.000000 pyham-1.1.9/tests/test_treeprofile.py
+-rw-r--r--   0 adriaal    (501) staff       (20)     4767 2018-11-09 15:44:12.000000 pyham-1.1.9/tests/test_treeprofile.pyc
+-rw-r--r--   0 adriaal    (501) staff       (20)      139 2017-05-10 08:25:29.000000 pyham-1.1.9/tests/test_utils.py
+-rw-r--r--   0 adriaal    (501) staff       (20)      699 2018-11-09 15:44:12.000000 pyham-1.1.9/tests/test_utils.pyc
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyham-1.1.8/PKG-INFO` & `pyham-1.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyham
-Version: 1.1.8
+Version: 1.1.9
 Summary: A tool to analyse Hierarchical Orthologous Groups (HOGs)
 Home-page: http://lab.dessimoz.org/ham
 Author: Dessimoz Lab - Laboratory of Computational Evolutionary Biology and Genomics
 Author-email: adrian.altenhoff@inf.ethz.ch
 License: MIT
 Description: pyHam: A Tool to Analyze Hierarchical Orthologous Groups (HOGs)
         ===============================================================
@@ -116,12 +116,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dev
 Provides-Extra: test
```

### Comparing `pyham-1.1.8/tests/test_conflict.py` & `pyham-1.1.9/tests/test_conflict.py`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/tests/test_abstractgene.pyc` & `pyham-1.1.9/tests/test_abstractgene.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 2.7 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 03f3 0d0a 6e8c e85e 6300 0000 0000 0000  ....n..^c.......
+00000000: 03f3 0d0a 6b5a f55a 6300 0000 0000 0000  ....kZ.Zc.......
 00000010: 0003 0000 0040 0000 0073 c400 0000 6400  .....@...s....d.
 00000020: 0064 0100 6c00 005a 0000 6400 0064 0200  .d..l..Z..d..d..
 00000030: 6c01 006d 0200 5a02 006d 0300 5a03 006d  l..m..Z..m..Z..m
 00000040: 0400 5a04 006d 0500 5a05 006d 0600 5a06  ..Z..m..Z..m..Z.
 00000050: 006d 0700 5a07 006d 0800 5a08 0001 6400  .m..Z..m..Z...d.
 00000060: 0064 0300 6c09 006d 0a00 5a0b 0001 6400  .d..l..m..Z...d.
 00000070: 0064 0100 6c0c 005a 0c00 6404 0065 0000  .d..l..Z..d..e..
@@ -32,437 +32,415 @@
 000001f0: 0074 0400 8302 0001 6400 0053 2802 0000  .t......d..S(...
 00000200: 004e 7403 0000 0033 3234 2805 0000 0074  .Nt....324(....t
 00000210: 0c00 0000 6173 7365 7274 5261 6973 6573  ....assertRaises
 00000220: 7409 0000 0054 7970 6545 7272 6f72 5200  t....TypeErrorR.
 00000230: 0000 0074 1000 0000 6173 7365 7274 4973  ...t....assertIs
 00000240: 496e 7374 616e 6365 5202 0000 0028 0100  InstanceR....(..
 00000250: 0000 7404 0000 0073 656c 6628 0000 0000  ..t....self(....
-00000260: 2800 0000 0073 4d00 0000 2f55 7365 7273  (....sM.../Users
-00000270: 2f61 646d 696e 2f57 6f72 6b2f 7072 6f6a  /admin/Work/proj
-00000280: 6563 742f 4465 7373 696d 6f7a 2f70 7968  ect/Dessimoz/pyh
-00000290: 616d 2d64 6576 2f70 7968 616d 2f74 6573  am-dev/pyham/tes
-000002a0: 7473 2f74 6573 745f 6162 7374 7261 6374  ts/test_abstract
-000002b0: 6765 6e65 2e70 7974 1000 0000 7465 7374  gene.pyt....test
-000002c0: 5f69 645f 7265 7175 6972 6564 0800 0000  _id_required....
-000002d0: 7306 0000 0000 0110 010d 0163 0100 0000  s..........c....
-000002e0: 0500 0000 0800 0000 4300 0000 73c9 0000  ........C...s...
-000002f0: 0074 0000 6401 0064 0200 8300 017d 0100  .t..d..d.....}..
-00000300: 7c00 006a 0100 7402 0083 0100 8f12 0001  |..j..t.........
-00000310: 7c01 006a 0300 6403 0083 0100 0157 6400  |..j..d......Wd.
-00000320: 0051 587c 0000 6a01 0074 0200 8301 008f  .QX|..j..t......
-00000330: 1b00 0174 0400 8300 007d 0200 7c01 006a  ...t.....}..|..j
-00000340: 0300 7c02 0083 0100 0157 6400 0051 5874  ..|......Wd..QXt
-00000350: 0500 6404 0064 0500 6406 0064 0700 8300  ..d..d..d..d....
-00000360: 027d 0300 7c01 006a 0300 7c03 0083 0100  .}..|..j..|.....
-00000370: 0174 0500 6404 0064 0800 6406 0064 0900  .t..d..d..d..d..
-00000380: 8300 027d 0400 7c00 006a 0100 7406 0083  ...}..|..j..t...
-00000390: 0100 8f12 0001 7c01 006a 0300 7c04 0083  ......|..j..|...
-000003a0: 0100 0157 6400 0051 587c 0100 6a03 007c  ...Wd..QX|..j..|
-000003b0: 0300 8301 0001 6400 0053 280a 0000 004e  ......d..S(....N
-000003c0: 7402 0000 0069 6474 0300 0000 3432 3374  t....idt....423t
-000003d0: 0500 0000 7772 6f6e 6774 0400 0000 6e61  ....wrongt....na
-000003e0: 6d65 7405 0000 0048 554d 414e 7409 0000  met....HUMANt...
-000003f0: 004e 4342 4954 6178 4964 7404 0000 0039  .NCBITaxIdt....9
-00000400: 3630 3174 0500 0000 4d4f 4e44 4f74 0200  601t....MONDOt..
-00000410: 0000 3936 2807 0000 0052 0000 0000 520a  ..96(....R....R.
-00000420: 0000 0052 0b00 0000 740a 0000 0073 6574  ...R....t....set
-00000430: 5f67 656e 6f6d 6552 0300 0000 5204 0000  _genomeR....R...
-00000440: 0074 0300 0000 4543 4528 0500 0000 520d  .t....ECE(....R.
-00000450: 0000 0074 0100 0000 6774 0100 0000 6174  ...t....gt....at
-00000460: 0100 0000 6274 0100 0000 6328 0000 0000  ....bt....c(....
-00000470: 2800 0000 0073 4d00 0000 2f55 7365 7273  (....sM.../Users
-00000480: 2f61 646d 696e 2f57 6f72 6b2f 7072 6f6a  /admin/Work/proj
-00000490: 6563 742f 4465 7373 696d 6f7a 2f70 7968  ect/Dessimoz/pyh
-000004a0: 616d 2d64 6576 2f70 7968 616d 2f74 6573  am-dev/pyham/tes
-000004b0: 7473 2f74 6573 745f 6162 7374 7261 6374  ts/test_abstract
-000004c0: 6765 6e65 2e70 7974 3400 0000 7465 7374  gene.pyt4...test
-000004d0: 5f63 616e 6e6f 745f 6164 645f 6d75 6c74  _cannot_add_mult
-000004e0: 6970 6c65 5f6d 6f72 655f 7468 616e 5f6f  iple_more_than_o
-000004f0: 6e65 5f65 7874 616e 745f 6765 6e6f 6d65  ne_extant_genome
-00000500: 0d00 0000 7318 0000 0000 010f 0310 0113  ....s...........
-00000510: 0310 0109 0113 0315 010d 0315 0110 0113  ................
-00000520: 0328 0400 0000 7408 0000 005f 5f6e 616d  .(....t....__nam
-00000530: 655f 5f74 0a00 0000 5f5f 6d6f 6475 6c65  e__t....__module
-00000540: 5f5f 520e 0000 0052 1e00 0000 2800 0000  __R....R....(...
-00000550: 0028 0000 0000 2800 0000 0073 4d00 0000  .(....(....sM...
-00000560: 2f55 7365 7273 2f61 646d 696e 2f57 6f72  /Users/admin/Wor
-00000570: 6b2f 7072 6f6a 6563 742f 4465 7373 696d  k/project/Dessim
-00000580: 6f7a 2f70 7968 616d 2d64 6576 2f70 7968  oz/pyham-dev/pyh
-00000590: 616d 2f74 6573 7473 2f74 6573 745f 6162  am/tests/test_ab
-000005a0: 7374 7261 6374 6765 6e65 2e70 7952 0800  stractgene.pyR..
-000005b0: 0000 0600 0000 7304 0000 0006 0209 0574  ......s........t
-000005c0: 0700 0000 486f 6754 6573 7463 0000 0000  ....HogTestc....
-000005d0: 0000 0000 0100 0000 4200 0000 7350 0000  ........B...sP..
-000005e0: 0065 0000 5a01 0064 0000 8400 005a 0200  .e..Z..d.....Z..
-000005f0: 6401 0084 0000 5a03 0064 0200 8400 005a  d.....Z..d.....Z
-00000600: 0400 6403 0084 0000 5a05 0064 0400 8400  ..d.....Z..d....
-00000610: 005a 0600 6405 0084 0000 5a07 0064 0600  .Z..d.....Z..d..
-00000620: 8400 005a 0800 6407 0084 0000 5a09 0052  ...Z..d.....Z..R
-00000630: 5328 0800 0000 6301 0000 0003 0000 0003  S(....c.........
-00000640: 0000 0043 0000 0073 4500 0000 7400 0064  ...C...sE...t..d
-00000650: 0100 6402 0083 0001 7d01 0074 0000 6401  ..d.....}..t..d.
-00000660: 0064 0300 8300 017d 0200 7c01 006a 0100  .d.....}..|..j..
-00000670: 7c02 0083 0100 017c 0000 6a02 007c 0200  |......|..j..|..
-00000680: 7c02 006a 0300 6a04 0083 0200 0164 0000  |..j..j......d..
-00000690: 5328 0400 0000 4e52 0f00 0000 521b 0000  S(....NR....R...
-000006a0: 0052 1c00 0000 2805 0000 0052 0100 0000  .R....(....R....
-000006b0: 7409 0000 0061 6464 5f63 6869 6c64 7408  t....add_childt.
-000006c0: 0000 0061 7373 6572 7449 6e74 0600 0000  ...assertInt....
-000006d0: 7061 7265 6e74 7408 0000 0063 6869 6c64  parentt....child
-000006e0: 7265 6e28 0300 0000 520d 0000 0052 1b00  ren(....R....R..
-000006f0: 0000 521c 0000 0028 0000 0000 2800 0000  ..R....(....(...
-00000700: 0073 4d00 0000 2f55 7365 7273 2f61 646d  .sM.../Users/adm
-00000710: 696e 2f57 6f72 6b2f 7072 6f6a 6563 742f  in/Work/project/
-00000720: 4465 7373 696d 6f7a 2f70 7968 616d 2d64  Dessimoz/pyham-d
-00000730: 6576 2f70 7968 616d 2f74 6573 7473 2f74  ev/pyham/tests/t
-00000740: 6573 745f 6162 7374 7261 6374 6765 6e65  est_abstractgene
-00000750: 2e70 7974 3000 0000 7465 7374 5f68 6f67  .pyt0...test_hog
-00000760: 5f63 616e 5f62 655f 6e65 7374 6564 5f61  _can_be_nested_a
-00000770: 6e64 5f74 7261 7665 7273 6564 5f75 705f  nd_traversed_up_
-00000780: 616e 645f 646f 776e 2700 0000 7308 0000  and_down'...s...
-00000790: 0000 010f 010f 010d 0163 0100 0000 0200  .........c......
-000007a0: 0000 0600 0000 4300 0000 7330 0000 0074  ......C...s0...t
-000007b0: 0000 8300 007d 0100 7c00 006a 0100 7402  .....}..|..j..t.
-000007c0: 0083 0100 8f12 0001 7c01 006a 0300 6401  ........|..j..d.
-000007d0: 0083 0100 0157 6400 0051 5864 0000 5328  .....Wd..QXd..S(
-000007e0: 0200 0000 4e74 0400 0000 7465 7374 2804  ....Nt....test(.
-000007f0: 0000 0052 0100 0000 520a 0000 0052 0b00  ...R....R....R..
-00000800: 0000 5222 0000 0028 0200 0000 520d 0000  ..R"...(....R...
-00000810: 0052 1b00 0000 2800 0000 0028 0000 0000  .R....(....(....
-00000820: 734d 0000 002f 5573 6572 732f 6164 6d69  sM.../Users/admi
-00000830: 6e2f 576f 726b 2f70 726f 6a65 6374 2f44  n/Work/project/D
-00000840: 6573 7369 6d6f 7a2f 7079 6861 6d2d 6465  essimoz/pyham-de
-00000850: 762f 7079 6861 6d2f 7465 7374 732f 7465  v/pyham/tests/te
-00000860: 7374 5f61 6273 7472 6163 7467 656e 652e  st_abstractgene.
-00000870: 7079 7421 0000 0074 6573 745f 6361 6e6e  pyt!...test_cann
-00000880: 6f74 5f61 6464 5f61 6e79 5f74 7970 655f  ot_add_any_type_
-00000890: 6173 5f63 6869 6c64 2d00 0000 7306 0000  as_child-...s...
-000008a0: 0000 0109 0110 0163 0100 0000 0200 0000  .......c........
-000008b0: 0600 0000 4300 0000 7330 0000 0074 0000  ....C...s0...t..
-000008c0: 8300 007d 0100 7c00 006a 0100 7402 0083  ...}..|..j..t...
-000008d0: 0100 8f12 0001 7c01 006a 0300 7c01 0083  ......|..j..|...
-000008e0: 0100 0157 6400 0051 5864 0000 5328 0100  ...Wd..QXd..S(..
-000008f0: 0000 4e28 0400 0000 5201 0000 0052 0a00  ..N(....R....R..
-00000900: 0000 5219 0000 0052 2200 0000 2802 0000  ..R....R"...(...
-00000910: 0052 0d00 0000 521b 0000 0028 0000 0000  .R....R....(....
-00000920: 2800 0000 0073 4d00 0000 2f55 7365 7273  (....sM.../Users
-00000930: 2f61 646d 696e 2f57 6f72 6b2f 7072 6f6a  /admin/Work/proj
-00000940: 6563 742f 4465 7373 696d 6f7a 2f70 7968  ect/Dessimoz/pyh
-00000950: 616d 2d64 6576 2f70 7968 616d 2f74 6573  am-dev/pyham/tes
-00000960: 7473 2f74 6573 745f 6162 7374 7261 6374  ts/test_abstract
-00000970: 6765 6e65 2e70 7974 1c00 0000 7465 7374  gene.pyt....test
-00000980: 5f63 616e 6e6f 745f 6265 5f63 6869 6c64  _cannot_be_child
-00000990: 5f6f 665f 7365 6c66 3200 0000 7306 0000  _of_self2...s...
-000009a0: 0000 0109 0110 0163 0100 0000 0400 0000  .......c........
-000009b0: 0400 0000 4300 0000 739a 0000 0074 0000  ....C...s....t..
-000009c0: 6401 0064 0200 8300 017d 0100 7400 0064  d..d.....}..t..d
-000009d0: 0100 6403 0083 0001 7d02 0074 0000 6401  ..d.....}..t..d.
-000009e0: 0064 0300 8300 017d 0300 7c00 006a 0100  .d.....}..|..j..
-000009f0: 7c01 006a 0200 6700 0083 0200 017c 0100  |..j..g......|..
-00000a00: 6a03 007c 0200 8301 0001 7c01 006a 0300  j..|......|..j..
-00000a10: 7c03 0083 0100 017c 0000 6a01 007c 0100  |......|..j..|..
-00000a20: 6a02 007c 0200 7c03 0067 0200 8302 0001  j..|..|..g......
-00000a30: 7c01 006a 0400 7c02 0083 0100 017c 0000  |..j..|......|..
-00000a40: 6a01 007c 0100 6a02 007c 0300 6701 0083  j..|..j..|..g...
-00000a50: 0200 0164 0000 5328 0400 0000 4e52 0f00  ...d..S(....NR..
-00000a60: 0000 521b 0000 0052 1c00 0000 2805 0000  ..R....R....(...
-00000a70: 0052 0100 0000 740f 0000 0061 7373 6572  .R....t....asser
-00000a80: 744c 6973 7445 7175 616c 5225 0000 0052  tListEqualR%...R
-00000a90: 2200 0000 740c 0000 0072 656d 6f76 655f  "...t....remove_
-00000aa0: 6368 696c 6428 0400 0000 520d 0000 0052  child(....R....R
-00000ab0: 1b00 0000 521c 0000 0052 1d00 0000 2800  ....R....R....(.
-00000ac0: 0000 0028 0000 0000 734d 0000 002f 5573  ...(....sM.../Us
-00000ad0: 6572 732f 6164 6d69 6e2f 576f 726b 2f70  ers/admin/Work/p
-00000ae0: 726f 6a65 6374 2f44 6573 7369 6d6f 7a2f  roject/Dessimoz/
-00000af0: 7079 6861 6d2d 6465 762f 7079 6861 6d2f  pyham-dev/pyham/
-00000b00: 7465 7374 732f 7465 7374 5f61 6273 7472  tests/test_abstr
-00000b10: 6163 7467 656e 652e 7079 7411 0000 0074  actgene.pyt....t
-00000b20: 6573 745f 7265 6d6f 7665 5f63 6869 6c64  est_remove_child
-00000b30: 3700 0000 7312 0000 0000 010f 010f 010f  7...s...........
-00000b40: 0213 020d 010d 0119 020d 0163 0100 0000  ...........c....
-00000b50: 0500 0000 0800 0000 4300 0000 73b1 0000  ........C...s...
-00000b60: 0074 0000 8300 007d 0100 7c00 006a 0100  .t.....}..|..j..
-00000b70: 7402 0083 0100 8f12 0001 7c01 006a 0300  t.........|..j..
-00000b80: 6401 0083 0100 0157 6400 0051 5874 0400  d......Wd..QXt..
-00000b90: 8300 007d 0200 7c01 006a 0300 7c02 0083  ...}..|..j..|...
-00000ba0: 0100 0174 0500 6402 0064 0300 8302 007d  ...t..d..d.....}
-00000bb0: 0300 7c00 006a 0100 7402 0083 0100 8f12  ..|..j..t.......
-00000bc0: 0001 7c01 006a 0300 7c03 0083 0100 0157  ..|..j..|......W
-00000bd0: 6400 0051 5874 0400 8300 007d 0400 7c00  d..QXt.....}..|.
-00000be0: 006a 0100 7406 0083 0100 8f12 0001 7c01  .j..t.........|.
-00000bf0: 006a 0300 7c04 0083 0100 0157 6400 0051  .j..|......Wd..Q
-00000c00: 587c 0100 6a03 007c 0200 8301 0001 6400  X|..j..|......d.
-00000c10: 0053 2804 0000 004e 5211 0000 0052 1300  .S(....NR....R..
-00000c20: 0000 7401 0000 0031 2807 0000 0052 0100  ..t....1(....R..
-00000c30: 0000 520a 0000 0052 0b00 0000 5218 0000  ..R....R....R...
-00000c40: 0052 0300 0000 5204 0000 0052 1900 0000  .R....R....R....
-00000c50: 2805 0000 0052 0d00 0000 7401 0000 0068  (....R....t....h
-00000c60: 521b 0000 0074 0300 0000 6875 6d52 1c00  R....t....humR..
-00000c70: 0000 2800 0000 0028 0000 0000 734d 0000  ..(....(....sM..
-00000c80: 002f 5573 6572 732f 6164 6d69 6e2f 576f  ./Users/admin/Wo
-00000c90: 726b 2f70 726f 6a65 6374 2f44 6573 7369  rk/project/Dessi
-00000ca0: 6d6f 7a2f 7079 6861 6d2d 6465 762f 7079  moz/pyham-dev/py
-00000cb0: 6861 6d2f 7465 7374 732f 7465 7374 5f61  ham/tests/test_a
-00000cc0: 6273 7472 6163 7467 656e 652e 7079 741d  bstractgene.pyt.
-00000cd0: 0000 0074 6573 745f 6f6e 6c79 5f6f 6e65  ...test_only_one
-00000ce0: 5f67 656e 6f6d 655f 706f 7373 6962 6c65  _genome_possible
-00000cf0: 4500 0000 7318 0000 0000 0109 0310 0113  E...s...........
-00000d00: 0309 010d 030f 0110 0113 0309 0110 0113  ................
-00000d10: 0363 0100 0000 0200 0000 0500 0000 4300  .c............C.
-00000d20: 0000 7332 0000 0074 0000 6401 0064 0200  ..s2...t..d..d..
-00000d30: 6403 0064 0400 8300 027d 0100 7c00 006a  d..d.....}..|..j
-00000d40: 0100 6405 006a 0200 7c01 0083 0100 6406  ..d..j..|.....d.
-00000d50: 0083 0200 0164 0000 5328 0700 0000 4e52  .....d..S(....NR
-00000d60: 0f00 0000 7306 0000 0034 3431 2e32 6174  ....s....441.2at
-00000d70: 0300 0000 626c 6173 0a00 0000 646f 6e27  ....blas....don'
-00000d80: 7420 6b6e 6f77 7304 0000 007b 2172 7d73  t knows....{!r}s
-00000d90: 0d00 0000 3c48 4f47 2834 3431 2e32 6129  ....<HOG(441.2a)
-00000da0: 3e28 0300 0000 5201 0000 0074 0b00 0000  >(....R....t....
-00000db0: 6173 7365 7274 4571 7561 6c74 0600 0000  assertEqualt....
-00000dc0: 666f 726d 6174 2802 0000 0052 0d00 0000  format(....R....
-00000dd0: 521b 0000 0028 0000 0000 2800 0000 0073  R....(....(....s
-00000de0: 4d00 0000 2f55 7365 7273 2f61 646d 696e  M.../Users/admin
-00000df0: 2f57 6f72 6b2f 7072 6f6a 6563 742f 4465  /Work/project/De
-00000e00: 7373 696d 6f7a 2f70 7968 616d 2d64 6576  ssimoz/pyham-dev
-00000e10: 2f70 7968 616d 2f74 6573 7473 2f74 6573  /pyham/tests/tes
-00000e20: 745f 6162 7374 7261 6374 6765 6e65 2e70  t_abstractgene.p
-00000e30: 7974 1a00 0000 7465 7374 5f72 6570 7265  yt....test_repre
-00000e40: 7365 6e74 6174 696f 6e5f 6f66 5f48 6f67  sentation_of_Hog
-00000e50: 5d00 0000 7304 0000 0000 0115 0163 0100  ]...s........c..
-00000e60: 0000 0200 0000 0300 0000 4300 0000 7336  ..........C...s6
-00000e70: 0000 0074 0000 8300 007d 0100 7c01 006a  ...t.....}..|..j
-00000e80: 0100 6401 0064 0200 8302 0001 7c00 006a  ..d..d......|..j
-00000e90: 0200 7c01 006a 0100 6401 0083 0100 6402  ..|..j..d.....d.
-00000ea0: 0083 0200 0164 0000 5328 0300 0000 4e74  .....d..S(....Nt
-00000eb0: 0900 0000 7465 7374 7363 6f72 6567 6de7  ....testscoregm.
-00000ec0: fba9 f1d2 ed3f 2803 0000 0052 0100 0000  .....?(....R....
-00000ed0: 7405 0000 0073 636f 7265 7411 0000 0061  t....scoret....a
-00000ee0: 7373 6572 7441 6c6d 6f73 7445 7175 616c  ssertAlmostEqual
-00000ef0: 2802 0000 0052 0d00 0000 521b 0000 0028  (....R....R....(
-00000f00: 0000 0000 2800 0000 0073 4d00 0000 2f55  ....(....sM.../U
-00000f10: 7365 7273 2f61 646d 696e 2f57 6f72 6b2f  sers/admin/Work/
-00000f20: 7072 6f6a 6563 742f 4465 7373 696d 6f7a  project/Dessimoz
-00000f30: 2f70 7968 616d 2d64 6576 2f70 7968 616d  /pyham-dev/pyham
-00000f40: 2f74 6573 7473 2f74 6573 745f 6162 7374  /tests/test_abst
-00000f50: 7261 6374 6765 6e65 2e70 7974 0e00 0000  ractgene.pyt....
-00000f60: 7465 7374 5f61 6464 5f73 636f 7265 6100  test_add_scorea.
-00000f70: 0000 7306 0000 0000 0109 0110 0163 0100  ..s..........c..
-00000f80: 0000 0200 0000 0600 0000 4300 0000 7330  ..........C...s0
-00000f90: 0000 0074 0000 8300 007d 0100 7c00 006a  ...t.....}..|..j
-00000fa0: 0100 7402 0083 0100 8f12 0001 7c01 006a  ..t.........|..j
-00000fb0: 0300 6401 0083 0100 0157 6400 0051 5864  ..d......Wd..QXd
-00000fc0: 0000 5328 0200 0000 4e52 3500 0000 2804  ..S(....NR5...(.
-00000fd0: 0000 0052 0100 0000 520a 0000 0074 0800  ...R....R....t..
-00000fe0: 0000 4b65 7945 7272 6f72 5236 0000 0028  ..KeyErrorR6...(
-00000ff0: 0200 0000 520d 0000 0052 1b00 0000 2800  ....R....R....(.
-00001000: 0000 0028 0000 0000 734d 0000 002f 5573  ...(....sM.../Us
-00001010: 6572 732f 6164 6d69 6e2f 576f 726b 2f70  ers/admin/Work/p
-00001020: 726f 6a65 6374 2f44 6573 7369 6d6f 7a2f  roject/Dessimoz/
-00001030: 7079 6861 6d2d 6465 762f 7079 6861 6d2f  pyham-dev/pyham/
-00001040: 7465 7374 732f 7465 7374 5f61 6273 7472  tests/test_abstr
-00001050: 6163 7467 656e 652e 7079 7422 0000 0074  actgene.pyt"...t
-00001060: 6573 745f 756e 6b6e 6f77 6e5f 7363 6f72  est_unknown_scor
-00001070: 655f 7261 6973 6573 5f6b 6579 6572 726f  e_raises_keyerro
-00001080: 7266 0000 0073 0600 0000 0001 0901 1001  rf...s..........
-00001090: 280a 0000 0052 1f00 0000 5220 0000 0052  (....R....R ...R
-000010a0: 2600 0000 5228 0000 0052 2900 0000 522c  &...R(...R)...R,
-000010b0: 0000 0052 3000 0000 5234 0000 0052 3800  ...R0...R4...R8.
-000010c0: 0000 523a 0000 0028 0000 0000 2800 0000  ..R:...(....(...
-000010d0: 0028 0000 0000 734d 0000 002f 5573 6572  .(....sM.../User
-000010e0: 732f 6164 6d69 6e2f 576f 726b 2f70 726f  s/admin/Work/pro
-000010f0: 6a65 6374 2f44 6573 7369 6d6f 7a2f 7079  ject/Dessimoz/py
-00001100: 6861 6d2d 6465 762f 7079 6861 6d2f 7465  ham-dev/pyham/te
-00001110: 7374 732f 7465 7374 5f61 6273 7472 6163  sts/test_abstrac
-00001120: 7467 656e 652e 7079 5221 0000 0026 0000  tgene.pyR!...&..
-00001130: 0073 1000 0000 0601 0906 0905 0905 090e  .s..............
-00001140: 0918 0904 0905 7410 0000 0041 6273 7472  ......t....Abstr
-00001150: 6163 7447 656e 6554 6573 7463 0000 0000  actGeneTestc....
-00001160: 0000 0000 0100 0000 4200 0000 732c 0000  ........B...s,..
-00001170: 0065 0000 5a01 0064 0000 8400 005a 0200  .e..Z..d.....Z..
-00001180: 6401 0084 0000 5a03 0064 0200 8400 005a  d.....Z..d.....Z
-00001190: 0400 6403 0084 0000 5a05 0052 5328 0400  ..d.....Z..RS(..
-000011a0: 0000 6301 0000 0004 0000 0005 0000 0043  ..c............C
-000011b0: 0000 0073 7600 0000 7400 006a 0100 6a02  ...sv...t..j..j.
-000011c0: 0074 0000 6a01 006a 0300 7404 0083 0100  .t..j..j..t.....
-000011d0: 6401 0083 0200 7d01 0074 0500 6a06 007c  d.....}..t..j..|
-000011e0: 0100 6402 0064 0300 8301 017d 0200 7400  ..d..d.....}..t.
-000011f0: 006a 0100 6a02 0074 0000 6a01 006a 0300  .j..j..t..j..j..
-00001200: 7404 0083 0100 6404 0083 0200 7d03 0074  t.....d.....}..t
-00001210: 0700 6a08 007c 0200 7c03 0064 0500 7409  ..j..|..|..d..t.
-00001220: 0083 0201 7c00 005f 0a00 6400 0053 2806  ....|.._..d..S(.
-00001230: 0000 004e 7313 0000 002e 2f64 6174 612f  ...Ns...../data/
-00001240: 7369 6d70 6c65 4578 2e6e 776b 7404 0000  simpleEx.nwkt...
-00001250: 0074 7970 6574 0300 0000 6e77 6b73 1800  .typet....nwks..
-00001260: 0000 2e2f 6461 7461 2f73 696d 706c 6545  .../data/simpleE
-00001270: 782e 6f72 7468 6f78 6d6c 7411 0000 0075  x.orthoxmlt....u
-00001280: 7365 5f69 6e74 6572 6e61 6c5f 6e61 6d65  se_internal_name
-00001290: 280b 0000 0074 0200 0000 6f73 7404 0000  (....t....ost...
-000012a0: 0070 6174 6874 0400 0000 6a6f 696e 7407  .patht....joint.
-000012b0: 0000 0064 6972 6e61 6d65 7408 0000 005f  ...dirnamet...._
-000012c0: 5f66 696c 655f 5f52 0500 0000 7411 0000  _file__R....t...
-000012d0: 0067 6574 5f6e 6577 6963 6b5f 7374 7269  .get_newick_stri
-000012e0: 6e67 5206 0000 0074 0300 0000 4861 6d74  ngR....t....Hamt
-000012f0: 0400 0000 5472 7565 522e 0000 0028 0400  ....TrueR....(..
-00001300: 0000 520d 0000 0074 0800 0000 6e77 6b5f  ..R....t....nwk_
-00001310: 7061 7468 7407 0000 006e 776b 5f73 7472  patht....nwk_str
-00001320: 740d 0000 006f 7274 686f 786d 6c5f 7061  t....orthoxml_pa
-00001330: 7468 2800 0000 0028 0000 0000 734d 0000  th(....(....sM..
-00001340: 002f 5573 6572 732f 6164 6d69 6e2f 576f  ./Users/admin/Wo
-00001350: 726b 2f70 726f 6a65 6374 2f44 6573 7369  rk/project/Dessi
-00001360: 6d6f 7a2f 7079 6861 6d2d 6465 762f 7079  moz/pyham-dev/py
-00001370: 6861 6d2f 7465 7374 732f 7465 7374 5f61  ham/tests/test_a
-00001380: 6273 7472 6163 7467 656e 652e 7079 7405  bstractgene.pyt.
-00001390: 0000 0073 6574 5570 6e00 0000 7308 0000  ...setUpn...s...
-000013a0: 0000 0121 0115 0121 0263 0100 0000 0800  ...!...!.c......
-000013b0: 0000 0300 0000 4300 0000 7350 0100 007c  ......C...sP...|
-000013c0: 0000 6a00 006a 0100 6401 0083 0100 7d01  ..j..j..d.....}.
-000013d0: 007c 0000 6a00 006a 0200 6401 0083 0100  .|..j..j..d.....
-000013e0: 7d02 007c 0100 6a03 007c 0200 6a04 0083  }..|..j..|..j...
-000013f0: 0100 5c02 007d 0300 7d04 007c 0000 6a05  ..\..}..}..|..j.
-00001400: 007c 0300 7c02 0083 0200 017c 0000 6a05  .|..|......|..j.
-00001410: 007c 0400 7406 0083 0200 017c 0000 6a00  .|..t......|..j.
-00001420: 006a 0200 6402 0083 0100 7d05 007c 0100  .j..d.....}..|..
-00001430: 6a03 007c 0500 6a04 0083 0100 5c02 007d  j..|..j.....\..}
-00001440: 0300 7d04 007c 0000 6a05 007c 0300 6400  ..}..|..j..|..d.
-00001450: 0083 0200 017c 0000 6a05 007c 0400 7406  .....|..j..|..t.
-00001460: 0083 0200 017c 0000 6a00 006a 0100 6403  .....|..j..j..d.
-00001470: 0083 0100 7d06 007c 0000 6a00 006a 0200  ....}..|..j..j..
-00001480: 6404 0083 0100 7d07 007c 0600 6a03 007c  d.....}..|..j..|
-00001490: 0700 6a04 0083 0100 5c02 007d 0300 7d04  ..j.....\..}..}.
-000014a0: 007c 0000 6a05 007c 0300 7c07 0083 0200  .|..j..|..|.....
-000014b0: 017c 0000 6a05 007c 0400 7408 0083 0200  .|..j..|..t.....
-000014c0: 017c 0000 6a00 006a 0200 6404 0083 0100  .|..j..j..d.....
-000014d0: 7d07 007c 0700 6a03 007c 0700 6a04 0083  }..|..j..|..j...
-000014e0: 0100 5c02 007d 0300 7d04 007c 0000 6a05  ..\..}..}..|..j.
-000014f0: 007c 0300 6400 0083 0200 017c 0000 6a05  .|..d......|..j.
-00001500: 007c 0400 7406 0083 0200 0164 0000 5328  .|..t......d..S(
-00001510: 0500 0000 4e74 0100 0000 3269 0100 0000  ....Nt....2i....
-00001520: 7401 0000 0033 6903 0000 0028 0900 0000  t....3i....(....
-00001530: 522e 0000 0074 0e00 0000 6765 745f 6765  R....t....get_ge
-00001540: 6e65 5f62 795f 6964 740d 0000 0067 6574  ne_by_idt....get
-00001550: 5f68 6f67 5f62 795f 6964 7427 0000 0073  _hog_by_idt'...s
-00001560: 6561 7263 685f 616e 6365 7374 6f72 5f68  earch_ancestor_h
-00001570: 6f67 5f69 6e5f 616e 6365 7374 7261 6c5f  og_in_ancestral_
-00001580: 6765 6e6f 6d65 7406 0000 0067 656e 6f6d  genomet....genom
-00001590: 6552 3200 0000 7405 0000 0046 616c 7365  eR2...t....False
-000015a0: 7404 0000 004e 6f6e 6552 4600 0000 2808  t....NoneRF...(.
-000015b0: 0000 0052 0d00 0000 7405 0000 0067 656e  ...R....t....gen
-000015c0: 6532 7404 0000 0068 6f67 3274 0800 0000  e2t....hog2t....
-000015d0: 616e 6365 7374 6f72 7406 0000 0069 735f  ancestort....is_
-000015e0: 6475 7074 0400 0000 686f 6731 7405 0000  dupt....hog1t...
-000015f0: 0067 656e 6533 7404 0000 0068 6f67 3328  .gene3t....hog3(
-00001600: 0000 0000 2800 0000 0073 4d00 0000 2f55  ....(....sM.../U
-00001610: 7365 7273 2f61 646d 696e 2f57 6f72 6b2f  sers/admin/Work/
-00001620: 7072 6f6a 6563 742f 4465 7373 696d 6f7a  project/Dessimoz
-00001630: 2f70 7968 616d 2d64 6576 2f70 7968 616d  /pyham-dev/pyham
-00001640: 2f74 6573 7473 2f74 6573 745f 6162 7374  /tests/test_abst
-00001650: 7261 6374 6765 6e65 2e70 7974 2c00 0000  ractgene.pyt,...
-00001660: 7465 7374 5f73 6561 7263 685f 616e 6365  test_search_ance
-00001670: 7374 6f72 5f68 6f67 5f69 6e5f 616e 6365  stor_hog_in_ance
-00001680: 7374 7261 6c5f 6765 6e6f 6d65 7500 0000  stral_genomeu...
-00001690: 7324 0000 0000 0312 0112 0218 0110 0110  s$..............
-000016a0: 0312 0218 0110 0110 0312 0112 0218 0110  ................
-000016b0: 0110 0312 0218 0110 0163 0100 0000 0500  .........c......
-000016c0: 0000 0300 0000 4300 0000 73a0 0000 007c  ......C...s....|
-000016d0: 0000 6a00 006a 0100 6401 0083 0100 7d01  ..j..j..d.....}.
-000016e0: 007c 0000 6a00 006a 0200 6401 0083 0100  .|..j..j..d.....
-000016f0: 7d02 007c 0100 6a03 0083 0000 7d03 007c  }..|..j.....}..|
-00001700: 0000 6a04 007c 0300 7c02 0083 0200 017c  ..j..|..|......|
-00001710: 0000 6a00 006a 0200 6401 0083 0100 7d02  ..j..j..d.....}.
-00001720: 007c 0200 6a03 0083 0000 7d03 007c 0000  .|..j.....}..|..
-00001730: 6a04 007c 0300 7c02 0083 0200 017c 0000  j..|..|......|..
-00001740: 6a00 006a 0100 6402 0083 0100 7d04 007c  j..j..d.....}..|
-00001750: 0400 6a03 0083 0000 7d03 007c 0000 6a04  ..j.....}..|..j.
-00001760: 007c 0300 7c04 0083 0200 0164 0000 5328  .|..|......d..S(
-00001770: 0300 0000 4e52 4b00 0000 7401 0000 0035  ....NRK...t....5
-00001780: 2805 0000 0052 2e00 0000 524d 0000 0052  (....R....RM...R
-00001790: 4e00 0000 7411 0000 0067 6574 5f74 6f70  N...t....get_top
-000017a0: 5f6c 6576 656c 5f68 6f67 5232 0000 0028  _level_hogR2...(
-000017b0: 0500 0000 520d 0000 0052 5300 0000 5254  ....R....RS...RT
-000017c0: 0000 0052 5500 0000 7409 0000 0073 696e  ...RU...t....sin
-000017d0: 676c 6574 6f6e 2800 0000 0028 0000 0000  gleton(....(....
-000017e0: 734d 0000 002f 5573 6572 732f 6164 6d69  sM.../Users/admi
-000017f0: 6e2f 576f 726b 2f70 726f 6a65 6374 2f44  n/Work/project/D
-00001800: 6573 7369 6d6f 7a2f 7079 6861 6d2d 6465  essimoz/pyham-de
-00001810: 762f 7079 6861 6d2f 7465 7374 732f 7465  v/pyham/tests/te
-00001820: 7374 5f61 6273 7472 6163 7467 656e 652e  st_abstractgene.
-00001830: 7079 7416 0000 0074 6573 745f 6765 745f  pyt....test_get_
-00001840: 746f 705f 6c65 7665 6c5f 686f 6795 0000  top_level_hog...
-00001850: 0073 1400 0000 0003 1201 1202 0c01 1003  .s..............
-00001860: 1202 0c01 1003 1202 0c01 6301 0000 0009  ..........c.....
-00001870: 0000 0009 0000 0043 0000 0073 4d01 0000  .......C...sM...
-00001880: 7c00 006a 0000 6a01 0064 0100 8301 007d  |..j..j..d.....}
-00001890: 0100 7c00 006a 0000 6a02 0064 0200 8301  ..|..j..j..d....
-000018a0: 007d 0200 7c00 006a 0000 6a02 0064 0300  .}..|..j..j..d..
-000018b0: 8301 007d 0300 7c00 006a 0000 6a03 0064  ...}..|..j..j..d
-000018c0: 0400 8301 007d 0400 7c00 006a 0000 6a03  .....}..|..j..j.
-000018d0: 0064 0500 8301 007d 0500 7c00 006a 0000  .d.....}..|..j..
-000018e0: 6a03 0064 0600 8301 007d 0600 7c00 006a  j..d.....}..|..j
-000018f0: 0400 7405 0083 0100 8f15 0001 7c01 006a  ..t.........|..j
-00001900: 0600 7c01 006a 0700 8301 0001 5764 0000  ..|..j......Wd..
-00001910: 5158 7c00 006a 0400 7405 0083 0100 8f15  QX|..j..t.......
-00001920: 0001 7c02 006a 0600 7c02 006a 0700 8301  ..|..j..|..j....
-00001930: 0001 5764 0000 5158 7c00 006a 0400 7408  ..Wd..QX|..j..t.
-00001940: 0083 0100 8f12 0001 7c01 006a 0600 6407  ........|..j..d.
-00001950: 0083 0100 0157 6400 0051 587c 0000 6a04  .....Wd..QX|..j.
-00001960: 0074 0500 8301 008f 1200 017c 0300 6a06  .t.........|..j.
-00001970: 007c 0400 8301 0001 5764 0000 5158 7c01  .|......Wd..QX|.
-00001980: 006a 0600 7c05 0083 0100 6408 0019 7d07  .j..|.....d...}.
-00001990: 007c 0000 6a09 007c 0700 6a07 007c 0500  .|..j..|..j..|..
-000019a0: 8302 0001 7c02 006a 0600 7c06 0083 0100  ....|..j..|.....
-000019b0: 7d08 007c 0000 6a09 0074 0a00 7c08 0083  }..|..j..t..|...
-000019c0: 0100 6409 0083 0200 0164 0000 5328 0a00  ..d......d..S(..
-000019d0: 0000 4e52 2d00 0000 524c 0000 0052 4b00  ..NR-...RL...RK.
-000019e0: 0000 740a 0000 0056 6572 7465 6272 6174  ..t....Vertebrat
-000019f0: 6174 0700 0000 526f 6465 6e74 7374 1000  at....Rodentst..
-00001a00: 0000 4575 6172 6368 6f6e 746f 676c 6972  ..Euarchontoglir
-00001a10: 6573 7400 0000 0069 0000 0000 6902 0000  est....i....i...
-00001a20: 0028 0b00 0000 522e 0000 0052 4d00 0000  .(....R....RM...
-00001a30: 524e 0000 0074 1c00 0000 6765 745f 616e  RN...t....get_an
-00001a40: 6365 7374 7261 6c5f 6765 6e6f 6d65 5f62  cestral_genome_b
-00001a50: 795f 6e61 6d65 520a 0000 0052 3900 0000  y_nameR....R9...
-00001a60: 740c 0000 0067 6574 5f61 745f 6c65 7665  t....get_at_leve
-00001a70: 6c52 5000 0000 520b 0000 0052 3200 0000  lRP...R....R2...
-00001a80: 7403 0000 006c 656e 2809 0000 0052 0d00  t....len(....R..
-00001a90: 0000 7405 0000 0067 656e 6531 5259 0000  ..t....gene1RY..
-00001aa0: 0052 5400 0000 7404 0000 0076 6572 7474  .RT...t....vertt
-00001ab0: 0700 0000 726f 6465 6e74 7374 0600 0000  ....rodentst....
-00001ac0: 6575 6172 6368 7405 0000 0067 616c 5f31  euarcht....gal_1
-00001ad0: 7405 0000 0067 616c 5f32 2800 0000 0028  t....gal_2(....(
-00001ae0: 0000 0000 734d 0000 002f 5573 6572 732f  ....sM.../Users/
-00001af0: 6164 6d69 6e2f 576f 726b 2f70 726f 6a65  admin/Work/proje
-00001b00: 6374 2f44 6573 7369 6d6f 7a2f 7079 6861  ct/Dessimoz/pyha
-00001b10: 6d2d 6465 762f 7079 6861 6d2f 7465 7374  m-dev/pyham/test
-00001b20: 732f 7465 7374 5f61 6273 7472 6163 7467  s/test_abstractg
-00001b30: 656e 652e 7079 7411 0000 0074 6573 745f  ene.pyt....test_
-00001b40: 6765 745f 6174 5f6c 6576 656c aa00 0000  get_at_level....
-00001b50: 7324 0000 0000 0112 0212 0112 0212 0112  s$..............
-00001b60: 0112 0310 0116 0110 0116 0310 0113 0110  ................
-00001b70: 0113 0213 0113 020f 0128 0600 0000 521f  .........(....R.
-00001b80: 0000 0052 2000 0000 524a 0000 0052 5a00  ...R ...RJ...RZ.
-00001b90: 0000 525e 0000 0052 6c00 0000 2800 0000  ..R^...Rl...(...
-00001ba0: 0028 0000 0000 2800 0000 0073 4d00 0000  .(....(....sM...
-00001bb0: 2f55 7365 7273 2f61 646d 696e 2f57 6f72  /Users/admin/Wor
-00001bc0: 6b2f 7072 6f6a 6563 742f 4465 7373 696d  k/project/Dessim
-00001bd0: 6f7a 2f70 7968 616d 2d64 6576 2f70 7968  oz/pyham-dev/pyh
-00001be0: 616d 2f74 6573 7473 2f74 6573 745f 6162  am/tests/test_ab
-00001bf0: 7374 7261 6374 6765 6e65 2e70 7952 3b00  stractgene.pyR;.
-00001c00: 0000 6c00 0000 7308 0000 0006 0209 0709  ..l...s.........
-00001c10: 2009 1574 0800 0000 5f5f 6d61 696e 5f5f   ..t....__main__
-00001c20: 2813 0000 0074 0800 0000 756e 6974 7465  (....t....unitte
-00001c30: 7374 7405 0000 0070 7968 616d 5200 0000  stt....pyhamR...
-00001c40: 0052 0100 0000 5202 0000 0052 0300 0000  .R....R....R....
-00001c50: 5204 0000 0052 0500 0000 5206 0000 0074  R....R....R....t
-00001c60: 1200 0000 7079 6861 6d2e 6162 7374 7261  ....pyham.abstra
-00001c70: 6374 6765 6e65 5207 0000 0052 1900 0000  ctgeneR....R....
-00001c80: 523f 0000 0074 0800 0000 5465 7374 4361  R?...t....TestCa
-00001c90: 7365 5208 0000 0052 2100 0000 523b 0000  seR....R!...R;..
-00001ca0: 0052 1f00 0000 7404 0000 006d 6169 6e28  .R....t....main(
-00001cb0: 0000 0000 2800 0000 0028 0000 0000 734d  ....(....(....sM
-00001cc0: 0000 002f 5573 6572 732f 6164 6d69 6e2f  .../Users/admin/
-00001cd0: 576f 726b 2f70 726f 6a65 6374 2f44 6573  Work/project/Des
-00001ce0: 7369 6d6f 7a2f 7079 6861 6d2d 6465 762f  simoz/pyham-dev/
-00001cf0: 7079 6861 6d2f 7465 7374 732f 7465 7374  pyham/tests/test
-00001d00: 5f61 6273 7472 6163 7467 656e 652e 7079  _abstractgene.py
-00001d10: 7408 0000 003c 6d6f 6475 6c65 3e01 0000  t....<module>...
-00001d20: 0073 1000 0000 0c01 3401 1001 0c02 1920  .s......4...... 
-00001d30: 1946 195b 0c01                           .F.[..
+00000260: 2800 0000 0073 3a00 0000 2f55 7365 7273  (....s:.../Users
+00000270: 2f61 6472 6961 616c 2f52 6570 6f73 6974  /adriaal/Reposit
+00000280: 6f72 6965 732f 4841 4d2f 7465 7374 732f  ories/HAM/tests/
+00000290: 7465 7374 5f61 6273 7472 6163 7467 656e  test_abstractgen
+000002a0: 652e 7079 7410 0000 0074 6573 745f 6964  e.pyt....test_id
+000002b0: 5f72 6571 7569 7265 6408 0000 0073 0600  _required....s..
+000002c0: 0000 0001 1001 0d01 6301 0000 0005 0000  ........c.......
+000002d0: 0008 0000 0043 0000 0073 c900 0000 7400  .....C...s....t.
+000002e0: 0064 0100 6402 0083 0001 7d01 007c 0000  .d..d.....}..|..
+000002f0: 6a01 0074 0200 8301 008f 1200 017c 0100  j..t.........|..
+00000300: 6a03 0064 0300 8301 0001 5764 0000 5158  j..d......Wd..QX
+00000310: 7c00 006a 0100 7402 0083 0100 8f1b 0001  |..j..t.........
+00000320: 7404 0083 0000 7d02 007c 0100 6a03 007c  t.....}..|..j..|
+00000330: 0200 8301 0001 5764 0000 5158 7405 0064  ......Wd..QXt..d
+00000340: 0400 6405 0064 0600 6407 0083 0002 7d03  ..d..d..d.....}.
+00000350: 007c 0100 6a03 007c 0300 8301 0001 7405  .|..j..|......t.
+00000360: 0064 0400 6408 0064 0600 6409 0083 0002  .d..d..d..d.....
+00000370: 7d04 007c 0000 6a01 0074 0600 8301 008f  }..|..j..t......
+00000380: 1200 017c 0100 6a03 007c 0400 8301 0001  ...|..j..|......
+00000390: 5764 0000 5158 7c01 006a 0300 7c03 0083  Wd..QX|..j..|...
+000003a0: 0100 0164 0000 5328 0a00 0000 4e74 0200  ...d..S(....Nt..
+000003b0: 0000 6964 7403 0000 0034 3233 7405 0000  ..idt....423t...
+000003c0: 0077 726f 6e67 7404 0000 006e 616d 6574  .wrongt....namet
+000003d0: 0500 0000 4855 4d41 4e74 0900 0000 4e43  ....HUMANt....NC
+000003e0: 4249 5461 7849 6474 0400 0000 3936 3031  BITaxIdt....9601
+000003f0: 7405 0000 004d 4f4e 444f 7402 0000 0039  t....MONDOt....9
+00000400: 3628 0700 0000 5200 0000 0052 0a00 0000  6(....R....R....
+00000410: 520b 0000 0074 0a00 0000 7365 745f 6765  R....t....set_ge
+00000420: 6e6f 6d65 5203 0000 0052 0400 0000 7403  nomeR....R....t.
+00000430: 0000 0045 4345 2805 0000 0052 0d00 0000  ...ECE(....R....
+00000440: 7401 0000 0067 7401 0000 0061 7401 0000  t....gt....at...
+00000450: 0062 7401 0000 0063 2800 0000 0028 0000  .bt....c(....(..
+00000460: 0000 733a 0000 002f 5573 6572 732f 6164  ..s:.../Users/ad
+00000470: 7269 6161 6c2f 5265 706f 7369 746f 7269  riaal/Repositori
+00000480: 6573 2f48 414d 2f74 6573 7473 2f74 6573  es/HAM/tests/tes
+00000490: 745f 6162 7374 7261 6374 6765 6e65 2e70  t_abstractgene.p
+000004a0: 7974 3400 0000 7465 7374 5f63 616e 6e6f  yt4...test_canno
+000004b0: 745f 6164 645f 6d75 6c74 6970 6c65 5f6d  t_add_multiple_m
+000004c0: 6f72 655f 7468 616e 5f6f 6e65 5f65 7874  ore_than_one_ext
+000004d0: 616e 745f 6765 6e6f 6d65 0d00 0000 7318  ant_genome....s.
+000004e0: 0000 0000 010f 0310 0113 0310 0109 0113  ................
+000004f0: 0315 010d 0315 0110 0113 0328 0400 0000  ...........(....
+00000500: 7408 0000 005f 5f6e 616d 655f 5f74 0a00  t....__name__t..
+00000510: 0000 5f5f 6d6f 6475 6c65 5f5f 520e 0000  ..__module__R...
+00000520: 0052 1e00 0000 2800 0000 0028 0000 0000  .R....(....(....
+00000530: 2800 0000 0073 3a00 0000 2f55 7365 7273  (....s:.../Users
+00000540: 2f61 6472 6961 616c 2f52 6570 6f73 6974  /adriaal/Reposit
+00000550: 6f72 6965 732f 4841 4d2f 7465 7374 732f  ories/HAM/tests/
+00000560: 7465 7374 5f61 6273 7472 6163 7467 656e  test_abstractgen
+00000570: 652e 7079 5208 0000 0006 0000 0073 0400  e.pyR........s..
+00000580: 0000 0602 0905 7407 0000 0048 6f67 5465  ......t....HogTe
+00000590: 7374 6300 0000 0000 0000 0001 0000 0042  stc............B
+000005a0: 0000 0073 5000 0000 6500 005a 0100 6400  ...sP...e..Z..d.
+000005b0: 0084 0000 5a02 0064 0100 8400 005a 0300  ....Z..d.....Z..
+000005c0: 6402 0084 0000 5a04 0064 0300 8400 005a  d.....Z..d.....Z
+000005d0: 0500 6404 0084 0000 5a06 0064 0500 8400  ..d.....Z..d....
+000005e0: 005a 0700 6406 0084 0000 5a08 0064 0700  .Z..d.....Z..d..
+000005f0: 8400 005a 0900 5253 2808 0000 0063 0100  ...Z..RS(....c..
+00000600: 0000 0300 0000 0300 0000 4300 0000 7345  ..........C...sE
+00000610: 0000 0074 0000 6401 0064 0200 8300 017d  ...t..d..d.....}
+00000620: 0100 7400 0064 0100 6403 0083 0001 7d02  ..t..d..d.....}.
+00000630: 007c 0100 6a01 007c 0200 8301 0001 7c00  .|..j..|......|.
+00000640: 006a 0200 7c02 007c 0200 6a03 006a 0400  .j..|..|..j..j..
+00000650: 8302 0001 6400 0053 2804 0000 004e 520f  ....d..S(....NR.
+00000660: 0000 0052 1b00 0000 521c 0000 0028 0500  ...R....R....(..
+00000670: 0000 5201 0000 0074 0900 0000 6164 645f  ..R....t....add_
+00000680: 6368 696c 6474 0800 0000 6173 7365 7274  childt....assert
+00000690: 496e 7406 0000 0070 6172 656e 7474 0800  Int....parentt..
+000006a0: 0000 6368 696c 6472 656e 2803 0000 0052  ..children(....R
+000006b0: 0d00 0000 521b 0000 0052 1c00 0000 2800  ....R....R....(.
+000006c0: 0000 0028 0000 0000 733a 0000 002f 5573  ...(....s:.../Us
+000006d0: 6572 732f 6164 7269 6161 6c2f 5265 706f  ers/adriaal/Repo
+000006e0: 7369 746f 7269 6573 2f48 414d 2f74 6573  sitories/HAM/tes
+000006f0: 7473 2f74 6573 745f 6162 7374 7261 6374  ts/test_abstract
+00000700: 6765 6e65 2e70 7974 3000 0000 7465 7374  gene.pyt0...test
+00000710: 5f68 6f67 5f63 616e 5f62 655f 6e65 7374  _hog_can_be_nest
+00000720: 6564 5f61 6e64 5f74 7261 7665 7273 6564  ed_and_traversed
+00000730: 5f75 705f 616e 645f 646f 776e 2700 0000  _up_and_down'...
+00000740: 7308 0000 0000 010f 010f 010d 0163 0100  s............c..
+00000750: 0000 0200 0000 0600 0000 4300 0000 7330  ..........C...s0
+00000760: 0000 0074 0000 8300 007d 0100 7c00 006a  ...t.....}..|..j
+00000770: 0100 7402 0083 0100 8f12 0001 7c01 006a  ..t.........|..j
+00000780: 0300 6401 0083 0100 0157 6400 0051 5864  ..d......Wd..QXd
+00000790: 0000 5328 0200 0000 4e74 0400 0000 7465  ..S(....Nt....te
+000007a0: 7374 2804 0000 0052 0100 0000 520a 0000  st(....R....R...
+000007b0: 0052 0b00 0000 5222 0000 0028 0200 0000  .R....R"...(....
+000007c0: 520d 0000 0052 1b00 0000 2800 0000 0028  R....R....(....(
+000007d0: 0000 0000 733a 0000 002f 5573 6572 732f  ....s:.../Users/
+000007e0: 6164 7269 6161 6c2f 5265 706f 7369 746f  adriaal/Reposito
+000007f0: 7269 6573 2f48 414d 2f74 6573 7473 2f74  ries/HAM/tests/t
+00000800: 6573 745f 6162 7374 7261 6374 6765 6e65  est_abstractgene
+00000810: 2e70 7974 2100 0000 7465 7374 5f63 616e  .pyt!...test_can
+00000820: 6e6f 745f 6164 645f 616e 795f 7479 7065  not_add_any_type
+00000830: 5f61 735f 6368 696c 642d 0000 0073 0600  _as_child-...s..
+00000840: 0000 0001 0901 1001 6301 0000 0002 0000  ........c.......
+00000850: 0006 0000 0043 0000 0073 3000 0000 7400  .....C...s0...t.
+00000860: 0083 0000 7d01 007c 0000 6a01 0074 0200  ....}..|..j..t..
+00000870: 8301 008f 1200 017c 0100 6a03 007c 0100  .......|..j..|..
+00000880: 8301 0001 5764 0000 5158 6400 0053 2801  ....Wd..QXd..S(.
+00000890: 0000 004e 2804 0000 0052 0100 0000 520a  ...N(....R....R.
+000008a0: 0000 0052 1900 0000 5222 0000 0028 0200  ...R....R"...(..
+000008b0: 0000 520d 0000 0052 1b00 0000 2800 0000  ..R....R....(...
+000008c0: 0028 0000 0000 733a 0000 002f 5573 6572  .(....s:.../User
+000008d0: 732f 6164 7269 6161 6c2f 5265 706f 7369  s/adriaal/Reposi
+000008e0: 746f 7269 6573 2f48 414d 2f74 6573 7473  tories/HAM/tests
+000008f0: 2f74 6573 745f 6162 7374 7261 6374 6765  /test_abstractge
+00000900: 6e65 2e70 7974 1c00 0000 7465 7374 5f63  ne.pyt....test_c
+00000910: 616e 6e6f 745f 6265 5f63 6869 6c64 5f6f  annot_be_child_o
+00000920: 665f 7365 6c66 3200 0000 7306 0000 0000  f_self2...s.....
+00000930: 0109 0110 0163 0100 0000 0400 0000 0400  .....c..........
+00000940: 0000 4300 0000 739a 0000 0074 0000 6401  ..C...s....t..d.
+00000950: 0064 0200 8300 017d 0100 7400 0064 0100  .d.....}..t..d..
+00000960: 6403 0083 0001 7d02 0074 0000 6401 0064  d.....}..t..d..d
+00000970: 0300 8300 017d 0300 7c00 006a 0100 7c01  .....}..|..j..|.
+00000980: 006a 0200 6700 0083 0200 017c 0100 6a03  .j..g......|..j.
+00000990: 007c 0200 8301 0001 7c01 006a 0300 7c03  .|......|..j..|.
+000009a0: 0083 0100 017c 0000 6a01 007c 0100 6a02  .....|..j..|..j.
+000009b0: 007c 0200 7c03 0067 0200 8302 0001 7c01  .|..|..g......|.
+000009c0: 006a 0400 7c02 0083 0100 017c 0000 6a01  .j..|......|..j.
+000009d0: 007c 0100 6a02 007c 0300 6701 0083 0200  .|..j..|..g.....
+000009e0: 0164 0000 5328 0400 0000 4e52 0f00 0000  .d..S(....NR....
+000009f0: 521b 0000 0052 1c00 0000 2805 0000 0052  R....R....(....R
+00000a00: 0100 0000 740f 0000 0061 7373 6572 744c  ....t....assertL
+00000a10: 6973 7445 7175 616c 5225 0000 0052 2200  istEqualR%...R".
+00000a20: 0000 740c 0000 0072 656d 6f76 655f 6368  ..t....remove_ch
+00000a30: 696c 6428 0400 0000 520d 0000 0052 1b00  ild(....R....R..
+00000a40: 0000 521c 0000 0052 1d00 0000 2800 0000  ..R....R....(...
+00000a50: 0028 0000 0000 733a 0000 002f 5573 6572  .(....s:.../User
+00000a60: 732f 6164 7269 6161 6c2f 5265 706f 7369  s/adriaal/Reposi
+00000a70: 746f 7269 6573 2f48 414d 2f74 6573 7473  tories/HAM/tests
+00000a80: 2f74 6573 745f 6162 7374 7261 6374 6765  /test_abstractge
+00000a90: 6e65 2e70 7974 1100 0000 7465 7374 5f72  ne.pyt....test_r
+00000aa0: 656d 6f76 655f 6368 696c 6437 0000 0073  emove_child7...s
+00000ab0: 1200 0000 0001 0f01 0f01 0f02 1302 0d01  ................
+00000ac0: 0d01 1902 0d01 6301 0000 0005 0000 0008  ......c.........
+00000ad0: 0000 0043 0000 0073 b100 0000 7400 0083  ...C...s....t...
+00000ae0: 0000 7d01 007c 0000 6a01 0074 0200 8301  ..}..|..j..t....
+00000af0: 008f 1200 017c 0100 6a03 0064 0100 8301  .....|..j..d....
+00000b00: 0001 5764 0000 5158 7404 0083 0000 7d02  ..Wd..QXt.....}.
+00000b10: 007c 0100 6a03 007c 0200 8301 0001 7405  .|..j..|......t.
+00000b20: 0064 0200 6403 0083 0200 7d03 007c 0000  .d..d.....}..|..
+00000b30: 6a01 0074 0200 8301 008f 1200 017c 0100  j..t.........|..
+00000b40: 6a03 007c 0300 8301 0001 5764 0000 5158  j..|......Wd..QX
+00000b50: 7404 0083 0000 7d04 007c 0000 6a01 0074  t.....}..|..j..t
+00000b60: 0600 8301 008f 1200 017c 0100 6a03 007c  .........|..j..|
+00000b70: 0400 8301 0001 5764 0000 5158 7c01 006a  ......Wd..QX|..j
+00000b80: 0300 7c02 0083 0100 0164 0000 5328 0400  ..|......d..S(..
+00000b90: 0000 4e52 1100 0000 5213 0000 0074 0100  ..NR....R....t..
+00000ba0: 0000 3128 0700 0000 5201 0000 0052 0a00  ..1(....R....R..
+00000bb0: 0000 520b 0000 0052 1800 0000 5203 0000  ..R....R....R...
+00000bc0: 0052 0400 0000 5219 0000 0028 0500 0000  .R....R....(....
+00000bd0: 520d 0000 0074 0100 0000 6852 1b00 0000  R....t....hR....
+00000be0: 7403 0000 0068 756d 521c 0000 0028 0000  t....humR....(..
+00000bf0: 0000 2800 0000 0073 3a00 0000 2f55 7365  ..(....s:.../Use
+00000c00: 7273 2f61 6472 6961 616c 2f52 6570 6f73  rs/adriaal/Repos
+00000c10: 6974 6f72 6965 732f 4841 4d2f 7465 7374  itories/HAM/test
+00000c20: 732f 7465 7374 5f61 6273 7472 6163 7467  s/test_abstractg
+00000c30: 656e 652e 7079 741d 0000 0074 6573 745f  ene.pyt....test_
+00000c40: 6f6e 6c79 5f6f 6e65 5f67 656e 6f6d 655f  only_one_genome_
+00000c50: 706f 7373 6962 6c65 4500 0000 7318 0000  possibleE...s...
+00000c60: 0000 0109 0310 0113 0309 010d 030f 0110  ................
+00000c70: 0113 0309 0110 0113 0363 0100 0000 0200  .........c......
+00000c80: 0000 0500 0000 4300 0000 7332 0000 0074  ......C...s2...t
+00000c90: 0000 6401 0064 0200 6403 0064 0400 8300  ..d..d..d..d....
+00000ca0: 027d 0100 7c00 006a 0100 6405 006a 0200  .}..|..j..d..j..
+00000cb0: 7c01 0083 0100 6406 0083 0200 0164 0000  |.....d......d..
+00000cc0: 5328 0700 0000 4e52 0f00 0000 7306 0000  S(....NR....s...
+00000cd0: 0034 3431 2e32 6174 0300 0000 626c 6173  .441.2at....blas
+00000ce0: 0a00 0000 646f 6e27 7420 6b6e 6f77 7304  ....don't knows.
+00000cf0: 0000 007b 2172 7d73 0d00 0000 3c48 4f47  ...{!r}s....<HOG
+00000d00: 2834 3431 2e32 6129 3e28 0300 0000 5201  (441.2a)>(....R.
+00000d10: 0000 0074 0b00 0000 6173 7365 7274 4571  ...t....assertEq
+00000d20: 7561 6c74 0600 0000 666f 726d 6174 2802  ualt....format(.
+00000d30: 0000 0052 0d00 0000 521b 0000 0028 0000  ...R....R....(..
+00000d40: 0000 2800 0000 0073 3a00 0000 2f55 7365  ..(....s:.../Use
+00000d50: 7273 2f61 6472 6961 616c 2f52 6570 6f73  rs/adriaal/Repos
+00000d60: 6974 6f72 6965 732f 4841 4d2f 7465 7374  itories/HAM/test
+00000d70: 732f 7465 7374 5f61 6273 7472 6163 7467  s/test_abstractg
+00000d80: 656e 652e 7079 741a 0000 0074 6573 745f  ene.pyt....test_
+00000d90: 7265 7072 6573 656e 7461 7469 6f6e 5f6f  representation_o
+00000da0: 665f 486f 675d 0000 0073 0400 0000 0001  f_Hog]...s......
+00000db0: 1501 6301 0000 0002 0000 0003 0000 0043  ..c............C
+00000dc0: 0000 0073 3600 0000 7400 0083 0000 7d01  ...s6...t.....}.
+00000dd0: 007c 0100 6a01 0064 0100 6402 0083 0200  .|..j..d..d.....
+00000de0: 017c 0000 6a02 007c 0100 6a01 0064 0100  .|..j..|..j..d..
+00000df0: 8301 0064 0200 8302 0001 6400 0053 2803  ...d......d..S(.
+00000e00: 0000 004e 7409 0000 0074 6573 7473 636f  ...Nt....testsco
+00000e10: 7265 676d e7fb a9f1 d2ed 3f28 0300 0000  regm......?(....
+00000e20: 5201 0000 0074 0500 0000 7363 6f72 6574  R....t....scoret
+00000e30: 1100 0000 6173 7365 7274 416c 6d6f 7374  ....assertAlmost
+00000e40: 4571 7561 6c28 0200 0000 520d 0000 0052  Equal(....R....R
+00000e50: 1b00 0000 2800 0000 0028 0000 0000 733a  ....(....(....s:
+00000e60: 0000 002f 5573 6572 732f 6164 7269 6161  .../Users/adriaa
+00000e70: 6c2f 5265 706f 7369 746f 7269 6573 2f48  l/Repositories/H
+00000e80: 414d 2f74 6573 7473 2f74 6573 745f 6162  AM/tests/test_ab
+00000e90: 7374 7261 6374 6765 6e65 2e70 7974 0e00  stractgene.pyt..
+00000ea0: 0000 7465 7374 5f61 6464 5f73 636f 7265  ..test_add_score
+00000eb0: 6100 0000 7306 0000 0000 0109 0110 0163  a...s..........c
+00000ec0: 0100 0000 0200 0000 0600 0000 4300 0000  ............C...
+00000ed0: 7330 0000 0074 0000 8300 007d 0100 7c00  s0...t.....}..|.
+00000ee0: 006a 0100 7402 0083 0100 8f12 0001 7c01  .j..t.........|.
+00000ef0: 006a 0300 6401 0083 0100 0157 6400 0051  .j..d......Wd..Q
+00000f00: 5864 0000 5328 0200 0000 4e52 3500 0000  Xd..S(....NR5...
+00000f10: 2804 0000 0052 0100 0000 520a 0000 0074  (....R....R....t
+00000f20: 0800 0000 4b65 7945 7272 6f72 5236 0000  ....KeyErrorR6..
+00000f30: 0028 0200 0000 520d 0000 0052 1b00 0000  .(....R....R....
+00000f40: 2800 0000 0028 0000 0000 733a 0000 002f  (....(....s:.../
+00000f50: 5573 6572 732f 6164 7269 6161 6c2f 5265  Users/adriaal/Re
+00000f60: 706f 7369 746f 7269 6573 2f48 414d 2f74  positories/HAM/t
+00000f70: 6573 7473 2f74 6573 745f 6162 7374 7261  ests/test_abstra
+00000f80: 6374 6765 6e65 2e70 7974 2200 0000 7465  ctgene.pyt"...te
+00000f90: 7374 5f75 6e6b 6e6f 776e 5f73 636f 7265  st_unknown_score
+00000fa0: 5f72 6169 7365 735f 6b65 7965 7272 6f72  _raises_keyerror
+00000fb0: 6600 0000 7306 0000 0000 0109 0110 0128  f...s..........(
+00000fc0: 0a00 0000 521f 0000 0052 2000 0000 5226  ....R....R ...R&
+00000fd0: 0000 0052 2800 0000 5229 0000 0052 2c00  ...R(...R)...R,.
+00000fe0: 0000 5230 0000 0052 3400 0000 5238 0000  ..R0...R4...R8..
+00000ff0: 0052 3a00 0000 2800 0000 0028 0000 0000  .R:...(....(....
+00001000: 2800 0000 0073 3a00 0000 2f55 7365 7273  (....s:.../Users
+00001010: 2f61 6472 6961 616c 2f52 6570 6f73 6974  /adriaal/Reposit
+00001020: 6f72 6965 732f 4841 4d2f 7465 7374 732f  ories/HAM/tests/
+00001030: 7465 7374 5f61 6273 7472 6163 7467 656e  test_abstractgen
+00001040: 652e 7079 5221 0000 0026 0000 0073 1000  e.pyR!...&...s..
+00001050: 0000 0601 0906 0905 0905 090e 0918 0904  ................
+00001060: 0905 7410 0000 0041 6273 7472 6163 7447  ..t....AbstractG
+00001070: 656e 6554 6573 7463 0000 0000 0000 0000  eneTestc........
+00001080: 0100 0000 4200 0000 732c 0000 0065 0000  ....B...s,...e..
+00001090: 5a01 0064 0000 8400 005a 0200 6401 0084  Z..d.....Z..d...
+000010a0: 0000 5a03 0064 0200 8400 005a 0400 6403  ..Z..d.....Z..d.
+000010b0: 0084 0000 5a05 0052 5328 0400 0000 6301  ....Z..RS(....c.
+000010c0: 0000 0004 0000 0005 0000 0043 0000 0073  ...........C...s
+000010d0: 7600 0000 7400 006a 0100 6a02 0074 0000  v...t..j..j..t..
+000010e0: 6a01 006a 0300 7404 0083 0100 6401 0083  j..j..t.....d...
+000010f0: 0200 7d01 0074 0500 6a06 007c 0100 6402  ..}..t..j..|..d.
+00001100: 0064 0300 8301 017d 0200 7400 006a 0100  .d.....}..t..j..
+00001110: 6a02 0074 0000 6a01 006a 0300 7404 0083  j..t..j..j..t...
+00001120: 0100 6404 0083 0200 7d03 0074 0700 6a08  ..d.....}..t..j.
+00001130: 007c 0200 7c03 0064 0500 7409 0083 0201  .|..|..d..t.....
+00001140: 7c00 005f 0a00 6400 0053 2806 0000 004e  |.._..d..S(....N
+00001150: 7313 0000 002e 2f64 6174 612f 7369 6d70  s...../data/simp
+00001160: 6c65 4578 2e6e 776b 7404 0000 0074 7970  leEx.nwkt....typ
+00001170: 6574 0300 0000 6e77 6b73 1800 0000 2e2f  et....nwks...../
+00001180: 6461 7461 2f73 696d 706c 6545 782e 6f72  data/simpleEx.or
+00001190: 7468 6f78 6d6c 7411 0000 0075 7365 5f69  thoxmlt....use_i
+000011a0: 6e74 6572 6e61 6c5f 6e61 6d65 280b 0000  nternal_name(...
+000011b0: 0074 0200 0000 6f73 7404 0000 0070 6174  .t....ost....pat
+000011c0: 6874 0400 0000 6a6f 696e 7407 0000 0064  ht....joint....d
+000011d0: 6972 6e61 6d65 7408 0000 005f 5f66 696c  irnamet....__fil
+000011e0: 655f 5f52 0500 0000 7411 0000 0067 6574  e__R....t....get
+000011f0: 5f6e 6577 6963 6b5f 7374 7269 6e67 5206  _newick_stringR.
+00001200: 0000 0074 0300 0000 4861 6d74 0400 0000  ...t....Hamt....
+00001210: 5472 7565 522e 0000 0028 0400 0000 520d  TrueR....(....R.
+00001220: 0000 0074 0800 0000 6e77 6b5f 7061 7468  ...t....nwk_path
+00001230: 7407 0000 006e 776b 5f73 7472 740d 0000  t....nwk_strt...
+00001240: 006f 7274 686f 786d 6c5f 7061 7468 2800  .orthoxml_path(.
+00001250: 0000 0028 0000 0000 733a 0000 002f 5573  ...(....s:.../Us
+00001260: 6572 732f 6164 7269 6161 6c2f 5265 706f  ers/adriaal/Repo
+00001270: 7369 746f 7269 6573 2f48 414d 2f74 6573  sitories/HAM/tes
+00001280: 7473 2f74 6573 745f 6162 7374 7261 6374  ts/test_abstract
+00001290: 6765 6e65 2e70 7974 0500 0000 7365 7455  gene.pyt....setU
+000012a0: 706e 0000 0073 0800 0000 0001 2101 1501  pn...s......!...
+000012b0: 2102 6301 0000 0008 0000 0003 0000 0043  !.c............C
+000012c0: 0000 0073 5001 0000 7c00 006a 0000 6a01  ...sP...|..j..j.
+000012d0: 0064 0100 8301 007d 0100 7c00 006a 0000  .d.....}..|..j..
+000012e0: 6a02 0064 0100 8301 007d 0200 7c01 006a  j..d.....}..|..j
+000012f0: 0300 7c02 006a 0400 8301 005c 0200 7d03  ..|..j.....\..}.
+00001300: 007d 0400 7c00 006a 0500 7c03 007c 0200  .}..|..j..|..|..
+00001310: 8302 0001 7c00 006a 0500 7c04 0074 0600  ....|..j..|..t..
+00001320: 8302 0001 7c00 006a 0000 6a02 0064 0200  ....|..j..j..d..
+00001330: 8301 007d 0500 7c01 006a 0300 7c05 006a  ...}..|..j..|..j
+00001340: 0400 8301 005c 0200 7d03 007d 0400 7c00  .....\..}..}..|.
+00001350: 006a 0500 7c03 0064 0000 8302 0001 7c00  .j..|..d......|.
+00001360: 006a 0500 7c04 0074 0600 8302 0001 7c00  .j..|..t......|.
+00001370: 006a 0000 6a01 0064 0300 8301 007d 0600  .j..j..d.....}..
+00001380: 7c00 006a 0000 6a02 0064 0400 8301 007d  |..j..j..d.....}
+00001390: 0700 7c06 006a 0300 7c07 006a 0400 8301  ..|..j..|..j....
+000013a0: 005c 0200 7d03 007d 0400 7c00 006a 0500  .\..}..}..|..j..
+000013b0: 7c03 007c 0700 8302 0001 7c00 006a 0500  |..|......|..j..
+000013c0: 7c04 0074 0800 8302 0001 7c00 006a 0000  |..t......|..j..
+000013d0: 6a02 0064 0400 8301 007d 0700 7c07 006a  j..d.....}..|..j
+000013e0: 0300 7c07 006a 0400 8301 005c 0200 7d03  ..|..j.....\..}.
+000013f0: 007d 0400 7c00 006a 0500 7c03 0064 0000  .}..|..j..|..d..
+00001400: 8302 0001 7c00 006a 0500 7c04 0074 0600  ....|..j..|..t..
+00001410: 8302 0001 6400 0053 2805 0000 004e 7401  ....d..S(....Nt.
+00001420: 0000 0032 6901 0000 0074 0100 0000 3369  ...2i....t....3i
+00001430: 0300 0000 2809 0000 0052 2e00 0000 740e  ....(....R....t.
+00001440: 0000 0067 6574 5f67 656e 655f 6279 5f69  ...get_gene_by_i
+00001450: 6474 0d00 0000 6765 745f 686f 675f 6279  dt....get_hog_by
+00001460: 5f69 6474 2700 0000 7365 6172 6368 5f61  _idt'...search_a
+00001470: 6e63 6573 746f 725f 686f 675f 696e 5f61  ncestor_hog_in_a
+00001480: 6e63 6573 7472 616c 5f67 656e 6f6d 6574  ncestral_genomet
+00001490: 0600 0000 6765 6e6f 6d65 5232 0000 0074  ....genomeR2...t
+000014a0: 0500 0000 4661 6c73 6574 0400 0000 4e6f  ....Falset....No
+000014b0: 6e65 5246 0000 0028 0800 0000 520d 0000  neRF...(....R...
+000014c0: 0074 0500 0000 6765 6e65 3274 0400 0000  .t....gene2t....
+000014d0: 686f 6732 7408 0000 0061 6e63 6573 746f  hog2t....ancesto
+000014e0: 7274 0600 0000 6973 5f64 7570 7404 0000  rt....is_dupt...
+000014f0: 0068 6f67 3174 0500 0000 6765 6e65 3374  .hog1t....gene3t
+00001500: 0400 0000 686f 6733 2800 0000 0028 0000  ....hog3(....(..
+00001510: 0000 733a 0000 002f 5573 6572 732f 6164  ..s:.../Users/ad
+00001520: 7269 6161 6c2f 5265 706f 7369 746f 7269  riaal/Repositori
+00001530: 6573 2f48 414d 2f74 6573 7473 2f74 6573  es/HAM/tests/tes
+00001540: 745f 6162 7374 7261 6374 6765 6e65 2e70  t_abstractgene.p
+00001550: 7974 2c00 0000 7465 7374 5f73 6561 7263  yt,...test_searc
+00001560: 685f 616e 6365 7374 6f72 5f68 6f67 5f69  h_ancestor_hog_i
+00001570: 6e5f 616e 6365 7374 7261 6c5f 6765 6e6f  n_ancestral_geno
+00001580: 6d65 7500 0000 7324 0000 0000 0312 0112  meu...s$........
+00001590: 0218 0110 0110 0312 0218 0110 0110 0312  ................
+000015a0: 0112 0218 0110 0110 0312 0218 0110 0163  ...............c
+000015b0: 0100 0000 0500 0000 0300 0000 4300 0000  ............C...
+000015c0: 73a0 0000 007c 0000 6a00 006a 0100 6401  s....|..j..j..d.
+000015d0: 0083 0100 7d01 007c 0000 6a00 006a 0200  ....}..|..j..j..
+000015e0: 6401 0083 0100 7d02 007c 0100 6a03 0083  d.....}..|..j...
+000015f0: 0000 7d03 007c 0000 6a04 007c 0300 7c02  ..}..|..j..|..|.
+00001600: 0083 0200 017c 0000 6a00 006a 0200 6401  .....|..j..j..d.
+00001610: 0083 0100 7d02 007c 0200 6a03 0083 0000  ....}..|..j.....
+00001620: 7d03 007c 0000 6a04 007c 0300 7c02 0083  }..|..j..|..|...
+00001630: 0200 017c 0000 6a00 006a 0100 6402 0083  ...|..j..j..d...
+00001640: 0100 7d04 007c 0400 6a03 0083 0000 7d03  ..}..|..j.....}.
+00001650: 007c 0000 6a04 007c 0300 7c04 0083 0200  .|..j..|..|.....
+00001660: 0164 0000 5328 0300 0000 4e52 4b00 0000  .d..S(....NRK...
+00001670: 7401 0000 0035 2805 0000 0052 2e00 0000  t....5(....R....
+00001680: 524d 0000 0052 4e00 0000 7411 0000 0067  RM...RN...t....g
+00001690: 6574 5f74 6f70 5f6c 6576 656c 5f68 6f67  et_top_level_hog
+000016a0: 5232 0000 0028 0500 0000 520d 0000 0052  R2...(....R....R
+000016b0: 5300 0000 5254 0000 0052 5500 0000 7409  S...RT...RU...t.
+000016c0: 0000 0073 696e 676c 6574 6f6e 2800 0000  ...singleton(...
+000016d0: 0028 0000 0000 733a 0000 002f 5573 6572  .(....s:.../User
+000016e0: 732f 6164 7269 6161 6c2f 5265 706f 7369  s/adriaal/Reposi
+000016f0: 746f 7269 6573 2f48 414d 2f74 6573 7473  tories/HAM/tests
+00001700: 2f74 6573 745f 6162 7374 7261 6374 6765  /test_abstractge
+00001710: 6e65 2e70 7974 1600 0000 7465 7374 5f67  ne.pyt....test_g
+00001720: 6574 5f74 6f70 5f6c 6576 656c 5f68 6f67  et_top_level_hog
+00001730: 9500 0000 7314 0000 0000 0312 0112 020c  ....s...........
+00001740: 0110 0312 020c 0110 0312 020c 0163 0100  .............c..
+00001750: 0000 0900 0000 0900 0000 4300 0000 734d  ..........C...sM
+00001760: 0100 007c 0000 6a00 006a 0100 6401 0083  ...|..j..j..d...
+00001770: 0100 7d01 007c 0000 6a00 006a 0200 6402  ..}..|..j..j..d.
+00001780: 0083 0100 7d02 007c 0000 6a00 006a 0200  ....}..|..j..j..
+00001790: 6403 0083 0100 7d03 007c 0000 6a00 006a  d.....}..|..j..j
+000017a0: 0300 6404 0083 0100 7d04 007c 0000 6a00  ..d.....}..|..j.
+000017b0: 006a 0300 6405 0083 0100 7d05 007c 0000  .j..d.....}..|..
+000017c0: 6a00 006a 0300 6406 0083 0100 7d06 007c  j..j..d.....}..|
+000017d0: 0000 6a04 0074 0500 8301 008f 1500 017c  ..j..t.........|
+000017e0: 0100 6a06 007c 0100 6a07 0083 0100 0157  ..j..|..j......W
+000017f0: 6400 0051 587c 0000 6a04 0074 0500 8301  d..QX|..j..t....
+00001800: 008f 1500 017c 0200 6a06 007c 0200 6a07  .....|..j..|..j.
+00001810: 0083 0100 0157 6400 0051 587c 0000 6a04  .....Wd..QX|..j.
+00001820: 0074 0800 8301 008f 1200 017c 0100 6a06  .t.........|..j.
+00001830: 0064 0700 8301 0001 5764 0000 5158 7c00  .d......Wd..QX|.
+00001840: 006a 0400 7405 0083 0100 8f12 0001 7c03  .j..t.........|.
+00001850: 006a 0600 7c04 0083 0100 0157 6400 0051  .j..|......Wd..Q
+00001860: 587c 0100 6a06 007c 0500 8301 0064 0800  X|..j..|.....d..
+00001870: 197d 0700 7c00 006a 0900 7c07 006a 0700  .}..|..j..|..j..
+00001880: 7c05 0083 0200 017c 0200 6a06 007c 0600  |......|..j..|..
+00001890: 8301 007d 0800 7c00 006a 0900 740a 007c  ...}..|..j..t..|
+000018a0: 0800 8301 0064 0900 8302 0001 6400 0053  .....d......d..S
+000018b0: 280a 0000 004e 522d 0000 0052 4c00 0000  (....NR-...RL...
+000018c0: 524b 0000 0074 0a00 0000 5665 7274 6562  RK...t....Verteb
+000018d0: 7261 7461 7407 0000 0052 6f64 656e 7473  ratat....Rodents
+000018e0: 7410 0000 0045 7561 7263 686f 6e74 6f67  t....Euarchontog
+000018f0: 6c69 7265 7374 0000 0000 6900 0000 0069  lirest....i....i
+00001900: 0200 0000 280b 0000 0052 2e00 0000 524d  ....(....R....RM
+00001910: 0000 0052 4e00 0000 741c 0000 0067 6574  ...RN...t....get
+00001920: 5f61 6e63 6573 7472 616c 5f67 656e 6f6d  _ancestral_genom
+00001930: 655f 6279 5f6e 616d 6552 0a00 0000 5239  e_by_nameR....R9
+00001940: 0000 0074 0c00 0000 6765 745f 6174 5f6c  ...t....get_at_l
+00001950: 6576 656c 5250 0000 0052 0b00 0000 5232  evelRP...R....R2
+00001960: 0000 0074 0300 0000 6c65 6e28 0900 0000  ...t....len(....
+00001970: 520d 0000 0074 0500 0000 6765 6e65 3152  R....t....gene1R
+00001980: 5900 0000 5254 0000 0074 0400 0000 7665  Y...RT...t....ve
+00001990: 7274 7407 0000 0072 6f64 656e 7473 7406  rtt....rodentst.
+000019a0: 0000 0065 7561 7263 6874 0500 0000 6761  ...euarcht....ga
+000019b0: 6c5f 3174 0500 0000 6761 6c5f 3228 0000  l_1t....gal_2(..
+000019c0: 0000 2800 0000 0073 3a00 0000 2f55 7365  ..(....s:.../Use
+000019d0: 7273 2f61 6472 6961 616c 2f52 6570 6f73  rs/adriaal/Repos
+000019e0: 6974 6f72 6965 732f 4841 4d2f 7465 7374  itories/HAM/test
+000019f0: 732f 7465 7374 5f61 6273 7472 6163 7467  s/test_abstractg
+00001a00: 656e 652e 7079 7411 0000 0074 6573 745f  ene.pyt....test_
+00001a10: 6765 745f 6174 5f6c 6576 656c aa00 0000  get_at_level....
+00001a20: 7324 0000 0000 0112 0212 0112 0212 0112  s$..............
+00001a30: 0112 0310 0116 0110 0116 0310 0113 0110  ................
+00001a40: 0113 0213 0113 020f 0128 0600 0000 521f  .........(....R.
+00001a50: 0000 0052 2000 0000 524a 0000 0052 5a00  ...R ...RJ...RZ.
+00001a60: 0000 525e 0000 0052 6c00 0000 2800 0000  ..R^...Rl...(...
+00001a70: 0028 0000 0000 2800 0000 0073 3a00 0000  .(....(....s:...
+00001a80: 2f55 7365 7273 2f61 6472 6961 616c 2f52  /Users/adriaal/R
+00001a90: 6570 6f73 6974 6f72 6965 732f 4841 4d2f  epositories/HAM/
+00001aa0: 7465 7374 732f 7465 7374 5f61 6273 7472  tests/test_abstr
+00001ab0: 6163 7467 656e 652e 7079 523b 0000 006c  actgene.pyR;...l
+00001ac0: 0000 0073 0800 0000 0602 0907 0920 0915  ...s......... ..
+00001ad0: 7408 0000 005f 5f6d 6169 6e5f 5f28 1300  t....__main__(..
+00001ae0: 0000 7408 0000 0075 6e69 7474 6573 7474  ..t....unittestt
+00001af0: 0500 0000 7079 6861 6d52 0000 0000 5201  ....pyhamR....R.
+00001b00: 0000 0052 0200 0000 5203 0000 0052 0400  ...R....R....R..
+00001b10: 0000 5205 0000 0052 0600 0000 7412 0000  ..R....R....t...
+00001b20: 0070 7968 616d 2e61 6273 7472 6163 7467  .pyham.abstractg
+00001b30: 656e 6552 0700 0000 5219 0000 0052 3f00  eneR....R....R?.
+00001b40: 0000 7408 0000 0054 6573 7443 6173 6552  ..t....TestCaseR
+00001b50: 0800 0000 5221 0000 0052 3b00 0000 521f  ....R!...R;...R.
+00001b60: 0000 0074 0400 0000 6d61 696e 2800 0000  ...t....main(...
+00001b70: 0028 0000 0000 2800 0000 0073 3a00 0000  .(....(....s:...
+00001b80: 2f55 7365 7273 2f61 6472 6961 616c 2f52  /Users/adriaal/R
+00001b90: 6570 6f73 6974 6f72 6965 732f 4841 4d2f  epositories/HAM/
+00001ba0: 7465 7374 732f 7465 7374 5f61 6273 7472  tests/test_abstr
+00001bb0: 6163 7467 656e 652e 7079 7408 0000 003c  actgene.pyt....<
+00001bc0: 6d6f 6475 6c65 3e01 0000 0073 1000 0000  module>....s....
+00001bd0: 0c01 3401 1001 0c02 1920 1946 195b 0c01  ..4...... .F.[..
```

### Comparing `pyham-1.1.8/tests/test_iham.py` & `pyham-1.1.9/tests/test_iham.py`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/tests/test_treeprofile.py` & `pyham-1.1.9/tests/test_treeprofile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import shutil
 import unittest
 from pyham import ham, utils, TreeProfile
 import tempfile
 import os
 from unittest import skip
 
 class TreeProfileTest(unittest.TestCase):
@@ -89,16 +90,21 @@
             if lvl.name in self.exp_full_nn.keys():
                 observed_level = [lvl.nbr_genes, lvl.retained, lvl.dupl, lvl.gain, lvl.lost]
                 self.assertListEqual(self.exp_full_nn[lvl.name], observed_level)
 
 
 class ServerBasedTreeProfileTest(unittest.TestCase):
 
-    @skip
+    def setUp(self):
+        self.tmpdir = tempfile.mkdtemp()
+
+    def tearDown(self):
+        shutil.rmtree(self.tmpdir)
+
     def test_non_luca_root_hog_works_from_omabrowser(self):
         analysis = ham.Ham(query_database='P53_RAT', use_data_from='oma')
-        with tempfile.TemporaryDirectory() as tmpdir:
-            fn = os.path.join(tmpdir, 'tree_profile.html')
-            analysis.create_tree_profile(outfile=fn)
-            with open(fn, 'rt') as fh:
-                html = fh.read()
-            self.assertIn('treeData', html)
+
+        fn = os.path.join(self.tmpdir, 'tree_profile.html')
+        analysis.create_tree_profile(outfile=fn)
+        with open(fn, 'rt') as fh:
+            html = fh.read()
+        self.assertIn('treeData', html)
```

### Comparing `pyham-1.1.8/tests/functional_test.py` & `pyham-1.1.9/tests/functional_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,23 @@
 import unittest
 from pyham import ham
 from pyham import utils
 import logging
 import os
 
 def _str_array(array):
-    array_converted = []
-    for e in array:
-        array_converted.append(str(e))
-    return set(array_converted)
+    return set(str(e) for e in array)
 
 
 def _str_dict_one_value(dict):
-    for kk in dict.keys():
-        dict[str(kk)] = dict.pop(kk)
-    for k, v in dict.items():
-        dict[k] = str(v)
-    return dict
+    return {str(key): str(val) for key, val in dict.items()}
 
 
 def _str_dict_array_value(dict):
-    for kk in dict.keys():
-        dict[str(kk)] = dict.pop(kk)
-    for k, vs in dict.items():
-        array = []
-        for v in vs:
-            array.append(str(v))
-        dict[k] = set(array)
-    return dict
+    return {str(key): set(str(v) for v in val) for key, val in dict.items()}
 
 
 class HamAnalysis(unittest.TestCase):
 
     def test_load_taxonomy_from_nwk_file_and_all_hogs_from_orthoxml_file_no_filter(self):
 
         # load the logger
```

### Comparing `pyham-1.1.8/tests/test_ham.py` & `pyham-1.1.9/tests/test_ham.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 import unittest
 from pyham import utils
 from pyham import ham
 import ete3
 import os
 
+
 # This helps to convert elements of list/dictionary to string in order to make easier assertEqual test.
 def _str_dict_one_value(dict):
-    for kk in dict.keys():
-        dict[str(kk)] = dict.pop(kk)
-    for k, v in dict.items():
-        dict[k] = str(v)
-    return dict
+    return {str(key): str(val) for key, val in dict.items()}
+
+
 def _str_array(array):
-    array_converted = []
-    for e in array:
-        array_converted.append(str(e))
-    return set(array_converted)
+    return set(str(e) for e in array)
 
 
 class HAMTestSetUp(unittest.TestCase):
 
     def setUp(self):
         self.nwk_str_empty = ""
         self.nwk_str_wrong = "(A,B)x0.4"
```

### Comparing `pyham-1.1.8/tests/test_genome.py` & `pyham-1.1.9/tests/test_genome.py`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/tests/test_orthoxmlparser.py` & `pyham-1.1.9/tests/test_orthoxmlparser.py`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/tests/test_taxonomy.pyc` & `pyham-1.1.9/tests/test_taxonomy.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 2.7 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 03f3 0d0a 6e8c e85e 6300 0000 0000 0000  ....n..^c.......
+00000000: 03f3 0d0a 0bc8 8f5b 6300 0000 0000 0000  .......[c.......
 00000010: 0003 0000 0040 0000 0073 4b00 0000 6400  .....@...sK...d.
 00000020: 0064 0100 6c00 005a 0000 6400 0064 0200  .d..l..Z..d..d..
 00000030: 6c01 006d 0200 5a02 006d 0300 5a03 0001  l..m..Z..m..Z...
 00000040: 6400 0064 0100 6c04 005a 0400 6403 0065  d..d..l..Z..d..e
 00000050: 0000 6a05 0066 0100 6404 0084 0000 8300  ..j..f..d.......
 00000060: 0059 5a06 0064 0100 5328 0500 0000 69ff  .YZ..d..S(....i.
 00000070: ffff ff4e 2802 0000 0074 0800 0000 7461  ...N(....t....ta
@@ -111,374 +111,350 @@
 000006e0: 5f66 696c 655f 6e6f 5f63 6c61 6465 5f6e  _file_no_clade_n
 000006f0: 616d 6574 1800 0000 6578 7065 6374 6564  amet....expected
 00000700: 5f6e 616d 655f 636f 6e63 6174 5f6e 6632  _name_concat_nf2
 00000710: 7410 0000 0073 6574 5f73 7065 6369 6573  t....set_species
 00000720: 5f6e 616d 6574 1300 0000 7365 745f 7370  _namet....set_sp
 00000730: 6563 6965 735f 7363 696e 616d 6528 0100  ecies_sciname(..
 00000740: 0000 7404 0000 0073 656c 6628 0000 0000  ..t....self(....
-00000750: 2800 0000 0073 4900 0000 2f55 7365 7273  (....sI.../Users
-00000760: 2f61 646d 696e 2f57 6f72 6b2f 7072 6f6a  /admin/Work/proj
-00000770: 6563 742f 4465 7373 696d 6f7a 2f70 7968  ect/Dessimoz/pyh
-00000780: 616d 2d64 6576 2f70 7968 616d 2f74 6573  am-dev/pyham/tes
-00000790: 7473 2f74 6573 745f 7461 786f 6e6f 6d79  ts/test_taxonomy
-000007a0: 2e70 7974 0500 0000 7365 7455 7008 0000  .pyt....setUp...
-000007b0: 0073 1e00 0000 0001 0901 0901 0901 1201  .s..............
-000007c0: 1202 2401 1801 1803 2401 2401 2401 0901  ..$.....$.$.$...
-000007d0: 0f02 1b01 6301 0000 0001 0000 0009 0000  ....c...........
-000007e0: 0043 0000 0073 5600 0000 7c00 006a 0000  .C...sV...|..j..
-000007f0: 7401 0083 0100 8f15 0001 7402 006a 0300  t.........t..j..
-00000800: 7c00 006a 0400 8301 0001 5764 0000 5158  |..j......Wd..QX
-00000810: 7c00 006a 0000 7401 0083 0100 8f1b 0001  |..j..t.........
-00000820: 7402 006a 0300 7c00 006a 0400 6401 0074  t..j..|..j..d..t
-00000830: 0500 8301 0101 5764 0000 5158 6400 0053  ......Wd..QXd..S
-00000840: 2802 0000 004e 7411 0000 0075 7365 5f69  (....Nt....use_i
-00000850: 6e74 6572 6e61 6c5f 6e61 6d65 2806 0000  nternal_name(...
-00000860: 0074 0c00 0000 6173 7365 7274 5261 6973  .t....assertRais
-00000870: 6573 7408 0000 004b 6579 4572 726f 7252  est....KeyErrorR
-00000880: 0000 0000 7408 0000 0054 6178 6f6e 6f6d  ....t....Taxonom
-00000890: 7952 1100 0000 7405 0000 0046 616c 7365  yR....t....False
-000008a0: 2801 0000 0052 2200 0000 2800 0000 0028  (....R"...(....(
-000008b0: 0000 0000 7349 0000 002f 5573 6572 732f  ....sI.../Users/
-000008c0: 6164 6d69 6e2f 576f 726b 2f70 726f 6a65  admin/Work/proje
-000008d0: 6374 2f44 6573 7369 6d6f 7a2f 7079 6861  ct/Dessimoz/pyha
-000008e0: 6d2d 6465 762f 7079 6861 6d2f 7465 7374  m-dev/pyham/test
-000008f0: 732f 7465 7374 5f74 6178 6f6e 6f6d 792e  s/test_taxonomy.
-00000900: 7079 741a 0000 0074 6573 745f 6e6f 6e5f  pyt....test_non_
-00000910: 756e 6971 7565 5f6c 6561 665f 6e61 6d65  unique_leaf_name
-00000920: 731d 0000 0073 0800 0000 0001 1001 1602  s....s..........
-00000930: 1001 6301 0000 0006 0000 000a 0000 0043  ..c............C
-00000940: 0000 0073 3e01 0000 7400 006a 0100 7c00  ...s>...t..j..|.
-00000950: 006a 0200 6401 0074 0300 8301 017d 0100  .j..d..t.....}..
-00000960: 6402 0084 0000 7c01 006a 0400 6a05 0083  d.....|..j..j...
-00000970: 0000 4483 0100 7d02 007c 0000 6a06 007c  ..D...}..|..j..|
-00000980: 0000 6a07 007c 0200 8302 0001 7400 006a  ..j..|......t..j
-00000990: 0100 7c00 006a 0800 6401 0074 0300 6403  ..|..j..d..t..d.
-000009a0: 0064 0400 8301 027d 0300 6405 0084 0000  .d.....}..d.....
-000009b0: 7c03 006a 0400 6a05 0083 0000 4483 0100  |..j..j.....D...
-000009c0: 7d02 007c 0000 6a06 007c 0000 6a09 007c  }..|..j..|..j..|
-000009d0: 0200 8302 0001 7400 006a 0100 7c00 006a  ......t..j..|..j
-000009e0: 0a00 6401 0074 0300 6403 0064 0600 6407  ..d..t..d..d..d.
-000009f0: 0064 0800 6409 0064 0800 8301 047d 0400  .d..d..d.....}..
-00000a00: 640a 0084 0000 7c04 006a 0400 6a05 0083  d.....|..j..j...
-00000a10: 0000 4483 0100 7d02 007c 0000 6a06 007c  ..D...}..|..j..|
-00000a20: 0000 6a09 007c 0200 8302 0001 7400 006a  ..j..|......t..j
-00000a30: 0100 7c00 006a 0a00 6401 0074 0300 6403  ..|..j..d..t..d.
-00000a40: 0064 0600 6407 0064 0b00 6409 0064 0800  .d..d..d..d..d..
-00000a50: 8301 047d 0500 640c 0084 0000 7c05 006a  ...}..d.....|..j
-00000a60: 0400 6a05 0083 0000 4483 0100 7d02 007c  ..j.....D...}..|
-00000a70: 0000 6a06 007c 0000 6a09 007c 0200 8302  ..j..|..j..|....
-00000a80: 0001 6400 0053 280d 0000 004e 5224 0000  ..d..S(....NR$..
-00000a90: 0063 0100 0000 0200 0000 0400 0000 5300  .c............S.
-00000aa0: 0000 732b 0000 0068 0000 7c00 005d 2100  ..s+...h..|..]!.
-00000ab0: 7d01 007c 0100 6a00 0083 0000 7401 006b  }..|..j.....t..k
-00000ac0: 0800 7206 007c 0100 6a02 0092 0200 7106  ..r..|..j.....q.
-00000ad0: 0053 2800 0000 0028 0300 0000 7407 0000  .S(....(....t...
-00000ae0: 0069 735f 6c65 6166 5228 0000 0074 0400  .is_leafR(...t..
-00000af0: 0000 6e61 6d65 2802 0000 0074 0200 0000  ..name(....t....
-00000b00: 2e30 7404 0000 006e 6f64 6528 0000 0000  .0t....node(....
-00000b10: 2800 0000 0073 4900 0000 2f55 7365 7273  (....sI.../Users
-00000b20: 2f61 646d 696e 2f57 6f72 6b2f 7072 6f6a  /admin/Work/proj
-00000b30: 6563 742f 4465 7373 696d 6f7a 2f70 7968  ect/Dessimoz/pyh
-00000b40: 616d 2d64 6576 2f70 7968 616d 2f74 6573  am-dev/pyham/tes
-00000b50: 7473 2f74 6573 745f 7461 786f 6e6f 6d79  ts/test_taxonomy
-00000b60: 2e70 7973 0900 0000 3c73 6574 636f 6d70  .pys....<setcomp
-00000b70: 3e29 0000 0073 0200 0000 0900 740b 0000  >)...s......t...
-00000b80: 0074 7265 655f 666f 726d 6174 7406 0000  .tree_formatt...
-00000b90: 006e 6577 6963 6b63 0100 0000 0200 0000  .newickc........
-00000ba0: 0400 0000 5300 0000 732b 0000 0068 0000  ....S...s+...h..
-00000bb0: 7c00 005d 2100 7d01 007c 0100 6a00 0083  |..]!.}..|..j...
-00000bc0: 0000 7401 006b 0800 7206 007c 0100 6a02  ..t..k..r..|..j.
-00000bd0: 0092 0200 7106 0053 2800 0000 0028 0300  ....q..S(....(..
-00000be0: 0000 522a 0000 0052 2800 0000 522b 0000  ..R*...R(...R+..
-00000bf0: 0028 0200 0000 522c 0000 0052 2d00 0000  .(....R,...R-...
-00000c00: 2800 0000 0028 0000 0000 7349 0000 002f  (....(....sI.../
-00000c10: 5573 6572 732f 6164 6d69 6e2f 576f 726b  Users/admin/Work
-00000c20: 2f70 726f 6a65 6374 2f44 6573 7369 6d6f  /project/Dessimo
-00000c30: 7a2f 7079 6861 6d2d 6465 762f 7079 6861  z/pyham-dev/pyha
-00000c40: 6d2f 7465 7374 732f 7465 7374 5f74 6178  m/tests/test_tax
-00000c50: 6f6e 6f6d 792e 7079 7309 0000 003c 7365  onomy.pys....<se
-00000c60: 7463 6f6d 703e 2e00 0000 7302 0000 0009  tcomp>....s.....
-00000c70: 0074 0800 0000 7068 796c 6f78 6d6c 741a  .t....phyloxmlt.
-00000c80: 0000 0070 6879 6c6f 786d 6c5f 696e 7465  ...phyloxml_inte
-00000c90: 726e 616c 5f6e 616d 655f 7461 6774 1800  rnal_name_tagt..
-00000ca0: 0000 7461 786f 6e6f 6d79 5f73 6369 656e  ..taxonomy_scien
-00000cb0: 7469 6669 635f 6e61 6d65 7416 0000 0070  tific_namet....p
-00000cc0: 6879 6c6f 786d 6c5f 6c65 6166 5f6e 616d  hyloxml_leaf_nam
-00000cd0: 655f 7461 6763 0100 0000 0200 0000 0400  e_tagc..........
-00000ce0: 0000 5300 0000 732b 0000 0068 0000 7c00  ..S...s+...h..|.
-00000cf0: 005d 2100 7d01 007c 0100 6a00 0083 0000  .]!.}..|..j.....
-00000d00: 7401 006b 0800 7206 007c 0100 6a02 0092  t..k..r..|..j...
-00000d10: 0200 7106 0053 2800 0000 0028 0300 0000  ..q..S(....(....
-00000d20: 522a 0000 0052 2800 0000 522b 0000 0028  R*...R(...R+...(
-00000d30: 0200 0000 522c 0000 0052 2d00 0000 2800  ....R,...R-...(.
-00000d40: 0000 0028 0000 0000 7349 0000 002f 5573  ...(....sI.../Us
-00000d50: 6572 732f 6164 6d69 6e2f 576f 726b 2f70  ers/admin/Work/p
-00000d60: 726f 6a65 6374 2f44 6573 7369 6d6f 7a2f  roject/Dessimoz/
-00000d70: 7079 6861 6d2d 6465 762f 7079 6861 6d2f  pyham-dev/pyham/
-00000d80: 7465 7374 732f 7465 7374 5f74 6178 6f6e  tests/test_taxon
-00000d90: 6f6d 792e 7079 7309 0000 003c 7365 7463  omy.pys....<setc
-00000da0: 6f6d 703e 3300 0000 7302 0000 0009 0074  omp>3...s......t
-00000db0: 0a00 0000 636c 6164 655f 6e61 6d65 6301  ....clade_namec.
-00000dc0: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
-00000dd0: 2b00 0000 6800 007c 0000 5d21 007d 0100  +...h..|..]!.}..
-00000de0: 7c01 006a 0000 8300 0074 0100 6b08 0072  |..j.....t..k..r
-00000df0: 0600 7c01 006a 0200 9202 0071 0600 5328  ..|..j.....q..S(
-00000e00: 0000 0000 2803 0000 0052 2a00 0000 5228  ....(....R*...R(
-00000e10: 0000 0052 2b00 0000 2802 0000 0052 2c00  ...R+...(....R,.
-00000e20: 0000 522d 0000 0028 0000 0000 2800 0000  ..R-...(....(...
-00000e30: 0073 4900 0000 2f55 7365 7273 2f61 646d  .sI.../Users/adm
-00000e40: 696e 2f57 6f72 6b2f 7072 6f6a 6563 742f  in/Work/project/
-00000e50: 4465 7373 696d 6f7a 2f70 7968 616d 2d64  Dessimoz/pyham-d
-00000e60: 6576 2f70 7968 616d 2f74 6573 7473 2f74  ev/pyham/tests/t
-00000e70: 6573 745f 7461 786f 6e6f 6d79 2e70 7973  est_taxonomy.pys
-00000e80: 0900 0000 3c73 6574 636f 6d70 3e3a 0000  ....<setcomp>:..
-00000e90: 0073 0200 0000 0900 280b 0000 0052 0000  .s......(....R..
-00000ea0: 0000 5227 0000 0052 0f00 0000 7404 0000  ..R'...R....t...
-00000eb0: 0054 7275 6574 0400 0000 7472 6565 7408  .Truet....treet.
-00000ec0: 0000 0074 7261 7665 7273 6574 0e00 0000  ...traverset....
-00000ed0: 6173 7365 7274 5365 7445 7175 616c 5212  assertSetEqualR.
-00000ee0: 0000 0052 1900 0000 521a 0000 0052 1c00  ...R....R....R..
-00000ef0: 0000 2806 0000 0052 2200 0000 7401 0000  ..(....R"...t...
-00000f00: 0074 740d 0000 006f 6273 6572 7665 645f  .tt....observed_
-00000f10: 6e61 6d65 7402 0000 0074 3274 0200 0000  namet....t2t....
-00000f20: 7433 7402 0000 0074 3428 0000 0000 2800  t3t....t4(....(.
-00000f30: 0000 0073 4900 0000 2f55 7365 7273 2f61  ...sI.../Users/a
-00000f40: 646d 696e 2f57 6f72 6b2f 7072 6f6a 6563  dmin/Work/projec
-00000f50: 742f 4465 7373 696d 6f7a 2f70 7968 616d  t/Dessimoz/pyham
-00000f60: 2d64 6576 2f70 7968 616d 2f74 6573 7473  -dev/pyham/tests
-00000f70: 2f74 6573 745f 7461 786f 6e6f 6d79 2e70  /test_taxonomy.p
-00000f80: 7974 1600 0000 7465 7374 5f75 7365 5f69  yt....test_use_i
-00000f90: 6e74 6572 6e61 6c5f 6e61 6d65 2500 0000  nternal_name%...
-00000fa0: 731c 0000 0000 0318 0119 0113 031e 0119  s...............
-00000fb0: 0113 032a 0119 0113 031b 0106 0109 0119  ...*............
-00000fc0: 0163 0100 0000 0700 0000 0800 0000 4300  .c............C.
-00000fd0: 0000 7376 0100 0074 0000 6a01 007c 0000  ..sv...t..j..|..
-00000fe0: 6a02 0064 0100 7403 0083 0101 7d01 0064  j..d..t.....}..d
-00000ff0: 0200 8400 007c 0100 6a04 006a 0500 8300  .....|..j..j....
-00001000: 0044 8301 007d 0200 7c00 006a 0600 7c00  .D...}..|..j..|.
-00001010: 006a 0700 7c02 0083 0200 0174 0000 6a01  .j..|......t..j.
-00001020: 007c 0000 6a08 0064 0100 7403 0064 0300  .|..j..d..t..d..
-00001030: 6404 0083 0102 7d03 0064 0500 8400 007c  d.....}..d.....|
-00001040: 0300 6a04 006a 0500 8300 0044 8301 007d  ..j..j.....D...}
-00001050: 0200 7c00 006a 0600 7c00 006a 0900 7c02  ..|..j..|..j..|.
-00001060: 0083 0200 0174 0000 6a01 007c 0000 6a0a  .....t..j..|..j.
-00001070: 0064 0100 7403 0064 0300 6406 0064 0700  .d..t..d..d..d..
-00001080: 6408 0083 0103 7d04 0064 0900 8400 007c  d.....}..d.....|
-00001090: 0400 6a04 006a 0500 8300 0044 8301 007d  ..j..j.....D...}
-000010a0: 0200 7c00 006a 0600 7c00 006a 0b00 7c02  ..|..j..|..j..|.
-000010b0: 0083 0200 0174 0000 6a01 007c 0000 6a0c  .....t..j..|..j.
-000010c0: 0064 0100 7403 0064 0300 6406 0064 0700  .d..t..d..d..d..
-000010d0: 6408 0083 0103 7d05 0064 0a00 8400 007c  d.....}..d.....|
-000010e0: 0500 6a04 006a 0500 8300 0044 8301 007d  ..j..j.....D...}
-000010f0: 0200 7c00 006a 0600 7c00 006a 0b00 7c02  ..|..j..|..j..|.
-00001100: 0083 0200 0174 0000 6a01 007c 0000 6a0d  .....t..j..|..j.
-00001110: 0064 0100 7403 0083 0101 7d06 0064 0b00  .d..t.....}..d..
-00001120: 8400 007c 0600 6a04 006a 0500 8300 0044  ...|..j..j.....D
-00001130: 8301 007d 0200 7c00 006a 0600 7c00 006a  ...}..|..j..|..j
-00001140: 0700 7c02 0083 0200 0164 0000 5328 0c00  ..|......d..S(..
-00001150: 0000 4e52 2400 0000 6301 0000 0002 0000  ..NR$...c.......
-00001160: 0004 0000 0053 0000 0073 2b00 0000 6800  .....S...s+...h.
-00001170: 007c 0000 5d21 007d 0100 7c01 006a 0000  .|..]!.}..|..j..
-00001180: 8300 0074 0100 6b08 0072 0600 7c01 006a  ...t..k..r..|..j
-00001190: 0200 9202 0071 0600 5328 0000 0000 2803  .....q..S(....(.
-000011a0: 0000 0052 2a00 0000 5228 0000 0052 2b00  ...R*...R(...R+.
-000011b0: 0000 2802 0000 0052 2c00 0000 522d 0000  ..(....R,...R-..
-000011c0: 0028 0000 0000 2800 0000 0073 4900 0000  .(....(....sI...
-000011d0: 2f55 7365 7273 2f61 646d 696e 2f57 6f72  /Users/admin/Wor
-000011e0: 6b2f 7072 6f6a 6563 742f 4465 7373 696d  k/project/Dessim
-000011f0: 6f7a 2f70 7968 616d 2d64 6576 2f70 7968  oz/pyham-dev/pyh
-00001200: 616d 2f74 6573 7473 2f74 6573 745f 7461  am/tests/test_ta
-00001210: 786f 6e6f 6d79 2e70 7973 0900 0000 3c73  xonomy.pys....<s
-00001220: 6574 636f 6d70 3e42 0000 0073 0200 0000  etcomp>B...s....
-00001230: 0900 522e 0000 0052 2f00 0000 6301 0000  ..R....R/...c...
-00001240: 0002 0000 0004 0000 0053 0000 0073 2b00  .........S...s+.
-00001250: 0000 6800 007c 0000 5d21 007d 0100 7c01  ..h..|..]!.}..|.
-00001260: 006a 0000 8300 0074 0100 6b08 0072 0600  .j.....t..k..r..
-00001270: 7c01 006a 0200 9202 0071 0600 5328 0000  |..j.....q..S(..
-00001280: 0000 2803 0000 0052 2a00 0000 5228 0000  ..(....R*...R(..
-00001290: 0052 2b00 0000 2802 0000 0052 2c00 0000  .R+...(....R,...
-000012a0: 522d 0000 0028 0000 0000 2800 0000 0073  R-...(....(....s
-000012b0: 4900 0000 2f55 7365 7273 2f61 646d 696e  I.../Users/admin
-000012c0: 2f57 6f72 6b2f 7072 6f6a 6563 742f 4465  /Work/project/De
-000012d0: 7373 696d 6f7a 2f70 7968 616d 2d64 6576  ssimoz/pyham-dev
-000012e0: 2f70 7968 616d 2f74 6573 7473 2f74 6573  /pyham/tests/tes
-000012f0: 745f 7461 786f 6e6f 6d79 2e70 7973 0900  t_taxonomy.pys..
-00001300: 0000 3c73 6574 636f 6d70 3e47 0000 0073  ..<setcomp>G...s
-00001310: 0200 0000 0900 5230 0000 0052 3300 0000  ......R0...R3...
-00001320: 740d 0000 0074 6178 6f6e 6f6d 795f 636f  t....taxonomy_co
-00001330: 6465 6301 0000 0002 0000 0004 0000 0053  dec............S
-00001340: 0000 0073 2b00 0000 6800 007c 0000 5d21  ...s+...h..|..]!
-00001350: 007d 0100 7c01 006a 0000 8300 0074 0100  .}..|..j.....t..
-00001360: 6b08 0072 0600 7c01 006a 0200 9202 0071  k..r..|..j.....q
-00001370: 0600 5328 0000 0000 2803 0000 0052 2a00  ..S(....(....R*.
-00001380: 0000 5228 0000 0052 2b00 0000 2802 0000  ..R(...R+...(...
-00001390: 0052 2c00 0000 522d 0000 0028 0000 0000  .R,...R-...(....
-000013a0: 2800 0000 0073 4900 0000 2f55 7365 7273  (....sI.../Users
-000013b0: 2f61 646d 696e 2f57 6f72 6b2f 7072 6f6a  /admin/Work/proj
-000013c0: 6563 742f 4465 7373 696d 6f7a 2f70 7968  ect/Dessimoz/pyh
-000013d0: 616d 2d64 6576 2f70 7968 616d 2f74 6573  am-dev/pyham/tes
-000013e0: 7473 2f74 6573 745f 7461 786f 6e6f 6d79  ts/test_taxonomy
-000013f0: 2e70 7973 0900 0000 3c73 6574 636f 6d70  .pys....<setcomp
-00001400: 3e4c 0000 0073 0200 0000 0900 6301 0000  >L...s......c...
-00001410: 0002 0000 0004 0000 0053 0000 0073 2b00  .........S...s+.
-00001420: 0000 6800 007c 0000 5d21 007d 0100 7c01  ..h..|..]!.}..|.
-00001430: 006a 0000 8300 0074 0100 6b08 0072 0600  .j.....t..k..r..
-00001440: 7c01 006a 0200 9202 0071 0600 5328 0000  |..j.....q..S(..
-00001450: 0000 2803 0000 0052 2a00 0000 5228 0000  ..(....R*...R(..
-00001460: 0052 2b00 0000 2802 0000 0052 2c00 0000  .R+...(....R,...
-00001470: 522d 0000 0028 0000 0000 2800 0000 0073  R-...(....(....s
-00001480: 4900 0000 2f55 7365 7273 2f61 646d 696e  I.../Users/admin
-00001490: 2f57 6f72 6b2f 7072 6f6a 6563 742f 4465  /Work/project/De
-000014a0: 7373 696d 6f7a 2f70 7968 616d 2d64 6576  ssimoz/pyham-dev
-000014b0: 2f70 7968 616d 2f74 6573 7473 2f74 6573  /pyham/tests/tes
-000014c0: 745f 7461 786f 6e6f 6d79 2e70 7973 0900  t_taxonomy.pys..
-000014d0: 0000 3c73 6574 636f 6d70 3e52 0000 0073  ..<setcomp>R...s
-000014e0: 0200 0000 0900 6301 0000 0002 0000 0004  ......c.........
-000014f0: 0000 0053 0000 0073 2b00 0000 6800 007c  ...S...s+...h..|
-00001500: 0000 5d21 007d 0100 7c01 006a 0000 8300  ..]!.}..|..j....
-00001510: 0074 0100 6b08 0072 0600 7c01 006a 0200  .t..k..r..|..j..
-00001520: 9202 0071 0600 5328 0000 0000 2803 0000  ...q..S(....(...
-00001530: 0052 2a00 0000 5228 0000 0052 2b00 0000  .R*...R(...R+...
-00001540: 2802 0000 0052 2c00 0000 522d 0000 0028  (....R,...R-...(
-00001550: 0000 0000 2800 0000 0073 4900 0000 2f55  ....(....sI.../U
-00001560: 7365 7273 2f61 646d 696e 2f57 6f72 6b2f  sers/admin/Work/
-00001570: 7072 6f6a 6563 742f 4465 7373 696d 6f7a  project/Dessimoz
-00001580: 2f70 7968 616d 2d64 6576 2f70 7968 616d  /pyham-dev/pyham
-00001590: 2f74 6573 7473 2f74 6573 745f 7461 786f  /tests/test_taxo
-000015a0: 6e6f 6d79 2e70 7973 0900 0000 3c73 6574  nomy.pys....<set
-000015b0: 636f 6d70 3e57 0000 0073 0200 0000 0900  comp>W...s......
-000015c0: 280e 0000 0052 0000 0000 5227 0000 0052  (....R....R'...R
-000015d0: 0f00 0000 5228 0000 0052 3600 0000 5237  ....R(...R6...R7
-000015e0: 0000 0052 3800 0000 5213 0000 0052 1900  ...R8...R....R..
-000015f0: 0000 521b 0000 0052 1c00 0000 521f 0000  ..R....R....R...
-00001600: 0052 1d00 0000 5210 0000 0028 0700 0000  .R....R....(....
-00001610: 5222 0000 0052 3900 0000 523a 0000 0052  R"...R9...R:...R
-00001620: 3b00 0000 523c 0000 0074 0200 0000 7436  ;...R<...t....t6
-00001630: 7409 0000 0074 5f73 7570 706f 7274 2800  t....t_support(.
-00001640: 0000 0028 0000 0000 7349 0000 002f 5573  ...(....sI.../Us
-00001650: 6572 732f 6164 6d69 6e2f 576f 726b 2f70  ers/admin/Work/p
-00001660: 726f 6a65 6374 2f44 6573 7369 6d6f 7a2f  roject/Dessimoz/
-00001670: 7079 6861 6d2d 6465 762f 7079 6861 6d2f  pyham-dev/pyham/
-00001680: 7465 7374 732f 7465 7374 5f74 6178 6f6e  tests/test_taxon
-00001690: 6f6d 792e 7079 741b 0000 0074 6573 745f  omy.pyt....test_
-000016a0: 646f 6e74 5f75 7365 5f69 6e74 6572 6e61  dont_use_interna
-000016b0: 6c5f 6e61 6d65 3e00 0000 731e 0000 0000  l_name>...s.....
-000016c0: 0318 0119 0113 031e 0119 0113 0324 0119  .............$..
-000016d0: 0113 0424 0119 0113 0318 0119 0163 0100  ...$.........c..
-000016e0: 0000 0600 0000 0a00 0000 4300 0000 7350  ..........C...sP
-000016f0: 0100 0074 0000 6a01 007c 0000 6a02 0064  ...t..j..|..j..d
-00001700: 0100 7403 0064 0200 6403 0083 0102 7d01  ..t..d..d.....}.
-00001710: 0064 0400 8400 007c 0100 6a04 006a 0500  .d.....|..j..j..
-00001720: 8300 0044 8301 007d 0200 7c00 006a 0600  ...D...}..|..j..
-00001730: 7c00 006a 0700 7c02 0083 0200 0174 0000  |..j..|......t..
-00001740: 6a01 007c 0000 6a08 0064 0100 7403 0064  j..|..j..d..t..d
-00001750: 0200 6405 0064 0600 6407 0064 0800 6409  ..d..d..d..d..d.
-00001760: 0083 0104 7d03 0064 0a00 8400 007c 0300  ....}..d.....|..
-00001770: 6a04 006a 0500 8300 0044 8301 007d 0200  j..j.....D...}..
-00001780: 7c00 006a 0600 7c00 006a 0700 7c02 0083  |..j..|..j..|...
-00001790: 0200 0174 0000 6a01 007c 0000 6a08 0064  ...t..j..|..j..d
-000017a0: 0100 7403 0064 0200 6405 0064 0600 6407  ..t..d..d..d..d.
-000017b0: 0064 0800 6407 0083 0104 7d04 0064 0b00  .d..d.....}..d..
-000017c0: 8400 007c 0400 6a04 006a 0500 8300 0044  ...|..j..j.....D
-000017d0: 8301 007d 0200 7c00 006a 0600 7c00 006a  ...}..|..j..|..j
-000017e0: 0900 7c02 0083 0200 0174 0000 6a01 007c  ..|......t..j..|
-000017f0: 0000 6a08 0064 0100 7403 0064 0200 6405  ..j..d..t..d..d.
-00001800: 0064 0600 6407 0064 0800 640c 0083 0104  .d..d..d..d.....
-00001810: 7d05 0064 0d00 8400 007c 0500 6a04 006a  }..d.....|..j..j
-00001820: 0500 8300 0044 8301 007d 0200 7c00 006a  .....D...}..|..j
-00001830: 0600 7c00 006a 0700 7c02 0083 0200 0164  ..|..j..|......d
-00001840: 0000 5328 0e00 0000 4e52 2400 0000 522e  ..S(....NR$...R.
-00001850: 0000 0052 2f00 0000 6301 0000 0002 0000  ...R/...c.......
-00001860: 0004 0000 0053 0000 0073 2b00 0000 6800  .....S...s+...h.
-00001870: 007c 0000 5d21 007d 0100 7c01 006a 0000  .|..]!.}..|..j..
-00001880: 8300 0074 0100 6b08 0072 0600 7c01 006a  ...t..k..r..|..j
-00001890: 0200 9202 0071 0600 5328 0000 0000 2803  .....q..S(....(.
-000018a0: 0000 0052 2a00 0000 5235 0000 0052 2b00  ...R*...R5...R+.
-000018b0: 0000 2802 0000 0052 2c00 0000 522d 0000  ..(....R,...R-..
-000018c0: 0028 0000 0000 2800 0000 0073 4900 0000  .(....(....sI...
-000018d0: 2f55 7365 7273 2f61 646d 696e 2f57 6f72  /Users/admin/Wor
-000018e0: 6b2f 7072 6f6a 6563 742f 4465 7373 696d  k/project/Dessim
-000018f0: 6f7a 2f70 7968 616d 2d64 6576 2f70 7968  oz/pyham-dev/pyh
-00001900: 616d 2f74 6573 7473 2f74 6573 745f 7461  am/tests/test_ta
-00001910: 786f 6e6f 6d79 2e70 7973 0900 0000 3c73  xonomy.pys....<s
-00001920: 6574 636f 6d70 3e5e 0000 0073 0200 0000  etcomp>^...s....
-00001930: 0900 5230 0000 0052 3100 0000 5232 0000  ..R0...R1...R2..
-00001940: 0052 3300 0000 5234 0000 0063 0100 0000  .R3...R4...c....
-00001950: 0200 0000 0400 0000 5300 0000 732b 0000  ........S...s+..
-00001960: 0068 0000 7c00 005d 2100 7d01 007c 0100  .h..|..]!.}..|..
-00001970: 6a00 0083 0000 7401 006b 0800 7206 007c  j.....t..k..r..|
-00001980: 0100 6a02 0092 0200 7106 0053 2800 0000  ..j.....q..S(...
-00001990: 0028 0300 0000 522a 0000 0052 3500 0000  .(....R*...R5...
-000019a0: 522b 0000 0028 0200 0000 522c 0000 0052  R+...(....R,...R
-000019b0: 2d00 0000 2800 0000 0028 0000 0000 7349  -...(....(....sI
-000019c0: 0000 002f 5573 6572 732f 6164 6d69 6e2f  .../Users/admin/
-000019d0: 576f 726b 2f70 726f 6a65 6374 2f44 6573  Work/project/Des
-000019e0: 7369 6d6f 7a2f 7079 6861 6d2d 6465 762f  simoz/pyham-dev/
-000019f0: 7079 6861 6d2f 7465 7374 732f 7465 7374  pyham/tests/test
-00001a00: 5f74 6178 6f6e 6f6d 792e 7079 7309 0000  _taxonomy.pys...
-00001a10: 003c 7365 7463 6f6d 703e 6300 0000 7302  .<setcomp>c...s.
-00001a20: 0000 0009 0063 0100 0000 0200 0000 0400  .....c..........
-00001a30: 0000 5300 0000 732b 0000 0068 0000 7c00  ..S...s+...h..|.
-00001a40: 005d 2100 7d01 007c 0100 6a00 0083 0000  .]!.}..|..j.....
-00001a50: 7401 006b 0800 7206 007c 0100 6a02 0092  t..k..r..|..j...
-00001a60: 0200 7106 0053 2800 0000 0028 0300 0000  ..q..S(....(....
-00001a70: 522a 0000 0052 3500 0000 522b 0000 0028  R*...R5...R+...(
-00001a80: 0200 0000 522c 0000 0052 2d00 0000 2800  ....R,...R-...(.
-00001a90: 0000 0028 0000 0000 7349 0000 002f 5573  ...(....sI.../Us
-00001aa0: 6572 732f 6164 6d69 6e2f 576f 726b 2f70  ers/admin/Work/p
-00001ab0: 726f 6a65 6374 2f44 6573 7369 6d6f 7a2f  roject/Dessimoz/
-00001ac0: 7079 6861 6d2d 6465 762f 7079 6861 6d2f  pyham-dev/pyham/
-00001ad0: 7465 7374 732f 7465 7374 5f74 6178 6f6e  tests/test_taxon
-00001ae0: 6f6d 792e 7079 7309 0000 003c 7365 7463  omy.pys....<setc
-00001af0: 6f6d 703e 6900 0000 7302 0000 0009 0052  omp>i...s......R
-00001b00: 3f00 0000 6301 0000 0002 0000 0004 0000  ?...c...........
-00001b10: 0053 0000 0073 2b00 0000 6800 007c 0000  .S...s+...h..|..
-00001b20: 5d21 007d 0100 7c01 006a 0000 8300 0074  ]!.}..|..j.....t
-00001b30: 0100 6b08 0072 0600 7c01 006a 0200 9202  ..k..r..|..j....
-00001b40: 0071 0600 5328 0000 0000 2803 0000 0052  .q..S(....(....R
-00001b50: 2a00 0000 5235 0000 0052 2b00 0000 2802  *...R5...R+...(.
-00001b60: 0000 0052 2c00 0000 522d 0000 0028 0000  ...R,...R-...(..
-00001b70: 0000 2800 0000 0073 4900 0000 2f55 7365  ..(....sI.../Use
-00001b80: 7273 2f61 646d 696e 2f57 6f72 6b2f 7072  rs/admin/Work/pr
-00001b90: 6f6a 6563 742f 4465 7373 696d 6f7a 2f70  oject/Dessimoz/p
-00001ba0: 7968 616d 2d64 6576 2f70 7968 616d 2f74  yham-dev/pyham/t
-00001bb0: 6573 7473 2f74 6573 745f 7461 786f 6e6f  ests/test_taxono
-00001bc0: 6d79 2e70 7973 0900 0000 3c73 6574 636f  my.pys....<setco
-00001bd0: 6d70 3e6f 0000 0073 0200 0000 0900 280a  mp>o...s......(.
-00001be0: 0000 0052 0000 0000 5227 0000 0052 1900  ...R....R'...R..
-00001bf0: 0000 5235 0000 0052 3600 0000 5237 0000  ..R5...R6...R7..
-00001c00: 0052 3800 0000 5220 0000 0052 1c00 0000  .R8...R ...R....
-00001c10: 5221 0000 0028 0600 0000 5222 0000 0052  R!...(....R"...R
-00001c20: 3b00 0000 523a 0000 0052 3d00 0000 7402  ;...R:...R=...t.
-00001c30: 0000 0074 3552 4000 0000 2800 0000 0028  ...t5R@...(....(
-00001c40: 0000 0000 7349 0000 002f 5573 6572 732f  ....sI.../Users/
-00001c50: 6164 6d69 6e2f 576f 726b 2f70 726f 6a65  admin/Work/proje
-00001c60: 6374 2f44 6573 7369 6d6f 7a2f 7079 6861  ct/Dessimoz/pyha
-00001c70: 6d2d 6465 762f 7079 6861 6d2f 7465 7374  m-dev/pyham/test
-00001c80: 732f 7465 7374 5f74 6178 6f6e 6f6d 792e  s/test_taxonomy.
-00001c90: 7079 7415 0000 0074 6573 745f 616c 6c5f  pyt....test_all_
-00001ca0: 636f 7272 6563 745f 6e61 6d65 5b00 0000  correct_name[...
-00001cb0: 731c 0000 0000 021e 0119 0113 032a 0119  s............*..
-00001cc0: 0113 0321 0109 0119 0113 0321 0109 0119  ...!.......!....
-00001cd0: 0128 0700 0000 7408 0000 005f 5f6e 616d  .(....t....__nam
-00001ce0: 655f 5f74 0a00 0000 5f5f 6d6f 6475 6c65  e__t....__module
-00001cf0: 5f5f 5223 0000 0052 2900 0000 523e 0000  __R#...R)...R>..
-00001d00: 0052 4200 0000 5244 0000 0028 0000 0000  .RB...RD...(....
-00001d10: 2800 0000 0028 0000 0000 7349 0000 002f  (....(....sI.../
-00001d20: 5573 6572 732f 6164 6d69 6e2f 576f 726b  Users/admin/Work
-00001d30: 2f70 726f 6a65 6374 2f44 6573 7369 6d6f  /project/Dessimo
-00001d40: 7a2f 7079 6861 6d2d 6465 762f 7079 6861  z/pyham-dev/pyha
-00001d50: 6d2f 7465 7374 732f 7465 7374 5f74 6178  m/tests/test_tax
-00001d60: 6f6e 6f6d 792e 7079 5202 0000 0006 0000  onomy.pyR.......
-00001d70: 0073 0a00 0000 0602 0915 0908 0919 091d  .s..............
-00001d80: 2807 0000 0074 0800 0000 756e 6974 7465  (....t....unitte
-00001d90: 7374 7405 0000 0070 7968 616d 5200 0000  stt....pyhamR...
-00001da0: 0052 0100 0000 5214 0000 0074 0800 0000  .R....R....t....
-00001db0: 5465 7374 4361 7365 5202 0000 0028 0000  TestCaseR....(..
-00001dc0: 0000 2800 0000 0028 0000 0000 7349 0000  ..(....(....sI..
-00001dd0: 002f 5573 6572 732f 6164 6d69 6e2f 576f  ./Users/admin/Wo
-00001de0: 726b 2f70 726f 6a65 6374 2f44 6573 7369  rk/project/Dessi
-00001df0: 6d6f 7a2f 7079 6861 6d2d 6465 762f 7079  moz/pyham-dev/py
-00001e00: 6861 6d2f 7465 7374 732f 7465 7374 5f74  ham/tests/test_t
-00001e10: 6178 6f6e 6f6d 792e 7079 7408 0000 003c  axonomy.pyt....<
-00001e20: 6d6f 6475 6c65 3e01 0000 0073 0600 0000  module>....s....
-00001e30: 0c01 1601 0c03                           ......
+00000750: 2800 0000 0073 3600 0000 2f55 7365 7273  (....s6.../Users
+00000760: 2f61 6472 6961 616c 2f52 6570 6f73 6974  /adriaal/Reposit
+00000770: 6f72 6965 732f 4841 4d2f 7465 7374 732f  ories/HAM/tests/
+00000780: 7465 7374 5f74 6178 6f6e 6f6d 792e 7079  test_taxonomy.py
+00000790: 7405 0000 0073 6574 5570 0800 0000 731e  t....setUp....s.
+000007a0: 0000 0000 0109 0109 0109 0112 0112 0224  ...............$
+000007b0: 0118 0118 0324 0124 0124 0109 010f 021b  .....$.$.$......
+000007c0: 0163 0100 0000 0100 0000 0900 0000 4300  .c............C.
+000007d0: 0000 7356 0000 007c 0000 6a00 0074 0100  ..sV...|..j..t..
+000007e0: 8301 008f 1500 0174 0200 6a03 007c 0000  .......t..j..|..
+000007f0: 6a04 0083 0100 0157 6400 0051 587c 0000  j......Wd..QX|..
+00000800: 6a00 0074 0100 8301 008f 1b00 0174 0200  j..t.........t..
+00000810: 6a03 007c 0000 6a04 0064 0100 7405 0083  j..|..j..d..t...
+00000820: 0101 0157 6400 0051 5864 0000 5328 0200  ...Wd..QXd..S(..
+00000830: 0000 4e74 1100 0000 7573 655f 696e 7465  ..Nt....use_inte
+00000840: 726e 616c 5f6e 616d 6528 0600 0000 740c  rnal_name(....t.
+00000850: 0000 0061 7373 6572 7452 6169 7365 7374  ...assertRaisest
+00000860: 0800 0000 4b65 7945 7272 6f72 5200 0000  ....KeyErrorR...
+00000870: 0074 0800 0000 5461 786f 6e6f 6d79 5211  .t....TaxonomyR.
+00000880: 0000 0074 0500 0000 4661 6c73 6528 0100  ...t....False(..
+00000890: 0000 5222 0000 0028 0000 0000 2800 0000  ..R"...(....(...
+000008a0: 0073 3600 0000 2f55 7365 7273 2f61 6472  .s6.../Users/adr
+000008b0: 6961 616c 2f52 6570 6f73 6974 6f72 6965  iaal/Repositorie
+000008c0: 732f 4841 4d2f 7465 7374 732f 7465 7374  s/HAM/tests/test
+000008d0: 5f74 6178 6f6e 6f6d 792e 7079 741a 0000  _taxonomy.pyt...
+000008e0: 0074 6573 745f 6e6f 6e5f 756e 6971 7565  .test_non_unique
+000008f0: 5f6c 6561 665f 6e61 6d65 731d 0000 0073  _leaf_names....s
+00000900: 0800 0000 0001 1001 1602 1001 6301 0000  ............c...
+00000910: 0006 0000 000a 0000 0043 0000 0073 3e01  .........C...s>.
+00000920: 0000 7400 006a 0100 7c00 006a 0200 6401  ..t..j..|..j..d.
+00000930: 0074 0300 8301 017d 0100 6402 0084 0000  .t.....}..d.....
+00000940: 7c01 006a 0400 6a05 0083 0000 4483 0100  |..j..j.....D...
+00000950: 7d02 007c 0000 6a06 007c 0000 6a07 007c  }..|..j..|..j..|
+00000960: 0200 8302 0001 7400 006a 0100 7c00 006a  ......t..j..|..j
+00000970: 0800 6401 0074 0300 6403 0064 0400 8301  ..d..t..d..d....
+00000980: 027d 0300 6405 0084 0000 7c03 006a 0400  .}..d.....|..j..
+00000990: 6a05 0083 0000 4483 0100 7d02 007c 0000  j.....D...}..|..
+000009a0: 6a06 007c 0000 6a09 007c 0200 8302 0001  j..|..j..|......
+000009b0: 7400 006a 0100 7c00 006a 0a00 6401 0074  t..j..|..j..d..t
+000009c0: 0300 6403 0064 0600 6407 0064 0800 6409  ..d..d..d..d..d.
+000009d0: 0064 0800 8301 047d 0400 640a 0084 0000  .d.....}..d.....
+000009e0: 7c04 006a 0400 6a05 0083 0000 4483 0100  |..j..j.....D...
+000009f0: 7d02 007c 0000 6a06 007c 0000 6a09 007c  }..|..j..|..j..|
+00000a00: 0200 8302 0001 7400 006a 0100 7c00 006a  ......t..j..|..j
+00000a10: 0a00 6401 0074 0300 6403 0064 0600 6407  ..d..t..d..d..d.
+00000a20: 0064 0b00 6409 0064 0800 8301 047d 0500  .d..d..d.....}..
+00000a30: 640c 0084 0000 7c05 006a 0400 6a05 0083  d.....|..j..j...
+00000a40: 0000 4483 0100 7d02 007c 0000 6a06 007c  ..D...}..|..j..|
+00000a50: 0000 6a09 007c 0200 8302 0001 6400 0053  ..j..|......d..S
+00000a60: 280d 0000 004e 5224 0000 0063 0100 0000  (....NR$...c....
+00000a70: 0200 0000 0400 0000 5300 0000 732b 0000  ........S...s+..
+00000a80: 0068 0000 7c00 005d 2100 7d01 007c 0100  .h..|..]!.}..|..
+00000a90: 6a00 0083 0000 7401 006b 0800 7206 007c  j.....t..k..r..|
+00000aa0: 0100 6a02 0092 0200 7106 0053 2800 0000  ..j.....q..S(...
+00000ab0: 0028 0300 0000 7407 0000 0069 735f 6c65  .(....t....is_le
+00000ac0: 6166 5228 0000 0074 0400 0000 6e61 6d65  afR(...t....name
+00000ad0: 2802 0000 0074 0200 0000 2e30 7404 0000  (....t.....0t...
+00000ae0: 006e 6f64 6528 0000 0000 2800 0000 0073  .node(....(....s
+00000af0: 3600 0000 2f55 7365 7273 2f61 6472 6961  6.../Users/adria
+00000b00: 616c 2f52 6570 6f73 6974 6f72 6965 732f  al/Repositories/
+00000b10: 4841 4d2f 7465 7374 732f 7465 7374 5f74  HAM/tests/test_t
+00000b20: 6178 6f6e 6f6d 792e 7079 7309 0000 003c  axonomy.pys....<
+00000b30: 7365 7463 6f6d 703e 2900 0000 7302 0000  setcomp>)...s...
+00000b40: 0009 0074 0b00 0000 7472 6565 5f66 6f72  ...t....tree_for
+00000b50: 6d61 7474 0600 0000 6e65 7769 636b 6301  matt....newickc.
+00000b60: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
+00000b70: 2b00 0000 6800 007c 0000 5d21 007d 0100  +...h..|..]!.}..
+00000b80: 7c01 006a 0000 8300 0074 0100 6b08 0072  |..j.....t..k..r
+00000b90: 0600 7c01 006a 0200 9202 0071 0600 5328  ..|..j.....q..S(
+00000ba0: 0000 0000 2803 0000 0052 2a00 0000 5228  ....(....R*...R(
+00000bb0: 0000 0052 2b00 0000 2802 0000 0052 2c00  ...R+...(....R,.
+00000bc0: 0000 522d 0000 0028 0000 0000 2800 0000  ..R-...(....(...
+00000bd0: 0073 3600 0000 2f55 7365 7273 2f61 6472  .s6.../Users/adr
+00000be0: 6961 616c 2f52 6570 6f73 6974 6f72 6965  iaal/Repositorie
+00000bf0: 732f 4841 4d2f 7465 7374 732f 7465 7374  s/HAM/tests/test
+00000c00: 5f74 6178 6f6e 6f6d 792e 7079 7309 0000  _taxonomy.pys...
+00000c10: 003c 7365 7463 6f6d 703e 2e00 0000 7302  .<setcomp>....s.
+00000c20: 0000 0009 0074 0800 0000 7068 796c 6f78  .....t....phylox
+00000c30: 6d6c 741a 0000 0070 6879 6c6f 786d 6c5f  mlt....phyloxml_
+00000c40: 696e 7465 726e 616c 5f6e 616d 655f 7461  internal_name_ta
+00000c50: 6774 1800 0000 7461 786f 6e6f 6d79 5f73  gt....taxonomy_s
+00000c60: 6369 656e 7469 6669 635f 6e61 6d65 7416  cientific_namet.
+00000c70: 0000 0070 6879 6c6f 786d 6c5f 6c65 6166  ...phyloxml_leaf
+00000c80: 5f6e 616d 655f 7461 6763 0100 0000 0200  _name_tagc......
+00000c90: 0000 0400 0000 5300 0000 732b 0000 0068  ......S...s+...h
+00000ca0: 0000 7c00 005d 2100 7d01 007c 0100 6a00  ..|..]!.}..|..j.
+00000cb0: 0083 0000 7401 006b 0800 7206 007c 0100  ....t..k..r..|..
+00000cc0: 6a02 0092 0200 7106 0053 2800 0000 0028  j.....q..S(....(
+00000cd0: 0300 0000 522a 0000 0052 2800 0000 522b  ....R*...R(...R+
+00000ce0: 0000 0028 0200 0000 522c 0000 0052 2d00  ...(....R,...R-.
+00000cf0: 0000 2800 0000 0028 0000 0000 7336 0000  ..(....(....s6..
+00000d00: 002f 5573 6572 732f 6164 7269 6161 6c2f  ./Users/adriaal/
+00000d10: 5265 706f 7369 746f 7269 6573 2f48 414d  Repositories/HAM
+00000d20: 2f74 6573 7473 2f74 6573 745f 7461 786f  /tests/test_taxo
+00000d30: 6e6f 6d79 2e70 7973 0900 0000 3c73 6574  nomy.pys....<set
+00000d40: 636f 6d70 3e33 0000 0073 0200 0000 0900  comp>3...s......
+00000d50: 740a 0000 0063 6c61 6465 5f6e 616d 6563  t....clade_namec
+00000d60: 0100 0000 0200 0000 0400 0000 5300 0000  ............S...
+00000d70: 732b 0000 0068 0000 7c00 005d 2100 7d01  s+...h..|..]!.}.
+00000d80: 007c 0100 6a00 0083 0000 7401 006b 0800  .|..j.....t..k..
+00000d90: 7206 007c 0100 6a02 0092 0200 7106 0053  r..|..j.....q..S
+00000da0: 2800 0000 0028 0300 0000 522a 0000 0052  (....(....R*...R
+00000db0: 2800 0000 522b 0000 0028 0200 0000 522c  (...R+...(....R,
+00000dc0: 0000 0052 2d00 0000 2800 0000 0028 0000  ...R-...(....(..
+00000dd0: 0000 7336 0000 002f 5573 6572 732f 6164  ..s6.../Users/ad
+00000de0: 7269 6161 6c2f 5265 706f 7369 746f 7269  riaal/Repositori
+00000df0: 6573 2f48 414d 2f74 6573 7473 2f74 6573  es/HAM/tests/tes
+00000e00: 745f 7461 786f 6e6f 6d79 2e70 7973 0900  t_taxonomy.pys..
+00000e10: 0000 3c73 6574 636f 6d70 3e3a 0000 0073  ..<setcomp>:...s
+00000e20: 0200 0000 0900 280b 0000 0052 0000 0000  ......(....R....
+00000e30: 5227 0000 0052 0f00 0000 7404 0000 0054  R'...R....t....T
+00000e40: 7275 6574 0400 0000 7472 6565 7408 0000  ruet....treet...
+00000e50: 0074 7261 7665 7273 6574 0e00 0000 6173  .traverset....as
+00000e60: 7365 7274 5365 7445 7175 616c 5212 0000  sertSetEqualR...
+00000e70: 0052 1900 0000 521a 0000 0052 1c00 0000  .R....R....R....
+00000e80: 2806 0000 0052 2200 0000 7401 0000 0074  (....R"...t....t
+00000e90: 740d 0000 006f 6273 6572 7665 645f 6e61  t....observed_na
+00000ea0: 6d65 7402 0000 0074 3274 0200 0000 7433  met....t2t....t3
+00000eb0: 7402 0000 0074 3428 0000 0000 2800 0000  t....t4(....(...
+00000ec0: 0073 3600 0000 2f55 7365 7273 2f61 6472  .s6.../Users/adr
+00000ed0: 6961 616c 2f52 6570 6f73 6974 6f72 6965  iaal/Repositorie
+00000ee0: 732f 4841 4d2f 7465 7374 732f 7465 7374  s/HAM/tests/test
+00000ef0: 5f74 6178 6f6e 6f6d 792e 7079 7416 0000  _taxonomy.pyt...
+00000f00: 0074 6573 745f 7573 655f 696e 7465 726e  .test_use_intern
+00000f10: 616c 5f6e 616d 6525 0000 0073 1c00 0000  al_name%...s....
+00000f20: 0003 1801 1901 1303 1e01 1901 1303 2a01  ..............*.
+00000f30: 1901 1303 1b01 0601 0901 1901 6301 0000  ............c...
+00000f40: 0007 0000 0008 0000 0043 0000 0073 7601  .........C...sv.
+00000f50: 0000 7400 006a 0100 7c00 006a 0200 6401  ..t..j..|..j..d.
+00000f60: 0074 0300 8301 017d 0100 6402 0084 0000  .t.....}..d.....
+00000f70: 7c01 006a 0400 6a05 0083 0000 4483 0100  |..j..j.....D...
+00000f80: 7d02 007c 0000 6a06 007c 0000 6a07 007c  }..|..j..|..j..|
+00000f90: 0200 8302 0001 7400 006a 0100 7c00 006a  ......t..j..|..j
+00000fa0: 0800 6401 0074 0300 6403 0064 0400 8301  ..d..t..d..d....
+00000fb0: 027d 0300 6405 0084 0000 7c03 006a 0400  .}..d.....|..j..
+00000fc0: 6a05 0083 0000 4483 0100 7d02 007c 0000  j.....D...}..|..
+00000fd0: 6a06 007c 0000 6a09 007c 0200 8302 0001  j..|..j..|......
+00000fe0: 7400 006a 0100 7c00 006a 0a00 6401 0074  t..j..|..j..d..t
+00000ff0: 0300 6403 0064 0600 6407 0064 0800 8301  ..d..d..d..d....
+00001000: 037d 0400 6409 0084 0000 7c04 006a 0400  .}..d.....|..j..
+00001010: 6a05 0083 0000 4483 0100 7d02 007c 0000  j.....D...}..|..
+00001020: 6a06 007c 0000 6a0b 007c 0200 8302 0001  j..|..j..|......
+00001030: 7400 006a 0100 7c00 006a 0c00 6401 0074  t..j..|..j..d..t
+00001040: 0300 6403 0064 0600 6407 0064 0800 8301  ..d..d..d..d....
+00001050: 037d 0500 640a 0084 0000 7c05 006a 0400  .}..d.....|..j..
+00001060: 6a05 0083 0000 4483 0100 7d02 007c 0000  j.....D...}..|..
+00001070: 6a06 007c 0000 6a0b 007c 0200 8302 0001  j..|..j..|......
+00001080: 7400 006a 0100 7c00 006a 0d00 6401 0074  t..j..|..j..d..t
+00001090: 0300 8301 017d 0600 640b 0084 0000 7c06  .....}..d.....|.
+000010a0: 006a 0400 6a05 0083 0000 4483 0100 7d02  .j..j.....D...}.
+000010b0: 007c 0000 6a06 007c 0000 6a07 007c 0200  .|..j..|..j..|..
+000010c0: 8302 0001 6400 0053 280c 0000 004e 5224  ....d..S(....NR$
+000010d0: 0000 0063 0100 0000 0200 0000 0400 0000  ...c............
+000010e0: 5300 0000 732b 0000 0068 0000 7c00 005d  S...s+...h..|..]
+000010f0: 2100 7d01 007c 0100 6a00 0083 0000 7401  !.}..|..j.....t.
+00001100: 006b 0800 7206 007c 0100 6a02 0092 0200  .k..r..|..j.....
+00001110: 7106 0053 2800 0000 0028 0300 0000 522a  q..S(....(....R*
+00001120: 0000 0052 2800 0000 522b 0000 0028 0200  ...R(...R+...(..
+00001130: 0000 522c 0000 0052 2d00 0000 2800 0000  ..R,...R-...(...
+00001140: 0028 0000 0000 7336 0000 002f 5573 6572  .(....s6.../User
+00001150: 732f 6164 7269 6161 6c2f 5265 706f 7369  s/adriaal/Reposi
+00001160: 746f 7269 6573 2f48 414d 2f74 6573 7473  tories/HAM/tests
+00001170: 2f74 6573 745f 7461 786f 6e6f 6d79 2e70  /test_taxonomy.p
+00001180: 7973 0900 0000 3c73 6574 636f 6d70 3e42  ys....<setcomp>B
+00001190: 0000 0073 0200 0000 0900 522e 0000 0052  ...s......R....R
+000011a0: 2f00 0000 6301 0000 0002 0000 0004 0000  /...c...........
+000011b0: 0053 0000 0073 2b00 0000 6800 007c 0000  .S...s+...h..|..
+000011c0: 5d21 007d 0100 7c01 006a 0000 8300 0074  ]!.}..|..j.....t
+000011d0: 0100 6b08 0072 0600 7c01 006a 0200 9202  ..k..r..|..j....
+000011e0: 0071 0600 5328 0000 0000 2803 0000 0052  .q..S(....(....R
+000011f0: 2a00 0000 5228 0000 0052 2b00 0000 2802  *...R(...R+...(.
+00001200: 0000 0052 2c00 0000 522d 0000 0028 0000  ...R,...R-...(..
+00001210: 0000 2800 0000 0073 3600 0000 2f55 7365  ..(....s6.../Use
+00001220: 7273 2f61 6472 6961 616c 2f52 6570 6f73  rs/adriaal/Repos
+00001230: 6974 6f72 6965 732f 4841 4d2f 7465 7374  itories/HAM/test
+00001240: 732f 7465 7374 5f74 6178 6f6e 6f6d 792e  s/test_taxonomy.
+00001250: 7079 7309 0000 003c 7365 7463 6f6d 703e  pys....<setcomp>
+00001260: 4700 0000 7302 0000 0009 0052 3000 0000  G...s......R0...
+00001270: 5233 0000 0074 0d00 0000 7461 786f 6e6f  R3...t....taxono
+00001280: 6d79 5f63 6f64 6563 0100 0000 0200 0000  my_codec........
+00001290: 0400 0000 5300 0000 732b 0000 0068 0000  ....S...s+...h..
+000012a0: 7c00 005d 2100 7d01 007c 0100 6a00 0083  |..]!.}..|..j...
+000012b0: 0000 7401 006b 0800 7206 007c 0100 6a02  ..t..k..r..|..j.
+000012c0: 0092 0200 7106 0053 2800 0000 0028 0300  ....q..S(....(..
+000012d0: 0000 522a 0000 0052 2800 0000 522b 0000  ..R*...R(...R+..
+000012e0: 0028 0200 0000 522c 0000 0052 2d00 0000  .(....R,...R-...
+000012f0: 2800 0000 0028 0000 0000 7336 0000 002f  (....(....s6.../
+00001300: 5573 6572 732f 6164 7269 6161 6c2f 5265  Users/adriaal/Re
+00001310: 706f 7369 746f 7269 6573 2f48 414d 2f74  positories/HAM/t
+00001320: 6573 7473 2f74 6573 745f 7461 786f 6e6f  ests/test_taxono
+00001330: 6d79 2e70 7973 0900 0000 3c73 6574 636f  my.pys....<setco
+00001340: 6d70 3e4c 0000 0073 0200 0000 0900 6301  mp>L...s......c.
+00001350: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
+00001360: 2b00 0000 6800 007c 0000 5d21 007d 0100  +...h..|..]!.}..
+00001370: 7c01 006a 0000 8300 0074 0100 6b08 0072  |..j.....t..k..r
+00001380: 0600 7c01 006a 0200 9202 0071 0600 5328  ..|..j.....q..S(
+00001390: 0000 0000 2803 0000 0052 2a00 0000 5228  ....(....R*...R(
+000013a0: 0000 0052 2b00 0000 2802 0000 0052 2c00  ...R+...(....R,.
+000013b0: 0000 522d 0000 0028 0000 0000 2800 0000  ..R-...(....(...
+000013c0: 0073 3600 0000 2f55 7365 7273 2f61 6472  .s6.../Users/adr
+000013d0: 6961 616c 2f52 6570 6f73 6974 6f72 6965  iaal/Repositorie
+000013e0: 732f 4841 4d2f 7465 7374 732f 7465 7374  s/HAM/tests/test
+000013f0: 5f74 6178 6f6e 6f6d 792e 7079 7309 0000  _taxonomy.pys...
+00001400: 003c 7365 7463 6f6d 703e 5200 0000 7302  .<setcomp>R...s.
+00001410: 0000 0009 0063 0100 0000 0200 0000 0400  .....c..........
+00001420: 0000 5300 0000 732b 0000 0068 0000 7c00  ..S...s+...h..|.
+00001430: 005d 2100 7d01 007c 0100 6a00 0083 0000  .]!.}..|..j.....
+00001440: 7401 006b 0800 7206 007c 0100 6a02 0092  t..k..r..|..j...
+00001450: 0200 7106 0053 2800 0000 0028 0300 0000  ..q..S(....(....
+00001460: 522a 0000 0052 2800 0000 522b 0000 0028  R*...R(...R+...(
+00001470: 0200 0000 522c 0000 0052 2d00 0000 2800  ....R,...R-...(.
+00001480: 0000 0028 0000 0000 7336 0000 002f 5573  ...(....s6.../Us
+00001490: 6572 732f 6164 7269 6161 6c2f 5265 706f  ers/adriaal/Repo
+000014a0: 7369 746f 7269 6573 2f48 414d 2f74 6573  sitories/HAM/tes
+000014b0: 7473 2f74 6573 745f 7461 786f 6e6f 6d79  ts/test_taxonomy
+000014c0: 2e70 7973 0900 0000 3c73 6574 636f 6d70  .pys....<setcomp
+000014d0: 3e57 0000 0073 0200 0000 0900 280e 0000  >W...s......(...
+000014e0: 0052 0000 0000 5227 0000 0052 0f00 0000  .R....R'...R....
+000014f0: 5228 0000 0052 3600 0000 5237 0000 0052  R(...R6...R7...R
+00001500: 3800 0000 5213 0000 0052 1900 0000 521b  8...R....R....R.
+00001510: 0000 0052 1c00 0000 521f 0000 0052 1d00  ...R....R....R..
+00001520: 0000 5210 0000 0028 0700 0000 5222 0000  ..R....(....R"..
+00001530: 0052 3900 0000 523a 0000 0052 3b00 0000  .R9...R:...R;...
+00001540: 523c 0000 0074 0200 0000 7436 7409 0000  R<...t....t6t...
+00001550: 0074 5f73 7570 706f 7274 2800 0000 0028  .t_support(....(
+00001560: 0000 0000 7336 0000 002f 5573 6572 732f  ....s6.../Users/
+00001570: 6164 7269 6161 6c2f 5265 706f 7369 746f  adriaal/Reposito
+00001580: 7269 6573 2f48 414d 2f74 6573 7473 2f74  ries/HAM/tests/t
+00001590: 6573 745f 7461 786f 6e6f 6d79 2e70 7974  est_taxonomy.pyt
+000015a0: 1b00 0000 7465 7374 5f64 6f6e 745f 7573  ....test_dont_us
+000015b0: 655f 696e 7465 726e 616c 5f6e 616d 653e  e_internal_name>
+000015c0: 0000 0073 1e00 0000 0003 1801 1901 1303  ...s............
+000015d0: 1e01 1901 1303 2401 1901 1304 2401 1901  ......$.....$...
+000015e0: 1303 1801 1901 6301 0000 0006 0000 000a  ......c.........
+000015f0: 0000 0043 0000 0073 5001 0000 7400 006a  ...C...sP...t..j
+00001600: 0100 7c00 006a 0200 6401 0074 0300 6402  ..|..j..d..t..d.
+00001610: 0064 0300 8301 027d 0100 6404 0084 0000  .d.....}..d.....
+00001620: 7c01 006a 0400 6a05 0083 0000 4483 0100  |..j..j.....D...
+00001630: 7d02 007c 0000 6a06 007c 0000 6a07 007c  }..|..j..|..j..|
+00001640: 0200 8302 0001 7400 006a 0100 7c00 006a  ......t..j..|..j
+00001650: 0800 6401 0074 0300 6402 0064 0500 6406  ..d..t..d..d..d.
+00001660: 0064 0700 6408 0064 0900 8301 047d 0300  .d..d..d.....}..
+00001670: 640a 0084 0000 7c03 006a 0400 6a05 0083  d.....|..j..j...
+00001680: 0000 4483 0100 7d02 007c 0000 6a06 007c  ..D...}..|..j..|
+00001690: 0000 6a07 007c 0200 8302 0001 7400 006a  ..j..|......t..j
+000016a0: 0100 7c00 006a 0800 6401 0074 0300 6402  ..|..j..d..t..d.
+000016b0: 0064 0500 6406 0064 0700 6408 0064 0700  .d..d..d..d..d..
+000016c0: 8301 047d 0400 640b 0084 0000 7c04 006a  ...}..d.....|..j
+000016d0: 0400 6a05 0083 0000 4483 0100 7d02 007c  ..j.....D...}..|
+000016e0: 0000 6a06 007c 0000 6a09 007c 0200 8302  ..j..|..j..|....
+000016f0: 0001 7400 006a 0100 7c00 006a 0800 6401  ..t..j..|..j..d.
+00001700: 0074 0300 6402 0064 0500 6406 0064 0700  .t..d..d..d..d..
+00001710: 6408 0064 0c00 8301 047d 0500 640d 0084  d..d.....}..d...
+00001720: 0000 7c05 006a 0400 6a05 0083 0000 4483  ..|..j..j.....D.
+00001730: 0100 7d02 007c 0000 6a06 007c 0000 6a07  ..}..|..j..|..j.
+00001740: 007c 0200 8302 0001 6400 0053 280e 0000  .|......d..S(...
+00001750: 004e 5224 0000 0052 2e00 0000 522f 0000  .NR$...R....R/..
+00001760: 0063 0100 0000 0200 0000 0400 0000 5300  .c............S.
+00001770: 0000 732b 0000 0068 0000 7c00 005d 2100  ..s+...h..|..]!.
+00001780: 7d01 007c 0100 6a00 0083 0000 7401 006b  }..|..j.....t..k
+00001790: 0800 7206 007c 0100 6a02 0092 0200 7106  ..r..|..j.....q.
+000017a0: 0053 2800 0000 0028 0300 0000 522a 0000  .S(....(....R*..
+000017b0: 0052 3500 0000 522b 0000 0028 0200 0000  .R5...R+...(....
+000017c0: 522c 0000 0052 2d00 0000 2800 0000 0028  R,...R-...(....(
+000017d0: 0000 0000 7336 0000 002f 5573 6572 732f  ....s6.../Users/
+000017e0: 6164 7269 6161 6c2f 5265 706f 7369 746f  adriaal/Reposito
+000017f0: 7269 6573 2f48 414d 2f74 6573 7473 2f74  ries/HAM/tests/t
+00001800: 6573 745f 7461 786f 6e6f 6d79 2e70 7973  est_taxonomy.pys
+00001810: 0900 0000 3c73 6574 636f 6d70 3e5e 0000  ....<setcomp>^..
+00001820: 0073 0200 0000 0900 5230 0000 0052 3100  .s......R0...R1.
+00001830: 0000 5232 0000 0052 3300 0000 5234 0000  ..R2...R3...R4..
+00001840: 0063 0100 0000 0200 0000 0400 0000 5300  .c............S.
+00001850: 0000 732b 0000 0068 0000 7c00 005d 2100  ..s+...h..|..]!.
+00001860: 7d01 007c 0100 6a00 0083 0000 7401 006b  }..|..j.....t..k
+00001870: 0800 7206 007c 0100 6a02 0092 0200 7106  ..r..|..j.....q.
+00001880: 0053 2800 0000 0028 0300 0000 522a 0000  .S(....(....R*..
+00001890: 0052 3500 0000 522b 0000 0028 0200 0000  .R5...R+...(....
+000018a0: 522c 0000 0052 2d00 0000 2800 0000 0028  R,...R-...(....(
+000018b0: 0000 0000 7336 0000 002f 5573 6572 732f  ....s6.../Users/
+000018c0: 6164 7269 6161 6c2f 5265 706f 7369 746f  adriaal/Reposito
+000018d0: 7269 6573 2f48 414d 2f74 6573 7473 2f74  ries/HAM/tests/t
+000018e0: 6573 745f 7461 786f 6e6f 6d79 2e70 7973  est_taxonomy.pys
+000018f0: 0900 0000 3c73 6574 636f 6d70 3e63 0000  ....<setcomp>c..
+00001900: 0073 0200 0000 0900 6301 0000 0002 0000  .s......c.......
+00001910: 0004 0000 0053 0000 0073 2b00 0000 6800  .....S...s+...h.
+00001920: 007c 0000 5d21 007d 0100 7c01 006a 0000  .|..]!.}..|..j..
+00001930: 8300 0074 0100 6b08 0072 0600 7c01 006a  ...t..k..r..|..j
+00001940: 0200 9202 0071 0600 5328 0000 0000 2803  .....q..S(....(.
+00001950: 0000 0052 2a00 0000 5235 0000 0052 2b00  ...R*...R5...R+.
+00001960: 0000 2802 0000 0052 2c00 0000 522d 0000  ..(....R,...R-..
+00001970: 0028 0000 0000 2800 0000 0073 3600 0000  .(....(....s6...
+00001980: 2f55 7365 7273 2f61 6472 6961 616c 2f52  /Users/adriaal/R
+00001990: 6570 6f73 6974 6f72 6965 732f 4841 4d2f  epositories/HAM/
+000019a0: 7465 7374 732f 7465 7374 5f74 6178 6f6e  tests/test_taxon
+000019b0: 6f6d 792e 7079 7309 0000 003c 7365 7463  omy.pys....<setc
+000019c0: 6f6d 703e 6900 0000 7302 0000 0009 0052  omp>i...s......R
+000019d0: 3f00 0000 6301 0000 0002 0000 0004 0000  ?...c...........
+000019e0: 0053 0000 0073 2b00 0000 6800 007c 0000  .S...s+...h..|..
+000019f0: 5d21 007d 0100 7c01 006a 0000 8300 0074  ]!.}..|..j.....t
+00001a00: 0100 6b08 0072 0600 7c01 006a 0200 9202  ..k..r..|..j....
+00001a10: 0071 0600 5328 0000 0000 2803 0000 0052  .q..S(....(....R
+00001a20: 2a00 0000 5235 0000 0052 2b00 0000 2802  *...R5...R+...(.
+00001a30: 0000 0052 2c00 0000 522d 0000 0028 0000  ...R,...R-...(..
+00001a40: 0000 2800 0000 0073 3600 0000 2f55 7365  ..(....s6.../Use
+00001a50: 7273 2f61 6472 6961 616c 2f52 6570 6f73  rs/adriaal/Repos
+00001a60: 6974 6f72 6965 732f 4841 4d2f 7465 7374  itories/HAM/test
+00001a70: 732f 7465 7374 5f74 6178 6f6e 6f6d 792e  s/test_taxonomy.
+00001a80: 7079 7309 0000 003c 7365 7463 6f6d 703e  pys....<setcomp>
+00001a90: 6f00 0000 7302 0000 0009 0028 0a00 0000  o...s......(....
+00001aa0: 5200 0000 0052 2700 0000 5219 0000 0052  R....R'...R....R
+00001ab0: 3500 0000 5236 0000 0052 3700 0000 5238  5...R6...R7...R8
+00001ac0: 0000 0052 2000 0000 521c 0000 0052 2100  ...R ...R....R!.
+00001ad0: 0000 2806 0000 0052 2200 0000 523b 0000  ..(....R"...R;..
+00001ae0: 0052 3a00 0000 523d 0000 0074 0200 0000  .R:...R=...t....
+00001af0: 7435 5240 0000 0028 0000 0000 2800 0000  t5R@...(....(...
+00001b00: 0073 3600 0000 2f55 7365 7273 2f61 6472  .s6.../Users/adr
+00001b10: 6961 616c 2f52 6570 6f73 6974 6f72 6965  iaal/Repositorie
+00001b20: 732f 4841 4d2f 7465 7374 732f 7465 7374  s/HAM/tests/test
+00001b30: 5f74 6178 6f6e 6f6d 792e 7079 7415 0000  _taxonomy.pyt...
+00001b40: 0074 6573 745f 616c 6c5f 636f 7272 6563  .test_all_correc
+00001b50: 745f 6e61 6d65 5b00 0000 731c 0000 0000  t_name[...s.....
+00001b60: 021e 0119 0113 032a 0119 0113 0321 0109  .......*.....!..
+00001b70: 0119 0113 0321 0109 0119 0128 0700 0000  .....!.....(....
+00001b80: 7408 0000 005f 5f6e 616d 655f 5f74 0a00  t....__name__t..
+00001b90: 0000 5f5f 6d6f 6475 6c65 5f5f 5223 0000  ..__module__R#..
+00001ba0: 0052 2900 0000 523e 0000 0052 4200 0000  .R)...R>...RB...
+00001bb0: 5244 0000 0028 0000 0000 2800 0000 0028  RD...(....(....(
+00001bc0: 0000 0000 7336 0000 002f 5573 6572 732f  ....s6.../Users/
+00001bd0: 6164 7269 6161 6c2f 5265 706f 7369 746f  adriaal/Reposito
+00001be0: 7269 6573 2f48 414d 2f74 6573 7473 2f74  ries/HAM/tests/t
+00001bf0: 6573 745f 7461 786f 6e6f 6d79 2e70 7952  est_taxonomy.pyR
+00001c00: 0200 0000 0600 0000 730a 0000 0006 0209  ........s.......
+00001c10: 1509 0809 1909 1d28 0700 0000 7408 0000  .......(....t...
+00001c20: 0075 6e69 7474 6573 7474 0500 0000 7079  .unittestt....py
+00001c30: 6861 6d52 0000 0000 5201 0000 0052 1400  hamR....R....R..
+00001c40: 0000 7408 0000 0054 6573 7443 6173 6552  ..t....TestCaseR
+00001c50: 0200 0000 2800 0000 0028 0000 0000 2800  ....(....(....(.
+00001c60: 0000 0073 3600 0000 2f55 7365 7273 2f61  ...s6.../Users/a
+00001c70: 6472 6961 616c 2f52 6570 6f73 6974 6f72  driaal/Repositor
+00001c80: 6965 732f 4841 4d2f 7465 7374 732f 7465  ies/HAM/tests/te
+00001c90: 7374 5f74 6178 6f6e 6f6d 792e 7079 7408  st_taxonomy.pyt.
+00001ca0: 0000 003c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00001cb0: 0600 0000 0c01 1601 0c03                 ..........
```

### Comparing `pyham-1.1.8/tests/test_abstractgene.py` & `pyham-1.1.9/tests/test_abstractgene.py`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/tests/test_orthoxmlparser.pyc` & `pyham-1.1.9/tests/test_orthoxmlparser.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 2.7 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,1386 +1,1225 @@
-00000000: 03f3 0d0a 6e8c e85e 6300 0000 0000 0000  ....n..^c.......
-00000010: 0003 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
+00000000: 03f3 0d0a 0bc8 8f5b 6300 0000 0000 0000  .......[c.......
+00000010: 0003 0000 0040 0000 0073 a300 0000 6400  .....@...s....d.
 00000020: 0064 0100 6c00 005a 0000 6400 0064 0100  .d..l..Z..d..d..
 00000030: 6c01 005a 0100 6400 0064 0200 6c02 006d  l..Z..d..d..l..m
 00000040: 0300 5a03 0001 6400 0064 0300 6c02 006d  ..Z...d..d..l..m
-00000050: 0400 5a04 0001 6400 0064 0400 6c02 006d  ..Z...d..d..l..m
-00000060: 0500 5a05 0001 6400 0064 0100 6c06 005a  ..Z...d..d..l..Z
-00000070: 0600 6400 0064 0100 6c07 005a 0800 6400  ..d..d..l..Z..d.
-00000080: 0064 0500 6c01 006d 0900 5a09 0001 6406  .d..l..m..Z...d.
-00000090: 0065 0100 6a0a 0066 0100 6407 0084 0000  .e..j..f..d.....
-000000a0: 8300 0059 5a0b 0064 0800 6501 006a 0a00  ...YZ..d..e..j..
-000000b0: 6601 0064 0900 8400 0083 0000 595a 0c00  f..d........YZ..
-000000c0: 640a 0065 0100 6a0a 0066 0100 640b 0084  d..e..j..f..d...
-000000d0: 0000 8300 0059 5a0d 0065 0e00 640c 006b  .....YZ..e..d..k
-000000e0: 0200 72d4 0065 0100 6a0f 0083 0000 016e  ..r..e..j......n
-000000f0: 0000 6401 0053 280d 0000 0069 ffff ffff  ..d..S(....i....
-00000100: 4e28 0100 0000 7403 0000 0068 616d 2801  N(....t....ham(.
-00000110: 0000 0074 0c00 0000 6162 7374 7261 6374  ...t....abstract
-00000120: 6765 6e65 2801 0000 0074 0500 0000 7574  gene(....t....ut
-00000130: 696c 7328 0100 0000 7404 0000 0073 6b69  ils(....t....ski
-00000140: 7074 1200 0000 4f72 7468 6f58 4d4c 5061  pt....OrthoXMLPa
-00000150: 7273 6572 5465 7374 6300 0000 0000 0000  rserTestc.......
-00000160: 0001 0000 0042 0000 0073 6b00 0000 6500  .....B...sk...e.
-00000170: 005a 0100 6400 0084 0000 5a02 0064 0100  .Z..d.....Z..d..
-00000180: 8400 005a 0300 6402 0084 0000 5a04 0064  ...Z..d.....Z..d
-00000190: 0300 8400 005a 0500 6404 0084 0000 5a06  .....Z..d.....Z.
-000001a0: 0064 0500 8400 005a 0700 6406 0084 0000  .d.....Z..d.....
-000001b0: 5a08 0064 0700 8400 005a 0900 6408 0084  Z..d.....Z..d...
-000001c0: 0000 5a0a 0064 0900 8400 005a 0b00 640a  ..Z..d.....Z..d.
-000001d0: 0084 0000 5a0c 0052 5328 0b00 0000 6302  ....Z..RS(....c.
-000001e0: 0000 0002 0000 0005 0000 0043 0000 0073  ...........C...s
-000001f0: 6c00 0000 7400 007c 0100 7401 006a 0200  l...t..|..t..j..
-00000200: 6a03 0083 0200 721c 007c 0100 6a04 0053  j.....r..|..j..S
-00000210: 7400 007c 0100 7401 006a 0200 6a05 0083  t..|..t..j..j...
-00000220: 0200 723e 007c 0100 6a06 006a 0700 6a08  ..r>.|..j..j..j.
-00000230: 0053 7409 0064 0100 6a0a 0074 0100 6a02  .St..d..j..t..j.
-00000240: 006a 0b00 6a0c 0074 0d00 7c01 0083 0100  .j..j..t..|.....
-00000250: 6a0c 0083 0200 8301 0082 0100 6400 0053  j...........d..S
-00000260: 2802 0000 004e 7323 0000 0065 7870 6563  (....Ns#...expec
-00000270: 7420 7375 6263 6c61 7373 206f 626a 206f  t subclass obj o
-00000280: 6620 277b 7d27 2c20 676f 7420 7b7d 280e  f '{}', got {}(.
-00000290: 0000 0074 0a00 0000 6973 696e 7374 616e  ...t....isinstan
-000002a0: 6365 5200 0000 0052 0100 0000 7404 0000  ceR....R....t...
-000002b0: 0047 656e 6574 0900 0000 756e 6971 7565  .Genet....unique
-000002c0: 5f69 6474 0300 0000 484f 4774 0600 0000  _idt....HOGt....
-000002d0: 6765 6e6f 6d65 7405 0000 0074 6178 6f6e  genomet....taxon
-000002e0: 7404 0000 006e 616d 6574 0900 0000 5479  t....namet....Ty
-000002f0: 7065 4572 726f 7274 0600 0000 666f 726d  peErrort....form
-00000300: 6174 740c 0000 0041 6273 7472 6163 7447  att....AbstractG
-00000310: 656e 6574 0800 0000 5f5f 6e61 6d65 5f5f  enet....__name__
-00000320: 7404 0000 0074 7970 6528 0200 0000 7404  t....type(....t.
-00000330: 0000 0073 656c 6674 0400 0000 6974 656d  ...selft....item
-00000340: 2800 0000 0028 0000 0000 734f 0000 002f  (....(....sO.../
-00000350: 5573 6572 732f 6164 6d69 6e2f 576f 726b  Users/admin/Work
-00000360: 2f70 726f 6a65 6374 2f44 6573 7369 6d6f  /project/Dessimo
-00000370: 7a2f 7079 6861 6d2d 6465 762f 7079 6861  z/pyham-dev/pyha
-00000380: 6d2f 7465 7374 732f 7465 7374 5f6f 7274  m/tests/test_ort
-00000390: 686f 786d 6c70 6172 7365 722e 7079 740f  hoxmlparser.pyt.
-000003a0: 0000 005f 6765 745f 6964 656e 7469 6669  ..._get_identifi
-000003b0: 6572 0c00 0000 730e 0000 0000 0115 0107  er....s.........
-000003c0: 0115 010d 0209 010c 0163 0300 0000 0500  .........c......
-000003d0: 0000 0300 0000 4300 0000 735d 0000 0067  ......C...s]...g
-000003e0: 0000 7d03 0078 3600 7c01 006a 0000 445d  ..}..x6.|..j..D]
-000003f0: 2b00 7d04 007c 0000 6a01 007c 0400 8301  +.}..|..j..|....
-00000400: 007c 0200 6b02 0072 1000 7c03 006a 0200  .|..k..r..|..j..
-00000410: 7c04 0083 0100 0171 1000 7110 0057 7403  |......q..q..Wt.
-00000420: 007c 0300 8301 0064 0100 6b02 0072 5900  .|.....d..k..rY.
-00000430: 7c03 0064 0200 1953 7c03 0053 2803 0000  |..d...S|..S(...
-00000440: 004e 6901 0000 0069 0000 0000 2804 0000  .Ni....i....(...
-00000450: 0074 0800 0000 6368 696c 6472 656e 5213  .t....childrenR.
-00000460: 0000 0074 0600 0000 6170 7065 6e64 7403  ...t....appendt.
-00000470: 0000 006c 656e 2805 0000 0052 1100 0000  ...len(....R....
-00000480: 5212 0000 0074 0500 0000 7175 6572 7974  R....t....queryt
-00000490: 1000 0000 666f 756e 6465 645f 6368 696c  ....founded_chil
-000004a0: 6472 656e 7405 0000 0063 6869 6c64 2800  drent....child(.
-000004b0: 0000 0028 0000 0000 734f 0000 002f 5573  ...(....sO.../Us
-000004c0: 6572 732f 6164 6d69 6e2f 576f 726b 2f70  ers/admin/Work/p
-000004d0: 726f 6a65 6374 2f44 6573 7369 6d6f 7a2f  roject/Dessimoz/
-000004e0: 7079 6861 6d2d 6465 762f 7079 6861 6d2f  pyham-dev/pyham/
-000004f0: 7465 7374 732f 7465 7374 5f6f 7274 686f  tests/test_ortho
-00000500: 786d 6c70 6172 7365 722e 7079 7418 0000  xmlparser.pyt...
-00000510: 005f 6765 745f 6368 696c 645f 6279 5f69  ._get_child_by_i
-00000520: 6465 6e74 6966 6965 7216 0000 0073 0e00  dentifier....s..
-00000530: 0000 0001 0601 1001 1501 1401 1201 0801  ................
-00000540: 6303 0000 0004 0000 0004 0000 0003 0000  c...............
-00000550: 0073 4b00 0000 7400 0074 0100 7c02 0083  .sK...t..t..|...
-00000560: 0100 8301 007d 0200 7400 0074 0100 8700  .....}..t..t....
-00000570: 0066 0100 6401 0086 0000 7c01 006a 0200  .f..d.....|..j..
-00000580: 4483 0100 8301 0083 0100 7d03 0088 0000  D.........}.....
-00000590: 6a03 007c 0200 7c03 0083 0200 0164 0000  j..|..|......d..
-000005a0: 5328 0200 0000 4e63 0100 0000 0200 0000  S(....Nc........
-000005b0: 0300 0000 3300 0000 731e 0000 007c 0000  ....3...s....|..
-000005c0: 5d14 007d 0100 8800 006a 0000 7c01 0083  ]..}.....j..|...
-000005d0: 0100 5601 7103 0064 0000 5328 0100 0000  ..V.q..d..S(....
-000005e0: 4e28 0100 0000 5213 0000 0028 0200 0000  N(....R....(....
-000005f0: 7402 0000 002e 3052 1200 0000 2801 0000  t.....0R....(...
-00000600: 0052 1100 0000 2800 0000 0073 4f00 0000  .R....(....sO...
-00000610: 2f55 7365 7273 2f61 646d 696e 2f57 6f72  /Users/admin/Wor
-00000620: 6b2f 7072 6f6a 6563 742f 4465 7373 696d  k/project/Dessim
-00000630: 6f7a 2f70 7968 616d 2d64 6576 2f70 7968  oz/pyham-dev/pyh
-00000640: 616d 2f74 6573 7473 2f74 6573 745f 6f72  am/tests/test_or
-00000650: 7468 6f78 6d6c 7061 7273 6572 2e70 7973  thoxmlparser.pys
-00000660: 0900 0000 3c67 656e 6578 7072 3e21 0000  ....<genexpr>!..
-00000670: 0073 0200 0000 0600 2804 0000 0074 0600  .s......(....t..
-00000680: 0000 736f 7274 6564 7404 0000 006c 6973  ..sortedt....lis
-00000690: 7452 1400 0000 740b 0000 0061 7373 6572  tR....t....asser
-000006a0: 7445 7175 616c 2804 0000 0052 1100 0000  tEqual(....R....
-000006b0: 7403 0000 0068 6f67 7410 0000 0065 7870  t....hogt....exp
-000006c0: 6563 7465 645f 6d65 6d62 6572 7374 1000  ected_memberst..
-000006d0: 0000 6f62 7365 7276 6564 5f6d 656d 6265  ..observed_membe
-000006e0: 7273 2800 0000 0028 0100 0000 5211 0000  rs(....(....R...
-000006f0: 0073 4f00 0000 2f55 7365 7273 2f61 646d  .sO.../Users/adm
-00000700: 696e 2f57 6f72 6b2f 7072 6f6a 6563 742f  in/Work/project/
-00000710: 4465 7373 696d 6f7a 2f70 7968 616d 2d64  Dessimoz/pyham-d
-00000720: 6576 2f70 7968 616d 2f74 6573 7473 2f74  ev/pyham/tests/t
-00000730: 6573 745f 6f72 7468 6f78 6d6c 7061 7273  est_orthoxmlpars
-00000740: 6572 2e70 7974 1b00 0000 5f63 6865 636b  er.pyt...._check
-00000750: 5f63 6869 6c64 7265 6e5f 636f 6e73 6973  _children_consis
-00000760: 7465 6e63 791f 0000 0073 0600 0000 0001  tency....s......
-00000770: 1201 2501 6301 0000 0004 0000 0009 0000  ..%.c...........
-00000780: 0043 0000 0073 a600 0000 7400 006a 0100  .C...s....t..j..
-00000790: 6a02 0074 0000 6a01 006a 0300 7404 0083  j..t..j..j..t...
-000007a0: 0100 6401 0083 0200 7d01 0074 0500 6a06  ..d.....}..t..j.
-000007b0: 007c 0100 6402 0064 0300 8301 017d 0200  .|..d..d.....}..
-000007c0: 7400 006a 0100 6a02 0074 0000 6a01 006a  t..j..j..t..j..j
-000007d0: 0300 7404 0083 0100 6404 0083 0200 7d03  ..t.....d.....}.
-000007e0: 0074 0700 6a08 0064 0500 7c02 0064 0600  .t..j..d..|..d..
-000007f0: 7c03 0064 0700 6408 0064 0900 7409 0083  |..d..d..d..t...
-00000800: 0004 7c00 005f 0a00 7c00 006a 0a00 6a0b  ..|.._..|..j..j.
-00000810: 0083 0000 7c00 005f 0c00 7c00 006a 0a00  ....|.._..|..j..
-00000820: 6a0d 0083 0000 7c00 005f 0e00 6400 0053  j.....|.._..d..S
-00000830: 280a 0000 004e 7313 0000 002e 2f64 6174  (....Ns...../dat
-00000840: 612f 7369 6d70 6c65 4578 2e6e 776b 5210  a/simpleEx.nwkR.
-00000850: 0000 0074 0300 0000 6e77 6b73 1800 0000  ...t....nwks....
-00000860: 2e2f 6461 7461 2f73 696d 706c 6545 782e  ./data/simpleEx.
-00000870: 6f72 7468 6f78 6d6c 7409 0000 0074 7265  orthoxmlt....tre
-00000880: 655f 6669 6c65 7408 0000 0068 6f67 5f66  e_filet....hog_f
-00000890: 696c 6574 0d00 0000 7479 7065 5f68 6f67  ilet....type_hog
-000008a0: 5f66 696c 6574 0800 0000 6f72 7468 6f78  _filet....orthox
-000008b0: 6d6c 7411 0000 0075 7365 5f69 6e74 6572  mlt....use_inter
-000008c0: 6e61 6c5f 6e61 6d65 280f 0000 0074 0200  nal_name(....t..
-000008d0: 0000 6f73 7404 0000 0070 6174 6874 0400  ..ost....patht..
-000008e0: 0000 6a6f 696e 7407 0000 0064 6972 6e61  ..joint....dirna
-000008f0: 6d65 7408 0000 005f 5f66 696c 655f 5f52  met....__file__R
-00000900: 0200 0000 7411 0000 0067 6574 5f6e 6577  ....t....get_new
-00000910: 6963 6b5f 7374 7269 6e67 5200 0000 0074  ick_stringR....t
-00000920: 0300 0000 4861 6d74 0400 0000 5472 7565  ....Hamt....True
-00000930: 740c 0000 0068 616d 5f61 6e61 6c79 7369  t....ham_analysi
-00000940: 7374 1700 0000 6765 745f 6469 6374 5f74  st....get_dict_t
-00000950: 6f70 5f6c 6576 656c 5f68 6f67 7374 0400  op_level_hogst..
-00000960: 0000 686f 6773 7415 0000 0067 6574 5f64  ..hogst....get_d
-00000970: 6963 745f 6578 7461 6e74 5f67 656e 6573  ict_extant_genes
-00000980: 7405 0000 0067 656e 6573 2804 0000 0052  t....genes(....R
-00000990: 1100 0000 7408 0000 006e 776b 5f70 6174  ....t....nwk_pat
-000009a0: 6874 0700 0000 6e77 6b5f 7374 7274 0d00  ht....nwk_strt..
-000009b0: 0000 6f72 7468 6f78 6d6c 5f70 6174 6828  ..orthoxml_path(
-000009c0: 0000 0000 2800 0000 0073 4f00 0000 2f55  ....(....sO.../U
-000009d0: 7365 7273 2f61 646d 696e 2f57 6f72 6b2f  sers/admin/Work/
-000009e0: 7072 6f6a 6563 742f 4465 7373 696d 6f7a  project/Dessimoz
-000009f0: 2f70 7968 616d 2d64 6576 2f70 7968 616d  /pyham-dev/pyham
-00000a00: 2f74 6573 7473 2f74 6573 745f 6f72 7468  /tests/test_orth
-00000a10: 6f78 6d6c 7061 7273 6572 2e70 7974 0500  oxmlparser.pyt..
-00000a20: 0000 7365 7455 7024 0000 0073 0e00 0000  ..setUp$...s....
-00000a30: 0001 2101 1501 2102 1b01 0c01 1201 6301  ..!...!.......c.
-00000a40: 0000 0004 0000 000d 0000 0043 0000 0073  ...........C...s
-00000a50: 8000 0000 7400 0064 0100 6402 0064 0300  ....t..d..d..d..
-00000a60: 6402 0064 0400 6402 0064 0500 6406 0064  d..d..d..d..d..d
-00000a70: 0700 6408 0064 0900 6406 0083 0006 7d01  ..d..d..d.....}.
-00000a80: 0074 0100 6a02 0074 0300 8301 007d 0200  .t..j..t.....}..
-00000a90: 782d 007c 0000 6a04 006a 0500 8300 0044  x-.|..j..j.....D
-00000aa0: 5d1c 007d 0300 7c02 007c 0300 6a06 006a  ]..}..|..|..j..j
-00000ab0: 0700 6302 0019 640a 0037 033c 714c 0057  ..c...d..7.<qL.W
-00000ac0: 7c00 006a 0800 7c02 007c 0100 8302 0001  |..j..|..|......
-00000ad0: 6400 0053 280b 0000 004e 7405 0000 0048  d..S(....Nt....H
-00000ae0: 554d 414e 6904 0000 0074 0500 0000 5041  UMANi....t....PA
-00000af0: 4e54 5274 0500 0000 4d4f 5553 4574 0500  NTRt....MOUSEt..
-00000b00: 0000 5241 544e 4f69 0200 0000 7405 0000  ..RATNOi....t...
-00000b10: 0043 414e 4641 6903 0000 0074 0500 0000  .CANFAi....t....
-00000b20: 5845 4e54 5269 0100 0000 2809 0000 0074  XENTRi....(....t
-00000b30: 0400 0000 6469 6374 740b 0000 0063 6f6c  ....dictt....col
-00000b40: 6c65 6374 696f 6e73 740b 0000 0064 6566  lectionst....def
-00000b50: 6175 6c74 6469 6374 7403 0000 0069 6e74  aultdictt....int
-00000b60: 5235 0000 0074 0600 0000 7661 6c75 6573  R5...t....values
-00000b70: 5209 0000 0052 0b00 0000 740f 0000 0061  R....R....t....a
-00000b80: 7373 6572 7444 6963 7445 7175 616c 2804  ssertDictEqual(.
-00000b90: 0000 0052 1100 0000 740d 0000 0065 7870  ...R....t....exp
-00000ba0: 6563 7465 645f 636e 7473 740d 0000 006f  ected_cntst....o
-00000bb0: 6273 6572 7665 645f 636e 7473 7401 0000  bserved_cntst...
-00000bc0: 0067 2800 0000 0028 0000 0000 734f 0000  .g(....(....sO..
-00000bd0: 002f 5573 6572 732f 6164 6d69 6e2f 576f  ./Users/admin/Wo
-00000be0: 726b 2f70 726f 6a65 6374 2f44 6573 7369  rk/project/Dessi
-00000bf0: 6d6f 7a2f 7079 6861 6d2d 6465 762f 7079  moz/pyham-dev/py
-00000c00: 6861 6d2f 7465 7374 732f 7465 7374 5f6f  ham/tests/test_o
-00000c10: 7274 686f 786d 6c70 6172 7365 722e 7079  rthoxmlparser.py
-00000c20: 741c 0000 0074 6573 745f 6e75 6d62 6572  t....test_number
-00000c30: 4f66 4765 6e65 7350 6572 5370 6563 6965  OfGenesPerSpecie
-00000c40: 732e 0000 0073 0c00 0000 0001 1e01 0f01  s....s..........
-00000c50: 0f01 1601 1a01 6301 0000 0005 0000 0006  ......c.........
-00000c60: 0000 0043 0000 0073 a500 0000 7c00 006a  ...C...s....|..j
-00000c70: 0000 6a01 0083 0000 7d01 0069 0500 6401  ..j.....}..i..d.
-00000c80: 0064 0200 3664 0300 6404 0036 6405 0064  .d..6d..d..6d..d
-00000c90: 0600 3664 0500 6407 0036 6405 0064 0800  ..6d..d..6d..d..
-00000ca0: 367d 0200 6905 0064 0900 6402 0036 6409  6}..i..d..d..6d.
-00000cb0: 0064 0400 3664 0900 6406 0036 6409 0064  .d..6d..d..6d..d
-00000cc0: 0700 3664 0900 6408 0036 7d03 0078 2d00  ..6d..d..6}..x-.
-00000cd0: 7c01 0044 5d25 007d 0400 7c03 007c 0400  |..D]%.}..|..|..
-00000ce0: 6a02 006a 0300 6302 0019 7404 007c 0400  j..j..c...t..|..
-00000cf0: 6a05 0083 0100 3703 3c71 6800 577c 0000  j.....7.<qh.W|..
-00000d00: 6a06 007c 0200 7c03 0083 0200 0164 0000  j..|..|......d..
-00000d10: 5328 0a00 0000 4e69 0200 0000 740a 0000  S(....Ni....t...
-00000d20: 0056 6572 7465 6272 6174 6169 0300 0000  .Vertebratai....
-00000d30: 7408 0000 004d 616d 6d61 6c69 6169 0400  t....Mammaliai..
-00000d40: 0000 7410 0000 0045 7561 7263 686f 6e74  ..t....Euarchont
-00000d50: 6f67 6c69 7265 7374 0700 0000 526f 6465  oglirest....Rode
-00000d60: 6e74 7374 0800 0000 5072 696d 6174 6573  ntst....Primates
-00000d70: 6900 0000 0028 0700 0000 5231 0000 0074  i....(....R1...t
-00000d80: 1a00 0000 6765 745f 6c69 7374 5f61 6e63  ....get_list_anc
-00000d90: 6573 7472 616c 5f67 656e 6f6d 6573 520a  estral_genomesR.
-00000da0: 0000 0052 0b00 0000 5216 0000 0052 3500  ...R....R....R5.
-00000db0: 0000 5245 0000 0028 0500 0000 5211 0000  ..RE...(....R...
-00000dc0: 0074 0300 0000 6167 7374 1000 0000 6578  .t....agst....ex
-00000dd0: 7065 6374 6564 5f6e 756d 6265 7273 7410  pected_numberst.
-00000de0: 0000 006f 6273 6572 7665 645f 6e75 6d62  ...observed_numb
-00000df0: 6572 7374 0200 0000 6167 2800 0000 0028  erst....ag(....(
-00000e00: 0000 0000 734f 0000 002f 5573 6572 732f  ....sO.../Users/
-00000e10: 6164 6d69 6e2f 576f 726b 2f70 726f 6a65  admin/Work/proje
-00000e20: 6374 2f44 6573 7369 6d6f 7a2f 7079 6861  ct/Dessimoz/pyha
-00000e30: 6d2d 6465 762f 7079 6861 6d2f 7465 7374  m-dev/pyham/test
-00000e40: 732f 7465 7374 5f6f 7274 686f 786d 6c70  s/test_orthoxmlp
-00000e50: 6172 7365 722e 7079 7424 0000 0074 6573  arser.pyt$...tes
-00000e60: 745f 6e75 6d62 6572 5f68 6f67 5f70 6572  t_number_hog_per
-00000e70: 5f61 6e63 6573 7472 616c 5f67 656e 6f6d  _ancestral_genom
-00000e80: 6536 0000 0073 0c00 0000 0001 0f01 2901  e6...s........).
-00000e90: 2901 0d01 2301 6301 0000 0001 0000 0007  )...#.c.........
-00000ea0: 0000 0043 0000 0073 7800 0000 7c00 006a  ...C...sx...|..j
-00000eb0: 0000 7c00 006a 0100 6401 0019 6a02 0064  ..|..j..d...j..d
-00000ec0: 0200 8301 0064 0300 8302 0001 7c00 006a  .....d......|..j
-00000ed0: 0300 7404 0083 0100 8f19 0001 7c00 006a  ..t.........|..j
-00000ee0: 0100 6404 0019 6a02 0064 0200 8301 0001  ..d...j..d......
-00000ef0: 5764 0000 5158 7c00 006a 0300 7404 0083  Wd..QX|..j..t...
-00000f00: 0100 8f19 0001 7c00 006a 0100 6401 0019  ......|..j..d...
-00000f10: 6a02 0064 0500 8301 0001 5764 0000 5158  j..d......Wd..QX
-00000f20: 6400 0053 2806 0000 004e 7401 0000 0031  d..S(....Nt....1
-00000f30: 740b 0000 0063 6f6e 7369 7374 656e 6379  t....consistency
-00000f40: 6901 0000 0074 0100 0000 3274 0800 0000  i....t....2t....
-00000f50: 636f 7665 7261 6765 2805 0000 0052 1e00  coverage(....R..
-00000f60: 0000 5233 0000 0074 0500 0000 7363 6f72  ..R3...t....scor
-00000f70: 6574 0c00 0000 6173 7365 7274 5261 6973  et....assertRais
-00000f80: 6573 7408 0000 004b 6579 4572 726f 7228  est....KeyError(
-00000f90: 0100 0000 5211 0000 0028 0000 0000 2800  ....R....(....(.
-00000fa0: 0000 0073 4f00 0000 2f55 7365 7273 2f61  ...sO.../Users/a
-00000fb0: 646d 696e 2f57 6f72 6b2f 7072 6f6a 6563  dmin/Work/projec
-00000fc0: 742f 4465 7373 696d 6f7a 2f70 7968 616d  t/Dessimoz/pyham
-00000fd0: 2d64 6576 2f70 7968 616d 2f74 6573 7473  -dev/pyham/tests
-00000fe0: 2f74 6573 745f 6f72 7468 6f78 6d6c 7061  /test_orthoxmlpa
-00000ff0: 7273 6572 2e70 7974 1700 0000 7465 7374  rser.pyt....test
-00001000: 5f73 636f 7265 735f 6f6e 5f74 6f70 6c65  _scores_on_tople
-00001010: 7665 6c3e 0000 0073 0a00 0000 0001 2001  vel>...s...... .
-00001020: 1001 1a01 1001 6301 0000 000d 0000 0007  ......c.........
-00001030: 0000 0043 0000 0073 0601 0000 7c00 006a  ...C...s....|..j
-00001040: 0000 6401 0019 7d01 007c 0000 6a00 0064  ..d...}..|..j..d
-00001050: 0200 197d 0200 7c00 006a 0000 6403 0019  ...}..|..j..d...
-00001060: 7d03 0064 0400 6405 0064 0100 6406 0064  }..d..d..d..d..d
-00001070: 0700 6408 0068 0600 7d04 0064 0900 640a  ..d..h..}..d..d.
-00001080: 0064 0200 640b 0068 0400 7d05 0064 0300  .d..d..h..}..d..
-00001090: 640c 0064 0d00 640e 0064 0f00 6410 0064  d..d..d..d..d..d
-000010a0: 1100 6807 007d 0600 7c01 006a 0100 8300  ..h..}..|..j....
-000010b0: 007d 0700 7c02 006a 0100 8300 007d 0800  .}..|..j.....}..
-000010c0: 7c03 006a 0100 8300 007d 0900 7402 0064  |..j.....}..t..d
-000010d0: 1200 8400 007c 0700 4483 0100 8301 007d  .....|..D......}
-000010e0: 0a00 7402 0064 1300 8400 007c 0800 4483  ..t..d.....|..D.
-000010f0: 0100 8301 007d 0b00 7402 0064 1400 8400  .....}..t..d....
-00001100: 007c 0900 4483 0100 8301 007d 0c00 7c00  .|..D......}..|.
-00001110: 006a 0300 7c04 007c 0a00 8302 0001 7c00  .j..|..|......|.
-00001120: 006a 0300 7c05 007c 0b00 8302 0001 7c00  .j..|..|......|.
-00001130: 006a 0300 7c06 007c 0c00 8302 0001 6400  .j..|..|......d.
-00001140: 0053 2815 0000 004e 5255 0000 0052 5700  .S(....NRU...RW.
-00001150: 0000 7401 0000 0033 7402 0000 0035 3174  ..t....3t....51t
-00001160: 0200 0000 3231 7402 0000 0031 3174 0200  ....21t....11t..
-00001170: 0000 3331 7402 0000 0034 3174 0200 0000  ..31t....41t....
-00001180: 3232 7402 0000 0033 3274 0200 0000 3132  22t....32t....12
-00001190: 7402 0000 0031 3374 0200 0000 3233 7402  t....13t....23t.
-000011a0: 0000 0033 3374 0200 0000 3533 7402 0000  ...33t....53t...
-000011b0: 0031 3474 0200 0000 3334 6301 0000 0002  .14t....34c.....
-000011c0: 0000 0002 0000 0073 0000 0073 1800 0000  .......s...s....
-000011d0: 7c00 005d 0e00 7d01 007c 0100 6a00 0056  |..]..}..|..j..V
-000011e0: 0171 0300 6400 0053 2801 0000 004e 2801  .q..d..S(....N(.
-000011f0: 0000 0052 0700 0000 2802 0000 0052 1b00  ...R....(....R..
-00001200: 0000 7401 0000 0078 2800 0000 0028 0000  ..t....x(....(..
-00001210: 0000 734f 0000 002f 5573 6572 732f 6164  ..sO.../Users/ad
-00001220: 6d69 6e2f 576f 726b 2f70 726f 6a65 6374  min/Work/project
-00001230: 2f44 6573 7369 6d6f 7a2f 7079 6861 6d2d  /Dessimoz/pyham-
-00001240: 6465 762f 7079 6861 6d2f 7465 7374 732f  dev/pyham/tests/
-00001250: 7465 7374 5f6f 7274 686f 786d 6c70 6172  test_orthoxmlpar
-00001260: 7365 722e 7079 7309 0000 003c 6765 6e65  ser.pys....<gene
-00001270: 7870 723e 5300 0000 7302 0000 0006 0063  xpr>S...s......c
-00001280: 0100 0000 0200 0000 0200 0000 7300 0000  ............s...
-00001290: 7318 0000 007c 0000 5d0e 007d 0100 7c01  s....|..]..}..|.
-000012a0: 006a 0000 5601 7103 0064 0000 5328 0100  .j..V.q..d..S(..
-000012b0: 0000 4e28 0100 0000 5207 0000 0028 0200  ..N(....R....(..
-000012c0: 0000 521b 0000 0052 6c00 0000 2800 0000  ..R....Rl...(...
-000012d0: 0028 0000 0000 734f 0000 002f 5573 6572  .(....sO.../User
-000012e0: 732f 6164 6d69 6e2f 576f 726b 2f70 726f  s/admin/Work/pro
-000012f0: 6a65 6374 2f44 6573 7369 6d6f 7a2f 7079  ject/Dessimoz/py
-00001300: 6861 6d2d 6465 762f 7079 6861 6d2f 7465  ham-dev/pyham/te
-00001310: 7374 732f 7465 7374 5f6f 7274 686f 786d  sts/test_orthoxm
-00001320: 6c70 6172 7365 722e 7079 7309 0000 003c  lparser.pys....<
-00001330: 6765 6e65 7870 723e 5400 0000 7302 0000  genexpr>T...s...
-00001340: 0006 0063 0100 0000 0200 0000 0200 0000  ...c............
-00001350: 7300 0000 7318 0000 007c 0000 5d0e 007d  s...s....|..]..}
-00001360: 0100 7c01 006a 0000 5601 7103 0064 0000  ..|..j..V.q..d..
-00001370: 5328 0100 0000 4e28 0100 0000 5207 0000  S(....N(....R...
-00001380: 0028 0200 0000 521b 0000 0052 6c00 0000  .(....R....Rl...
-00001390: 2800 0000 0028 0000 0000 734f 0000 002f  (....(....sO.../
-000013a0: 5573 6572 732f 6164 6d69 6e2f 576f 726b  Users/admin/Work
-000013b0: 2f70 726f 6a65 6374 2f44 6573 7369 6d6f  /project/Dessimo
-000013c0: 7a2f 7079 6861 6d2d 6465 762f 7079 6861  z/pyham-dev/pyha
-000013d0: 6d2f 7465 7374 732f 7465 7374 5f6f 7274  m/tests/test_ort
-000013e0: 686f 786d 6c70 6172 7365 722e 7079 7309  hoxmlparser.pys.
-000013f0: 0000 003c 6765 6e65 7870 723e 5500 0000  ...<genexpr>U...
-00001400: 7302 0000 0006 0028 0400 0000 5233 0000  s......(....R3..
-00001410: 0074 1800 0000 6765 745f 616c 6c5f 6465  .t....get_all_de
-00001420: 7363 656e 6461 6e74 5f67 656e 6573 7403  scendant_genest.
-00001430: 0000 0073 6574 740e 0000 0061 7373 6572  ...sett....asser
-00001440: 7453 6574 4571 7561 6c28 0d00 0000 5211  tSetEqual(....R.
-00001450: 0000 0074 0400 0000 686f 6731 7404 0000  ...t....hog1t...
-00001460: 0068 6f67 3274 0400 0000 686f 6733 7411  .hog2t....hog3t.
-00001470: 0000 0065 7870 6563 7465 644d 656d 6265  ...expectedMembe
-00001480: 7273 5f31 7411 0000 0065 7870 6563 7465  rs_1t....expecte
-00001490: 644d 656d 6265 7273 5f32 7411 0000 0065  dMembers_2t....e
-000014a0: 7870 6563 7465 644d 656d 6265 7273 5f33  xpectedMembers_3
-000014b0: 740a 0000 0068 6f67 315f 6765 6e65 7374  t....hog1_genest
-000014c0: 0a00 0000 686f 6732 5f67 656e 6573 740a  ....hog2_genest.
-000014d0: 0000 0068 6f67 335f 6765 6e65 7374 0900  ...hog3_genest..
-000014e0: 0000 6d65 6d62 6572 735f 3174 0900 0000  ..members_1t....
-000014f0: 6d65 6d62 6572 735f 3274 0900 0000 6d65  members_2t....me
-00001500: 6d62 6572 735f 3328 0000 0000 2800 0000  mbers_3(....(...
-00001510: 0073 4f00 0000 2f55 7365 7273 2f61 646d  .sO.../Users/adm
-00001520: 696e 2f57 6f72 6b2f 7072 6f6a 6563 742f  in/Work/project/
-00001530: 4465 7373 696d 6f7a 2f70 7968 616d 2d64  Dessimoz/pyham-d
-00001540: 6576 2f70 7968 616d 2f74 6573 7473 2f74  ev/pyham/tests/t
-00001550: 6573 745f 6f72 7468 6f78 6d6c 7061 7273  est_orthoxmlpars
-00001560: 6572 2e70 7974 1300 0000 7465 7374 5f68  er.pyt....test_h
-00001570: 6f67 5f6d 656d 6265 7273 6869 7045 0000  og_membershipE..
-00001580: 0073 1e00 0000 0002 0d01 0d01 0d02 1801  .s..............
-00001590: 1201 1b02 0c01 0c01 0c02 1601 1601 1602  ................
-000015a0: 1001 1001 6301 0000 0006 0000 0004 0000  ....c...........
-000015b0: 0043 0000 0073 e000 0000 7c00 006a 0000  .C...s....|..j..
-000015c0: 6401 0019 7d01 007c 0000 6a01 0064 0200  d...}..|..j..d..
-000015d0: 7c01 006a 0200 6a03 006a 0400 8302 0001  |..j..j..j......
-000015e0: 7c00 006a 0500 7c01 0064 0300 6404 0067  |..j..|..d..d..g
-000015f0: 0200 8302 0001 7c00 006a 0600 7c01 0064  ......|..j..|..d
-00001600: 0400 8302 007d 0200 7c00 006a 0500 7c02  .....}..|..j..|.
-00001610: 0064 0500 6406 0067 0200 8302 0001 7c00  .d..d..g......|.
-00001620: 006a 0600 7c02 0064 0600 8302 007d 0300  .j..|..d.....}..
-00001630: 7c00 006a 0500 7c03 0064 0700 6408 0067  |..j..|..d..d..g
-00001640: 0200 8302 0001 7c00 006a 0600 7c03 0064  ......|..j..|..d
-00001650: 0700 8302 007d 0400 7c00 006a 0500 7c04  .....}..|..j..|.
-00001660: 0064 0900 640a 0067 0200 8302 0001 7c00  .d..d..g......|.
-00001670: 006a 0600 7c03 0064 0800 8302 007d 0500  .j..|..d.....}..
-00001680: 7c00 006a 0500 7c05 0064 0100 640b 0067  |..j..|..d..d..g
-00001690: 0200 8302 0001 6400 0053 280c 0000 004e  ......d..S(....N
-000016a0: 5255 0000 0052 4a00 0000 525e 0000 0052  RU...RJ...R^...R
-000016b0: 4b00 0000 525f 0000 0052 4c00 0000 524d  K...R_...RL...RM
-000016c0: 0000 0052 4e00 0000 5262 0000 0052 6100  ...RN...Rb...Ra.
-000016d0: 0000 5260 0000 0028 0700 0000 5233 0000  ..R`...(....R3..
-000016e0: 0052 1e00 0000 5209 0000 0052 0a00 0000  .R....R....R....
-000016f0: 520b 0000 0052 2200 0000 521a 0000 0028  R....R"...R....(
-00001700: 0600 0000 5211 0000 0052 7000 0000 7408  ....R....Rp...t.
-00001710: 0000 006d 616d 6d61 6c69 6174 1000 0000  ...mammaliat....
-00001720: 6575 6172 6368 6f6e 746f 676c 6972 6573  euarchontoglires
-00001730: 7407 0000 0072 6f64 656e 7473 7408 0000  t....rodentst...
-00001740: 0070 7269 6d61 7465 7328 0000 0000 2800  .primates(....(.
-00001750: 0000 0073 4f00 0000 2f55 7365 7273 2f61  ...sO.../Users/a
-00001760: 646d 696e 2f57 6f72 6b2f 7072 6f6a 6563  dmin/Work/projec
-00001770: 742f 4465 7373 696d 6f7a 2f70 7968 616d  t/Dessimoz/pyham
-00001780: 2d64 6576 2f70 7968 616d 2f74 6573 7473  -dev/pyham/tests
-00001790: 2f74 6573 745f 6f72 7468 6f78 6d6c 7061  /test_orthoxmlpa
-000017a0: 7273 6572 2e70 7974 1900 0000 7465 7374  rser.pyt....test
-000017b0: 5f73 696d 706c 655f 686f 675f 7374 7275  _simple_hog_stru
-000017c0: 6374 7572 655b 0000 0073 1600 0000 0002  cture[...s......
-000017d0: 0d03 1901 1603 1201 1603 1201 1603 1201  ................
-000017e0: 1603 1201 6301 0000 0005 0000 0004 0000  ....c...........
-000017f0: 0043 0000 0073 b500 0000 7c00 006a 0000  .C...s....|..j..
-00001800: 6401 0019 7d01 007c 0000 6a01 0064 0200  d...}..|..j..d..
-00001810: 7c01 006a 0200 6a03 006a 0400 8302 0001  |..j..j..j......
-00001820: 7c00 006a 0500 7c01 0064 0300 6404 0067  |..j..|..d..d..g
-00001830: 0200 8302 0001 7c00 006a 0600 7c01 0064  ......|..j..|..d
-00001840: 0400 8302 007d 0200 7c00 006a 0500 7c02  .....}..|..j..|.
-00001850: 0064 0500 6406 0067 0200 8302 0001 7c00  .d..d..g......|.
-00001860: 006a 0600 7c02 0064 0600 8302 007d 0300  .j..|..d.....}..
-00001870: 7c00 006a 0500 7c03 0064 0100 6407 0067  |..j..|..d..d..g
-00001880: 0200 8302 0001 7c00 006a 0600 7c02 0064  ......|..j..|..d
-00001890: 0500 8302 007d 0400 7c00 006a 0500 7c04  .....}..|..j..|.
-000018a0: 0064 0800 6801 0083 0200 0164 0000 5328  .d..h......d..S(
-000018b0: 0900 0000 4e52 5700 0000 524b 0000 0052  ....NRW...RK...R
-000018c0: 6300 0000 524c 0000 0052 4d00 0000 524e  c...RL...RM...RN
-000018d0: 0000 0052 6500 0000 5264 0000 0028 0700  ...Re...Rd...(..
-000018e0: 0000 5233 0000 0052 1e00 0000 5209 0000  ..R3...R....R...
-000018f0: 0052 0a00 0000 520b 0000 0052 2200 0000  .R....R....R"...
-00001900: 521a 0000 0028 0500 0000 5211 0000 0052  R....(....R....R
-00001910: 7100 0000 527e 0000 0052 8000 0000 527f  q...R~...R....R.
-00001920: 0000 0028 0000 0000 2800 0000 0073 4f00  ...(....(....sO.
-00001930: 0000 2f55 7365 7273 2f61 646d 696e 2f57  ../Users/admin/W
-00001940: 6f72 6b2f 7072 6f6a 6563 742f 4465 7373  ork/project/Dess
-00001950: 696d 6f7a 2f70 7968 616d 2d64 6576 2f70  imoz/pyham-dev/p
-00001960: 7968 616d 2f74 6573 7473 2f74 6573 745f  yham/tests/test_
-00001970: 6f72 7468 6f78 6d6c 7061 7273 6572 2e70  orthoxmlparser.p
-00001980: 7974 2700 0000 7465 7374 5f69 6e63 6f6d  yt'...test_incom
-00001990: 706c 6574 655f 6c69 6e65 6167 655f 7461  plete_lineage_ta
-000019a0: 786f 6e5f 6578 7061 6e73 696f 6e73 0000  xon_expansions..
-000019b0: 0073 1200 0000 0002 0d03 1901 1603 1201  .s..............
-000019c0: 1603 1201 1603 1201 6301 0000 0007 0000  ........c.......
-000019d0: 0005 0000 0043 0000 0073 7f01 0000 7c00  .....C...s....|.
-000019e0: 006a 0000 6401 0019 7d01 007c 0000 6a01  .j..d...}..|..j.
-000019f0: 0064 0200 7c01 006a 0200 6a03 006a 0400  .d..|..j..j..j..
-00001a00: 8302 0001 7c00 006a 0500 7c01 0064 0300  ....|..j..|..d..
-00001a10: 6404 0067 0200 8302 0001 7c00 006a 0600  d..g......|..j..
-00001a20: 7c01 006a 0700 8301 0001 7c00 006a 0800  |..j......|..j..
-00001a30: 7c01 0064 0400 8302 007d 0200 7c00 006a  |..d.....}..|..j
-00001a40: 0500 7c02 0064 0500 6406 0064 0600 6703  ..|..d..d..d..g.
-00001a50: 0083 0200 017c 0000 6a06 007c 0200 6a07  .....|..j..|..j.
-00001a60: 0083 0100 017c 0000 6a08 007c 0200 6406  .....|..j..|..d.
-00001a70: 0083 0200 7d03 0078 df00 7c03 0044 5dd7  ....}..x..|..D].
-00001a80: 007d 0400 7c00 006a 0900 7c04 006a 0700  .}..|..j..|..j..
-00001a90: 8301 0001 7c00 006a 0500 7c04 0064 0700  ....|..j..|..d..
-00001aa0: 6408 0067 0200 8302 0001 7c00 006a 0800  d..g......|..j..
-00001ab0: 7c04 0064 0700 8302 007d 0500 7c00 006a  |..d.....}..|..j
-00001ac0: 0600 7c05 006a 0700 8301 0001 7c00 006a  ..|..j......|..j
-00001ad0: 0800 7c04 0064 0800 8302 007d 0600 7c00  ..|..d.....}..|.
-00001ae0: 006a 0600 7c06 006a 0700 8301 0001 740a  .j..|..j......t.
-00001af0: 007c 0500 6a0b 0083 0100 6409 006b 0200  .|..j.....d..k..
-00001b00: 7251 017c 0000 6a05 007c 0600 640a 0067  rQ.|..j..|..d..g
-00001b10: 0100 8302 0001 7c00 006a 0500 7c05 0064  ......|..j..|..d
-00001b20: 0100 640b 0067 0200 8302 0001 71a0 007c  ..d..g......q..|
-00001b30: 0000 6a05 007c 0600 640c 0067 0100 8302  ..j..|..d..g....
-00001b40: 0001 7c00 006a 0500 7c05 0064 0d00 6701  ..|..j..|..d..g.
-00001b50: 0083 0200 0171 a000 5764 0000 5328 0e00  .....q..Wd..S(..
-00001b60: 0000 4e52 5d00 0000 524a 0000 0052 6900  ..NR]...RJ...Ri.
-00001b70: 0000 524b 0000 0052 6700 0000 524c 0000  ..RK...Rg...RL..
-00001b80: 0052 4e00 0000 524d 0000 0069 0200 0000  .RN...RM...i....
-00001b90: 5268 0000 0052 6600 0000 526b 0000 0052  Rh...Rf...Rk...R
-00001ba0: 6a00 0000 280c 0000 0052 3300 0000 521e  j...(....R3...R.
-00001bb0: 0000 0052 0900 0000 520a 0000 0052 0b00  ...R....R....R..
-00001bc0: 0000 5222 0000 0074 0b00 0000 6173 7365  ..R"...t....asse
-00001bd0: 7274 4661 6c73 6574 1400 0000 6172 6f73  rtFalset....aros
-00001be0: 655f 6279 5f64 7570 6c69 6361 7469 6f6e  e_by_duplication
-00001bf0: 521a 0000 0074 0a00 0000 6173 7365 7274  R....t....assert
-00001c00: 5472 7565 5216 0000 0052 1400 0000 2807  TrueR....R....(.
-00001c10: 0000 0052 1100 0000 5272 0000 0052 7d00  ...R....Rr...R}.
-00001c20: 0000 527e 0000 0074 0f00 0000 6575 6172  ..R~...t....euar
-00001c30: 6368 6f6e 746f 676c 6972 6552 8000 0000  chontoglireR....
-00001c40: 527f 0000 0028 0000 0000 2800 0000 0073  R....(....(....s
-00001c50: 4f00 0000 2f55 7365 7273 2f61 646d 696e  O.../Users/admin
-00001c60: 2f57 6f72 6b2f 7072 6f6a 6563 742f 4465  /Work/project/De
-00001c70: 7373 696d 6f7a 2f70 7968 616d 2d64 6576  ssimoz/pyham-dev
-00001c80: 2f70 7968 616d 2f74 6573 7473 2f74 6573  /pyham/tests/tes
-00001c90: 745f 6f72 7468 6f78 6d6c 7061 7273 6572  t_orthoxmlparser
-00001ca0: 2e70 7974 1900 0000 7465 7374 5f68 6f67  .pyt....test_hog
-00001cb0: 5f77 6974 685f 6475 706c 6963 6174 696f  _with_duplicatio
-00001cc0: 6e87 0000 0073 2800 0000 0002 0d03 1901  n....s(.........
-00001cd0: 1601 1003 1201 1901 1003 1201 0d01 1001  ................
-00001ce0: 1603 1201 1001 1201 1002 1501 1301 1902  ................
-00001cf0: 1301 280d 0000 0052 0f00 0000 740a 0000  ..(....R....t...
-00001d00: 005f 5f6d 6f64 756c 655f 5f52 1300 0000  .__module__R....
-00001d10: 521a 0000 0052 2200 0000 5239 0000 0052  R....R"...R9...R
-00001d20: 4900 0000 5254 0000 0052 5c00 0000 527c  I...RT...R\...R|
-00001d30: 0000 0052 8100 0000 5282 0000 0052 8700  ...R....R....R..
-00001d40: 0000 2800 0000 0028 0000 0000 2800 0000  ..(....(....(...
-00001d50: 0073 4f00 0000 2f55 7365 7273 2f61 646d  .sO.../Users/adm
-00001d60: 696e 2f57 6f72 6b2f 7072 6f6a 6563 742f  in/Work/project/
-00001d70: 4465 7373 696d 6f7a 2f70 7968 616d 2d64  Dessimoz/pyham-d
-00001d80: 6576 2f70 7968 616d 2f74 6573 7473 2f74  ev/pyham/tests/t
-00001d90: 6573 745f 6f72 7468 6f78 6d6c 7061 7273  est_orthoxmlpars
-00001da0: 6572 2e70 7952 0400 0000 0b00 0000 7316  er.pyR........s.
-00001db0: 0000 0006 0109 0a09 0909 0509 0a09 0809  ................
-00001dc0: 0809 0709 1609 1809 1474 2200 0000 4f72  .........t"...Or
-00001dd0: 7468 6f58 4d4c 5061 7273 6572 5465 7374  thoXMLParserTest
-00001de0: 5f63 6f6d 706c 6578 5061 7261 6c6f 6773  _complexParalogs
-00001df0: 6300 0000 0000 0000 0001 0000 0042 0000  c............B..
-00001e00: 0073 9800 0000 6500 005a 0100 6400 0084  .s....e..Z..d...
-00001e10: 0000 5a02 0064 0100 8400 005a 0300 6402  ..Z..d.....Z..d.
-00001e20: 0084 0000 5a04 0064 0300 8400 005a 0500  ....Z..d.....Z..
-00001e30: 6404 0084 0000 5a06 0064 0500 8400 005a  d.....Z..d.....Z
-00001e40: 0700 6406 0084 0000 5a08 0064 0700 8400  ..d.....Z..d....
-00001e50: 005a 0900 6408 0084 0000 5a0a 0064 0900  .Z..d.....Z..d..
-00001e60: 8400 005a 0b00 640a 0084 0000 5a0c 0064  ...Z..d.....Z..d
-00001e70: 0b00 8400 005a 0d00 640c 0084 0000 5a0e  .....Z..d.....Z.
-00001e80: 0064 0d00 8400 005a 0f00 640e 0084 0000  .d.....Z..d.....
-00001e90: 5a10 0064 0f00 8400 005a 1100 5253 2810  Z..d.....Z..RS(.
-00001ea0: 0000 0063 0200 0000 0200 0000 0500 0000  ...c............
-00001eb0: 4300 0000 736c 0000 0074 0000 7c01 0074  C...sl...t..|..t
-00001ec0: 0100 6a02 006a 0300 8302 0072 1c00 7c01  ..j..j.....r..|.
-00001ed0: 006a 0400 5374 0000 7c01 0074 0100 6a02  .j..St..|..t..j.
-00001ee0: 006a 0500 8302 0072 3e00 7c01 006a 0600  .j.....r>.|..j..
-00001ef0: 6a07 006a 0800 5374 0900 6401 006a 0a00  j..j..St..d..j..
-00001f00: 7401 006a 0200 6a0b 006a 0c00 740d 007c  t..j..j..j..t..|
-00001f10: 0100 8301 006a 0c00 8302 0083 0100 8201  .....j..........
-00001f20: 0064 0000 5328 0200 0000 4e73 2300 0000  .d..S(....Ns#...
-00001f30: 6578 7065 6374 2073 7562 636c 6173 7320  expect subclass 
-00001f40: 6f62 6a20 6f66 2027 7b7d 272c 2067 6f74  obj of '{}', got
-00001f50: 207b 7d28 0e00 0000 5205 0000 0052 0000   {}(....R....R..
-00001f60: 0000 5201 0000 0052 0600 0000 5207 0000  ..R....R....R...
-00001f70: 0052 0800 0000 5209 0000 0052 0a00 0000  .R....R....R....
-00001f80: 520b 0000 0052 0c00 0000 520d 0000 0052  R....R....R....R
-00001f90: 0e00 0000 520f 0000 0052 1000 0000 2802  ....R....R....(.
-00001fa0: 0000 0052 1100 0000 5212 0000 0028 0000  ...R....R....(..
-00001fb0: 0000 2800 0000 0073 4f00 0000 2f55 7365  ..(....sO.../Use
-00001fc0: 7273 2f61 646d 696e 2f57 6f72 6b2f 7072  rs/admin/Work/pr
-00001fd0: 6f6a 6563 742f 4465 7373 696d 6f7a 2f70  oject/Dessimoz/p
-00001fe0: 7968 616d 2d64 6576 2f70 7968 616d 2f74  yham-dev/pyham/t
-00001ff0: 6573 7473 2f74 6573 745f 6f72 7468 6f78  ests/test_orthox
-00002000: 6d6c 7061 7273 6572 2e70 7952 1300 0000  mlparser.pyR....
-00002010: aa00 0000 730e 0000 0000 0115 0107 0115  ....s...........
-00002020: 010d 0209 010c 0163 0300 0000 0500 0000  .......c........
-00002030: 0300 0000 4300 0000 735d 0000 0067 0000  ....C...s]...g..
-00002040: 7d03 0078 3600 7c01 006a 0000 445d 2b00  }..x6.|..j..D]+.
-00002050: 7d04 007c 0000 6a01 007c 0400 8301 007c  }..|..j..|.....|
-00002060: 0200 6b02 0072 1000 7c03 006a 0200 7c04  ..k..r..|..j..|.
-00002070: 0083 0100 0171 1000 7110 0057 7403 007c  .....q..q..Wt..|
-00002080: 0300 8301 0064 0100 6b02 0072 5900 7c03  .....d..k..rY.|.
-00002090: 0064 0200 1953 7c03 0053 2803 0000 004e  .d...S|..S(....N
-000020a0: 6901 0000 0069 0000 0000 2804 0000 0052  i....i....(....R
-000020b0: 1400 0000 5213 0000 0052 1500 0000 5216  ....R....R....R.
-000020c0: 0000 0028 0500 0000 5211 0000 0052 1200  ...(....R....R..
-000020d0: 0000 5217 0000 0052 1800 0000 5219 0000  ..R....R....R...
-000020e0: 0028 0000 0000 2800 0000 0073 4f00 0000  .(....(....sO...
-000020f0: 2f55 7365 7273 2f61 646d 696e 2f57 6f72  /Users/admin/Wor
-00002100: 6b2f 7072 6f6a 6563 742f 4465 7373 696d  k/project/Dessim
-00002110: 6f7a 2f70 7968 616d 2d64 6576 2f70 7968  oz/pyham-dev/pyh
-00002120: 616d 2f74 6573 7473 2f74 6573 745f 6f72  am/tests/test_or
-00002130: 7468 6f78 6d6c 7061 7273 6572 2e70 7952  thoxmlparser.pyR
-00002140: 1a00 0000 b400 0000 730e 0000 0000 0106  ........s.......
-00002150: 0110 0115 0114 0112 0108 0163 0300 0000  ...........c....
-00002160: 0400 0000 0400 0000 0300 0000 734b 0000  ............sK..
-00002170: 0074 0000 7401 007c 0200 8301 0083 0100  .t..t..|........
-00002180: 7d02 0074 0000 7401 0087 0000 6601 0064  }..t..t.....f..d
-00002190: 0100 8600 007c 0100 6a02 0044 8301 0083  .....|..j..D....
-000021a0: 0100 8301 007d 0300 8800 006a 0300 7c02  .....}.....j..|.
-000021b0: 007c 0300 8302 0001 6400 0053 2802 0000  .|......d..S(...
-000021c0: 004e 6301 0000 0002 0000 0003 0000 0033  .Nc............3
-000021d0: 0000 0073 1e00 0000 7c00 005d 1400 7d01  ...s....|..]..}.
-000021e0: 0088 0000 6a00 007c 0100 8301 0056 0171  ....j..|.....V.q
-000021f0: 0300 6400 0053 2801 0000 004e 2801 0000  ..d..S(....N(...
-00002200: 0052 1300 0000 2802 0000 0052 1b00 0000  .R....(....R....
-00002210: 5212 0000 0028 0100 0000 5211 0000 0028  R....(....R....(
-00002220: 0000 0000 734f 0000 002f 5573 6572 732f  ....sO.../Users/
-00002230: 6164 6d69 6e2f 576f 726b 2f70 726f 6a65  admin/Work/proje
-00002240: 6374 2f44 6573 7369 6d6f 7a2f 7079 6861  ct/Dessimoz/pyha
-00002250: 6d2d 6465 762f 7079 6861 6d2f 7465 7374  m-dev/pyham/test
-00002260: 732f 7465 7374 5f6f 7274 686f 786d 6c70  s/test_orthoxmlp
-00002270: 6172 7365 722e 7079 7309 0000 003c 6765  arser.pys....<ge
-00002280: 6e65 7870 723e bf00 0000 7302 0000 0006  nexpr>....s.....
-00002290: 0028 0400 0000 521c 0000 0052 1d00 0000  .(....R....R....
-000022a0: 5214 0000 0052 1e00 0000 2804 0000 0052  R....R....(....R
-000022b0: 1100 0000 521f 0000 0052 2000 0000 5221  ....R....R ...R!
-000022c0: 0000 0028 0000 0000 2801 0000 0052 1100  ...(....(....R..
-000022d0: 0000 734f 0000 002f 5573 6572 732f 6164  ..sO.../Users/ad
-000022e0: 6d69 6e2f 576f 726b 2f70 726f 6a65 6374  min/Work/project
-000022f0: 2f44 6573 7369 6d6f 7a2f 7079 6861 6d2d  /Dessimoz/pyham-
-00002300: 6465 762f 7079 6861 6d2f 7465 7374 732f  dev/pyham/tests/
-00002310: 7465 7374 5f6f 7274 686f 786d 6c70 6172  test_orthoxmlpar
-00002320: 7365 722e 7079 5222 0000 00bd 0000 0073  ser.pyR".......s
-00002330: 0600 0000 0001 1201 2501 6301 0000 0005  ........%.c.....
-00002340: 0000 0009 0000 0043 0000 0073 1201 0000  .......C...s....
-00002350: 7400 006a 0100 6a02 0074 0000 6a01 006a  t..j..j..t..j..j
-00002360: 0300 7404 0083 0100 6401 0083 0200 7d01  ..t.....d.....}.
-00002370: 0074 0500 6a06 007c 0100 6402 0064 0300  .t..j..|..d..d..
-00002380: 8301 017d 0200 7400 006a 0100 6a02 0074  ...}..t..j..j..t
-00002390: 0000 6a01 006a 0300 7404 0083 0100 6404  ..j..j..t.....d.
-000023a0: 0083 0200 7d03 0074 0000 6a01 006a 0200  ....}..t..j..j..
-000023b0: 7400 006a 0100 6a03 0074 0400 8301 0064  t..j..j..t.....d
-000023c0: 0500 8302 007d 0400 7407 006a 0800 6406  .....}..t..j..d.
-000023d0: 007c 0200 6407 007c 0300 6408 0064 0900  .|..d..|..d..d..
-000023e0: 640a 0074 0900 8300 047c 0000 5f0a 007c  d..t.....|.._..|
-000023f0: 0000 6a0a 006a 0b00 8300 007c 0000 5f0c  ..j..j.....|.._.
-00002400: 007c 0000 6a0a 006a 0d00 8300 007c 0000  .|..j..j.....|..
-00002410: 5f0e 0074 0700 6a08 0064 0600 7c02 0064  _..t..j..d..|..d
-00002420: 0700 7c04 0064 0800 6409 0064 0a00 7409  ..|..d..d..d..t.
-00002430: 0083 0004 7c00 005f 0f00 7c00 006a 0f00  ....|.._..|..j..
-00002440: 6a0b 0083 0000 7c00 005f 1000 7c00 006a  j.....|.._..|..j
-00002450: 0f00 6a0d 0083 0000 7c00 005f 1100 6400  ..j.....|.._..d.
-00002460: 0053 280b 0000 004e 7313 0000 002e 2f64  .S(....Ns...../d
-00002470: 6174 612f 7369 6d70 6c65 4578 2e6e 776b  ata/simpleEx.nwk
-00002480: 5210 0000 0052 2300 0000 7328 0000 002e  R....R#...s(....
-00002490: 2f64 6174 612f 7369 6d70 6c65 4578 5f63  /data/simpleEx_c
-000024a0: 6f6d 706c 6578 5061 7261 6c6f 6773 2e6f  omplexParalogs.o
-000024b0: 7274 686f 786d 6c73 3000 0000 2e2f 6461  rthoxmls0..../da
-000024c0: 7461 2f53 696d 706c 6545 785f 636f 6d70  ta/SimpleEx_comp
-000024d0: 6c65 7850 6172 616c 6f67 4765 7448 4f47  lexParalogGetHOG
-000024e0: 5333 666f 726d 6174 2e78 6d6c 5224 0000  S3format.xmlR$..
-000024f0: 0052 2500 0000 5226 0000 0052 2700 0000  .R%...R&...R'...
-00002500: 5228 0000 0028 1200 0000 5229 0000 0052  R(...(....R)...R
-00002510: 2a00 0000 522b 0000 0052 2c00 0000 522d  *...R+...R,...R-
-00002520: 0000 0052 0200 0000 522e 0000 0052 0000  ...R....R....R..
-00002530: 0000 522f 0000 0052 3000 0000 5231 0000  ..R/...R0...R1..
-00002540: 0052 3200 0000 5233 0000 0052 3400 0000  .R2...R3...R4...
-00002550: 5235 0000 0074 0f00 0000 6861 6d5f 616e  R5...t....ham_an
-00002560: 616c 7973 6973 5f76 3374 0700 0000 686f  alysis_v3t....ho
-00002570: 6773 5f76 3374 0800 0000 6765 6e65 735f  gs_v3t....genes_
-00002580: 7633 2805 0000 0052 1100 0000 5236 0000  v3(....R....R6..
-00002590: 0052 3700 0000 5238 0000 0074 1000 0000  .R7...R8...t....
-000025a0: 6f72 7468 6f78 6d6c 5f70 6174 685f 7633  orthoxml_path_v3
-000025b0: 2800 0000 0028 0000 0000 734f 0000 002f  (....(....sO.../
-000025c0: 5573 6572 732f 6164 6d69 6e2f 576f 726b  Users/admin/Work
-000025d0: 2f70 726f 6a65 6374 2f44 6573 7369 6d6f  /project/Dessimo
-000025e0: 7a2f 7079 6861 6d2d 6465 762f 7079 6861  z/pyham-dev/pyha
-000025f0: 6d2f 7465 7374 732f 7465 7374 5f6f 7274  m/tests/test_ort
-00002600: 686f 786d 6c70 6172 7365 722e 7079 5239  hoxmlparser.pyR9
-00002610: 0000 00c2 0000 0073 1800 0000 0001 2101  .......s......!.
-00002620: 1501 2101 2102 1b01 0c01 1201 1202 1b01  ..!.!...........
-00002630: 0c01 1201 6301 0000 0004 0000 0003 0000  ....c...........
-00002640: 0043 0000 0073 5000 0000 6401 0064 0200  .C...sP...d..d..
-00002650: 6c00 006d 0100 7d01 0001 7c01 007c 0000  l..m..}...|..|..
-00002660: 6a02 0083 0100 7d02 0078 2a00 7c00 006a  j.....}..x*.|..j
-00002670: 0200 6a03 006a 0400 8300 0044 5d16 007d  ..j..j.....D]..}
-00002680: 0300 7c00 006a 0500 7c03 006a 0600 8301  ..|..j..|..j....
-00002690: 0001 7132 0057 6400 0053 2803 0000 004e  ..q2.Wd..S(....N
-000026a0: 69ff ffff ff28 0100 0000 740b 0000 0054  i....(....t....T
-000026b0: 7265 6550 726f 6669 6c65 2807 0000 0074  reeProfile(....t
-000026c0: 0500 0000 7079 6861 6d52 8e00 0000 5231  ....pyhamR....R1
-000026d0: 0000 0074 0700 0000 484f 474d 6170 7352  ...t....HOGMapsR
-000026e0: 4400 0000 5285 0000 0074 0a00 0000 636f  D...R....t....co
-000026f0: 6e73 6973 7465 6e74 2804 0000 0052 1100  nsistent(....R..
-00002700: 0000 528e 0000 0074 0200 0000 7470 7402  ..R....t....tpt.
-00002710: 0000 0068 6728 0000 0000 2800 0000 0073  ...hg(....(....s
-00002720: 4f00 0000 2f55 7365 7273 2f61 646d 696e  O.../Users/admin
-00002730: 2f57 6f72 6b2f 7072 6f6a 6563 742f 4465  /Work/project/De
-00002740: 7373 696d 6f7a 2f70 7968 616d 2d64 6576  ssimoz/pyham-dev
-00002750: 2f70 7968 616d 2f74 6573 7473 2f74 6573  /pyham/tests/tes
-00002760: 745f 6f72 7468 6f78 6d6c 7061 7273 6572  t_orthoxmlparser
-00002770: 2e70 7974 1700 0000 7465 7374 5f63 6f6e  .pyt....test_con
-00002780: 7369 7374 656e 6379 5f6e 756d 6265 72d2  sistency_number.
-00002790: 0000 0073 0800 0000 0002 1003 0f03 1901  ...s............
-000027a0: 6301 0000 0002 0000 0002 0000 0003 0000  c...............
-000027b0: 0073 2d00 0000 8700 0066 0100 6401 0086  .s-......f..d...
-000027c0: 0000 7d01 007c 0100 8800 006a 0000 8301  ..}..|.....j....
-000027d0: 0001 7c01 0088 0000 6a01 0083 0100 0164  ..|.....j......d
-000027e0: 0000 5328 0200 0000 4e63 0100 0000 0400  ..S(....Nc......
-000027f0: 0000 0d00 0000 1300 0000 737d 0000 0074  ..........s}...t
-00002800: 0000 6401 0064 0200 6403 0064 0400 6405  ..d..d..d..d..d.
-00002810: 0064 0600 6407 0064 0800 6409 0064 0a00  .d..d..d..d..d..
-00002820: 640b 0064 0800 8300 067d 0100 7401 006a  d..d.....}..t..j
-00002830: 0200 7403 0083 0100 7d02 0078 2a00 7c00  ..t.....}..x*.|.
-00002840: 006a 0400 8300 0044 5d1c 007d 0300 7c02  .j.....D]..}..|.
-00002850: 007c 0300 6a05 006a 0600 6302 0019 640c  .|..j..j..c...d.
-00002860: 0037 033c 7149 0057 8800 006a 0700 7c02  .7.<qI.W...j..|.
-00002870: 007c 0100 8302 0001 6400 0053 280d 0000  .|......d..S(...
-00002880: 004e 523a 0000 0069 0600 0000 523b 0000  .NR:...i....R;..
-00002890: 0069 0900 0000 523c 0000 0069 0800 0000  .i....R<...i....
-000028a0: 523d 0000 0069 0400 0000 523e 0000 0069  R=...i....R>...i
-000028b0: 0700 0000 523f 0000 0069 0100 0000 2808  ....R?...i....(.
-000028c0: 0000 0052 4000 0000 5241 0000 0052 4200  ...R@...RA...RB.
-000028d0: 0000 5243 0000 0052 4400 0000 5209 0000  ..RC...RD...R...
-000028e0: 0052 0b00 0000 5245 0000 0028 0400 0000  .R....RE...(....
-000028f0: 5235 0000 0052 4600 0000 5247 0000 0052  R5...RF...RG...R
-00002900: 4800 0000 2801 0000 0052 1100 0000 2800  H...(....R....(.
-00002910: 0000 0073 4f00 0000 2f55 7365 7273 2f61  ...sO.../Users/a
-00002920: 646d 696e 2f57 6f72 6b2f 7072 6f6a 6563  dmin/Work/projec
-00002930: 742f 4465 7373 696d 6f7a 2f70 7968 616d  t/Dessimoz/pyham
-00002940: 2d64 6576 2f70 7968 616d 2f74 6573 7473  -dev/pyham/tests
-00002950: 2f74 6573 745f 6f72 7468 6f78 6d6c 7061  /test_orthoxmlpa
-00002960: 7273 6572 2e70 7974 0900 0000 5f74 6573  rser.pyt...._tes
-00002970: 745f 6f6e 65df 0000 0073 0c00 0000 0001  t_one....s......
-00002980: 1e01 0f01 0f01 1301 1a01 2802 0000 0052  ..........(....R
-00002990: 3500 0000 528c 0000 0028 0200 0000 5211  5...R....(....R.
-000029a0: 0000 0052 9500 0000 2800 0000 0028 0100  ...R....(....(..
-000029b0: 0000 5211 0000 0073 4f00 0000 2f55 7365  ..R....sO.../Use
-000029c0: 7273 2f61 646d 696e 2f57 6f72 6b2f 7072  rs/admin/Work/pr
-000029d0: 6f6a 6563 742f 4465 7373 696d 6f7a 2f70  oject/Dessimoz/p
-000029e0: 7968 616d 2d64 6576 2f70 7968 616d 2f74  yham-dev/pyham/t
-000029f0: 6573 7473 2f74 6573 745f 6f72 7468 6f78  ests/test_orthox
-00002a00: 6d6c 7061 7273 6572 2e70 7952 4900 0000  mlparser.pyRI...
-00002a10: dd00 0000 7306 0000 0000 020f 080d 0163  ....s..........c
-00002a20: 0100 0000 0200 0000 0200 0000 4300 0000  ............C...
-00002a30: 7327 0000 0064 0100 8400 007d 0100 7c01  s'...d.....}..|.
-00002a40: 007c 0000 6a00 0083 0100 017c 0100 7c00  .|..j......|..|.
-00002a50: 006a 0100 8301 0001 6400 0053 2802 0000  .j......d..S(...
-00002a60: 004e 6301 0000 0005 0000 0006 0000 0053  .Nc............S
-00002a70: 0000 0073 9200 0000 7c00 006a 0000 8300  ...s....|..j....
-00002a80: 007d 0100 6905 0064 0100 6402 0036 6403  .}..i..d..d..6d.
-00002a90: 0064 0400 3664 0500 6406 0036 6407 0064  .d..6d..d..6d..d
-00002aa0: 0800 3664 0900 640a 0036 7d02 0069 0500  ..6d..d..6}..i..
-00002ab0: 640b 0064 0200 3664 0b00 6404 0036 640b  d..d..6d..d..6d.
-00002ac0: 0064 0600 3664 0b00 6408 0036 640b 0064  .d..6d..d..6d..d
-00002ad0: 0a00 367d 0300 782d 007c 0100 445d 2500  ..6}..x-.|..D]%.
-00002ae0: 7d04 007c 0300 7c04 006a 0100 6a02 0063  }..|..|..j..j..c
-00002af0: 0200 1974 0300 7c04 006a 0400 8301 0037  ...t..|..j.....7
-00002b00: 033c 7165 0057 6400 0053 280c 0000 004e  .<qe.Wd..S(....N
-00002b10: 6904 0000 0052 4a00 0000 6906 0000 0052  i....RJ...i....R
-00002b20: 4b00 0000 6908 0000 0052 4c00 0000 6905  K...i....RL...i.
-00002b30: 0000 0052 4d00 0000 6907 0000 0052 4e00  ...RM...i....RN.
-00002b40: 0000 6900 0000 0028 0500 0000 524f 0000  ..i....(....RO..
-00002b50: 0052 0a00 0000 520b 0000 0052 1600 0000  .R....R....R....
-00002b60: 5235 0000 0028 0500 0000 5200 0000 0052  R5...(....R....R
-00002b70: 5000 0000 5251 0000 0052 5200 0000 5253  P...RQ...RR...RS
-00002b80: 0000 0028 0000 0000 2800 0000 0073 4f00  ...(....(....sO.
-00002b90: 0000 2f55 7365 7273 2f61 646d 696e 2f57  ../Users/admin/W
-00002ba0: 6f72 6b2f 7072 6f6a 6563 742f 4465 7373  ork/project/Dess
-00002bb0: 696d 6f7a 2f70 7968 616d 2d64 6576 2f70  imoz/pyham-dev/p
-00002bc0: 7968 616d 2f74 6573 7473 2f74 6573 745f  yham/tests/test_
-00002bd0: 6f72 7468 6f78 6d6c 7061 7273 6572 2e70  orthoxmlparser.p
-00002be0: 7952 9500 0000 ec00 0000 730a 0000 0000  yR........s.....
-00002bf0: 010c 0129 0129 010d 0128 0200 0000 5231  ...).)...(....R1
-00002c00: 0000 0052 8a00 0000 2802 0000 0052 1100  ...R....(....R..
-00002c10: 0000 5295 0000 0028 0000 0000 2800 0000  ..R....(....(...
-00002c20: 0073 4f00 0000 2f55 7365 7273 2f61 646d  .sO.../Users/adm
-00002c30: 696e 2f57 6f72 6b2f 7072 6f6a 6563 742f  in/Work/project/
-00002c40: 4465 7373 696d 6f7a 2f70 7968 616d 2d64  Dessimoz/pyham-d
-00002c50: 6576 2f70 7968 616d 2f74 6573 7473 2f74  ev/pyham/tests/t
-00002c60: 6573 745f 6f72 7468 6f78 6d6c 7061 7273  est_orthoxmlpars
-00002c70: 6572 2e70 7952 5400 0000 ea00 0000 7306  er.pyRT.......s.
-00002c80: 0000 0000 0209 070d 0163 0100 0000 0200  .........c......
-00002c90: 0000 0200 0000 0300 0000 732d 0000 0087  ..........s-....
-00002ca0: 0000 6601 0064 0100 8600 007d 0100 7c01  ..f..d.....}..|.
-00002cb0: 0088 0000 6a00 0083 0100 017c 0100 8800  ....j......|....
-00002cc0: 006a 0100 8301 0001 6400 0053 2802 0000  .j......d..S(...
-00002cd0: 004e 6301 0000 0001 0000 0007 0000 0013  .Nc.............
-00002ce0: 0000 0073 6f00 0000 8800 006a 0000 7c00  ...so......j..|.
-00002cf0: 0064 0100 196a 0100 6402 0083 0100 6403  .d...j..d.....d.
-00002d00: 0083 0200 0188 0000 6a02 0074 0300 8301  ........j..t....
-00002d10: 008f 1600 017c 0000 6404 0019 6a01 0064  .....|..d...j..d
-00002d20: 0200 8301 0001 5764 0000 5158 8800 006a  ......Wd..QX...j
-00002d30: 0200 7403 0083 0100 8f16 0001 7c00 0064  ..t.........|..d
-00002d40: 0100 196a 0100 6405 0083 0100 0157 6400  ...j..d......Wd.
-00002d50: 0051 5864 0000 5328 0600 0000 4e52 5500  .QXd..S(....NRU.
-00002d60: 0000 5256 0000 0069 0100 0000 5257 0000  ..RV...i....RW..
-00002d70: 0052 5800 0000 2804 0000 0052 1e00 0000  .RX...(....R....
-00002d80: 5259 0000 0052 5a00 0000 525b 0000 0028  RY...RZ...R[...(
-00002d90: 0100 0000 5233 0000 0028 0100 0000 5211  ....R3...(....R.
-00002da0: 0000 0028 0000 0000 734f 0000 002f 5573  ...(....sO.../Us
-00002db0: 6572 732f 6164 6d69 6e2f 576f 726b 2f70  ers/admin/Work/p
-00002dc0: 726f 6a65 6374 2f44 6573 7369 6d6f 7a2f  roject/Dessimoz/
-00002dd0: 7079 6861 6d2d 6465 762f 7079 6861 6d2f  pyham-dev/pyham/
-00002de0: 7465 7374 732f 7465 7374 5f6f 7274 686f  tests/test_ortho
-00002df0: 786d 6c70 6172 7365 722e 7079 5295 0000  xmlparser.pyR...
-00002e00: 00f8 0000 0073 0a00 0000 0001 1d01 1001  .....s..........
-00002e10: 1701 1001 2802 0000 0052 3300 0000 528b  ....(....R3...R.
-00002e20: 0000 0028 0200 0000 5211 0000 0052 9500  ...(....R....R..
-00002e30: 0000 2800 0000 0028 0100 0000 5211 0000  ..(....(....R...
-00002e40: 0073 4f00 0000 2f55 7365 7273 2f61 646d  .sO.../Users/adm
-00002e50: 696e 2f57 6f72 6b2f 7072 6f6a 6563 742f  in/Work/project/
-00002e60: 4465 7373 696d 6f7a 2f70 7968 616d 2d64  Dessimoz/pyham-d
-00002e70: 6576 2f70 7968 616d 2f74 6573 7473 2f74  ev/pyham/tests/t
-00002e80: 6573 745f 6f72 7468 6f78 6d6c 7061 7273  est_orthoxmlpars
-00002e90: 6572 2e70 7952 5c00 0000 f600 0000 7306  er.pyR\.......s.
-00002ea0: 0000 0000 020f 070d 0163 0100 0000 0200  .........c......
-00002eb0: 0000 0200 0000 0300 0000 732d 0000 0087  ..........s-....
-00002ec0: 0000 6601 0064 0100 8600 007d 0100 7c01  ..f..d.....}..|.
-00002ed0: 0088 0000 6a00 0083 0100 017c 0100 8800  ....j......|....
-00002ee0: 006a 0100 8301 0001 6400 0053 2802 0000  .j......d..S(...
-00002ef0: 004e 6301 0000 0019 0000 000a 0000 0013  .Nc.............
-00002f00: 0000 0073 f301 0000 7c00 0064 0100 197d  ...s....|..d...}
-00002f10: 0100 7c00 0064 0200 197d 0200 7c00 0064  ..|..d...}..|..d
-00002f20: 0300 197d 0300 7c00 0064 0400 197d 0400  ...}..|..d...}..
-00002f30: 7c00 0064 0500 197d 0500 7c00 0064 0600  |..d...}..|..d..
-00002f40: 197d 0600 6407 0064 0800 6401 0064 0900  .}..d..d..d..d..
-00002f50: 640a 0064 0b00 6806 007d 0700 640c 0064  d..d..h..}..d..d
-00002f60: 0d00 6402 0064 0e00 6804 007d 0800 640f  ..d..d..h..}..d.
-00002f70: 0064 1000 6411 0064 1200 6804 007d 0900  .d..d..d..h..}..
-00002f80: 6413 0064 1400 6415 0064 1600 6417 0068  d..d..d..d..d..h
-00002f90: 0500 7d0a 0064 1800 6406 0064 1900 641a  ..}..d..d..d..d.
-00002fa0: 0064 1b00 641c 0064 1d00 641e 0064 1f00  .d..d..d..d..d..
-00002fb0: 6420 0068 0a00 7d0b 0064 2100 6422 0064  d .h..}..d!.d".d
-00002fc0: 2300 6424 0068 0400 7d0c 007c 0100 6a00  #.d$.h..}..|..j.
-00002fd0: 0083 0000 7d0d 007c 0200 6a00 0083 0000  ....}..|..j.....
-00002fe0: 7d0e 007c 0300 6a00 0083 0000 7d0f 007c  }..|..j.....}..|
-00002ff0: 0400 6a00 0083 0000 7d10 007c 0500 6a00  ..j.....}..|..j.
-00003000: 0083 0000 7d11 007c 0600 6a00 0083 0000  ....}..|..j.....
-00003010: 7d12 0074 0100 6425 0084 0000 7c0d 0044  }..t..d%....|..D
-00003020: 8301 0083 0100 7d13 0074 0100 6426 0084  ......}..t..d&..
-00003030: 0000 7c0e 0044 8301 0083 0100 7d14 0074  ..|..D......}..t
-00003040: 0100 6427 0084 0000 7c0f 0044 8301 0083  ..d'....|..D....
-00003050: 0100 7d15 0074 0100 6428 0084 0000 7c10  ..}..t..d(....|.
-00003060: 0044 8301 0083 0100 7d16 0074 0100 6429  .D......}..t..d)
-00003070: 0084 0000 7c11 0044 8301 0083 0100 7d17  ....|..D......}.
-00003080: 0074 0100 642a 0084 0000 7c12 0044 8301  .t..d*....|..D..
-00003090: 0083 0100 7d18 0088 0000 6a02 007c 0700  ....}.....j..|..
-000030a0: 7c13 0083 0200 0188 0000 6a02 007c 0800  |.........j..|..
-000030b0: 7c14 0083 0200 0188 0000 6a02 007c 0900  |.........j..|..
-000030c0: 7c15 0083 0200 0188 0000 6a02 007c 0a00  |.........j..|..
-000030d0: 7c16 0083 0200 0188 0000 6a02 007c 0b00  |.........j..|..
-000030e0: 7c17 0083 0200 0188 0000 6a02 007c 0c00  |.........j..|..
-000030f0: 7c18 0083 0200 0164 0000 5328 2b00 0000  |......d..S(+...
-00003100: 4e52 5500 0000 5257 0000 0052 5d00 0000  NRU...RW...R]...
-00003110: 7401 0000 0034 7401 0000 0035 7401 0000  t....4t....5t...
-00003120: 0036 525e 0000 0052 5f00 0000 5260 0000  .6R^...R_...R`..
-00003130: 0052 6100 0000 5262 0000 0052 6300 0000  .Ra...Rb...Rc...
-00003140: 5264 0000 0052 6500 0000 5266 0000 0052  Rd...Re...Rf...R
-00003150: 6700 0000 5269 0000 0052 6a00 0000 7402  g...Ri...Rj...t.
-00003160: 0000 0031 3574 0200 0000 3136 7402 0000  ...15t....16t...
-00003170: 0032 3474 0200 0000 3235 7402 0000 0035  .24t....25t....5
-00003180: 3474 0200 0000 3236 7402 0000 0031 3774  4t....26t....17t
-00003190: 0200 0000 3335 7402 0000 0034 3474 0100  ....35t....44t..
-000031a0: 0000 3774 0200 0000 3138 7402 0000 0033  ..7t....18t....3
-000031b0: 3674 0200 0000 3337 7402 0000 0034 3574  6t....37t....45t
-000031c0: 0200 0000 3139 7402 0000 0033 3874 0200  ....19t....38t..
-000031d0: 0000 3237 7402 0000 0035 3663 0100 0000  ..27t....56c....
-000031e0: 0200 0000 0200 0000 7300 0000 7318 0000  ........s...s...
-000031f0: 007c 0000 5d0e 007d 0100 7c01 006a 0000  .|..]..}..|..j..
-00003200: 5601 7103 0064 0000 5328 0100 0000 4e28  V.q..d..S(....N(
-00003210: 0100 0000 5207 0000 0028 0200 0000 521b  ....R....(....R.
-00003220: 0000 0052 6c00 0000 2800 0000 0028 0000  ...Rl...(....(..
-00003230: 0000 734f 0000 002f 5573 6572 732f 6164  ..sO.../Users/ad
-00003240: 6d69 6e2f 576f 726b 2f70 726f 6a65 6374  min/Work/project
-00003250: 2f44 6573 7369 6d6f 7a2f 7079 6861 6d2d  /Dessimoz/pyham-
-00003260: 6465 762f 7079 6861 6d2f 7465 7374 732f  dev/pyham/tests/
-00003270: 7465 7374 5f6f 7274 686f 786d 6c70 6172  test_orthoxmlpar
-00003280: 7365 722e 7079 7309 0000 003c 6765 6e65  ser.pys....<gene
-00003290: 7870 723e 1a01 0000 7302 0000 0006 0063  xpr>....s......c
-000032a0: 0100 0000 0200 0000 0200 0000 7300 0000  ............s...
-000032b0: 7318 0000 007c 0000 5d0e 007d 0100 7c01  s....|..]..}..|.
-000032c0: 006a 0000 5601 7103 0064 0000 5328 0100  .j..V.q..d..S(..
-000032d0: 0000 4e28 0100 0000 5207 0000 0028 0200  ..N(....R....(..
-000032e0: 0000 521b 0000 0052 6c00 0000 2800 0000  ..R....Rl...(...
-000032f0: 0028 0000 0000 734f 0000 002f 5573 6572  .(....sO.../User
-00003300: 732f 6164 6d69 6e2f 576f 726b 2f70 726f  s/admin/Work/pro
-00003310: 6a65 6374 2f44 6573 7369 6d6f 7a2f 7079  ject/Dessimoz/py
-00003320: 6861 6d2d 6465 762f 7079 6861 6d2f 7465  ham-dev/pyham/te
-00003330: 7374 732f 7465 7374 5f6f 7274 686f 786d  sts/test_orthoxm
-00003340: 6c70 6172 7365 722e 7079 7309 0000 003c  lparser.pys....<
-00003350: 6765 6e65 7870 723e 1b01 0000 7302 0000  genexpr>....s...
-00003360: 0006 0063 0100 0000 0200 0000 0200 0000  ...c............
-00003370: 7300 0000 7318 0000 007c 0000 5d0e 007d  s...s....|..]..}
-00003380: 0100 7c01 006a 0000 5601 7103 0064 0000  ..|..j..V.q..d..
-00003390: 5328 0100 0000 4e28 0100 0000 5207 0000  S(....N(....R...
-000033a0: 0028 0200 0000 521b 0000 0052 6c00 0000  .(....R....Rl...
-000033b0: 2800 0000 0028 0000 0000 734f 0000 002f  (....(....sO.../
-000033c0: 5573 6572 732f 6164 6d69 6e2f 576f 726b  Users/admin/Work
-000033d0: 2f70 726f 6a65 6374 2f44 6573 7369 6d6f  /project/Dessimo
-000033e0: 7a2f 7079 6861 6d2d 6465 762f 7079 6861  z/pyham-dev/pyha
-000033f0: 6d2f 7465 7374 732f 7465 7374 5f6f 7274  m/tests/test_ort
-00003400: 686f 786d 6c70 6172 7365 722e 7079 7309  hoxmlparser.pys.
-00003410: 0000 003c 6765 6e65 7870 723e 1c01 0000  ...<genexpr>....
-00003420: 7302 0000 0006 0063 0100 0000 0200 0000  s......c........
-00003430: 0200 0000 7300 0000 7318 0000 007c 0000  ....s...s....|..
-00003440: 5d0e 007d 0100 7c01 006a 0000 5601 7103  ]..}..|..j..V.q.
-00003450: 0064 0000 5328 0100 0000 4e28 0100 0000  .d..S(....N(....
-00003460: 5207 0000 0028 0200 0000 521b 0000 0052  R....(....R....R
-00003470: 6c00 0000 2800 0000 0028 0000 0000 734f  l...(....(....sO
-00003480: 0000 002f 5573 6572 732f 6164 6d69 6e2f  .../Users/admin/
-00003490: 576f 726b 2f70 726f 6a65 6374 2f44 6573  Work/project/Des
-000034a0: 7369 6d6f 7a2f 7079 6861 6d2d 6465 762f  simoz/pyham-dev/
-000034b0: 7079 6861 6d2f 7465 7374 732f 7465 7374  pyham/tests/test
-000034c0: 5f6f 7274 686f 786d 6c70 6172 7365 722e  _orthoxmlparser.
-000034d0: 7079 7309 0000 003c 6765 6e65 7870 723e  pys....<genexpr>
-000034e0: 1d01 0000 7302 0000 0006 0063 0100 0000  ....s......c....
-000034f0: 0200 0000 0200 0000 7300 0000 7318 0000  ........s...s...
-00003500: 007c 0000 5d0e 007d 0100 7c01 006a 0000  .|..]..}..|..j..
-00003510: 5601 7103 0064 0000 5328 0100 0000 4e28  V.q..d..S(....N(
-00003520: 0100 0000 5207 0000 0028 0200 0000 521b  ....R....(....R.
-00003530: 0000 0052 6c00 0000 2800 0000 0028 0000  ...Rl...(....(..
-00003540: 0000 734f 0000 002f 5573 6572 732f 6164  ..sO.../Users/ad
-00003550: 6d69 6e2f 576f 726b 2f70 726f 6a65 6374  min/Work/project
-00003560: 2f44 6573 7369 6d6f 7a2f 7079 6861 6d2d  /Dessimoz/pyham-
-00003570: 6465 762f 7079 6861 6d2f 7465 7374 732f  dev/pyham/tests/
-00003580: 7465 7374 5f6f 7274 686f 786d 6c70 6172  test_orthoxmlpar
-00003590: 7365 722e 7079 7309 0000 003c 6765 6e65  ser.pys....<gene
-000035a0: 7870 723e 1e01 0000 7302 0000 0006 0063  xpr>....s......c
-000035b0: 0100 0000 0200 0000 0200 0000 7300 0000  ............s...
-000035c0: 7318 0000 007c 0000 5d0e 007d 0100 7c01  s....|..]..}..|.
-000035d0: 006a 0000 5601 7103 0064 0000 5328 0100  .j..V.q..d..S(..
-000035e0: 0000 4e28 0100 0000 5207 0000 0028 0200  ..N(....R....(..
-000035f0: 0000 521b 0000 0052 6c00 0000 2800 0000  ..R....Rl...(...
-00003600: 0028 0000 0000 734f 0000 002f 5573 6572  .(....sO.../User
-00003610: 732f 6164 6d69 6e2f 576f 726b 2f70 726f  s/admin/Work/pro
-00003620: 6a65 6374 2f44 6573 7369 6d6f 7a2f 7079  ject/Dessimoz/py
-00003630: 6861 6d2d 6465 762f 7079 6861 6d2f 7465  ham-dev/pyham/te
-00003640: 7374 732f 7465 7374 5f6f 7274 686f 786d  sts/test_orthoxm
-00003650: 6c70 6172 7365 722e 7079 7309 0000 003c  lparser.pys....<
-00003660: 6765 6e65 7870 723e 1f01 0000 7302 0000  genexpr>....s...
-00003670: 0006 0028 0300 0000 526d 0000 0052 6e00  ...(....Rm...Rn.
-00003680: 0000 526f 0000 0028 1900 0000 5233 0000  ..Ro...(....R3..
-00003690: 0052 7000 0000 5271 0000 0052 7200 0000  .Rp...Rq...Rr...
-000036a0: 7404 0000 0068 6f67 3474 0400 0000 686f  t....hog4t....ho
-000036b0: 6735 7404 0000 0068 6f67 3652 7300 0000  g5t....hog6Rs...
-000036c0: 5274 0000 0052 7500 0000 7411 0000 0065  Rt...Ru...t....e
-000036d0: 7870 6563 7465 644d 656d 6265 7273 5f34  xpectedMembers_4
-000036e0: 7411 0000 0065 7870 6563 7465 644d 656d  t....expectedMem
-000036f0: 6265 7273 5f35 7411 0000 0065 7870 6563  bers_5t....expec
-00003700: 7465 644d 656d 6265 7273 5f36 5276 0000  tedMembers_6Rv..
-00003710: 0052 7700 0000 5278 0000 0074 0a00 0000  .Rw...Rx...t....
-00003720: 686f 6734 5f67 656e 6573 740a 0000 0068  hog4_genest....h
-00003730: 6f67 355f 6765 6e65 7374 0a00 0000 686f  og5_genest....ho
-00003740: 6736 5f67 656e 6573 5279 0000 0052 7a00  g6_genesRy...Rz.
-00003750: 0000 527b 0000 0074 0900 0000 6d65 6d62  ..R{...t....memb
-00003760: 6572 735f 3474 0900 0000 6d65 6d62 6572  ers_4t....member
-00003770: 735f 3574 0900 0000 6d65 6d62 6572 735f  s_5t....members_
-00003780: 3628 0100 0000 5211 0000 0028 0000 0000  6(....R....(....
-00003790: 734f 0000 002f 5573 6572 732f 6164 6d69  sO.../Users/admi
-000037a0: 6e2f 576f 726b 2f70 726f 6a65 6374 2f44  n/Work/project/D
-000037b0: 6573 7369 6d6f 7a2f 7079 6861 6d2d 6465  essimoz/pyham-de
-000037c0: 762f 7079 6861 6d2f 7465 7374 732f 7465  v/pyham/tests/te
-000037d0: 7374 5f6f 7274 686f 786d 6c70 6172 7365  st_orthoxmlparse
-000037e0: 722e 7079 5295 0000 0004 0100 0073 3c00  r.pyR........s<.
-000037f0: 0000 0001 0a01 0a01 0a01 0a01 0a01 0a02  ................
-00003800: 1801 1201 1201 1501 2401 1202 0c01 0c01  ........$.......
-00003810: 0c01 0c01 0c01 0c02 1601 1601 1601 1601  ................
-00003820: 1601 1602 1001 1001 1001 1001 1001 2802  ..............(.
-00003830: 0000 0052 3300 0000 528b 0000 0028 0200  ...R3...R....(..
-00003840: 0000 5211 0000 0052 9500 0000 2800 0000  ..R....R....(...
-00003850: 0028 0100 0000 5211 0000 0073 4f00 0000  .(....R....sO...
-00003860: 2f55 7365 7273 2f61 646d 696e 2f57 6f72  /Users/admin/Wor
-00003870: 6b2f 7072 6f6a 6563 742f 4465 7373 696d  k/project/Dessim
-00003880: 6f7a 2f70 7968 616d 2d64 6576 2f70 7968  oz/pyham-dev/pyh
-00003890: 616d 2f74 6573 7473 2f74 6573 745f 6f72  am/tests/test_or
-000038a0: 7468 6f78 6d6c 7061 7273 6572 2e70 7952  thoxmlparser.pyR
-000038b0: 7c00 0000 0201 0000 7306 0000 0000 020f  |.......s.......
-000038c0: 240d 0163 0100 0000 0200 0000 0300 0000  $..c............
-000038d0: 0300 0000 7335 0000 0087 0000 6601 0064  ....s5......f..d
-000038e0: 0100 8600 007d 0100 7c01 0088 0000 6a00  .....}..|.....j.
-000038f0: 0064 0200 1983 0100 017c 0100 8800 006a  .d.......|.....j
-00003900: 0100 6402 0019 8301 0001 6400 0053 2803  ..d.......d..S(.
-00003910: 0000 004e 6301 0000 0005 0000 0004 0000  ...Nc...........
-00003920: 0013 0000 0073 d300 0000 8800 006a 0000  .....s.......j..
-00003930: 6401 007c 0000 6a01 006a 0200 6a03 0083  d..|..j..j..j...
-00003940: 0200 0188 0000 6a04 007c 0000 6402 0064  ......j..|..d..d
-00003950: 0300 6702 0083 0200 0188 0000 6a05 007c  ..g.........j..|
-00003960: 0000 6403 0083 0200 7d01 0088 0000 6a04  ..d.....}.....j.
-00003970: 007c 0100 6404 0064 0500 6702 0083 0200  .|..d..d..g.....
-00003980: 0188 0000 6a05 007c 0100 6405 0083 0200  ....j..|..d.....
-00003990: 7d02 0088 0000 6a04 007c 0200 6406 0064  }.....j..|..d..d
-000039a0: 0700 6702 0083 0200 0188 0000 6a05 007c  ..g.........j..|
-000039b0: 0200 6406 0083 0200 7d03 0088 0000 6a04  ..d.....}.....j.
-000039c0: 007c 0300 6408 0064 0900 6702 0083 0200  .|..d..d..g.....
-000039d0: 0188 0000 6a05 007c 0200 6407 0083 0200  ....j..|..d.....
-000039e0: 7d04 0088 0000 6a04 007c 0400 640a 0064  }.....j..|..d..d
-000039f0: 0b00 6702 0083 0200 0164 0000 5328 0c00  ..g......d..S(..
-00003a00: 0000 4e52 4a00 0000 525e 0000 0052 4b00  ..NRJ...R^...RK.
-00003a10: 0000 525f 0000 0052 4c00 0000 524d 0000  ..R_...RL...RM..
-00003a20: 0052 4e00 0000 5262 0000 0052 6100 0000  .RN...Rb...Ra...
-00003a30: 5255 0000 0052 6000 0000 2806 0000 0052  RU...R`...(....R
-00003a40: 1e00 0000 5209 0000 0052 0a00 0000 520b  ....R....R....R.
-00003a50: 0000 0052 2200 0000 521a 0000 0028 0500  ...R"...R....(..
-00003a60: 0000 521f 0000 0052 7d00 0000 527e 0000  ..R....R}...R~..
-00003a70: 0052 7f00 0000 5280 0000 0028 0100 0000  .R....R....(....
-00003a80: 5211 0000 0028 0000 0000 734f 0000 002f  R....(....sO.../
-00003a90: 5573 6572 732f 6164 6d69 6e2f 576f 726b  Users/admin/Work
-00003aa0: 2f70 726f 6a65 6374 2f44 6573 7369 6d6f  /project/Dessimo
-00003ab0: 7a2f 7079 6861 6d2d 6465 762f 7079 6861  z/pyham-dev/pyha
-00003ac0: 6d2f 7465 7374 732f 7465 7374 5f6f 7274  m/tests/test_ort
-00003ad0: 686f 786d 6c70 6172 7365 722e 7079 5295  hoxmlparser.pyR.
-00003ae0: 0000 002d 0100 0073 1400 0000 0002 1901  ...-...s........
-00003af0: 1603 1201 1603 1201 1603 1201 1603 1201  ................
-00003b00: 5255 0000 0028 0200 0000 5233 0000 0052  RU...(....R3...R
-00003b10: 8b00 0000 2802 0000 0052 1100 0000 5295  ....(....R....R.
-00003b20: 0000 0028 0000 0000 2801 0000 0052 1100  ...(....(....R..
-00003b30: 0000 734f 0000 002f 5573 6572 732f 6164  ..sO.../Users/ad
-00003b40: 6d69 6e2f 576f 726b 2f70 726f 6a65 6374  min/Work/project
-00003b50: 2f44 6573 7369 6d6f 7a2f 7079 6861 6d2d  /Dessimoz/pyham-
-00003b60: 6465 762f 7079 6861 6d2f 7465 7374 732f  dev/pyham/tests/
-00003b70: 7465 7374 5f6f 7274 686f 786d 6c70 6172  test_orthoxmlpar
-00003b80: 7365 722e 7079 5281 0000 002b 0100 0073  ser.pyR....+...s
-00003b90: 0600 0000 0002 0f15 1101 6301 0000 0002  ..........c.....
-00003ba0: 0000 0003 0000 0003 0000 0073 3500 0000  ...........s5...
-00003bb0: 8700 0066 0100 6401 0086 0000 7d01 007c  ...f..d.....}..|
-00003bc0: 0100 8800 006a 0000 6402 0019 8301 0001  .....j..d.......
-00003bd0: 7c01 0088 0000 6a01 0064 0200 1983 0100  |.....j..d......
-00003be0: 0164 0000 5328 0300 0000 4e63 0100 0000  .d..S(....Nc....
-00003bf0: 0400 0000 0400 0000 1300 0000 73a8 0000  ............s...
-00003c00: 0088 0000 6a00 0064 0100 7c00 006a 0100  ....j..d..|..j..
-00003c10: 6a02 006a 0300 8302 0001 8800 006a 0400  j..j.........j..
-00003c20: 7c00 0064 0200 6403 0067 0200 8302 0001  |..d..d..g......
-00003c30: 8800 006a 0500 7c00 0064 0300 8302 007d  ...j..|..d.....}
-00003c40: 0100 8800 006a 0400 7c01 0064 0400 6405  .....j..|..d..d.
-00003c50: 0067 0200 8302 0001 8800 006a 0500 7c01  .g.........j..|.
-00003c60: 0064 0500 8302 007d 0200 8800 006a 0400  .d.....}.....j..
-00003c70: 7c02 0064 0600 6407 0067 0200 8302 0001  |..d..d..g......
-00003c80: 8800 006a 0500 7c01 0064 0400 8302 007d  ...j..|..d.....}
-00003c90: 0300 8800 006a 0400 7c03 0064 0800 6801  .....j..|..d..h.
-00003ca0: 0083 0200 0164 0000 5328 0900 0000 4e52  .....d..S(....NR
-00003cb0: 4b00 0000 5263 0000 0052 4c00 0000 524d  K...Rc...RL...RM
-00003cc0: 0000 0052 4e00 0000 5257 0000 0052 6500  ...RN...RW...Re.
-00003cd0: 0000 5264 0000 0028 0600 0000 521e 0000  ..Rd...(....R...
-00003ce0: 0052 0900 0000 520a 0000 0052 0b00 0000  .R....R....R....
-00003cf0: 5222 0000 0052 1a00 0000 2804 0000 0052  R"...R....(....R
-00003d00: 7100 0000 527e 0000 0052 8000 0000 527f  q...R~...R....R.
-00003d10: 0000 0028 0100 0000 5211 0000 0028 0000  ...(....R....(..
-00003d20: 0000 734f 0000 002f 5573 6572 732f 6164  ..sO.../Users/ad
-00003d30: 6d69 6e2f 576f 726b 2f70 726f 6a65 6374  min/Work/project
-00003d40: 2f44 6573 7369 6d6f 7a2f 7079 6861 6d2d  /Dessimoz/pyham-
-00003d50: 6465 762f 7079 6861 6d2f 7465 7374 732f  dev/pyham/tests/
-00003d60: 7465 7374 5f6f 7274 686f 786d 6c70 6172  test_orthoxmlpar
-00003d70: 7365 722e 7079 5295 0000 0047 0100 0073  ser.pyR....G...s
-00003d80: 1000 0000 0002 1901 1603 1201 1603 1201  ................
-00003d90: 1603 1201 5257 0000 0028 0200 0000 5233  ....RW...(....R3
-00003da0: 0000 0052 8b00 0000 2802 0000 0052 1100  ...R....(....R..
-00003db0: 0000 5295 0000 0028 0000 0000 2801 0000  ..R....(....(...
-00003dc0: 0052 1100 0000 734f 0000 002f 5573 6572  .R....sO.../User
-00003dd0: 732f 6164 6d69 6e2f 576f 726b 2f70 726f  s/admin/Work/pro
-00003de0: 6a65 6374 2f44 6573 7369 6d6f 7a2f 7079  ject/Dessimoz/py
-00003df0: 6861 6d2d 6465 762f 7079 6861 6d2f 7465  ham-dev/pyham/te
-00003e00: 7374 732f 7465 7374 5f6f 7274 686f 786d  sts/test_orthoxm
-00003e10: 6c70 6172 7365 722e 7079 5282 0000 0045  lparser.pyR....E
-00003e20: 0100 0073 0600 0000 0002 0f11 1101 6301  ...s..........c.
-00003e30: 0000 0002 0000 0003 0000 0003 0000 0073  ...............s
-00003e40: 3500 0000 8700 0066 0100 6401 0086 0000  5......f..d.....
-00003e50: 7d01 007c 0100 8800 006a 0000 6402 0019  }..|.....j..d...
-00003e60: 8301 0001 7c01 0088 0000 6a01 0064 0200  ....|.....j..d..
-00003e70: 1983 0100 0164 0000 5328 0300 0000 4e63  .....d..S(....Nc
-00003e80: 0100 0000 0600 0000 0400 0000 1300 0000  ................
-00003e90: 732c 0100 0088 0000 6a00 0064 0100 7c00  s,......j..d..|.
-00003ea0: 006a 0100 6a02 006a 0300 8302 0001 8800  .j..j..j........
-00003eb0: 006a 0400 7c00 0064 0200 6403 0067 0200  .j..|..d..d..g..
-00003ec0: 8302 0001 8800 006a 0500 7c00 006a 0600  .......j..|..j..
-00003ed0: 8301 0001 8800 006a 0700 7c00 0064 0300  .......j..|..d..
-00003ee0: 8302 007d 0100 8800 006a 0400 7c01 0064  ...}.....j..|..d
-00003ef0: 0400 6405 0067 0200 8302 0001 8800 006a  ..d..g.........j
-00003f00: 0500 7c01 006a 0600 8301 0001 8800 006a  ..|..j.........j
-00003f10: 0700 7c01 0064 0500 8302 007d 0200 8800  ..|..d.....}....
-00003f20: 006a 0500 7c02 006a 0600 8301 0001 8800  .j..|..j........
-00003f30: 006a 0400 7c02 0064 0600 6701 0083 0200  .j..|..d..g.....
-00003f40: 0188 0000 6a07 007c 0200 6406 0083 0200  ....j..|..d.....
-00003f50: 7d03 0088 0000 6a05 007c 0300 6a06 0083  }.....j..|..j...
-00003f60: 0100 0188 0000 6a04 007c 0300 6407 0064  ......j..|..d..d
-00003f70: 0800 6702 0083 0200 0188 0000 6a08 006a  ..g.........j..j
-00003f80: 0900 6407 0083 0100 7d04 0088 0000 6a0a  ..d.....}.....j.
-00003f90: 007c 0400 6a06 0083 0100 0188 0000 6a08  .|..j.........j.
-00003fa0: 006a 0900 6408 0083 0100 7d05 0088 0000  .j..d.....}.....
-00003fb0: 6a0a 007c 0500 6a06 0083 0100 0164 0000  j..|..j......d..
-00003fc0: 5328 0900 0000 4e52 4a00 0000 5269 0000  S(....NRJ...Ri..
-00003fd0: 0052 4b00 0000 5267 0000 0052 4c00 0000  .RK...Rg...RL...
-00003fe0: 524e 0000 0052 6600 0000 526a 0000 0028  RN...Rf...Rj...(
-00003ff0: 0b00 0000 521e 0000 0052 0900 0000 520a  ....R....R....R.
-00004000: 0000 0052 0b00 0000 5222 0000 0052 8300  ...R....R"...R..
-00004010: 0000 5284 0000 0052 1a00 0000 5231 0000  ..R....R....R1..
-00004020: 0074 0e00 0000 6765 745f 6765 6e65 5f62  .t....get_gene_b
-00004030: 795f 6964 5285 0000 0028 0600 0000 5272  y_idR....(....Rr
-00004040: 0000 0052 7d00 0000 5286 0000 0052 8000  ...R}...R....R..
-00004050: 0000 7403 0000 0067 3133 7403 0000 0067  ..t....g13t....g
-00004060: 3134 2801 0000 0052 1100 0000 2800 0000  14(....R....(...
-00004070: 0073 4f00 0000 2f55 7365 7273 2f61 646d  .sO.../Users/adm
-00004080: 696e 2f57 6f72 6b2f 7072 6f6a 6563 742f  in/Work/project/
-00004090: 4465 7373 696d 6f7a 2f70 7968 616d 2d64  Dessimoz/pyham-d
-000040a0: 6576 2f70 7968 616d 2f74 6573 7473 2f74  ev/pyham/tests/t
-000040b0: 6573 745f 6f72 7468 6f78 6d6c 7061 7273  est_orthoxmlpars
-000040c0: 6572 2e70 7952 9500 0000 5d01 0000 7320  er.pyR....]...s 
-000040d0: 0000 0000 0219 0116 0110 0312 0116 0110  ................
-000040e0: 0312 0110 0113 0312 0110 0116 0112 0110  ................
-000040f0: 0112 0152 5d00 0000 2802 0000 0052 3300  ...R]...(....R3.
-00004100: 0000 528b 0000 0028 0200 0000 5211 0000  ..R....(....R...
-00004110: 0052 9500 0000 2800 0000 0028 0100 0000  .R....(....(....
-00004120: 5211 0000 0073 4f00 0000 2f55 7365 7273  R....sO.../Users
-00004130: 2f61 646d 696e 2f57 6f72 6b2f 7072 6f6a  /admin/Work/proj
-00004140: 6563 742f 4465 7373 696d 6f7a 2f70 7968  ect/Dessimoz/pyh
-00004150: 616d 2d64 6576 2f70 7968 616d 2f74 6573  am-dev/pyham/tes
-00004160: 7473 2f74 6573 745f 6f72 7468 6f78 6d6c  ts/test_orthoxml
-00004170: 7061 7273 6572 2e70 7952 8700 0000 5b01  parser.pyR....[.
-00004180: 0000 7306 0000 0000 020f 1911 0163 0100  ..s..........c..
-00004190: 0000 0200 0000 0300 0000 0300 0000 7335  ..............s5
-000041a0: 0000 0087 0000 6601 0064 0100 8600 007d  ......f..d.....}
-000041b0: 0100 7c01 0088 0000 6a00 0064 0200 1983  ..|.....j..d....
-000041c0: 0100 017c 0100 8800 006a 0100 6402 0019  ...|.....j..d...
-000041d0: 8301 0001 6400 0053 2803 0000 004e 6301  ....d..S(....Nc.
-000041e0: 0000 0008 0000 0005 0000 0013 0000 0073  ...............s
-000041f0: 7301 0000 8800 006a 0000 6401 007c 0000  s......j..d..|..
-00004200: 6a01 006a 0200 6a03 0083 0200 0188 0000  j..j..j.........
-00004210: 6a04 007c 0000 6402 0064 0300 6702 0083  j..|..d..d..g...
-00004220: 0200 0188 0000 6a05 007c 0000 6a06 0083  ......j..|..j...
-00004230: 0100 0188 0000 6a07 007c 0000 6403 0083  ......j..|..d...
-00004240: 0200 7d01 0088 0000 6a04 007c 0100 6404  ..}.....j..|..d.
-00004250: 0064 0500 6406 0067 0300 8302 0001 8800  .d..d..g........
-00004260: 006a 0500 7c01 006a 0600 8301 0001 8800  .j..|..j........
-00004270: 006a 0800 6a09 0064 0400 8301 007d 0200  .j..j..d.....}..
-00004280: 8800 006a 0a00 7c02 006a 0600 8301 0001  ...j..|..j......
-00004290: 8800 006a 0800 6a09 0064 0500 8301 007d  ...j..j..d.....}
-000042a0: 0300 8800 006a 0a00 7c03 006a 0600 8301  .....j..|..j....
-000042b0: 0001 8800 006a 0700 7c01 0064 0600 8302  .....j..|..d....
-000042c0: 007d 0400 8800 006a 0500 7c04 006a 0600  .}.....j..|..j..
-000042d0: 8301 0001 8800 006a 0400 7c04 0064 0700  .......j..|..d..
-000042e0: 6701 0083 0200 0188 0000 6a07 007c 0400  g.........j..|..
-000042f0: 6407 0083 0200 7d05 0088 0000 6a05 007c  d.....}.....j..|
-00004300: 0500 6a06 0083 0100 0188 0000 6a04 007c  ..j.........j..|
-00004310: 0500 6408 0064 0900 6702 0083 0200 0188  ..d..d..g.......
-00004320: 0000 6a08 006a 0900 6408 0083 0100 7d06  ..j..j..d.....}.
-00004330: 0088 0000 6a0a 007c 0600 6a06 0083 0100  ....j..|..j.....
-00004340: 0188 0000 6a08 006a 0900 6409 0083 0100  ....j..j..d.....
-00004350: 7d07 0088 0000 6a0a 007c 0700 6a06 0083  }.....j..|..j...
-00004360: 0100 0164 0000 5328 0a00 0000 4e52 4a00  ...d..S(....NRJ.
-00004370: 0000 529d 0000 0052 4b00 0000 529b 0000  ..R....RK...R...
-00004380: 0052 9c00 0000 524c 0000 0052 4e00 0000  .R....RL...RN...
-00004390: 5299 0000 0052 9a00 0000 280b 0000 0052  R....R....(....R
-000043a0: 1e00 0000 5209 0000 0052 0a00 0000 520b  ....R....R....R.
-000043b0: 0000 0052 2200 0000 5283 0000 0052 8400  ...R"...R....R..
-000043c0: 0000 521a 0000 0052 3100 0000 52b7 0000  ..R....R1...R...
-000043d0: 0052 8500 0000 2808 0000 0052 ab00 0000  .R....(....R....
-000043e0: 527d 0000 0074 0300 0000 6732 3474 0300  R}...t....g24t..
-000043f0: 0000 6732 3552 8600 0000 5280 0000 0074  ..g25R....R....t
-00004400: 0300 0000 6731 3574 0300 0000 6731 3628  ....g15t....g16(
-00004410: 0100 0000 5211 0000 0028 0000 0000 734f  ....R....(....sO
-00004420: 0000 002f 5573 6572 732f 6164 6d69 6e2f  .../Users/admin/
-00004430: 576f 726b 2f70 726f 6a65 6374 2f44 6573  Work/project/Des
-00004440: 7369 6d6f 7a2f 7079 6861 6d2d 6465 762f  simoz/pyham-dev/
-00004450: 7079 6861 6d2f 7465 7374 732f 7465 7374  pyham/tests/test
-00004460: 5f6f 7274 686f 786d 6c70 6172 7365 722e  _orthoxmlparser.
-00004470: 7079 5295 0000 007b 0100 0073 2800 0000  pyR....{...s(...
-00004480: 0002 1901 1601 1003 1201 1901 1001 1201  ................
-00004490: 1001 1201 1003 1201 1001 1303 1201 1001  ................
-000044a0: 1601 1201 1001 1201 5296 0000 0028 0200  ........R....(..
-000044b0: 0000 5233 0000 0052 8b00 0000 2802 0000  ..R3...R....(...
-000044c0: 0052 1100 0000 5295 0000 0028 0000 0000  .R....R....(....
-000044d0: 2801 0000 0052 1100 0000 734f 0000 002f  (....R....sO.../
-000044e0: 5573 6572 732f 6164 6d69 6e2f 576f 726b  Users/admin/Work
-000044f0: 2f70 726f 6a65 6374 2f44 6573 7369 6d6f  /project/Dessimo
-00004500: 7a2f 7079 6861 6d2d 6465 762f 7079 6861  z/pyham-dev/pyha
-00004510: 6d2f 7465 7374 732f 7465 7374 5f6f 7274  m/tests/test_ort
-00004520: 686f 786d 6c70 6172 7365 722e 7079 7420  hoxmlparser.pyt 
-00004530: 0000 0074 6573 745f 686f 675f 7769 7468  ...test_hog_with
-00004540: 5f73 6973 7465 725f 6475 706c 6963 6174  _sister_duplicat
-00004550: 696f 6e79 0100 0073 0600 0000 0002 0f1d  iony...s........
-00004560: 1101 6301 0000 0002 0000 0003 0000 0003  ..c.............
-00004570: 0000 0073 3500 0000 8700 0066 0100 6401  ...s5......f..d.
-00004580: 0086 0000 7d01 007c 0100 8800 006a 0000  ....}..|.....j..
-00004590: 6402 0019 8301 0001 7c01 0088 0000 6a01  d.......|.....j.
-000045a0: 0064 0200 1983 0100 0164 0000 5328 0300  .d.......d..S(..
-000045b0: 0000 4e63 0100 0000 0800 0000 0500 0000  ..Nc............
-000045c0: 1300 0000 7324 0200 0088 0000 6a00 0064  ....s$......j..d
-000045d0: 0100 7c00 006a 0100 6a02 006a 0300 8302  ..|..j..j..j....
-000045e0: 0001 8800 006a 0400 7c00 0064 0200 6403  .....j..|..d..d.
-000045f0: 0064 0300 6703 0083 0200 0188 0000 6a05  .d..g.........j.
-00004600: 007c 0000 6a06 0083 0100 0188 0000 6a07  .|..j.........j.
-00004610: 007c 0000 6403 0083 0200 7d01 0088 0000  .|..d.....}.....
-00004620: 6a08 006a 0900 6404 0083 0100 7c01 0064  j..j..d.....|..d
-00004630: 0500 196a 0a00 8300 006b 0600 728d 007c  ...j.....k..r..|
-00004640: 0100 6406 0019 7d02 007c 0100 6405 0019  ..d...}..|..d...
-00004650: 7d03 006e 1400 7c01 0064 0500 197d 0200  }..n..|..d...}..
-00004660: 7c01 0064 0600 197d 0300 8800 006a 0b00  |..d...}.....j..
-00004670: 740c 007c 0200 6a06 0083 0200 0188 0000  t..|..j.........
-00004680: 6a04 007c 0200 6407 0064 0800 6702 0083  j..|..d..d..g...
-00004690: 0200 0188 0000 6a07 007c 0200 6407 0083  ......j..|..d...
-000046a0: 0200 7d04 0088 0000 6a05 007c 0400 6a06  ..}.....j..|..j.
-000046b0: 0083 0100 0188 0000 6a04 007c 0400 6409  ........j..|..d.
-000046c0: 0064 0a00 6702 0083 0200 0188 0000 6a07  .d..g.........j.
-000046d0: 007c 0200 6408 0083 0200 7d05 0088 0000  .|..d.....}.....
-000046e0: 6a05 007c 0500 6a06 0083 0100 0188 0000  j..|..j.........
-000046f0: 6a04 007c 0500 640b 0064 0c00 640d 0067  j..|..d..d..d..g
-00004700: 0300 8302 0001 8800 006a 0800 6a09 0064  .........j..j..d
-00004710: 0b00 8301 007d 0600 8800 006a 0b00 740c  .....}.....j..t.
-00004720: 007c 0600 6a06 0083 0200 0188 0000 6a08  .|..j.........j.
-00004730: 006a 0900 640c 0083 0100 7d07 0088 0000  .j..d.....}.....
-00004740: 6a0b 0074 0c00 7c07 006a 0600 8302 0001  j..t..|..j......
-00004750: 8800 006a 0b00 740c 007c 0300 6a06 0083  ...j..t..|..j...
-00004760: 0200 0188 0000 6a04 007c 0300 6407 0064  ......j..|..d..d
-00004770: 0800 6702 0083 0200 0188 0000 6a07 007c  ..g.........j..|
-00004780: 0300 6407 0083 0200 7d04 0088 0000 6a05  ..d.....}.....j.
-00004790: 007c 0400 6a06 0083 0100 0188 0000 6a04  .|..j.........j.
-000047a0: 007c 0400 640e 0064 0f00 6702 0083 0200  .|..d..d..g.....
-000047b0: 0188 0000 6a07 007c 0300 6408 0083 0200  ....j..|..d.....
-000047c0: 7d05 0088 0000 6a05 007c 0500 6a06 0083  }.....j..|..j...
-000047d0: 0100 0188 0000 6a04 007c 0500 6404 0064  ......j..|..d..d
-000047e0: 1000 6702 0083 0200 0164 0000 5328 1100  ..g......d..S(..
-000047f0: 0000 4e52 4b00 0000 529e 0000 0052 4c00  ..NRK...R....RL.
-00004800: 0000 52a0 0000 0069 0000 0000 6901 0000  ..R....i....i...
-00004810: 0052 4e00 0000 524d 0000 0052 9800 0000  .RN...RM...R....
-00004820: 529f 0000 0052 a400 0000 52a5 0000 0052  R....R....R....R
-00004830: a100 0000 52a2 0000 0052 a300 0000 52a6  ....R....R....R.
-00004840: 0000 0028 0d00 0000 521e 0000 0052 0900  ...(....R....R..
-00004850: 0000 520a 0000 0052 0b00 0000 5222 0000  ..R....R....R"..
-00004860: 0052 8300 0000 5284 0000 0052 1a00 0000  .R....R....R....
-00004870: 5231 0000 0052 b700 0000 526d 0000 0074  R1...R....Rm...t
-00004880: 0e00 0000 6173 7365 7274 4e6f 7445 7175  ....assertNotEqu
-00004890: 616c 7405 0000 0046 616c 7365 2808 0000  alt....False(...
-000048a0: 0052 ac00 0000 527e 0000 0074 1200 0000  .R....R~...t....
-000048b0: 6575 6172 6368 6f6e 746f 676c 6972 6573  euarchontoglires
-000048c0: 5f41 7412 0000 0065 7561 7263 686f 6e74  _At....euarchont
-000048d0: 6f67 6c69 7265 735f 4252 8000 0000 527f  oglires_BR....R.
-000048e0: 0000 0074 0300 0000 6733 3674 0300 0000  ...t....g36t....
-000048f0: 6733 3728 0100 0000 5211 0000 0028 0000  g37(....R....(..
-00004900: 0000 734f 0000 002f 5573 6572 732f 6164  ..sO.../Users/ad
-00004910: 6d69 6e2f 576f 726b 2f70 726f 6a65 6374  min/Work/project
-00004920: 2f44 6573 7369 6d6f 7a2f 7079 6861 6d2d  /Dessimoz/pyham-
-00004930: 6465 762f 7079 6861 6d2f 7465 7374 732f  dev/pyham/tests/
-00004940: 7465 7374 5f6f 7274 686f 786d 6c70 6172  test_orthoxmlpar
-00004950: 7365 722e 7079 5295 0000 009d 0100 0073  ser.pyR........s
-00004960: 3a00 0000 0002 1901 1901 1003 1202 2201  :.............".
-00004970: 0a01 0d02 0a01 0a03 1301 1602 1201 1001  ................
-00004980: 1602 1201 1001 1901 1201 1301 1201 1303  ................
-00004990: 1301 1602 1201 1001 1602 1201 1001 5297  ..............R.
-000049a0: 0000 0028 0200 0000 5233 0000 0052 8b00  ...(....R3...R..
-000049b0: 0000 2802 0000 0052 1100 0000 5295 0000  ..(....R....R...
-000049c0: 0028 0000 0000 2801 0000 0052 1100 0000  .(....(....R....
-000049d0: 734f 0000 002f 5573 6572 732f 6164 6d69  sO.../Users/admi
-000049e0: 6e2f 576f 726b 2f70 726f 6a65 6374 2f44  n/Work/project/D
-000049f0: 6573 7369 6d6f 7a2f 7079 6861 6d2d 6465  essimoz/pyham-de
-00004a00: 762f 7079 6861 6d2f 7465 7374 732f 7465  v/pyham/tests/te
-00004a10: 7374 5f6f 7274 686f 786d 6c70 6172 7365  st_orthoxmlparse
-00004a20: 722e 7079 7420 0000 0074 6573 745f 686f  r.pyt ...test_ho
-00004a30: 675f 7769 7468 5f6e 6573 7465 645f 6475  g_with_nested_du
-00004a40: 706c 6963 6174 696f 6e9b 0100 0073 0600  plication....s..
-00004a50: 0000 0002 0f2c 1101 6301 0000 0002 0000  .....,..c.......
-00004a60: 0003 0000 0003 0000 0073 3500 0000 8700  .........s5.....
-00004a70: 0066 0100 6401 0086 0000 7d01 007c 0100  .f..d.....}..|..
-00004a80: 8800 006a 0000 6402 0019 8301 0001 7c01  ...j..d.......|.
-00004a90: 0088 0000 6a01 0064 0200 1983 0100 0164  ....j..d.......d
-00004aa0: 0000 5328 0300 0000 4e63 0100 0000 0900  ..S(....Nc......
-00004ab0: 0000 0500 0000 1300 0000 73dd 0100 0088  ..........s.....
-00004ac0: 0000 6a00 0064 0100 7c00 006a 0100 6a02  ..j..d..|..j..j.
-00004ad0: 006a 0300 8302 0001 8800 006a 0400 7c00  .j.........j..|.
-00004ae0: 0064 0200 6403 0067 0200 8302 0001 8800  .d..d..g........
-00004af0: 006a 0500 7c00 006a 0600 8301 0001 8800  .j..|..j........
-00004b00: 006a 0700 7c00 0064 0300 8302 007d 0100  .j..|..d.....}..
-00004b10: 8800 006a 0400 7c01 0064 0400 6405 0064  ...j..|..d..d..d
-00004b20: 0500 6703 0083 0200 0188 0000 6a05 007c  ..g.........j..|
-00004b30: 0100 6a06 0083 0100 0188 0000 6a07 007c  ..j.........j..|
-00004b40: 0100 6405 0083 0200 7d02 0088 0000 6a08  ..d.....}.....j.
-00004b50: 006a 0900 6406 0083 0100 7c02 0064 0700  .j..d.....|..d..
-00004b60: 196a 0a00 8300 006b 0600 72c5 007c 0200  .j.....k..r..|..
-00004b70: 6408 0019 7d03 007c 0200 6407 0019 7d04  d...}..|..d...}.
-00004b80: 006e 1400 7c02 0064 0700 197d 0300 7c02  .n..|..d...}..|.
-00004b90: 0064 0800 197d 0400 8800 006a 0b00 740c  .d...}.....j..t.
-00004ba0: 007c 0300 6a06 0083 0200 0188 0000 6a04  .|..j.........j.
-00004bb0: 007c 0300 6409 0067 0100 8302 0001 8800  .|..d..g........
-00004bc0: 006a 0700 7c03 0064 0900 8302 007d 0500  .j..|..d.....}..
-00004bd0: 8800 006a 0500 7c05 006a 0600 8301 0001  ...j..|..j......
-00004be0: 8800 006a 0400 7c05 0064 0a00 6701 0083  ...j..|..d..g...
-00004bf0: 0200 0188 0000 6a08 006a 0900 640a 0083  ......j..j..d...
-00004c00: 0100 7d06 0088 0000 6a00 0074 0c00 7c06  ..}.....j..t..|.
-00004c10: 006a 0600 8302 0001 8800 006a 0b00 740c  .j.........j..t.
-00004c20: 007c 0400 6a06 0083 0200 0188 0000 6a04  .|..j.........j.
-00004c30: 007c 0400 640b 0067 0100 8302 0001 8800  .|..d..g........
-00004c40: 006a 0700 7c04 0064 0b00 8302 007d 0700  .j..|..d.....}..
-00004c50: 8800 006a 0500 7c07 006a 0600 8301 0001  ...j..|..j......
-00004c60: 8800 006a 0400 7c07 0064 0600 6701 0083  ...j..|..d..g...
-00004c70: 0200 0188 0000 6a08 006a 0900 6406 0083  ......j..j..d...
-00004c80: 0100 7d08 0088 0000 6a00 0074 0c00 7c08  ..}.....j..t..|.
-00004c90: 006a 0600 8302 0001 6400 0053 280c 0000  .j......d..S(...
-00004ca0: 004e 524a 0000 0052 aa00 0000 524b 0000  .NRJ...R....RK..
-00004cb0: 0052 a900 0000 524c 0000 0052 a800 0000  .R....RL...R....
-00004cc0: 6900 0000 0069 0100 0000 524e 0000 0052  i....i....RN...R
-00004cd0: a700 0000 524d 0000 0028 0d00 0000 521e  ....RM...(....R.
-00004ce0: 0000 0052 0900 0000 520a 0000 0052 0b00  ...R....R....R..
-00004cf0: 0000 5222 0000 0052 8300 0000 5284 0000  ..R"...R....R...
-00004d00: 0052 1a00 0000 5231 0000 0052 b700 0000  .R....R1...R....
-00004d10: 526d 0000 0052 bf00 0000 52c0 0000 0028  Rm...R....R....(
-00004d20: 0900 0000 52ad 0000 0052 7d00 0000 527e  ....R....R}...R~
-00004d30: 0000 0052 c100 0000 52c2 0000 0052 8000  ...R....R....R..
-00004d40: 0000 7403 0000 0067 3139 527f 0000 0074  ..t....g19R....t
-00004d50: 0300 0000 6733 3828 0100 0000 5211 0000  ....g38(....R...
-00004d60: 0028 0000 0000 734f 0000 002f 5573 6572  .(....sO.../User
-00004d70: 732f 6164 6d69 6e2f 576f 726b 2f70 726f  s/admin/Work/pro
-00004d80: 6a65 6374 2f44 6573 7369 6d6f 7a2f 7079  ject/Dessimoz/py
-00004d90: 6861 6d2d 6465 762f 7079 6861 6d2f 7465  ham-dev/pyham/te
-00004da0: 7374 732f 7465 7374 5f6f 7274 686f 786d  sts/test_orthoxm
-00004db0: 6c70 6172 7365 722e 7079 5295 0000 00ce  lparser.pyR.....
-00004dc0: 0100 0073 3400 0000 0002 1901 1601 1003  ...s4...........
-00004dd0: 1201 1901 1003 1202 2201 0a01 0d02 0a01  ........".......
-00004de0: 0a04 1301 1302 1201 1001 1301 1201 1303  ................
-00004df0: 1301 1302 1201 1001 1301 1201 5298 0000  ............R...
-00004e00: 0028 0200 0000 5233 0000 0052 8b00 0000  .(....R3...R....
-00004e10: 2802 0000 0052 1100 0000 5295 0000 0028  (....R....R....(
-00004e20: 0000 0000 2801 0000 0052 1100 0000 734f  ....(....R....sO
-00004e30: 0000 002f 5573 6572 732f 6164 6d69 6e2f  .../Users/admin/
-00004e40: 576f 726b 2f70 726f 6a65 6374 2f44 6573  Work/project/Des
-00004e50: 7369 6d6f 7a2f 7079 6861 6d2d 6465 762f  simoz/pyham-dev/
-00004e60: 7079 6861 6d2f 7465 7374 732f 7465 7374  pyham/tests/test
-00004e70: 5f6f 7274 686f 786d 6c70 6172 7365 722e  _orthoxmlparser.
-00004e80: 7079 7420 0000 0074 6573 745f 686f 675f  pyt ...test_hog_
-00004e90: 7769 7468 5f6c 6f73 7365 735f 6475 706c  with_losses_dupl
-00004ea0: 6963 6174 696f 6ecc 0100 0073 0600 0000  ication....s....
-00004eb0: 0002 0f2a 1101 6301 0000 0005 0000 0007  ...*..c.........
-00004ec0: 0000 0043 0000 0073 7300 0000 786c 007c  ...C...ss...xl.|
-00004ed0: 0000 6a00 006a 0100 8300 0044 5d5b 007d  ..j..j.....D][.}
-00004ee0: 0100 7852 007c 0100 6a02 0083 0000 445d  ..xR.|..j.....D]
-00004ef0: 4400 7d02 0078 3b00 7c02 006a 0300 445d  D.}..x;.|..j..D]
-00004f00: 3000 7d03 0078 2700 7c03 006a 0400 445d  0.}..x'.|..j..D]
-00004f10: 1c00 7d04 007c 0000 6a05 007c 0400 7c02  ..}..|..j..|..|.
-00004f20: 006a 0400 6b06 0083 0100 0171 4300 5771  .j..k......qC.Wq
-00004f30: 3300 5771 2300 5771 1000 5764 0000 5328  3.Wq#.Wq..Wd..S(
-00004f40: 0100 0000 4e28 0600 0000 5231 0000 0074  ....N(....R1...t
-00004f50: 1700 0000 6765 745f 6c69 7374 5f74 6f70  ....get_list_top
-00004f60: 5f6c 6576 656c 5f68 6f67 7374 1700 0000  _level_hogst....
-00004f70: 6765 745f 616c 6c5f 6465 7363 656e 6461  get_all_descenda
-00004f80: 6e74 5f68 6f67 7374 0c00 0000 6475 706c  nt_hogst....dupl
-00004f90: 6963 6174 696f 6e73 5214 0000 0052 8500  icationsR....R..
-00004fa0: 0000 2805 0000 0052 1100 0000 7407 0000  ..(....R....t...
-00004fb0: 0074 6f70 5f68 6f67 7407 0000 0073 7562  .top_hogt....sub
-00004fc0: 5f68 6f67 7403 0000 0064 7570 7401 0000  _hogt....dupt...
-00004fd0: 0065 2800 0000 0028 0000 0000 734f 0000  .e(....(....sO..
-00004fe0: 002f 5573 6572 732f 6164 6d69 6e2f 576f  ./Users/admin/Wo
-00004ff0: 726b 2f70 726f 6a65 6374 2f44 6573 7369  rk/project/Dessi
-00005000: 6d6f 7a2f 7079 6861 6d2d 6465 762f 7079  moz/pyham-dev/py
-00005010: 6861 6d2f 7465 7374 732f 7465 7374 5f6f  ham/tests/test_o
-00005020: 7274 686f 786d 6c70 6172 7365 722e 7079  rthoxmlparser.py
-00005030: 742d 0000 0074 6573 745f 6475 706c 6963  t-...test_duplic
-00005040: 6174 696f 6e5f 6368 696c 6472 656e 5f61  ation_children_a
-00005050: 6c6c 5f69 6e5f 686f 675f 6368 696c 6472  ll_in_hog_childr
-00005060: 656e fb01 0000 730a 0000 0000 0216 0213  en....s.........
-00005070: 0210 0210 0128 1200 0000 520f 0000 0052  .....(....R....R
-00005080: 8800 0000 5213 0000 0052 1a00 0000 5222  ....R....R....R"
-00005090: 0000 0052 3900 0000 5294 0000 0052 4900  ...R9...R....RI.
-000050a0: 0000 5254 0000 0052 5c00 0000 527c 0000  ..RT...R\...R|..
-000050b0: 0052 8100 0000 5282 0000 0052 8700 0000  .R....R....R....
-000050c0: 52be 0000 0052 c500 0000 52c8 0000 0052  R....R....R....R
-000050d0: d000 0000 2800 0000 0028 0000 0000 2800  ....(....(....(.
-000050e0: 0000 0073 4f00 0000 2f55 7365 7273 2f61  ...sO.../Users/a
-000050f0: 646d 696e 2f57 6f72 6b2f 7072 6f6a 6563  dmin/Work/projec
-00005100: 742f 4465 7373 696d 6f7a 2f70 7968 616d  t/Dessimoz/pyham
-00005110: 2d64 6576 2f70 7968 616d 2f74 6573 7473  -dev/pyham/tests
-00005120: 2f74 6573 745f 6f72 7468 6f78 6d6c 7061  /test_orthoxmlpa
-00005130: 7273 6572 2e70 7952 8900 0000 a900 0000  rser.pyR........
-00005140: 7320 0000 0006 0109 0a09 0909 0509 1009  s ..............
-00005150: 0b09 0d09 0c09 0c09 2909 1a09 1609 1e09  ........).......
-00005160: 2209 3109 2f74 3300 0000 4f72 7468 6f58  ".1./t3...OrthoX
-00005170: 4d4c 5061 7273 6572 5f57 6569 7264 5f45  MLParser_Weird_E
-00005180: 6c65 6d65 6e74 5f49 6e5f 6475 706c 6963  lement_In_duplic
-00005190: 6174 696f 6e43 6869 6c64 7265 6e63 0000  ationChildrenc..
-000051a0: 0000 0000 0000 0100 0000 4200 0000 731a  ..........B...s.
-000051b0: 0000 0065 0000 5a01 0064 0000 8400 005a  ...e..Z..d.....Z
-000051c0: 0200 6401 0084 0000 5a03 0052 5328 0200  ..d.....Z..RS(..
-000051d0: 0000 6301 0000 0004 0000 0009 0000 0043  ..c............C
-000051e0: 0000 0073 8200 0000 7400 006a 0100 6a02  ...s....t..j..j.
-000051f0: 0074 0000 6a01 006a 0300 7404 0083 0100  .t..j..j..t.....
-00005200: 6401 0083 0200 7d01 0074 0500 6a06 007c  d.....}..t..j..|
-00005210: 0100 6402 0064 0300 8301 017d 0200 7400  ..d..d.....}..t.
-00005220: 006a 0100 6a02 0074 0000 6a01 006a 0300  .j..j..t..j..j..
-00005230: 7404 0083 0100 6404 0083 0200 7d03 0074  t.....d.....}..t
-00005240: 0700 6a08 0064 0500 7c02 0064 0600 7c03  ..j..d..|..d..|.
-00005250: 0064 0700 6408 0064 0900 7409 0083 0004  .d..d..d..t.....
-00005260: 7c00 005f 0a00 6400 0053 280a 0000 004e  |.._..d..S(....N
-00005270: 7319 0000 002e 2f64 6174 612f 7061 7273  s...../data/pars
-00005280: 6572 2f74 7265 652e 6e65 7769 636b 5210  er/tree.newickR.
-00005290: 0000 0052 2300 0000 7334 0000 002e 2f64  ...R#...s4..../d
-000052a0: 6174 612f 7061 7273 6572 2f63 6f6e 666c  ata/parser/confl
-000052b0: 6963 745f 6475 706c 6963 6174 696f 6e5f  ict_duplication_
-000052c0: 6368 696c 6472 656e 2e6f 7274 686f 786d  children.orthoxm
-000052d0: 6c52 2400 0000 5225 0000 0052 2600 0000  lR$...R%...R&...
-000052e0: 5227 0000 0052 2800 0000 280b 0000 0052  R'...R(...(....R
-000052f0: 2900 0000 522a 0000 0052 2b00 0000 522c  )...R*...R+...R,
-00005300: 0000 0052 2d00 0000 5202 0000 0052 2e00  ...R-...R....R..
-00005310: 0000 5200 0000 0052 2f00 0000 5230 0000  ..R....R/...R0..
-00005320: 0052 3100 0000 2804 0000 0052 1100 0000  .R1...(....R....
-00005330: 5236 0000 0052 3700 0000 5238 0000 0028  R6...R7...R8...(
-00005340: 0000 0000 2800 0000 0073 4f00 0000 2f55  ....(....sO.../U
-00005350: 7365 7273 2f61 646d 696e 2f57 6f72 6b2f  sers/admin/Work/
-00005360: 7072 6f6a 6563 742f 4465 7373 696d 6f7a  project/Dessimoz
-00005370: 2f70 7968 616d 2d64 6576 2f70 7968 616d  /pyham-dev/pyham
-00005380: 2f74 6573 7473 2f74 6573 745f 6f72 7468  /tests/test_orth
-00005390: 6f78 6d6c 7061 7273 6572 2e70 7952 3900  oxmlparser.pyR9.
-000053a0: 0000 0902 0000 730a 0000 0000 0221 0115  ......s......!..
-000053b0: 0121 021b 0163 0100 0000 0500 0000 0700  .!...c..........
-000053c0: 0000 4300 0000 7373 0000 0078 6c00 7c00  ..C...ss...xl.|.
-000053d0: 006a 0000 6a01 0083 0000 445d 5b00 7d01  .j..j.....D][.}.
-000053e0: 0078 5200 7c01 006a 0200 8300 0044 5d44  .xR.|..j.....D]D
-000053f0: 007d 0200 783b 007c 0200 6a03 0044 5d30  .}..x;.|..j..D]0
-00005400: 007d 0300 7827 007c 0300 6a04 0044 5d1c  .}..x'.|..j..D].
-00005410: 007d 0400 7c00 006a 0500 7c04 007c 0200  .}..|..j..|..|..
-00005420: 6a04 006b 0600 8301 0001 7143 0057 7133  j..k......qC.Wq3
-00005430: 0057 7123 0057 7110 0057 6400 0053 2801  .Wq#.Wq..Wd..S(.
-00005440: 0000 004e 2806 0000 0052 3100 0000 52c9  ...N(....R1...R.
-00005450: 0000 0052 ca00 0000 52cb 0000 0052 1400  ...R....R....R..
-00005460: 0000 5285 0000 0028 0500 0000 5211 0000  ..R....(....R...
-00005470: 0052 cc00 0000 52cd 0000 0052 ce00 0000  .R....R....R....
-00005480: 52cf 0000 0028 0000 0000 2800 0000 0073  R....(....(....s
-00005490: 4f00 0000 2f55 7365 7273 2f61 646d 696e  O.../Users/admin
-000054a0: 2f57 6f72 6b2f 7072 6f6a 6563 742f 4465  /Work/project/De
-000054b0: 7373 696d 6f7a 2f70 7968 616d 2d64 6576  ssimoz/pyham-dev
-000054c0: 2f70 7968 616d 2f74 6573 7473 2f74 6573  /pyham/tests/tes
-000054d0: 745f 6f72 7468 6f78 6d6c 7061 7273 6572  t_orthoxmlparser
-000054e0: 2e70 7952 d000 0000 1202 0000 730a 0000  .pyR........s...
-000054f0: 0000 0216 0213 0210 0210 0128 0400 0000  ...........(....
-00005500: 520f 0000 0052 8800 0000 5239 0000 0052  R....R....R9...R
-00005510: d000 0000 2800 0000 0028 0000 0000 2800  ....(....(....(.
-00005520: 0000 0073 4f00 0000 2f55 7365 7273 2f61  ...sO.../Users/a
-00005530: 646d 696e 2f57 6f72 6b2f 7072 6f6a 6563  dmin/Work/projec
-00005540: 742f 4465 7373 696d 6f7a 2f70 7968 616d  t/Dessimoz/pyham
-00005550: 2d64 6576 2f70 7968 616d 2f74 6573 7473  -dev/pyham/tests
-00005560: 2f74 6573 745f 6f72 7468 6f78 6d6c 7061  /test_orthoxmlpa
-00005570: 7273 6572 2e70 7952 d100 0000 0702 0000  rser.pyR........
-00005580: 7304 0000 0006 0209 0974 0800 0000 5f5f  s........t....__
-00005590: 6d61 696e 5f5f 2810 0000 0052 4100 0000  main__(....RA...
-000055a0: 7408 0000 0075 6e69 7474 6573 7452 8f00  t....unittestR..
-000055b0: 0000 5200 0000 0052 0100 0000 5202 0000  ..R....R....R...
-000055c0: 0052 2900 0000 7405 0000 006e 756d 7079  .R)...t....numpy
-000055d0: 7402 0000 006e 7052 0300 0000 7408 0000  t....npR....t...
-000055e0: 0054 6573 7443 6173 6552 0400 0000 5289  .TestCaseR....R.
-000055f0: 0000 0052 d100 0000 520f 0000 0074 0400  ...R....R....t..
-00005600: 0000 6d61 696e 2800 0000 0028 0000 0000  ..main(....(....
-00005610: 2800 0000 0073 4f00 0000 2f55 7365 7273  (....sO.../Users
-00005620: 2f61 646d 696e 2f57 6f72 6b2f 7072 6f6a  /admin/Work/proj
-00005630: 6563 742f 4465 7373 696d 6f7a 2f70 7968  ect/Dessimoz/pyh
-00005640: 616d 2d64 6576 2f70 7968 616d 2f74 6573  am-dev/pyham/tes
-00005650: 7473 2f74 6573 745f 6f72 7468 6f78 6d6c  ts/test_orthoxml
-00005660: 7061 7273 6572 2e70 7974 0800 0000 3c6d  parser.pyt....<m
-00005670: 6f64 756c 653e 0100 0000 731a 0000 000c  odule>....s.....
-00005680: 010c 0110 0110 0110 010c 010c 0110 0319  ................
-00005690: 9e19 ff00 5f19 1b0c 01                   ...._....
+00000050: 0400 5a04 0001 6400 0064 0100 6c05 005a  ..Z...d..d..l..Z
+00000060: 0500 6400 0064 0400 6c01 006d 0600 5a06  ..d..d..l..m..Z.
+00000070: 0001 6405 0065 0100 6a07 0066 0100 6406  ..d..e..j..f..d.
+00000080: 0084 0000 8300 0059 5a08 0064 0700 6501  .......YZ..d..e.
+00000090: 006a 0700 6601 0064 0800 8400 0083 0000  .j..f..d........
+000000a0: 595a 0900 650a 0064 0900 6b02 0072 9f00  YZ..e..d..k..r..
+000000b0: 6501 006a 0b00 8300 0001 6e00 0064 0100  e..j......n..d..
+000000c0: 5328 0a00 0000 69ff ffff ff4e 2801 0000  S(....i....N(...
+000000d0: 0074 0300 0000 6861 6d28 0100 0000 7405  .t....ham(....t.
+000000e0: 0000 0075 7469 6c73 2801 0000 0074 0400  ...utils(....t..
+000000f0: 0000 736b 6970 7412 0000 004f 7274 686f  ..skipt....Ortho
+00000100: 584d 4c50 6172 7365 7254 6573 7463 0000  XMLParserTestc..
+00000110: 0000 0000 0000 0100 0000 4200 0000 736b  ..........B...sk
+00000120: 0000 0065 0000 5a01 0064 0000 8400 005a  ...e..Z..d.....Z
+00000130: 0200 6401 0084 0000 5a03 0064 0200 8400  ..d.....Z..d....
+00000140: 005a 0400 6403 0084 0000 5a05 0064 0400  .Z..d.....Z..d..
+00000150: 8400 005a 0600 6405 0084 0000 5a07 0064  ...Z..d.....Z..d
+00000160: 0600 8400 005a 0800 6407 0084 0000 5a09  .....Z..d.....Z.
+00000170: 0064 0800 8400 005a 0a00 6409 0084 0000  .d.....Z..d.....
+00000180: 5a0b 0064 0a00 8400 005a 0c00 5253 280b  Z..d.....Z..RS(.
+00000190: 0000 0063 0200 0000 0200 0000 0500 0000  ...c............
+000001a0: 4300 0000 736c 0000 0074 0000 7c01 0074  C...sl...t..|..t
+000001b0: 0100 6a02 006a 0300 8302 0072 1c00 7c01  ..j..j.....r..|.
+000001c0: 006a 0400 5374 0000 7c01 0074 0100 6a02  .j..St..|..t..j.
+000001d0: 006a 0500 8302 0072 3e00 7c01 006a 0600  .j.....r>.|..j..
+000001e0: 6a07 006a 0800 5374 0900 6401 006a 0a00  j..j..St..d..j..
+000001f0: 7401 006a 0200 6a0b 006a 0c00 740d 007c  t..j..j..j..t..|
+00000200: 0100 8301 006a 0c00 8302 0083 0100 8201  .....j..........
+00000210: 0064 0000 5328 0200 0000 4e73 2300 0000  .d..S(....Ns#...
+00000220: 6578 7065 6374 2073 7562 636c 6173 7320  expect subclass 
+00000230: 6f62 6a20 6f66 2027 7b7d 272c 2067 6f74  obj of '{}', got
+00000240: 207b 7d28 0e00 0000 740a 0000 0069 7369   {}(....t....isi
+00000250: 6e73 7461 6e63 6552 0000 0000 740c 0000  nstanceR....t...
+00000260: 0061 6273 7472 6163 7467 656e 6574 0400  .abstractgenet..
+00000270: 0000 4765 6e65 7409 0000 0075 6e69 7175  ..Genet....uniqu
+00000280: 655f 6964 7403 0000 0048 4f47 7406 0000  e_idt....HOGt...
+00000290: 0067 656e 6f6d 6574 0500 0000 7461 786f  .genomet....taxo
+000002a0: 6e74 0400 0000 6e61 6d65 7409 0000 0054  nt....namet....T
+000002b0: 7970 6545 7272 6f72 7406 0000 0066 6f72  ypeErrort....for
+000002c0: 6d61 7474 0c00 0000 4162 7374 7261 6374  matt....Abstract
+000002d0: 4765 6e65 7408 0000 005f 5f6e 616d 655f  Genet....__name_
+000002e0: 5f74 0400 0000 7479 7065 2802 0000 0074  _t....type(....t
+000002f0: 0400 0000 7365 6c66 7404 0000 0069 7465  ....selft....ite
+00000300: 6d28 0000 0000 2800 0000 0073 3c00 0000  m(....(....s<...
+00000310: 2f55 7365 7273 2f61 6472 6961 616c 2f52  /Users/adriaal/R
+00000320: 6570 6f73 6974 6f72 6965 732f 4841 4d2f  epositories/HAM/
+00000330: 7465 7374 732f 7465 7374 5f6f 7274 686f  tests/test_ortho
+00000340: 786d 6c70 6172 7365 722e 7079 740f 0000  xmlparser.pyt...
+00000350: 005f 6765 745f 6964 656e 7469 6669 6572  ._get_identifier
+00000360: 0a00 0000 730e 0000 0000 0115 0107 0115  ....s...........
+00000370: 010d 0209 010c 0163 0300 0000 0500 0000  .......c........
+00000380: 0300 0000 4300 0000 735d 0000 0067 0000  ....C...s]...g..
+00000390: 7d03 0078 3600 7c01 006a 0000 445d 2b00  }..x6.|..j..D]+.
+000003a0: 7d04 007c 0000 6a01 007c 0400 8301 007c  }..|..j..|.....|
+000003b0: 0200 6b02 0072 1000 7c03 006a 0200 7c04  ..k..r..|..j..|.
+000003c0: 0083 0100 0171 1000 7110 0057 7403 007c  .....q..q..Wt..|
+000003d0: 0300 8301 0064 0100 6b02 0072 5900 7c03  .....d..k..rY.|.
+000003e0: 0064 0200 1953 7c03 0053 2803 0000 004e  .d...S|..S(....N
+000003f0: 6901 0000 0069 0000 0000 2804 0000 0074  i....i....(....t
+00000400: 0800 0000 6368 696c 6472 656e 5213 0000  ....childrenR...
+00000410: 0074 0600 0000 6170 7065 6e64 7403 0000  .t....appendt...
+00000420: 006c 656e 2805 0000 0052 1100 0000 5212  .len(....R....R.
+00000430: 0000 0074 0500 0000 7175 6572 7974 1000  ...t....queryt..
+00000440: 0000 666f 756e 6465 645f 6368 696c 6472  ..founded_childr
+00000450: 656e 7405 0000 0063 6869 6c64 2800 0000  ent....child(...
+00000460: 0028 0000 0000 733c 0000 002f 5573 6572  .(....s<.../User
+00000470: 732f 6164 7269 6161 6c2f 5265 706f 7369  s/adriaal/Reposi
+00000480: 746f 7269 6573 2f48 414d 2f74 6573 7473  tories/HAM/tests
+00000490: 2f74 6573 745f 6f72 7468 6f78 6d6c 7061  /test_orthoxmlpa
+000004a0: 7273 6572 2e70 7974 1800 0000 5f67 6574  rser.pyt...._get
+000004b0: 5f63 6869 6c64 5f62 795f 6964 656e 7469  _child_by_identi
+000004c0: 6669 6572 1400 0000 730e 0000 0000 0106  fier....s.......
+000004d0: 0110 0115 0114 0112 0108 0163 0300 0000  ...........c....
+000004e0: 0400 0000 0400 0000 0300 0000 734b 0000  ............sK..
+000004f0: 0074 0000 7401 007c 0200 8301 0083 0100  .t..t..|........
+00000500: 7d02 0074 0000 7401 0087 0000 6601 0064  }..t..t.....f..d
+00000510: 0100 8600 007c 0100 6a02 0044 8301 0083  .....|..j..D....
+00000520: 0100 8301 007d 0300 8800 006a 0300 7c02  .....}.....j..|.
+00000530: 007c 0300 8302 0001 6400 0053 2802 0000  .|......d..S(...
+00000540: 004e 6301 0000 0002 0000 0003 0000 0033  .Nc............3
+00000550: 0000 0073 1e00 0000 7c00 005d 1400 7d01  ...s....|..]..}.
+00000560: 0088 0000 6a00 007c 0100 8301 0056 0171  ....j..|.....V.q
+00000570: 0300 6400 0053 2801 0000 004e 2801 0000  ..d..S(....N(...
+00000580: 0052 1300 0000 2802 0000 0074 0200 0000  .R....(....t....
+00000590: 2e30 5212 0000 0028 0100 0000 5211 0000  .0R....(....R...
+000005a0: 0028 0000 0000 733c 0000 002f 5573 6572  .(....s<.../User
+000005b0: 732f 6164 7269 6161 6c2f 5265 706f 7369  s/adriaal/Reposi
+000005c0: 746f 7269 6573 2f48 414d 2f74 6573 7473  tories/HAM/tests
+000005d0: 2f74 6573 745f 6f72 7468 6f78 6d6c 7061  /test_orthoxmlpa
+000005e0: 7273 6572 2e70 7973 0900 0000 3c67 656e  rser.pys....<gen
+000005f0: 6578 7072 3e1f 0000 0073 0200 0000 0600  expr>....s......
+00000600: 2804 0000 0074 0600 0000 736f 7274 6564  (....t....sorted
+00000610: 7404 0000 006c 6973 7452 1400 0000 740b  t....listR....t.
+00000620: 0000 0061 7373 6572 7445 7175 616c 2804  ...assertEqual(.
+00000630: 0000 0052 1100 0000 7403 0000 0068 6f67  ...R....t....hog
+00000640: 7410 0000 0065 7870 6563 7465 645f 6d65  t....expected_me
+00000650: 6d62 6572 7374 1000 0000 6f62 7365 7276  mberst....observ
+00000660: 6564 5f6d 656d 6265 7273 2800 0000 0028  ed_members(....(
+00000670: 0100 0000 5211 0000 0073 3c00 0000 2f55  ....R....s<.../U
+00000680: 7365 7273 2f61 6472 6961 616c 2f52 6570  sers/adriaal/Rep
+00000690: 6f73 6974 6f72 6965 732f 4841 4d2f 7465  ositories/HAM/te
+000006a0: 7374 732f 7465 7374 5f6f 7274 686f 786d  sts/test_orthoxm
+000006b0: 6c70 6172 7365 722e 7079 741b 0000 005f  lparser.pyt...._
+000006c0: 6368 6563 6b5f 6368 696c 6472 656e 5f63  check_children_c
+000006d0: 6f6e 7369 7374 656e 6379 1d00 0000 7306  onsistency....s.
+000006e0: 0000 0000 0112 0125 0163 0100 0000 0400  .......%.c......
+000006f0: 0000 0900 0000 4300 0000 73a6 0000 0074  ......C...s....t
+00000700: 0000 6a01 006a 0200 7400 006a 0100 6a03  ..j..j..t..j..j.
+00000710: 0074 0400 8301 0064 0100 8302 007d 0100  .t.....d.....}..
+00000720: 7405 006a 0600 7c01 0064 0200 6403 0083  t..j..|..d..d...
+00000730: 0101 7d02 0074 0000 6a01 006a 0200 7400  ..}..t..j..j..t.
+00000740: 006a 0100 6a03 0074 0400 8301 0064 0400  .j..j..t.....d..
+00000750: 8302 007d 0300 7407 006a 0800 6405 007c  ...}..t..j..d..|
+00000760: 0200 6406 007c 0300 6407 0064 0800 6409  ..d..|..d..d..d.
+00000770: 0074 0900 8300 047c 0000 5f0a 007c 0000  .t.....|.._..|..
+00000780: 6a0a 006a 0b00 8300 007c 0000 5f0c 007c  j..j.....|.._..|
+00000790: 0000 6a0a 006a 0d00 8300 007c 0000 5f0e  ..j..j.....|.._.
+000007a0: 0064 0000 5328 0a00 0000 4e73 1300 0000  .d..S(....Ns....
+000007b0: 2e2f 6461 7461 2f73 696d 706c 6545 782e  ./data/simpleEx.
+000007c0: 6e77 6b52 1000 0000 7403 0000 006e 776b  nwkR....t....nwk
+000007d0: 7318 0000 002e 2f64 6174 612f 7369 6d70  s...../data/simp
+000007e0: 6c65 4578 2e6f 7274 686f 786d 6c74 0900  leEx.orthoxmlt..
+000007f0: 0000 7472 6565 5f66 696c 6574 0800 0000  ..tree_filet....
+00000800: 686f 675f 6669 6c65 740d 0000 0074 7970  hog_filet....typ
+00000810: 655f 686f 675f 6669 6c65 7408 0000 006f  e_hog_filet....o
+00000820: 7274 686f 786d 6c74 1100 0000 7573 655f  rthoxmlt....use_
+00000830: 696e 7465 726e 616c 5f6e 616d 6528 0f00  internal_name(..
+00000840: 0000 7402 0000 006f 7374 0400 0000 7061  ..t....ost....pa
+00000850: 7468 7404 0000 006a 6f69 6e74 0700 0000  tht....joint....
+00000860: 6469 726e 616d 6574 0800 0000 5f5f 6669  dirnamet....__fi
+00000870: 6c65 5f5f 5201 0000 0074 1100 0000 6765  le__R....t....ge
+00000880: 745f 6e65 7769 636b 5f73 7472 696e 6752  t_newick_stringR
+00000890: 0000 0000 7403 0000 0048 616d 7404 0000  ....t....Hamt...
+000008a0: 0054 7275 6574 0c00 0000 6861 6d5f 616e  .Truet....ham_an
+000008b0: 616c 7973 6973 7417 0000 0067 6574 5f64  alysist....get_d
+000008c0: 6963 745f 746f 705f 6c65 7665 6c5f 686f  ict_top_level_ho
+000008d0: 6773 7404 0000 0068 6f67 7374 1500 0000  gst....hogst....
+000008e0: 6765 745f 6469 6374 5f65 7874 616e 745f  get_dict_extant_
+000008f0: 6765 6e65 7374 0500 0000 6765 6e65 7328  genest....genes(
+00000900: 0400 0000 5211 0000 0074 0800 0000 6e77  ....R....t....nw
+00000910: 6b5f 7061 7468 7407 0000 006e 776b 5f73  k_patht....nwk_s
+00000920: 7472 740d 0000 006f 7274 686f 786d 6c5f  trt....orthoxml_
+00000930: 7061 7468 2800 0000 0028 0000 0000 733c  path(....(....s<
+00000940: 0000 002f 5573 6572 732f 6164 7269 6161  .../Users/adriaa
+00000950: 6c2f 5265 706f 7369 746f 7269 6573 2f48  l/Repositories/H
+00000960: 414d 2f74 6573 7473 2f74 6573 745f 6f72  AM/tests/test_or
+00000970: 7468 6f78 6d6c 7061 7273 6572 2e70 7974  thoxmlparser.pyt
+00000980: 0500 0000 7365 7455 7022 0000 0073 0e00  ....setUp"...s..
+00000990: 0000 0001 2101 1501 2102 1b01 0c01 1201  ....!...!.......
+000009a0: 6301 0000 0004 0000 000d 0000 0043 0000  c............C..
+000009b0: 0073 8000 0000 7400 0064 0100 6402 0064  .s....t..d..d..d
+000009c0: 0300 6402 0064 0400 6402 0064 0500 6406  ..d..d..d..d..d.
+000009d0: 0064 0700 6408 0064 0900 6406 0083 0006  .d..d..d..d.....
+000009e0: 7d01 0074 0100 6a02 0074 0300 8301 007d  }..t..j..t.....}
+000009f0: 0200 782d 007c 0000 6a04 006a 0500 8300  ..x-.|..j..j....
+00000a00: 0044 5d1c 007d 0300 7c02 007c 0300 6a06  .D]..}..|..|..j.
+00000a10: 006a 0700 6302 0019 640a 0037 033c 714c  .j..c...d..7.<qL
+00000a20: 0057 7c00 006a 0800 7c02 007c 0100 8302  .W|..j..|..|....
+00000a30: 0001 6400 0053 280b 0000 004e 7405 0000  ..d..S(....Nt...
+00000a40: 0048 554d 414e 6904 0000 0074 0500 0000  .HUMANi....t....
+00000a50: 5041 4e54 5274 0500 0000 4d4f 5553 4574  PANTRt....MOUSEt
+00000a60: 0500 0000 5241 544e 4f69 0200 0000 7405  ....RATNOi....t.
+00000a70: 0000 0043 414e 4641 6903 0000 0074 0500  ...CANFAi....t..
+00000a80: 0000 5845 4e54 5269 0100 0000 2809 0000  ..XENTRi....(...
+00000a90: 0074 0400 0000 6469 6374 740b 0000 0063  .t....dictt....c
+00000aa0: 6f6c 6c65 6374 696f 6e73 740b 0000 0064  ollectionst....d
+00000ab0: 6566 6175 6c74 6469 6374 7403 0000 0069  efaultdictt....i
+00000ac0: 6e74 5235 0000 0074 0600 0000 7661 6c75  ntR5...t....valu
+00000ad0: 6573 5209 0000 0052 0b00 0000 740f 0000  esR....R....t...
+00000ae0: 0061 7373 6572 7444 6963 7445 7175 616c  .assertDictEqual
+00000af0: 2804 0000 0052 1100 0000 740d 0000 0065  (....R....t....e
+00000b00: 7870 6563 7465 645f 636e 7473 740d 0000  xpected_cntst...
+00000b10: 006f 6273 6572 7665 645f 636e 7473 7401  .observed_cntst.
+00000b20: 0000 0067 2800 0000 0028 0000 0000 733c  ...g(....(....s<
+00000b30: 0000 002f 5573 6572 732f 6164 7269 6161  .../Users/adriaa
+00000b40: 6c2f 5265 706f 7369 746f 7269 6573 2f48  l/Repositories/H
+00000b50: 414d 2f74 6573 7473 2f74 6573 745f 6f72  AM/tests/test_or
+00000b60: 7468 6f78 6d6c 7061 7273 6572 2e70 7974  thoxmlparser.pyt
+00000b70: 1c00 0000 7465 7374 5f6e 756d 6265 724f  ....test_numberO
+00000b80: 6647 656e 6573 5065 7253 7065 6369 6573  fGenesPerSpecies
+00000b90: 2c00 0000 730c 0000 0000 011e 010f 010f  ,...s...........
+00000ba0: 0116 011a 0163 0100 0000 0500 0000 0600  .....c..........
+00000bb0: 0000 4300 0000 73a5 0000 007c 0000 6a00  ..C...s....|..j.
+00000bc0: 006a 0100 8300 007d 0100 6905 0064 0100  .j.....}..i..d..
+00000bd0: 6402 0036 6403 0064 0400 3664 0500 6406  d..6d..d..6d..d.
+00000be0: 0036 6405 0064 0700 3664 0500 6408 0036  .6d..d..6d..d..6
+00000bf0: 7d02 0069 0500 6409 0064 0200 3664 0900  }..i..d..d..6d..
+00000c00: 6404 0036 6409 0064 0600 3664 0900 6407  d..6d..d..6d..d.
+00000c10: 0036 6409 0064 0800 367d 0300 782d 007c  .6d..d..6}..x-.|
+00000c20: 0100 445d 2500 7d04 007c 0300 7c04 006a  ..D]%.}..|..|..j
+00000c30: 0200 6a03 0063 0200 1974 0400 7c04 006a  ..j..c...t..|..j
+00000c40: 0500 8301 0037 033c 7168 0057 7c00 006a  .....7.<qh.W|..j
+00000c50: 0600 7c02 007c 0300 8302 0001 6400 0053  ..|..|......d..S
+00000c60: 280a 0000 004e 6902 0000 0074 0a00 0000  (....Ni....t....
+00000c70: 5665 7274 6562 7261 7461 6903 0000 0074  Vertebratai....t
+00000c80: 0800 0000 4d61 6d6d 616c 6961 6904 0000  ....Mammaliai...
+00000c90: 0074 1000 0000 4575 6172 6368 6f6e 746f  .t....Euarchonto
+00000ca0: 676c 6972 6573 7407 0000 0052 6f64 656e  glirest....Roden
+00000cb0: 7473 7408 0000 0050 7269 6d61 7465 7369  tst....Primatesi
+00000cc0: 0000 0000 2807 0000 0052 3100 0000 741a  ....(....R1...t.
+00000cd0: 0000 0067 6574 5f6c 6973 745f 616e 6365  ...get_list_ance
+00000ce0: 7374 7261 6c5f 6765 6e6f 6d65 7352 0a00  stral_genomesR..
+00000cf0: 0000 520b 0000 0052 1600 0000 5235 0000  ..R....R....R5..
+00000d00: 0052 4500 0000 2805 0000 0052 1100 0000  .RE...(....R....
+00000d10: 7403 0000 0061 6773 7410 0000 0065 7870  t....agst....exp
+00000d20: 6563 7465 645f 6e75 6d62 6572 7374 1000  ected_numberst..
+00000d30: 0000 6f62 7365 7276 6564 5f6e 756d 6265  ..observed_numbe
+00000d40: 7273 7402 0000 0061 6728 0000 0000 2800  rst....ag(....(.
+00000d50: 0000 0073 3c00 0000 2f55 7365 7273 2f61  ...s<.../Users/a
+00000d60: 6472 6961 616c 2f52 6570 6f73 6974 6f72  driaal/Repositor
+00000d70: 6965 732f 4841 4d2f 7465 7374 732f 7465  ies/HAM/tests/te
+00000d80: 7374 5f6f 7274 686f 786d 6c70 6172 7365  st_orthoxmlparse
+00000d90: 722e 7079 7424 0000 0074 6573 745f 6e75  r.pyt$...test_nu
+00000da0: 6d62 6572 5f68 6f67 5f70 6572 5f61 6e63  mber_hog_per_anc
+00000db0: 6573 7472 616c 5f67 656e 6f6d 6534 0000  estral_genome4..
+00000dc0: 0073 0c00 0000 0001 0f01 2901 2901 0d01  .s........).)...
+00000dd0: 2301 6301 0000 0001 0000 0007 0000 0043  #.c............C
+00000de0: 0000 0073 7800 0000 7c00 006a 0000 7c00  ...sx...|..j..|.
+00000df0: 006a 0100 6401 0019 6a02 0064 0200 8301  .j..d...j..d....
+00000e00: 0064 0300 8302 0001 7c00 006a 0300 7404  .d......|..j..t.
+00000e10: 0083 0100 8f19 0001 7c00 006a 0100 6404  ........|..j..d.
+00000e20: 0019 6a02 0064 0200 8301 0001 5764 0000  ..j..d......Wd..
+00000e30: 5158 7c00 006a 0300 7404 0083 0100 8f19  QX|..j..t.......
+00000e40: 0001 7c00 006a 0100 6401 0019 6a02 0064  ..|..j..d...j..d
+00000e50: 0500 8301 0001 5764 0000 5158 6400 0053  ......Wd..QXd..S
+00000e60: 2806 0000 004e 7401 0000 0031 740b 0000  (....Nt....1t...
+00000e70: 0063 6f6e 7369 7374 656e 6379 6901 0000  .consistencyi...
+00000e80: 0074 0100 0000 3274 0800 0000 636f 7665  .t....2t....cove
+00000e90: 7261 6765 2805 0000 0052 1e00 0000 5233  rage(....R....R3
+00000ea0: 0000 0074 0500 0000 7363 6f72 6574 0c00  ...t....scoret..
+00000eb0: 0000 6173 7365 7274 5261 6973 6573 7408  ..assertRaisest.
+00000ec0: 0000 004b 6579 4572 726f 7228 0100 0000  ...KeyError(....
+00000ed0: 5211 0000 0028 0000 0000 2800 0000 0073  R....(....(....s
+00000ee0: 3c00 0000 2f55 7365 7273 2f61 6472 6961  <.../Users/adria
+00000ef0: 616c 2f52 6570 6f73 6974 6f72 6965 732f  al/Repositories/
+00000f00: 4841 4d2f 7465 7374 732f 7465 7374 5f6f  HAM/tests/test_o
+00000f10: 7274 686f 786d 6c70 6172 7365 722e 7079  rthoxmlparser.py
+00000f20: 7417 0000 0074 6573 745f 7363 6f72 6573  t....test_scores
+00000f30: 5f6f 6e5f 746f 706c 6576 656c 3c00 0000  _on_toplevel<...
+00000f40: 730a 0000 0000 0120 0110 011a 0110 0163  s...... .......c
+00000f50: 0100 0000 0d00 0000 0700 0000 4300 0000  ............C...
+00000f60: 7306 0100 007c 0000 6a00 0064 0100 197d  s....|..j..d...}
+00000f70: 0100 7c00 006a 0000 6402 0019 7d02 007c  ..|..j..d...}..|
+00000f80: 0000 6a00 0064 0300 197d 0300 6404 0064  ..j..d...}..d..d
+00000f90: 0500 6401 0064 0600 6407 0064 0800 6806  ..d..d..d..d..h.
+00000fa0: 007d 0400 6409 0064 0a00 6402 0064 0b00  .}..d..d..d..d..
+00000fb0: 6804 007d 0500 6403 0064 0c00 640d 0064  h..}..d..d..d..d
+00000fc0: 0e00 640f 0064 1000 6411 0068 0700 7d06  ..d..d..d..h..}.
+00000fd0: 007c 0100 6a01 0083 0000 7d07 007c 0200  .|..j.....}..|..
+00000fe0: 6a01 0083 0000 7d08 007c 0300 6a01 0083  j.....}..|..j...
+00000ff0: 0000 7d09 0074 0200 6412 0084 0000 7c07  ..}..t..d.....|.
+00001000: 0044 8301 0083 0100 7d0a 0074 0200 6413  .D......}..t..d.
+00001010: 0084 0000 7c08 0044 8301 0083 0100 7d0b  ....|..D......}.
+00001020: 0074 0200 6414 0084 0000 7c09 0044 8301  .t..d.....|..D..
+00001030: 0083 0100 7d0c 007c 0000 6a03 007c 0400  ....}..|..j..|..
+00001040: 7c0a 0083 0200 017c 0000 6a03 007c 0500  |......|..j..|..
+00001050: 7c0b 0083 0200 017c 0000 6a03 007c 0600  |......|..j..|..
+00001060: 7c0c 0083 0200 0164 0000 5328 1500 0000  |......d..S(....
+00001070: 4e52 5500 0000 5257 0000 0074 0100 0000  NRU...RW...t....
+00001080: 3374 0200 0000 3531 7402 0000 0032 3174  3t....51t....21t
+00001090: 0200 0000 3131 7402 0000 0033 3174 0200  ....11t....31t..
+000010a0: 0000 3431 7402 0000 0032 3274 0200 0000  ..41t....22t....
+000010b0: 3332 7402 0000 0031 3274 0200 0000 3133  32t....12t....13
+000010c0: 7402 0000 0032 3374 0200 0000 3333 7402  t....23t....33t.
+000010d0: 0000 0035 3374 0200 0000 3134 7402 0000  ...53t....14t...
+000010e0: 0033 3463 0100 0000 0200 0000 0200 0000  .34c............
+000010f0: 7300 0000 7318 0000 007c 0000 5d0e 007d  s...s....|..]..}
+00001100: 0100 7c01 006a 0000 5601 7103 0064 0000  ..|..j..V.q..d..
+00001110: 5328 0100 0000 4e28 0100 0000 5207 0000  S(....N(....R...
+00001120: 0028 0200 0000 521b 0000 0074 0100 0000  .(....R....t....
+00001130: 7828 0000 0000 2800 0000 0073 3c00 0000  x(....(....s<...
+00001140: 2f55 7365 7273 2f61 6472 6961 616c 2f52  /Users/adriaal/R
+00001150: 6570 6f73 6974 6f72 6965 732f 4841 4d2f  epositories/HAM/
+00001160: 7465 7374 732f 7465 7374 5f6f 7274 686f  tests/test_ortho
+00001170: 786d 6c70 6172 7365 722e 7079 7309 0000  xmlparser.pys...
+00001180: 003c 6765 6e65 7870 723e 5100 0000 7302  .<genexpr>Q...s.
+00001190: 0000 0006 0063 0100 0000 0200 0000 0200  .....c..........
+000011a0: 0000 7300 0000 7318 0000 007c 0000 5d0e  ..s...s....|..].
+000011b0: 007d 0100 7c01 006a 0000 5601 7103 0064  .}..|..j..V.q..d
+000011c0: 0000 5328 0100 0000 4e28 0100 0000 5207  ..S(....N(....R.
+000011d0: 0000 0028 0200 0000 521b 0000 0052 6c00  ...(....R....Rl.
+000011e0: 0000 2800 0000 0028 0000 0000 733c 0000  ..(....(....s<..
+000011f0: 002f 5573 6572 732f 6164 7269 6161 6c2f  ./Users/adriaal/
+00001200: 5265 706f 7369 746f 7269 6573 2f48 414d  Repositories/HAM
+00001210: 2f74 6573 7473 2f74 6573 745f 6f72 7468  /tests/test_orth
+00001220: 6f78 6d6c 7061 7273 6572 2e70 7973 0900  oxmlparser.pys..
+00001230: 0000 3c67 656e 6578 7072 3e52 0000 0073  ..<genexpr>R...s
+00001240: 0200 0000 0600 6301 0000 0002 0000 0002  ......c.........
+00001250: 0000 0073 0000 0073 1800 0000 7c00 005d  ...s...s....|..]
+00001260: 0e00 7d01 007c 0100 6a00 0056 0171 0300  ..}..|..j..V.q..
+00001270: 6400 0053 2801 0000 004e 2801 0000 0052  d..S(....N(....R
+00001280: 0700 0000 2802 0000 0052 1b00 0000 526c  ....(....R....Rl
+00001290: 0000 0028 0000 0000 2800 0000 0073 3c00  ...(....(....s<.
+000012a0: 0000 2f55 7365 7273 2f61 6472 6961 616c  ../Users/adriaal
+000012b0: 2f52 6570 6f73 6974 6f72 6965 732f 4841  /Repositories/HA
+000012c0: 4d2f 7465 7374 732f 7465 7374 5f6f 7274  M/tests/test_ort
+000012d0: 686f 786d 6c70 6172 7365 722e 7079 7309  hoxmlparser.pys.
+000012e0: 0000 003c 6765 6e65 7870 723e 5300 0000  ...<genexpr>S...
+000012f0: 7302 0000 0006 0028 0400 0000 5233 0000  s......(....R3..
+00001300: 0074 1800 0000 6765 745f 616c 6c5f 6465  .t....get_all_de
+00001310: 7363 656e 6461 6e74 5f67 656e 6573 7403  scendant_genest.
+00001320: 0000 0073 6574 740e 0000 0061 7373 6572  ...sett....asser
+00001330: 7453 6574 4571 7561 6c28 0d00 0000 5211  tSetEqual(....R.
+00001340: 0000 0074 0400 0000 686f 6731 7404 0000  ...t....hog1t...
+00001350: 0068 6f67 3274 0400 0000 686f 6733 7411  .hog2t....hog3t.
+00001360: 0000 0065 7870 6563 7465 644d 656d 6265  ...expectedMembe
+00001370: 7273 5f31 7411 0000 0065 7870 6563 7465  rs_1t....expecte
+00001380: 644d 656d 6265 7273 5f32 7411 0000 0065  dMembers_2t....e
+00001390: 7870 6563 7465 644d 656d 6265 7273 5f33  xpectedMembers_3
+000013a0: 740a 0000 0068 6f67 315f 6765 6e65 7374  t....hog1_genest
+000013b0: 0a00 0000 686f 6732 5f67 656e 6573 740a  ....hog2_genest.
+000013c0: 0000 0068 6f67 335f 6765 6e65 7374 0900  ...hog3_genest..
+000013d0: 0000 6d65 6d62 6572 735f 3174 0900 0000  ..members_1t....
+000013e0: 6d65 6d62 6572 735f 3274 0900 0000 6d65  members_2t....me
+000013f0: 6d62 6572 735f 3328 0000 0000 2800 0000  mbers_3(....(...
+00001400: 0073 3c00 0000 2f55 7365 7273 2f61 6472  .s<.../Users/adr
+00001410: 6961 616c 2f52 6570 6f73 6974 6f72 6965  iaal/Repositorie
+00001420: 732f 4841 4d2f 7465 7374 732f 7465 7374  s/HAM/tests/test
+00001430: 5f6f 7274 686f 786d 6c70 6172 7365 722e  _orthoxmlparser.
+00001440: 7079 7413 0000 0074 6573 745f 686f 675f  pyt....test_hog_
+00001450: 6d65 6d62 6572 7368 6970 4300 0000 731e  membershipC...s.
+00001460: 0000 0000 020d 010d 010d 0218 0112 011b  ................
+00001470: 020c 010c 010c 0216 0116 0116 0210 0110  ................
+00001480: 0163 0100 0000 0600 0000 0400 0000 4300  .c............C.
+00001490: 0000 73e0 0000 007c 0000 6a00 0064 0100  ..s....|..j..d..
+000014a0: 197d 0100 7c00 006a 0100 6402 007c 0100  .}..|..j..d..|..
+000014b0: 6a02 006a 0300 6a04 0083 0200 017c 0000  j..j..j......|..
+000014c0: 6a05 007c 0100 6403 0064 0400 6702 0083  j..|..d..d..g...
+000014d0: 0200 017c 0000 6a06 007c 0100 6404 0083  ...|..j..|..d...
+000014e0: 0200 7d02 007c 0000 6a05 007c 0200 6405  ..}..|..j..|..d.
+000014f0: 0064 0600 6702 0083 0200 017c 0000 6a06  .d..g......|..j.
+00001500: 007c 0200 6406 0083 0200 7d03 007c 0000  .|..d.....}..|..
+00001510: 6a05 007c 0300 6407 0064 0800 6702 0083  j..|..d..d..g...
+00001520: 0200 017c 0000 6a06 007c 0300 6407 0083  ...|..j..|..d...
+00001530: 0200 7d04 007c 0000 6a05 007c 0400 6409  ..}..|..j..|..d.
+00001540: 0064 0a00 6702 0083 0200 017c 0000 6a06  .d..g......|..j.
+00001550: 007c 0300 6408 0083 0200 7d05 007c 0000  .|..d.....}..|..
+00001560: 6a05 007c 0500 6401 0064 0b00 6702 0083  j..|..d..d..g...
+00001570: 0200 0164 0000 5328 0c00 0000 4e52 5500  ...d..S(....NRU.
+00001580: 0000 524a 0000 0052 5e00 0000 524b 0000  ..RJ...R^...RK..
+00001590: 0052 5f00 0000 524c 0000 0052 4d00 0000  .R_...RL...RM...
+000015a0: 524e 0000 0052 6200 0000 5261 0000 0052  RN...Rb...Ra...R
+000015b0: 6000 0000 2807 0000 0052 3300 0000 521e  `...(....R3...R.
+000015c0: 0000 0052 0900 0000 520a 0000 0052 0b00  ...R....R....R..
+000015d0: 0000 5222 0000 0052 1a00 0000 2806 0000  ..R"...R....(...
+000015e0: 0052 1100 0000 5270 0000 0074 0800 0000  .R....Rp...t....
+000015f0: 6d61 6d6d 616c 6961 7410 0000 0065 7561  mammaliat....eua
+00001600: 7263 686f 6e74 6f67 6c69 7265 7374 0700  rchontoglirest..
+00001610: 0000 726f 6465 6e74 7374 0800 0000 7072  ..rodentst....pr
+00001620: 696d 6174 6573 2800 0000 0028 0000 0000  imates(....(....
+00001630: 733c 0000 002f 5573 6572 732f 6164 7269  s<.../Users/adri
+00001640: 6161 6c2f 5265 706f 7369 746f 7269 6573  aal/Repositories
+00001650: 2f48 414d 2f74 6573 7473 2f74 6573 745f  /HAM/tests/test_
+00001660: 6f72 7468 6f78 6d6c 7061 7273 6572 2e70  orthoxmlparser.p
+00001670: 7974 1900 0000 7465 7374 5f73 696d 706c  yt....test_simpl
+00001680: 655f 686f 675f 7374 7275 6374 7572 6559  e_hog_structureY
+00001690: 0000 0073 1600 0000 0002 0d03 1901 1603  ...s............
+000016a0: 1201 1603 1201 1603 1201 1603 1201 6301  ..............c.
+000016b0: 0000 0005 0000 0004 0000 0043 0000 0073  ...........C...s
+000016c0: b500 0000 7c00 006a 0000 6401 0019 7d01  ....|..j..d...}.
+000016d0: 007c 0000 6a01 0064 0200 7c01 006a 0200  .|..j..d..|..j..
+000016e0: 6a03 006a 0400 8302 0001 7c00 006a 0500  j..j......|..j..
+000016f0: 7c01 0064 0300 6404 0067 0200 8302 0001  |..d..d..g......
+00001700: 7c00 006a 0600 7c01 0064 0400 8302 007d  |..j..|..d.....}
+00001710: 0200 7c00 006a 0500 7c02 0064 0500 6406  ..|..j..|..d..d.
+00001720: 0067 0200 8302 0001 7c00 006a 0600 7c02  .g......|..j..|.
+00001730: 0064 0600 8302 007d 0300 7c00 006a 0500  .d.....}..|..j..
+00001740: 7c03 0064 0100 6407 0067 0200 8302 0001  |..d..d..g......
+00001750: 7c00 006a 0600 7c02 0064 0500 8302 007d  |..j..|..d.....}
+00001760: 0400 7c00 006a 0500 7c04 0064 0800 6801  ..|..j..|..d..h.
+00001770: 0083 0200 0164 0000 5328 0900 0000 4e52  .....d..S(....NR
+00001780: 5700 0000 524b 0000 0052 6300 0000 524c  W...RK...Rc...RL
+00001790: 0000 0052 4d00 0000 524e 0000 0052 6500  ...RM...RN...Re.
+000017a0: 0000 5264 0000 0028 0700 0000 5233 0000  ..Rd...(....R3..
+000017b0: 0052 1e00 0000 5209 0000 0052 0a00 0000  .R....R....R....
+000017c0: 520b 0000 0052 2200 0000 521a 0000 0028  R....R"...R....(
+000017d0: 0500 0000 5211 0000 0052 7100 0000 527e  ....R....Rq...R~
+000017e0: 0000 0052 8000 0000 527f 0000 0028 0000  ...R....R....(..
+000017f0: 0000 2800 0000 0073 3c00 0000 2f55 7365  ..(....s<.../Use
+00001800: 7273 2f61 6472 6961 616c 2f52 6570 6f73  rs/adriaal/Repos
+00001810: 6974 6f72 6965 732f 4841 4d2f 7465 7374  itories/HAM/test
+00001820: 732f 7465 7374 5f6f 7274 686f 786d 6c70  s/test_orthoxmlp
+00001830: 6172 7365 722e 7079 7427 0000 0074 6573  arser.pyt'...tes
+00001840: 745f 696e 636f 6d70 6c65 7465 5f6c 696e  t_incomplete_lin
+00001850: 6561 6765 5f74 6178 6f6e 5f65 7870 616e  eage_taxon_expan
+00001860: 7369 6f6e 7100 0000 7312 0000 0000 020d  sionq...s.......
+00001870: 0319 0116 0312 0116 0312 0116 0312 0163  ...............c
+00001880: 0100 0000 0700 0000 0500 0000 4300 0000  ............C...
+00001890: 737f 0100 007c 0000 6a00 0064 0100 197d  s....|..j..d...}
+000018a0: 0100 7c00 006a 0100 6402 007c 0100 6a02  ..|..j..d..|..j.
+000018b0: 006a 0300 6a04 0083 0200 017c 0000 6a05  .j..j......|..j.
+000018c0: 007c 0100 6403 0064 0400 6702 0083 0200  .|..d..d..g.....
+000018d0: 017c 0000 6a06 007c 0100 6a07 0083 0100  .|..j..|..j.....
+000018e0: 017c 0000 6a08 007c 0100 6404 0083 0200  .|..j..|..d.....
+000018f0: 7d02 007c 0000 6a05 007c 0200 6405 0064  }..|..j..|..d..d
+00001900: 0600 6406 0067 0300 8302 0001 7c00 006a  ..d..g......|..j
+00001910: 0600 7c02 006a 0700 8301 0001 7c00 006a  ..|..j......|..j
+00001920: 0800 7c02 0064 0600 8302 007d 0300 78df  ..|..d.....}..x.
+00001930: 007c 0300 445d d700 7d04 007c 0000 6a09  .|..D]..}..|..j.
+00001940: 007c 0400 6a07 0083 0100 017c 0000 6a05  .|..j......|..j.
+00001950: 007c 0400 6407 0064 0800 6702 0083 0200  .|..d..d..g.....
+00001960: 017c 0000 6a08 007c 0400 6407 0083 0200  .|..j..|..d.....
+00001970: 7d05 007c 0000 6a06 007c 0500 6a07 0083  }..|..j..|..j...
+00001980: 0100 017c 0000 6a08 007c 0400 6408 0083  ...|..j..|..d...
+00001990: 0200 7d06 007c 0000 6a06 007c 0600 6a07  ..}..|..j..|..j.
+000019a0: 0083 0100 0174 0a00 7c05 006a 0b00 8301  .....t..|..j....
+000019b0: 0064 0900 6b02 0072 5101 7c00 006a 0500  .d..k..rQ.|..j..
+000019c0: 7c06 0064 0a00 6701 0083 0200 017c 0000  |..d..g......|..
+000019d0: 6a05 007c 0500 6401 0064 0b00 6702 0083  j..|..d..d..g...
+000019e0: 0200 0171 a000 7c00 006a 0500 7c06 0064  ...q..|..j..|..d
+000019f0: 0c00 6701 0083 0200 017c 0000 6a05 007c  ..g......|..j..|
+00001a00: 0500 640d 0067 0100 8302 0001 71a0 0057  ..d..g......q..W
+00001a10: 6400 0053 280e 0000 004e 525d 0000 0052  d..S(....NR]...R
+00001a20: 4a00 0000 5269 0000 0052 4b00 0000 5267  J...Ri...RK...Rg
+00001a30: 0000 0052 4c00 0000 524e 0000 0052 4d00  ...RL...RN...RM.
+00001a40: 0000 6902 0000 0052 6800 0000 5266 0000  ..i....Rh...Rf..
+00001a50: 0052 6b00 0000 526a 0000 0028 0c00 0000  .Rk...Rj...(....
+00001a60: 5233 0000 0052 1e00 0000 5209 0000 0052  R3...R....R....R
+00001a70: 0a00 0000 520b 0000 0052 2200 0000 740b  ....R....R"...t.
+00001a80: 0000 0061 7373 6572 7446 616c 7365 7414  ...assertFalset.
+00001a90: 0000 0061 726f 7365 5f62 795f 6475 706c  ...arose_by_dupl
+00001aa0: 6963 6174 696f 6e52 1a00 0000 740a 0000  icationR....t...
+00001ab0: 0061 7373 6572 7454 7275 6552 1600 0000  .assertTrueR....
+00001ac0: 5214 0000 0028 0700 0000 5211 0000 0052  R....(....R....R
+00001ad0: 7200 0000 527d 0000 0052 7e00 0000 740f  r...R}...R~...t.
+00001ae0: 0000 0065 7561 7263 686f 6e74 6f67 6c69  ...euarchontogli
+00001af0: 7265 5280 0000 0052 7f00 0000 2800 0000  reR....R....(...
+00001b00: 0028 0000 0000 733c 0000 002f 5573 6572  .(....s<.../User
+00001b10: 732f 6164 7269 6161 6c2f 5265 706f 7369  s/adriaal/Reposi
+00001b20: 746f 7269 6573 2f48 414d 2f74 6573 7473  tories/HAM/tests
+00001b30: 2f74 6573 745f 6f72 7468 6f78 6d6c 7061  /test_orthoxmlpa
+00001b40: 7273 6572 2e70 7974 1900 0000 7465 7374  rser.pyt....test
+00001b50: 5f68 6f67 5f77 6974 685f 6475 706c 6963  _hog_with_duplic
+00001b60: 6174 696f 6e85 0000 0073 2800 0000 0002  ation....s(.....
+00001b70: 0d03 1901 1601 1003 1201 1901 1003 1201  ................
+00001b80: 0d01 1001 1603 1201 1001 1201 1002 1501  ................
+00001b90: 1301 1902 1301 280d 0000 0052 0f00 0000  ......(....R....
+00001ba0: 740a 0000 005f 5f6d 6f64 756c 655f 5f52  t....__module__R
+00001bb0: 1300 0000 521a 0000 0052 2200 0000 5239  ....R....R"...R9
+00001bc0: 0000 0052 4900 0000 5254 0000 0052 5c00  ...RI...RT...R\.
+00001bd0: 0000 527c 0000 0052 8100 0000 5282 0000  ..R|...R....R...
+00001be0: 0052 8700 0000 2800 0000 0028 0000 0000  .R....(....(....
+00001bf0: 2800 0000 0073 3c00 0000 2f55 7365 7273  (....s<.../Users
+00001c00: 2f61 6472 6961 616c 2f52 6570 6f73 6974  /adriaal/Reposit
+00001c10: 6f72 6965 732f 4841 4d2f 7465 7374 732f  ories/HAM/tests/
+00001c20: 7465 7374 5f6f 7274 686f 786d 6c70 6172  test_orthoxmlpar
+00001c30: 7365 722e 7079 5203 0000 0009 0000 0073  ser.pyR........s
+00001c40: 1600 0000 0601 090a 0909 0905 090a 0908  ................
+00001c50: 0908 0907 0916 0918 0914 7422 0000 004f  ..........t"...O
+00001c60: 7274 686f 584d 4c50 6172 7365 7254 6573  rthoXMLParserTes
+00001c70: 745f 636f 6d70 6c65 7850 6172 616c 6f67  t_complexParalog
+00001c80: 7363 0000 0000 0000 0000 0100 0000 4200  sc............B.
+00001c90: 0000 738f 0000 0065 0000 5a01 0064 0000  ..s....e..Z..d..
+00001ca0: 8400 005a 0200 6401 0084 0000 5a03 0064  ...Z..d.....Z..d
+00001cb0: 0200 8400 005a 0400 6403 0084 0000 5a05  .....Z..d.....Z.
+00001cc0: 0064 0400 8400 005a 0600 6405 0084 0000  .d.....Z..d.....
+00001cd0: 5a07 0064 0600 8400 005a 0800 6407 0084  Z..d.....Z..d...
+00001ce0: 0000 5a09 0064 0800 8400 005a 0a00 6409  ..Z..d.....Z..d.
+00001cf0: 0084 0000 5a0b 0064 0a00 8400 005a 0c00  ....Z..d.....Z..
+00001d00: 640b 0084 0000 5a0d 0064 0c00 8400 005a  d.....Z..d.....Z
+00001d10: 0e00 640d 0084 0000 5a0f 0064 0e00 8400  ..d.....Z..d....
+00001d20: 005a 1000 5253 280f 0000 0063 0200 0000  .Z..RS(....c....
+00001d30: 0200 0000 0500 0000 4300 0000 736c 0000  ........C...sl..
+00001d40: 0074 0000 7c01 0074 0100 6a02 006a 0300  .t..|..t..j..j..
+00001d50: 8302 0072 1c00 7c01 006a 0400 5374 0000  ...r..|..j..St..
+00001d60: 7c01 0074 0100 6a02 006a 0500 8302 0072  |..t..j..j.....r
+00001d70: 3e00 7c01 006a 0600 6a07 006a 0800 5374  >.|..j..j..j..St
+00001d80: 0900 6401 006a 0a00 7401 006a 0200 6a0b  ..d..j..t..j..j.
+00001d90: 006a 0c00 740d 007c 0100 8301 006a 0c00  .j..t..|.....j..
+00001da0: 8302 0083 0100 8201 0064 0000 5328 0200  .........d..S(..
+00001db0: 0000 4e73 2300 0000 6578 7065 6374 2073  ..Ns#...expect s
+00001dc0: 7562 636c 6173 7320 6f62 6a20 6f66 2027  ubclass obj of '
+00001dd0: 7b7d 272c 2067 6f74 207b 7d28 0e00 0000  {}', got {}(....
+00001de0: 5204 0000 0052 0000 0000 5205 0000 0052  R....R....R....R
+00001df0: 0600 0000 5207 0000 0052 0800 0000 5209  ....R....R....R.
+00001e00: 0000 0052 0a00 0000 520b 0000 0052 0c00  ...R....R....R..
+00001e10: 0000 520d 0000 0052 0e00 0000 520f 0000  ..R....R....R...
+00001e20: 0052 1000 0000 2802 0000 0052 1100 0000  .R....(....R....
+00001e30: 5212 0000 0028 0000 0000 2800 0000 0073  R....(....(....s
+00001e40: 3c00 0000 2f55 7365 7273 2f61 6472 6961  <.../Users/adria
+00001e50: 616c 2f52 6570 6f73 6974 6f72 6965 732f  al/Repositories/
+00001e60: 4841 4d2f 7465 7374 732f 7465 7374 5f6f  HAM/tests/test_o
+00001e70: 7274 686f 786d 6c70 6172 7365 722e 7079  rthoxmlparser.py
+00001e80: 5213 0000 00a8 0000 0073 0e00 0000 0001  R........s......
+00001e90: 1501 0701 1501 0d02 0901 0c01 6303 0000  ............c...
+00001ea0: 0005 0000 0003 0000 0043 0000 0073 5d00  .........C...s].
+00001eb0: 0000 6700 007d 0300 7836 007c 0100 6a00  ..g..}..x6.|..j.
+00001ec0: 0044 5d2b 007d 0400 7c00 006a 0100 7c04  .D]+.}..|..j..|.
+00001ed0: 0083 0100 7c02 006b 0200 7210 007c 0300  ....|..k..r..|..
+00001ee0: 6a02 007c 0400 8301 0001 7110 0071 1000  j..|......q..q..
+00001ef0: 5774 0300 7c03 0083 0100 6401 006b 0200  Wt..|.....d..k..
+00001f00: 7259 007c 0300 6402 0019 537c 0300 5328  rY.|..d...S|..S(
+00001f10: 0300 0000 4e69 0100 0000 6900 0000 0028  ....Ni....i....(
+00001f20: 0400 0000 5214 0000 0052 1300 0000 5215  ....R....R....R.
+00001f30: 0000 0052 1600 0000 2805 0000 0052 1100  ...R....(....R..
+00001f40: 0000 5212 0000 0052 1700 0000 5218 0000  ..R....R....R...
+00001f50: 0052 1900 0000 2800 0000 0028 0000 0000  .R....(....(....
+00001f60: 733c 0000 002f 5573 6572 732f 6164 7269  s<.../Users/adri
+00001f70: 6161 6c2f 5265 706f 7369 746f 7269 6573  aal/Repositories
+00001f80: 2f48 414d 2f74 6573 7473 2f74 6573 745f  /HAM/tests/test_
+00001f90: 6f72 7468 6f78 6d6c 7061 7273 6572 2e70  orthoxmlparser.p
+00001fa0: 7952 1a00 0000 b200 0000 730e 0000 0000  yR........s.....
+00001fb0: 0106 0110 0115 0114 0112 0108 0163 0300  .............c..
+00001fc0: 0000 0400 0000 0400 0000 0300 0000 734b  ..............sK
+00001fd0: 0000 0074 0000 7401 007c 0200 8301 0083  ...t..t..|......
+00001fe0: 0100 7d02 0074 0000 7401 0087 0000 6601  ..}..t..t.....f.
+00001ff0: 0064 0100 8600 007c 0100 6a02 0044 8301  .d.....|..j..D..
+00002000: 0083 0100 8301 007d 0300 8800 006a 0300  .......}.....j..
+00002010: 7c02 007c 0300 8302 0001 6400 0053 2802  |..|......d..S(.
+00002020: 0000 004e 6301 0000 0002 0000 0003 0000  ...Nc...........
+00002030: 0033 0000 0073 1e00 0000 7c00 005d 1400  .3...s....|..]..
+00002040: 7d01 0088 0000 6a00 007c 0100 8301 0056  }.....j..|.....V
+00002050: 0171 0300 6400 0053 2801 0000 004e 2801  .q..d..S(....N(.
+00002060: 0000 0052 1300 0000 2802 0000 0052 1b00  ...R....(....R..
+00002070: 0000 5212 0000 0028 0100 0000 5211 0000  ..R....(....R...
+00002080: 0028 0000 0000 733c 0000 002f 5573 6572  .(....s<.../User
+00002090: 732f 6164 7269 6161 6c2f 5265 706f 7369  s/adriaal/Reposi
+000020a0: 746f 7269 6573 2f48 414d 2f74 6573 7473  tories/HAM/tests
+000020b0: 2f74 6573 745f 6f72 7468 6f78 6d6c 7061  /test_orthoxmlpa
+000020c0: 7273 6572 2e70 7973 0900 0000 3c67 656e  rser.pys....<gen
+000020d0: 6578 7072 3ebd 0000 0073 0200 0000 0600  expr>....s......
+000020e0: 2804 0000 0052 1c00 0000 521d 0000 0052  (....R....R....R
+000020f0: 1400 0000 521e 0000 0028 0400 0000 5211  ....R....(....R.
+00002100: 0000 0052 1f00 0000 5220 0000 0052 2100  ...R....R ...R!.
+00002110: 0000 2800 0000 0028 0100 0000 5211 0000  ..(....(....R...
+00002120: 0073 3c00 0000 2f55 7365 7273 2f61 6472  .s<.../Users/adr
+00002130: 6961 616c 2f52 6570 6f73 6974 6f72 6965  iaal/Repositorie
+00002140: 732f 4841 4d2f 7465 7374 732f 7465 7374  s/HAM/tests/test
+00002150: 5f6f 7274 686f 786d 6c70 6172 7365 722e  _orthoxmlparser.
+00002160: 7079 5222 0000 00bb 0000 0073 0600 0000  pyR".......s....
+00002170: 0001 1201 2501 6301 0000 0005 0000 0009  ....%.c.........
+00002180: 0000 0043 0000 0073 1201 0000 7400 006a  ...C...s....t..j
+00002190: 0100 6a02 0074 0000 6a01 006a 0300 7404  ..j..t..j..j..t.
+000021a0: 0083 0100 6401 0083 0200 7d01 0074 0500  ....d.....}..t..
+000021b0: 6a06 007c 0100 6402 0064 0300 8301 017d  j..|..d..d.....}
+000021c0: 0200 7400 006a 0100 6a02 0074 0000 6a01  ..t..j..j..t..j.
+000021d0: 006a 0300 7404 0083 0100 6404 0083 0200  .j..t.....d.....
+000021e0: 7d03 0074 0000 6a01 006a 0200 7400 006a  }..t..j..j..t..j
+000021f0: 0100 6a03 0074 0400 8301 0064 0500 8302  ..j..t.....d....
+00002200: 007d 0400 7407 006a 0800 6406 007c 0200  .}..t..j..d..|..
+00002210: 6407 007c 0300 6408 0064 0900 640a 0074  d..|..d..d..d..t
+00002220: 0900 8300 047c 0000 5f0a 007c 0000 6a0a  .....|.._..|..j.
+00002230: 006a 0b00 8300 007c 0000 5f0c 007c 0000  .j.....|.._..|..
+00002240: 6a0a 006a 0d00 8300 007c 0000 5f0e 0074  j..j.....|.._..t
+00002250: 0700 6a08 0064 0600 7c02 0064 0700 7c04  ..j..d..|..d..|.
+00002260: 0064 0800 6409 0064 0a00 7409 0083 0004  .d..d..d..t.....
+00002270: 7c00 005f 0f00 7c00 006a 0f00 6a0b 0083  |.._..|..j..j...
+00002280: 0000 7c00 005f 1000 7c00 006a 0f00 6a0d  ..|.._..|..j..j.
+00002290: 0083 0000 7c00 005f 1100 6400 0053 280b  ....|.._..d..S(.
+000022a0: 0000 004e 7313 0000 002e 2f64 6174 612f  ...Ns...../data/
+000022b0: 7369 6d70 6c65 4578 2e6e 776b 5210 0000  simpleEx.nwkR...
+000022c0: 0052 2300 0000 7328 0000 002e 2f64 6174  .R#...s(..../dat
+000022d0: 612f 7369 6d70 6c65 4578 5f63 6f6d 706c  a/simpleEx_compl
+000022e0: 6578 5061 7261 6c6f 6773 2e6f 7274 686f  exParalogs.ortho
+000022f0: 786d 6c73 3000 0000 2e2f 6461 7461 2f53  xmls0..../data/S
+00002300: 696d 706c 6545 785f 636f 6d70 6c65 7850  impleEx_complexP
+00002310: 6172 616c 6f67 4765 7448 4f47 5333 666f  aralogGetHOGS3fo
+00002320: 726d 6174 2e78 6d6c 5224 0000 0052 2500  rmat.xmlR$...R%.
+00002330: 0000 5226 0000 0052 2700 0000 5228 0000  ..R&...R'...R(..
+00002340: 0028 1200 0000 5229 0000 0052 2a00 0000  .(....R)...R*...
+00002350: 522b 0000 0052 2c00 0000 522d 0000 0052  R+...R,...R-...R
+00002360: 0100 0000 522e 0000 0052 0000 0000 522f  ....R....R....R/
+00002370: 0000 0052 3000 0000 5231 0000 0052 3200  ...R0...R1...R2.
+00002380: 0000 5233 0000 0052 3400 0000 5235 0000  ..R3...R4...R5..
+00002390: 0074 0f00 0000 6861 6d5f 616e 616c 7973  .t....ham_analys
+000023a0: 6973 5f76 3374 0700 0000 686f 6773 5f76  is_v3t....hogs_v
+000023b0: 3374 0800 0000 6765 6e65 735f 7633 2805  3t....genes_v3(.
+000023c0: 0000 0052 1100 0000 5236 0000 0052 3700  ...R....R6...R7.
+000023d0: 0000 5238 0000 0074 1000 0000 6f72 7468  ..R8...t....orth
+000023e0: 6f78 6d6c 5f70 6174 685f 7633 2800 0000  oxml_path_v3(...
+000023f0: 0028 0000 0000 733c 0000 002f 5573 6572  .(....s<.../User
+00002400: 732f 6164 7269 6161 6c2f 5265 706f 7369  s/adriaal/Reposi
+00002410: 746f 7269 6573 2f48 414d 2f74 6573 7473  tories/HAM/tests
+00002420: 2f74 6573 745f 6f72 7468 6f78 6d6c 7061  /test_orthoxmlpa
+00002430: 7273 6572 2e70 7952 3900 0000 c000 0000  rser.pyR9.......
+00002440: 7318 0000 0000 0121 0115 0121 0121 021b  s......!...!.!..
+00002450: 010c 0112 0112 021b 010c 0112 0163 0100  .............c..
+00002460: 0000 0400 0000 0300 0000 4300 0000 7350  ..........C...sP
+00002470: 0000 0064 0100 6402 006c 0000 6d01 007d  ...d..d..l..m..}
+00002480: 0100 017c 0100 7c00 006a 0200 8301 007d  ...|..|..j.....}
+00002490: 0200 782a 007c 0000 6a02 006a 0300 6a04  ..x*.|..j..j..j.
+000024a0: 0083 0000 445d 1600 7d03 007c 0000 6a05  ....D]..}..|..j.
+000024b0: 007c 0300 6a06 0083 0100 0171 3200 5764  .|..j......q2.Wd
+000024c0: 0000 5328 0300 0000 4e69 ffff ffff 2801  ..S(....Ni....(.
+000024d0: 0000 0074 0b00 0000 5472 6565 5072 6f66  ...t....TreeProf
+000024e0: 696c 6528 0700 0000 7405 0000 0070 7968  ile(....t....pyh
+000024f0: 616d 528e 0000 0052 3100 0000 7407 0000  amR....R1...t...
+00002500: 0048 4f47 4d61 7073 5244 0000 0052 8500  .HOGMapsRD...R..
+00002510: 0000 740a 0000 0063 6f6e 7369 7374 656e  ..t....consisten
+00002520: 7428 0400 0000 5211 0000 0052 8e00 0000  t(....R....R....
+00002530: 7402 0000 0074 7074 0200 0000 6867 2800  t....tpt....hg(.
+00002540: 0000 0028 0000 0000 733c 0000 002f 5573  ...(....s<.../Us
+00002550: 6572 732f 6164 7269 6161 6c2f 5265 706f  ers/adriaal/Repo
+00002560: 7369 746f 7269 6573 2f48 414d 2f74 6573  sitories/HAM/tes
+00002570: 7473 2f74 6573 745f 6f72 7468 6f78 6d6c  ts/test_orthoxml
+00002580: 7061 7273 6572 2e70 7974 1700 0000 7465  parser.pyt....te
+00002590: 7374 5f63 6f6e 7369 7374 656e 6379 5f6e  st_consistency_n
+000025a0: 756d 6265 72d0 0000 0073 0800 0000 0002  umber....s......
+000025b0: 1003 0f03 1901 6301 0000 0002 0000 0002  ......c.........
+000025c0: 0000 0003 0000 0073 2d00 0000 8700 0066  .......s-......f
+000025d0: 0100 6401 0086 0000 7d01 007c 0100 8800  ..d.....}..|....
+000025e0: 006a 0000 8301 0001 7c01 0088 0000 6a01  .j......|.....j.
+000025f0: 0083 0100 0164 0000 5328 0200 0000 4e63  .....d..S(....Nc
+00002600: 0100 0000 0400 0000 0d00 0000 1300 0000  ................
+00002610: 737d 0000 0074 0000 6401 0064 0200 6403  s}...t..d..d..d.
+00002620: 0064 0400 6405 0064 0600 6407 0064 0800  .d..d..d..d..d..
+00002630: 6409 0064 0a00 640b 0064 0800 8300 067d  d..d..d..d.....}
+00002640: 0100 7401 006a 0200 7403 0083 0100 7d02  ..t..j..t.....}.
+00002650: 0078 2a00 7c00 006a 0400 8300 0044 5d1c  .x*.|..j.....D].
+00002660: 007d 0300 7c02 007c 0300 6a05 006a 0600  .}..|..|..j..j..
+00002670: 6302 0019 640c 0037 033c 7149 0057 8800  c...d..7.<qI.W..
+00002680: 006a 0700 7c02 007c 0100 8302 0001 6400  .j..|..|......d.
+00002690: 0053 280d 0000 004e 523a 0000 0069 0600  .S(....NR:...i..
+000026a0: 0000 523b 0000 0069 0900 0000 523c 0000  ..R;...i....R<..
+000026b0: 0069 0800 0000 523d 0000 0069 0400 0000  .i....R=...i....
+000026c0: 523e 0000 0069 0700 0000 523f 0000 0069  R>...i....R?...i
+000026d0: 0100 0000 2808 0000 0052 4000 0000 5241  ....(....R@...RA
+000026e0: 0000 0052 4200 0000 5243 0000 0052 4400  ...RB...RC...RD.
+000026f0: 0000 5209 0000 0052 0b00 0000 5245 0000  ..R....R....RE..
+00002700: 0028 0400 0000 5235 0000 0052 4600 0000  .(....R5...RF...
+00002710: 5247 0000 0052 4800 0000 2801 0000 0052  RG...RH...(....R
+00002720: 1100 0000 2800 0000 0073 3c00 0000 2f55  ....(....s<.../U
+00002730: 7365 7273 2f61 6472 6961 616c 2f52 6570  sers/adriaal/Rep
+00002740: 6f73 6974 6f72 6965 732f 4841 4d2f 7465  ositories/HAM/te
+00002750: 7374 732f 7465 7374 5f6f 7274 686f 786d  sts/test_orthoxm
+00002760: 6c70 6172 7365 722e 7079 7409 0000 005f  lparser.pyt...._
+00002770: 7465 7374 5f6f 6e65 dd00 0000 730c 0000  test_one....s...
+00002780: 0000 011e 010f 010f 0113 011a 0128 0200  .............(..
+00002790: 0000 5235 0000 0052 8c00 0000 2802 0000  ..R5...R....(...
+000027a0: 0052 1100 0000 5295 0000 0028 0000 0000  .R....R....(....
+000027b0: 2801 0000 0052 1100 0000 733c 0000 002f  (....R....s<.../
+000027c0: 5573 6572 732f 6164 7269 6161 6c2f 5265  Users/adriaal/Re
+000027d0: 706f 7369 746f 7269 6573 2f48 414d 2f74  positories/HAM/t
+000027e0: 6573 7473 2f74 6573 745f 6f72 7468 6f78  ests/test_orthox
+000027f0: 6d6c 7061 7273 6572 2e70 7952 4900 0000  mlparser.pyRI...
+00002800: db00 0000 7306 0000 0000 020f 080d 0163  ....s..........c
+00002810: 0100 0000 0200 0000 0200 0000 4300 0000  ............C...
+00002820: 7327 0000 0064 0100 8400 007d 0100 7c01  s'...d.....}..|.
+00002830: 007c 0000 6a00 0083 0100 017c 0100 7c00  .|..j......|..|.
+00002840: 006a 0100 8301 0001 6400 0053 2802 0000  .j......d..S(...
+00002850: 004e 6301 0000 0005 0000 0006 0000 0053  .Nc............S
+00002860: 0000 0073 9200 0000 7c00 006a 0000 8300  ...s....|..j....
+00002870: 007d 0100 6905 0064 0100 6402 0036 6403  .}..i..d..d..6d.
+00002880: 0064 0400 3664 0500 6406 0036 6407 0064  .d..6d..d..6d..d
+00002890: 0800 3664 0900 640a 0036 7d02 0069 0500  ..6d..d..6}..i..
+000028a0: 640b 0064 0200 3664 0b00 6404 0036 640b  d..d..6d..d..6d.
+000028b0: 0064 0600 3664 0b00 6408 0036 640b 0064  .d..6d..d..6d..d
+000028c0: 0a00 367d 0300 782d 007c 0100 445d 2500  ..6}..x-.|..D]%.
+000028d0: 7d04 007c 0300 7c04 006a 0100 6a02 0063  }..|..|..j..j..c
+000028e0: 0200 1974 0300 7c04 006a 0400 8301 0037  ...t..|..j.....7
+000028f0: 033c 7165 0057 6400 0053 280c 0000 004e  .<qe.Wd..S(....N
+00002900: 6904 0000 0052 4a00 0000 6906 0000 0052  i....RJ...i....R
+00002910: 4b00 0000 6908 0000 0052 4c00 0000 6905  K...i....RL...i.
+00002920: 0000 0052 4d00 0000 6907 0000 0052 4e00  ...RM...i....RN.
+00002930: 0000 6900 0000 0028 0500 0000 524f 0000  ..i....(....RO..
+00002940: 0052 0a00 0000 520b 0000 0052 1600 0000  .R....R....R....
+00002950: 5235 0000 0028 0500 0000 5200 0000 0052  R5...(....R....R
+00002960: 5000 0000 5251 0000 0052 5200 0000 5253  P...RQ...RR...RS
+00002970: 0000 0028 0000 0000 2800 0000 0073 3c00  ...(....(....s<.
+00002980: 0000 2f55 7365 7273 2f61 6472 6961 616c  ../Users/adriaal
+00002990: 2f52 6570 6f73 6974 6f72 6965 732f 4841  /Repositories/HA
+000029a0: 4d2f 7465 7374 732f 7465 7374 5f6f 7274  M/tests/test_ort
+000029b0: 686f 786d 6c70 6172 7365 722e 7079 5295  hoxmlparser.pyR.
+000029c0: 0000 00ea 0000 0073 0a00 0000 0001 0c01  .......s........
+000029d0: 2901 2901 0d01 2802 0000 0052 3100 0000  ).)...(....R1...
+000029e0: 528a 0000 0028 0200 0000 5211 0000 0052  R....(....R....R
+000029f0: 9500 0000 2800 0000 0028 0000 0000 733c  ....(....(....s<
+00002a00: 0000 002f 5573 6572 732f 6164 7269 6161  .../Users/adriaa
+00002a10: 6c2f 5265 706f 7369 746f 7269 6573 2f48  l/Repositories/H
+00002a20: 414d 2f74 6573 7473 2f74 6573 745f 6f72  AM/tests/test_or
+00002a30: 7468 6f78 6d6c 7061 7273 6572 2e70 7952  thoxmlparser.pyR
+00002a40: 5400 0000 e800 0000 7306 0000 0000 0209  T.......s.......
+00002a50: 070d 0163 0100 0000 0200 0000 0200 0000  ...c............
+00002a60: 0300 0000 732d 0000 0087 0000 6601 0064  ....s-......f..d
+00002a70: 0100 8600 007d 0100 7c01 0088 0000 6a00  .....}..|.....j.
+00002a80: 0083 0100 017c 0100 8800 006a 0100 8301  .....|.....j....
+00002a90: 0001 6400 0053 2802 0000 004e 6301 0000  ..d..S(....Nc...
+00002aa0: 0001 0000 0007 0000 0013 0000 0073 6f00  .............so.
+00002ab0: 0000 8800 006a 0000 7c00 0064 0100 196a  .....j..|..d...j
+00002ac0: 0100 6402 0083 0100 6403 0083 0200 0188  ..d.....d.......
+00002ad0: 0000 6a02 0074 0300 8301 008f 1600 017c  ..j..t.........|
+00002ae0: 0000 6404 0019 6a01 0064 0200 8301 0001  ..d...j..d......
+00002af0: 5764 0000 5158 8800 006a 0200 7403 0083  Wd..QX...j..t...
+00002b00: 0100 8f16 0001 7c00 0064 0100 196a 0100  ......|..d...j..
+00002b10: 6405 0083 0100 0157 6400 0051 5864 0000  d......Wd..QXd..
+00002b20: 5328 0600 0000 4e52 5500 0000 5256 0000  S(....NRU...RV..
+00002b30: 0069 0100 0000 5257 0000 0052 5800 0000  .i....RW...RX...
+00002b40: 2804 0000 0052 1e00 0000 5259 0000 0052  (....R....RY...R
+00002b50: 5a00 0000 525b 0000 0028 0100 0000 5233  Z...R[...(....R3
+00002b60: 0000 0028 0100 0000 5211 0000 0028 0000  ...(....R....(..
+00002b70: 0000 733c 0000 002f 5573 6572 732f 6164  ..s<.../Users/ad
+00002b80: 7269 6161 6c2f 5265 706f 7369 746f 7269  riaal/Repositori
+00002b90: 6573 2f48 414d 2f74 6573 7473 2f74 6573  es/HAM/tests/tes
+00002ba0: 745f 6f72 7468 6f78 6d6c 7061 7273 6572  t_orthoxmlparser
+00002bb0: 2e70 7952 9500 0000 f600 0000 730a 0000  .pyR........s...
+00002bc0: 0000 011d 0110 0117 0110 0128 0200 0000  ...........(....
+00002bd0: 5233 0000 0052 8b00 0000 2802 0000 0052  R3...R....(....R
+00002be0: 1100 0000 5295 0000 0028 0000 0000 2801  ....R....(....(.
+00002bf0: 0000 0052 1100 0000 733c 0000 002f 5573  ...R....s<.../Us
+00002c00: 6572 732f 6164 7269 6161 6c2f 5265 706f  ers/adriaal/Repo
+00002c10: 7369 746f 7269 6573 2f48 414d 2f74 6573  sitories/HAM/tes
+00002c20: 7473 2f74 6573 745f 6f72 7468 6f78 6d6c  ts/test_orthoxml
+00002c30: 7061 7273 6572 2e70 7952 5c00 0000 f400  parser.pyR\.....
+00002c40: 0000 7306 0000 0000 020f 070d 0163 0100  ..s..........c..
+00002c50: 0000 0200 0000 0200 0000 0300 0000 732d  ..............s-
+00002c60: 0000 0087 0000 6601 0064 0100 8600 007d  ......f..d.....}
+00002c70: 0100 7c01 0088 0000 6a00 0083 0100 017c  ..|.....j......|
+00002c80: 0100 8800 006a 0100 8301 0001 6400 0053  .....j......d..S
+00002c90: 2802 0000 004e 6301 0000 0019 0000 000a  (....Nc.........
+00002ca0: 0000 0013 0000 0073 f301 0000 7c00 0064  .......s....|..d
+00002cb0: 0100 197d 0100 7c00 0064 0200 197d 0200  ...}..|..d...}..
+00002cc0: 7c00 0064 0300 197d 0300 7c00 0064 0400  |..d...}..|..d..
+00002cd0: 197d 0400 7c00 0064 0500 197d 0500 7c00  .}..|..d...}..|.
+00002ce0: 0064 0600 197d 0600 6407 0064 0800 6401  .d...}..d..d..d.
+00002cf0: 0064 0900 640a 0064 0b00 6806 007d 0700  .d..d..d..h..}..
+00002d00: 640c 0064 0d00 6402 0064 0e00 6804 007d  d..d..d..d..h..}
+00002d10: 0800 640f 0064 1000 6411 0064 1200 6804  ..d..d..d..d..h.
+00002d20: 007d 0900 6413 0064 1400 6415 0064 1600  .}..d..d..d..d..
+00002d30: 6417 0068 0500 7d0a 0064 1800 6406 0064  d..h..}..d..d..d
+00002d40: 1900 641a 0064 1b00 641c 0064 1d00 641e  ..d..d..d..d..d.
+00002d50: 0064 1f00 6420 0068 0a00 7d0b 0064 2100  .d..d .h..}..d!.
+00002d60: 6422 0064 2300 6424 0068 0400 7d0c 007c  d".d#.d$.h..}..|
+00002d70: 0100 6a00 0083 0000 7d0d 007c 0200 6a00  ..j.....}..|..j.
+00002d80: 0083 0000 7d0e 007c 0300 6a00 0083 0000  ....}..|..j.....
+00002d90: 7d0f 007c 0400 6a00 0083 0000 7d10 007c  }..|..j.....}..|
+00002da0: 0500 6a00 0083 0000 7d11 007c 0600 6a00  ..j.....}..|..j.
+00002db0: 0083 0000 7d12 0074 0100 6425 0084 0000  ....}..t..d%....
+00002dc0: 7c0d 0044 8301 0083 0100 7d13 0074 0100  |..D......}..t..
+00002dd0: 6426 0084 0000 7c0e 0044 8301 0083 0100  d&....|..D......
+00002de0: 7d14 0074 0100 6427 0084 0000 7c0f 0044  }..t..d'....|..D
+00002df0: 8301 0083 0100 7d15 0074 0100 6428 0084  ......}..t..d(..
+00002e00: 0000 7c10 0044 8301 0083 0100 7d16 0074  ..|..D......}..t
+00002e10: 0100 6429 0084 0000 7c11 0044 8301 0083  ..d)....|..D....
+00002e20: 0100 7d17 0074 0100 642a 0084 0000 7c12  ..}..t..d*....|.
+00002e30: 0044 8301 0083 0100 7d18 0088 0000 6a02  .D......}.....j.
+00002e40: 007c 0700 7c13 0083 0200 0188 0000 6a02  .|..|.........j.
+00002e50: 007c 0800 7c14 0083 0200 0188 0000 6a02  .|..|.........j.
+00002e60: 007c 0900 7c15 0083 0200 0188 0000 6a02  .|..|.........j.
+00002e70: 007c 0a00 7c16 0083 0200 0188 0000 6a02  .|..|.........j.
+00002e80: 007c 0b00 7c17 0083 0200 0188 0000 6a02  .|..|.........j.
+00002e90: 007c 0c00 7c18 0083 0200 0164 0000 5328  .|..|......d..S(
+00002ea0: 2b00 0000 4e52 5500 0000 5257 0000 0052  +...NRU...RW...R
+00002eb0: 5d00 0000 7401 0000 0034 7401 0000 0035  ]...t....4t....5
+00002ec0: 7401 0000 0036 525e 0000 0052 5f00 0000  t....6R^...R_...
+00002ed0: 5260 0000 0052 6100 0000 5262 0000 0052  R`...Ra...Rb...R
+00002ee0: 6300 0000 5264 0000 0052 6500 0000 5266  c...Rd...Re...Rf
+00002ef0: 0000 0052 6700 0000 5269 0000 0052 6a00  ...Rg...Ri...Rj.
+00002f00: 0000 7402 0000 0031 3574 0200 0000 3136  ..t....15t....16
+00002f10: 7402 0000 0032 3474 0200 0000 3235 7402  t....24t....25t.
+00002f20: 0000 0035 3474 0200 0000 3236 7402 0000  ...54t....26t...
+00002f30: 0031 3774 0200 0000 3335 7402 0000 0034  .17t....35t....4
+00002f40: 3474 0100 0000 3774 0200 0000 3138 7402  4t....7t....18t.
+00002f50: 0000 0033 3674 0200 0000 3337 7402 0000  ...36t....37t...
+00002f60: 0034 3574 0200 0000 3139 7402 0000 0033  .45t....19t....3
+00002f70: 3874 0200 0000 3237 7402 0000 0035 3663  8t....27t....56c
+00002f80: 0100 0000 0200 0000 0200 0000 7300 0000  ............s...
+00002f90: 7318 0000 007c 0000 5d0e 007d 0100 7c01  s....|..]..}..|.
+00002fa0: 006a 0000 5601 7103 0064 0000 5328 0100  .j..V.q..d..S(..
+00002fb0: 0000 4e28 0100 0000 5207 0000 0028 0200  ..N(....R....(..
+00002fc0: 0000 521b 0000 0052 6c00 0000 2800 0000  ..R....Rl...(...
+00002fd0: 0028 0000 0000 733c 0000 002f 5573 6572  .(....s<.../User
+00002fe0: 732f 6164 7269 6161 6c2f 5265 706f 7369  s/adriaal/Reposi
+00002ff0: 746f 7269 6573 2f48 414d 2f74 6573 7473  tories/HAM/tests
+00003000: 2f74 6573 745f 6f72 7468 6f78 6d6c 7061  /test_orthoxmlpa
+00003010: 7273 6572 2e70 7973 0900 0000 3c67 656e  rser.pys....<gen
+00003020: 6578 7072 3e18 0100 0073 0200 0000 0600  expr>....s......
+00003030: 6301 0000 0002 0000 0002 0000 0073 0000  c............s..
+00003040: 0073 1800 0000 7c00 005d 0e00 7d01 007c  .s....|..]..}..|
+00003050: 0100 6a00 0056 0171 0300 6400 0053 2801  ..j..V.q..d..S(.
+00003060: 0000 004e 2801 0000 0052 0700 0000 2802  ...N(....R....(.
+00003070: 0000 0052 1b00 0000 526c 0000 0028 0000  ...R....Rl...(..
+00003080: 0000 2800 0000 0073 3c00 0000 2f55 7365  ..(....s<.../Use
+00003090: 7273 2f61 6472 6961 616c 2f52 6570 6f73  rs/adriaal/Repos
+000030a0: 6974 6f72 6965 732f 4841 4d2f 7465 7374  itories/HAM/test
+000030b0: 732f 7465 7374 5f6f 7274 686f 786d 6c70  s/test_orthoxmlp
+000030c0: 6172 7365 722e 7079 7309 0000 003c 6765  arser.pys....<ge
+000030d0: 6e65 7870 723e 1901 0000 7302 0000 0006  nexpr>....s.....
+000030e0: 0063 0100 0000 0200 0000 0200 0000 7300  .c............s.
+000030f0: 0000 7318 0000 007c 0000 5d0e 007d 0100  ..s....|..]..}..
+00003100: 7c01 006a 0000 5601 7103 0064 0000 5328  |..j..V.q..d..S(
+00003110: 0100 0000 4e28 0100 0000 5207 0000 0028  ....N(....R....(
+00003120: 0200 0000 521b 0000 0052 6c00 0000 2800  ....R....Rl...(.
+00003130: 0000 0028 0000 0000 733c 0000 002f 5573  ...(....s<.../Us
+00003140: 6572 732f 6164 7269 6161 6c2f 5265 706f  ers/adriaal/Repo
+00003150: 7369 746f 7269 6573 2f48 414d 2f74 6573  sitories/HAM/tes
+00003160: 7473 2f74 6573 745f 6f72 7468 6f78 6d6c  ts/test_orthoxml
+00003170: 7061 7273 6572 2e70 7973 0900 0000 3c67  parser.pys....<g
+00003180: 656e 6578 7072 3e1a 0100 0073 0200 0000  enexpr>....s....
+00003190: 0600 6301 0000 0002 0000 0002 0000 0073  ..c............s
+000031a0: 0000 0073 1800 0000 7c00 005d 0e00 7d01  ...s....|..]..}.
+000031b0: 007c 0100 6a00 0056 0171 0300 6400 0053  .|..j..V.q..d..S
+000031c0: 2801 0000 004e 2801 0000 0052 0700 0000  (....N(....R....
+000031d0: 2802 0000 0052 1b00 0000 526c 0000 0028  (....R....Rl...(
+000031e0: 0000 0000 2800 0000 0073 3c00 0000 2f55  ....(....s<.../U
+000031f0: 7365 7273 2f61 6472 6961 616c 2f52 6570  sers/adriaal/Rep
+00003200: 6f73 6974 6f72 6965 732f 4841 4d2f 7465  ositories/HAM/te
+00003210: 7374 732f 7465 7374 5f6f 7274 686f 786d  sts/test_orthoxm
+00003220: 6c70 6172 7365 722e 7079 7309 0000 003c  lparser.pys....<
+00003230: 6765 6e65 7870 723e 1b01 0000 7302 0000  genexpr>....s...
+00003240: 0006 0063 0100 0000 0200 0000 0200 0000  ...c............
+00003250: 7300 0000 7318 0000 007c 0000 5d0e 007d  s...s....|..]..}
+00003260: 0100 7c01 006a 0000 5601 7103 0064 0000  ..|..j..V.q..d..
+00003270: 5328 0100 0000 4e28 0100 0000 5207 0000  S(....N(....R...
+00003280: 0028 0200 0000 521b 0000 0052 6c00 0000  .(....R....Rl...
+00003290: 2800 0000 0028 0000 0000 733c 0000 002f  (....(....s<.../
+000032a0: 5573 6572 732f 6164 7269 6161 6c2f 5265  Users/adriaal/Re
+000032b0: 706f 7369 746f 7269 6573 2f48 414d 2f74  positories/HAM/t
+000032c0: 6573 7473 2f74 6573 745f 6f72 7468 6f78  ests/test_orthox
+000032d0: 6d6c 7061 7273 6572 2e70 7973 0900 0000  mlparser.pys....
+000032e0: 3c67 656e 6578 7072 3e1c 0100 0073 0200  <genexpr>....s..
+000032f0: 0000 0600 6301 0000 0002 0000 0002 0000  ....c...........
+00003300: 0073 0000 0073 1800 0000 7c00 005d 0e00  .s...s....|..]..
+00003310: 7d01 007c 0100 6a00 0056 0171 0300 6400  }..|..j..V.q..d.
+00003320: 0053 2801 0000 004e 2801 0000 0052 0700  .S(....N(....R..
+00003330: 0000 2802 0000 0052 1b00 0000 526c 0000  ..(....R....Rl..
+00003340: 0028 0000 0000 2800 0000 0073 3c00 0000  .(....(....s<...
+00003350: 2f55 7365 7273 2f61 6472 6961 616c 2f52  /Users/adriaal/R
+00003360: 6570 6f73 6974 6f72 6965 732f 4841 4d2f  epositories/HAM/
+00003370: 7465 7374 732f 7465 7374 5f6f 7274 686f  tests/test_ortho
+00003380: 786d 6c70 6172 7365 722e 7079 7309 0000  xmlparser.pys...
+00003390: 003c 6765 6e65 7870 723e 1d01 0000 7302  .<genexpr>....s.
+000033a0: 0000 0006 0028 0300 0000 526d 0000 0052  .....(....Rm...R
+000033b0: 6e00 0000 526f 0000 0028 1900 0000 5233  n...Ro...(....R3
+000033c0: 0000 0052 7000 0000 5271 0000 0052 7200  ...Rp...Rq...Rr.
+000033d0: 0000 7404 0000 0068 6f67 3474 0400 0000  ..t....hog4t....
+000033e0: 686f 6735 7404 0000 0068 6f67 3652 7300  hog5t....hog6Rs.
+000033f0: 0000 5274 0000 0052 7500 0000 7411 0000  ..Rt...Ru...t...
+00003400: 0065 7870 6563 7465 644d 656d 6265 7273  .expectedMembers
+00003410: 5f34 7411 0000 0065 7870 6563 7465 644d  _4t....expectedM
+00003420: 656d 6265 7273 5f35 7411 0000 0065 7870  embers_5t....exp
+00003430: 6563 7465 644d 656d 6265 7273 5f36 5276  ectedMembers_6Rv
+00003440: 0000 0052 7700 0000 5278 0000 0074 0a00  ...Rw...Rx...t..
+00003450: 0000 686f 6734 5f67 656e 6573 740a 0000  ..hog4_genest...
+00003460: 0068 6f67 355f 6765 6e65 7374 0a00 0000  .hog5_genest....
+00003470: 686f 6736 5f67 656e 6573 5279 0000 0052  hog6_genesRy...R
+00003480: 7a00 0000 527b 0000 0074 0900 0000 6d65  z...R{...t....me
+00003490: 6d62 6572 735f 3474 0900 0000 6d65 6d62  mbers_4t....memb
+000034a0: 6572 735f 3574 0900 0000 6d65 6d62 6572  ers_5t....member
+000034b0: 735f 3628 0100 0000 5211 0000 0028 0000  s_6(....R....(..
+000034c0: 0000 733c 0000 002f 5573 6572 732f 6164  ..s<.../Users/ad
+000034d0: 7269 6161 6c2f 5265 706f 7369 746f 7269  riaal/Repositori
+000034e0: 6573 2f48 414d 2f74 6573 7473 2f74 6573  es/HAM/tests/tes
+000034f0: 745f 6f72 7468 6f78 6d6c 7061 7273 6572  t_orthoxmlparser
+00003500: 2e70 7952 9500 0000 0201 0000 733c 0000  .pyR........s<..
+00003510: 0000 010a 010a 010a 010a 010a 010a 0218  ................
+00003520: 0112 0112 0115 0124 0112 020c 010c 010c  .......$........
+00003530: 010c 010c 010c 0216 0116 0116 0116 0116  ................
+00003540: 0116 0210 0110 0110 0110 0110 0128 0200  .............(..
+00003550: 0000 5233 0000 0052 8b00 0000 2802 0000  ..R3...R....(...
+00003560: 0052 1100 0000 5295 0000 0028 0000 0000  .R....R....(....
+00003570: 2801 0000 0052 1100 0000 733c 0000 002f  (....R....s<.../
+00003580: 5573 6572 732f 6164 7269 6161 6c2f 5265  Users/adriaal/Re
+00003590: 706f 7369 746f 7269 6573 2f48 414d 2f74  positories/HAM/t
+000035a0: 6573 7473 2f74 6573 745f 6f72 7468 6f78  ests/test_orthox
+000035b0: 6d6c 7061 7273 6572 2e70 7952 7c00 0000  mlparser.pyR|...
+000035c0: 0001 0000 7306 0000 0000 020f 240d 0163  ....s.......$..c
+000035d0: 0100 0000 0200 0000 0300 0000 0300 0000  ................
+000035e0: 7335 0000 0087 0000 6601 0064 0100 8600  s5......f..d....
+000035f0: 007d 0100 7c01 0088 0000 6a00 0064 0200  .}..|.....j..d..
+00003600: 1983 0100 017c 0100 8800 006a 0100 6402  .....|.....j..d.
+00003610: 0019 8301 0001 6400 0053 2803 0000 004e  ......d..S(....N
+00003620: 6301 0000 0005 0000 0004 0000 0013 0000  c...............
+00003630: 0073 d300 0000 8800 006a 0000 6401 007c  .s.......j..d..|
+00003640: 0000 6a01 006a 0200 6a03 0083 0200 0188  ..j..j..j.......
+00003650: 0000 6a04 007c 0000 6402 0064 0300 6702  ..j..|..d..d..g.
+00003660: 0083 0200 0188 0000 6a05 007c 0000 6403  ........j..|..d.
+00003670: 0083 0200 7d01 0088 0000 6a04 007c 0100  ....}.....j..|..
+00003680: 6404 0064 0500 6702 0083 0200 0188 0000  d..d..g.........
+00003690: 6a05 007c 0100 6405 0083 0200 7d02 0088  j..|..d.....}...
+000036a0: 0000 6a04 007c 0200 6406 0064 0700 6702  ..j..|..d..d..g.
+000036b0: 0083 0200 0188 0000 6a05 007c 0200 6406  ........j..|..d.
+000036c0: 0083 0200 7d03 0088 0000 6a04 007c 0300  ....}.....j..|..
+000036d0: 6408 0064 0900 6702 0083 0200 0188 0000  d..d..g.........
+000036e0: 6a05 007c 0200 6407 0083 0200 7d04 0088  j..|..d.....}...
+000036f0: 0000 6a04 007c 0400 640a 0064 0b00 6702  ..j..|..d..d..g.
+00003700: 0083 0200 0164 0000 5328 0c00 0000 4e52  .....d..S(....NR
+00003710: 4a00 0000 525e 0000 0052 4b00 0000 525f  J...R^...RK...R_
+00003720: 0000 0052 4c00 0000 524d 0000 0052 4e00  ...RL...RM...RN.
+00003730: 0000 5262 0000 0052 6100 0000 5255 0000  ..Rb...Ra...RU..
+00003740: 0052 6000 0000 2806 0000 0052 1e00 0000  .R`...(....R....
+00003750: 5209 0000 0052 0a00 0000 520b 0000 0052  R....R....R....R
+00003760: 2200 0000 521a 0000 0028 0500 0000 521f  "...R....(....R.
+00003770: 0000 0052 7d00 0000 527e 0000 0052 7f00  ...R}...R~...R..
+00003780: 0000 5280 0000 0028 0100 0000 5211 0000  ..R....(....R...
+00003790: 0028 0000 0000 733c 0000 002f 5573 6572  .(....s<.../User
+000037a0: 732f 6164 7269 6161 6c2f 5265 706f 7369  s/adriaal/Reposi
+000037b0: 746f 7269 6573 2f48 414d 2f74 6573 7473  tories/HAM/tests
+000037c0: 2f74 6573 745f 6f72 7468 6f78 6d6c 7061  /test_orthoxmlpa
+000037d0: 7273 6572 2e70 7952 9500 0000 2b01 0000  rser.pyR....+...
+000037e0: 7314 0000 0000 0219 0116 0312 0116 0312  s...............
+000037f0: 0116 0312 0116 0312 0152 5500 0000 2802  .........RU...(.
+00003800: 0000 0052 3300 0000 528b 0000 0028 0200  ...R3...R....(..
+00003810: 0000 5211 0000 0052 9500 0000 2800 0000  ..R....R....(...
+00003820: 0028 0100 0000 5211 0000 0073 3c00 0000  .(....R....s<...
+00003830: 2f55 7365 7273 2f61 6472 6961 616c 2f52  /Users/adriaal/R
+00003840: 6570 6f73 6974 6f72 6965 732f 4841 4d2f  epositories/HAM/
+00003850: 7465 7374 732f 7465 7374 5f6f 7274 686f  tests/test_ortho
+00003860: 786d 6c70 6172 7365 722e 7079 5281 0000  xmlparser.pyR...
+00003870: 0029 0100 0073 0600 0000 0002 0f15 1101  .)...s..........
+00003880: 6301 0000 0002 0000 0003 0000 0003 0000  c...............
+00003890: 0073 3500 0000 8700 0066 0100 6401 0086  .s5......f..d...
+000038a0: 0000 7d01 007c 0100 8800 006a 0000 6402  ..}..|.....j..d.
+000038b0: 0019 8301 0001 7c01 0088 0000 6a01 0064  ......|.....j..d
+000038c0: 0200 1983 0100 0164 0000 5328 0300 0000  .......d..S(....
+000038d0: 4e63 0100 0000 0400 0000 0400 0000 1300  Nc..............
+000038e0: 0000 73a8 0000 0088 0000 6a00 0064 0100  ..s.......j..d..
+000038f0: 7c00 006a 0100 6a02 006a 0300 8302 0001  |..j..j..j......
+00003900: 8800 006a 0400 7c00 0064 0200 6403 0067  ...j..|..d..d..g
+00003910: 0200 8302 0001 8800 006a 0500 7c00 0064  .........j..|..d
+00003920: 0300 8302 007d 0100 8800 006a 0400 7c01  .....}.....j..|.
+00003930: 0064 0400 6405 0067 0200 8302 0001 8800  .d..d..g........
+00003940: 006a 0500 7c01 0064 0500 8302 007d 0200  .j..|..d.....}..
+00003950: 8800 006a 0400 7c02 0064 0600 6407 0067  ...j..|..d..d..g
+00003960: 0200 8302 0001 8800 006a 0500 7c01 0064  .........j..|..d
+00003970: 0400 8302 007d 0300 8800 006a 0400 7c03  .....}.....j..|.
+00003980: 0064 0800 6801 0083 0200 0164 0000 5328  .d..h......d..S(
+00003990: 0900 0000 4e52 4b00 0000 5263 0000 0052  ....NRK...Rc...R
+000039a0: 4c00 0000 524d 0000 0052 4e00 0000 5257  L...RM...RN...RW
+000039b0: 0000 0052 6500 0000 5264 0000 0028 0600  ...Re...Rd...(..
+000039c0: 0000 521e 0000 0052 0900 0000 520a 0000  ..R....R....R...
+000039d0: 0052 0b00 0000 5222 0000 0052 1a00 0000  .R....R"...R....
+000039e0: 2804 0000 0052 7100 0000 527e 0000 0052  (....Rq...R~...R
+000039f0: 8000 0000 527f 0000 0028 0100 0000 5211  ....R....(....R.
+00003a00: 0000 0028 0000 0000 733c 0000 002f 5573  ...(....s<.../Us
+00003a10: 6572 732f 6164 7269 6161 6c2f 5265 706f  ers/adriaal/Repo
+00003a20: 7369 746f 7269 6573 2f48 414d 2f74 6573  sitories/HAM/tes
+00003a30: 7473 2f74 6573 745f 6f72 7468 6f78 6d6c  ts/test_orthoxml
+00003a40: 7061 7273 6572 2e70 7952 9500 0000 4501  parser.pyR....E.
+00003a50: 0000 7310 0000 0000 0219 0116 0312 0116  ..s.............
+00003a60: 0312 0116 0312 0152 5700 0000 2802 0000  .......RW...(...
+00003a70: 0052 3300 0000 528b 0000 0028 0200 0000  .R3...R....(....
+00003a80: 5211 0000 0052 9500 0000 2800 0000 0028  R....R....(....(
+00003a90: 0100 0000 5211 0000 0073 3c00 0000 2f55  ....R....s<.../U
+00003aa0: 7365 7273 2f61 6472 6961 616c 2f52 6570  sers/adriaal/Rep
+00003ab0: 6f73 6974 6f72 6965 732f 4841 4d2f 7465  ositories/HAM/te
+00003ac0: 7374 732f 7465 7374 5f6f 7274 686f 786d  sts/test_orthoxm
+00003ad0: 6c70 6172 7365 722e 7079 5282 0000 0043  lparser.pyR....C
+00003ae0: 0100 0073 0600 0000 0002 0f11 1101 6301  ...s..........c.
+00003af0: 0000 0002 0000 0003 0000 0003 0000 0073  ...............s
+00003b00: 3500 0000 8700 0066 0100 6401 0086 0000  5......f..d.....
+00003b10: 7d01 007c 0100 8800 006a 0000 6402 0019  }..|.....j..d...
+00003b20: 8301 0001 7c01 0088 0000 6a01 0064 0200  ....|.....j..d..
+00003b30: 1983 0100 0164 0000 5328 0300 0000 4e63  .....d..S(....Nc
+00003b40: 0100 0000 0600 0000 0400 0000 1300 0000  ................
+00003b50: 732c 0100 0088 0000 6a00 0064 0100 7c00  s,......j..d..|.
+00003b60: 006a 0100 6a02 006a 0300 8302 0001 8800  .j..j..j........
+00003b70: 006a 0400 7c00 0064 0200 6403 0067 0200  .j..|..d..d..g..
+00003b80: 8302 0001 8800 006a 0500 7c00 006a 0600  .......j..|..j..
+00003b90: 8301 0001 8800 006a 0700 7c00 0064 0300  .......j..|..d..
+00003ba0: 8302 007d 0100 8800 006a 0400 7c01 0064  ...}.....j..|..d
+00003bb0: 0400 6405 0067 0200 8302 0001 8800 006a  ..d..g.........j
+00003bc0: 0500 7c01 006a 0600 8301 0001 8800 006a  ..|..j.........j
+00003bd0: 0700 7c01 0064 0500 8302 007d 0200 8800  ..|..d.....}....
+00003be0: 006a 0500 7c02 006a 0600 8301 0001 8800  .j..|..j........
+00003bf0: 006a 0400 7c02 0064 0600 6701 0083 0200  .j..|..d..g.....
+00003c00: 0188 0000 6a07 007c 0200 6406 0083 0200  ....j..|..d.....
+00003c10: 7d03 0088 0000 6a05 007c 0300 6a06 0083  }.....j..|..j...
+00003c20: 0100 0188 0000 6a04 007c 0300 6407 0064  ......j..|..d..d
+00003c30: 0800 6702 0083 0200 0188 0000 6a08 006a  ..g.........j..j
+00003c40: 0900 6407 0083 0100 7d04 0088 0000 6a0a  ..d.....}.....j.
+00003c50: 007c 0400 6a06 0083 0100 0188 0000 6a08  .|..j.........j.
+00003c60: 006a 0900 6408 0083 0100 7d05 0088 0000  .j..d.....}.....
+00003c70: 6a0a 007c 0500 6a06 0083 0100 0164 0000  j..|..j......d..
+00003c80: 5328 0900 0000 4e52 4a00 0000 5269 0000  S(....NRJ...Ri..
+00003c90: 0052 4b00 0000 5267 0000 0052 4c00 0000  .RK...Rg...RL...
+00003ca0: 524e 0000 0052 6600 0000 526a 0000 0028  RN...Rf...Rj...(
+00003cb0: 0b00 0000 521e 0000 0052 0900 0000 520a  ....R....R....R.
+00003cc0: 0000 0052 0b00 0000 5222 0000 0052 8300  ...R....R"...R..
+00003cd0: 0000 5284 0000 0052 1a00 0000 5231 0000  ..R....R....R1..
+00003ce0: 0074 0e00 0000 6765 745f 6765 6e65 5f62  .t....get_gene_b
+00003cf0: 795f 6964 5285 0000 0028 0600 0000 5272  y_idR....(....Rr
+00003d00: 0000 0052 7d00 0000 5286 0000 0052 8000  ...R}...R....R..
+00003d10: 0000 7403 0000 0067 3133 7403 0000 0067  ..t....g13t....g
+00003d20: 3134 2801 0000 0052 1100 0000 2800 0000  14(....R....(...
+00003d30: 0073 3c00 0000 2f55 7365 7273 2f61 6472  .s<.../Users/adr
+00003d40: 6961 616c 2f52 6570 6f73 6974 6f72 6965  iaal/Repositorie
+00003d50: 732f 4841 4d2f 7465 7374 732f 7465 7374  s/HAM/tests/test
+00003d60: 5f6f 7274 686f 786d 6c70 6172 7365 722e  _orthoxmlparser.
+00003d70: 7079 5295 0000 005b 0100 0073 2000 0000  pyR....[...s ...
+00003d80: 0002 1901 1601 1003 1201 1601 1003 1201  ................
+00003d90: 1001 1303 1201 1001 1601 1201 1001 1201  ................
+00003da0: 525d 0000 0028 0200 0000 5233 0000 0052  R]...(....R3...R
+00003db0: 8b00 0000 2802 0000 0052 1100 0000 5295  ....(....R....R.
+00003dc0: 0000 0028 0000 0000 2801 0000 0052 1100  ...(....(....R..
+00003dd0: 0000 733c 0000 002f 5573 6572 732f 6164  ..s<.../Users/ad
+00003de0: 7269 6161 6c2f 5265 706f 7369 746f 7269  riaal/Repositori
+00003df0: 6573 2f48 414d 2f74 6573 7473 2f74 6573  es/HAM/tests/tes
+00003e00: 745f 6f72 7468 6f78 6d6c 7061 7273 6572  t_orthoxmlparser
+00003e10: 2e70 7952 8700 0000 5901 0000 7306 0000  .pyR....Y...s...
+00003e20: 0000 020f 1911 0163 0100 0000 0200 0000  .......c........
+00003e30: 0300 0000 0300 0000 7335 0000 0087 0000  ........s5......
+00003e40: 6601 0064 0100 8600 007d 0100 7c01 0088  f..d.....}..|...
+00003e50: 0000 6a00 0064 0200 1983 0100 017c 0100  ..j..d.......|..
+00003e60: 8800 006a 0100 6402 0019 8301 0001 6400  ...j..d.......d.
+00003e70: 0053 2803 0000 004e 6301 0000 0008 0000  .S(....Nc.......
+00003e80: 0005 0000 0013 0000 0073 7301 0000 8800  .........ss.....
+00003e90: 006a 0000 6401 007c 0000 6a01 006a 0200  .j..d..|..j..j..
+00003ea0: 6a03 0083 0200 0188 0000 6a04 007c 0000  j.........j..|..
+00003eb0: 6402 0064 0300 6702 0083 0200 0188 0000  d..d..g.........
+00003ec0: 6a05 007c 0000 6a06 0083 0100 0188 0000  j..|..j.........
+00003ed0: 6a07 007c 0000 6403 0083 0200 7d01 0088  j..|..d.....}...
+00003ee0: 0000 6a04 007c 0100 6404 0064 0500 6406  ..j..|..d..d..d.
+00003ef0: 0067 0300 8302 0001 8800 006a 0500 7c01  .g.........j..|.
+00003f00: 006a 0600 8301 0001 8800 006a 0800 6a09  .j.........j..j.
+00003f10: 0064 0400 8301 007d 0200 8800 006a 0a00  .d.....}.....j..
+00003f20: 7c02 006a 0600 8301 0001 8800 006a 0800  |..j.........j..
+00003f30: 6a09 0064 0500 8301 007d 0300 8800 006a  j..d.....}.....j
+00003f40: 0a00 7c03 006a 0600 8301 0001 8800 006a  ..|..j.........j
+00003f50: 0700 7c01 0064 0600 8302 007d 0400 8800  ..|..d.....}....
+00003f60: 006a 0500 7c04 006a 0600 8301 0001 8800  .j..|..j........
+00003f70: 006a 0400 7c04 0064 0700 6701 0083 0200  .j..|..d..g.....
+00003f80: 0188 0000 6a07 007c 0400 6407 0083 0200  ....j..|..d.....
+00003f90: 7d05 0088 0000 6a05 007c 0500 6a06 0083  }.....j..|..j...
+00003fa0: 0100 0188 0000 6a04 007c 0500 6408 0064  ......j..|..d..d
+00003fb0: 0900 6702 0083 0200 0188 0000 6a08 006a  ..g.........j..j
+00003fc0: 0900 6408 0083 0100 7d06 0088 0000 6a0a  ..d.....}.....j.
+00003fd0: 007c 0600 6a06 0083 0100 0188 0000 6a08  .|..j.........j.
+00003fe0: 006a 0900 6409 0083 0100 7d07 0088 0000  .j..d.....}.....
+00003ff0: 6a0a 007c 0700 6a06 0083 0100 0164 0000  j..|..j......d..
+00004000: 5328 0a00 0000 4e52 4a00 0000 529d 0000  S(....NRJ...R...
+00004010: 0052 4b00 0000 529b 0000 0052 9c00 0000  .RK...R....R....
+00004020: 524c 0000 0052 4e00 0000 5299 0000 0052  RL...RN...R....R
+00004030: 9a00 0000 280b 0000 0052 1e00 0000 5209  ....(....R....R.
+00004040: 0000 0052 0a00 0000 520b 0000 0052 2200  ...R....R....R".
+00004050: 0000 5283 0000 0052 8400 0000 521a 0000  ..R....R....R...
+00004060: 0052 3100 0000 52b7 0000 0052 8500 0000  .R1...R....R....
+00004070: 2808 0000 0052 ab00 0000 527d 0000 0074  (....R....R}...t
+00004080: 0300 0000 6732 3474 0300 0000 6732 3552  ....g24t....g25R
+00004090: 8600 0000 5280 0000 0074 0300 0000 6731  ....R....t....g1
+000040a0: 3574 0300 0000 6731 3628 0100 0000 5211  5t....g16(....R.
+000040b0: 0000 0028 0000 0000 733c 0000 002f 5573  ...(....s<.../Us
+000040c0: 6572 732f 6164 7269 6161 6c2f 5265 706f  ers/adriaal/Repo
+000040d0: 7369 746f 7269 6573 2f48 414d 2f74 6573  sitories/HAM/tes
+000040e0: 7473 2f74 6573 745f 6f72 7468 6f78 6d6c  ts/test_orthoxml
+000040f0: 7061 7273 6572 2e70 7952 9500 0000 7901  parser.pyR....y.
+00004100: 0000 7328 0000 0000 0219 0116 0110 0312  ..s(............
+00004110: 0119 0110 0112 0110 0112 0110 0312 0110  ................
+00004120: 0113 0312 0110 0116 0112 0110 0112 0152  ...............R
+00004130: 9600 0000 2802 0000 0052 3300 0000 528b  ....(....R3...R.
+00004140: 0000 0028 0200 0000 5211 0000 0052 9500  ...(....R....R..
+00004150: 0000 2800 0000 0028 0100 0000 5211 0000  ..(....(....R...
+00004160: 0073 3c00 0000 2f55 7365 7273 2f61 6472  .s<.../Users/adr
+00004170: 6961 616c 2f52 6570 6f73 6974 6f72 6965  iaal/Repositorie
+00004180: 732f 4841 4d2f 7465 7374 732f 7465 7374  s/HAM/tests/test
+00004190: 5f6f 7274 686f 786d 6c70 6172 7365 722e  _orthoxmlparser.
+000041a0: 7079 7420 0000 0074 6573 745f 686f 675f  pyt ...test_hog_
+000041b0: 7769 7468 5f73 6973 7465 725f 6475 706c  with_sister_dupl
+000041c0: 6963 6174 696f 6e77 0100 0073 0600 0000  icationw...s....
+000041d0: 0002 0f1d 1101 6301 0000 0002 0000 0003  ......c.........
+000041e0: 0000 0003 0000 0073 3500 0000 8700 0066  .......s5......f
+000041f0: 0100 6401 0086 0000 7d01 007c 0100 8800  ..d.....}..|....
+00004200: 006a 0000 6402 0019 8301 0001 7c01 0088  .j..d.......|...
+00004210: 0000 6a01 0064 0200 1983 0100 0164 0000  ..j..d.......d..
+00004220: 5328 0300 0000 4e63 0100 0000 0800 0000  S(....Nc........
+00004230: 0500 0000 1300 0000 7324 0200 0088 0000  ........s$......
+00004240: 6a00 0064 0100 7c00 006a 0100 6a02 006a  j..d..|..j..j..j
+00004250: 0300 8302 0001 8800 006a 0400 7c00 0064  .........j..|..d
+00004260: 0200 6403 0064 0300 6703 0083 0200 0188  ..d..d..g.......
+00004270: 0000 6a05 007c 0000 6a06 0083 0100 0188  ..j..|..j.......
+00004280: 0000 6a07 007c 0000 6403 0083 0200 7d01  ..j..|..d.....}.
+00004290: 0088 0000 6a08 006a 0900 6404 0083 0100  ....j..j..d.....
+000042a0: 7c01 0064 0500 196a 0a00 8300 006b 0600  |..d...j.....k..
+000042b0: 728d 007c 0100 6406 0019 7d02 007c 0100  r..|..d...}..|..
+000042c0: 6405 0019 7d03 006e 1400 7c01 0064 0500  d...}..n..|..d..
+000042d0: 197d 0200 7c01 0064 0600 197d 0300 8800  .}..|..d...}....
+000042e0: 006a 0b00 740c 007c 0200 6a06 0083 0200  .j..t..|..j.....
+000042f0: 0188 0000 6a04 007c 0200 6407 0064 0800  ....j..|..d..d..
+00004300: 6702 0083 0200 0188 0000 6a07 007c 0200  g.........j..|..
+00004310: 6407 0083 0200 7d04 0088 0000 6a05 007c  d.....}.....j..|
+00004320: 0400 6a06 0083 0100 0188 0000 6a04 007c  ..j.........j..|
+00004330: 0400 6409 0064 0a00 6702 0083 0200 0188  ..d..d..g.......
+00004340: 0000 6a07 007c 0200 6408 0083 0200 7d05  ..j..|..d.....}.
+00004350: 0088 0000 6a05 007c 0500 6a06 0083 0100  ....j..|..j.....
+00004360: 0188 0000 6a04 007c 0500 640b 0064 0c00  ....j..|..d..d..
+00004370: 640d 0067 0300 8302 0001 8800 006a 0800  d..g.........j..
+00004380: 6a09 0064 0b00 8301 007d 0600 8800 006a  j..d.....}.....j
+00004390: 0b00 740c 007c 0600 6a06 0083 0200 0188  ..t..|..j.......
+000043a0: 0000 6a08 006a 0900 640c 0083 0100 7d07  ..j..j..d.....}.
+000043b0: 0088 0000 6a0b 0074 0c00 7c07 006a 0600  ....j..t..|..j..
+000043c0: 8302 0001 8800 006a 0b00 740c 007c 0300  .......j..t..|..
+000043d0: 6a06 0083 0200 0188 0000 6a04 007c 0300  j.........j..|..
+000043e0: 6407 0064 0800 6702 0083 0200 0188 0000  d..d..g.........
+000043f0: 6a07 007c 0300 6407 0083 0200 7d04 0088  j..|..d.....}...
+00004400: 0000 6a05 007c 0400 6a06 0083 0100 0188  ..j..|..j.......
+00004410: 0000 6a04 007c 0400 640e 0064 0f00 6702  ..j..|..d..d..g.
+00004420: 0083 0200 0188 0000 6a07 007c 0300 6408  ........j..|..d.
+00004430: 0083 0200 7d05 0088 0000 6a05 007c 0500  ....}.....j..|..
+00004440: 6a06 0083 0100 0188 0000 6a04 007c 0500  j.........j..|..
+00004450: 6404 0064 1000 6702 0083 0200 0164 0000  d..d..g......d..
+00004460: 5328 1100 0000 4e52 4b00 0000 529e 0000  S(....NRK...R...
+00004470: 0052 4c00 0000 52a0 0000 0069 0000 0000  .RL...R....i....
+00004480: 6901 0000 0052 4e00 0000 524d 0000 0052  i....RN...RM...R
+00004490: 9800 0000 529f 0000 0052 a400 0000 52a5  ....R....R....R.
+000044a0: 0000 0052 a100 0000 52a2 0000 0052 a300  ...R....R....R..
+000044b0: 0000 52a6 0000 0028 0d00 0000 521e 0000  ..R....(....R...
+000044c0: 0052 0900 0000 520a 0000 0052 0b00 0000  .R....R....R....
+000044d0: 5222 0000 0052 8300 0000 5284 0000 0052  R"...R....R....R
+000044e0: 1a00 0000 5231 0000 0052 b700 0000 526d  ....R1...R....Rm
+000044f0: 0000 0074 0e00 0000 6173 7365 7274 4e6f  ...t....assertNo
+00004500: 7445 7175 616c 7405 0000 0046 616c 7365  tEqualt....False
+00004510: 2808 0000 0052 ac00 0000 527e 0000 0074  (....R....R~...t
+00004520: 1200 0000 6575 6172 6368 6f6e 746f 676c  ....euarchontogl
+00004530: 6972 6573 5f41 7412 0000 0065 7561 7263  ires_At....euarc
+00004540: 686f 6e74 6f67 6c69 7265 735f 4252 8000  hontoglires_BR..
+00004550: 0000 527f 0000 0074 0300 0000 6733 3674  ..R....t....g36t
+00004560: 0300 0000 6733 3728 0100 0000 5211 0000  ....g37(....R...
+00004570: 0028 0000 0000 733c 0000 002f 5573 6572  .(....s<.../User
+00004580: 732f 6164 7269 6161 6c2f 5265 706f 7369  s/adriaal/Reposi
+00004590: 746f 7269 6573 2f48 414d 2f74 6573 7473  tories/HAM/tests
+000045a0: 2f74 6573 745f 6f72 7468 6f78 6d6c 7061  /test_orthoxmlpa
+000045b0: 7273 6572 2e70 7952 9500 0000 9b01 0000  rser.pyR........
+000045c0: 733a 0000 0000 0219 0119 0110 0312 0222  s:............."
+000045d0: 010a 010d 020a 010a 0313 0116 0212 0110  ................
+000045e0: 0116 0212 0110 0119 0112 0113 0112 0113  ................
+000045f0: 0313 0116 0212 0110 0116 0212 0110 0152  ...............R
+00004600: 9700 0000 2802 0000 0052 3300 0000 528b  ....(....R3...R.
+00004610: 0000 0028 0200 0000 5211 0000 0052 9500  ...(....R....R..
+00004620: 0000 2800 0000 0028 0100 0000 5211 0000  ..(....(....R...
+00004630: 0073 3c00 0000 2f55 7365 7273 2f61 6472  .s<.../Users/adr
+00004640: 6961 616c 2f52 6570 6f73 6974 6f72 6965  iaal/Repositorie
+00004650: 732f 4841 4d2f 7465 7374 732f 7465 7374  s/HAM/tests/test
+00004660: 5f6f 7274 686f 786d 6c70 6172 7365 722e  _orthoxmlparser.
+00004670: 7079 7420 0000 0074 6573 745f 686f 675f  pyt ...test_hog_
+00004680: 7769 7468 5f6e 6573 7465 645f 6475 706c  with_nested_dupl
+00004690: 6963 6174 696f 6e99 0100 0073 0600 0000  ication....s....
+000046a0: 0002 0f2c 1101 6301 0000 0002 0000 0003  ...,..c.........
+000046b0: 0000 0003 0000 0073 3500 0000 8700 0066  .......s5......f
+000046c0: 0100 6401 0086 0000 7d01 007c 0100 8800  ..d.....}..|....
+000046d0: 006a 0000 6402 0019 8301 0001 7c01 0088  .j..d.......|...
+000046e0: 0000 6a01 0064 0200 1983 0100 0164 0000  ..j..d.......d..
+000046f0: 5328 0300 0000 4e63 0100 0000 0900 0000  S(....Nc........
+00004700: 0500 0000 1300 0000 73dd 0100 0088 0000  ........s.......
+00004710: 6a00 0064 0100 7c00 006a 0100 6a02 006a  j..d..|..j..j..j
+00004720: 0300 8302 0001 8800 006a 0400 7c00 0064  .........j..|..d
+00004730: 0200 6403 0067 0200 8302 0001 8800 006a  ..d..g.........j
+00004740: 0500 7c00 006a 0600 8301 0001 8800 006a  ..|..j.........j
+00004750: 0700 7c00 0064 0300 8302 007d 0100 8800  ..|..d.....}....
+00004760: 006a 0400 7c01 0064 0400 6405 0064 0500  .j..|..d..d..d..
+00004770: 6703 0083 0200 0188 0000 6a05 007c 0100  g.........j..|..
+00004780: 6a06 0083 0100 0188 0000 6a07 007c 0100  j.........j..|..
+00004790: 6405 0083 0200 7d02 0088 0000 6a08 006a  d.....}.....j..j
+000047a0: 0900 6406 0083 0100 7c02 0064 0700 196a  ..d.....|..d...j
+000047b0: 0a00 8300 006b 0600 72c5 007c 0200 6408  .....k..r..|..d.
+000047c0: 0019 7d03 007c 0200 6407 0019 7d04 006e  ..}..|..d...}..n
+000047d0: 1400 7c02 0064 0700 197d 0300 7c02 0064  ..|..d...}..|..d
+000047e0: 0800 197d 0400 8800 006a 0b00 740c 007c  ...}.....j..t..|
+000047f0: 0300 6a06 0083 0200 0188 0000 6a04 007c  ..j.........j..|
+00004800: 0300 6409 0067 0100 8302 0001 8800 006a  ..d..g.........j
+00004810: 0700 7c03 0064 0900 8302 007d 0500 8800  ..|..d.....}....
+00004820: 006a 0500 7c05 006a 0600 8301 0001 8800  .j..|..j........
+00004830: 006a 0400 7c05 0064 0a00 6701 0083 0200  .j..|..d..g.....
+00004840: 0188 0000 6a08 006a 0900 640a 0083 0100  ....j..j..d.....
+00004850: 7d06 0088 0000 6a00 0074 0c00 7c06 006a  }.....j..t..|..j
+00004860: 0600 8302 0001 8800 006a 0b00 740c 007c  .........j..t..|
+00004870: 0400 6a06 0083 0200 0188 0000 6a04 007c  ..j.........j..|
+00004880: 0400 640b 0067 0100 8302 0001 8800 006a  ..d..g.........j
+00004890: 0700 7c04 0064 0b00 8302 007d 0700 8800  ..|..d.....}....
+000048a0: 006a 0500 7c07 006a 0600 8301 0001 8800  .j..|..j........
+000048b0: 006a 0400 7c07 0064 0600 6701 0083 0200  .j..|..d..g.....
+000048c0: 0188 0000 6a08 006a 0900 6406 0083 0100  ....j..j..d.....
+000048d0: 7d08 0088 0000 6a00 0074 0c00 7c08 006a  }.....j..t..|..j
+000048e0: 0600 8302 0001 6400 0053 280c 0000 004e  ......d..S(....N
+000048f0: 524a 0000 0052 aa00 0000 524b 0000 0052  RJ...R....RK...R
+00004900: a900 0000 524c 0000 0052 a800 0000 6900  ....RL...R....i.
+00004910: 0000 0069 0100 0000 524e 0000 0052 a700  ...i....RN...R..
+00004920: 0000 524d 0000 0028 0d00 0000 521e 0000  ..RM...(....R...
+00004930: 0052 0900 0000 520a 0000 0052 0b00 0000  .R....R....R....
+00004940: 5222 0000 0052 8300 0000 5284 0000 0052  R"...R....R....R
+00004950: 1a00 0000 5231 0000 0052 b700 0000 526d  ....R1...R....Rm
+00004960: 0000 0052 bf00 0000 52c0 0000 0028 0900  ...R....R....(..
+00004970: 0000 52ad 0000 0052 7d00 0000 527e 0000  ..R....R}...R~..
+00004980: 0052 c100 0000 52c2 0000 0052 8000 0000  .R....R....R....
+00004990: 7403 0000 0067 3139 527f 0000 0074 0300  t....g19R....t..
+000049a0: 0000 6733 3828 0100 0000 5211 0000 0028  ..g38(....R....(
+000049b0: 0000 0000 733c 0000 002f 5573 6572 732f  ....s<.../Users/
+000049c0: 6164 7269 6161 6c2f 5265 706f 7369 746f  adriaal/Reposito
+000049d0: 7269 6573 2f48 414d 2f74 6573 7473 2f74  ries/HAM/tests/t
+000049e0: 6573 745f 6f72 7468 6f78 6d6c 7061 7273  est_orthoxmlpars
+000049f0: 6572 2e70 7952 9500 0000 cc01 0000 7334  er.pyR........s4
+00004a00: 0000 0000 0219 0116 0110 0312 0119 0110  ................
+00004a10: 0312 0222 010a 010d 020a 010a 0413 0113  ..."............
+00004a20: 0212 0110 0113 0112 0113 0313 0113 0212  ................
+00004a30: 0110 0113 0112 0152 9800 0000 2802 0000  .......R....(...
+00004a40: 0052 3300 0000 528b 0000 0028 0200 0000  .R3...R....(....
+00004a50: 5211 0000 0052 9500 0000 2800 0000 0028  R....R....(....(
+00004a60: 0100 0000 5211 0000 0073 3c00 0000 2f55  ....R....s<.../U
+00004a70: 7365 7273 2f61 6472 6961 616c 2f52 6570  sers/adriaal/Rep
+00004a80: 6f73 6974 6f72 6965 732f 4841 4d2f 7465  ositories/HAM/te
+00004a90: 7374 732f 7465 7374 5f6f 7274 686f 786d  sts/test_orthoxm
+00004aa0: 6c70 6172 7365 722e 7079 7420 0000 0074  lparser.pyt ...t
+00004ab0: 6573 745f 686f 675f 7769 7468 5f6c 6f73  est_hog_with_los
+00004ac0: 7365 735f 6475 706c 6963 6174 696f 6eca  ses_duplication.
+00004ad0: 0100 0073 0600 0000 0002 0f2a 1101 2811  ...s.......*..(.
+00004ae0: 0000 0052 0f00 0000 5288 0000 0052 1300  ...R....R....R..
+00004af0: 0000 521a 0000 0052 2200 0000 5239 0000  ..R....R"...R9..
+00004b00: 0052 9400 0000 5249 0000 0052 5400 0000  .R....RI...RT...
+00004b10: 525c 0000 0052 7c00 0000 5281 0000 0052  R\...R|...R....R
+00004b20: 8200 0000 5287 0000 0052 be00 0000 52c5  ....R....R....R.
+00004b30: 0000 0052 c800 0000 2800 0000 0028 0000  ...R....(....(..
+00004b40: 0000 2800 0000 0073 3c00 0000 2f55 7365  ..(....s<.../Use
+00004b50: 7273 2f61 6472 6961 616c 2f52 6570 6f73  rs/adriaal/Repos
+00004b60: 6974 6f72 6965 732f 4841 4d2f 7465 7374  itories/HAM/test
+00004b70: 732f 7465 7374 5f6f 7274 686f 786d 6c70  s/test_orthoxmlp
+00004b80: 6172 7365 722e 7079 5289 0000 00a7 0000  arser.pyR.......
+00004b90: 0073 1e00 0000 0601 090a 0909 0905 0910  .s..............
+00004ba0: 090b 090d 090c 090c 0929 091a 0916 091e  .........)......
+00004bb0: 0922 0931 7408 0000 005f 5f6d 6169 6e5f  .".1t....__main_
+00004bc0: 5f28 0c00 0000 5241 0000 0074 0800 0000  _(....RA...t....
+00004bd0: 756e 6974 7465 7374 528f 0000 0052 0000  unittestR....R..
+00004be0: 0000 5201 0000 0052 2900 0000 5202 0000  ..R....R)...R...
+00004bf0: 0074 0800 0000 5465 7374 4361 7365 5203  .t....TestCaseR.
+00004c00: 0000 0052 8900 0000 520f 0000 0074 0400  ...R....R....t..
+00004c10: 0000 6d61 696e 2800 0000 0028 0000 0000  ..main(....(....
+00004c20: 2800 0000 0073 3c00 0000 2f55 7365 7273  (....s<.../Users
+00004c30: 2f61 6472 6961 616c 2f52 6570 6f73 6974  /adriaal/Reposit
+00004c40: 6f72 6965 732f 4841 4d2f 7465 7374 732f  ories/HAM/tests/
+00004c50: 7465 7374 5f6f 7274 686f 786d 6c70 6172  test_orthoxmlpar
+00004c60: 7365 722e 7079 7408 0000 003c 6d6f 6475  ser.pyt....<modu
+00004c70: 6c65 3e01 0000 0073 1400 0000 0c01 0c01  le>....s........
+00004c80: 1001 1001 0c01 1003 199e 19ff 0058 0c01  .............X..
```

### Comparing `pyham-1.1.8/tests/test_mapper.py` & `pyham-1.1.9/tests/test_mapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,23 @@
 import unittest
 from pyham import ham
 from pyham import utils
 from pyham import HOGsMap, MapLateral, MapVertical
 import os
 
 def _str_array(array):
-    array_converted = []
-    for e in array:
-        array_converted.append(str(e))
-    return array_converted
+    return set(str(e) for e in array)
 
 
 def _str_dict_one_value(dict):
-    for kk in dict.keys():
-        dict[str(kk)] = dict.pop(kk)
-    for k, v in dict.items():
-        dict[k] = str(v)
-    return dict
+    return {str(key): str(val) for key, val in dict.items()}
 
 
 def _str_dict_array_value(dict):
-    for kk in dict.keys():
-        dict[str(kk)] = dict.pop(kk)
-    for k, vs in dict.items():
-        array = []
-        for v in vs:
-            array.append(str(v))
-        dict[k] = set(array)
-    return dict
+    return {str(key): set(str(v) for v in val) for key, val in dict.items()}
 
 
 class MapperTestCases:
 
     class MapperTest(unittest.TestCase):
         def setUp(self):
 
@@ -190,15 +176,15 @@
     def test_get_lost(self):
         vertical_map = MapVertical(self.ham_analysis)
         map = HOGsMap(self.ham_analysis, self.human, self.euarchontoglires)
         self.assertTrue(map.consistent)
         vertical_map.add_map(map)
 
         loss = vertical_map.get_lost()
-        self.assertEqual(["<HOG(3.E.2)>"], _str_array(loss))
+        self.assertEqual(set(["<HOG(3.E.2)>"]), _str_array(loss))
 
         vertical_map2 = MapVertical(self.ham_analysis)
         map2 = HOGsMap(self.ham_analysis, self.rat, self.euarchontoglires)
         self.assertTrue(map2.consistent)
         vertical_map2.add_map(map2)
 
         loss2 = vertical_map2.get_lost()
```

### Comparing `pyham-1.1.8/tests/test_taxonomy.py` & `pyham-1.1.9/tests/test_taxonomy.py`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/tests/test_mapper.pyc` & `pyham-1.1.9/tests/test_mapper.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 2.7 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 03f3 0d0a 6e8c e85e 6300 0000 0000 0000  ....n..^c.......
+00000000: 03f3 0d0a 0bc8 8f5b 6300 0000 0000 0000  .......[c.......
 00000010: 0003 0000 0040 0000 0073 ea00 0000 6400  .....@...s....d.
 00000020: 0064 0100 6c00 005a 0000 6400 0064 0200  .d..l..Z..d..d..
 00000030: 6c01 006d 0200 5a02 0001 6400 0064 0300  l..m..Z...d..d..
 00000040: 6c01 006d 0300 5a03 0001 6400 0064 0400  l..m..Z...d..d..
 00000050: 6c01 006d 0400 5a04 006d 0500 5a05 006d  l..m..Z..m..Z..m
 00000060: 0600 5a06 0001 6400 0064 0100 6c07 005a  ..Z...d..d..l..Z
 00000070: 0700 6405 0084 0000 5a08 0064 0600 8400  ..d.....Z..d....
@@ -25,949 +25,905 @@
 00000180: 0044 5d19 007d 0200 7c01 006a 0000 7401  .D]..}..|..j..t.
 00000190: 007c 0200 8301 0083 0100 0171 0d00 577c  .|.........q..W|
 000001a0: 0100 5328 0100 0000 4e28 0200 0000 7406  ..S(....N(....t.
 000001b0: 0000 0061 7070 656e 6474 0300 0000 7374  ...appendt....st
 000001c0: 7228 0300 0000 7405 0000 0061 7272 6179  r(....t....array
 000001d0: 740f 0000 0061 7272 6179 5f63 6f6e 7665  t....array_conve
 000001e0: 7274 6564 7401 0000 0065 2800 0000 0028  rtedt....e(....(
-000001f0: 0000 0000 7347 0000 002f 5573 6572 732f  ....sG.../Users/
-00000200: 6164 6d69 6e2f 576f 726b 2f70 726f 6a65  admin/Work/proje
-00000210: 6374 2f44 6573 7369 6d6f 7a2f 7079 6861  ct/Dessimoz/pyha
-00000220: 6d2d 6465 762f 7079 6861 6d2f 7465 7374  m-dev/pyham/test
-00000230: 732f 7465 7374 5f6d 6170 7065 722e 7079  s/test_mapper.py
-00000240: 740a 0000 005f 7374 725f 6172 7261 7907  t...._str_array.
-00000250: 0000 0073 0800 0000 0001 0601 0d01 1701  ...s............
-00000260: 6301 0000 0004 0000 0005 0000 0043 0000  c............C..
-00000270: 0073 6100 0000 782d 007c 0000 6a00 0083  .sa...x-.|..j...
-00000280: 0000 445d 1f00 7d01 007c 0000 6a01 007c  ..D]..}..|..j..|
-00000290: 0100 8301 007c 0000 7402 007c 0100 8301  .....|..t..|....
-000002a0: 003c 710d 0057 782a 007c 0000 6a03 0083  .<q..Wx*.|..j...
-000002b0: 0000 445d 1c00 5c02 007d 0200 7d03 0074  ..D]..\..}..}..t
-000002c0: 0200 7c03 0083 0100 7c00 007c 0200 3c71  ..|.....|..|..<q
-000002d0: 3d00 577c 0000 5328 0100 0000 4e28 0400  =.W|..S(....N(..
-000002e0: 0000 7404 0000 006b 6579 7374 0300 0000  ..t....keyst....
-000002f0: 706f 7052 0600 0000 7405 0000 0069 7465  popR....t....ite
-00000300: 6d73 2804 0000 0074 0400 0000 6469 6374  ms(....t....dict
-00000310: 7402 0000 006b 6b74 0100 0000 6b74 0100  t....kkt....kt..
-00000320: 0000 7628 0000 0000 2800 0000 0073 4700  ..v(....(....sG.
-00000330: 0000 2f55 7365 7273 2f61 646d 696e 2f57  ../Users/admin/W
-00000340: 6f72 6b2f 7072 6f6a 6563 742f 4465 7373  ork/project/Dess
-00000350: 696d 6f7a 2f70 7968 616d 2d64 6576 2f70  imoz/pyham-dev/p
-00000360: 7968 616d 2f74 6573 7473 2f74 6573 745f  yham/tests/test_
-00000370: 6d61 7070 6572 2e70 7974 1300 0000 5f73  mapper.pyt...._s
-00000380: 7472 5f64 6963 745f 6f6e 655f 7661 6c75  tr_dict_one_valu
-00000390: 650e 0000 0073 0a00 0000 0001 1301 1d01  e....s..........
-000003a0: 1901 1401 6301 0000 0006 0000 0005 0000  ....c...........
-000003b0: 0043 0000 0073 8b00 0000 782d 007c 0000  .C...s....x-.|..
-000003c0: 6a00 0083 0000 445d 1f00 7d01 007c 0000  j.....D]..}..|..
-000003d0: 6a01 007c 0100 8301 007c 0000 7402 007c  j..|.....|..t..|
-000003e0: 0100 8301 003c 710d 0057 7854 007c 0000  .....<q..WxT.|..
-000003f0: 6a03 0083 0000 445d 4600 5c02 007d 0200  j.....D]F.\..}..
-00000400: 7d03 0067 0000 7d04 0078 2100 7c03 0044  }..g..}..x!.|..D
-00000410: 5d19 007d 0500 7c04 006a 0400 7402 007c  ]..}..|..j..t..|
-00000420: 0500 8301 0083 0100 0171 5600 5774 0500  .........qV.Wt..
-00000430: 7c04 0083 0100 7c00 007c 0200 3c71 3d00  |.....|..|..<q=.
-00000440: 577c 0000 5328 0100 0000 4e28 0600 0000  W|..S(....N(....
-00000450: 520b 0000 0052 0c00 0000 5206 0000 0052  R....R....R....R
-00000460: 0d00 0000 5205 0000 0074 0300 0000 7365  ....R....t....se
-00000470: 7428 0600 0000 520e 0000 0052 0f00 0000  t(....R....R....
-00000480: 5210 0000 0074 0200 0000 7673 5207 0000  R....t....vsR...
-00000490: 0052 1100 0000 2800 0000 0028 0000 0000  .R....(....(....
-000004a0: 7347 0000 002f 5573 6572 732f 6164 6d69  sG.../Users/admi
-000004b0: 6e2f 576f 726b 2f70 726f 6a65 6374 2f44  n/Work/project/D
-000004c0: 6573 7369 6d6f 7a2f 7079 6861 6d2d 6465  essimoz/pyham-de
-000004d0: 762f 7079 6861 6d2f 7465 7374 732f 7465  v/pyham/tests/te
-000004e0: 7374 5f6d 6170 7065 722e 7079 7415 0000  st_mapper.pyt...
-000004f0: 005f 7374 725f 6469 6374 5f61 7272 6179  ._str_dict_array
-00000500: 5f76 616c 7565 1600 0000 7310 0000 0000  _value....s.....
-00000510: 0113 011d 0119 0106 010d 0117 0114 0174  ...............t
-00000520: 0f00 0000 4d61 7070 6572 5465 7374 4361  ....MapperTestCa
-00000530: 7365 7363 0000 0000 0000 0000 0300 0000  sesc............
-00000540: 4200 0000 7321 0000 0065 0000 5a01 0064  B...s!...e..Z..d
-00000550: 0000 6502 006a 0300 6601 0064 0100 8400  ..e..j..f..d....
-00000560: 0083 0000 595a 0400 5253 2802 0000 0074  ....YZ..RS(....t
-00000570: 0a00 0000 4d61 7070 6572 5465 7374 6300  ....MapperTestc.
-00000580: 0000 0000 0000 0001 0000 0042 0000 0073  ...........B...s
-00000590: 1100 0000 6500 005a 0100 6400 0084 0000  ....e..Z..d.....
-000005a0: 5a02 0052 5328 0100 0000 6301 0000 0004  Z..RS(....c.....
-000005b0: 0000 0009 0000 0043 0000 0073 7e01 0000  .......C...s~...
-000005c0: 7400 006a 0100 6a02 0074 0000 6a01 006a  t..j..j..t..j..j
-000005d0: 0300 7404 0083 0100 6401 0083 0200 7d01  ..t.....d.....}.
-000005e0: 0074 0500 6a06 007c 0100 6402 0064 0300  .t..j..|..d..d..
-000005f0: 8301 017d 0200 7400 006a 0100 6a02 0074  ...}..t..j..j..t
-00000600: 0000 6a01 006a 0300 7404 0083 0100 6404  ..j..j..t.....d.
-00000610: 0083 0200 7d03 0074 0700 6a08 0064 0500  ....}..t..j..d..
-00000620: 7c02 0064 0600 7c03 0064 0700 6408 0064  |..d..|..d..d..d
-00000630: 0900 7409 0083 0004 7c00 005f 0a00 7c00  ..t.....|.._..|.
-00000640: 006a 0a00 6a0b 0064 0a00 640b 0083 0001  .j..j..d..d.....
-00000650: 7c00 005f 0c00 7c00 006a 0a00 6a0b 0064  |.._..|..j..j..d
-00000660: 0a00 640c 0083 0001 7c00 005f 0d00 7c00  ..d.....|.._..|.
-00000670: 006a 0a00 6a0b 0064 0a00 640d 0083 0001  .j..j..d..d.....
-00000680: 7c00 005f 0e00 7c00 006a 0a00 6a0b 0064  |.._..|..j..j..d
-00000690: 0a00 640e 0083 0001 7c00 005f 0f00 7c00  ..d.....|.._..|.
-000006a0: 006a 0a00 6a0b 0064 0a00 640f 0083 0001  .j..j..d..d.....
-000006b0: 7c00 005f 1000 7c00 006a 0a00 6a11 007c  |.._..|..j..j..|
-000006c0: 0000 6a0c 007c 0000 6a0d 0068 0200 8301  ..j..|..j..h....
-000006d0: 007c 0000 5f12 007c 0000 6a0a 006a 1100  .|.._..|..j..j..
-000006e0: 7c00 006a 0e00 7c00 006a 0f00 6802 0083  |..j..|..j..h...
-000006f0: 0100 7c00 005f 1300 7c00 006a 0a00 6a11  ..|.._..|..j..j.
-00000700: 007c 0000 6a0c 007c 0000 6a10 0068 0200  .|..j..|..j..h..
-00000710: 8301 007c 0000 5f14 007c 0000 6a0a 006a  ...|.._..|..j..j
-00000720: 1100 7c00 006a 0c00 7c00 006a 0e00 6802  ..|..j..|..j..h.
-00000730: 0083 0100 7c00 005f 1500 6400 0053 2810  ....|.._..d..S(.
-00000740: 0000 004e 7313 0000 002e 2f64 6174 612f  ...Ns...../data/
-00000750: 7369 6d70 6c65 4578 2e6e 776b 7404 0000  simpleEx.nwkt...
-00000760: 0074 7970 6574 0300 0000 6e77 6b73 1800  .typet....nwks..
-00000770: 0000 2e2f 6461 7461 2f73 696d 706c 6545  .../data/simpleE
-00000780: 782e 6f72 7468 6f78 6d6c 7409 0000 0074  x.orthoxmlt....t
-00000790: 7265 655f 6669 6c65 7408 0000 0068 6f67  ree_filet....hog
-000007a0: 5f66 696c 6574 0d00 0000 7479 7065 5f68  _filet....type_h
-000007b0: 6f67 5f66 696c 6574 0800 0000 6f72 7468  og_filet....orth
-000007c0: 6f78 6d6c 7411 0000 0075 7365 5f69 6e74  oxmlt....use_int
-000007d0: 6572 6e61 6c5f 6e61 6d65 7404 0000 006e  ernal_namet....n
-000007e0: 616d 6574 0500 0000 4855 4d41 4e74 0500  amet....HUMANt..
-000007f0: 0000 5845 4e54 5274 0500 0000 4d4f 5553  ..XENTRt....MOUS
-00000800: 4574 0500 0000 5241 544e 4f74 0500 0000  Et....RATNOt....
-00000810: 5041 4e54 5228 1600 0000 7402 0000 006f  PANTR(....t....o
-00000820: 7374 0400 0000 7061 7468 7404 0000 006a  st....patht....j
-00000830: 6f69 6e74 0700 0000 6469 726e 616d 6574  oint....dirnamet
-00000840: 0800 0000 5f5f 6669 6c65 5f5f 5201 0000  ....__file__R...
-00000850: 0074 1100 0000 6765 745f 6e65 7769 636b  .t....get_newick
-00000860: 5f73 7472 696e 6752 0000 0000 7403 0000  _stringR....t...
-00000870: 0048 616d 7404 0000 0054 7275 6574 0c00  .Hamt....Truet..
-00000880: 0000 6861 6d5f 616e 616c 7973 6973 7419  ..ham_analysist.
-00000890: 0000 0067 6574 5f65 7874 616e 745f 6765  ...get_extant_ge
-000008a0: 6e6f 6d65 5f62 795f 6e61 6d65 7405 0000  nome_by_namet...
-000008b0: 0068 756d 616e 7404 0000 0066 726f 6774  .humant....frogt
-000008c0: 0500 0000 6d6f 7573 6574 0300 0000 7261  ....mouset....ra
-000008d0: 7474 0500 0000 6368 696d 7074 2a00 0000  tt....chimpt*...
-000008e0: 6765 745f 616e 6365 7374 7261 6c5f 6765  get_ancestral_ge
-000008f0: 6e6f 6d65 5f62 795f 6d72 6361 5f6f 665f  nome_by_mrca_of_
-00000900: 6765 6e6f 6d65 5f73 6574 740b 0000 0076  genome_sett....v
-00000910: 6572 7465 6272 6174 6573 7407 0000 0072  ertebratest....r
-00000920: 6f64 656e 7473 7408 0000 0070 7269 6d61  odentst....prima
-00000930: 7465 7374 1000 0000 6575 6172 6368 6f6e  test....euarchon
-00000940: 746f 676c 6972 6573 2804 0000 0074 0400  toglires(....t..
-00000950: 0000 7365 6c66 7408 0000 006e 776b 5f70  ..selft....nwk_p
-00000960: 6174 6874 0800 0000 7472 6565 5f73 7472  atht....tree_str
-00000970: 740d 0000 006f 7274 686f 786d 6c5f 7061  t....orthoxml_pa
-00000980: 7468 2800 0000 0028 0000 0000 7347 0000  th(....(....sG..
-00000990: 002f 5573 6572 732f 6164 6d69 6e2f 576f  ./Users/admin/Wo
-000009a0: 726b 2f70 726f 6a65 6374 2f44 6573 7369  rk/project/Dessi
-000009b0: 6d6f 7a2f 7079 6861 6d2d 6465 762f 7079  moz/pyham-dev/py
-000009c0: 6861 6d2f 7465 7374 732f 7465 7374 5f6d  ham/tests/test_m
-000009d0: 6170 7065 722e 7079 7405 0000 0073 6574  apper.pyt....set
-000009e0: 5570 2400 0000 731c 0000 0000 0221 0115  Up$...s......!..
-000009f0: 0121 0227 0218 0118 0118 0118 0118 0121  .!.'...........!
-00000a00: 0121 0121 0109 0128 0300 0000 7408 0000  .!.!...(....t...
-00000a10: 005f 5f6e 616d 655f 5f74 0a00 0000 5f5f  .__name__t....__
-00000a20: 6d6f 6475 6c65 5f5f 523d 0000 0028 0000  module__R=...(..
-00000a30: 0000 2800 0000 0028 0000 0000 7347 0000  ..(....(....sG..
-00000a40: 002f 5573 6572 732f 6164 6d69 6e2f 576f  ./Users/admin/Wo
-00000a50: 726b 2f70 726f 6a65 6374 2f44 6573 7369  rk/project/Dessi
-00000a60: 6d6f 7a2f 7079 6861 6d2d 6465 762f 7079  moz/pyham-dev/py
-00000a70: 6861 6d2f 7465 7374 732f 7465 7374 5f6d  ham/tests/test_m
-00000a80: 6170 7065 722e 7079 5217 0000 0023 0000  apper.pyR....#..
-00000a90: 0073 0200 0000 0601 2805 0000 0052 3e00  .s......(....R>.
-00000aa0: 0000 523f 0000 0074 0800 0000 756e 6974  ..R?...t....unit
-00000ab0: 7465 7374 7408 0000 0054 6573 7443 6173  testt....TestCas
-00000ac0: 6552 1700 0000 2800 0000 0028 0000 0000  eR....(....(....
-00000ad0: 2800 0000 0073 4700 0000 2f55 7365 7273  (....sG.../Users
-00000ae0: 2f61 646d 696e 2f57 6f72 6b2f 7072 6f6a  /admin/Work/proj
-00000af0: 6563 742f 4465 7373 696d 6f7a 2f70 7968  ect/Dessimoz/pyh
-00000b00: 616d 2d64 6576 2f70 7968 616d 2f74 6573  am-dev/pyham/tes
-00000b10: 7473 2f74 6573 745f 6d61 7070 6572 2e70  ts/test_mapper.p
-00000b20: 7952 1600 0000 2100 0000 7302 0000 0006  yR....!...s.....
-00000b30: 0274 0b00 0000 484f 4773 4d61 7054 6573  .t....HOGsMapTes
-00000b40: 7463 0000 0000 0000 0000 0100 0000 4200  tc............B.
-00000b50: 0000 733e 0000 0065 0000 5a01 0064 0000  ..s>...e..Z..d..
-00000b60: 8400 005a 0200 6401 0084 0000 5a03 0064  ...Z..d.....Z..d
-00000b70: 0200 8400 005a 0400 6403 0084 0000 5a05  .....Z..d.....Z.
-00000b80: 0064 0400 8400 005a 0600 6405 0084 0000  .d.....Z..d.....
-00000b90: 5a07 0052 5328 0600 0000 6302 0000 0002  Z..RS(....c.....
-00000ba0: 0000 0005 0000 0043 0000 0073 9500 0000  .......C...s....
-00000bb0: 7400 007c 0100 7401 006a 0200 6a03 0083  t..|..t..j..j...
-00000bc0: 0200 721c 007c 0100 6a04 0053 7400 007c  ..r..|..j..St..|
-00000bd0: 0100 7401 006a 0200 6a05 0083 0200 7257  ..t..j..j.....rW
-00000be0: 007c 0100 6a06 0064 0000 6b03 0072 4700  .|..j..d..k..rG.
-00000bf0: 7c01 006a 0600 537c 0100 6a08 006a 0900  |..j..S|..j..j..
-00000c00: 6a0a 0053 6e3a 007c 0100 6400 006b 0200  j..Sn:.|..d..k..
-00000c10: 7267 007c 0100 5374 0b00 6401 006a 0c00  rg.|..St..d..j..
-00000c20: 7401 006a 0200 6a0d 006a 0e00 740f 007c  t..j..j..j..t..|
-00000c30: 0100 8301 006a 0e00 8302 0083 0100 8201  .....j..........
-00000c40: 0064 0000 5328 0200 0000 4e73 2300 0000  .d..S(....Ns#...
-00000c50: 6578 7065 6374 2073 7562 636c 6173 7320  expect subclass 
-00000c60: 6f62 6a20 6f66 2027 7b7d 272c 2067 6f74  obj of '{}', got
-00000c70: 207b 7d28 1000 0000 740a 0000 0069 7369   {}(....t....isi
-00000c80: 6e73 7461 6e63 6552 0000 0000 740c 0000  nstanceR....t...
-00000c90: 0061 6273 7472 6163 7467 656e 6574 0400  .abstractgenet..
-00000ca0: 0000 4765 6e65 7409 0000 0075 6e69 7175  ..Genet....uniqu
-00000cb0: 655f 6964 7403 0000 0048 4f47 7406 0000  e_idt....HOGt...
-00000cc0: 0068 6f67 5f69 6474 0400 0000 4e6f 6e65  .hog_idt....None
-00000cd0: 7406 0000 0067 656e 6f6d 6574 0500 0000  t....genomet....
-00000ce0: 7461 786f 6e52 1f00 0000 7409 0000 0054  taxonR....t....T
-00000cf0: 7970 6545 7272 6f72 7406 0000 0066 6f72  ypeErrort....for
-00000d00: 6d61 7474 0c00 0000 4162 7374 7261 6374  matt....Abstract
-00000d10: 4765 6e65 523e 0000 0052 1800 0000 2802  GeneR>...R....(.
-00000d20: 0000 0052 3900 0000 7404 0000 0069 7465  ...R9...t....ite
-00000d30: 6d28 0000 0000 2800 0000 0073 4700 0000  m(....(....sG...
-00000d40: 2f55 7365 7273 2f61 646d 696e 2f57 6f72  /Users/admin/Wor
-00000d50: 6b2f 7072 6f6a 6563 742f 4465 7373 696d  k/project/Dessim
-00000d60: 6f7a 2f70 7968 616d 2d64 6576 2f70 7968  oz/pyham-dev/pyh
-00000d70: 616d 2f74 6573 7473 2f74 6573 745f 6d61  am/tests/test_ma
-00000d80: 7070 6572 2e70 7974 0f00 0000 5f67 6574  pper.pyt...._get
-00000d90: 5f69 6465 6e74 6966 6965 723a 0000 0073  _identifier:...s
-00000da0: 1600 0000 0001 1501 0701 1501 0f01 0702  ................
-00000db0: 1001 0c01 0402 0901 0c01 6302 0000 0003  ..........c.....
-00000dc0: 0000 0002 0000 0043 0000 0073 2c00 0000  .......C...s,...
-00000dd0: 7c01 007d 0200 781c 007c 0200 6a00 0064  |..}..x..|..j..d
-00000de0: 0000 6b09 0072 2400 7c02 006a 0000 7d02  ..k..r$.|..j..}.
-00000df0: 0071 0900 577c 0200 6a02 0053 2801 0000  .q..W|..j..S(...
-00000e00: 004e 2803 0000 0074 0600 0000 7061 7265  .N(....t....pare
-00000e10: 6e74 5249 0000 0052 4800 0000 2803 0000  ntRI...RH...(...
-00000e20: 0052 3900 0000 7403 0000 0068 6f67 740b  .R9...t....hogt.
-00000e30: 0000 0063 7572 7265 6e74 5f68 6f67 2800  ...current_hog(.
-00000e40: 0000 0028 0000 0000 7347 0000 002f 5573  ...(....sG.../Us
-00000e50: 6572 732f 6164 6d69 6e2f 576f 726b 2f70  ers/admin/Work/p
-00000e60: 726f 6a65 6374 2f44 6573 7369 6d6f 7a2f  roject/Dessimoz/
-00000e70: 7079 6861 6d2d 6465 762f 7079 6861 6d2f  pyham-dev/pyham/
-00000e80: 7465 7374 732f 7465 7374 5f6d 6170 7065  tests/test_mappe
-00000e90: 722e 7079 7410 0000 005f 6765 745f 746f  r.pyt...._get_to
-00000ea0: 704c 6576 656c 5f69 6449 0000 0073 0800  pLevel_idI...s..
-00000eb0: 0000 0001 0601 1201 0d01 6301 0000 0002  ..........c.....
-00000ec0: 0000 0004 0000 0043 0000 0073 5e00 0000  .......C...s^...
-00000ed0: 7400 007c 0000 6a01 007c 0000 6a02 007c  t..|..j..|..j..|
-00000ee0: 0000 6a03 0083 0300 7d01 007c 0000 6a04  ..j.....}..|..j.
-00000ef0: 007c 0100 6a05 0083 0100 017c 0000 6a06  .|..j......|..j.
-00000f00: 0064 0100 7c01 006a 0700 6a08 006a 0900  .d..|..j..j..j..
-00000f10: 8302 0001 7c00 006a 0600 7c00 006a 0200  ....|..j..|..j..
-00000f20: 7c01 006a 0a00 8302 0001 6400 0053 2802  |..j......d..S(.
-00000f30: 0000 004e 7410 0000 0045 7561 7263 686f  ...Nt....Euarcho
-00000f40: 6e74 6f67 6c69 7265 7328 0b00 0000 5202  ntoglires(....R.
-00000f50: 0000 0052 2d00 0000 522f 0000 0052 3800  ...R-...R/...R8.
-00000f60: 0000 740a 0000 0061 7373 6572 7454 7275  ..t....assertTru
-00000f70: 6574 0a00 0000 636f 6e73 6973 7465 6e74  et....consistent
-00000f80: 740b 0000 0061 7373 6572 7445 7175 616c  t....assertEqual
-00000f90: 7408 0000 0061 6e63 6573 746f 7252 4b00  t....ancestorRK.
-00000fa0: 0000 521f 0000 0074 0a00 0000 6465 7363  ..R....t....desc
-00000fb0: 656e 6461 6e74 2802 0000 0052 3900 0000  endant(....R9...
-00000fc0: 7403 0000 006d 6170 2800 0000 0028 0000  t....map(....(..
-00000fd0: 0000 7347 0000 002f 5573 6572 732f 6164  ..sG.../Users/ad
-00000fe0: 6d69 6e2f 576f 726b 2f70 726f 6a65 6374  min/Work/project
-00000ff0: 2f44 6573 7369 6d6f 7a2f 7079 6861 6d2d  /Dessimoz/pyham-
-00001000: 6465 762f 7079 6861 6d2f 7465 7374 732f  dev/pyham/tests/
-00001010: 7465 7374 5f6d 6170 7065 722e 7079 7420  test_mapper.pyt 
-00001020: 0000 0074 6573 745f 7365 745f 616e 6365  ...test_set_ance
-00001030: 7374 6f72 5f61 6e64 5f64 6573 6365 6e64  stor_and_descend
-00001040: 616e 744f 0000 0073 0800 0000 0003 1b01  antO...s........
-00001050: 1001 1901 6301 0000 0002 0000 0008 0000  ....c...........
-00001060: 0043 0000 0073 4500 0000 7c00 006a 0000  .C...sE...|..j..
-00001070: 7401 0083 0100 8f30 0001 7402 007c 0000  t......0..t..|..
-00001080: 6a03 007c 0000 6a04 007c 0000 6a05 0083  j..|..j..|..j...
-00001090: 0300 7d01 007c 0000 6a06 007c 0100 6a07  ..}..|..j..|..j.
-000010a0: 0083 0100 0157 6400 0051 5864 0000 5328  .....Wd..QXd..S(
-000010b0: 0100 0000 4e28 0800 0000 740c 0000 0061  ....N(....t....a
-000010c0: 7373 6572 7452 6169 7365 7352 4c00 0000  ssertRaisesRL...
-000010d0: 5202 0000 0052 2d00 0000 5230 0000 0052  R....R-...R0...R
-000010e0: 3700 0000 5256 0000 0052 5700 0000 2802  7...RV...RW...(.
-000010f0: 0000 0052 3900 0000 7404 0000 006d 6170  ...R9...t....map
-00001100: 3228 0000 0000 2800 0000 0073 4700 0000  2(....(....sG...
-00001110: 2f55 7365 7273 2f61 646d 696e 2f57 6f72  /Users/admin/Wor
-00001120: 6b2f 7072 6f6a 6563 742f 4465 7373 696d  k/project/Dessim
-00001130: 6f7a 2f70 7968 616d 2d64 6576 2f70 7968  oz/pyham-dev/pyh
-00001140: 616d 2f74 6573 7473 2f74 6573 745f 6d61  am/tests/test_ma
-00001150: 7070 6572 2e70 7974 1e00 0000 7465 7374  pper.pyt....test
-00001160: 5f61 6464 5f67 656e 6f6d 655f 6e6f 745f  _add_genome_not_
-00001170: 6f6e 5f6c 696e 6561 6765 5700 0000 7306  on_lineageW...s.
-00001180: 0000 0000 0210 011b 0163 0100 0000 0500  .........c......
-00001190: 0000 0400 0000 0300 0000 737f 0000 0087  ..........s.....
-000011a0: 0000 6601 0064 0100 8600 007d 0100 7400  ..f..d.....}..t.
-000011b0: 0088 0000 6a01 0088 0000 6a02 0088 0000  ....j.....j.....
-000011c0: 6a03 0083 0300 7d02 0088 0000 6a04 007c  j.....}.....j..|
-000011d0: 0200 6a05 0083 0100 0169 0400 6402 0064  ..j......i..d..d
-000011e0: 0200 3664 0000 6403 0036 6404 0064 0400  ..6d..d..6d..d..
-000011f0: 3664 0000 6405 0036 7d03 007c 0100 7c02  6d..d..6}..|..|.
-00001200: 006a 0700 8301 007d 0400 8800 006a 0800  .j.....}.....j..
-00001210: 7c03 007c 0400 8302 0001 6400 0053 2806  |..|......d..S(.
-00001220: 0000 004e 6301 0000 0004 0000 0005 0000  ...Nc...........
-00001230: 0013 0000 0073 4700 0000 6900 007d 0100  .....sG...i..}..
-00001240: 783a 007c 0000 6a00 0083 0000 445d 2c00  x:.|..j.....D],.
-00001250: 5c02 007d 0200 7d03 0088 0000 6a01 007c  \..}..}.....j..|
-00001260: 0300 6401 0019 8301 007c 0100 8800 006a  ..d......|.....j
-00001270: 0100 7c02 0083 0100 3c71 1300 577c 0100  ..|.....<q..W|..
-00001280: 5328 0200 0000 4e69 0000 0000 2802 0000  S(....Ni....(...
-00001290: 0052 0d00 0000 5250 0000 0028 0400 0000  .R....RP...(....
-000012a0: 740c 0000 0073 696e 676c 655f 6d61 7055  t....single_mapU
-000012b0: 7074 0c00 0000 6f62 7365 7276 6564 5f6d  pt....observed_m
-000012c0: 6170 7406 0000 0073 6f75 7263 6574 0600  apt....sourcet..
-000012d0: 0000 7461 7267 6574 2801 0000 0052 3900  ..target(....R9.
-000012e0: 0000 2800 0000 0073 4700 0000 2f55 7365  ..(....sG.../Use
-000012f0: 7273 2f61 646d 696e 2f57 6f72 6b2f 7072  rs/admin/Work/pr
-00001300: 6f6a 6563 742f 4465 7373 696d 6f7a 2f70  oject/Dessimoz/p
-00001310: 7968 616d 2d64 6576 2f70 7968 616d 2f74  yham-dev/pyham/t
-00001320: 6573 7473 2f74 6573 745f 6d61 7070 6572  ests/test_mapper
-00001330: 2e70 7974 0c00 0000 5f63 6f6e 7665 7274  .pyt...._convert
-00001340: 5f6d 6170 5f00 0000 7308 0000 0000 0106  _map_...s.......
-00001350: 0119 0124 0174 0100 0000 3174 0100 0000  ...$.t....1t....
-00001360: 3274 0100 0000 3374 0100 0000 3528 0900  2t....3t....5(..
-00001370: 0000 5202 0000 0052 2d00 0000 522f 0000  ..R....R-...R/..
-00001380: 0052 3500 0000 5256 0000 0052 5700 0000  .R5...RV...RW...
-00001390: 5249 0000 0074 0500 0000 7570 4d61 7074  RI...t....upMapt
-000013a0: 0f00 0000 6173 7365 7274 4469 6374 4571  ....assertDictEq
-000013b0: 7561 6c28 0500 0000 5239 0000 0052 6400  ual(....R9...Rd.
-000013c0: 0000 525b 0000 0074 0c00 0000 6578 7065  ..R[...t....expe
-000013d0: 6374 6564 5f6d 6170 5261 0000 0028 0000  cted_mapRa...(..
-000013e0: 0000 2801 0000 0052 3900 0000 7347 0000  ..(....R9...sG..
-000013f0: 002f 5573 6572 732f 6164 6d69 6e2f 576f  ./Users/admin/Wo
-00001400: 726b 2f70 726f 6a65 6374 2f44 6573 7369  rk/project/Dessi
-00001410: 6d6f 7a2f 7079 6861 6d2d 6465 762f 7079  moz/pyham-dev/py
-00001420: 6861 6d2f 7465 7374 732f 7465 7374 5f6d  ham/tests/test_m
-00001430: 6170 7065 722e 7079 740a 0000 0074 6573  apper.pyt....tes
-00001440: 745f 5570 4d61 705d 0000 0073 0c00 0000  t_UpMap]...s....
-00001450: 0002 0f07 1b01 1001 2201 0f01 6301 0000  ........"...c...
-00001460: 000a 0000 0004 0000 0043 0000 0073 2701  .........C...s'.
-00001470: 0000 6401 0084 0000 7d01 0064 0200 8400  ..d.....}..d....
-00001480: 007d 0200 6403 0084 0000 7d03 0064 0400  .}..d.....}..d..
-00001490: 8400 007d 0400 7400 007c 0000 6a01 007c  ...}..t..|..j..|
-000014a0: 0000 6a02 007c 0000 6a03 0083 0300 7d05  ..j..|..j.....}.
-000014b0: 007c 0000 6a04 007c 0500 6a05 0083 0100  .|..j..|..j.....
-000014c0: 0174 0600 8300 007d 0600 7c00 006a 0700  .t.....}..|..j..
-000014d0: 7c06 007c 0100 7c05 006a 0800 8301 0083  |..|..|..j......
-000014e0: 0200 0174 0600 8300 007d 0700 7c07 006a  ...t.....}..|..j
-000014f0: 0900 6405 0083 0100 017c 0700 6a09 0064  ..d......|..j..d
-00001500: 0600 8301 0001 7c00 006a 0700 7c07 007c  ......|..j..|..|
-00001510: 0200 7c05 006a 0a00 8301 0083 0200 0174  ..|..j.........t
-00001520: 0600 8300 007d 0800 7c08 006a 0900 740b  .....}..|..j..t.
-00001530: 0064 0700 6408 0067 0200 8301 0083 0100  .d..d..g........
-00001540: 017c 0000 6a07 007c 0800 7c03 007c 0500  .|..j..|..|..|..
-00001550: 6a0c 0083 0100 8302 0001 7406 0083 0000  j.........t.....
-00001560: 7d09 007c 0900 6a09 0074 0b00 6409 0064  }..|..j..t..d..d
-00001570: 0a00 6702 0083 0100 8301 0001 7c00 006a  ..g.........|..j
-00001580: 0700 7c09 007c 0400 7c05 006a 0d00 8301  ..|..|..|..j....
-00001590: 0083 0200 0164 0000 5328 0b00 0000 4e63  .....d..S(....Nc
-000015a0: 0100 0000 0200 0000 0500 0000 5300 0000  ............S...
-000015b0: 7323 0000 0074 0000 6700 007c 0000 445d  s#...t..g..|..D]
-000015c0: 1200 7d01 0074 0100 7c01 0083 0100 5e02  ..}..t..|.....^.
-000015d0: 0071 0a00 8301 0053 2801 0000 004e 2802  .q.....S(....N(.
-000015e0: 0000 0052 1300 0000 5206 0000 0028 0200  ...R....R....(..
-000015f0: 0000 7404 0000 004c 4f53 5374 0c00 0000  ..t....LOSSt....
-00001600: 686f 675f 616e 6365 7374 6f72 2800 0000  hog_ancestor(...
-00001610: 0028 0000 0000 7347 0000 002f 5573 6572  .(....sG.../User
-00001620: 732f 6164 6d69 6e2f 576f 726b 2f70 726f  s/admin/Work/pro
-00001630: 6a65 6374 2f44 6573 7369 6d6f 7a2f 7079  ject/Dessimoz/py
-00001640: 6861 6d2d 6465 762f 7079 6861 6d2f 7465  ham-dev/pyham/te
-00001650: 7374 732f 7465 7374 5f6d 6170 7065 722e  sts/test_mapper.
-00001660: 7079 740c 0000 0063 6f6e 7665 7274 5f4c  pyt....convert_L
-00001670: 4f53 536e 0000 0073 0200 0000 0001 6301  OSSn...s......c.
-00001680: 0000 0002 0000 0005 0000 0053 0000 0073  ...........S...s
-00001690: 2300 0000 7400 0067 0000 7c00 0044 5d12  #...t..g..|..D].
-000016a0: 007d 0100 7401 007c 0100 8301 005e 0200  .}..t..|.....^..
-000016b0: 710a 0083 0100 5328 0100 0000 4e28 0200  q.....S(....N(..
-000016c0: 0000 5213 0000 0052 0600 0000 2802 0000  ..R....R....(...
-000016d0: 0074 0400 0000 4741 494e 7407 0000 006e  .t....GAINt....n
-000016e0: 6577 5f68 6f67 2800 0000 0028 0000 0000  ew_hog(....(....
-000016f0: 7347 0000 002f 5573 6572 732f 6164 6d69  sG.../Users/admi
-00001700: 6e2f 576f 726b 2f70 726f 6a65 6374 2f44  n/Work/project/D
-00001710: 6573 7369 6d6f 7a2f 7079 6861 6d2d 6465  essimoz/pyham-de
-00001720: 762f 7079 6861 6d2f 7465 7374 732f 7465  v/pyham/tests/te
-00001730: 7374 5f6d 6170 7065 722e 7079 740c 0000  st_mapper.pyt...
-00001740: 0063 6f6e 7665 7274 5f47 4149 4e71 0000  .convert_GAINq..
-00001750: 0073 0200 0000 0001 6301 0000 0005 0000  .s......c.......
-00001760: 0004 0000 0053 0000 0073 5500 0000 7400  .....S...sU...t.
-00001770: 0083 0000 7d01 0078 4500 7c00 006a 0100  ....}..xE.|..j..
-00001780: 8300 0044 5d37 005c 0200 7d02 007d 0300  ...D]7.\..}..}..
-00001790: 7402 007c 0200 8301 0074 0200 7c03 0083  t..|.....t..|...
-000017a0: 0100 6702 007d 0400 7c01 006a 0300 7404  ..g..}..|..j..t.
-000017b0: 007c 0400 8301 0083 0100 0171 1600 577c  .|.........q..W|
-000017c0: 0100 5328 0100 0000 4e28 0500 0000 5213  ..S(....N(....R.
-000017d0: 0000 0052 0d00 0000 5206 0000 0074 0300  ...R....R....t..
-000017e0: 0000 6164 6474 0900 0000 6672 6f7a 656e  ..addt....frozen
-000017f0: 7365 7428 0500 0000 7408 0000 0052 4554  set(....t....RET
-00001800: 4149 4e45 4474 0900 0000 6352 4554 4149  AINEDt....cRETAI
-00001810: 4e45 4452 6e00 0000 740e 0000 0068 6f67  NEDRn...t....hog
-00001820: 5f64 6573 6365 6e64 616e 7474 0100 0000  _descendantt....
-00001830: 7828 0000 0000 2800 0000 0073 4700 0000  x(....(....sG...
-00001840: 2f55 7365 7273 2f61 646d 696e 2f57 6f72  /Users/admin/Wor
-00001850: 6b2f 7072 6f6a 6563 742f 4465 7373 696d  k/project/Dessim
-00001860: 6f7a 2f70 7968 616d 2d64 6576 2f70 7968  oz/pyham-dev/pyh
-00001870: 616d 2f74 6573 7473 2f74 6573 745f 6d61  am/tests/test_ma
-00001880: 7070 6572 2e70 7974 1000 0000 636f 6e76  pper.pyt....conv
-00001890: 6572 745f 5245 5441 494e 4544 7400 0000  ert_RETAINEDt...
-000018a0: 730a 0000 0000 0109 0119 0118 0117 0163  s..............c
-000018b0: 0100 0000 0600 0000 0500 0000 5300 0000  ............S...
-000018c0: 7370 0000 0074 0000 8300 007d 0100 7860  sp...t.....}..x`
-000018d0: 007c 0000 6a01 0083 0000 445d 5200 5c02  .|..j.....D]R.\.
-000018e0: 007d 0200 7d03 0074 0200 7c02 0083 0100  .}..}..t..|.....
-000018f0: 6701 007d 0400 7821 007c 0300 445d 1900  g..}..x!.|..D]..
-00001900: 7d05 007c 0400 6a03 0074 0200 7c05 0083  }..|..j..t..|...
-00001910: 0100 8301 0001 7138 0057 7c01 006a 0400  ......q8.W|..j..
-00001920: 7405 007c 0400 8301 0083 0100 0171 1600  t..|.........q..
-00001930: 577c 0100 5328 0100 0000 4e28 0600 0000  W|..S(....N(....
-00001940: 5213 0000 0052 0d00 0000 5206 0000 0052  R....R....R....R
-00001950: 0500 0000 5273 0000 0052 7400 0000 2806  ....Rs...Rt...(.
-00001960: 0000 0074 0900 0000 4455 504c 4943 4154  ...t....DUPLICAT
-00001970: 4574 0a00 0000 6344 5550 4c49 4341 5445  Et....cDUPLICATE
-00001980: 526e 0000 0074 0f00 0000 686f 675f 6465  Rn...t....hog_de
-00001990: 7363 656e 6461 6e74 7352 7800 0000 7401  scendantsRx...t.
-000019a0: 0000 0067 2800 0000 0028 0000 0000 7347  ...g(....(....sG
-000019b0: 0000 002f 5573 6572 732f 6164 6d69 6e2f  .../Users/admin/
-000019c0: 576f 726b 2f70 726f 6a65 6374 2f44 6573  Work/project/Des
-000019d0: 7369 6d6f 7a2f 7079 6861 6d2d 6465 762f  simoz/pyham-dev/
-000019e0: 7079 6861 6d2f 7465 7374 732f 7465 7374  pyham/tests/test
-000019f0: 5f6d 6170 7065 722e 7079 7411 0000 0063  _mapper.pyt....c
-00001a00: 6f6e 7665 7274 5f44 5550 4c49 4341 5445  onvert_DUPLICATE
-00001a10: 7b00 0000 730e 0000 0000 0109 0119 010f  {...s...........
-00001a20: 010d 0117 0117 0173 0700 0000 4765 6e65  .......s....Gene
-00001a30: 2832 2973 0700 0000 4765 6e65 2835 2973  (2)s....Gene(5)s
-00001a40: 0800 0000 3c48 4f47 2831 293e 7307 0000  ....<HOG(1)>s...
-00001a50: 0047 656e 6528 3129 7308 0000 003c 484f  .Gene(1)s....<HO
-00001a60: 4728 3329 3e73 0700 0000 4765 6e65 2833  G(3)>s....Gene(3
-00001a70: 2928 0e00 0000 5202 0000 0052 2d00 0000  )(....R....R-...
-00001a80: 522f 0000 0052 3500 0000 5256 0000 0052  R/...R5...RV...R
-00001a90: 5700 0000 5213 0000 0074 0e00 0000 6173  W...R....t....as
-00001aa0: 7365 7274 5365 7445 7175 616c 526d 0000  sertSetEqualRm..
-00001ab0: 0052 7300 0000 5270 0000 0052 7400 0000  .Rs...Rp...Rt...
-00001ac0: 5275 0000 0052 7a00 0000 280a 0000 0052  Ru...Rz...(....R
-00001ad0: 3900 0000 526f 0000 0052 7200 0000 5279  9...Ro...Rr...Ry
-00001ae0: 0000 0052 7e00 0000 525b 0000 0074 0d00  ...R~...R[...t..
-00001af0: 0000 6578 7065 6374 6564 5f4c 4f53 5374  ..expected_LOSSt
-00001b00: 0d00 0000 6578 7065 6374 6564 5f47 4149  ....expected_GAI
-00001b10: 4e74 1100 0000 6578 7065 6374 6564 5f52  Nt....expected_R
-00001b20: 4554 4149 4e45 4474 1200 0000 6578 7065  ETAINEDt....expe
-00001b30: 6374 6564 5f44 5550 4c49 4341 5445 2800  cted_DUPLICATE(.
-00001b40: 0000 0028 0000 0000 7347 0000 002f 5573  ...(....sG.../Us
-00001b50: 6572 732f 6164 6d69 6e2f 576f 726b 2f70  ers/admin/Work/p
-00001b60: 726f 6a65 6374 2f44 6573 7369 6d6f 7a2f  roject/Dessimoz/
-00001b70: 7079 6861 6d2d 6465 762f 7079 6861 6d2f  pyham-dev/pyham/
-00001b80: 7465 7374 732f 7465 7374 5f6d 6170 7065  tests/test_mappe
-00001b90: 722e 7079 7417 0000 0074 6573 745f 6275  r.pyt....test_bu
-00001ba0: 696c 6445 7665 6e74 436c 7573 7465 7273  ildEventClusters
-00001bb0: 6c00 0000 7324 0000 0000 0209 0309 0309  l...s$..........
-00001bc0: 0709 0a1b 0110 0209 0119 0209 010d 010d  ................
-00001bd0: 0119 0209 0119 0119 0209 0119 0128 0800  .............(..
-00001be0: 0000 523e 0000 0052 3f00 0000 5250 0000  ..R>...R?...RP..
-00001bf0: 0052 5400 0000 525c 0000 0052 5f00 0000  .RT...R\...R_...
-00001c00: 526c 0000 0052 8400 0000 2800 0000 0028  Rl...R....(....(
-00001c10: 0000 0000 2800 0000 0073 4700 0000 2f55  ....(....sG.../U
-00001c20: 7365 7273 2f61 646d 696e 2f57 6f72 6b2f  sers/admin/Work/
-00001c30: 7072 6f6a 6563 742f 4465 7373 696d 6f7a  project/Dessimoz
-00001c40: 2f70 7968 616d 2d64 6576 2f70 7968 616d  /pyham-dev/pyham
-00001c50: 2f74 6573 7473 2f74 6573 745f 6d61 7070  /tests/test_mapp
-00001c60: 6572 2e70 7952 4200 0000 3800 0000 730c  er.pyRB...8...s.
-00001c70: 0000 0006 0209 0f09 0609 0809 0609 0f74  ...............t
-00001c80: 1200 0000 5665 7274 6963 616c 4d61 7070  ....VerticalMapp
-00001c90: 6572 5465 7374 6300 0000 0000 0000 0001  erTestc.........
-00001ca0: 0000 0042 0000 0073 5000 0000 6500 005a  ...B...sP...e..Z
-00001cb0: 0100 6400 0084 0000 5a02 0064 0100 8400  ..d.....Z..d....
-00001cc0: 005a 0300 6402 0084 0000 5a04 0064 0300  .Z..d.....Z..d..
-00001cd0: 8400 005a 0500 6404 0084 0000 5a06 0064  ...Z..d.....Z..d
-00001ce0: 0500 8400 005a 0700 6406 0084 0000 5a08  .....Z..d.....Z.
-00001cf0: 0064 0700 8400 005a 0900 5253 2808 0000  .d.....Z..RS(...
-00001d00: 0063 0100 0000 0300 0000 0400 0000 4300  .c............C.
-00001d10: 0000 738d 0000 0074 0000 7c00 006a 0100  ..s....t..|..j..
-00001d20: 8301 007d 0100 7402 007c 0000 6a01 007c  ...}..t..|..j..|
-00001d30: 0000 6a03 007c 0000 6a04 0083 0300 7d02  ..j..|..j.....}.
-00001d40: 007c 0000 6a05 007c 0200 6a06 0083 0100  .|..j..|..j.....
-00001d50: 017c 0100 6a07 007c 0200 8301 0001 7c00  .|..j..|......|.
-00001d60: 006a 0800 7c00 006a 0400 7c01 006a 0900  .j..|..j..|..j..
-00001d70: 8302 0001 7c00 006a 0800 7c00 006a 0300  ....|..j..|..j..
-00001d80: 7c01 006a 0a00 8302 0001 7c00 006a 0800  |..j......|..j..
-00001d90: 7c00 006a 0100 7c01 006a 0b00 8302 0001  |..j..|..j......
-00001da0: 6400 0053 2801 0000 004e 280c 0000 0052  d..S(....N(....R
-00001db0: 0400 0000 522d 0000 0052 0200 0000 522f  ....R-...R....R/
-00001dc0: 0000 0052 3800 0000 5256 0000 0052 5700  ...R8...RV...RW.
-00001dd0: 0000 7407 0000 0061 6464 5f6d 6170 5258  ..t....add_mapRX
-00001de0: 0000 0052 5900 0000 525a 0000 0074 0300  ...RY...RZ...t..
-00001df0: 0000 4841 4d28 0300 0000 5239 0000 0074  ..HAM(....R9...t
-00001e00: 0c00 0000 7665 7274 6963 616c 5f6d 6170  ....vertical_map
-00001e10: 525b 0000 0028 0000 0000 2800 0000 0073  R[...(....(....s
-00001e20: 4700 0000 2f55 7365 7273 2f61 646d 696e  G.../Users/admin
-00001e30: 2f57 6f72 6b2f 7072 6f6a 6563 742f 4465  /Work/project/De
-00001e40: 7373 696d 6f7a 2f70 7968 616d 2d64 6576  ssimoz/pyham-dev
-00001e50: 2f70 7968 616d 2f74 6573 7473 2f74 6573  /pyham/tests/tes
-00001e60: 745f 6d61 7070 6572 2e70 7974 2200 0000  t_mapper.pyt"...
-00001e70: 7465 7374 5f63 7265 6174 655f 636f 7272  test_create_corr
-00001e80: 6563 746c 795f 7665 7274 6963 616c 5f6d  ectly_vertical_m
-00001e90: 6170 9a00 0000 730e 0000 0000 010f 021b  ap....s.........
-00001ea0: 0110 010d 0216 0116 0163 0100 0000 0400  .........c......
-00001eb0: 0000 0600 0000 4300 0000 7399 0000 0074  ......C...s....t
-00001ec0: 0000 7c00 006a 0100 8301 007d 0100 7402  ..|..j.....}..t.
-00001ed0: 007c 0000 6a01 007c 0000 6a03 007c 0000  .|..j..|..j..|..
-00001ee0: 6a04 0083 0300 7d02 007c 0000 6a05 007c  j.....}..|..j..|
-00001ef0: 0200 6a06 0083 0100 017c 0100 6a07 007c  ..j......|..j..|
-00001f00: 0200 8301 0001 7402 007c 0000 6a01 007c  ......t..|..j..|
-00001f10: 0000 6a03 007c 0000 6a08 0083 0300 7d03  ..j..|..j.....}.
-00001f20: 007c 0000 6a05 007c 0300 6a06 0083 0100  .|..j..|..j.....
-00001f30: 017c 0000 6a09 0074 0a00 8301 008f 1200  .|..j..t........
-00001f40: 017c 0100 6a07 007c 0300 8301 0001 5764  .|..j..|......Wd
-00001f50: 0000 5158 6400 0053 2801 0000 004e 280b  ..QXd..S(....N(.
-00001f60: 0000 0052 0400 0000 522d 0000 0052 0200  ...R....R-...R..
-00001f70: 0000 522f 0000 0052 3800 0000 5256 0000  ..R/...R8...RV..
-00001f80: 0052 5700 0000 5286 0000 0052 3500 0000  .RW...R....R5...
-00001f90: 525d 0000 0052 4c00 0000 2804 0000 0052  R]...RL...(....R
-00001fa0: 3900 0000 5288 0000 0052 5b00 0000 525e  9...R....R[...R^
-00001fb0: 0000 0028 0000 0000 2800 0000 0073 4700  ...(....(....sG.
-00001fc0: 0000 2f55 7365 7273 2f61 646d 696e 2f57  ../Users/admin/W
-00001fd0: 6f72 6b2f 7072 6f6a 6563 742f 4465 7373  ork/project/Dess
-00001fe0: 696d 6f7a 2f70 7968 616d 2d64 6576 2f70  imoz/pyham-dev/p
-00001ff0: 7968 616d 2f74 6573 7473 2f74 6573 745f  yham/tests/test_
-00002000: 6d61 7070 6572 2e70 7974 2100 0000 7465  mapper.pyt!...te
-00002010: 7374 5f63 616e 6e6f 745f 6164 645f 6d6f  st_cannot_add_mo
-00002020: 7265 5f74 6861 6e5f 6f6e 655f 6d61 70a5  re_than_one_map.
-00002030: 0000 0073 1000 0000 0001 0f02 1b01 1001  ...s............
-00002040: 0d02 1b01 1001 1001 6301 0000 0002 0000  ........c.......
-00002050: 0007 0000 0043 0000 0073 5900 0000 7400  .....C...sY...t.
-00002060: 007c 0000 6a01 0083 0100 7d01 007c 0000  .|..j.....}..|..
-00002070: 6a02 0074 0300 8301 008f 1200 017c 0100  j..t.........|..
-00002080: 6a04 0064 0100 8301 0001 5764 0000 5158  j..d......Wd..QX
-00002090: 7c00 006a 0200 7403 0083 0100 8f12 0001  |..j..t.........
-000020a0: 7c01 006a 0400 6402 0083 0100 0157 6400  |..j..d......Wd.
-000020b0: 0051 5864 0000 5328 0300 0000 4e74 0300  .QXd..S(....Nt..
-000020c0: 0000 3131 3174 0000 0000 2805 0000 0052  ..111t....(....R
-000020d0: 0400 0000 522d 0000 0052 5d00 0000 524c  ....R-...R]...RL
-000020e0: 0000 0052 8600 0000 2802 0000 0052 3900  ...R....(....R9.
-000020f0: 0000 5288 0000 0028 0000 0000 2800 0000  ..R....(....(...
-00002100: 0073 4700 0000 2f55 7365 7273 2f61 646d  .sG.../Users/adm
-00002110: 696e 2f57 6f72 6b2f 7072 6f6a 6563 742f  in/Work/project/
-00002120: 4465 7373 696d 6f7a 2f70 7968 616d 2d64  Dessimoz/pyham-d
-00002130: 6576 2f70 7968 616d 2f74 6573 7473 2f74  ev/pyham/tests/t
-00002140: 6573 745f 6d61 7070 6572 2e70 7974 1f00  est_mapper.pyt..
-00002150: 0000 7465 7374 5f63 616e 5f6f 6e6c 795f  ..test_can_only_
-00002160: 6164 645f 484f 474d 4150 5f61 735f 6d61  add_HOGMAP_as_ma
-00002170: 70b1 0000 0073 0a00 0000 0001 0f02 1001  p....s..........
-00002180: 1302 1001 6301 0000 0001 0000 0005 0000  ....c...........
-00002190: 0043 0000 0073 2100 0000 7c00 006a 0000  .C...s!...|..j..
-000021a0: 7401 0083 0100 8f0c 0001 7402 0083 0000  t.........t.....
-000021b0: 0157 6400 0051 5864 0000 5328 0100 0000  .Wd..QXd..S(....
-000021c0: 4e28 0300 0000 525d 0000 0052 4c00 0000  N(....R]...RL...
-000021d0: 5204 0000 0028 0100 0000 5239 0000 0028  R....(....R9...(
-000021e0: 0000 0000 2800 0000 0073 4700 0000 2f55  ....(....sG.../U
-000021f0: 7365 7273 2f61 646d 696e 2f57 6f72 6b2f  sers/admin/Work/
-00002200: 7072 6f6a 6563 742f 4465 7373 696d 6f7a  project/Dessimoz
-00002210: 2f70 7968 616d 2d64 6576 2f70 7968 616d  /pyham-dev/pyham
-00002220: 2f74 6573 7473 2f74 6573 745f 6d61 7070  /tests/test_mapp
-00002230: 6572 2e70 7974 3100 0000 7465 7374 5f63  er.pyt1...test_c
-00002240: 616e 5f6f 6e6c 795f 6372 6561 7465 5f76  an_only_create_v
-00002250: 6572 7469 6361 6c5f 6d61 705f 7769 7468  ertical_map_with
-00002260: 5f68 616d 5f6f 626a 6563 74ba 0000 0073  _ham_object....s
-00002270: 0400 0000 0001 1001 6301 0000 0007 0000  ........c.......
-00002280: 0005 0000 0043 0000 0073 e800 0000 7400  .....C...s....t.
-00002290: 007c 0000 6a01 0083 0100 7d01 0074 0200  .|..j.....}..t..
-000022a0: 7c00 006a 0100 7c00 006a 0300 7c00 006a  |..j..|..j..|..j
-000022b0: 0400 8303 007d 0200 7c00 006a 0500 7c02  .....}..|..j..|.
-000022c0: 006a 0600 8301 0001 7c01 006a 0700 7c02  .j......|..j..|.
-000022d0: 0083 0100 017c 0100 6a08 0083 0000 7d03  .....|..j.....}.
-000022e0: 007c 0000 6a09 0064 0100 6701 0074 0a00  .|..j..d..g..t..
-000022f0: 7c03 0083 0100 8302 0001 7400 007c 0000  |.........t..|..
-00002300: 6a01 0083 0100 7d04 0074 0200 7c00 006a  j.....}..t..|..j
-00002310: 0100 7c00 006a 0b00 7c00 006a 0400 8303  ..|..j..|..j....
-00002320: 007d 0500 7c00 006a 0500 7c05 006a 0600  .}..|..j..|..j..
-00002330: 8301 0001 7c04 006a 0700 7c05 0083 0100  ....|..j..|.....
-00002340: 017c 0400 6a08 0083 0000 7d06 007c 0000  .|..j.....}..|..
-00002350: 6a09 0064 0200 6401 0064 0300 6803 0074  j..d..d..d..h..t
-00002360: 0c00 740a 007c 0600 8301 0083 0100 8302  ..t..|..........
-00002370: 0001 6400 0053 2804 0000 004e 730c 0000  ..d..S(....Ns...
-00002380: 003c 484f 4728 332e 452e 3229 3e73 0a00  .<HOG(3.E.2)>s..
-00002390: 0000 3c48 4f47 2832 2e45 293e 730c 0000  ..<HOG(2.E)>s...
-000023a0: 003c 484f 4728 332e 452e 3129 3e28 0d00  .<HOG(3.E.1)>(..
-000023b0: 0000 5204 0000 0052 2d00 0000 5202 0000  ..R....R-...R...
-000023c0: 0052 2f00 0000 5238 0000 0052 5600 0000  .R/...R8...RV...
-000023d0: 5257 0000 0052 8600 0000 7408 0000 0067  RW...R....t....g
-000023e0: 6574 5f6c 6f73 7452 5800 0000 520a 0000  et_lostRX...R...
-000023f0: 0052 3200 0000 5213 0000 0028 0700 0000  .R2...R....(....
-00002400: 5239 0000 0052 8800 0000 525b 0000 0074  R9...R....R[...t
-00002410: 0400 0000 6c6f 7373 740d 0000 0076 6572  ....losst....ver
-00002420: 7469 6361 6c5f 6d61 7032 525e 0000 0074  tical_map2R^...t
-00002430: 0500 0000 6c6f 7373 3228 0000 0000 2800  ....loss2(....(.
-00002440: 0000 0073 4700 0000 2f55 7365 7273 2f61  ...sG.../Users/a
-00002450: 646d 696e 2f57 6f72 6b2f 7072 6f6a 6563  dmin/Work/projec
-00002460: 742f 4465 7373 696d 6f7a 2f70 7968 616d  t/Dessimoz/pyham
-00002470: 2d64 6576 2f70 7968 616d 2f74 6573 7473  -dev/pyham/tests
-00002480: 2f74 6573 745f 6d61 7070 6572 2e70 7974  /test_mapper.pyt
-00002490: 0d00 0000 7465 7374 5f67 6574 5f6c 6f73  ....test_get_los
-000024a0: 74be 0000 0073 1800 0000 0001 0f01 1b01  t....s..........
-000024b0: 1001 0d02 0c01 1902 0f01 1b01 1001 0d02  ................
-000024c0: 0c01 6301 0000 0004 0000 0005 0000 0043  ..c............C
-000024d0: 0000 0073 7900 0000 7400 007c 0000 6a01  ...sy...t..|..j.
-000024e0: 0083 0100 7d01 0074 0200 7c00 006a 0100  ....}..t..|..j..
-000024f0: 7c00 006a 0300 7c00 006a 0400 8303 007d  |..j..|..j.....}
-00002500: 0200 7c00 006a 0500 7c02 006a 0600 8301  ..|..j..|..j....
-00002510: 0001 7c01 006a 0700 7c02 0083 0100 017c  ..|..j..|......|
-00002520: 0100 6a08 0083 0000 7d03 007c 0000 6a09  ..j.....}..|..j.
-00002530: 0064 0100 6402 0068 0200 740a 0074 0b00  .d..d..h..t..t..
-00002540: 7c03 0083 0100 8301 0083 0200 0164 0000  |............d..
-00002550: 5328 0300 0000 4e73 0700 0000 4765 6e65  S(....Ns....Gene
-00002560: 2832 2973 0700 0000 4765 6e65 2835 2928  (2)s....Gene(5)(
-00002570: 0c00 0000 5204 0000 0052 2d00 0000 5202  ....R....R-...R.
-00002580: 0000 0052 2f00 0000 5235 0000 0052 5600  ...R/...R5...RV.
-00002590: 0000 5257 0000 0052 8600 0000 740a 0000  ..RW...R....t...
-000025a0: 0067 6574 5f67 6169 6e65 6452 5800 0000  .get_gainedRX...
-000025b0: 5213 0000 0052 0a00 0000 2804 0000 0052  R....R....(....R
-000025c0: 3900 0000 5288 0000 0052 5b00 0000 7404  9...R....R[...t.
-000025d0: 0000 0067 6169 6e28 0000 0000 2800 0000  ...gain(....(...
-000025e0: 0073 4700 0000 2f55 7365 7273 2f61 646d  .sG.../Users/adm
-000025f0: 696e 2f57 6f72 6b2f 7072 6f6a 6563 742f  in/Work/project/
-00002600: 4465 7373 696d 6f7a 2f70 7968 616d 2d64  Dessimoz/pyham-d
-00002610: 6576 2f70 7968 616d 2f74 6573 7473 2f74  ev/pyham/tests/t
-00002620: 6573 745f 6d61 7070 6572 2e70 7974 0f00  est_mapper.pyt..
-00002630: 0000 7465 7374 5f67 6574 5f67 6169 6e65  ..test_get_gaine
-00002640: 64cf 0000 0073 0c00 0000 0001 0f01 1b01  d....s..........
-00002650: 1001 0d02 0c01 6301 0000 0004 0000 0004  ......c.........
-00002660: 0000 0043 0000 0073 7400 0000 7400 007c  ...C...st...t..|
-00002670: 0000 6a01 0083 0100 7d01 0074 0200 7c00  ..j.....}..t..|.
-00002680: 006a 0100 7c00 006a 0300 7c00 006a 0400  .j..|..j..|..j..
-00002690: 8303 007d 0200 7c00 006a 0500 7c02 006a  ...}..|..j..|..j
-000026a0: 0600 8301 0001 7c01 006a 0700 7c02 0083  ......|..j..|...
-000026b0: 0100 017c 0100 6a08 0083 0000 7d03 007c  ...|..j.....}..|
-000026c0: 0000 6a09 0069 0100 6401 0064 0200 3674  ..j..i..d..d..6t
-000026d0: 0a00 7c03 0083 0100 8302 0001 6400 0053  ..|.........d..S
-000026e0: 2803 0000 004e 7307 0000 0047 656e 6528  (....Ns....Gene(
-000026f0: 3129 7308 0000 003c 484f 4728 3129 3e28  1)s....<HOG(1)>(
-00002700: 0b00 0000 5204 0000 0052 2d00 0000 5202  ....R....R-...R.
-00002710: 0000 0052 2f00 0000 5235 0000 0052 5600  ...R/...R5...RV.
-00002720: 0000 5257 0000 0052 8600 0000 740c 0000  ..RW...R....t...
-00002730: 0067 6574 5f72 6574 6169 6e65 6452 6a00  .get_retainedRj.
-00002740: 0000 5212 0000 0028 0400 0000 5239 0000  ..R....(....R9..
-00002750: 0052 8800 0000 525b 0000 0074 0600 0000  .R....R[...t....
-00002760: 7369 6e67 6c65 2800 0000 0028 0000 0000  single(....(....
-00002770: 7347 0000 002f 5573 6572 732f 6164 6d69  sG.../Users/admi
-00002780: 6e2f 576f 726b 2f70 726f 6a65 6374 2f44  n/Work/project/D
-00002790: 6573 7369 6d6f 7a2f 7079 6861 6d2d 6465  essimoz/pyham-de
-000027a0: 762f 7079 6861 6d2f 7465 7374 732f 7465  v/pyham/tests/te
-000027b0: 7374 5f6d 6170 7065 722e 7079 740f 0000  st_mapper.pyt...
-000027c0: 0074 6573 745f 6765 745f 7369 6e67 6c65  .test_get_single
-000027d0: d800 0000 730c 0000 0000 010f 011b 0110  ....s...........
-000027e0: 010d 020c 0163 0100 0000 0400 0000 0400  .....c..........
-000027f0: 0000 4300 0000 737a 0000 0074 0000 7c00  ..C...sz...t..|.
-00002800: 006a 0100 8301 007d 0100 7402 007c 0000  .j.....}..t..|..
-00002810: 6a01 007c 0000 6a03 007c 0000 6a04 0083  j..|..j..|..j...
-00002820: 0300 7d02 007c 0000 6a05 007c 0200 6a06  ..}..|..j..|..j.
-00002830: 0083 0100 017c 0100 6a07 007c 0200 8301  .....|..j..|....
-00002840: 0001 7c01 006a 0800 8300 007d 0300 7c00  ..|..j.....}..|.
-00002850: 006a 0900 6901 0064 0100 6402 0068 0200  .j..i..d..d..h..
-00002860: 6403 0036 740a 007c 0300 8301 0083 0200  d..6t..|........
-00002870: 0164 0000 5328 0400 0000 4e73 0800 0000  .d..S(....Ns....
-00002880: 4765 6e65 2833 3329 7308 0000 0047 656e  Gene(33)s....Gen
-00002890: 6528 3334 2973 0800 0000 3c48 4f47 2833  e(34)s....<HOG(3
-000028a0: 293e 280b 0000 0052 0400 0000 522d 0000  )>(....R....R-..
-000028b0: 0052 0200 0000 5231 0000 0052 3500 0000  .R....R1...R5...
-000028c0: 5256 0000 0052 5700 0000 5286 0000 0074  RV...RW...R....t
-000028d0: 0e00 0000 6765 745f 6475 706c 6963 6174  ....get_duplicat
-000028e0: 6564 526a 0000 0052 1500 0000 2804 0000  edRj...R....(...
-000028f0: 0052 3900 0000 5288 0000 0052 5b00 0000  .R9...R....R[...
-00002900: 7409 0000 0064 7570 6c69 6361 7465 2800  t....duplicate(.
-00002910: 0000 0028 0000 0000 7347 0000 002f 5573  ...(....sG.../Us
-00002920: 6572 732f 6164 6d69 6e2f 576f 726b 2f70  ers/admin/Work/p
-00002930: 726f 6a65 6374 2f44 6573 7369 6d6f 7a2f  roject/Dessimoz/
-00002940: 7079 6861 6d2d 6465 762f 7079 6861 6d2f  pyham-dev/pyham/
-00002950: 7465 7374 732f 7465 7374 5f6d 6170 7065  tests/test_mappe
-00002960: 722e 7079 7413 0000 0074 6573 745f 6765  r.pyt....test_ge
-00002970: 745f 6475 706c 6963 6174 6564 e100 0000  t_duplicated....
-00002980: 730c 0000 0000 010f 011b 0110 010d 020c  s...............
-00002990: 0128 0a00 0000 523e 0000 0052 3f00 0000  .(....R>...R?...
-000029a0: 5289 0000 0052 8a00 0000 528d 0000 0052  R....R....R....R
-000029b0: 8e00 0000 5293 0000 0052 9600 0000 5299  ....R....R....R.
-000029c0: 0000 0052 9c00 0000 2800 0000 0028 0000  ...R....(....(..
-000029d0: 0000 2800 0000 0073 4700 0000 2f55 7365  ..(....sG.../Use
-000029e0: 7273 2f61 646d 696e 2f57 6f72 6b2f 7072  rs/admin/Work/pr
-000029f0: 6f6a 6563 742f 4465 7373 696d 6f7a 2f70  oject/Dessimoz/p
-00002a00: 7968 616d 2d64 6576 2f70 7968 616d 2f74  yham-dev/pyham/t
-00002a10: 6573 7473 2f74 6573 745f 6d61 7070 6572  ests/test_mapper
-00002a20: 2e70 7952 8500 0000 9900 0000 7310 0000  .pyR........s...
-00002a30: 0006 0109 0b09 0c09 0909 0409 1109 0909  ................
-00002a40: 0974 1100 0000 4c61 7465 7261 6c4d 6170  .t....LateralMap
-00002a50: 7065 7254 6573 7463 0000 0000 0000 0000  perTestc........
-00002a60: 0100 0000 4200 0000 7350 0000 0065 0000  ....B...sP...e..
-00002a70: 5a01 0064 0000 8400 005a 0200 6401 0084  Z..d.....Z..d...
-00002a80: 0000 5a03 0064 0200 8400 005a 0400 6403  ..Z..d.....Z..d.
-00002a90: 0084 0000 5a05 0064 0400 8400 005a 0600  ....Z..d.....Z..
-00002aa0: 6405 0084 0000 5a07 0064 0600 8400 005a  d.....Z..d.....Z
-00002ab0: 0800 6407 0084 0000 5a09 0052 5328 0800  ..d.....Z..RS(..
-00002ac0: 0000 6301 0000 0004 0000 0004 0000 0043  ..c............C
-00002ad0: 0000 0073 ce00 0000 7400 007c 0000 6a01  ...s....t..|..j.
-00002ae0: 0083 0100 7d01 0074 0200 7c00 006a 0100  ....}..t..|..j..
-00002af0: 7c00 006a 0300 7c00 006a 0400 8303 007d  |..j..|..j.....}
-00002b00: 0200 7c00 006a 0500 7c02 006a 0600 8301  ..|..j..|..j....
-00002b10: 0001 7c01 006a 0700 7c02 0083 0100 0174  ..|..j..|......t
-00002b20: 0200 7c00 006a 0100 7c00 006a 0800 7c00  ..|..j..|..j..|.
-00002b30: 006a 0400 8303 007d 0300 7c00 006a 0500  .j.....}..|..j..
-00002b40: 7c03 006a 0600 8301 0001 7c01 006a 0700  |..j......|..j..
-00002b50: 7c03 0083 0100 017c 0000 6a09 007c 0000  |......|..j..|..
-00002b60: 6a04 007c 0100 6a0a 0083 0200 017c 0000  j..|..j......|..
-00002b70: 6a09 007c 0000 6a03 007c 0000 6a08 0067  j..|..j..|..j..g
-00002b80: 0200 7c01 006a 0b00 8302 0001 7c00 006a  ..|..j......|..j
-00002b90: 0900 7c00 006a 0100 7c01 006a 0c00 8302  ..|..j..|..j....
-00002ba0: 0001 6400 0053 2801 0000 004e 280d 0000  ..d..S(....N(...
-00002bb0: 0052 0300 0000 522d 0000 0052 0200 0000  .R....R-...R....
-00002bc0: 522f 0000 0052 3800 0000 5256 0000 0052  R/...R8...RV...R
-00002bd0: 5700 0000 5286 0000 0052 3600 0000 5258  W...R....R6...RX
-00002be0: 0000 0052 5900 0000 740b 0000 0064 6573  ...RY...t....des
-00002bf0: 6365 6e64 616e 7473 5287 0000 0028 0400  cendantsR....(..
-00002c00: 0000 5239 0000 0074 0b00 0000 6c61 7465  ..R9...t....late
-00002c10: 7261 6c5f 6d61 7052 5b00 0000 525e 0000  ral_mapR[...R^..
-00002c20: 0028 0000 0000 2800 0000 0073 4700 0000  .(....(....sG...
-00002c30: 2f55 7365 7273 2f61 646d 696e 2f57 6f72  /Users/admin/Wor
-00002c40: 6b2f 7072 6f6a 6563 742f 4465 7373 696d  k/project/Dessim
-00002c50: 6f7a 2f70 7968 616d 2d64 6576 2f70 7968  oz/pyham-dev/pyh
-00002c60: 616d 2f74 6573 7473 2f74 6573 745f 6d61  am/tests/test_ma
-00002c70: 7070 6572 2e70 7974 2100 0000 7465 7374  pper.pyt!...test
-00002c80: 5f63 7265 6174 655f 636f 7272 6563 746c  _create_correctl
-00002c90: 795f 6c61 7465 7261 6c5f 6d61 70ed 0000  y_lateral_map...
-00002ca0: 0073 1400 0000 0001 0f02 1b01 1001 0d02  .s..............
-00002cb0: 1b01 1001 0d02 1601 1f01 6301 0000 0004  ..........c.....
-00002cc0: 0000 0006 0000 0043 0000 0073 9900 0000  .......C...s....
-00002cd0: 7400 007c 0000 6a01 0083 0100 7d01 0074  t..|..j.....}..t
-00002ce0: 0200 7c00 006a 0100 7c00 006a 0300 7c00  ..|..j..|..j..|.
-00002cf0: 006a 0400 8303 007d 0200 7c00 006a 0500  .j.....}..|..j..
-00002d00: 7c02 006a 0600 8301 0001 7c01 006a 0700  |..j......|..j..
-00002d10: 7c02 0083 0100 0174 0200 7c00 006a 0100  |......t..|..j..
-00002d20: 7c00 006a 0300 7c00 006a 0800 8303 007d  |..j..|..j.....}
-00002d30: 0300 7c00 006a 0500 7c03 006a 0600 8301  ..|..j..|..j....
-00002d40: 0001 7c00 006a 0900 740a 0083 0100 8f12  ..|..j..t.......
-00002d50: 0001 7c01 006a 0700 7c03 0083 0100 0157  ..|..j..|......W
-00002d60: 6400 0051 5864 0000 5328 0100 0000 4e28  d..QXd..S(....N(
-00002d70: 0b00 0000 5203 0000 0052 2d00 0000 5202  ....R....R-...R.
-00002d80: 0000 0052 2f00 0000 5238 0000 0052 5600  ...R/...R8...RV.
-00002d90: 0000 5257 0000 0052 8600 0000 5235 0000  ..RW...R....R5..
-00002da0: 0052 5d00 0000 524c 0000 0028 0400 0000  .R]...RL...(....
-00002db0: 5239 0000 0052 9f00 0000 525b 0000 0052  R9...R....R[...R
-00002dc0: 5e00 0000 2800 0000 0028 0000 0000 7347  ^...(....(....sG
-00002dd0: 0000 002f 5573 6572 732f 6164 6d69 6e2f  .../Users/admin/
-00002de0: 576f 726b 2f70 726f 6a65 6374 2f44 6573  Work/project/Des
-00002df0: 7369 6d6f 7a2f 7079 6861 6d2d 6465 762f  simoz/pyham-dev/
-00002e00: 7079 6861 6d2f 7465 7374 732f 7465 7374  pyham/tests/test
-00002e10: 5f6d 6170 7065 722e 7079 742b 0000 0074  _mapper.pyt+...t
-00002e20: 6573 745f 6361 6e6e 6f74 5f61 6464 5f6d  est_cannot_add_m
-00002e30: 6170 5f77 6974 685f 6469 6666 6572 656e  ap_with_differen
-00002e40: 745f 616e 6365 7374 6f72 fc00 0000 7310  t_ancestor....s.
-00002e50: 0000 0000 010f 021b 0110 010d 021b 0110  ................
-00002e60: 0110 0163 0100 0000 0200 0000 0700 0000  ...c............
-00002e70: 4300 0000 7359 0000 0074 0000 7c00 006a  C...sY...t..|..j
-00002e80: 0100 8301 007d 0100 7c00 006a 0200 7403  .....}..|..j..t.
-00002e90: 0083 0100 8f12 0001 7c01 006a 0400 6401  ........|..j..d.
-00002ea0: 0083 0100 0157 6400 0051 587c 0000 6a02  .....Wd..QX|..j.
-00002eb0: 0074 0300 8301 008f 1200 017c 0100 6a04  .t.........|..j.
-00002ec0: 0064 0200 8301 0001 5764 0000 5158 6400  .d......Wd..QXd.
-00002ed0: 0053 2803 0000 004e 528b 0000 0052 8c00  .S(....NR....R..
-00002ee0: 0000 2805 0000 0052 0300 0000 522d 0000  ..(....R....R-..
-00002ef0: 0052 5d00 0000 524c 0000 0052 8600 0000  .R]...RL...R....
-00002f00: 2802 0000 0052 3900 0000 529f 0000 0028  (....R9...R....(
-00002f10: 0000 0000 2800 0000 0073 4700 0000 2f55  ....(....sG.../U
-00002f20: 7365 7273 2f61 646d 696e 2f57 6f72 6b2f  sers/admin/Work/
-00002f30: 7072 6f6a 6563 742f 4465 7373 696d 6f7a  project/Dessimoz
-00002f40: 2f70 7968 616d 2d64 6576 2f70 7968 616d  /pyham-dev/pyham
-00002f50: 2f74 6573 7473 2f74 6573 745f 6d61 7070  /tests/test_mapp
-00002f60: 6572 2e70 7952 8d00 0000 0801 0000 730a  er.pyR........s.
-00002f70: 0000 0000 010f 0210 0113 0210 0163 0100  .............c..
-00002f80: 0000 0200 0000 0500 0000 4300 0000 7323  ..........C...s#
-00002f90: 0000 007c 0000 6a00 0074 0100 8301 008f  ...|..j..t......
-00002fa0: 0e00 0174 0200 8300 007d 0100 5764 0000  ...t.....}..Wd..
-00002fb0: 5158 6400 0053 2801 0000 004e 2803 0000  QXd..S(....N(...
-00002fc0: 0052 5d00 0000 524c 0000 0052 0300 0000  .R]...RL...R....
-00002fd0: 2802 0000 0052 3900 0000 529f 0000 0028  (....R9...R....(
-00002fe0: 0000 0000 2800 0000 0073 4700 0000 2f55  ....(....sG.../U
-00002ff0: 7365 7273 2f61 646d 696e 2f57 6f72 6b2f  sers/admin/Work/
-00003000: 7072 6f6a 6563 742f 4465 7373 696d 6f7a  project/Dessimoz
-00003010: 2f70 7968 616d 2d64 6576 2f70 7968 616d  /pyham-dev/pyham
-00003020: 2f74 6573 7473 2f74 6573 745f 6d61 7070  /tests/test_mapp
-00003030: 6572 2e70 7952 8e00 0000 1101 0000 7304  er.pyR........s.
-00003040: 0000 0000 0110 0163 0100 0000 0a00 0000  .......c........
-00003050: 0500 0000 4300 0000 73cf 0100 0074 0000  ....C...s....t..
-00003060: 7c00 006a 0100 8301 007d 0100 7402 007c  |..j.....}..t..|
-00003070: 0000 6a01 007c 0000 6a03 007c 0000 6a04  ..j..|..j..|..j.
-00003080: 0083 0300 7d02 007c 0000 6a05 007c 0200  ....}..|..j..|..
-00003090: 6a06 0083 0100 017c 0100 6a07 007c 0200  j......|..j..|..
-000030a0: 8301 0001 7402 007c 0000 6a01 007c 0000  ....t..|..j..|..
-000030b0: 6a08 007c 0000 6a04 0083 0300 7d03 007c  j..|..j.....}..|
-000030c0: 0000 6a05 007c 0300 6a06 0083 0100 017c  ..j..|..j......|
-000030d0: 0100 6a07 007c 0300 8301 0001 7c01 006a  ..j..|......|..j
-000030e0: 0900 8300 007d 0400 7865 007c 0400 6a0a  .....}..xe.|..j.
-000030f0: 0083 0000 445d 5700 7d05 0074 0b00 7c05  ....D]W.}..t..|.
-00003100: 0083 0100 6401 006b 0200 72b9 007c 0500  ....d..k..r..|..
-00003110: 7d06 0071 9800 740b 007c 0500 8301 0064  }..q..t..|.....d
-00003120: 0200 6b02 0072 d400 7c05 007d 0700 7198  ..k..r..|..}..q.
-00003130: 0074 0b00 7c05 0083 0100 6403 006b 0200  .t..|.....d..k..
-00003140: 7298 007c 0500 7d08 0071 9800 7198 0057  r..|..}..q..q..W
-00003150: 7c00 006a 0c00 7c00 006a 0800 6801 0074  |..j..|..j..h..t
-00003160: 0d00 7c04 007c 0800 1983 0100 8302 0001  ..|..|..........
-00003170: 7c00 006a 0c00 7c00 006a 0800 6801 0074  |..j..|..j..h..t
-00003180: 0d00 7c04 007c 0700 1983 0100 8302 0001  ..|..|..........
-00003190: 7c00 006a 0c00 7c00 006a 0800 7c00 006a  |..j..|..j..|..j
-000031a0: 0300 6802 0074 0d00 7c04 007c 0600 1983  ..h..t..|..|....
-000031b0: 0100 8302 0001 7c01 006a 0900 8300 007d  ......|..j.....}
-000031c0: 0900 7c00 006a 0c00 7c00 006a 0800 6801  ..|..j..|..j..h.
-000031d0: 0074 0d00 7c09 007c 0800 1983 0100 8302  .t..|..|........
-000031e0: 0001 7c00 006a 0c00 7c00 006a 0800 6801  ..|..j..|..j..h.
-000031f0: 0074 0d00 7c09 007c 0700 1983 0100 8302  .t..|..|........
-00003200: 0001 7c00 006a 0c00 7c00 006a 0800 7c00  ..|..j..|..j..|.
-00003210: 006a 0300 6802 0074 0d00 7c09 007c 0600  .j..h..t..|..|..
-00003220: 1983 0100 8302 0001 6400 0053 2804 0000  ........d..S(...
-00003230: 004e 730c 0000 003c 484f 4728 332e 452e  .Ns....<HOG(3.E.
-00003240: 3229 3e73 0c00 0000 3c48 4f47 2833 2e45  2)>s....<HOG(3.E
-00003250: 2e31 293e 730a 0000 003c 484f 4728 322e  .1)>s....<HOG(2.
-00003260: 4529 3e28 0e00 0000 5203 0000 0052 2d00  E)>(....R....R-.
-00003270: 0000 5202 0000 0052 2f00 0000 5238 0000  ..R....R/...R8..
-00003280: 0052 5600 0000 5257 0000 0052 8600 0000  .RV...RW...R....
-00003290: 5232 0000 0052 8f00 0000 520b 0000 0052  R2...R....R....R
-000032a0: 0600 0000 5258 0000 0052 1300 0000 280a  ....RX...R....(.
-000032b0: 0000 0052 3900 0000 529f 0000 0074 0f00  ...R9...R....t..
-000032c0: 0000 6d61 705f 6875 6d61 6e5f 6575 6172  ..map_human_euar
-000032d0: 6374 0d00 0000 6d61 705f 7261 745f 6575  ct....map_rat_eu
-000032e0: 6172 6352 9000 0000 5252 0000 0074 0600  arcR....RR...t..
-000032f0: 0000 4833 5f45 5f32 7406 0000 0048 335f  ..H3_E_2t....H3_
-00003300: 455f 3174 0400 0000 4832 5f45 5292 0000  E_1t....H2_ER...
-00003310: 0028 0000 0000 2800 0000 0073 4700 0000  .(....(....sG...
-00003320: 2f55 7365 7273 2f61 646d 696e 2f57 6f72  /Users/admin/Wor
-00003330: 6b2f 7072 6f6a 6563 742f 4465 7373 696d  k/project/Dessim
-00003340: 6f7a 2f70 7968 616d 2d64 6576 2f70 7968  oz/pyham-dev/pyh
-00003350: 616d 2f74 6573 7473 2f74 6573 745f 6d61  am/tests/test_ma
-00003360: 7070 6572 2e70 7952 9300 0000 1501 0000  pper.pyR........
-00003370: 732c 0000 0000 010f 021b 0110 010d 021b  s,..............
-00003380: 0110 010d 020c 0213 0112 0109 0112 0109  ................
-00003390: 0112 010d 0220 0120 0126 030c 0120 0120  ..... . .&... . 
-000033a0: 0163 0100 0000 0500 0000 0600 0000 4300  .c............C.
-000033b0: 0000 73de 0000 0074 0000 7c00 006a 0100  ..s....t..|..j..
-000033c0: 8301 007d 0100 7402 007c 0000 6a01 007c  ...}..t..|..j..|
-000033d0: 0000 6a03 007c 0000 6a04 0083 0300 7d02  ..j..|..j.....}.
-000033e0: 007c 0000 6a05 007c 0200 6a06 0083 0100  .|..j..|..j.....
-000033f0: 017c 0100 6a07 007c 0200 8301 0001 7402  .|..j..|......t.
-00003400: 007c 0000 6a01 007c 0000 6a08 007c 0000  .|..j..|..j..|..
-00003410: 6a04 0083 0300 7d03 007c 0000 6a05 007c  j.....}..|..j..|
-00003420: 0300 6a06 0083 0100 017c 0100 6a07 007c  ..j......|..j..|
-00003430: 0300 8301 0001 7c01 006a 0900 8300 007d  ......|..j.....}
-00003440: 0400 7c00 006a 0a00 740b 0083 0000 740b  ..|..j..t.....t.
-00003450: 0074 0c00 7c04 007c 0000 6a03 0019 8301  .t..|..|..j.....
-00003460: 0083 0100 8302 0001 7c00 006a 0a00 6401  ........|..j..d.
-00003470: 0064 0200 6802 0074 0b00 740c 007c 0400  .d..h..t..t..|..
-00003480: 7c00 006a 0800 1983 0100 8301 0083 0200  |..j............
-00003490: 0164 0000 5328 0300 0000 4e73 0700 0000  .d..S(....Ns....
-000034a0: 4765 6e65 2832 2973 0700 0000 4765 6e65  Gene(2)s....Gene
-000034b0: 2835 2928 0d00 0000 5203 0000 0052 2d00  (5)(....R....R-.
-000034c0: 0000 5202 0000 0052 3000 0000 5235 0000  ..R....R0...R5..
-000034d0: 0052 5600 0000 5257 0000 0052 8600 0000  .RV...RW...R....
-000034e0: 522f 0000 0052 9400 0000 5258 0000 0052  R/...R....RX...R
-000034f0: 1300 0000 520a 0000 0028 0500 0000 5239  ....R....(....R9
-00003500: 0000 0052 9f00 0000 7413 0000 006d 6170  ...R....t....map
-00003510: 5f66 726f 675f 7665 7274 6562 7261 7465  _frog_vertebrate
-00003520: 52a2 0000 0052 9500 0000 2800 0000 0028  R....R....(....(
-00003530: 0000 0000 7347 0000 002f 5573 6572 732f  ....sG.../Users/
-00003540: 6164 6d69 6e2f 576f 726b 2f70 726f 6a65  admin/Work/proje
-00003550: 6374 2f44 6573 7369 6d6f 7a2f 7079 6861  ct/Dessimoz/pyha
-00003560: 6d2d 6465 762f 7079 6861 6d2f 7465 7374  m-dev/pyham/test
-00003570: 732f 7465 7374 5f6d 6170 7065 722e 7079  s/test_mapper.py
-00003580: 5296 0000 0034 0100 0073 1400 0000 0002  R....4...s......
-00003590: 0f02 1b01 1001 0d02 1b01 1001 0d02 0c01  ................
-000035a0: 2601 6301 0000 0009 0000 0005 0000 0043  &.c............C
-000035b0: 0000 0073 8501 0000 7400 007c 0000 6a01  ...s....t..|..j.
-000035c0: 0083 0100 7d01 0074 0200 7c00 006a 0100  ....}..t..|..j..
-000035d0: 7c00 006a 0300 7c00 006a 0400 8303 007d  |..j..|..j.....}
-000035e0: 0200 7c00 006a 0500 7c02 006a 0600 8301  ..|..j..|..j....
-000035f0: 0001 7c01 006a 0700 7c02 0083 0100 0174  ..|..j..|......t
-00003600: 0200 7c00 006a 0100 7c00 006a 0800 7c00  ..|..j..|..j..|.
-00003610: 006a 0400 8303 007d 0300 7c00 006a 0500  .j.....}..|..j..
-00003620: 7c03 006a 0600 8301 0001 7c01 006a 0700  |..j......|..j..
-00003630: 7c03 0083 0100 017c 0100 6a09 0083 0000  |......|..j.....
-00003640: 7d04 0078 6500 7c04 006a 0a00 8300 0044  }..xe.|..j.....D
-00003650: 5d57 007d 0500 740b 007c 0500 8301 0064  ]W.}..t..|.....d
-00003660: 0100 6b02 0072 b900 7c05 007d 0600 7198  ..k..r..|..}..q.
-00003670: 0074 0b00 7c05 0083 0100 6402 006b 0200  .t..|.....d..k..
-00003680: 72d4 007c 0500 7d07 0071 9800 740b 007c  r..|..}..q..t..|
-00003690: 0500 8301 0064 0300 6b02 0072 9800 7c05  .....d..k..r..|.
-000036a0: 007d 0800 7198 0071 9800 577c 0000 6a0c  .}..q..q..W|..j.
-000036b0: 0069 0100 6404 0074 0b00 7c00 006a 0300  .i..d..t..|..j..
-000036c0: 8301 0036 740d 007c 0400 7c06 0019 8301  ...6t..|..|.....
-000036d0: 0083 0200 017c 0000 6a0c 0069 0200 6405  .....|..j..i..d.
-000036e0: 0074 0b00 7c00 006a 0300 8301 0036 6406  .t..|..j.....6d.
-000036f0: 0074 0b00 7c00 006a 0800 8301 0036 740d  .t..|..j.....6t.
-00003700: 007c 0400 7c07 0019 8301 0083 0200 017c  .|..|..........|
-00003710: 0000 6a0c 0069 0100 6407 0074 0b00 7c00  ..j..i..d..t..|.
-00003720: 006a 0300 8301 0036 740d 007c 0400 7c08  .j.....6t..|..|.
-00003730: 0019 8301 0083 0200 0164 0000 5328 0800  .........d..S(..
-00003740: 0000 4e73 0c00 0000 3c48 4f47 2833 2e45  ..Ns....<HOG(3.E
-00003750: 2e31 293e 730c 0000 003c 484f 4728 312e  .1)>s....<HOG(1.
-00003760: 4d2e 4529 3e73 0a00 0000 3c48 4f47 2832  M.E)>s....<HOG(2
-00003770: 2e45 293e 7307 0000 0047 656e 6528 3329  .E)>s....Gene(3)
-00003780: 7307 0000 0047 656e 6528 3129 7308 0000  s....Gene(1)s...
-00003790: 0047 656e 6528 3431 2973 0700 0000 4765  .Gene(41)s....Ge
-000037a0: 6e65 2832 2928 0e00 0000 5203 0000 0052  ne(2)(....R....R
-000037b0: 2d00 0000 5202 0000 0052 2f00 0000 5238  -...R....R/...R8
-000037c0: 0000 0052 5600 0000 5257 0000 0052 8600  ...RV...RW...R..
-000037d0: 0000 5232 0000 0052 9700 0000 520b 0000  ..R2...R....R...
-000037e0: 0052 0600 0000 526a 0000 0052 1200 0000  .R....Rj...R....
-000037f0: 2809 0000 0052 3900 0000 529f 0000 0052  (....R9...R....R
-00003800: a200 0000 52a3 0000 0052 9800 0000 5252  ....R....R....RR
-00003810: 0000 0052 a500 0000 7406 0000 0048 315f  ...R....t....H1_
-00003820: 4d5f 4552 a600 0000 2800 0000 0028 0000  M_ER....(....(..
-00003830: 0000 7347 0000 002f 5573 6572 732f 6164  ..sG.../Users/ad
-00003840: 6d69 6e2f 576f 726b 2f70 726f 6a65 6374  min/Work/project
-00003850: 2f44 6573 7369 6d6f 7a2f 7079 6861 6d2d  /Dessimoz/pyham-
-00003860: 6465 762f 7079 6861 6d2f 7465 7374 732f  dev/pyham/tests/
-00003870: 7465 7374 5f6d 6170 7065 722e 7079 5299  test_mapper.pyR.
-00003880: 0000 0044 0100 0073 2400 0000 0001 0f02  ...D...s$.......
-00003890: 1b01 1001 0d02 1b01 1001 0d02 0c02 1301  ................
-000038a0: 1201 0901 1201 0901 1201 0d02 2a01 3a01  ............*.:.
-000038b0: 6301 0000 0007 0000 0005 0000 0043 0000  c............C..
-000038c0: 0073 0401 0000 7400 007c 0000 6a01 0083  .s....t..|..j...
-000038d0: 0100 7d01 0074 0200 7c00 006a 0100 7c00  ..}..t..|..j..|.
-000038e0: 006a 0300 7c00 006a 0400 8303 007d 0200  .j..|..j.....}..
-000038f0: 7c00 006a 0500 7c02 006a 0600 8301 0001  |..j..|..j......
-00003900: 7c01 006a 0700 7c02 0083 0100 0174 0200  |..j..|......t..
-00003910: 7c00 006a 0100 7c00 006a 0800 7c00 006a  |..j..|..j..|..j
-00003920: 0400 8303 007d 0300 7c00 006a 0500 7c03  .....}..|..j..|.
-00003930: 006a 0600 8301 0001 7c01 006a 0700 7c03  .j......|..j..|.
-00003940: 0083 0100 017c 0100 6a09 0083 0000 7d04  .....|..j.....}.
-00003950: 0078 2f00 7c04 006a 0a00 8300 0044 5d21  .x/.|..j.....D]!
-00003960: 007d 0500 740b 007c 0500 8301 0064 0100  .}..t..|.....d..
-00003970: 6b02 0072 9800 7c05 007d 0600 7198 0071  k..r..|..}..q..q
-00003980: 9800 577c 0000 6a0c 0069 0200 6402 0068  ..W|..j..i..d..h
-00003990: 0100 740b 007c 0000 6a03 0083 0100 3664  ..t..|..j.....6d
-000039a0: 0300 6404 0068 0200 740b 007c 0000 6a08  ..d..h..t..|..j.
-000039b0: 0083 0100 3674 0d00 7c04 007c 0600 1983  ....6t..|..|....
-000039c0: 0100 8302 0001 6400 0053 2805 0000 004e  ......d..S(....N
-000039d0: 7308 0000 003c 484f 4728 3329 3e73 0700  s....<HOG(3)>s..
-000039e0: 0000 4765 6e65 2833 2973 0800 0000 4765  ..Gene(3)s....Ge
-000039f0: 6e65 2833 3329 7308 0000 0047 656e 6528  ne(33)s....Gene(
-00003a00: 3334 2928 0e00 0000 5203 0000 0052 2d00  34)(....R....R-.
-00003a10: 0000 5202 0000 0052 2f00 0000 5235 0000  ..R....R/...R5..
-00003a20: 0052 5600 0000 5257 0000 0052 8600 0000  .RV...RW...R....
-00003a30: 5231 0000 0052 9a00 0000 520b 0000 0052  R1...R....R....R
-00003a40: 0600 0000 526a 0000 0052 1500 0000 2807  ....Rj...R....(.
-00003a50: 0000 0052 3900 0000 529f 0000 0074 0e00  ...R9...R....t..
-00003a60: 0000 6d61 705f 6875 6d61 6e5f 7665 7274  ..map_human_vert
-00003a70: 740e 0000 006d 6170 5f6d 6f75 7365 5f76  t....map_mouse_v
-00003a80: 6572 7452 9b00 0000 5252 0000 0074 0100  ertR....RR...t..
-00003a90: 0000 4828 0000 0000 2800 0000 0073 4700  ..H(....(....sG.
-00003aa0: 0000 2f55 7365 7273 2f61 646d 696e 2f57  ../Users/admin/W
-00003ab0: 6f72 6b2f 7072 6f6a 6563 742f 4465 7373  ork/project/Dess
-00003ac0: 696d 6f7a 2f70 7968 616d 2d64 6576 2f70  imoz/pyham-dev/p
-00003ad0: 7968 616d 2f74 6573 7473 2f74 6573 745f  yham/tests/test_
-00003ae0: 6d61 7070 6572 2e70 7952 9c00 0000 5d01  mapper.pyR....].
-00003af0: 0000 7318 0000 0000 010f 021b 0110 010d  ..s.............
-00003b00: 021b 0110 010d 020c 0213 0112 010d 0228  ...............(
-00003b10: 0a00 0000 523e 0000 0052 3f00 0000 52a0  ....R>...R?...R.
-00003b20: 0000 0052 a100 0000 528d 0000 0052 8e00  ...R....R....R..
-00003b30: 0000 5293 0000 0052 9600 0000 5299 0000  ..R....R....R...
-00003b40: 0052 9c00 0000 2800 0000 0028 0000 0000  .R....(....(....
-00003b50: 2800 0000 0073 4700 0000 2f55 7365 7273  (....sG.../Users
-00003b60: 2f61 646d 696e 2f57 6f72 6b2f 7072 6f6a  /admin/Work/proj
-00003b70: 6563 742f 4465 7373 696d 6f7a 2f70 7968  ect/Dessimoz/pyh
-00003b80: 616d 2d64 6576 2f70 7968 616d 2f74 6573  am-dev/pyham/tes
-00003b90: 7473 2f74 6573 745f 6d61 7070 6572 2e70  ts/test_mapper.p
-00003ba0: 7952 9d00 0000 eb00 0000 7310 0000 0006  yR........s.....
-00003bb0: 0209 0f09 0c09 0909 0409 1f09 1009 1974  ...............t
-00003bc0: 0800 0000 5f5f 6d61 696e 5f5f 2800 0000  ....__main__(...
-00003bd0: 0028 1200 0000 5240 0000 0074 0500 0000  .(....R@...t....
-00003be0: 7079 6861 6d52 0000 0000 5201 0000 0052  pyhamR....R....R
-00003bf0: 0200 0000 5203 0000 0052 0400 0000 5225  ....R....R....R%
-00003c00: 0000 0052 0a00 0000 5212 0000 0052 1500  ...R....R....R..
-00003c10: 0000 5216 0000 0052 1700 0000 5242 0000  ..R....R....RB..
-00003c20: 0052 8500 0000 529d 0000 0052 3e00 0000  .R....R....R>...
-00003c30: 7404 0000 006d 6169 6e28 0000 0000 2800  t....main(....(.
-00003c40: 0000 0028 0000 0000 7347 0000 002f 5573  ...(....sG.../Us
-00003c50: 6572 732f 6164 6d69 6e2f 576f 726b 2f70  ers/admin/Work/p
-00003c60: 726f 6a65 6374 2f44 6573 7369 6d6f 7a2f  roject/Dessimoz/
-00003c70: 7079 6861 6d2d 6465 762f 7079 6861 6d2f  pyham-dev/pyham/
-00003c80: 7465 7374 732f 7465 7374 5f6d 6170 7065  tests/test_mappe
-00003c90: 722e 7079 7408 0000 003c 6d6f 6475 6c65  r.pyt....<module
-00003ca0: 3e01 0000 0073 1a00 0000 0c01 1001 1001  >....s..........
-00003cb0: 1c01 0c02 0907 0908 090b 1317 1961 1952  .............a.R
-00003cc0: 1985 0c01                                ....
+000001f0: 0000 0000 7334 0000 002f 5573 6572 732f  ....s4.../Users/
+00000200: 6164 7269 6161 6c2f 5265 706f 7369 746f  adriaal/Reposito
+00000210: 7269 6573 2f48 414d 2f74 6573 7473 2f74  ries/HAM/tests/t
+00000220: 6573 745f 6d61 7070 6572 2e70 7974 0a00  est_mapper.pyt..
+00000230: 0000 5f73 7472 5f61 7272 6179 0700 0000  .._str_array....
+00000240: 7308 0000 0000 0106 010d 0117 0163 0100  s............c..
+00000250: 0000 0400 0000 0500 0000 4300 0000 7361  ..........C...sa
+00000260: 0000 0078 2d00 7c00 006a 0000 8300 0044  ...x-.|..j.....D
+00000270: 5d1f 007d 0100 7c00 006a 0100 7c01 0083  ]..}..|..j..|...
+00000280: 0100 7c00 0074 0200 7c01 0083 0100 3c71  ..|..t..|.....<q
+00000290: 0d00 5778 2a00 7c00 006a 0300 8300 0044  ..Wx*.|..j.....D
+000002a0: 5d1c 005c 0200 7d02 007d 0300 7402 007c  ]..\..}..}..t..|
+000002b0: 0300 8301 007c 0000 7c02 003c 713d 0057  .....|..|..<q=.W
+000002c0: 7c00 0053 2801 0000 004e 2804 0000 0074  |..S(....N(....t
+000002d0: 0400 0000 6b65 7973 7403 0000 0070 6f70  ....keyst....pop
+000002e0: 5206 0000 0074 0500 0000 6974 656d 7328  R....t....items(
+000002f0: 0400 0000 7404 0000 0064 6963 7474 0200  ....t....dictt..
+00000300: 0000 6b6b 7401 0000 006b 7401 0000 0076  ..kkt....kt....v
+00000310: 2800 0000 0028 0000 0000 7334 0000 002f  (....(....s4.../
+00000320: 5573 6572 732f 6164 7269 6161 6c2f 5265  Users/adriaal/Re
+00000330: 706f 7369 746f 7269 6573 2f48 414d 2f74  positories/HAM/t
+00000340: 6573 7473 2f74 6573 745f 6d61 7070 6572  ests/test_mapper
+00000350: 2e70 7974 1300 0000 5f73 7472 5f64 6963  .pyt...._str_dic
+00000360: 745f 6f6e 655f 7661 6c75 650e 0000 0073  t_one_value....s
+00000370: 0a00 0000 0001 1301 1d01 1901 1401 6301  ..............c.
+00000380: 0000 0006 0000 0005 0000 0043 0000 0073  ...........C...s
+00000390: 8b00 0000 782d 007c 0000 6a00 0083 0000  ....x-.|..j.....
+000003a0: 445d 1f00 7d01 007c 0000 6a01 007c 0100  D]..}..|..j..|..
+000003b0: 8301 007c 0000 7402 007c 0100 8301 003c  ...|..t..|.....<
+000003c0: 710d 0057 7854 007c 0000 6a03 0083 0000  q..WxT.|..j.....
+000003d0: 445d 4600 5c02 007d 0200 7d03 0067 0000  D]F.\..}..}..g..
+000003e0: 7d04 0078 2100 7c03 0044 5d19 007d 0500  }..x!.|..D]..}..
+000003f0: 7c04 006a 0400 7402 007c 0500 8301 0083  |..j..t..|......
+00000400: 0100 0171 5600 5774 0500 7c04 0083 0100  ...qV.Wt..|.....
+00000410: 7c00 007c 0200 3c71 3d00 577c 0000 5328  |..|..<q=.W|..S(
+00000420: 0100 0000 4e28 0600 0000 520b 0000 0052  ....N(....R....R
+00000430: 0c00 0000 5206 0000 0052 0d00 0000 5205  ....R....R....R.
+00000440: 0000 0074 0300 0000 7365 7428 0600 0000  ...t....set(....
+00000450: 520e 0000 0052 0f00 0000 5210 0000 0074  R....R....R....t
+00000460: 0200 0000 7673 5207 0000 0052 1100 0000  ....vsR....R....
+00000470: 2800 0000 0028 0000 0000 7334 0000 002f  (....(....s4.../
+00000480: 5573 6572 732f 6164 7269 6161 6c2f 5265  Users/adriaal/Re
+00000490: 706f 7369 746f 7269 6573 2f48 414d 2f74  positories/HAM/t
+000004a0: 6573 7473 2f74 6573 745f 6d61 7070 6572  ests/test_mapper
+000004b0: 2e70 7974 1500 0000 5f73 7472 5f64 6963  .pyt...._str_dic
+000004c0: 745f 6172 7261 795f 7661 6c75 6516 0000  t_array_value...
+000004d0: 0073 1000 0000 0001 1301 1d01 1901 0601  .s..............
+000004e0: 0d01 1701 1401 740f 0000 004d 6170 7065  ......t....Mappe
+000004f0: 7254 6573 7443 6173 6573 6300 0000 0000  rTestCasesc.....
+00000500: 0000 0003 0000 0042 0000 0073 2100 0000  .......B...s!...
+00000510: 6500 005a 0100 6400 0065 0200 6a03 0066  e..Z..d..e..j..f
+00000520: 0100 6401 0084 0000 8300 0059 5a04 0052  ..d........YZ..R
+00000530: 5328 0200 0000 740a 0000 004d 6170 7065  S(....t....Mappe
+00000540: 7254 6573 7463 0000 0000 0000 0000 0100  rTestc..........
+00000550: 0000 4200 0000 7311 0000 0065 0000 5a01  ..B...s....e..Z.
+00000560: 0064 0000 8400 005a 0200 5253 2801 0000  .d.....Z..RS(...
+00000570: 0063 0100 0000 0400 0000 0900 0000 4300  .c............C.
+00000580: 0000 737e 0100 0074 0000 6a01 006a 0200  ..s~...t..j..j..
+00000590: 7400 006a 0100 6a03 0074 0400 8301 0064  t..j..j..t.....d
+000005a0: 0100 8302 007d 0100 7405 006a 0600 7c01  .....}..t..j..|.
+000005b0: 0064 0200 6403 0083 0101 7d02 0074 0000  .d..d.....}..t..
+000005c0: 6a01 006a 0200 7400 006a 0100 6a03 0074  j..j..t..j..j..t
+000005d0: 0400 8301 0064 0400 8302 007d 0300 7407  .....d.....}..t.
+000005e0: 006a 0800 6405 007c 0200 6406 007c 0300  .j..d..|..d..|..
+000005f0: 6407 0064 0800 6409 0074 0900 8300 047c  d..d..d..t.....|
+00000600: 0000 5f0a 007c 0000 6a0a 006a 0b00 640a  .._..|..j..j..d.
+00000610: 0064 0b00 8300 017c 0000 5f0c 007c 0000  .d.....|.._..|..
+00000620: 6a0a 006a 0b00 640a 0064 0c00 8300 017c  j..j..d..d.....|
+00000630: 0000 5f0d 007c 0000 6a0a 006a 0b00 640a  .._..|..j..j..d.
+00000640: 0064 0d00 8300 017c 0000 5f0e 007c 0000  .d.....|.._..|..
+00000650: 6a0a 006a 0b00 640a 0064 0e00 8300 017c  j..j..d..d.....|
+00000660: 0000 5f0f 007c 0000 6a0a 006a 0b00 640a  .._..|..j..j..d.
+00000670: 0064 0f00 8300 017c 0000 5f10 007c 0000  .d.....|.._..|..
+00000680: 6a0a 006a 1100 7c00 006a 0c00 7c00 006a  j..j..|..j..|..j
+00000690: 0d00 6802 0083 0100 7c00 005f 1200 7c00  ..h.....|.._..|.
+000006a0: 006a 0a00 6a11 007c 0000 6a0e 007c 0000  .j..j..|..j..|..
+000006b0: 6a0f 0068 0200 8301 007c 0000 5f13 007c  j..h.....|.._..|
+000006c0: 0000 6a0a 006a 1100 7c00 006a 0c00 7c00  ..j..j..|..j..|.
+000006d0: 006a 1000 6802 0083 0100 7c00 005f 1400  .j..h.....|.._..
+000006e0: 7c00 006a 0a00 6a11 007c 0000 6a0c 007c  |..j..j..|..j..|
+000006f0: 0000 6a0e 0068 0200 8301 007c 0000 5f15  ..j..h.....|.._.
+00000700: 0064 0000 5328 1000 0000 4e73 1300 0000  .d..S(....Ns....
+00000710: 2e2f 6461 7461 2f73 696d 706c 6545 782e  ./data/simpleEx.
+00000720: 6e77 6b74 0400 0000 7479 7065 7403 0000  nwkt....typet...
+00000730: 006e 776b 7318 0000 002e 2f64 6174 612f  .nwks...../data/
+00000740: 7369 6d70 6c65 4578 2e6f 7274 686f 786d  simpleEx.orthoxm
+00000750: 6c74 0900 0000 7472 6565 5f66 696c 6574  lt....tree_filet
+00000760: 0800 0000 686f 675f 6669 6c65 740d 0000  ....hog_filet...
+00000770: 0074 7970 655f 686f 675f 6669 6c65 7408  .type_hog_filet.
+00000780: 0000 006f 7274 686f 786d 6c74 1100 0000  ...orthoxmlt....
+00000790: 7573 655f 696e 7465 726e 616c 5f6e 616d  use_internal_nam
+000007a0: 6574 0400 0000 6e61 6d65 7405 0000 0048  et....namet....H
+000007b0: 554d 414e 7405 0000 0058 454e 5452 7405  UMANt....XENTRt.
+000007c0: 0000 004d 4f55 5345 7405 0000 0052 4154  ...MOUSEt....RAT
+000007d0: 4e4f 7405 0000 0050 414e 5452 2816 0000  NOt....PANTR(...
+000007e0: 0074 0200 0000 6f73 7404 0000 0070 6174  .t....ost....pat
+000007f0: 6874 0400 0000 6a6f 696e 7407 0000 0064  ht....joint....d
+00000800: 6972 6e61 6d65 7408 0000 005f 5f66 696c  irnamet....__fil
+00000810: 655f 5f52 0100 0000 7411 0000 0067 6574  e__R....t....get
+00000820: 5f6e 6577 6963 6b5f 7374 7269 6e67 5200  _newick_stringR.
+00000830: 0000 0074 0300 0000 4861 6d74 0400 0000  ...t....Hamt....
+00000840: 5472 7565 740c 0000 0068 616d 5f61 6e61  Truet....ham_ana
+00000850: 6c79 7369 7374 1900 0000 6765 745f 6578  lysist....get_ex
+00000860: 7461 6e74 5f67 656e 6f6d 655f 6279 5f6e  tant_genome_by_n
+00000870: 616d 6574 0500 0000 6875 6d61 6e74 0400  amet....humant..
+00000880: 0000 6672 6f67 7405 0000 006d 6f75 7365  ..frogt....mouse
+00000890: 7403 0000 0072 6174 7405 0000 0063 6869  t....ratt....chi
+000008a0: 6d70 742a 0000 0067 6574 5f61 6e63 6573  mpt*...get_ances
+000008b0: 7472 616c 5f67 656e 6f6d 655f 6279 5f6d  tral_genome_by_m
+000008c0: 7263 615f 6f66 5f67 656e 6f6d 655f 7365  rca_of_genome_se
+000008d0: 7474 0b00 0000 7665 7274 6562 7261 7465  tt....vertebrate
+000008e0: 7374 0700 0000 726f 6465 6e74 7374 0800  st....rodentst..
+000008f0: 0000 7072 696d 6174 6573 7410 0000 0065  ..primatest....e
+00000900: 7561 7263 686f 6e74 6f67 6c69 7265 7328  uarchontoglires(
+00000910: 0400 0000 7404 0000 0073 656c 6674 0800  ....t....selft..
+00000920: 0000 6e77 6b5f 7061 7468 7408 0000 0074  ..nwk_patht....t
+00000930: 7265 655f 7374 7274 0d00 0000 6f72 7468  ree_strt....orth
+00000940: 6f78 6d6c 5f70 6174 6828 0000 0000 2800  oxml_path(....(.
+00000950: 0000 0073 3400 0000 2f55 7365 7273 2f61  ...s4.../Users/a
+00000960: 6472 6961 616c 2f52 6570 6f73 6974 6f72  driaal/Repositor
+00000970: 6965 732f 4841 4d2f 7465 7374 732f 7465  ies/HAM/tests/te
+00000980: 7374 5f6d 6170 7065 722e 7079 7405 0000  st_mapper.pyt...
+00000990: 0073 6574 5570 2400 0000 731c 0000 0000  .setUp$...s.....
+000009a0: 0221 0115 0121 0227 0218 0118 0118 0118  .!...!.'........
+000009b0: 0118 0121 0121 0121 0109 0128 0300 0000  ...!.!.!...(....
+000009c0: 7408 0000 005f 5f6e 616d 655f 5f74 0a00  t....__name__t..
+000009d0: 0000 5f5f 6d6f 6475 6c65 5f5f 523d 0000  ..__module__R=..
+000009e0: 0028 0000 0000 2800 0000 0028 0000 0000  .(....(....(....
+000009f0: 7334 0000 002f 5573 6572 732f 6164 7269  s4.../Users/adri
+00000a00: 6161 6c2f 5265 706f 7369 746f 7269 6573  aal/Repositories
+00000a10: 2f48 414d 2f74 6573 7473 2f74 6573 745f  /HAM/tests/test_
+00000a20: 6d61 7070 6572 2e70 7952 1700 0000 2300  mapper.pyR....#.
+00000a30: 0000 7302 0000 0006 0128 0500 0000 523e  ..s......(....R>
+00000a40: 0000 0052 3f00 0000 7408 0000 0075 6e69  ...R?...t....uni
+00000a50: 7474 6573 7474 0800 0000 5465 7374 4361  ttestt....TestCa
+00000a60: 7365 5217 0000 0028 0000 0000 2800 0000  seR....(....(...
+00000a70: 0028 0000 0000 7334 0000 002f 5573 6572  .(....s4.../User
+00000a80: 732f 6164 7269 6161 6c2f 5265 706f 7369  s/adriaal/Reposi
+00000a90: 746f 7269 6573 2f48 414d 2f74 6573 7473  tories/HAM/tests
+00000aa0: 2f74 6573 745f 6d61 7070 6572 2e70 7952  /test_mapper.pyR
+00000ab0: 1600 0000 2100 0000 7302 0000 0006 0274  ....!...s......t
+00000ac0: 0b00 0000 484f 4773 4d61 7054 6573 7463  ....HOGsMapTestc
+00000ad0: 0000 0000 0000 0000 0100 0000 4200 0000  ............B...
+00000ae0: 733e 0000 0065 0000 5a01 0064 0000 8400  s>...e..Z..d....
+00000af0: 005a 0200 6401 0084 0000 5a03 0064 0200  .Z..d.....Z..d..
+00000b00: 8400 005a 0400 6403 0084 0000 5a05 0064  ...Z..d.....Z..d
+00000b10: 0400 8400 005a 0600 6405 0084 0000 5a07  .....Z..d.....Z.
+00000b20: 0052 5328 0600 0000 6302 0000 0002 0000  .RS(....c.......
+00000b30: 0005 0000 0043 0000 0073 9500 0000 7400  .....C...s....t.
+00000b40: 007c 0100 7401 006a 0200 6a03 0083 0200  .|..t..j..j.....
+00000b50: 721c 007c 0100 6a04 0053 7400 007c 0100  r..|..j..St..|..
+00000b60: 7401 006a 0200 6a05 0083 0200 7257 007c  t..j..j.....rW.|
+00000b70: 0100 6a06 0064 0000 6b03 0072 4700 7c01  ..j..d..k..rG.|.
+00000b80: 006a 0600 537c 0100 6a08 006a 0900 6a0a  .j..S|..j..j..j.
+00000b90: 0053 6e3a 007c 0100 6400 006b 0200 7267  .Sn:.|..d..k..rg
+00000ba0: 007c 0100 5374 0b00 6401 006a 0c00 7401  .|..St..d..j..t.
+00000bb0: 006a 0200 6a0d 006a 0e00 740f 007c 0100  .j..j..j..t..|..
+00000bc0: 8301 006a 0e00 8302 0083 0100 8201 0064  ...j...........d
+00000bd0: 0000 5328 0200 0000 4e73 2300 0000 6578  ..S(....Ns#...ex
+00000be0: 7065 6374 2073 7562 636c 6173 7320 6f62  pect subclass ob
+00000bf0: 6a20 6f66 2027 7b7d 272c 2067 6f74 207b  j of '{}', got {
+00000c00: 7d28 1000 0000 740a 0000 0069 7369 6e73  }(....t....isins
+00000c10: 7461 6e63 6552 0000 0000 740c 0000 0061  tanceR....t....a
+00000c20: 6273 7472 6163 7467 656e 6574 0400 0000  bstractgenet....
+00000c30: 4765 6e65 7409 0000 0075 6e69 7175 655f  Genet....unique_
+00000c40: 6964 7403 0000 0048 4f47 7406 0000 0068  idt....HOGt....h
+00000c50: 6f67 5f69 6474 0400 0000 4e6f 6e65 7406  og_idt....Nonet.
+00000c60: 0000 0067 656e 6f6d 6574 0500 0000 7461  ...genomet....ta
+00000c70: 786f 6e52 1f00 0000 7409 0000 0054 7970  xonR....t....Typ
+00000c80: 6545 7272 6f72 7406 0000 0066 6f72 6d61  eErrort....forma
+00000c90: 7474 0c00 0000 4162 7374 7261 6374 4765  tt....AbstractGe
+00000ca0: 6e65 523e 0000 0052 1800 0000 2802 0000  neR>...R....(...
+00000cb0: 0052 3900 0000 7404 0000 0069 7465 6d28  .R9...t....item(
+00000cc0: 0000 0000 2800 0000 0073 3400 0000 2f55  ....(....s4.../U
+00000cd0: 7365 7273 2f61 6472 6961 616c 2f52 6570  sers/adriaal/Rep
+00000ce0: 6f73 6974 6f72 6965 732f 4841 4d2f 7465  ositories/HAM/te
+00000cf0: 7374 732f 7465 7374 5f6d 6170 7065 722e  sts/test_mapper.
+00000d00: 7079 740f 0000 005f 6765 745f 6964 656e  pyt...._get_iden
+00000d10: 7469 6669 6572 3a00 0000 7316 0000 0000  tifier:...s.....
+00000d20: 0115 0107 0115 010f 0107 0210 010c 0104  ................
+00000d30: 0209 010c 0163 0200 0000 0300 0000 0200  .....c..........
+00000d40: 0000 4300 0000 732c 0000 007c 0100 7d02  ..C...s,...|..}.
+00000d50: 0078 1c00 7c02 006a 0000 6400 006b 0900  .x..|..j..d..k..
+00000d60: 7224 007c 0200 6a00 007d 0200 7109 0057  r$.|..j..}..q..W
+00000d70: 7c02 006a 0200 5328 0100 0000 4e28 0300  |..j..S(....N(..
+00000d80: 0000 7406 0000 0070 6172 656e 7452 4900  ..t....parentRI.
+00000d90: 0000 5248 0000 0028 0300 0000 5239 0000  ..RH...(....R9..
+00000da0: 0074 0300 0000 686f 6774 0b00 0000 6375  .t....hogt....cu
+00000db0: 7272 656e 745f 686f 6728 0000 0000 2800  rrent_hog(....(.
+00000dc0: 0000 0073 3400 0000 2f55 7365 7273 2f61  ...s4.../Users/a
+00000dd0: 6472 6961 616c 2f52 6570 6f73 6974 6f72  driaal/Repositor
+00000de0: 6965 732f 4841 4d2f 7465 7374 732f 7465  ies/HAM/tests/te
+00000df0: 7374 5f6d 6170 7065 722e 7079 7410 0000  st_mapper.pyt...
+00000e00: 005f 6765 745f 746f 704c 6576 656c 5f69  ._get_topLevel_i
+00000e10: 6449 0000 0073 0800 0000 0001 0601 1201  dI...s..........
+00000e20: 0d01 6301 0000 0002 0000 0004 0000 0043  ..c............C
+00000e30: 0000 0073 5e00 0000 7400 007c 0000 6a01  ...s^...t..|..j.
+00000e40: 007c 0000 6a02 007c 0000 6a03 0083 0300  .|..j..|..j.....
+00000e50: 7d01 007c 0000 6a04 007c 0100 6a05 0083  }..|..j..|..j...
+00000e60: 0100 017c 0000 6a06 0064 0100 7c01 006a  ...|..j..d..|..j
+00000e70: 0700 6a08 006a 0900 8302 0001 7c00 006a  ..j..j......|..j
+00000e80: 0600 7c00 006a 0200 7c01 006a 0a00 8302  ..|..j..|..j....
+00000e90: 0001 6400 0053 2802 0000 004e 7410 0000  ..d..S(....Nt...
+00000ea0: 0045 7561 7263 686f 6e74 6f67 6c69 7265  .Euarchontoglire
+00000eb0: 7328 0b00 0000 5202 0000 0052 2d00 0000  s(....R....R-...
+00000ec0: 522f 0000 0052 3800 0000 740a 0000 0061  R/...R8...t....a
+00000ed0: 7373 6572 7454 7275 6574 0a00 0000 636f  ssertTruet....co
+00000ee0: 6e73 6973 7465 6e74 740b 0000 0061 7373  nsistentt....ass
+00000ef0: 6572 7445 7175 616c 7408 0000 0061 6e63  ertEqualt....anc
+00000f00: 6573 746f 7252 4b00 0000 521f 0000 0074  estorRK...R....t
+00000f10: 0a00 0000 6465 7363 656e 6461 6e74 2802  ....descendant(.
+00000f20: 0000 0052 3900 0000 7403 0000 006d 6170  ...R9...t....map
+00000f30: 2800 0000 0028 0000 0000 7334 0000 002f  (....(....s4.../
+00000f40: 5573 6572 732f 6164 7269 6161 6c2f 5265  Users/adriaal/Re
+00000f50: 706f 7369 746f 7269 6573 2f48 414d 2f74  positories/HAM/t
+00000f60: 6573 7473 2f74 6573 745f 6d61 7070 6572  ests/test_mapper
+00000f70: 2e70 7974 2000 0000 7465 7374 5f73 6574  .pyt ...test_set
+00000f80: 5f61 6e63 6573 746f 725f 616e 645f 6465  _ancestor_and_de
+00000f90: 7363 656e 6461 6e74 4f00 0000 7308 0000  scendantO...s...
+00000fa0: 0000 031b 0110 0119 0163 0100 0000 0200  .........c......
+00000fb0: 0000 0800 0000 4300 0000 7345 0000 007c  ......C...sE...|
+00000fc0: 0000 6a00 0074 0100 8301 008f 3000 0174  ..j..t......0..t
+00000fd0: 0200 7c00 006a 0300 7c00 006a 0400 7c00  ..|..j..|..j..|.
+00000fe0: 006a 0500 8303 007d 0100 7c00 006a 0600  .j.....}..|..j..
+00000ff0: 7c01 006a 0700 8301 0001 5764 0000 5158  |..j......Wd..QX
+00001000: 6400 0053 2801 0000 004e 2808 0000 0074  d..S(....N(....t
+00001010: 0c00 0000 6173 7365 7274 5261 6973 6573  ....assertRaises
+00001020: 524c 0000 0052 0200 0000 522d 0000 0052  RL...R....R-...R
+00001030: 3000 0000 5237 0000 0052 5600 0000 5257  0...R7...RV...RW
+00001040: 0000 0028 0200 0000 5239 0000 0074 0400  ...(....R9...t..
+00001050: 0000 6d61 7032 2800 0000 0028 0000 0000  ..map2(....(....
+00001060: 7334 0000 002f 5573 6572 732f 6164 7269  s4.../Users/adri
+00001070: 6161 6c2f 5265 706f 7369 746f 7269 6573  aal/Repositories
+00001080: 2f48 414d 2f74 6573 7473 2f74 6573 745f  /HAM/tests/test_
+00001090: 6d61 7070 6572 2e70 7974 1e00 0000 7465  mapper.pyt....te
+000010a0: 7374 5f61 6464 5f67 656e 6f6d 655f 6e6f  st_add_genome_no
+000010b0: 745f 6f6e 5f6c 696e 6561 6765 5700 0000  t_on_lineageW...
+000010c0: 7306 0000 0000 0210 011b 0163 0100 0000  s..........c....
+000010d0: 0500 0000 0400 0000 0300 0000 737f 0000  ............s...
+000010e0: 0087 0000 6601 0064 0100 8600 007d 0100  ....f..d.....}..
+000010f0: 7400 0088 0000 6a01 0088 0000 6a02 0088  t.....j.....j...
+00001100: 0000 6a03 0083 0300 7d02 0088 0000 6a04  ..j.....}.....j.
+00001110: 007c 0200 6a05 0083 0100 0169 0400 6402  .|..j......i..d.
+00001120: 0064 0200 3664 0000 6403 0036 6404 0064  .d..6d..d..6d..d
+00001130: 0400 3664 0000 6405 0036 7d03 007c 0100  ..6d..d..6}..|..
+00001140: 7c02 006a 0700 8301 007d 0400 8800 006a  |..j.....}.....j
+00001150: 0800 7c03 007c 0400 8302 0001 6400 0053  ..|..|......d..S
+00001160: 2806 0000 004e 6301 0000 0004 0000 0005  (....Nc.........
+00001170: 0000 0013 0000 0073 4700 0000 6900 007d  .......sG...i..}
+00001180: 0100 783a 007c 0000 6a00 0083 0000 445d  ..x:.|..j.....D]
+00001190: 2c00 5c02 007d 0200 7d03 0088 0000 6a01  ,.\..}..}.....j.
+000011a0: 007c 0300 6401 0019 8301 007c 0100 8800  .|..d......|....
+000011b0: 006a 0100 7c02 0083 0100 3c71 1300 577c  .j..|.....<q..W|
+000011c0: 0100 5328 0200 0000 4e69 0000 0000 2802  ..S(....Ni....(.
+000011d0: 0000 0052 0d00 0000 5250 0000 0028 0400  ...R....RP...(..
+000011e0: 0000 740c 0000 0073 696e 676c 655f 6d61  ..t....single_ma
+000011f0: 7055 7074 0c00 0000 6f62 7365 7276 6564  pUpt....observed
+00001200: 5f6d 6170 7406 0000 0073 6f75 7263 6574  _mapt....sourcet
+00001210: 0600 0000 7461 7267 6574 2801 0000 0052  ....target(....R
+00001220: 3900 0000 2800 0000 0073 3400 0000 2f55  9...(....s4.../U
+00001230: 7365 7273 2f61 6472 6961 616c 2f52 6570  sers/adriaal/Rep
+00001240: 6f73 6974 6f72 6965 732f 4841 4d2f 7465  ositories/HAM/te
+00001250: 7374 732f 7465 7374 5f6d 6170 7065 722e  sts/test_mapper.
+00001260: 7079 740c 0000 005f 636f 6e76 6572 745f  pyt...._convert_
+00001270: 6d61 705f 0000 0073 0800 0000 0001 0601  map_...s........
+00001280: 1901 2401 7401 0000 0031 7401 0000 0032  ..$.t....1t....2
+00001290: 7401 0000 0033 7401 0000 0035 2809 0000  t....3t....5(...
+000012a0: 0052 0200 0000 522d 0000 0052 2f00 0000  .R....R-...R/...
+000012b0: 5235 0000 0052 5600 0000 5257 0000 0052  R5...RV...RW...R
+000012c0: 4900 0000 7405 0000 0075 704d 6170 740f  I...t....upMapt.
+000012d0: 0000 0061 7373 6572 7444 6963 7445 7175  ...assertDictEqu
+000012e0: 616c 2805 0000 0052 3900 0000 5264 0000  al(....R9...Rd..
+000012f0: 0052 5b00 0000 740c 0000 0065 7870 6563  .R[...t....expec
+00001300: 7465 645f 6d61 7052 6100 0000 2800 0000  ted_mapRa...(...
+00001310: 0028 0100 0000 5239 0000 0073 3400 0000  .(....R9...s4...
+00001320: 2f55 7365 7273 2f61 6472 6961 616c 2f52  /Users/adriaal/R
+00001330: 6570 6f73 6974 6f72 6965 732f 4841 4d2f  epositories/HAM/
+00001340: 7465 7374 732f 7465 7374 5f6d 6170 7065  tests/test_mappe
+00001350: 722e 7079 740a 0000 0074 6573 745f 5570  r.pyt....test_Up
+00001360: 4d61 705d 0000 0073 0c00 0000 0002 0f07  Map]...s........
+00001370: 1b01 1001 2201 0f01 6301 0000 000a 0000  ...."...c.......
+00001380: 0004 0000 0043 0000 0073 2701 0000 6401  .....C...s'...d.
+00001390: 0084 0000 7d01 0064 0200 8400 007d 0200  ....}..d.....}..
+000013a0: 6403 0084 0000 7d03 0064 0400 8400 007d  d.....}..d.....}
+000013b0: 0400 7400 007c 0000 6a01 007c 0000 6a02  ..t..|..j..|..j.
+000013c0: 007c 0000 6a03 0083 0300 7d05 007c 0000  .|..j.....}..|..
+000013d0: 6a04 007c 0500 6a05 0083 0100 0174 0600  j..|..j......t..
+000013e0: 8300 007d 0600 7c00 006a 0700 7c06 007c  ...}..|..j..|..|
+000013f0: 0100 7c05 006a 0800 8301 0083 0200 0174  ..|..j.........t
+00001400: 0600 8300 007d 0700 7c07 006a 0900 6405  .....}..|..j..d.
+00001410: 0083 0100 017c 0700 6a09 0064 0600 8301  .....|..j..d....
+00001420: 0001 7c00 006a 0700 7c07 007c 0200 7c05  ..|..j..|..|..|.
+00001430: 006a 0a00 8301 0083 0200 0174 0600 8300  .j.........t....
+00001440: 007d 0800 7c08 006a 0900 740b 0064 0700  .}..|..j..t..d..
+00001450: 6408 0067 0200 8301 0083 0100 017c 0000  d..g.........|..
+00001460: 6a07 007c 0800 7c03 007c 0500 6a0c 0083  j..|..|..|..j...
+00001470: 0100 8302 0001 7406 0083 0000 7d09 007c  ......t.....}..|
+00001480: 0900 6a09 0074 0b00 6409 0064 0a00 6702  ..j..t..d..d..g.
+00001490: 0083 0100 8301 0001 7c00 006a 0700 7c09  ........|..j..|.
+000014a0: 007c 0400 7c05 006a 0d00 8301 0083 0200  .|..|..j........
+000014b0: 0164 0000 5328 0b00 0000 4e63 0100 0000  .d..S(....Nc....
+000014c0: 0200 0000 0500 0000 5300 0000 7323 0000  ........S...s#..
+000014d0: 0074 0000 6700 007c 0000 445d 1200 7d01  .t..g..|..D]..}.
+000014e0: 0074 0100 7c01 0083 0100 5e02 0071 0a00  .t..|.....^..q..
+000014f0: 8301 0053 2801 0000 004e 2802 0000 0052  ...S(....N(....R
+00001500: 1300 0000 5206 0000 0028 0200 0000 7404  ....R....(....t.
+00001510: 0000 004c 4f53 5374 0c00 0000 686f 675f  ...LOSSt....hog_
+00001520: 616e 6365 7374 6f72 2800 0000 0028 0000  ancestor(....(..
+00001530: 0000 7334 0000 002f 5573 6572 732f 6164  ..s4.../Users/ad
+00001540: 7269 6161 6c2f 5265 706f 7369 746f 7269  riaal/Repositori
+00001550: 6573 2f48 414d 2f74 6573 7473 2f74 6573  es/HAM/tests/tes
+00001560: 745f 6d61 7070 6572 2e70 7974 0c00 0000  t_mapper.pyt....
+00001570: 636f 6e76 6572 745f 4c4f 5353 6e00 0000  convert_LOSSn...
+00001580: 7302 0000 0000 0163 0100 0000 0200 0000  s......c........
+00001590: 0500 0000 5300 0000 7323 0000 0074 0000  ....S...s#...t..
+000015a0: 6700 007c 0000 445d 1200 7d01 0074 0100  g..|..D]..}..t..
+000015b0: 7c01 0083 0100 5e02 0071 0a00 8301 0053  |.....^..q.....S
+000015c0: 2801 0000 004e 2802 0000 0052 1300 0000  (....N(....R....
+000015d0: 5206 0000 0028 0200 0000 7404 0000 0047  R....(....t....G
+000015e0: 4149 4e74 0700 0000 6e65 775f 686f 6728  AINt....new_hog(
+000015f0: 0000 0000 2800 0000 0073 3400 0000 2f55  ....(....s4.../U
+00001600: 7365 7273 2f61 6472 6961 616c 2f52 6570  sers/adriaal/Rep
+00001610: 6f73 6974 6f72 6965 732f 4841 4d2f 7465  ositories/HAM/te
+00001620: 7374 732f 7465 7374 5f6d 6170 7065 722e  sts/test_mapper.
+00001630: 7079 740c 0000 0063 6f6e 7665 7274 5f47  pyt....convert_G
+00001640: 4149 4e71 0000 0073 0200 0000 0001 6301  AINq...s......c.
+00001650: 0000 0005 0000 0004 0000 0053 0000 0073  ...........S...s
+00001660: 5500 0000 7400 0083 0000 7d01 0078 4500  U...t.....}..xE.
+00001670: 7c00 006a 0100 8300 0044 5d37 005c 0200  |..j.....D]7.\..
+00001680: 7d02 007d 0300 7402 007c 0200 8301 0074  }..}..t..|.....t
+00001690: 0200 7c03 0083 0100 6702 007d 0400 7c01  ..|.....g..}..|.
+000016a0: 006a 0300 7404 007c 0400 8301 0083 0100  .j..t..|........
+000016b0: 0171 1600 577c 0100 5328 0100 0000 4e28  .q..W|..S(....N(
+000016c0: 0500 0000 5213 0000 0052 0d00 0000 5206  ....R....R....R.
+000016d0: 0000 0074 0300 0000 6164 6474 0900 0000  ...t....addt....
+000016e0: 6672 6f7a 656e 7365 7428 0500 0000 7408  frozenset(....t.
+000016f0: 0000 0052 4554 4149 4e45 4474 0900 0000  ...RETAINEDt....
+00001700: 6352 4554 4149 4e45 4452 6e00 0000 740e  cRETAINEDRn...t.
+00001710: 0000 0068 6f67 5f64 6573 6365 6e64 616e  ...hog_descendan
+00001720: 7474 0100 0000 7828 0000 0000 2800 0000  tt....x(....(...
+00001730: 0073 3400 0000 2f55 7365 7273 2f61 6472  .s4.../Users/adr
+00001740: 6961 616c 2f52 6570 6f73 6974 6f72 6965  iaal/Repositorie
+00001750: 732f 4841 4d2f 7465 7374 732f 7465 7374  s/HAM/tests/test
+00001760: 5f6d 6170 7065 722e 7079 7410 0000 0063  _mapper.pyt....c
+00001770: 6f6e 7665 7274 5f52 4554 4149 4e45 4474  onvert_RETAINEDt
+00001780: 0000 0073 0a00 0000 0001 0901 1901 1801  ...s............
+00001790: 1701 6301 0000 0006 0000 0005 0000 0053  ..c............S
+000017a0: 0000 0073 7000 0000 7400 0083 0000 7d01  ...sp...t.....}.
+000017b0: 0078 6000 7c00 006a 0100 8300 0044 5d52  .x`.|..j.....D]R
+000017c0: 005c 0200 7d02 007d 0300 7402 007c 0200  .\..}..}..t..|..
+000017d0: 8301 0067 0100 7d04 0078 2100 7c03 0044  ...g..}..x!.|..D
+000017e0: 5d19 007d 0500 7c04 006a 0300 7402 007c  ]..}..|..j..t..|
+000017f0: 0500 8301 0083 0100 0171 3800 577c 0100  .........q8.W|..
+00001800: 6a04 0074 0500 7c04 0083 0100 8301 0001  j..t..|.........
+00001810: 7116 0057 7c01 0053 2801 0000 004e 2806  q..W|..S(....N(.
+00001820: 0000 0052 1300 0000 520d 0000 0052 0600  ...R....R....R..
+00001830: 0000 5205 0000 0052 7300 0000 5274 0000  ..R....Rs...Rt..
+00001840: 0028 0600 0000 7409 0000 0044 5550 4c49  .(....t....DUPLI
+00001850: 4341 5445 740a 0000 0063 4455 504c 4943  CATEt....cDUPLIC
+00001860: 4154 4552 6e00 0000 740f 0000 0068 6f67  ATERn...t....hog
+00001870: 5f64 6573 6365 6e64 616e 7473 5278 0000  _descendantsRx..
+00001880: 0074 0100 0000 6728 0000 0000 2800 0000  .t....g(....(...
+00001890: 0073 3400 0000 2f55 7365 7273 2f61 6472  .s4.../Users/adr
+000018a0: 6961 616c 2f52 6570 6f73 6974 6f72 6965  iaal/Repositorie
+000018b0: 732f 4841 4d2f 7465 7374 732f 7465 7374  s/HAM/tests/test
+000018c0: 5f6d 6170 7065 722e 7079 7411 0000 0063  _mapper.pyt....c
+000018d0: 6f6e 7665 7274 5f44 5550 4c49 4341 5445  onvert_DUPLICATE
+000018e0: 7b00 0000 730e 0000 0000 0109 0119 010f  {...s...........
+000018f0: 010d 0117 0117 0173 0700 0000 4765 6e65  .......s....Gene
+00001900: 2832 2973 0700 0000 4765 6e65 2835 2973  (2)s....Gene(5)s
+00001910: 0800 0000 3c48 4f47 2831 293e 7307 0000  ....<HOG(1)>s...
+00001920: 0047 656e 6528 3129 7308 0000 003c 484f  .Gene(1)s....<HO
+00001930: 4728 3329 3e73 0700 0000 4765 6e65 2833  G(3)>s....Gene(3
+00001940: 2928 0e00 0000 5202 0000 0052 2d00 0000  )(....R....R-...
+00001950: 522f 0000 0052 3500 0000 5256 0000 0052  R/...R5...RV...R
+00001960: 5700 0000 5213 0000 0074 0e00 0000 6173  W...R....t....as
+00001970: 7365 7274 5365 7445 7175 616c 526d 0000  sertSetEqualRm..
+00001980: 0052 7300 0000 5270 0000 0052 7400 0000  .Rs...Rp...Rt...
+00001990: 5275 0000 0052 7a00 0000 280a 0000 0052  Ru...Rz...(....R
+000019a0: 3900 0000 526f 0000 0052 7200 0000 5279  9...Ro...Rr...Ry
+000019b0: 0000 0052 7e00 0000 525b 0000 0074 0d00  ...R~...R[...t..
+000019c0: 0000 6578 7065 6374 6564 5f4c 4f53 5374  ..expected_LOSSt
+000019d0: 0d00 0000 6578 7065 6374 6564 5f47 4149  ....expected_GAI
+000019e0: 4e74 1100 0000 6578 7065 6374 6564 5f52  Nt....expected_R
+000019f0: 4554 4149 4e45 4474 1200 0000 6578 7065  ETAINEDt....expe
+00001a00: 6374 6564 5f44 5550 4c49 4341 5445 2800  cted_DUPLICATE(.
+00001a10: 0000 0028 0000 0000 7334 0000 002f 5573  ...(....s4.../Us
+00001a20: 6572 732f 6164 7269 6161 6c2f 5265 706f  ers/adriaal/Repo
+00001a30: 7369 746f 7269 6573 2f48 414d 2f74 6573  sitories/HAM/tes
+00001a40: 7473 2f74 6573 745f 6d61 7070 6572 2e70  ts/test_mapper.p
+00001a50: 7974 1700 0000 7465 7374 5f62 7569 6c64  yt....test_build
+00001a60: 4576 656e 7443 6c75 7374 6572 736c 0000  EventClustersl..
+00001a70: 0073 2400 0000 0002 0903 0903 0907 090a  .s$.............
+00001a80: 1b01 1002 0901 1902 0901 0d01 0d01 1902  ................
+00001a90: 0901 1901 1902 0901 1901 2808 0000 0052  ..........(....R
+00001aa0: 3e00 0000 523f 0000 0052 5000 0000 5254  >...R?...RP...RT
+00001ab0: 0000 0052 5c00 0000 525f 0000 0052 6c00  ...R\...R_...Rl.
+00001ac0: 0000 5284 0000 0028 0000 0000 2800 0000  ..R....(....(...
+00001ad0: 0028 0000 0000 7334 0000 002f 5573 6572  .(....s4.../User
+00001ae0: 732f 6164 7269 6161 6c2f 5265 706f 7369  s/adriaal/Reposi
+00001af0: 746f 7269 6573 2f48 414d 2f74 6573 7473  tories/HAM/tests
+00001b00: 2f74 6573 745f 6d61 7070 6572 2e70 7952  /test_mapper.pyR
+00001b10: 4200 0000 3800 0000 730c 0000 0006 0209  B...8...s.......
+00001b20: 0f09 0609 0809 0609 0f74 1200 0000 5665  .........t....Ve
+00001b30: 7274 6963 616c 4d61 7070 6572 5465 7374  rticalMapperTest
+00001b40: 6300 0000 0000 0000 0001 0000 0042 0000  c............B..
+00001b50: 0073 5000 0000 6500 005a 0100 6400 0084  .sP...e..Z..d...
+00001b60: 0000 5a02 0064 0100 8400 005a 0300 6402  ..Z..d.....Z..d.
+00001b70: 0084 0000 5a04 0064 0300 8400 005a 0500  ....Z..d.....Z..
+00001b80: 6404 0084 0000 5a06 0064 0500 8400 005a  d.....Z..d.....Z
+00001b90: 0700 6406 0084 0000 5a08 0064 0700 8400  ..d.....Z..d....
+00001ba0: 005a 0900 5253 2808 0000 0063 0100 0000  .Z..RS(....c....
+00001bb0: 0300 0000 0400 0000 4300 0000 738d 0000  ........C...s...
+00001bc0: 0074 0000 7c00 006a 0100 8301 007d 0100  .t..|..j.....}..
+00001bd0: 7402 007c 0000 6a01 007c 0000 6a03 007c  t..|..j..|..j..|
+00001be0: 0000 6a04 0083 0300 7d02 007c 0000 6a05  ..j.....}..|..j.
+00001bf0: 007c 0200 6a06 0083 0100 017c 0100 6a07  .|..j......|..j.
+00001c00: 007c 0200 8301 0001 7c00 006a 0800 7c00  .|......|..j..|.
+00001c10: 006a 0400 7c01 006a 0900 8302 0001 7c00  .j..|..j......|.
+00001c20: 006a 0800 7c00 006a 0300 7c01 006a 0a00  .j..|..j..|..j..
+00001c30: 8302 0001 7c00 006a 0800 7c00 006a 0100  ....|..j..|..j..
+00001c40: 7c01 006a 0b00 8302 0001 6400 0053 2801  |..j......d..S(.
+00001c50: 0000 004e 280c 0000 0052 0400 0000 522d  ...N(....R....R-
+00001c60: 0000 0052 0200 0000 522f 0000 0052 3800  ...R....R/...R8.
+00001c70: 0000 5256 0000 0052 5700 0000 7407 0000  ..RV...RW...t...
+00001c80: 0061 6464 5f6d 6170 5258 0000 0052 5900  .add_mapRX...RY.
+00001c90: 0000 525a 0000 0074 0300 0000 4841 4d28  ..RZ...t....HAM(
+00001ca0: 0300 0000 5239 0000 0074 0c00 0000 7665  ....R9...t....ve
+00001cb0: 7274 6963 616c 5f6d 6170 525b 0000 0028  rtical_mapR[...(
+00001cc0: 0000 0000 2800 0000 0073 3400 0000 2f55  ....(....s4.../U
+00001cd0: 7365 7273 2f61 6472 6961 616c 2f52 6570  sers/adriaal/Rep
+00001ce0: 6f73 6974 6f72 6965 732f 4841 4d2f 7465  ositories/HAM/te
+00001cf0: 7374 732f 7465 7374 5f6d 6170 7065 722e  sts/test_mapper.
+00001d00: 7079 7422 0000 0074 6573 745f 6372 6561  pyt"...test_crea
+00001d10: 7465 5f63 6f72 7265 6374 6c79 5f76 6572  te_correctly_ver
+00001d20: 7469 6361 6c5f 6d61 709a 0000 0073 0e00  tical_map....s..
+00001d30: 0000 0001 0f02 1b01 1001 0d02 1601 1601  ................
+00001d40: 6301 0000 0004 0000 0006 0000 0043 0000  c............C..
+00001d50: 0073 9900 0000 7400 007c 0000 6a01 0083  .s....t..|..j...
+00001d60: 0100 7d01 0074 0200 7c00 006a 0100 7c00  ..}..t..|..j..|.
+00001d70: 006a 0300 7c00 006a 0400 8303 007d 0200  .j..|..j.....}..
+00001d80: 7c00 006a 0500 7c02 006a 0600 8301 0001  |..j..|..j......
+00001d90: 7c01 006a 0700 7c02 0083 0100 0174 0200  |..j..|......t..
+00001da0: 7c00 006a 0100 7c00 006a 0300 7c00 006a  |..j..|..j..|..j
+00001db0: 0800 8303 007d 0300 7c00 006a 0500 7c03  .....}..|..j..|.
+00001dc0: 006a 0600 8301 0001 7c00 006a 0900 740a  .j......|..j..t.
+00001dd0: 0083 0100 8f12 0001 7c01 006a 0700 7c03  ........|..j..|.
+00001de0: 0083 0100 0157 6400 0051 5864 0000 5328  .....Wd..QXd..S(
+00001df0: 0100 0000 4e28 0b00 0000 5204 0000 0052  ....N(....R....R
+00001e00: 2d00 0000 5202 0000 0052 2f00 0000 5238  -...R....R/...R8
+00001e10: 0000 0052 5600 0000 5257 0000 0052 8600  ...RV...RW...R..
+00001e20: 0000 5235 0000 0052 5d00 0000 524c 0000  ..R5...R]...RL..
+00001e30: 0028 0400 0000 5239 0000 0052 8800 0000  .(....R9...R....
+00001e40: 525b 0000 0052 5e00 0000 2800 0000 0028  R[...R^...(....(
+00001e50: 0000 0000 7334 0000 002f 5573 6572 732f  ....s4.../Users/
+00001e60: 6164 7269 6161 6c2f 5265 706f 7369 746f  adriaal/Reposito
+00001e70: 7269 6573 2f48 414d 2f74 6573 7473 2f74  ries/HAM/tests/t
+00001e80: 6573 745f 6d61 7070 6572 2e70 7974 2100  est_mapper.pyt!.
+00001e90: 0000 7465 7374 5f63 616e 6e6f 745f 6164  ..test_cannot_ad
+00001ea0: 645f 6d6f 7265 5f74 6861 6e5f 6f6e 655f  d_more_than_one_
+00001eb0: 6d61 70a5 0000 0073 1000 0000 0001 0f02  map....s........
+00001ec0: 1b01 1001 0d02 1b01 1001 1001 6301 0000  ............c...
+00001ed0: 0002 0000 0007 0000 0043 0000 0073 5900  .........C...sY.
+00001ee0: 0000 7400 007c 0000 6a01 0083 0100 7d01  ..t..|..j.....}.
+00001ef0: 007c 0000 6a02 0074 0300 8301 008f 1200  .|..j..t........
+00001f00: 017c 0100 6a04 0064 0100 8301 0001 5764  .|..j..d......Wd
+00001f10: 0000 5158 7c00 006a 0200 7403 0083 0100  ..QX|..j..t.....
+00001f20: 8f12 0001 7c01 006a 0400 6402 0083 0100  ....|..j..d.....
+00001f30: 0157 6400 0051 5864 0000 5328 0300 0000  .Wd..QXd..S(....
+00001f40: 4e74 0300 0000 3131 3174 0000 0000 2805  Nt....111t....(.
+00001f50: 0000 0052 0400 0000 522d 0000 0052 5d00  ...R....R-...R].
+00001f60: 0000 524c 0000 0052 8600 0000 2802 0000  ..RL...R....(...
+00001f70: 0052 3900 0000 5288 0000 0028 0000 0000  .R9...R....(....
+00001f80: 2800 0000 0073 3400 0000 2f55 7365 7273  (....s4.../Users
+00001f90: 2f61 6472 6961 616c 2f52 6570 6f73 6974  /adriaal/Reposit
+00001fa0: 6f72 6965 732f 4841 4d2f 7465 7374 732f  ories/HAM/tests/
+00001fb0: 7465 7374 5f6d 6170 7065 722e 7079 741f  test_mapper.pyt.
+00001fc0: 0000 0074 6573 745f 6361 6e5f 6f6e 6c79  ...test_can_only
+00001fd0: 5f61 6464 5f48 4f47 4d41 505f 6173 5f6d  _add_HOGMAP_as_m
+00001fe0: 6170 b100 0000 730a 0000 0000 010f 0210  ap....s.........
+00001ff0: 0113 0210 0163 0100 0000 0100 0000 0500  .....c..........
+00002000: 0000 4300 0000 7321 0000 007c 0000 6a00  ..C...s!...|..j.
+00002010: 0074 0100 8301 008f 0c00 0174 0200 8300  .t.........t....
+00002020: 0001 5764 0000 5158 6400 0053 2801 0000  ..Wd..QXd..S(...
+00002030: 004e 2803 0000 0052 5d00 0000 524c 0000  .N(....R]...RL..
+00002040: 0052 0400 0000 2801 0000 0052 3900 0000  .R....(....R9...
+00002050: 2800 0000 0028 0000 0000 7334 0000 002f  (....(....s4.../
+00002060: 5573 6572 732f 6164 7269 6161 6c2f 5265  Users/adriaal/Re
+00002070: 706f 7369 746f 7269 6573 2f48 414d 2f74  positories/HAM/t
+00002080: 6573 7473 2f74 6573 745f 6d61 7070 6572  ests/test_mapper
+00002090: 2e70 7974 3100 0000 7465 7374 5f63 616e  .pyt1...test_can
+000020a0: 5f6f 6e6c 795f 6372 6561 7465 5f76 6572  _only_create_ver
+000020b0: 7469 6361 6c5f 6d61 705f 7769 7468 5f68  tical_map_with_h
+000020c0: 616d 5f6f 626a 6563 74ba 0000 0073 0400  am_object....s..
+000020d0: 0000 0001 1001 6301 0000 0007 0000 0005  ......c.........
+000020e0: 0000 0043 0000 0073 e800 0000 7400 007c  ...C...s....t..|
+000020f0: 0000 6a01 0083 0100 7d01 0074 0200 7c00  ..j.....}..t..|.
+00002100: 006a 0100 7c00 006a 0300 7c00 006a 0400  .j..|..j..|..j..
+00002110: 8303 007d 0200 7c00 006a 0500 7c02 006a  ...}..|..j..|..j
+00002120: 0600 8301 0001 7c01 006a 0700 7c02 0083  ......|..j..|...
+00002130: 0100 017c 0100 6a08 0083 0000 7d03 007c  ...|..j.....}..|
+00002140: 0000 6a09 0064 0100 6701 0074 0a00 7c03  ..j..d..g..t..|.
+00002150: 0083 0100 8302 0001 7400 007c 0000 6a01  ........t..|..j.
+00002160: 0083 0100 7d04 0074 0200 7c00 006a 0100  ....}..t..|..j..
+00002170: 7c00 006a 0b00 7c00 006a 0400 8303 007d  |..j..|..j.....}
+00002180: 0500 7c00 006a 0500 7c05 006a 0600 8301  ..|..j..|..j....
+00002190: 0001 7c04 006a 0700 7c05 0083 0100 017c  ..|..j..|......|
+000021a0: 0400 6a08 0083 0000 7d06 007c 0000 6a09  ..j.....}..|..j.
+000021b0: 0064 0200 6401 0064 0300 6803 0074 0c00  .d..d..d..h..t..
+000021c0: 740a 007c 0600 8301 0083 0100 8302 0001  t..|............
+000021d0: 6400 0053 2804 0000 004e 730c 0000 003c  d..S(....Ns....<
+000021e0: 484f 4728 332e 452e 3229 3e73 0a00 0000  HOG(3.E.2)>s....
+000021f0: 3c48 4f47 2832 2e45 293e 730c 0000 003c  <HOG(2.E)>s....<
+00002200: 484f 4728 332e 452e 3129 3e28 0d00 0000  HOG(3.E.1)>(....
+00002210: 5204 0000 0052 2d00 0000 5202 0000 0052  R....R-...R....R
+00002220: 2f00 0000 5238 0000 0052 5600 0000 5257  /...R8...RV...RW
+00002230: 0000 0052 8600 0000 7408 0000 0067 6574  ...R....t....get
+00002240: 5f6c 6f73 7452 5800 0000 520a 0000 0052  _lostRX...R....R
+00002250: 3200 0000 5213 0000 0028 0700 0000 5239  2...R....(....R9
+00002260: 0000 0052 8800 0000 525b 0000 0074 0400  ...R....R[...t..
+00002270: 0000 6c6f 7373 740d 0000 0076 6572 7469  ..losst....verti
+00002280: 6361 6c5f 6d61 7032 525e 0000 0074 0500  cal_map2R^...t..
+00002290: 0000 6c6f 7373 3228 0000 0000 2800 0000  ..loss2(....(...
+000022a0: 0073 3400 0000 2f55 7365 7273 2f61 6472  .s4.../Users/adr
+000022b0: 6961 616c 2f52 6570 6f73 6974 6f72 6965  iaal/Repositorie
+000022c0: 732f 4841 4d2f 7465 7374 732f 7465 7374  s/HAM/tests/test
+000022d0: 5f6d 6170 7065 722e 7079 740d 0000 0074  _mapper.pyt....t
+000022e0: 6573 745f 6765 745f 6c6f 7374 be00 0000  est_get_lost....
+000022f0: 7318 0000 0000 010f 011b 0110 010d 020c  s...............
+00002300: 0119 020f 011b 0110 010d 020c 0163 0100  .............c..
+00002310: 0000 0400 0000 0500 0000 4300 0000 7379  ..........C...sy
+00002320: 0000 0074 0000 7c00 006a 0100 8301 007d  ...t..|..j.....}
+00002330: 0100 7402 007c 0000 6a01 007c 0000 6a03  ..t..|..j..|..j.
+00002340: 007c 0000 6a04 0083 0300 7d02 007c 0000  .|..j.....}..|..
+00002350: 6a05 007c 0200 6a06 0083 0100 017c 0100  j..|..j......|..
+00002360: 6a07 007c 0200 8301 0001 7c01 006a 0800  j..|......|..j..
+00002370: 8300 007d 0300 7c00 006a 0900 6401 0064  ...}..|..j..d..d
+00002380: 0200 6802 0074 0a00 740b 007c 0300 8301  ..h..t..t..|....
+00002390: 0083 0100 8302 0001 6400 0053 2803 0000  ........d..S(...
+000023a0: 004e 7307 0000 0047 656e 6528 3229 7307  .Ns....Gene(2)s.
+000023b0: 0000 0047 656e 6528 3529 280c 0000 0052  ...Gene(5)(....R
+000023c0: 0400 0000 522d 0000 0052 0200 0000 522f  ....R-...R....R/
+000023d0: 0000 0052 3500 0000 5256 0000 0052 5700  ...R5...RV...RW.
+000023e0: 0000 5286 0000 0074 0a00 0000 6765 745f  ..R....t....get_
+000023f0: 6761 696e 6564 5258 0000 0052 1300 0000  gainedRX...R....
+00002400: 520a 0000 0028 0400 0000 5239 0000 0052  R....(....R9...R
+00002410: 8800 0000 525b 0000 0074 0400 0000 6761  ....R[...t....ga
+00002420: 696e 2800 0000 0028 0000 0000 7334 0000  in(....(....s4..
+00002430: 002f 5573 6572 732f 6164 7269 6161 6c2f  ./Users/adriaal/
+00002440: 5265 706f 7369 746f 7269 6573 2f48 414d  Repositories/HAM
+00002450: 2f74 6573 7473 2f74 6573 745f 6d61 7070  /tests/test_mapp
+00002460: 6572 2e70 7974 0f00 0000 7465 7374 5f67  er.pyt....test_g
+00002470: 6574 5f67 6169 6e65 64cf 0000 0073 0c00  et_gained....s..
+00002480: 0000 0001 0f01 1b01 1001 0d02 0c01 6301  ..............c.
+00002490: 0000 0004 0000 0004 0000 0043 0000 0073  ...........C...s
+000024a0: 7400 0000 7400 007c 0000 6a01 0083 0100  t...t..|..j.....
+000024b0: 7d01 0074 0200 7c00 006a 0100 7c00 006a  }..t..|..j..|..j
+000024c0: 0300 7c00 006a 0400 8303 007d 0200 7c00  ..|..j.....}..|.
+000024d0: 006a 0500 7c02 006a 0600 8301 0001 7c01  .j..|..j......|.
+000024e0: 006a 0700 7c02 0083 0100 017c 0100 6a08  .j..|......|..j.
+000024f0: 0083 0000 7d03 007c 0000 6a09 0069 0100  ....}..|..j..i..
+00002500: 6401 0064 0200 3674 0a00 7c03 0083 0100  d..d..6t..|.....
+00002510: 8302 0001 6400 0053 2803 0000 004e 7307  ....d..S(....Ns.
+00002520: 0000 0047 656e 6528 3129 7308 0000 003c  ...Gene(1)s....<
+00002530: 484f 4728 3129 3e28 0b00 0000 5204 0000  HOG(1)>(....R...
+00002540: 0052 2d00 0000 5202 0000 0052 2f00 0000  .R-...R....R/...
+00002550: 5235 0000 0052 5600 0000 5257 0000 0052  R5...RV...RW...R
+00002560: 8600 0000 740c 0000 0067 6574 5f72 6574  ....t....get_ret
+00002570: 6169 6e65 6452 6a00 0000 5212 0000 0028  ainedRj...R....(
+00002580: 0400 0000 5239 0000 0052 8800 0000 525b  ....R9...R....R[
+00002590: 0000 0074 0600 0000 7369 6e67 6c65 2800  ...t....single(.
+000025a0: 0000 0028 0000 0000 7334 0000 002f 5573  ...(....s4.../Us
+000025b0: 6572 732f 6164 7269 6161 6c2f 5265 706f  ers/adriaal/Repo
+000025c0: 7369 746f 7269 6573 2f48 414d 2f74 6573  sitories/HAM/tes
+000025d0: 7473 2f74 6573 745f 6d61 7070 6572 2e70  ts/test_mapper.p
+000025e0: 7974 0f00 0000 7465 7374 5f67 6574 5f73  yt....test_get_s
+000025f0: 696e 676c 65d8 0000 0073 0c00 0000 0001  ingle....s......
+00002600: 0f01 1b01 1001 0d02 0c01 6301 0000 0004  ..........c.....
+00002610: 0000 0004 0000 0043 0000 0073 7a00 0000  .......C...sz...
+00002620: 7400 007c 0000 6a01 0083 0100 7d01 0074  t..|..j.....}..t
+00002630: 0200 7c00 006a 0100 7c00 006a 0300 7c00  ..|..j..|..j..|.
+00002640: 006a 0400 8303 007d 0200 7c00 006a 0500  .j.....}..|..j..
+00002650: 7c02 006a 0600 8301 0001 7c01 006a 0700  |..j......|..j..
+00002660: 7c02 0083 0100 017c 0100 6a08 0083 0000  |......|..j.....
+00002670: 7d03 007c 0000 6a09 0069 0100 6401 0064  }..|..j..i..d..d
+00002680: 0200 6802 0064 0300 3674 0a00 7c03 0083  ..h..d..6t..|...
+00002690: 0100 8302 0001 6400 0053 2804 0000 004e  ......d..S(....N
+000026a0: 7308 0000 0047 656e 6528 3333 2973 0800  s....Gene(33)s..
+000026b0: 0000 4765 6e65 2833 3429 7308 0000 003c  ..Gene(34)s....<
+000026c0: 484f 4728 3329 3e28 0b00 0000 5204 0000  HOG(3)>(....R...
+000026d0: 0052 2d00 0000 5202 0000 0052 3100 0000  .R-...R....R1...
+000026e0: 5235 0000 0052 5600 0000 5257 0000 0052  R5...RV...RW...R
+000026f0: 8600 0000 740e 0000 0067 6574 5f64 7570  ....t....get_dup
+00002700: 6c69 6361 7465 6452 6a00 0000 5215 0000  licatedRj...R...
+00002710: 0028 0400 0000 5239 0000 0052 8800 0000  .(....R9...R....
+00002720: 525b 0000 0074 0900 0000 6475 706c 6963  R[...t....duplic
+00002730: 6174 6528 0000 0000 2800 0000 0073 3400  ate(....(....s4.
+00002740: 0000 2f55 7365 7273 2f61 6472 6961 616c  ../Users/adriaal
+00002750: 2f52 6570 6f73 6974 6f72 6965 732f 4841  /Repositories/HA
+00002760: 4d2f 7465 7374 732f 7465 7374 5f6d 6170  M/tests/test_map
+00002770: 7065 722e 7079 7413 0000 0074 6573 745f  per.pyt....test_
+00002780: 6765 745f 6475 706c 6963 6174 6564 e100  get_duplicated..
+00002790: 0000 730c 0000 0000 010f 011b 0110 010d  ..s.............
+000027a0: 020c 0128 0a00 0000 523e 0000 0052 3f00  ...(....R>...R?.
+000027b0: 0000 5289 0000 0052 8a00 0000 528d 0000  ..R....R....R...
+000027c0: 0052 8e00 0000 5293 0000 0052 9600 0000  .R....R....R....
+000027d0: 5299 0000 0052 9c00 0000 2800 0000 0028  R....R....(....(
+000027e0: 0000 0000 2800 0000 0073 3400 0000 2f55  ....(....s4.../U
+000027f0: 7365 7273 2f61 6472 6961 616c 2f52 6570  sers/adriaal/Rep
+00002800: 6f73 6974 6f72 6965 732f 4841 4d2f 7465  ositories/HAM/te
+00002810: 7374 732f 7465 7374 5f6d 6170 7065 722e  sts/test_mapper.
+00002820: 7079 5285 0000 0099 0000 0073 1000 0000  pyR........s....
+00002830: 0601 090b 090c 0909 0904 0911 0909 0909  ................
+00002840: 7411 0000 004c 6174 6572 616c 4d61 7070  t....LateralMapp
+00002850: 6572 5465 7374 6300 0000 0000 0000 0001  erTestc.........
+00002860: 0000 0042 0000 0073 5000 0000 6500 005a  ...B...sP...e..Z
+00002870: 0100 6400 0084 0000 5a02 0064 0100 8400  ..d.....Z..d....
+00002880: 005a 0300 6402 0084 0000 5a04 0064 0300  .Z..d.....Z..d..
+00002890: 8400 005a 0500 6404 0084 0000 5a06 0064  ...Z..d.....Z..d
+000028a0: 0500 8400 005a 0700 6406 0084 0000 5a08  .....Z..d.....Z.
+000028b0: 0064 0700 8400 005a 0900 5253 2808 0000  .d.....Z..RS(...
+000028c0: 0063 0100 0000 0400 0000 0400 0000 4300  .c............C.
+000028d0: 0000 73ce 0000 0074 0000 7c00 006a 0100  ..s....t..|..j..
+000028e0: 8301 007d 0100 7402 007c 0000 6a01 007c  ...}..t..|..j..|
+000028f0: 0000 6a03 007c 0000 6a04 0083 0300 7d02  ..j..|..j.....}.
+00002900: 007c 0000 6a05 007c 0200 6a06 0083 0100  .|..j..|..j.....
+00002910: 017c 0100 6a07 007c 0200 8301 0001 7402  .|..j..|......t.
+00002920: 007c 0000 6a01 007c 0000 6a08 007c 0000  .|..j..|..j..|..
+00002930: 6a04 0083 0300 7d03 007c 0000 6a05 007c  j.....}..|..j..|
+00002940: 0300 6a06 0083 0100 017c 0100 6a07 007c  ..j......|..j..|
+00002950: 0300 8301 0001 7c00 006a 0900 7c00 006a  ......|..j..|..j
+00002960: 0400 7c01 006a 0a00 8302 0001 7c00 006a  ..|..j......|..j
+00002970: 0900 7c00 006a 0300 7c00 006a 0800 6702  ..|..j..|..j..g.
+00002980: 007c 0100 6a0b 0083 0200 017c 0000 6a09  .|..j......|..j.
+00002990: 007c 0000 6a01 007c 0100 6a0c 0083 0200  .|..j..|..j.....
+000029a0: 0164 0000 5328 0100 0000 4e28 0d00 0000  .d..S(....N(....
+000029b0: 5203 0000 0052 2d00 0000 5202 0000 0052  R....R-...R....R
+000029c0: 2f00 0000 5238 0000 0052 5600 0000 5257  /...R8...RV...RW
+000029d0: 0000 0052 8600 0000 5236 0000 0052 5800  ...R....R6...RX.
+000029e0: 0000 5259 0000 0074 0b00 0000 6465 7363  ..RY...t....desc
+000029f0: 656e 6461 6e74 7352 8700 0000 2804 0000  endantsR....(...
+00002a00: 0052 3900 0000 740b 0000 006c 6174 6572  .R9...t....later
+00002a10: 616c 5f6d 6170 525b 0000 0052 5e00 0000  al_mapR[...R^...
+00002a20: 2800 0000 0028 0000 0000 7334 0000 002f  (....(....s4.../
+00002a30: 5573 6572 732f 6164 7269 6161 6c2f 5265  Users/adriaal/Re
+00002a40: 706f 7369 746f 7269 6573 2f48 414d 2f74  positories/HAM/t
+00002a50: 6573 7473 2f74 6573 745f 6d61 7070 6572  ests/test_mapper
+00002a60: 2e70 7974 2100 0000 7465 7374 5f63 7265  .pyt!...test_cre
+00002a70: 6174 655f 636f 7272 6563 746c 795f 6c61  ate_correctly_la
+00002a80: 7465 7261 6c5f 6d61 70ed 0000 0073 1400  teral_map....s..
+00002a90: 0000 0001 0f02 1b01 1001 0d02 1b01 1001  ................
+00002aa0: 0d02 1601 1f01 6301 0000 0004 0000 0006  ......c.........
+00002ab0: 0000 0043 0000 0073 9900 0000 7400 007c  ...C...s....t..|
+00002ac0: 0000 6a01 0083 0100 7d01 0074 0200 7c00  ..j.....}..t..|.
+00002ad0: 006a 0100 7c00 006a 0300 7c00 006a 0400  .j..|..j..|..j..
+00002ae0: 8303 007d 0200 7c00 006a 0500 7c02 006a  ...}..|..j..|..j
+00002af0: 0600 8301 0001 7c01 006a 0700 7c02 0083  ......|..j..|...
+00002b00: 0100 0174 0200 7c00 006a 0100 7c00 006a  ...t..|..j..|..j
+00002b10: 0300 7c00 006a 0800 8303 007d 0300 7c00  ..|..j.....}..|.
+00002b20: 006a 0500 7c03 006a 0600 8301 0001 7c00  .j..|..j......|.
+00002b30: 006a 0900 740a 0083 0100 8f12 0001 7c01  .j..t.........|.
+00002b40: 006a 0700 7c03 0083 0100 0157 6400 0051  .j..|......Wd..Q
+00002b50: 5864 0000 5328 0100 0000 4e28 0b00 0000  Xd..S(....N(....
+00002b60: 5203 0000 0052 2d00 0000 5202 0000 0052  R....R-...R....R
+00002b70: 2f00 0000 5238 0000 0052 5600 0000 5257  /...R8...RV...RW
+00002b80: 0000 0052 8600 0000 5235 0000 0052 5d00  ...R....R5...R].
+00002b90: 0000 524c 0000 0028 0400 0000 5239 0000  ..RL...(....R9..
+00002ba0: 0052 9f00 0000 525b 0000 0052 5e00 0000  .R....R[...R^...
+00002bb0: 2800 0000 0028 0000 0000 7334 0000 002f  (....(....s4.../
+00002bc0: 5573 6572 732f 6164 7269 6161 6c2f 5265  Users/adriaal/Re
+00002bd0: 706f 7369 746f 7269 6573 2f48 414d 2f74  positories/HAM/t
+00002be0: 6573 7473 2f74 6573 745f 6d61 7070 6572  ests/test_mapper
+00002bf0: 2e70 7974 2b00 0000 7465 7374 5f63 616e  .pyt+...test_can
+00002c00: 6e6f 745f 6164 645f 6d61 705f 7769 7468  not_add_map_with
+00002c10: 5f64 6966 6665 7265 6e74 5f61 6e63 6573  _different_ances
+00002c20: 746f 72fc 0000 0073 1000 0000 0001 0f02  tor....s........
+00002c30: 1b01 1001 0d02 1b01 1001 1001 6301 0000  ............c...
+00002c40: 0002 0000 0007 0000 0043 0000 0073 5900  .........C...sY.
+00002c50: 0000 7400 007c 0000 6a01 0083 0100 7d01  ..t..|..j.....}.
+00002c60: 007c 0000 6a02 0074 0300 8301 008f 1200  .|..j..t........
+00002c70: 017c 0100 6a04 0064 0100 8301 0001 5764  .|..j..d......Wd
+00002c80: 0000 5158 7c00 006a 0200 7403 0083 0100  ..QX|..j..t.....
+00002c90: 8f12 0001 7c01 006a 0400 6402 0083 0100  ....|..j..d.....
+00002ca0: 0157 6400 0051 5864 0000 5328 0300 0000  .Wd..QXd..S(....
+00002cb0: 4e52 8b00 0000 528c 0000 0028 0500 0000  NR....R....(....
+00002cc0: 5203 0000 0052 2d00 0000 525d 0000 0052  R....R-...R]...R
+00002cd0: 4c00 0000 5286 0000 0028 0200 0000 5239  L...R....(....R9
+00002ce0: 0000 0052 9f00 0000 2800 0000 0028 0000  ...R....(....(..
+00002cf0: 0000 7334 0000 002f 5573 6572 732f 6164  ..s4.../Users/ad
+00002d00: 7269 6161 6c2f 5265 706f 7369 746f 7269  riaal/Repositori
+00002d10: 6573 2f48 414d 2f74 6573 7473 2f74 6573  es/HAM/tests/tes
+00002d20: 745f 6d61 7070 6572 2e70 7952 8d00 0000  t_mapper.pyR....
+00002d30: 0801 0000 730a 0000 0000 010f 0210 0113  ....s...........
+00002d40: 0210 0163 0100 0000 0200 0000 0500 0000  ...c............
+00002d50: 4300 0000 7323 0000 007c 0000 6a00 0074  C...s#...|..j..t
+00002d60: 0100 8301 008f 0e00 0174 0200 8300 007d  .........t.....}
+00002d70: 0100 5764 0000 5158 6400 0053 2801 0000  ..Wd..QXd..S(...
+00002d80: 004e 2803 0000 0052 5d00 0000 524c 0000  .N(....R]...RL..
+00002d90: 0052 0300 0000 2802 0000 0052 3900 0000  .R....(....R9...
+00002da0: 529f 0000 0028 0000 0000 2800 0000 0073  R....(....(....s
+00002db0: 3400 0000 2f55 7365 7273 2f61 6472 6961  4.../Users/adria
+00002dc0: 616c 2f52 6570 6f73 6974 6f72 6965 732f  al/Repositories/
+00002dd0: 4841 4d2f 7465 7374 732f 7465 7374 5f6d  HAM/tests/test_m
+00002de0: 6170 7065 722e 7079 528e 0000 0011 0100  apper.pyR.......
+00002df0: 0073 0400 0000 0001 1001 6301 0000 000a  .s........c.....
+00002e00: 0000 0005 0000 0043 0000 0073 cf01 0000  .......C...s....
+00002e10: 7400 007c 0000 6a01 0083 0100 7d01 0074  t..|..j.....}..t
+00002e20: 0200 7c00 006a 0100 7c00 006a 0300 7c00  ..|..j..|..j..|.
+00002e30: 006a 0400 8303 007d 0200 7c00 006a 0500  .j.....}..|..j..
+00002e40: 7c02 006a 0600 8301 0001 7c01 006a 0700  |..j......|..j..
+00002e50: 7c02 0083 0100 0174 0200 7c00 006a 0100  |......t..|..j..
+00002e60: 7c00 006a 0800 7c00 006a 0400 8303 007d  |..j..|..j.....}
+00002e70: 0300 7c00 006a 0500 7c03 006a 0600 8301  ..|..j..|..j....
+00002e80: 0001 7c01 006a 0700 7c03 0083 0100 017c  ..|..j..|......|
+00002e90: 0100 6a09 0083 0000 7d04 0078 6500 7c04  ..j.....}..xe.|.
+00002ea0: 006a 0a00 8300 0044 5d57 007d 0500 740b  .j.....D]W.}..t.
+00002eb0: 007c 0500 8301 0064 0100 6b02 0072 b900  .|.....d..k..r..
+00002ec0: 7c05 007d 0600 7198 0074 0b00 7c05 0083  |..}..q..t..|...
+00002ed0: 0100 6402 006b 0200 72d4 007c 0500 7d07  ..d..k..r..|..}.
+00002ee0: 0071 9800 740b 007c 0500 8301 0064 0300  .q..t..|.....d..
+00002ef0: 6b02 0072 9800 7c05 007d 0800 7198 0071  k..r..|..}..q..q
+00002f00: 9800 577c 0000 6a0c 007c 0000 6a08 0068  ..W|..j..|..j..h
+00002f10: 0100 740d 007c 0400 7c08 0019 8301 0083  ..t..|..|.......
+00002f20: 0200 017c 0000 6a0c 007c 0000 6a08 0068  ...|..j..|..j..h
+00002f30: 0100 740d 007c 0400 7c07 0019 8301 0083  ..t..|..|.......
+00002f40: 0200 017c 0000 6a0c 007c 0000 6a08 007c  ...|..j..|..j..|
+00002f50: 0000 6a03 0068 0200 740d 007c 0400 7c06  ..j..h..t..|..|.
+00002f60: 0019 8301 0083 0200 017c 0100 6a09 0083  .........|..j...
+00002f70: 0000 7d09 007c 0000 6a0c 007c 0000 6a08  ..}..|..j..|..j.
+00002f80: 0068 0100 740d 007c 0900 7c08 0019 8301  .h..t..|..|.....
+00002f90: 0083 0200 017c 0000 6a0c 007c 0000 6a08  .....|..j..|..j.
+00002fa0: 0068 0100 740d 007c 0900 7c07 0019 8301  .h..t..|..|.....
+00002fb0: 0083 0200 017c 0000 6a0c 007c 0000 6a08  .....|..j..|..j.
+00002fc0: 007c 0000 6a03 0068 0200 740d 007c 0900  .|..j..h..t..|..
+00002fd0: 7c06 0019 8301 0083 0200 0164 0000 5328  |..........d..S(
+00002fe0: 0400 0000 4e73 0c00 0000 3c48 4f47 2833  ....Ns....<HOG(3
+00002ff0: 2e45 2e32 293e 730c 0000 003c 484f 4728  .E.2)>s....<HOG(
+00003000: 332e 452e 3129 3e73 0a00 0000 3c48 4f47  3.E.1)>s....<HOG
+00003010: 2832 2e45 293e 280e 0000 0052 0300 0000  (2.E)>(....R....
+00003020: 522d 0000 0052 0200 0000 522f 0000 0052  R-...R....R/...R
+00003030: 3800 0000 5256 0000 0052 5700 0000 5286  8...RV...RW...R.
+00003040: 0000 0052 3200 0000 528f 0000 0052 0b00  ...R2...R....R..
+00003050: 0000 5206 0000 0052 5800 0000 5213 0000  ..R....RX...R...
+00003060: 0028 0a00 0000 5239 0000 0052 9f00 0000  .(....R9...R....
+00003070: 740f 0000 006d 6170 5f68 756d 616e 5f65  t....map_human_e
+00003080: 7561 7263 740d 0000 006d 6170 5f72 6174  uarct....map_rat
+00003090: 5f65 7561 7263 5290 0000 0052 5200 0000  _euarcR....RR...
+000030a0: 7406 0000 0048 335f 455f 3274 0600 0000  t....H3_E_2t....
+000030b0: 4833 5f45 5f31 7404 0000 0048 325f 4552  H3_E_1t....H2_ER
+000030c0: 9200 0000 2800 0000 0028 0000 0000 7334  ....(....(....s4
+000030d0: 0000 002f 5573 6572 732f 6164 7269 6161  .../Users/adriaa
+000030e0: 6c2f 5265 706f 7369 746f 7269 6573 2f48  l/Repositories/H
+000030f0: 414d 2f74 6573 7473 2f74 6573 745f 6d61  AM/tests/test_ma
+00003100: 7070 6572 2e70 7952 9300 0000 1501 0000  pper.pyR........
+00003110: 732c 0000 0000 010f 021b 0110 010d 021b  s,..............
+00003120: 0110 010d 020c 0213 0112 0109 0112 0109  ................
+00003130: 0112 010d 0220 0120 0126 030c 0120 0120  ..... . .&... . 
+00003140: 0163 0100 0000 0500 0000 0600 0000 4300  .c............C.
+00003150: 0000 73de 0000 0074 0000 7c00 006a 0100  ..s....t..|..j..
+00003160: 8301 007d 0100 7402 007c 0000 6a01 007c  ...}..t..|..j..|
+00003170: 0000 6a03 007c 0000 6a04 0083 0300 7d02  ..j..|..j.....}.
+00003180: 007c 0000 6a05 007c 0200 6a06 0083 0100  .|..j..|..j.....
+00003190: 017c 0100 6a07 007c 0200 8301 0001 7402  .|..j..|......t.
+000031a0: 007c 0000 6a01 007c 0000 6a08 007c 0000  .|..j..|..j..|..
+000031b0: 6a04 0083 0300 7d03 007c 0000 6a05 007c  j.....}..|..j..|
+000031c0: 0300 6a06 0083 0100 017c 0100 6a07 007c  ..j......|..j..|
+000031d0: 0300 8301 0001 7c01 006a 0900 8300 007d  ......|..j.....}
+000031e0: 0400 7c00 006a 0a00 740b 0083 0000 740b  ..|..j..t.....t.
+000031f0: 0074 0c00 7c04 007c 0000 6a03 0019 8301  .t..|..|..j.....
+00003200: 0083 0100 8302 0001 7c00 006a 0a00 6401  ........|..j..d.
+00003210: 0064 0200 6802 0074 0b00 740c 007c 0400  .d..h..t..t..|..
+00003220: 7c00 006a 0800 1983 0100 8301 0083 0200  |..j............
+00003230: 0164 0000 5328 0300 0000 4e73 0700 0000  .d..S(....Ns....
+00003240: 4765 6e65 2832 2973 0700 0000 4765 6e65  Gene(2)s....Gene
+00003250: 2835 2928 0d00 0000 5203 0000 0052 2d00  (5)(....R....R-.
+00003260: 0000 5202 0000 0052 3000 0000 5235 0000  ..R....R0...R5..
+00003270: 0052 5600 0000 5257 0000 0052 8600 0000  .RV...RW...R....
+00003280: 522f 0000 0052 9400 0000 5258 0000 0052  R/...R....RX...R
+00003290: 1300 0000 520a 0000 0028 0500 0000 5239  ....R....(....R9
+000032a0: 0000 0052 9f00 0000 7413 0000 006d 6170  ...R....t....map
+000032b0: 5f66 726f 675f 7665 7274 6562 7261 7465  _frog_vertebrate
+000032c0: 52a2 0000 0052 9500 0000 2800 0000 0028  R....R....(....(
+000032d0: 0000 0000 7334 0000 002f 5573 6572 732f  ....s4.../Users/
+000032e0: 6164 7269 6161 6c2f 5265 706f 7369 746f  adriaal/Reposito
+000032f0: 7269 6573 2f48 414d 2f74 6573 7473 2f74  ries/HAM/tests/t
+00003300: 6573 745f 6d61 7070 6572 2e70 7952 9600  est_mapper.pyR..
+00003310: 0000 3401 0000 7314 0000 0000 020f 021b  ..4...s.........
+00003320: 0110 010d 021b 0110 010d 020c 0126 0163  .............&.c
+00003330: 0100 0000 0900 0000 0500 0000 4300 0000  ............C...
+00003340: 7385 0100 0074 0000 7c00 006a 0100 8301  s....t..|..j....
+00003350: 007d 0100 7402 007c 0000 6a01 007c 0000  .}..t..|..j..|..
+00003360: 6a03 007c 0000 6a04 0083 0300 7d02 007c  j..|..j.....}..|
+00003370: 0000 6a05 007c 0200 6a06 0083 0100 017c  ..j..|..j......|
+00003380: 0100 6a07 007c 0200 8301 0001 7402 007c  ..j..|......t..|
+00003390: 0000 6a01 007c 0000 6a08 007c 0000 6a04  ..j..|..j..|..j.
+000033a0: 0083 0300 7d03 007c 0000 6a05 007c 0300  ....}..|..j..|..
+000033b0: 6a06 0083 0100 017c 0100 6a07 007c 0300  j......|..j..|..
+000033c0: 8301 0001 7c01 006a 0900 8300 007d 0400  ....|..j.....}..
+000033d0: 7865 007c 0400 6a0a 0083 0000 445d 5700  xe.|..j.....D]W.
+000033e0: 7d05 0074 0b00 7c05 0083 0100 6401 006b  }..t..|.....d..k
+000033f0: 0200 72b9 007c 0500 7d06 0071 9800 740b  ..r..|..}..q..t.
+00003400: 007c 0500 8301 0064 0200 6b02 0072 d400  .|.....d..k..r..
+00003410: 7c05 007d 0700 7198 0074 0b00 7c05 0083  |..}..q..t..|...
+00003420: 0100 6403 006b 0200 7298 007c 0500 7d08  ..d..k..r..|..}.
+00003430: 0071 9800 7198 0057 7c00 006a 0c00 6901  .q..q..W|..j..i.
+00003440: 0064 0400 740b 007c 0000 6a03 0083 0100  .d..t..|..j.....
+00003450: 3674 0d00 7c04 007c 0600 1983 0100 8302  6t..|..|........
+00003460: 0001 7c00 006a 0c00 6902 0064 0500 740b  ..|..j..i..d..t.
+00003470: 007c 0000 6a03 0083 0100 3664 0600 740b  .|..j.....6d..t.
+00003480: 007c 0000 6a08 0083 0100 3674 0d00 7c04  .|..j.....6t..|.
+00003490: 007c 0700 1983 0100 8302 0001 7c00 006a  .|..........|..j
+000034a0: 0c00 6901 0064 0700 740b 007c 0000 6a03  ..i..d..t..|..j.
+000034b0: 0083 0100 3674 0d00 7c04 007c 0800 1983  ....6t..|..|....
+000034c0: 0100 8302 0001 6400 0053 2808 0000 004e  ......d..S(....N
+000034d0: 730c 0000 003c 484f 4728 332e 452e 3129  s....<HOG(3.E.1)
+000034e0: 3e73 0c00 0000 3c48 4f47 2831 2e4d 2e45  >s....<HOG(1.M.E
+000034f0: 293e 730a 0000 003c 484f 4728 322e 4529  )>s....<HOG(2.E)
+00003500: 3e73 0700 0000 4765 6e65 2833 2973 0700  >s....Gene(3)s..
+00003510: 0000 4765 6e65 2831 2973 0800 0000 4765  ..Gene(1)s....Ge
+00003520: 6e65 2834 3129 7307 0000 0047 656e 6528  ne(41)s....Gene(
+00003530: 3229 280e 0000 0052 0300 0000 522d 0000  2)(....R....R-..
+00003540: 0052 0200 0000 522f 0000 0052 3800 0000  .R....R/...R8...
+00003550: 5256 0000 0052 5700 0000 5286 0000 0052  RV...RW...R....R
+00003560: 3200 0000 5297 0000 0052 0b00 0000 5206  2...R....R....R.
+00003570: 0000 0052 6a00 0000 5212 0000 0028 0900  ...Rj...R....(..
+00003580: 0000 5239 0000 0052 9f00 0000 52a2 0000  ..R9...R....R...
+00003590: 0052 a300 0000 5298 0000 0052 5200 0000  .R....R....RR...
+000035a0: 52a5 0000 0074 0600 0000 4831 5f4d 5f45  R....t....H1_M_E
+000035b0: 52a6 0000 0028 0000 0000 2800 0000 0073  R....(....(....s
+000035c0: 3400 0000 2f55 7365 7273 2f61 6472 6961  4.../Users/adria
+000035d0: 616c 2f52 6570 6f73 6974 6f72 6965 732f  al/Repositories/
+000035e0: 4841 4d2f 7465 7374 732f 7465 7374 5f6d  HAM/tests/test_m
+000035f0: 6170 7065 722e 7079 5299 0000 0044 0100  apper.pyR....D..
+00003600: 0073 2400 0000 0001 0f02 1b01 1001 0d02  .s$.............
+00003610: 1b01 1001 0d02 0c02 1301 1201 0901 1201  ................
+00003620: 0901 1201 0d02 2a01 3a01 6301 0000 0007  ......*.:.c.....
+00003630: 0000 0005 0000 0043 0000 0073 0401 0000  .......C...s....
+00003640: 7400 007c 0000 6a01 0083 0100 7d01 0074  t..|..j.....}..t
+00003650: 0200 7c00 006a 0100 7c00 006a 0300 7c00  ..|..j..|..j..|.
+00003660: 006a 0400 8303 007d 0200 7c00 006a 0500  .j.....}..|..j..
+00003670: 7c02 006a 0600 8301 0001 7c01 006a 0700  |..j......|..j..
+00003680: 7c02 0083 0100 0174 0200 7c00 006a 0100  |......t..|..j..
+00003690: 7c00 006a 0800 7c00 006a 0400 8303 007d  |..j..|..j.....}
+000036a0: 0300 7c00 006a 0500 7c03 006a 0600 8301  ..|..j..|..j....
+000036b0: 0001 7c01 006a 0700 7c03 0083 0100 017c  ..|..j..|......|
+000036c0: 0100 6a09 0083 0000 7d04 0078 2f00 7c04  ..j.....}..x/.|.
+000036d0: 006a 0a00 8300 0044 5d21 007d 0500 740b  .j.....D]!.}..t.
+000036e0: 007c 0500 8301 0064 0100 6b02 0072 9800  .|.....d..k..r..
+000036f0: 7c05 007d 0600 7198 0071 9800 577c 0000  |..}..q..q..W|..
+00003700: 6a0c 0069 0200 6402 0068 0100 740b 007c  j..i..d..h..t..|
+00003710: 0000 6a03 0083 0100 3664 0300 6404 0068  ..j.....6d..d..h
+00003720: 0200 740b 007c 0000 6a08 0083 0100 3674  ..t..|..j.....6t
+00003730: 0d00 7c04 007c 0600 1983 0100 8302 0001  ..|..|..........
+00003740: 6400 0053 2805 0000 004e 7308 0000 003c  d..S(....Ns....<
+00003750: 484f 4728 3329 3e73 0700 0000 4765 6e65  HOG(3)>s....Gene
+00003760: 2833 2973 0800 0000 4765 6e65 2833 3329  (3)s....Gene(33)
+00003770: 7308 0000 0047 656e 6528 3334 2928 0e00  s....Gene(34)(..
+00003780: 0000 5203 0000 0052 2d00 0000 5202 0000  ..R....R-...R...
+00003790: 0052 2f00 0000 5235 0000 0052 5600 0000  .R/...R5...RV...
+000037a0: 5257 0000 0052 8600 0000 5231 0000 0052  RW...R....R1...R
+000037b0: 9a00 0000 520b 0000 0052 0600 0000 526a  ....R....R....Rj
+000037c0: 0000 0052 1500 0000 2807 0000 0052 3900  ...R....(....R9.
+000037d0: 0000 529f 0000 0074 0e00 0000 6d61 705f  ..R....t....map_
+000037e0: 6875 6d61 6e5f 7665 7274 740e 0000 006d  human_vertt....m
+000037f0: 6170 5f6d 6f75 7365 5f76 6572 7452 9b00  ap_mouse_vertR..
+00003800: 0000 5252 0000 0074 0100 0000 4828 0000  ..RR...t....H(..
+00003810: 0000 2800 0000 0073 3400 0000 2f55 7365  ..(....s4.../Use
+00003820: 7273 2f61 6472 6961 616c 2f52 6570 6f73  rs/adriaal/Repos
+00003830: 6974 6f72 6965 732f 4841 4d2f 7465 7374  itories/HAM/test
+00003840: 732f 7465 7374 5f6d 6170 7065 722e 7079  s/test_mapper.py
+00003850: 529c 0000 005d 0100 0073 1800 0000 0001  R....]...s......
+00003860: 0f02 1b01 1001 0d02 1b01 1001 0d02 0c02  ................
+00003870: 1301 1201 0d02 280a 0000 0052 3e00 0000  ......(....R>...
+00003880: 523f 0000 0052 a000 0000 52a1 0000 0052  R?...R....R....R
+00003890: 8d00 0000 528e 0000 0052 9300 0000 5296  ....R....R....R.
+000038a0: 0000 0052 9900 0000 529c 0000 0028 0000  ...R....R....(..
+000038b0: 0000 2800 0000 0028 0000 0000 7334 0000  ..(....(....s4..
+000038c0: 002f 5573 6572 732f 6164 7269 6161 6c2f  ./Users/adriaal/
+000038d0: 5265 706f 7369 746f 7269 6573 2f48 414d  Repositories/HAM
+000038e0: 2f74 6573 7473 2f74 6573 745f 6d61 7070  /tests/test_mapp
+000038f0: 6572 2e70 7952 9d00 0000 eb00 0000 7310  er.pyR........s.
+00003900: 0000 0006 0209 0f09 0c09 0909 0409 1f09  ................
+00003910: 1009 1974 0800 0000 5f5f 6d61 696e 5f5f  ...t....__main__
+00003920: 2800 0000 0028 1200 0000 5240 0000 0074  (....(....R@...t
+00003930: 0500 0000 7079 6861 6d52 0000 0000 5201  ....pyhamR....R.
+00003940: 0000 0052 0200 0000 5203 0000 0052 0400  ...R....R....R..
+00003950: 0000 5225 0000 0052 0a00 0000 5212 0000  ..R%...R....R...
+00003960: 0052 1500 0000 5216 0000 0052 1700 0000  .R....R....R....
+00003970: 5242 0000 0052 8500 0000 529d 0000 0052  RB...R....R....R
+00003980: 3e00 0000 7404 0000 006d 6169 6e28 0000  >...t....main(..
+00003990: 0000 2800 0000 0028 0000 0000 7334 0000  ..(....(....s4..
+000039a0: 002f 5573 6572 732f 6164 7269 6161 6c2f  ./Users/adriaal/
+000039b0: 5265 706f 7369 746f 7269 6573 2f48 414d  Repositories/HAM
+000039c0: 2f74 6573 7473 2f74 6573 745f 6d61 7070  /tests/test_mapp
+000039d0: 6572 2e70 7974 0800 0000 3c6d 6f64 756c  er.pyt....<modul
+000039e0: 653e 0100 0000 731a 0000 000c 0110 0110  e>....s.........
+000039f0: 011c 010c 0209 0709 0809 0b13 1719 6119  ..............a.
+00003a00: 5219 850c 01                             R....
```

### Comparing `pyham-1.1.8/tests/data/simpleEx_complexParalogs.orthoxml` & `pyham-1.1.9/tests/data/simpleEx_complexParalogs.orthoxml`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/tests/data/SimpleEx_complexParalogGetHOGS3format.xml` & `pyham-1.1.9/tests/data/SimpleEx_complexParalogGetHOGS3format.xml`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/tests/data/simpleExNoCladeName.phyloxml` & `pyham-1.1.9/tests/data/simpleExNoCladeName.phyloxml`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/tests/data/simpleEx.phyloxml` & `pyham-1.1.9/tests/data/simpleEx.phyloxml`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/tests/data/simpleExNoName.phyloxml` & `pyham-1.1.9/tests/data/simpleExNoName.phyloxml`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/tests/data/hogvisEx.orthoxml` & `pyham-1.1.9/tests/data/hogvisEx.orthoxml`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/tests/data/simpleEx.orthoxml` & `pyham-1.1.9/tests/data/simpleEx.orthoxml`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/tests/test_iham.pyc` & `pyham-1.1.9/tests/test_iham.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 2.7 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 03f3 0d0a 6e8c e85e 6300 0000 0000 0000  ....n..^c.......
+00000000: 03f3 0d0a 0bc8 8f5b 6300 0000 0000 0000  .......[c.......
 00000010: 0003 0000 0040 0000 0073 5100 0000 6400  .....@...sQ...d.
 00000020: 0064 0100 6c00 005a 0000 6400 0064 0200  .d..l..Z..d..d..
 00000030: 6c01 006d 0200 5a02 006d 0300 5a03 006d  l..m..Z..m..Z..m
 00000040: 0400 5a04 0001 6400 0064 0100 6c05 005a  ..Z...d..d..l..Z
 00000050: 0500 6403 0065 0000 6a06 0066 0100 6404  ..d..e..j..f..d.
 00000060: 0084 0000 8300 0059 5a07 0064 0100 5328  .......YZ..d..S(
 00000070: 0500 0000 69ff ffff ff4e 2803 0000 0074  ....i....N(....t
@@ -38,51 +38,47 @@
 00000250: 0067 6574 5f6e 6577 6963 6b5f 7374 7269  .get_newick_stri
 00000260: 6e67 5200 0000 0074 0300 0000 4861 6d74  ngR....t....Hamt
 00000270: 0400 0000 5472 7565 740c 0000 0068 616d  ....Truet....ham
 00000280: 5f61 6e61 6c79 7369 7328 0400 0000 7404  _analysis(....t.
 00000290: 0000 0073 656c 6674 0800 0000 6e77 6b5f  ...selft....nwk_
 000002a0: 7061 7468 7408 0000 0074 7265 655f 7374  patht....tree_st
 000002b0: 7274 0d00 0000 6f72 7468 6f78 6d6c 5f70  rt....orthoxml_p
-000002c0: 6174 6828 0000 0000 2800 0000 0073 4500  ath(....(....sE.
-000002d0: 0000 2f55 7365 7273 2f61 646d 696e 2f57  ../Users/admin/W
-000002e0: 6f72 6b2f 7072 6f6a 6563 742f 4465 7373  ork/project/Dess
-000002f0: 696d 6f7a 2f70 7968 616d 2d64 6576 2f70  imoz/pyham-dev/p
-00000300: 7968 616d 2f74 6573 7473 2f74 6573 745f  yham/tests/test_
-00000310: 6968 616d 2e70 7974 0500 0000 7365 7455  iham.pyt....setU
-00000320: 7007 0000 0073 0a00 0000 0002 2101 1501  p....s......!...
-00000330: 2102 1b01 6301 0000 0002 0000 0003 0000  !...c...........
-00000340: 0043 0000 0073 2900 0000 7c00 006a 0000  .C...s)...|..j..
-00000350: 6a01 0064 0100 8301 007d 0100 7c00 006a  j..d.....}..|..j
-00000360: 0000 6a02 0064 0200 7c01 0083 0001 0164  ..j..d..|......d
-00000370: 0000 5328 0300 0000 4e69 0100 0000 7403  ..S(....Ni....t.
-00000380: 0000 0068 6f67 2803 0000 0052 1300 0000  ...hog(....R....
-00000390: 740d 0000 0067 6574 5f68 6f67 5f62 795f  t....get_hog_by_
-000003a0: 6964 740b 0000 0063 7265 6174 655f 6948  idt....create_iH
-000003b0: 616d 2802 0000 0052 1400 0000 7405 0000  am(....R....t...
-000003c0: 0068 6f67 5f33 2800 0000 0028 0000 0000  .hog_3(....(....
-000003d0: 7345 0000 002f 5573 6572 732f 6164 6d69  sE.../Users/admi
-000003e0: 6e2f 576f 726b 2f70 726f 6a65 6374 2f44  n/Work/project/D
-000003f0: 6573 7369 6d6f 7a2f 7079 6861 6d2d 6465  essimoz/pyham-de
-00000400: 762f 7079 6861 6d2f 7465 7374 732f 7465  v/pyham/tests/te
-00000410: 7374 5f69 6861 6d2e 7079 7407 0000 0074  st_iham.pyt....t
-00000420: 6573 745f 6f6b 1000 0000 7304 0000 0000  est_ok....s.....
-00000430: 0212 0128 0400 0000 7408 0000 005f 5f6e  ...(....t....__n
-00000440: 616d 655f 5f74 0a00 0000 5f5f 6d6f 6475  ame__t....__modu
-00000450: 6c65 5f5f 5218 0000 0052 1d00 0000 2800  le__R....R....(.
-00000460: 0000 0028 0000 0000 2800 0000 0073 4500  ...(....(....sE.
-00000470: 0000 2f55 7365 7273 2f61 646d 696e 2f57  ../Users/admin/W
-00000480: 6f72 6b2f 7072 6f6a 6563 742f 4465 7373  ork/project/Dess
-00000490: 696d 6f7a 2f70 7968 616d 2d64 6576 2f70  imoz/pyham-dev/p
-000004a0: 7968 616d 2f74 6573 7473 2f74 6573 745f  yham/tests/test_
-000004b0: 6968 616d 2e70 7952 0300 0000 0500 0000  iham.pyR........
-000004c0: 7304 0000 0006 0209 0928 0800 0000 7408  s........(....t.
-000004d0: 0000 0075 6e69 7474 6573 7474 0500 0000  ...unittestt....
-000004e0: 7079 6861 6d52 0000 0000 5201 0000 0052  pyhamR....R....R
-000004f0: 0200 0000 520b 0000 0074 0800 0000 5465  ....R....t....Te
-00000500: 7374 4361 7365 5203 0000 0028 0000 0000  stCaseR....(....
-00000510: 2800 0000 0028 0000 0000 7345 0000 002f  (....(....sE.../
-00000520: 5573 6572 732f 6164 6d69 6e2f 576f 726b  Users/admin/Work
-00000530: 2f70 726f 6a65 6374 2f44 6573 7369 6d6f  /project/Dessimo
-00000540: 7a2f 7079 6861 6d2d 6465 762f 7079 6861  z/pyham-dev/pyha
-00000550: 6d2f 7465 7374 732f 7465 7374 5f69 6861  m/tests/test_iha
-00000560: 6d2e 7079 7408 0000 003c 6d6f 6475 6c65  m.pyt....<module
-00000570: 3e01 0000 0073 0600 0000 0c01 1c01 0c02  >....s..........
+000002c0: 6174 6828 0000 0000 2800 0000 0073 3200  ath(....(....s2.
+000002d0: 0000 2f55 7365 7273 2f61 6472 6961 616c  ../Users/adriaal
+000002e0: 2f52 6570 6f73 6974 6f72 6965 732f 4841  /Repositories/HA
+000002f0: 4d2f 7465 7374 732f 7465 7374 5f69 6861  M/tests/test_iha
+00000300: 6d2e 7079 7405 0000 0073 6574 5570 0700  m.pyt....setUp..
+00000310: 0000 730a 0000 0000 0221 0115 0121 021b  ..s......!...!..
+00000320: 0163 0100 0000 0200 0000 0300 0000 4300  .c............C.
+00000330: 0000 7329 0000 007c 0000 6a00 006a 0100  ..s)...|..j..j..
+00000340: 6401 0083 0100 7d01 007c 0000 6a00 006a  d.....}..|..j..j
+00000350: 0200 6402 007c 0100 8300 0101 6400 0053  ..d..|......d..S
+00000360: 2803 0000 004e 6901 0000 0074 0300 0000  (....Ni....t....
+00000370: 686f 6728 0300 0000 5213 0000 0074 0d00  hog(....R....t..
+00000380: 0000 6765 745f 686f 675f 6279 5f69 6474  ..get_hog_by_idt
+00000390: 0b00 0000 6372 6561 7465 5f69 4861 6d28  ....create_iHam(
+000003a0: 0200 0000 5214 0000 0074 0500 0000 686f  ....R....t....ho
+000003b0: 675f 3328 0000 0000 2800 0000 0073 3200  g_3(....(....s2.
+000003c0: 0000 2f55 7365 7273 2f61 6472 6961 616c  ../Users/adriaal
+000003d0: 2f52 6570 6f73 6974 6f72 6965 732f 4841  /Repositories/HA
+000003e0: 4d2f 7465 7374 732f 7465 7374 5f69 6861  M/tests/test_iha
+000003f0: 6d2e 7079 7407 0000 0074 6573 745f 6f6b  m.pyt....test_ok
+00000400: 1000 0000 7304 0000 0000 0212 0128 0400  ....s........(..
+00000410: 0000 7408 0000 005f 5f6e 616d 655f 5f74  ..t....__name__t
+00000420: 0a00 0000 5f5f 6d6f 6475 6c65 5f5f 5218  ....__module__R.
+00000430: 0000 0052 1d00 0000 2800 0000 0028 0000  ...R....(....(..
+00000440: 0000 2800 0000 0073 3200 0000 2f55 7365  ..(....s2.../Use
+00000450: 7273 2f61 6472 6961 616c 2f52 6570 6f73  rs/adriaal/Repos
+00000460: 6974 6f72 6965 732f 4841 4d2f 7465 7374  itories/HAM/test
+00000470: 732f 7465 7374 5f69 6861 6d2e 7079 5203  s/test_iham.pyR.
+00000480: 0000 0005 0000 0073 0400 0000 0602 0909  .......s........
+00000490: 2808 0000 0074 0800 0000 756e 6974 7465  (....t....unitte
+000004a0: 7374 7405 0000 0070 7968 616d 5200 0000  stt....pyhamR...
+000004b0: 0052 0100 0000 5202 0000 0052 0b00 0000  .R....R....R....
+000004c0: 7408 0000 0054 6573 7443 6173 6552 0300  t....TestCaseR..
+000004d0: 0000 2800 0000 0028 0000 0000 2800 0000  ..(....(....(...
+000004e0: 0073 3200 0000 2f55 7365 7273 2f61 6472  .s2.../Users/adr
+000004f0: 6961 616c 2f52 6570 6f73 6974 6f72 6965  iaal/Repositorie
+00000500: 732f 4841 4d2f 7465 7374 732f 7465 7374  s/HAM/tests/test
+00000510: 5f69 6861 6d2e 7079 7408 0000 003c 6d6f  _iham.pyt....<mo
+00000520: 6475 6c65 3e01 0000 0073 0600 0000 0c01  dule>....s......
+00000530: 1c01 0c02                                ....
```

### Comparing `pyham-1.1.8/tests/test_genome.pyc` & `pyham-1.1.9/tests/test_genome.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 2.7 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 03f3 0d0a 6e8c e85e 6300 0000 0000 0000  ....n..^c.......
+00000000: 03f3 0d0a de42 755b 6300 0000 0000 0000  .....Bu[c.......
 00000010: 0003 0000 0040 0000 0073 ae00 0000 6400  .....@...s....d.
 00000020: 005a 0000 6401 0064 0200 6c01 005a 0100  .Z..d..d..l..Z..
 00000030: 6401 0064 0300 6c02 006d 0300 5a03 006d  d..d..l..m..Z..m
 00000040: 0400 5a04 006d 0500 5a05 006d 0600 5a06  ..Z..m..Z..m..Z.
 00000050: 0001 6401 0064 0400 6c01 006d 0700 5a07  ..d..d..l..m..Z.
 00000060: 0001 6401 0064 0200 6c08 006a 0900 5a0a  ..d..d..l..j..Z.
 00000070: 0064 0100 6402 006c 0b00 5a0b 0064 0500  .d..d..l..Z..d..
@@ -40,106 +40,100 @@
 00000270: 0900 0000 5479 7065 4572 726f 7274 0100  ....TypeErrort..
 00000280: 0000 6774 0c00 0000 4578 7461 6e74 4765  ..gt....ExtantGe
 00000290: 6e6f 6d65 740b 0000 0061 7373 6572 7445  nomet....assertE
 000002a0: 7175 616c 7405 0000 0074 6178 6964 7410  qualt....taxidt.
 000002b0: 0000 0061 7373 6572 7449 7349 6e73 7461  ...assertIsInsta
 000002c0: 6e63 6528 0400 0000 7404 0000 0073 656c  nce(....t....sel
 000002d0: 6674 0100 0000 6174 0100 0000 6274 0100  ft....at....bt..
-000002e0: 0000 6328 0000 0000 2800 0000 0073 4700  ..c(....(....sG.
-000002f0: 0000 2f55 7365 7273 2f61 646d 696e 2f57  ../Users/admin/W
-00000300: 6f72 6b2f 7072 6f6a 6563 742f 4465 7373  ork/project/Dess
-00000310: 696d 6f7a 2f70 7968 616d 2d64 6576 2f70  imoz/pyham-dev/p
-00000320: 7968 616d 2f74 6573 7473 2f74 6573 745f  yham/tests/test_
-00000330: 6765 6e6f 6d65 2e70 7974 2000 0000 7465  genome.pyt ...te
-00000340: 7374 5f6e 616d 655f 616e 645f 4e43 4249  st_name_and_NCBI
-00000350: 5461 7849 645f 7265 7175 6972 6564 0c00  TaxId_required..
-00000360: 0000 730e 0000 0000 0310 0112 0312 0113  ..s.............
-00000370: 0310 0118 0328 0300 0000 7408 0000 005f  .....(....t...._
-00000380: 5f6e 616d 655f 5f74 0a00 0000 5f5f 6d6f  _name__t....__mo
-00000390: 6475 6c65 5f5f 5216 0000 0028 0000 0000  dule__R....(....
-000003a0: 2800 0000 0028 0000 0000 7347 0000 002f  (....(....sG.../
-000003b0: 5573 6572 732f 6164 6d69 6e2f 576f 726b  Users/admin/Work
-000003c0: 2f70 726f 6a65 6374 2f44 6573 7369 6d6f  /project/Dessimo
-000003d0: 7a2f 7079 6861 6d2d 6465 762f 7079 6861  z/pyham-dev/pyha
-000003e0: 6d2f 7465 7374 732f 7465 7374 5f67 656e  m/tests/test_gen
-000003f0: 6f6d 652e 7079 5206 0000 000a 0000 0073  ome.pyR........s
-00000400: 0200 0000 0602 740a 0000 0047 656e 6f6d  ......t....Genom
-00000410: 6554 6573 7463 0000 0000 0000 0000 0100  eTestc..........
-00000420: 0000 4200 0000 7311 0000 0065 0000 5a01  ..B...s....e..Z.
-00000430: 0064 0000 8400 005a 0200 5253 2801 0000  .d.....Z..RS(...
-00000440: 0063 0100 0000 0600 0000 0900 0000 4300  .c............C.
-00000450: 0000 7345 0100 0074 0000 6a01 0064 0100  ..sE...t..j..d..
-00000460: 6402 0064 0300 6404 0083 0002 7d01 0074  d..d..d.....}..t
-00000470: 0000 6a02 0083 0000 7d02 0074 0300 6405  ..j.....}..t..d.
-00000480: 0064 0600 8300 017d 0300 7c00 006a 0400  .d.....}..|..j..
-00000490: 7405 0083 0100 8f12 0001 7c01 006a 0600  t.........|..j..
-000004a0: 7c03 0083 0100 0157 6400 0051 587c 0000  |......Wd..QX|..
-000004b0: 6a04 0074 0500 8301 008f 1200 017c 0200  j..t.........|..
-000004c0: 6a06 007c 0300 8301 0001 5764 0000 5158  j..|......Wd..QX
-000004d0: 7407 006a 0800 6407 0064 0800 6409 0083  t..j..d..d..d...
-000004e0: 0101 7d04 007c 0100 6a06 007c 0400 6a09  ..}..|..j..|..j.
-000004f0: 0083 0000 8301 0001 7c02 006a 0600 7c04  ........|..j..|.
-00000500: 006a 0900 8300 0083 0100 0174 0700 6a08  .j.........t..j.
-00000510: 0064 0a00 6408 0064 0900 8301 017d 0500  .d..d..d.....}..
-00000520: 7c00 006a 0400 740a 0083 0100 8f18 0001  |..j..t.........
-00000530: 7c01 006a 0600 7c05 006a 0900 8300 0083  |..j..|..j......
-00000540: 0100 0157 6400 0051 587c 0000 6a04 0074  ...Wd..QX|..j..t
-00000550: 0a00 8301 008f 1800 017c 0200 6a06 007c  .........|..j..|
-00000560: 0500 6a09 0083 0000 8301 0001 5764 0000  ..j.........Wd..
-00000570: 5158 7c01 006a 0600 7c04 006a 0900 8300  QX|..j..|..j....
-00000580: 0083 0100 017c 0200 6a06 007c 0400 6a09  .....|..j..|..j.
-00000590: 0083 0000 8301 0001 6400 0053 280b 0000  ........d..S(...
-000005a0: 004e 5207 0000 0052 0800 0000 5209 0000  .NR....R....R...
-000005b0: 0052 0a00 0000 7402 0000 0069 6474 0300  .R....t....idt..
-000005c0: 0000 3432 3373 3600 0000 2841 3a31 2c28  ..423s6...(A:1,(
-000005d0: 423a 312c 2845 3a31 2c44 3a31 2949 6e74  B:1,(E:1,D:1)Int
-000005e0: 6572 6e61 6c5f 313a 302e 3529 496e 7465  ernal_1:0.5)Inte
-000005f0: 726e 616c 5f32 3a30 2e35 2952 6f6f 743b  rnal_2:0.5)Root;
-00000600: 7406 0000 0066 6f72 6d61 7469 0100 0000  t....formati....
-00000610: 7312 0000 0028 453a 312c 443a 3129 496e  s....(E:1,D:1)In
-00000620: 7465 726e 616c 3b28 0b00 0000 520d 0000  ternal;(....R...
-00000630: 0052 0e00 0000 740f 0000 0041 6e63 6573  .R....t....Ances
-00000640: 7472 616c 4765 6e6f 6d65 5201 0000 0052  tralGenomeR....R
-00000650: 0b00 0000 520c 0000 0074 0900 0000 7365  ....R....t....se
-00000660: 745f 7461 786f 6e74 0400 0000 6574 6533  t_taxont....ete3
-00000670: 7404 0000 0054 7265 6574 0d00 0000 6765  t....Treet....ge
-00000680: 745f 7472 6565 5f72 6f6f 7452 0400 0000  t_tree_rootR....
-00000690: 2806 0000 0052 1200 0000 7402 0000 0061  (....R....t....a
-000006a0: 3174 0200 0000 6132 5214 0000 0052 1500  1t....a2R....R..
-000006b0: 0000 7401 0000 0064 2800 0000 0028 0000  ..t....d(....(..
-000006c0: 0000 7347 0000 002f 5573 6572 732f 6164  ..sG.../Users/ad
-000006d0: 6d69 6e2f 576f 726b 2f70 726f 6a65 6374  min/Work/project
-000006e0: 2f44 6573 7369 6d6f 7a2f 7079 6861 6d2d  /Dessimoz/pyham-
-000006f0: 6465 762f 7079 6861 6d2f 7465 7374 732f  dev/pyham/tests/
-00000700: 7465 7374 5f67 656e 6f6d 652e 7079 7427  test_genome.pyt'
-00000710: 0000 0074 6573 745f 6361 6e6e 6f74 5f61  ...test_cannot_a
-00000720: 6464 5f61 6e79 7468 696e 675f 6173 5f74  dd_anything_as_t
-00000730: 6178 6f6e 5f72 616e 6765 2000 0000 7322  axon_range ...s"
-00000740: 0000 0000 0118 010c 010f 0310 0113 0110  ................
-00000750: 0113 0315 0113 0113 0315 0110 0119 0110  ................
-00000760: 0119 0313 0128 0300 0000 5217 0000 0052  .....(....R....R
-00000770: 1800 0000 5225 0000 0028 0000 0000 2800  ....R%...(....(.
-00000780: 0000 0028 0000 0000 7347 0000 002f 5573  ...(....sG.../Us
-00000790: 6572 732f 6164 6d69 6e2f 576f 726b 2f70  ers/admin/Work/p
-000007a0: 726f 6a65 6374 2f44 6573 7369 6d6f 7a2f  roject/Dessimoz/
-000007b0: 7079 6861 6d2d 6465 762f 7079 6861 6d2f  pyham-dev/pyham/
-000007c0: 7465 7374 732f 7465 7374 5f67 656e 6f6d  tests/test_genom
-000007d0: 652e 7079 5219 0000 001e 0000 0073 0200  e.pyR........s..
-000007e0: 0000 0602 7408 0000 005f 5f6d 6169 6e5f  ....t....__main_
-000007f0: 5f28 1100 0000 740a 0000 005f 5f61 7574  _(....t....__aut
-00000800: 686f 725f 5f74 0800 0000 756e 6974 7465  hor__t....unitte
-00000810: 7374 7405 0000 0070 7968 616d 5201 0000  stt....pyhamR...
-00000820: 0052 0200 0000 5203 0000 0052 0400 0000  .R....R....R....
-00000830: 5205 0000 0074 0c00 0000 7079 6861 6d2e  R....t....pyham.
-00000840: 6765 6e6f 6d65 7406 0000 0067 656e 6f6d  genomet....genom
-00000850: 6552 0d00 0000 521f 0000 0074 0800 0000  eR....R....t....
-00000860: 5465 7374 4361 7365 5206 0000 0052 1900  TestCaseR....R..
-00000870: 0000 5217 0000 0074 0400 0000 6d61 696e  ..R....t....main
-00000880: 2800 0000 0028 0000 0000 2800 0000 0073  (....(....(....s
-00000890: 4700 0000 2f55 7365 7273 2f61 646d 696e  G.../Users/admin
-000008a0: 2f57 6f72 6b2f 7072 6f6a 6563 742f 4465  /Work/project/De
-000008b0: 7373 696d 6f7a 2f70 7968 616d 2d64 6576  ssimoz/pyham-dev
-000008c0: 2f70 7968 616d 2f74 6573 7473 2f74 6573  /pyham/tests/tes
-000008d0: 745f 6765 6e6f 6d65 2e70 7974 0800 0000  t_genome.pyt....
-000008e0: 3c6d 6f64 756c 653e 0100 0000 7312 0000  <module>....s...
-000008f0: 0006 020c 0122 0110 010f 010c 0319 1419  ....."..........
-00000900: 1e0c 01                                  ...
+000002e0: 0000 6328 0000 0000 2800 0000 0073 3400  ..c(....(....s4.
+000002f0: 0000 2f55 7365 7273 2f61 6472 6961 616c  ../Users/adriaal
+00000300: 2f52 6570 6f73 6974 6f72 6965 732f 4841  /Repositories/HA
+00000310: 4d2f 7465 7374 732f 7465 7374 5f67 656e  M/tests/test_gen
+00000320: 6f6d 652e 7079 7420 0000 0074 6573 745f  ome.pyt ...test_
+00000330: 6e61 6d65 5f61 6e64 5f4e 4342 4954 6178  name_and_NCBITax
+00000340: 4964 5f72 6571 7569 7265 640c 0000 0073  Id_required....s
+00000350: 0e00 0000 0003 1001 1203 1201 1303 1001  ................
+00000360: 1803 2803 0000 0074 0800 0000 5f5f 6e61  ..(....t....__na
+00000370: 6d65 5f5f 740a 0000 005f 5f6d 6f64 756c  me__t....__modul
+00000380: 655f 5f52 1600 0000 2800 0000 0028 0000  e__R....(....(..
+00000390: 0000 2800 0000 0073 3400 0000 2f55 7365  ..(....s4.../Use
+000003a0: 7273 2f61 6472 6961 616c 2f52 6570 6f73  rs/adriaal/Repos
+000003b0: 6974 6f72 6965 732f 4841 4d2f 7465 7374  itories/HAM/test
+000003c0: 732f 7465 7374 5f67 656e 6f6d 652e 7079  s/test_genome.py
+000003d0: 5206 0000 000a 0000 0073 0200 0000 0602  R........s......
+000003e0: 740a 0000 0047 656e 6f6d 6554 6573 7463  t....GenomeTestc
+000003f0: 0000 0000 0000 0000 0100 0000 4200 0000  ............B...
+00000400: 7311 0000 0065 0000 5a01 0064 0000 8400  s....e..Z..d....
+00000410: 005a 0200 5253 2801 0000 0063 0100 0000  .Z..RS(....c....
+00000420: 0600 0000 0900 0000 4300 0000 7345 0100  ........C...sE..
+00000430: 0074 0000 6a01 0064 0100 6402 0064 0300  .t..j..d..d..d..
+00000440: 6404 0083 0002 7d01 0074 0000 6a02 0083  d.....}..t..j...
+00000450: 0000 7d02 0074 0300 6405 0064 0600 8300  ..}..t..d..d....
+00000460: 017d 0300 7c00 006a 0400 7405 0083 0100  .}..|..j..t.....
+00000470: 8f12 0001 7c01 006a 0600 7c03 0083 0100  ....|..j..|.....
+00000480: 0157 6400 0051 587c 0000 6a04 0074 0500  .Wd..QX|..j..t..
+00000490: 8301 008f 1200 017c 0200 6a06 007c 0300  .......|..j..|..
+000004a0: 8301 0001 5764 0000 5158 7407 006a 0800  ....Wd..QXt..j..
+000004b0: 6407 0064 0800 6409 0083 0101 7d04 007c  d..d..d.....}..|
+000004c0: 0100 6a06 007c 0400 6a09 0083 0000 8301  ..j..|..j.......
+000004d0: 0001 7c02 006a 0600 7c04 006a 0900 8300  ..|..j..|..j....
+000004e0: 0083 0100 0174 0700 6a08 0064 0a00 6408  .....t..j..d..d.
+000004f0: 0064 0900 8301 017d 0500 7c00 006a 0400  .d.....}..|..j..
+00000500: 740a 0083 0100 8f18 0001 7c01 006a 0600  t.........|..j..
+00000510: 7c05 006a 0900 8300 0083 0100 0157 6400  |..j.........Wd.
+00000520: 0051 587c 0000 6a04 0074 0a00 8301 008f  .QX|..j..t......
+00000530: 1800 017c 0200 6a06 007c 0500 6a09 0083  ...|..j..|..j...
+00000540: 0000 8301 0001 5764 0000 5158 7c01 006a  ......Wd..QX|..j
+00000550: 0600 7c04 006a 0900 8300 0083 0100 017c  ..|..j.........|
+00000560: 0200 6a06 007c 0400 6a09 0083 0000 8301  ..j..|..j.......
+00000570: 0001 6400 0053 280b 0000 004e 5207 0000  ..d..S(....NR...
+00000580: 0052 0800 0000 5209 0000 0052 0a00 0000  .R....R....R....
+00000590: 7402 0000 0069 6474 0300 0000 3432 3373  t....idt....423s
+000005a0: 3600 0000 2841 3a31 2c28 423a 312c 2845  6...(A:1,(B:1,(E
+000005b0: 3a31 2c44 3a31 2949 6e74 6572 6e61 6c5f  :1,D:1)Internal_
+000005c0: 313a 302e 3529 496e 7465 726e 616c 5f32  1:0.5)Internal_2
+000005d0: 3a30 2e35 2952 6f6f 743b 7406 0000 0066  :0.5)Root;t....f
+000005e0: 6f72 6d61 7469 0100 0000 7312 0000 0028  ormati....s....(
+000005f0: 453a 312c 443a 3129 496e 7465 726e 616c  E:1,D:1)Internal
+00000600: 3b28 0b00 0000 520d 0000 0052 0e00 0000  ;(....R....R....
+00000610: 740f 0000 0041 6e63 6573 7472 616c 4765  t....AncestralGe
+00000620: 6e6f 6d65 5201 0000 0052 0b00 0000 520c  nomeR....R....R.
+00000630: 0000 0074 0900 0000 7365 745f 7461 786f  ...t....set_taxo
+00000640: 6e74 0400 0000 6574 6533 7404 0000 0054  nt....ete3t....T
+00000650: 7265 6574 0d00 0000 6765 745f 7472 6565  reet....get_tree
+00000660: 5f72 6f6f 7452 0400 0000 2806 0000 0052  _rootR....(....R
+00000670: 1200 0000 7402 0000 0061 3174 0200 0000  ....t....a1t....
+00000680: 6132 5214 0000 0052 1500 0000 7401 0000  a2R....R....t...
+00000690: 0064 2800 0000 0028 0000 0000 7334 0000  .d(....(....s4..
+000006a0: 002f 5573 6572 732f 6164 7269 6161 6c2f  ./Users/adriaal/
+000006b0: 5265 706f 7369 746f 7269 6573 2f48 414d  Repositories/HAM
+000006c0: 2f74 6573 7473 2f74 6573 745f 6765 6e6f  /tests/test_geno
+000006d0: 6d65 2e70 7974 2700 0000 7465 7374 5f63  me.pyt'...test_c
+000006e0: 616e 6e6f 745f 6164 645f 616e 7974 6869  annot_add_anythi
+000006f0: 6e67 5f61 735f 7461 786f 6e5f 7261 6e67  ng_as_taxon_rang
+00000700: 6520 0000 0073 2200 0000 0001 1801 0c01  e ...s".........
+00000710: 0f03 1001 1301 1001 1303 1501 1301 1303  ................
+00000720: 1501 1001 1901 1001 1903 1301 2803 0000  ............(...
+00000730: 0052 1700 0000 5218 0000 0052 2500 0000  .R....R....R%...
+00000740: 2800 0000 0028 0000 0000 2800 0000 0073  (....(....(....s
+00000750: 3400 0000 2f55 7365 7273 2f61 6472 6961  4.../Users/adria
+00000760: 616c 2f52 6570 6f73 6974 6f72 6965 732f  al/Repositories/
+00000770: 4841 4d2f 7465 7374 732f 7465 7374 5f67  HAM/tests/test_g
+00000780: 656e 6f6d 652e 7079 5219 0000 001e 0000  enome.pyR.......
+00000790: 0073 0200 0000 0602 7408 0000 005f 5f6d  .s......t....__m
+000007a0: 6169 6e5f 5f28 1100 0000 740a 0000 005f  ain__(....t...._
+000007b0: 5f61 7574 686f 725f 5f74 0800 0000 756e  _author__t....un
+000007c0: 6974 7465 7374 7405 0000 0070 7968 616d  ittestt....pyham
+000007d0: 5201 0000 0052 0200 0000 5203 0000 0052  R....R....R....R
+000007e0: 0400 0000 5205 0000 0074 0c00 0000 7079  ....R....t....py
+000007f0: 6861 6d2e 6765 6e6f 6d65 7406 0000 0067  ham.genomet....g
+00000800: 656e 6f6d 6552 0d00 0000 521f 0000 0074  enomeR....R....t
+00000810: 0800 0000 5465 7374 4361 7365 5206 0000  ....TestCaseR...
+00000820: 0052 1900 0000 5217 0000 0074 0400 0000  .R....R....t....
+00000830: 6d61 696e 2800 0000 0028 0000 0000 2800  main(....(....(.
+00000840: 0000 0073 3400 0000 2f55 7365 7273 2f61  ...s4.../Users/a
+00000850: 6472 6961 616c 2f52 6570 6f73 6974 6f72  driaal/Repositor
+00000860: 6965 732f 4841 4d2f 7465 7374 732f 7465  ies/HAM/tests/te
+00000870: 7374 5f67 656e 6f6d 652e 7079 7408 0000  st_genome.pyt...
+00000880: 003c 6d6f 6475 6c65 3e01 0000 0073 1200  .<module>....s..
+00000890: 0000 0602 0c01 2201 1001 0f01 0c03 1914  ......".........
+000008a0: 191e 0c01                                ....
```

### Comparing `pyham-1.1.8/tests/test_ham.pyc` & `pyham-1.1.9/tests/test_ham.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 2.7 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 03f3 0d0a 6e8c e85e 6300 0000 0000 0000  ....n..^c.......
+00000000: 03f3 0d0a a2fc a15b 6300 0000 0000 0000  .......[c.......
 00000010: 0003 0000 0040 0000 0073 d700 0000 6400  .....@...s....d.
 00000020: 0064 0100 6c00 005a 0000 6400 0064 0200  .d..l..Z..d..d..
 00000030: 6c01 006d 0200 5a02 0001 6400 0064 0300  l..m..Z...d..d..
 00000040: 6c01 006d 0300 5a03 0001 6400 0064 0100  l..m..Z...d..d..
 00000050: 6c04 005a 0400 6400 0064 0100 6c05 005a  l..Z..d..d..l..Z
 00000060: 0500 6404 0084 0000 5a06 0064 0500 8400  ..d.....Z..d....
 00000070: 005a 0700 6406 0065 0000 6a08 0066 0100  .Z..d..e..j..f..
@@ -24,1155 +24,1115 @@
 00000170: 1c00 5c02 007d 0200 7d03 0074 0200 7c03  ..\..}..}..t..|.
 00000180: 0083 0100 7c00 007c 0200 3c71 3d00 577c  ....|..|..<q=.W|
 00000190: 0000 5328 0100 0000 4e28 0400 0000 7404  ..S(....N(....t.
 000001a0: 0000 006b 6579 7374 0300 0000 706f 7074  ...keyst....popt
 000001b0: 0300 0000 7374 7274 0500 0000 6974 656d  ....strt....item
 000001c0: 7328 0400 0000 7404 0000 0064 6963 7474  s(....t....dictt
 000001d0: 0200 0000 6b6b 7401 0000 006b 7401 0000  ....kkt....kt...
-000001e0: 0076 2800 0000 0028 0000 0000 7344 0000  .v(....(....sD..
-000001f0: 002f 5573 6572 732f 6164 6d69 6e2f 576f  ./Users/admin/Wo
-00000200: 726b 2f70 726f 6a65 6374 2f44 6573 7369  rk/project/Dessi
-00000210: 6d6f 7a2f 7079 6861 6d2d 6465 762f 7079  moz/pyham-dev/py
-00000220: 6861 6d2f 7465 7374 732f 7465 7374 5f68  ham/tests/test_h
-00000230: 616d 2e70 7974 1300 0000 5f73 7472 5f64  am.pyt...._str_d
-00000240: 6963 745f 6f6e 655f 7661 6c75 6508 0000  ict_one_value...
-00000250: 0073 0a00 0000 0001 1301 1d01 1901 1401  .s..............
-00000260: 6301 0000 0003 0000 0004 0000 0043 0000  c............C..
-00000270: 0073 3400 0000 6700 007d 0100 7821 007c  .s4...g..}..x!.|
-00000280: 0000 445d 1900 7d02 007c 0100 6a00 0074  ..D]..}..|..j..t
-00000290: 0100 7c02 0083 0100 8301 0001 710d 0057  ..|.........q..W
-000002a0: 7402 007c 0100 8301 0053 2801 0000 004e  t..|.....S(....N
-000002b0: 2803 0000 0074 0600 0000 6170 7065 6e64  (....t....append
-000002c0: 5204 0000 0074 0300 0000 7365 7428 0300  R....t....set(..
-000002d0: 0000 7405 0000 0061 7272 6179 740f 0000  ..t....arrayt...
-000002e0: 0061 7272 6179 5f63 6f6e 7665 7274 6564  .array_converted
-000002f0: 7401 0000 0065 2800 0000 0028 0000 0000  t....e(....(....
-00000300: 7344 0000 002f 5573 6572 732f 6164 6d69  sD.../Users/admi
-00000310: 6e2f 576f 726b 2f70 726f 6a65 6374 2f44  n/Work/project/D
-00000320: 6573 7369 6d6f 7a2f 7079 6861 6d2d 6465  essimoz/pyham-de
-00000330: 762f 7079 6861 6d2f 7465 7374 732f 7465  v/pyham/tests/te
-00000340: 7374 5f68 616d 2e70 7974 0a00 0000 5f73  st_ham.pyt...._s
-00000350: 7472 5f61 7272 6179 0e00 0000 7308 0000  tr_array....s...
-00000360: 0000 0106 010d 0117 0174 0c00 0000 4841  .........t....HA
-00000370: 4d54 6573 7453 6574 5570 6300 0000 0000  MTestSetUpc.....
-00000380: 0000 0001 0000 0042 0000 0073 4700 0000  .......B...sG...
-00000390: 6500 005a 0100 6400 0084 0000 5a02 0064  e..Z..d.....Z..d
-000003a0: 0100 8400 005a 0300 6402 0084 0000 5a04  .....Z..d.....Z.
-000003b0: 0064 0300 8400 005a 0500 6404 0084 0000  .d.....Z..d.....
-000003c0: 5a06 0064 0500 8400 005a 0700 6406 0084  Z..d.....Z..d...
-000003d0: 0000 5a08 0052 5328 0700 0000 6301 0000  ..Z..RS(....c...
-000003e0: 0004 0000 0006 0000 0043 0000 0073 c700  .........C...s..
-000003f0: 0000 6401 007c 0000 5f00 0064 0200 7c00  ..d..|.._..d..|.
-00000400: 005f 0100 7402 006a 0300 6a04 0074 0200  ._..t..j..j..t..
-00000410: 6a03 006a 0500 7406 0083 0100 6403 0083  j..j..t.....d...
-00000420: 0200 7d01 0074 0700 6a08 007c 0100 6404  ..}..t..j..|..d.
-00000430: 0064 0500 8301 017c 0000 5f09 0074 0200  .d.....|.._..t..
-00000440: 6a03 006a 0400 7402 006a 0300 6a05 0074  j..j..t..j..j..t
-00000450: 0600 8301 0064 0600 8302 007c 0000 5f0a  .....d.....|.._.
-00000460: 0074 0200 6a03 006a 0400 7402 006a 0300  .t..j..j..t..j..
-00000470: 6a05 0074 0600 8301 0064 0700 8302 007c  j..t.....d.....|
-00000480: 0000 5f0b 0074 0c00 7c00 006a 0b00 6408  .._..t..|..j..d.
-00000490: 0083 0200 8f1c 007d 0200 7c02 006a 0d00  .......}..|..j..
-000004a0: 8300 007d 0300 7c03 007c 0000 5f0e 0057  ...}..|..|.._..W
-000004b0: 6400 0051 5864 0000 5328 0900 0000 4e74  d..QXd..S(....Nt
-000004c0: 0000 0000 7309 0000 0028 412c 4229 7830  ....s....(A,B)x0
-000004d0: 2e34 7313 0000 002e 2f64 6174 612f 7369  .4s...../data/si
-000004e0: 6d70 6c65 4578 2e6e 776b 7404 0000 0074  mpleEx.nwkt....t
-000004f0: 7970 6574 0300 0000 6e77 6b73 1800 0000  ypet....nwks....
-00000500: 2e2f 6461 7461 2f73 696d 706c 6545 782e  ./data/simpleEx.
-00000510: 7068 796c 6f78 6d6c 7318 0000 002e 2f64  phyloxmls...../d
-00000520: 6174 612f 7369 6d70 6c65 4578 2e6f 7274  ata/simpleEx.ort
-00000530: 686f 786d 6c74 0100 0000 7228 0f00 0000  hoxmlt....r(....
-00000540: 740d 0000 006e 776b 5f73 7472 5f65 6d70  t....nwk_str_emp
-00000550: 7479 740d 0000 006e 776b 5f73 7472 5f77  tyt....nwk_str_w
-00000560: 726f 6e67 7402 0000 006f 7374 0400 0000  rongt....ost....
-00000570: 7061 7468 7404 0000 006a 6f69 6e74 0700  patht....joint..
-00000580: 0000 6469 726e 616d 6574 0800 0000 5f5f  ..dirnamet....__
-00000590: 6669 6c65 5f5f 5200 0000 0074 1100 0000  file__R....t....
-000005a0: 6765 745f 6e65 7769 636b 5f73 7472 696e  get_newick_strin
-000005b0: 6774 0700 0000 6e77 6b5f 7374 7274 0d00  gt....nwk_strt..
-000005c0: 0000 7068 796c 6f78 6d6c 5f66 696c 6574  ..phyloxml_filet
-000005d0: 0d00 0000 6f72 7468 6f78 6d6c 5f70 6174  ....orthoxml_pat
-000005e0: 6874 0400 0000 6f70 656e 7404 0000 0072  ht....opent....r
-000005f0: 6561 6474 0f00 0000 6f72 7468 6f78 6d6c  eadt....orthoxml
-00000600: 5f73 7472 696e 6728 0400 0000 7404 0000  _string(....t...
-00000610: 0073 656c 6674 0800 0000 6e77 6b5f 7061  .selft....nwk_pa
-00000620: 7468 740d 0000 006f 7274 686f 786d 6c5f  tht....orthoxml_
-00000630: 6669 6c65 7404 0000 0064 6174 6128 0000  filet....data(..
-00000640: 0000 2800 0000 0073 4400 0000 2f55 7365  ..(....sD.../Use
-00000650: 7273 2f61 646d 696e 2f57 6f72 6b2f 7072  rs/admin/Work/pr
-00000660: 6f6a 6563 742f 4465 7373 696d 6f7a 2f70  oject/Dessimoz/p
-00000670: 7968 616d 2d64 6576 2f70 7968 616d 2f74  yham-dev/pyham/t
-00000680: 6573 7473 2f74 6573 745f 6861 6d2e 7079  ests/test_ham.py
-00000690: 7405 0000 0073 6574 5570 1700 0000 7312  t....setUp....s.
-000006a0: 0000 0000 0109 0109 0121 0118 0224 0224  .........!...$.$
-000006b0: 0215 010c 0163 0100 0000 0100 0000 0800  .....c..........
-000006c0: 0000 4300 0000 7350 0000 007c 0000 6a00  ..C...sP...|..j.
-000006d0: 0074 0100 8301 008f 1500 0174 0200 6a03  .t.........t..j.
-000006e0: 0064 0100 6402 0083 0001 0157 6400 0051  .d..d......Wd..Q
-000006f0: 587c 0000 6a00 0074 0100 8301 008f 1500  X|..j..t........
-00000700: 0174 0200 6a03 0064 0100 6403 0083 0001  .t..j..d..d.....
-00000710: 0157 6400 0051 5864 0000 5328 0400 0000  .Wd..QXd..S(....
-00000720: 4e74 0d00 0000 7573 655f 6461 7461 5f66  Nt....use_data_f
-00000730: 726f 6d74 0300 0000 7878 7874 0300 0000  romt....xxxt....
-00000740: 6f6d 6128 0400 0000 740c 0000 0061 7373  oma(....t....ass
-00000750: 6572 7452 6169 7365 7374 0900 0000 5479  ertRaisest....Ty
-00000760: 7065 4572 726f 7252 0100 0000 7403 0000  peErrorR....t...
-00000770: 0048 616d 2801 0000 0052 2400 0000 2800  .Ham(....R$...(.
-00000780: 0000 0028 0000 0000 7344 0000 002f 5573  ...(....sD.../Us
-00000790: 6572 732f 6164 6d69 6e2f 576f 726b 2f70  ers/admin/Work/p
-000007a0: 726f 6a65 6374 2f44 6573 7369 6d6f 7a2f  roject/Dessimoz/
-000007b0: 7079 6861 6d2d 6465 762f 7079 6861 6d2f  pyham-dev/pyham/
-000007c0: 7465 7374 732f 7465 7374 5f68 616d 2e70  tests/test_ham.p
-000007d0: 7974 1500 0000 7465 7374 5f6c 6f61 645f  yt....test_load_
-000007e0: 6672 6f6d 5f73 6572 7665 7225 0000 0073  from_server%...s
-000007f0: 0800 0000 0003 1001 1603 1001 6301 0000  ............c...
-00000800: 0001 0000 000a 0000 0043 0000 0073 7a00  .........C...sz.
-00000810: 0000 7c00 006a 0000 7401 006a 0200 6a03  ..|..j..t..j..j.
-00000820: 006a 0400 8301 008f 2100 0174 0500 6a06  .j......!..t..j.
-00000830: 007c 0000 6a07 007c 0000 6a08 0064 0100  .|..j..|..j..d..
-00000840: 6402 0083 0201 0157 6400 0051 587c 0000  d......Wd..QX|..
-00000850: 6a00 0074 0100 6a02 006a 0300 6a04 0083  j..t..j..j..j...
-00000860: 0100 8f21 0001 7405 006a 0600 7c00 006a  ...!..t..j..|..j
-00000870: 0900 7c00 006a 0800 6401 0064 0200 8302  ..|..j..d..d....
-00000880: 0101 5764 0000 5158 6400 0053 2803 0000  ..Wd..QXd..S(...
-00000890: 004e 740d 0000 0074 7970 655f 686f 675f  .Nt....type_hog_
-000008a0: 6669 6c65 7408 0000 006f 7274 686f 786d  filet....orthoxm
-000008b0: 6c28 0a00 0000 522c 0000 0074 0400 0000  l(....R,...t....
-000008c0: 6574 6533 7406 0000 0070 6172 7365 7274  ete3t....parsert
-000008d0: 0600 0000 6e65 7769 636b 740b 0000 004e  ....newickt....N
-000008e0: 6577 6963 6b45 7272 6f72 5201 0000 0052  ewickErrorR....R
-000008f0: 2e00 0000 5216 0000 0052 2000 0000 5217  ....R....R ...R.
-00000900: 0000 0028 0100 0000 5224 0000 0028 0000  ...(....R$...(..
-00000910: 0000 2800 0000 0073 4400 0000 2f55 7365  ..(....sD.../Use
-00000920: 7273 2f61 646d 696e 2f57 6f72 6b2f 7072  rs/admin/Work/pr
-00000930: 6f6a 6563 742f 4465 7373 696d 6f7a 2f70  oject/Dessimoz/p
-00000940: 7968 616d 2d64 6576 2f70 7968 616d 2f74  yham-dev/pyham/t
-00000950: 6573 7473 2f74 6573 745f 6861 6d2e 7079  ests/test_ham.py
-00000960: 7415 0000 0074 6573 745f 7772 6f6e 675f  t....test_wrong_
-00000970: 6e65 7769 636b 5f73 7472 3b00 0000 7308  newick_str;...s.
-00000980: 0000 0000 0219 0122 0219 0163 0100 0000  ......."...c....
-00000990: 0100 0000 0d00 0000 4300 0000 736a 0000  ........C...sj..
-000009a0: 007c 0000 6a00 0074 0100 8301 008f 2d00  .|..j..t......-.
-000009b0: 0174 0200 6a03 007c 0000 6a04 007c 0000  .t..j..|..j..|..
-000009c0: 6a05 0064 0100 6402 0064 0300 6404 0064  j..d..d..d..d..d
-000009d0: 0500 6406 0083 0203 0157 6400 0051 5874  ..d......Wd..QXt
-000009e0: 0200 6a03 007c 0000 6a04 007c 0000 6a05  ..j..|..j..|..j.
-000009f0: 0064 0100 6402 0064 0300 6404 0064 0500  .d..d..d..d..d..
-00000a00: 6407 0083 0203 0164 0000 5328 0800 0000  d......d..S(....
-00000a10: 4e52 3000 0000 5231 0000 0074 0b00 0000  NR0...R1...t....
-00000a20: 7472 6565 5f66 6f72 6d61 7474 0800 0000  tree_formatt....
-00000a30: 7068 796c 6f78 6d6c 7416 0000 0070 6879  phyloxmlt....phy
-00000a40: 6c6f 786d 6c5f 6c65 6166 5f6e 616d 655f  loxml_leaf_name_
-00000a50: 7461 6774 0400 0000 4e6f 6e65 740a 0000  tagt....Nonet...
-00000a60: 0063 6c61 6465 5f6e 616d 6528 0600 0000  .clade_name(....
-00000a70: 522c 0000 0052 2d00 0000 5201 0000 0052  R,...R-...R....R
-00000a80: 2e00 0000 521f 0000 0052 2000 0000 2801  ....R....R ...(.
-00000a90: 0000 0052 2400 0000 2800 0000 0028 0000  ...R$...(....(..
-00000aa0: 0000 7344 0000 002f 5573 6572 732f 6164  ..sD.../Users/ad
-00000ab0: 6d69 6e2f 576f 726b 2f70 726f 6a65 6374  min/Work/project
-00000ac0: 2f44 6573 7369 6d6f 7a2f 7079 6861 6d2d  /Dessimoz/pyham-
-00000ad0: 6465 762f 7079 6861 6d2f 7465 7374 732f  dev/pyham/tests/
-00000ae0: 7465 7374 5f68 616d 2e70 7974 1100 0000  test_ham.pyt....
-00000af0: 7465 7374 5f70 6879 6c6f 786d 6c5f 7461  test_phyloxml_ta
-00000b00: 6743 0000 0073 0600 0000 0002 1001 2e02  gC...s..........
-00000b10: 6301 0000 0001 0000 000b 0000 0043 0000  c............C..
-00000b20: 0073 9a00 0000 7c00 006a 0000 7401 0083  .s....|..j..t...
-00000b30: 0100 8f21 0001 7402 006a 0300 7c00 006a  ...!..t..j..|..j
-00000b40: 0400 7c00 006a 0500 6401 0064 0200 8302  ..|..j..d..d....
-00000b50: 0101 5764 0000 5158 7c00 006a 0000 7401  ..Wd..QX|..j..t.
-00000b60: 0083 0100 8f21 0001 7402 006a 0300 7c00  .....!..t..j..|.
-00000b70: 006a 0400 7c00 006a 0500 6401 0064 0300  .j..|..j..d..d..
-00000b80: 8302 0101 5764 0000 5158 7c00 006a 0000  ....Wd..QX|..j..
-00000b90: 7401 0083 0100 8f21 0001 7402 006a 0300  t......!..t..j..
-00000ba0: 7c00 006a 0400 7c00 006a 0500 6401 0064  |..j..|..j..d..d
-00000bb0: 0000 8302 0101 5764 0000 5158 6400 0053  ......Wd..QXd..S
-00000bc0: 2804 0000 004e 5230 0000 0074 0200 0000  (....NR0...t....
-00000bd0: 7873 5212 0000 0028 0700 0000 522c 0000  xsR....(....R,..
-00000be0: 0052 2d00 0000 5201 0000 0052 2e00 0000  .R-...R....R....
-00000bf0: 521e 0000 0052 2000 0000 523a 0000 0028  R....R ...R:...(
-00000c00: 0100 0000 5224 0000 0028 0000 0000 2800  ....R$...(....(.
-00000c10: 0000 0073 4400 0000 2f55 7365 7273 2f61  ...sD.../Users/a
-00000c20: 646d 696e 2f57 6f72 6b2f 7072 6f6a 6563  dmin/Work/projec
-00000c30: 742f 4465 7373 696d 6f7a 2f70 7968 616d  t/Dessimoz/pyham
-00000c40: 2d64 6576 2f70 7968 616d 2f74 6573 7473  -dev/pyham/tests
-00000c50: 2f74 6573 745f 6861 6d2e 7079 7418 0000  /test_ham.pyt...
-00000c60: 0074 6573 745f 7772 6f6e 675f 7479 7065  .test_wrong_type
-00000c70: 5f68 6f67 5f66 696c 654a 0000 0073 0c00  _hog_fileJ...s..
-00000c80: 0000 0002 1001 2202 1001 2202 1001 6301  ......"..."...c.
-00000c90: 0000 0001 0000 0009 0000 0043 0000 0073  ...........C...s
-00000ca0: 3600 0000 7c00 006a 0000 7401 0083 0100  6...|..j..t.....
-00000cb0: 8f21 0001 7402 006a 0300 7c00 006a 0400  .!..t..j..|..j..
-00000cc0: 7c00 006a 0500 6401 0064 0200 8302 0101  |..j..d..d......
-00000cd0: 5764 0000 5158 6400 0053 2803 0000 004e  Wd..QXd..S(....N
-00000ce0: 740d 0000 0066 696c 7465 725f 6f62 6a65  t....filter_obje
-00000cf0: 6374 7401 0000 0078 2806 0000 0052 2c00  ctt....x(....R,.
-00000d00: 0000 522d 0000 0052 0100 0000 522e 0000  ..R-...R....R...
-00000d10: 0052 1e00 0000 5220 0000 0028 0100 0000  .R....R ...(....
-00000d20: 5224 0000 0028 0000 0000 2800 0000 0073  R$...(....(....s
-00000d30: 4400 0000 2f55 7365 7273 2f61 646d 696e  D.../Users/admin
-00000d40: 2f57 6f72 6b2f 7072 6f6a 6563 742f 4465  /Work/project/De
-00000d50: 7373 696d 6f7a 2f70 7968 616d 2d64 6576  ssimoz/pyham-dev
-00000d60: 2f70 7968 616d 2f74 6573 7473 2f74 6573  /pyham/tests/tes
-00000d70: 745f 6861 6d2e 7079 7411 0000 0074 6573  t_ham.pyt....tes
-00000d80: 745f 7772 6f6e 675f 6669 6c74 6572 5500  t_wrong_filterU.
-00000d90: 0000 7304 0000 0000 0110 0163 0100 0000  ..s........c....
-00000da0: 0100 0000 0b00 0000 4300 0000 736e 0000  ........C...sn..
-00000db0: 0074 0000 6a01 0064 0100 7c00 006a 0200  .t..j..d..|..j..
-00000dc0: 6402 007c 0000 6a03 0064 0300 6404 0064  d..|..j..d..d..d
-00000dd0: 0500 7404 0083 0004 7c00 005f 0500 7c00  ..t.....|.._..|.
-00000de0: 006a 0600 7407 0083 0100 8f2c 0001 7400  .j..t......,..t.
-00000df0: 006a 0100 6401 007c 0000 6a02 0064 0200  .j..d..|..j..d..
-00000e00: 7c00 006a 0300 6403 0064 0400 8300 037c  |..j..d..d.....|
-00000e10: 0000 5f05 0057 6400 0051 5864 0000 5328  .._..Wd..QXd..S(
-00000e20: 0600 0000 4e74 0900 0000 7472 6565 5f66  ....Nt....tree_f
-00000e30: 696c 6574 0800 0000 686f 675f 6669 6c65  ilet....hog_file
-00000e40: 5230 0000 0052 3100 0000 7412 0000 006f  R0...R1...t....o
-00000e50: 7274 686f 584d 4c5f 6173 5f73 7472 696e  rthoXML_as_strin
-00000e60: 6728 0800 0000 5201 0000 0052 2e00 0000  g(....R....R....
-00000e70: 521e 0000 0052 2300 0000 7404 0000 0054  R....R#...t....T
-00000e80: 7275 6574 0c00 0000 6861 6d5f 616e 616c  ruet....ham_anal
-00000e90: 7973 6973 522c 0000 0074 0700 0000 494f  ysisR,...t....IO
-00000ea0: 4572 726f 7228 0100 0000 5224 0000 0028  Error(....R$...(
-00000eb0: 0000 0000 2800 0000 0073 4400 0000 2f55  ....(....sD.../U
-00000ec0: 7365 7273 2f61 646d 696e 2f57 6f72 6b2f  sers/admin/Work/
-00000ed0: 7072 6f6a 6563 742f 4465 7373 696d 6f7a  project/Dessimoz
-00000ee0: 2f70 7968 616d 2d64 6576 2f70 7968 616d  /pyham-dev/pyham
-00000ef0: 2f74 6573 7473 2f74 6573 745f 6861 6d2e  /tests/test_ham.
-00000f00: 7079 7417 0000 0074 6573 745f 6f72 7468  pyt....test_orth
-00000f10: 6f78 6d6c 5f61 735f 7374 7269 6e67 5900  oxml_as_stringY.
-00000f20: 0000 7306 0000 0000 022d 0210 0128 0900  ..s......-...(..
-00000f30: 0000 7408 0000 005f 5f6e 616d 655f 5f74  ..t....__name__t
-00000f40: 0a00 0000 5f5f 6d6f 6475 6c65 5f5f 5228  ....__module__R(
-00000f50: 0000 0052 2f00 0000 5236 0000 0052 3c00  ...R/...R6...R<.
-00000f60: 0000 523e 0000 0052 4100 0000 5248 0000  ..R>...RA...RH..
-00000f70: 0028 0000 0000 2800 0000 0028 0000 0000  .(....(....(....
-00000f80: 7344 0000 002f 5573 6572 732f 6164 6d69  sD.../Users/admi
-00000f90: 6e2f 576f 726b 2f70 726f 6a65 6374 2f44  n/Work/project/D
-00000fa0: 6573 7369 6d6f 7a2f 7079 6861 6d2d 6465  essimoz/pyham-de
-00000fb0: 762f 7079 6861 6d2f 7465 7374 732f 7465  v/pyham/tests/te
-00000fc0: 7374 5f68 616d 2e70 7952 1100 0000 1500  st_ham.pyR......
-00000fd0: 0000 730e 0000 0006 0209 0e09 1609 0809  ..s.............
-00000fe0: 0709 0b09 0474 0700 0000 4841 4d54 6573  .....t....HAMTes
-00000ff0: 7463 0000 0000 0000 0000 0100 0000 4200  tc............B.
-00001000: 0000 7323 0000 0065 0000 5a01 0064 0000  ..s#...e..Z..d..
-00001010: 8400 005a 0200 6401 0084 0000 5a03 0064  ...Z..d.....Z..d
-00001020: 0200 8400 005a 0400 5253 2803 0000 0063  .....Z..RS(....c
-00001030: 0100 0000 0400 0000 0700 0000 4300 0000  ............C...
-00001040: 7339 0100 0074 0000 6a01 006a 0200 7400  s9...t..j..j..t.
-00001050: 006a 0100 6a03 0074 0400 8301 0064 0100  .j..j..t.....d..
-00001060: 8302 007d 0100 7405 006a 0600 7c01 0064  ...}..t..j..|..d
-00001070: 0200 6403 0083 0101 7d02 0074 0000 6a01  ..d.....}..t..j.
-00001080: 006a 0200 7400 006a 0100 6a03 0074 0400  .j..t..j..j..t..
-00001090: 8301 0064 0400 8302 007d 0300 7407 006a  ...d.....}..t..j
-000010a0: 0800 6405 007c 0200 6406 007c 0300 6407  ..d..|..d..|..d.
-000010b0: 0064 0800 8300 037c 0000 5f09 007c 0000  .d.....|.._..|..
-000010c0: 6a09 006a 0a00 8300 007c 0000 5f0b 007c  j..j.....|.._..|
-000010d0: 0000 6a09 006a 0c00 8300 007c 0000 5f0d  ..j..j.....|.._.
-000010e0: 007c 0000 6a09 006a 0e00 6409 0064 0a00  .|..j..j..d..d..
-000010f0: 8300 017c 0000 5f0f 007c 0000 6a09 006a  ...|.._..|..j..j
-00001100: 0e00 6409 0064 0b00 8300 017c 0000 5f10  ..d..d.....|.._.
-00001110: 007c 0000 6a09 006a 0e00 6409 0064 0c00  .|..j..j..d..d..
-00001120: 8300 017c 0000 5f11 007c 0000 6a09 006a  ...|.._..|..j..j
-00001130: 0e00 6409 0064 0d00 8300 017c 0000 5f12  ..d..d.....|.._.
-00001140: 007c 0000 6a09 006a 0e00 6409 0064 0e00  .|..j..j..d..d..
-00001150: 8300 017c 0000 5f13 007c 0000 6a09 006a  ...|.._..|..j..j
-00001160: 1400 7c00 006a 0f00 7c00 006a 1000 6802  ..|..j..|..j..h.
-00001170: 0083 0100 7c00 005f 1500 6400 0053 280f  ....|.._..d..S(.
-00001180: 0000 004e 7313 0000 002e 2f64 6174 612f  ...Ns...../data/
-00001190: 7369 6d70 6c65 4578 2e6e 776b 5213 0000  simpleEx.nwkR...
-000011a0: 0052 1400 0000 7318 0000 002e 2f64 6174  .R....s...../dat
-000011b0: 612f 7369 6d70 6c65 4578 2e6f 7274 686f  a/simpleEx.ortho
-000011c0: 786d 6c52 4200 0000 5243 0000 0052 3000  xmlRB...RC...R0.
-000011d0: 0000 5231 0000 0074 0400 0000 6e61 6d65  ..R1...t....name
-000011e0: 7405 0000 0048 554d 414e 7405 0000 0058  t....HUMANt....X
-000011f0: 454e 5452 7405 0000 004d 4f55 5345 7405  ENTRt....MOUSEt.
-00001200: 0000 0052 4154 4e4f 7405 0000 0050 414e  ...RATNOt....PAN
-00001210: 5452 2816 0000 0052 1800 0000 5219 0000  TR(....R....R...
-00001220: 0052 1a00 0000 521b 0000 0052 1c00 0000  .R....R....R....
-00001230: 5200 0000 0052 1d00 0000 5201 0000 0052  R....R....R....R
-00001240: 2e00 0000 5246 0000 0074 1700 0000 6765  ....RF...t....ge
-00001250: 745f 6469 6374 5f74 6f70 5f6c 6576 656c  t_dict_top_level
-00001260: 5f68 6f67 7374 0400 0000 686f 6773 7415  _hogst....hogst.
-00001270: 0000 0067 6574 5f64 6963 745f 6578 7461  ...get_dict_exta
-00001280: 6e74 5f67 656e 6573 7405 0000 0067 656e  nt_genest....gen
-00001290: 6573 7419 0000 0067 6574 5f65 7874 616e  est....get_extan
-000012a0: 745f 6765 6e6f 6d65 5f62 795f 6e61 6d65  t_genome_by_name
-000012b0: 7405 0000 0068 756d 616e 7404 0000 0066  t....humant....f
-000012c0: 726f 6774 0500 0000 6d6f 7573 6574 0300  rogt....mouset..
-000012d0: 0000 7261 7474 0500 0000 6368 696d 7074  ..ratt....chimpt
-000012e0: 2a00 0000 6765 745f 616e 6365 7374 7261  *...get_ancestra
-000012f0: 6c5f 6765 6e6f 6d65 5f62 795f 6d72 6361  l_genome_by_mrca
-00001300: 5f6f 665f 6765 6e6f 6d65 5f73 6574 740b  _of_genome_sett.
-00001310: 0000 0076 6572 7465 6272 6174 6573 2804  ...vertebrates(.
-00001320: 0000 0052 2400 0000 5225 0000 0074 0800  ...R$...R%...t..
-00001330: 0000 7472 6565 5f73 7472 5220 0000 0028  ..tree_strR ...(
-00001340: 0000 0000 2800 0000 0073 4400 0000 2f55  ....(....sD.../U
-00001350: 7365 7273 2f61 646d 696e 2f57 6f72 6b2f  sers/admin/Work/
-00001360: 7072 6f6a 6563 742f 4465 7373 696d 6f7a  project/Dessimoz
-00001370: 2f70 7968 616d 2d64 6576 2f70 7968 616d  /pyham-dev/pyham
-00001380: 2f74 6573 7473 2f74 6573 745f 6861 6d2e  /tests/test_ham.
-00001390: 7079 5228 0000 0063 0000 0073 1800 0000  pyR(...c...s....
-000013a0: 0001 2101 1502 2102 2101 1201 1202 1801  ..!...!.!.......
-000013b0: 1801 1801 1801 1801 6301 0000 0001 0000  ........c.......
-000013c0: 0007 0000 0043 0000 0073 3000 0000 7c00  .....C...s0...|.
-000013d0: 006a 0000 7401 0083 0100 8f1b 0001 7c00  .j..t.........|.
-000013e0: 006a 0200 6a03 0064 0000 7c00 006a 0500  .j..j..d..|..j..
-000013f0: 8302 0001 5764 0000 5158 6400 0053 2801  ....Wd..QXd..S(.
-00001400: 0000 004e 2806 0000 0052 2c00 0000 522d  ...N(....R,...R-
-00001410: 0000 0052 4600 0000 741a 0000 0063 6f6d  ...RF...t....com
-00001420: 7061 7265 5f67 656e 6f6d 6573 5f76 6572  pare_genomes_ver
-00001430: 7469 6361 6c6c 7952 3a00 0000 525b 0000  ticallyR:...R[..
-00001440: 0028 0100 0000 5224 0000 0028 0000 0000  .(....R$...(....
-00001450: 2800 0000 0073 4400 0000 2f55 7365 7273  (....sD.../Users
-00001460: 2f61 646d 696e 2f57 6f72 6b2f 7072 6f6a  /admin/Work/proj
-00001470: 6563 742f 4465 7373 696d 6f7a 2f70 7968  ect/Dessimoz/pyh
-00001480: 616d 2d64 6576 2f70 7968 616d 2f74 6573  am-dev/pyham/tes
-00001490: 7473 2f74 6573 745f 6861 6d2e 7079 7429  ts/test_ham.pyt)
-000014a0: 0000 0074 6573 745f 636f 6d70 6172 655f  ...test_compare_
-000014b0: 6c65 7665 6c5f 636f 7272 6563 745f 696e  level_correct_in
-000014c0: 7075 745f 7665 7274 6963 616c 7400 0000  put_verticalt...
-000014d0: 7304 0000 0000 0310 0163 0100 0000 0100  s........c......
-000014e0: 0000 0700 0000 4300 0000 7330 0000 007c  ......C...s0...|
-000014f0: 0000 6a00 0074 0100 8301 008f 1b00 017c  ..j..t.........|
-00001500: 0000 6a02 006a 0300 6400 007c 0000 6a05  ..j..j..d..|..j.
-00001510: 0083 0200 0157 6400 0051 5864 0000 5328  .....Wd..QXd..S(
-00001520: 0100 0000 4e28 0600 0000 522c 0000 0052  ....N(....R,...R
-00001530: 2d00 0000 5246 0000 0074 1700 0000 636f  -...RF...t....co
-00001540: 6d70 6172 655f 6765 6e6f 6d65 735f 6c61  mpare_genomes_la
-00001550: 7465 7261 6c52 3a00 0000 525b 0000 0028  teralR:...R[...(
-00001560: 0100 0000 5224 0000 0028 0000 0000 2800  ....R$...(....(.
-00001570: 0000 0073 4400 0000 2f55 7365 7273 2f61  ...sD.../Users/a
-00001580: 646d 696e 2f57 6f72 6b2f 7072 6f6a 6563  dmin/Work/projec
-00001590: 742f 4465 7373 696d 6f7a 2f70 7968 616d  t/Dessimoz/pyham
-000015a0: 2d64 6576 2f70 7968 616d 2f74 6573 7473  -dev/pyham/tests
-000015b0: 2f74 6573 745f 6861 6d2e 7079 7428 0000  /test_ham.pyt(..
-000015c0: 0074 6573 745f 636f 6d70 6172 655f 6c65  .test_compare_le
-000015d0: 7665 6c5f 636f 7272 6563 745f 696e 7075  vel_correct_inpu
-000015e0: 745f 6c61 7465 7261 6c7a 0000 0073 0400  t_lateralz...s..
-000015f0: 0000 0003 1001 2805 0000 0052 4900 0000  ......(....RI...
-00001600: 524a 0000 0052 2800 0000 5260 0000 0052  RJ...R(...R`...R
-00001610: 6200 0000 2800 0000 0028 0000 0000 2800  b...(....(....(.
-00001620: 0000 0073 4400 0000 2f55 7365 7273 2f61  ...sD.../Users/a
-00001630: 646d 696e 2f57 6f72 6b2f 7072 6f6a 6563  dmin/Work/projec
-00001640: 742f 4465 7373 696d 6f7a 2f70 7968 616d  t/Dessimoz/pyham
-00001650: 2d64 6576 2f70 7968 616d 2f74 6573 7473  -dev/pyham/tests
-00001660: 2f74 6573 745f 6861 6d2e 7079 524b 0000  /test_ham.pyRK..
-00001670: 0061 0000 0073 0600 0000 0602 0911 0906  .a...s..........
-00001680: 740c 0000 0048 414d 5465 7374 5175 6572  t....HAMTestQuer
-00001690: 7963 0000 0000 0000 0000 0100 0000 4200  yc............B.
-000016a0: 0000 7398 0000 0065 0000 5a01 0064 0000  ..s....e..Z..d..
-000016b0: 8400 005a 0200 6401 0084 0000 5a03 0064  ...Z..d.....Z..d
-000016c0: 0200 8400 005a 0400 6403 0084 0000 5a05  .....Z..d.....Z.
-000016d0: 0064 0400 8400 005a 0600 6405 0084 0000  .d.....Z..d.....
-000016e0: 5a07 0064 0600 8400 005a 0800 6407 0084  Z..d.....Z..d...
-000016f0: 0000 5a09 0064 0800 8400 005a 0a00 6409  ..Z..d.....Z..d.
-00001700: 0084 0000 5a0b 0064 0a00 8400 005a 0c00  ....Z..d.....Z..
-00001710: 640b 0084 0000 5a0d 0064 0c00 8400 005a  d.....Z..d.....Z
-00001720: 0e00 640d 0084 0000 5a0f 0064 0e00 8400  ..d.....Z..d....
-00001730: 005a 1000 640f 0084 0000 5a11 0052 5328  .Z..d.....Z..RS(
-00001740: 1000 0000 6301 0000 000a 0000 000e 0000  ....c...........
-00001750: 0043 0000 0073 9002 0000 7400 006a 0100  .C...s....t..j..
-00001760: 6a02 0074 0000 6a01 006a 0300 7404 0083  j..t..j..j..t...
-00001770: 0100 6401 0083 0200 7d01 0074 0500 6a06  ..d.....}..t..j.
-00001780: 007c 0100 6402 0064 0300 8301 017d 0200  .|..d..d.....}..
-00001790: 7400 006a 0100 6a02 0074 0000 6a01 006a  t..j..j..t..j..j
-000017a0: 0300 7404 0083 0100 6401 0083 0200 7d03  ..t.....d.....}.
-000017b0: 0074 0500 6a06 007c 0300 6402 0064 0300  .t..j..|..d..d..
-000017c0: 8301 017d 0400 7400 006a 0100 6a02 0074  ...}..t..j..j..t
-000017d0: 0000 6a01 006a 0300 7404 0083 0100 6404  ..j..j..t.....d.
-000017e0: 0083 0200 7d05 0074 0000 6a01 006a 0200  ....}..t..j..j..
-000017f0: 7400 006a 0100 6a03 0074 0400 8301 0064  t..j..j..t.....d
-00001800: 0500 8302 007d 0600 7407 007c 0600 6406  .....}..t..|..d.
-00001810: 0083 0200 8f1c 007d 0700 7c07 006a 0800  .......}..|..j..
-00001820: 8300 007d 0800 7c08 007c 0000 5f09 0057  ...}..|..|.._..W
-00001830: 6400 0051 5874 0a00 6a0b 007c 0200 7c06  d..QXt..j..|..|.
-00001840: 0064 0700 740c 0083 0201 7c00 005f 0d00  .d..t.....|.._..
-00001850: 740a 006a 0b00 7c04 007c 0600 8302 007c  t..j..|..|.....|
-00001860: 0000 5f0e 0074 0a00 6a0b 007c 0500 7c06  .._..t..j..|..|.
-00001870: 0064 0700 740c 0064 0800 6409 0064 0a00  .d..t..d..d..d..
-00001880: 640b 0064 0c00 640d 0083 0204 7c00 005f  d..d..d.....|.._
-00001890: 0f00 640e 0064 0f00 6410 0064 1100 6804  ..d..d..d..d..h.
-000018a0: 007c 0000 5f10 0064 1200 6413 0064 1400  .|.._..d..d..d..
-000018b0: 6415 0068 0400 7c00 005f 1100 6416 0064  d..h..|.._..d..d
-000018c0: 1700 6418 0064 1900 6804 007c 0000 5f12  ..d..d..h..|.._.
-000018d0: 0064 1200 6801 007c 0000 5f13 0064 1a00  .d..h..|.._..d..
-000018e0: 641b 0068 0200 7c00 005f 1400 641c 0064  d..h..|.._..d..d
-000018f0: 1d00 641e 0064 1f00 6420 0064 2100 6422  ..d..d..d .d!.d"
-00001900: 0064 2300 6424 0064 2500 6426 0064 2700  .d#.d$.d%.d&.d'.
-00001910: 6428 0068 0d00 7c00 005f 1500 6429 0064  d(.h..|.._..d).d
-00001920: 2a00 642b 0064 2c00 642d 0064 2e00 642f  *.d+.d,.d-.d..d/
-00001930: 0064 3000 6431 0064 3200 6433 0064 3400  .d0.d1.d2.d3.d4.
-00001940: 6435 0068 0d00 7c00 005f 1600 641c 0064  d5.h..|.._..d..d
-00001950: 2200 6802 007c 0000 5f17 0074 0a00 6a18  ".h..|.._..t..j.
-00001960: 0083 0000 7d09 007c 0900 6a19 0064 3600  ....}..|..j..d6.
-00001970: 6701 0083 0100 0174 0a00 6a0b 007c 0200  g......t..j..|..
-00001980: 7c06 0064 3700 7c09 0064 0700 740c 0083  |..d7.|..d..t...
-00001990: 0202 7c00 005f 1a00 740a 006a 0b00 7c02  ..|.._..t..j..|.
-000019a0: 007c 0000 6a09 0064 0700 740c 0064 3800  .|..j..d..t..d8.
-000019b0: 740c 0083 0202 7c00 005f 1b00 740a 006a  t.....|.._..t..j
-000019c0: 0b00 7c02 007c 0000 6a09 0064 3700 7c09  ..|..|..j..d7.|.
-000019d0: 0064 0700 740c 0064 3800 740c 0083 0203  .d..t..d8.t.....
-000019e0: 7c00 005f 1c00 6400 0053 2839 0000 004e  |.._..d..S(9...N
-000019f0: 7313 0000 002e 2f64 6174 612f 7369 6d70  s...../data/simp
-00001a00: 6c65 4578 2e6e 776b 5213 0000 0052 1400  leEx.nwkR....R..
-00001a10: 0000 7318 0000 002e 2f64 6174 612f 7369  ..s...../data/si
-00001a20: 6d70 6c65 4578 2e70 6879 6c6f 786d 6c73  mpleEx.phyloxmls
-00001a30: 1800 0000 2e2f 6461 7461 2f73 696d 706c  ...../data/simpl
-00001a40: 6545 782e 6f72 7468 6f78 6d6c 5215 0000  eEx.orthoxmlR...
-00001a50: 0074 1100 0000 7573 655f 696e 7465 726e  .t....use_intern
-00001a60: 616c 5f6e 616d 6552 3700 0000 5238 0000  al_nameR7...R8..
-00001a70: 0074 1a00 0000 7068 796c 6f78 6d6c 5f69  .t....phyloxml_i
-00001a80: 6e74 6572 6e61 6c5f 6e61 6d65 5f74 6167  nternal_name_tag
-00001a90: 7418 0000 0074 6178 6f6e 6f6d 795f 7363  t....taxonomy_sc
-00001aa0: 6965 6e74 6966 6963 5f6e 616d 6552 3900  ientific_nameR9.
-00001ab0: 0000 740d 0000 0074 6178 6f6e 6f6d 795f  ..t....taxonomy_
-00001ac0: 636f 6465 524d 0000 0052 4f00 0000 7405  codeRM...RO...t.
-00001ad0: 0000 0043 414e 4641 5251 0000 0074 0100  ...CANFARQ...t..
-00001ae0: 0000 3274 0200 0000 3332 7402 0000 0032  ..2t....32t....2
-00001af0: 3274 0200 0000 3132 7406 0000 0048 554d  2t....12t....HUM
-00001b00: 414e 3274 0600 0000 4d4f 5553 4532 7406  AN2t....MOUSE2t.
-00001b10: 0000 0043 414e 4641 3274 0600 0000 5041  ...CANFA2t....PA
-00001b20: 4e54 5232 524e 0000 0052 5000 0000 7401  NTR2RN...RP...t.
-00001b30: 0000 0031 7402 0000 0031 3174 0200 0000  ...1t....11t....
-00001b40: 3231 7402 0000 0033 3174 0200 0000 3431  21t....31t....41
-00001b50: 7402 0000 0035 3174 0100 0000 3374 0200  t....51t....3t..
-00001b60: 0000 3133 7402 0000 0032 3374 0200 0000  ..13t....23t....
-00001b70: 3333 7402 0000 0035 3374 0200 0000 3334  33t....53t....34
-00001b80: 7402 0000 0031 3474 0600 0000 4855 4d41  t....14t....HUMA
-00001b90: 4e31 7406 0000 0050 414e 5452 3174 0600  N1t....PANTR1t..
-00001ba0: 0000 4341 4e46 4131 7406 0000 004d 4f55  ..CANFA1t....MOU
-00001bb0: 5345 3174 0600 0000 5241 544e 4f31 7406  SE1t....RATNO1t.
-00001bc0: 0000 0058 454e 5452 3174 0600 0000 4855  ...XENTR1t....HU
-00001bd0: 4d41 4e33 7406 0000 0050 414e 5452 3374  MAN3t....PANTR3t
-00001be0: 0600 0000 4341 4e46 4133 7406 0000 004d  ....CANFA3t....M
-00001bf0: 4f55 5345 3374 0600 0000 5845 4e54 5233  OUSE3t....XENTR3
-00001c00: 7406 0000 004d 4f55 5345 3474 0600 0000  t....MOUSE4t....
-00001c10: 5041 4e54 5234 6902 0000 0052 3f00 0000  PANTR4i....R?...
-00001c20: 5244 0000 0028 1d00 0000 5218 0000 0052  RD...(....R....R
-00001c30: 1900 0000 521a 0000 0052 1b00 0000 521c  ....R....R....R.
-00001c40: 0000 0052 0000 0000 521d 0000 0052 2100  ...R....R....R!.
-00001c50: 0000 5222 0000 0052 2300 0000 5201 0000  ..R"...R#...R...
-00001c60: 0052 2e00 0000 5245 0000 0074 0100 0000  .R....RE...t....
-00001c70: 6874 0200 0000 686e 7403 0000 0068 7078  ht....hnt....hpx
-00001c80: 740d 0000 0066 696c 7465 725f 6765 6e6f  t....filter_geno
-00001c90: 6d65 740c 0000 0066 696c 7465 725f 6765  met....filter_ge
-00001ca0: 6e65 7374 1000 0000 6669 6c74 6572 5f67  nest....filter_g
-00001cb0: 656e 6573 5f65 7874 740b 0000 0066 696c  enes_extt....fil
-00001cc0: 7465 725f 686f 6773 7410 0000 006e 6f5f  ter_hogst....no_
-00001cd0: 6669 6c74 6572 5f67 656e 6f6d 6574 0f00  filter_genomet..
-00001ce0: 0000 6e6f 5f66 696c 7465 725f 6765 6e65  ..no_filter_gene
-00001cf0: 7374 1300 0000 6e6f 5f66 696c 7465 725f  st....no_filter_
-00001d00: 6765 6e65 735f 6578 7474 0e00 0000 6e6f  genes_extt....no
-00001d10: 5f66 696c 7465 725f 686f 6773 740c 0000  _filter_hogst...
-00001d20: 0050 6172 7365 7246 696c 7465 7274 1200  .ParserFiltert..
-00001d30: 0000 6164 645f 686f 6773 5f76 6961 5f68  ..add_hogs_via_h
-00001d40: 6f67 4964 7402 0000 0068 6674 0700 0000  ogIdt....hft....
-00001d50: 6873 7472 696e 6774 0800 0000 6866 7374  hstringt....hfst
-00001d60: 7269 6e67 280a 0000 0052 2400 0000 5225  ring(....R$...R%
-00001d70: 0000 0052 1e00 0000 7410 0000 006e 776b  ...R....t....nwk
-00001d80: 5f70 6174 685f 6e6f 5f6e 616d 6574 0f00  _path_no_namet..
-00001d90: 0000 6e77 6b5f 7374 725f 6e6f 5f6e 616d  ..nwk_str_no_nam
-00001da0: 6552 1f00 0000 5220 0000 0052 2600 0000  eR....R ...R&...
-00001db0: 5227 0000 0074 0100 0000 6628 0000 0000  R'...t....f(....
-00001dc0: 2800 0000 0073 4400 0000 2f55 7365 7273  (....sD.../Users
-00001dd0: 2f61 646d 696e 2f57 6f72 6b2f 7072 6f6a  /admin/Work/proj
-00001de0: 6563 742f 4465 7373 696d 6f7a 2f70 7968  ect/Dessimoz/pyh
-00001df0: 616d 2d64 6576 2f70 7968 616d 2f74 6573  am-dev/pyham/tes
-00001e00: 7473 2f74 6573 745f 6861 6d2e 7079 5228  ts/test_ham.pyR(
-00001e10: 0000 0083 0000 0073 3600 0000 0001 2101  .......s6.....!.
-00001e20: 1502 2101 1502 2102 2102 1201 0c01 0f03  ..!...!.!.......
-00001e30: 1b03 1503 2d03 1501 1501 1501 0c01 0f01  ....-...........
-00001e40: 3001 1501 1b01 0f01 0c01 1001 2103 1801  0...........!...
-00001e50: 0c03 6301 0000 0004 0000 0009 0000 0043  ..c............C
-00001e60: 0000 0073 a001 0000 7c00 006a 0000 7401  ...s....|..j..t.
-00001e70: 0083 0100 8f15 0001 7c00 006a 0200 6a03  ........|..j..j.
-00001e80: 0064 0100 8301 0001 5764 0000 5158 7c00  .d......Wd..QX|.
-00001e90: 006a 0200 6a03 0064 0200 8301 007d 0100  .j..j..d.....}..
-00001ea0: 7c00 006a 0400 7405 007c 0100 8301 0064  |..j..t..|.....d
-00001eb0: 0300 8302 0001 7c00 006a 0200 6a03 0064  ......|..j..j..d
-00001ec0: 0400 8301 007d 0100 7c00 006a 0400 7405  .....}..|..j..t.
-00001ed0: 007c 0100 8301 0064 0300 8302 0001 7c00  .|.....d......|.
-00001ee0: 006a 0600 6a03 0064 0400 8301 007d 0100  .j..j..d.....}..
-00001ef0: 7c00 006a 0400 7405 007c 0100 8301 0064  |..j..t..|.....d
-00001f00: 0300 8302 0001 7c00 006a 0700 6a03 0064  ......|..j..j..d
-00001f10: 0400 8301 007d 0100 7c00 006a 0400 7405  .....}..|..j..t.
-00001f20: 007c 0100 8301 0064 0300 8302 0001 7873  .|.....d......xs
-00001f30: 007c 0000 6a08 0044 5d68 007d 0200 7c00  .|..j..D]h.}..|.
-00001f40: 006a 0900 6a03 007c 0200 8301 007d 0300  .j..j..|.....}..
-00001f50: 7c00 006a 0400 7405 007c 0300 8301 0064  |..j..t..|.....d
-00001f60: 0500 6a0a 007c 0200 8301 0083 0200 017c  ..j..|.........|
-00001f70: 0000 6a0b 006a 0300 7c02 0083 0100 7d03  ..j..j..|.....}.
-00001f80: 007c 0000 6a04 0074 0500 7c03 0083 0100  .|..j..t..|.....
-00001f90: 6405 006a 0a00 7c02 0083 0100 8302 0001  d..j..|.........
-00001fa0: 71d0 0057 785d 007c 0000 6a0c 0044 5d52  q..Wx].|..j..D]R
-00001fb0: 007d 0200 7c00 006a 0000 7401 0083 0100  .}..|..j..t.....
-00001fc0: 8f15 0001 7c00 006a 0900 6a03 007c 0200  ....|..j..j..|..
-00001fd0: 8301 0001 5764 0000 5158 7c00 006a 0000  ....Wd..QX|..j..
-00001fe0: 7401 0083 0100 8f15 0001 7c00 006a 0b00  t.........|..j..
-00001ff0: 6a03 007c 0200 8301 0001 5764 0000 5158  j..|......Wd..QX
-00002000: 7146 0157 6400 0053 2806 0000 004e 7401  qF.Wd..S(....Nt.
-00002010: 0000 0064 5277 0000 0073 0800 0000 3c48  ...dRw...s....<H
-00002020: 4f47 2833 293e 6903 0000 0073 0900 0000  OG(3)>i....s....
-00002030: 3c48 4f47 287b 7d29 3e28 0d00 0000 522c  <HOG({})>(....R,
-00002040: 0000 0074 0800 0000 4b65 7945 7272 6f72  ...t....KeyError
-00002050: 528b 0000 0074 0d00 0000 6765 745f 686f  R....t....get_ho
-00002060: 675f 6279 5f69 6474 0b00 0000 6173 7365  g_by_idt....asse
-00002070: 7274 4571 7561 6c52 0400 0000 5299 0000  rtEqualR....R...
-00002080: 0052 8d00 0000 5291 0000 0052 9800 0000  .R....R....R....
-00002090: 7406 0000 0066 6f72 6d61 7452 9a00 0000  t....formatR....
-000020a0: 5295 0000 0028 0400 0000 5224 0000 0074  R....(....R$...t
-000020b0: 0400 0000 686f 6733 7406 0000 0068 6f67  ....hog3t....hog
-000020c0: 5f69 6474 0300 0000 686f 6728 0000 0000  _idt....hog(....
-000020d0: 2800 0000 0073 4400 0000 2f55 7365 7273  (....sD.../Users
-000020e0: 2f61 646d 696e 2f57 6f72 6b2f 7072 6f6a  /admin/Work/proj
-000020f0: 6563 742f 4465 7373 696d 6f7a 2f70 7968  ect/Dessimoz/pyh
-00002100: 616d 2d64 6576 2f70 7968 616d 2f74 6573  am-dev/pyham/tes
-00002110: 7473 2f74 6573 745f 6861 6d2e 7079 7412  ts/test_ham.pyt.
-00002120: 0000 0074 6573 745f 6765 745f 686f 675f  ...test_get_hog_
-00002130: 6279 5f69 64b2 0000 0073 2800 0000 0003  by_id....s(.....
-00002140: 1001 1603 1201 1603 1201 1602 1201 1602  ................
-00002150: 1201 1607 1001 1201 1f02 1201 2302 1001  ............#...
-00002160: 1001 1602 1001 6301 0000 0006 0000 0008  ......c.........
-00002170: 0000 0043 0000 0073 3201 0000 7c00 006a  ...C...s2...|..j
-00002180: 0000 6a01 0064 0100 8301 007d 0100 7c00  ..j..d.....}..|.
-00002190: 006a 0000 6a02 007c 0100 8301 007d 0200  .j..j..|.....}..
-000021a0: 7c00 006a 0300 7404 007c 0200 8301 0064  |..j..t..|.....d
-000021b0: 0200 8302 0001 7c00 006a 0500 6a02 007c  ......|..j..j..|
-000021c0: 0100 8301 007d 0200 7c00 006a 0300 7404  .....}..|..j..t.
-000021d0: 007c 0200 8301 0064 0200 8302 0001 7c00  .|.....d......|.
-000021e0: 006a 0600 7407 0083 0100 8f15 0001 7c00  .j..t.........|.
-000021f0: 006a 0000 6a02 0064 0300 8301 0001 5764  .j..j..d......Wd
-00002200: 0000 5158 7857 007c 0000 6a08 0044 5d4c  ..QXxW.|..j..D]L
-00002210: 007d 0300 7c00 006a 0900 6a01 007c 0300  .}..|..j..j..|..
-00002220: 8301 007d 0400 7c00 006a 0900 6a02 007c  ...}..|..j..j..|
-00002230: 0400 8301 007d 0500 7c00 006a 0300 7404  .....}..|..j..t.
-00002240: 007c 0500 8301 0064 0400 6a0a 007c 0500  .|.....d..j..|..
-00002250: 6a0b 0083 0100 8302 0001 7192 0057 7849  j.........q..WxI
-00002260: 007c 0000 6a0c 0044 5d3e 007d 0300 7c00  .|..j..D]>.}..|.
-00002270: 006a 0600 7407 0083 0100 8f27 0001 7c00  .j..t......'..|.
-00002280: 006a 0900 6a01 007c 0300 8301 007d 0400  .j..j..|.....}..
-00002290: 7c00 006a 0900 6a02 007c 0400 8301 0001  |..j..j..|......
-000022a0: 5764 0000 5158 71ec 0057 6400 0053 2805  Wd..QXq..Wd..S(.
-000022b0: 0000 004e 5277 0000 0073 0800 0000 3c48  ...NRw...s....<H
-000022c0: 4f47 2833 293e 7404 0000 0067 656e 6573  OG(3)>t....genes
-000022d0: 0900 0000 3c48 4f47 287b 7d29 3e28 0d00  ....<HOG({})>(..
-000022e0: 0000 528b 0000 0074 0e00 0000 6765 745f  ..R....t....get_
-000022f0: 6765 6e65 5f62 795f 6964 740f 0000 0067  gene_by_idt....g
-00002300: 6574 5f68 6f67 5f62 795f 6765 6e65 52a1  et_hog_by_geneR.
-00002310: 0000 0052 0400 0000 528d 0000 0052 2c00  ...R....R....R,.
-00002320: 0000 529f 0000 0052 8f00 0000 5298 0000  ..R....R....R...
-00002330: 0052 a200 0000 52a4 0000 0052 9300 0000  .R....R....R....
-00002340: 2806 0000 0052 2400 0000 7405 0000 0067  (....R$...t....g
-00002350: 656e 6533 52a3 0000 0074 0700 0000 6765  ene3R....t....ge
-00002360: 6e65 5f69 6452 a700 0000 52a5 0000 0028  ne_idR....R....(
-00002370: 0000 0000 2800 0000 0073 4400 0000 2f55  ....(....sD.../U
-00002380: 7365 7273 2f61 646d 696e 2f57 6f72 6b2f  sers/admin/Work/
-00002390: 7072 6f6a 6563 742f 4465 7373 696d 6f7a  project/Dessimoz
-000023a0: 2f70 7968 616d 2d64 6576 2f70 7968 616d  /pyham-dev/pyham
-000023b0: 2f74 6573 7473 2f74 6573 745f 6861 6d2e  /tests/test_ham.
-000023c0: 7079 7414 0000 0074 6573 745f 6765 745f  pyt....test_get_
-000023d0: 686f 675f 6279 5f67 656e 65d9 0000 0073  hog_by_gene....s
-000023e0: 1e00 0000 0002 1203 1201 1602 1201 1603  ................
-000023f0: 1001 1606 1001 1201 1201 2602 1001 1001  ..........&.....
-00002400: 1201 6301 0000 0002 0000 0005 0000 0043  ..c............C
-00002410: 0000 0073 8800 0000 7c00 006a 0000 6a01  ...s....|..j..j.
-00002420: 0083 0000 7d01 007c 0000 6a02 0074 0300  ....}..|..j..t..
-00002430: 7c01 0083 0100 6401 0064 0200 6403 0068  |.....d..d..d..h
-00002440: 0300 8302 0001 7c00 006a 0400 6a01 0083  ......|..j..j...
-00002450: 0000 7d01 007c 0000 6a02 0074 0300 7c01  ..}..|..j..t..|.
-00002460: 0083 0100 6401 0064 0200 6403 0068 0300  ....d..d..d..h..
-00002470: 8302 0001 7c00 006a 0500 6a01 0083 0000  ....|..j..j.....
-00002480: 7d01 007c 0000 6a02 0074 0300 7c01 0083  }..|..j..t..|...
-00002490: 0100 6401 0068 0100 8302 0001 6400 0053  ..d..h......d..S
-000024a0: 2804 0000 004e 7308 0000 003c 484f 4728  (....Ns....<HOG(
-000024b0: 3229 3e73 0800 0000 3c48 4f47 2831 293e  2)>s....<HOG(1)>
-000024c0: 7308 0000 003c 484f 4728 3329 3e28 0600  s....<HOG(3)>(..
-000024d0: 0000 528b 0000 0074 1700 0000 6765 745f  ..R....t....get_
-000024e0: 6c69 7374 5f74 6f70 5f6c 6576 656c 5f68  list_top_level_h
-000024f0: 6f67 7374 0e00 0000 6173 7365 7274 5365  ogst....assertSe
-00002500: 7445 7175 616c 5210 0000 0052 8d00 0000  tEqualR....R....
-00002510: 5298 0000 0028 0200 0000 5224 0000 0052  R....(....R$...R
-00002520: 5300 0000 2800 0000 0028 0000 0000 7344  S...(....(....sD
-00002530: 0000 002f 5573 6572 732f 6164 6d69 6e2f  .../Users/admin/
-00002540: 576f 726b 2f70 726f 6a65 6374 2f44 6573  Work/project/Des
-00002550: 7369 6d6f 7a2f 7079 6861 6d2d 6465 762f  simoz/pyham-dev/
-00002560: 7079 6861 6d2f 7465 7374 732f 7465 7374  pyham/tests/test
-00002570: 5f68 616d 2e70 7974 1c00 0000 7465 7374  _ham.pyt....test
-00002580: 5f67 6574 5f6c 6973 745f 746f 705f 6c65  _get_list_top_le
-00002590: 7665 6c5f 686f 6773 f600 0000 730c 0000  vel_hogs....s...
-000025a0: 0000 010f 011f 020f 011f 060f 0163 0100  .............c..
-000025b0: 0000 0200 0000 0500 0000 4300 0000 73d0  ..........C...s.
-000025c0: 0000 007c 0000 6a00 006a 0100 8300 007d  ...|..j..j.....}
-000025d0: 0100 7c00 006a 0200 7403 007c 0100 8301  ..|..j..t..|....
-000025e0: 0069 0300 6401 0064 0200 3664 0300 6404  .i..d..d..6d..d.
-000025f0: 0036 6405 0064 0600 3683 0200 017c 0000  .6d..d..6....|..
-00002600: 6a04 006a 0100 8300 007d 0100 7c00 006a  j..j.....}..|..j
-00002610: 0200 7403 007c 0100 8301 0069 0300 6401  ..t..|.....i..d.
-00002620: 0064 0200 3664 0300 6404 0036 6405 0064  .d..6d..d..6d..d
-00002630: 0600 3683 0200 017c 0000 6a05 006a 0100  ..6....|..j..j..
-00002640: 8300 007d 0100 7c00 006a 0200 7403 007c  ...}..|..j..t..|
-00002650: 0100 8301 0069 0100 6401 0064 0200 3683  .....i..d..d..6.
-00002660: 0200 017c 0000 6a06 006a 0100 8300 007d  ...|..j..j.....}
-00002670: 0100 7c00 006a 0200 7403 007c 0100 8301  ..|..j..t..|....
-00002680: 0069 0100 6401 0064 0200 3683 0200 0164  .i..d..d..6....d
-00002690: 0000 5328 0700 0000 4e73 0800 0000 3c48  ..S(....Ns....<H
-000026a0: 4f47 2832 293e 5269 0000 0073 0800 0000  OG(2)>Ri...s....
-000026b0: 3c48 4f47 2831 293e 5271 0000 0073 0800  <HOG(1)>Rq...s..
-000026c0: 0000 3c48 4f47 2833 293e 5277 0000 0028  ..<HOG(3)>Rw...(
-000026d0: 0700 0000 528b 0000 0052 5200 0000 740f  ....R....RR...t.
-000026e0: 0000 0061 7373 6572 7444 6963 7445 7175  ...assertDictEqu
-000026f0: 616c 520a 0000 0052 8d00 0000 5298 0000  alR....R....R...
-00002700: 0052 9a00 0000 2802 0000 0052 2400 0000  .R....(....R$...
-00002710: 5253 0000 0028 0000 0000 2800 0000 0073  RS...(....(....s
-00002720: 4400 0000 2f55 7365 7273 2f61 646d 696e  D.../Users/admin
-00002730: 2f57 6f72 6b2f 7072 6f6a 6563 742f 4465  /Work/project/De
-00002740: 7373 696d 6f7a 2f70 7968 616d 2d64 6576  ssimoz/pyham-dev
-00002750: 2f70 7968 616d 2f74 6573 7473 2f74 6573  /pyham/tests/tes
-00002760: 745f 6861 6d2e 7079 741c 0000 0074 6573  t_ham.pyt....tes
-00002770: 745f 6765 745f 6469 6374 5f74 6f70 5f6c  t_get_dict_top_l
-00002780: 6576 656c 5f68 6f67 7304 0100 0073 1000  evel_hogs....s..
-00002790: 0000 0001 0f01 2b02 0f01 2b06 0f01 1d02  ......+...+.....
-000027a0: 0f01 6301 0000 0004 0000 0008 0000 0043  ..c............C
-000027b0: 0000 0073 2101 0000 7c00 006a 0000 7401  ...s!...|..j..t.
-000027c0: 0083 0100 8f15 0001 7c00 006a 0200 6a03  ........|..j..j.
-000027d0: 0064 0100 8301 0001 5764 0000 5158 7c00  .d......Wd..QX|.
-000027e0: 006a 0200 6a03 0064 0200 8301 007d 0100  .j..j..d.....}..
-000027f0: 7c00 006a 0400 7405 007c 0100 8301 0064  |..j..t..|.....d
-00002800: 0300 8302 0001 7c00 006a 0600 6a03 0064  ......|..j..j..d
-00002810: 0200 8301 007d 0100 7c00 006a 0400 7405  .....}..|..j..t.
-00002820: 007c 0100 8301 0064 0300 8302 0001 7c00  .|.....d......|.
-00002830: 006a 0200 6a03 0064 0400 8301 007d 0100  .j..j..d.....}..
-00002840: 7c00 006a 0400 7405 007c 0100 8301 0064  |..j..t..|.....d
-00002850: 0300 8302 0001 7842 007c 0000 6a07 0044  ......xB.|..j..D
-00002860: 5d37 007d 0200 7c00 006a 0800 6a03 007c  ]7.}..|..j..j..|
-00002870: 0200 8301 007d 0300 7c00 006a 0400 7405  .....}..|..j..t.
-00002880: 007c 0300 8301 0064 0500 6a09 007c 0200  .|.....d..j..|..
-00002890: 8301 0083 0200 0171 a800 5778 3700 7c00  .......q..Wx7.|.
-000028a0: 006a 0a00 445d 2c00 7d02 007c 0000 6a00  .j..D],.}..|..j.
-000028b0: 0074 0100 8301 008f 1500 017c 0000 6a08  .t.........|..j.
-000028c0: 006a 0300 7c02 0083 0100 0157 6400 0051  .j..|......Wd..Q
-000028d0: 5871 ed00 5764 0000 5328 0600 0000 4e52  Xq..Wd..S(....NR
-000028e0: 9e00 0000 5277 0000 0073 0700 0000 4765  ....Rw...s....Ge
-000028f0: 6e65 2833 2969 0300 0000 7308 0000 0047  ne(3)i....s....G
-00002900: 656e 6528 7b7d 2928 0b00 0000 522c 0000  ene({})(....R,..
-00002910: 0052 9f00 0000 528b 0000 0052 a800 0000  .R....R....R....
-00002920: 52a1 0000 0052 0400 0000 528d 0000 0052  R....R....R....R
-00002930: 9100 0000 5298 0000 0052 a200 0000 5293  ....R....R....R.
-00002940: 0000 0028 0400 0000 5224 0000 0052 aa00  ...(....R$...R..
-00002950: 0000 52ab 0000 0052 a700 0000 2800 0000  ..R....R....(...
-00002960: 0028 0000 0000 7344 0000 002f 5573 6572  .(....sD.../User
-00002970: 732f 6164 6d69 6e2f 576f 726b 2f70 726f  s/admin/Work/pro
-00002980: 6a65 6374 2f44 6573 7369 6d6f 7a2f 7079  ject/Dessimoz/py
-00002990: 6861 6d2d 6465 762f 7079 6861 6d2f 7465  ham-dev/pyham/te
-000029a0: 7374 732f 7465 7374 5f68 616d 2e70 7974  sts/test_ham.pyt
-000029b0: 1300 0000 7465 7374 5f67 6574 5f67 656e  ....test_get_gen
-000029c0: 655f 6279 5f69 6417 0100 0073 1c00 0000  e_by_id....s....
-000029d0: 0003 1001 1603 1201 1602 1201 1603 1201  ................
-000029e0: 1606 1001 1201 2302 1001 1001 6301 0000  ......#.....c...
-000029f0: 0004 0000 0008 0000 0043 0000 0073 9301  .........C...s..
-00002a00: 0000 7c00 006a 0000 7401 0083 0100 8f15  ..|..j..t.......
-00002a10: 0001 7c00 006a 0200 6a03 0064 0100 8301  ..|..j..j..d....
-00002a20: 0001 5764 0000 5158 7c00 006a 0200 6a03  ..Wd..QX|..j..j.
-00002a30: 0064 0200 8301 0064 0300 197d 0100 7c00  .d.....d...}..|.
-00002a40: 006a 0400 7405 007c 0100 8301 0064 0400  .j..t..|.....d..
-00002a50: 8302 0001 7c00 006a 0200 6a03 0064 0500  ....|..j..j..d..
-00002a60: 8301 0064 0300 197d 0100 7c00 006a 0400  ...d...}..|..j..
-00002a70: 7405 007c 0100 8301 0064 0400 8302 0001  t..|.....d......
-00002a80: 7c00 006a 0600 6a03 0064 0500 8301 0064  |..j..j..d.....d
-00002a90: 0300 197d 0100 7c00 006a 0400 7405 007c  ...}..|..j..t..|
-00002aa0: 0100 8301 0064 0400 8302 0001 7c00 006a  .....d......|..j
-00002ab0: 0700 6a03 0064 0200 8301 0064 0300 197d  ..j..d.....d...}
-00002ac0: 0100 7c00 006a 0400 7405 007c 0100 8301  ..|..j..t..|....
-00002ad0: 0064 0400 8302 0001 7c00 006a 0700 6a03  .d......|..j..j.
-00002ae0: 0064 0500 8301 0064 0300 197d 0100 7c00  .d.....d...}..|.
-00002af0: 006a 0400 7405 007c 0100 8301 0064 0400  .j..t..|.....d..
-00002b00: 8302 0001 7850 007c 0000 6a08 0044 5d45  ....xP.|..j..D]E
-00002b10: 007d 0200 7c00 006a 0900 6a03 007c 0200  .}..|..j..j..|..
-00002b20: 8301 007d 0300 7c00 006a 0400 740a 007c  ...}..|..j..t..|
-00002b30: 0300 8301 0064 0600 8302 0001 7c00 006a  .....d......|..j
-00002b40: 0400 7c03 0064 0300 196a 0b00 7c02 0083  ..|..d...j..|...
-00002b50: 0200 0171 0c01 5778 3700 7c00 006a 0c00  ...q..Wx7.|..j..
-00002b60: 445d 2c00 7d02 007c 0000 6a00 0074 0100  D],.}..|..j..t..
-00002b70: 8301 008f 1500 017c 0000 6a09 006a 0300  .......|..j..j..
-00002b80: 7c02 0083 0100 0157 6400 0051 5871 5f01  |......Wd..QXq_.
-00002b90: 5764 0000 5328 0700 0000 4e52 9e00 0000  Wd..S(....NR....
-00002ba0: 5270 0000 0069 0000 0000 7308 0000 0047  Rp...i....s....G
-00002bb0: 656e 6528 3132 2974 0700 0000 5041 4e54  ene(12)t....PANT
-00002bc0: 5267 3269 0100 0000 280d 0000 0052 2c00  Rg2i....(....R,.
-00002bd0: 0000 529f 0000 0052 8b00 0000 7418 0000  ..R....R....t...
-00002be0: 0067 6574 5f67 656e 6573 5f62 795f 6578  .get_genes_by_ex
-00002bf0: 7465 726e 616c 5f69 6452 a100 0000 5204  ternal_idR....R.
-00002c00: 0000 0052 9900 0000 528d 0000 0052 9000  ...R....R....R..
-00002c10: 0000 5298 0000 0074 0300 0000 6c65 6e74  ..R....t....lent
-00002c20: 0700 0000 7072 6f74 5f69 6452 9400 0000  ....prot_idR....
-00002c30: 2804 0000 0052 2400 0000 7406 0000 0067  (....R$...t....g
-00002c40: 656e 6531 3252 ab00 0000 5255 0000 0028  ene12R....RU...(
-00002c50: 0000 0000 2800 0000 0073 4400 0000 2f55  ....(....sD.../U
-00002c60: 7365 7273 2f61 646d 696e 2f57 6f72 6b2f  sers/admin/Work/
-00002c70: 7072 6f6a 6563 742f 4465 7373 696d 6f7a  project/Dessimoz
-00002c80: 2f70 7968 616d 2d64 6576 2f70 7968 616d  /pyham-dev/pyham
-00002c90: 2f74 6573 7473 2f74 6573 745f 6861 6d2e  /tests/test_ham.
-00002ca0: 7079 741d 0000 0074 6573 745f 6765 745f  pyt....test_get_
-00002cb0: 6765 6e65 735f 6279 5f65 7874 6572 6e61  genes_by_externa
-00002cc0: 6c5f 6964 3401 0000 7326 0000 0000 0310  l_id4...s&......
-00002cd0: 0116 0316 0116 0316 0116 0216 0116 0316  ................
-00002ce0: 0116 0316 0116 0710 0112 0116 011b 0210  ................
-00002cf0: 0110 0163 0100 0000 0400 0000 1300 0000  ...c............
-00002d00: 4300 0000 7348 0100 007c 0000 6a00 006a  C...sH...|..j..j
-00002d10: 0100 8300 007d 0100 6401 0064 0200 6403  .....}..d..d..d.
-00002d20: 0064 0400 6405 0064 0600 6407 0064 0800  .d..d..d..d..d..
-00002d30: 6409 0064 0a00 640b 0064 0c00 640d 0064  d..d..d..d..d..d
-00002d40: 0e00 640f 0064 1000 6411 0064 1200 6413  ..d..d..d..d..d.
-00002d50: 0068 1300 7d02 007c 0000 6a02 0074 0300  .h..}..|..j..t..
-00002d60: 7c01 0083 0100 7c02 0083 0200 017c 0000  |.....|......|..
-00002d70: 6a04 006a 0100 8300 007d 0100 6401 0064  j..j.....}..d..d
-00002d80: 0200 6403 0064 0400 6405 0064 0600 6407  ..d..d..d..d..d.
-00002d90: 0064 0800 6409 0064 0a00 640b 0064 0c00  .d..d..d..d..d..
-00002da0: 640d 0064 0e00 640f 0064 1000 6411 0064  d..d..d..d..d..d
-00002db0: 1200 6413 0068 1300 7d02 007c 0000 6a02  ..d..h..}..|..j.
-00002dc0: 0074 0300 7c01 0083 0100 7c02 0083 0200  .t..|.....|.....
-00002dd0: 017c 0000 6a05 006a 0100 8300 007d 0100  .|..j..j.....}..
-00002de0: 7c00 006a 0200 7406 0067 0000 7c01 0044  |..j..t..g..|..D
-00002df0: 5d0f 007d 0300 7c03 006a 0700 5e02 0071  ]..}..|..j..^..q
-00002e00: e700 8301 007c 0000 6a08 0083 0200 017c  .....|..j......|
-00002e10: 0000 6a09 006a 0100 8300 007d 0100 7c00  ..j..j.....}..|.
-00002e20: 006a 0200 7406 0067 0000 7c01 0044 5d0f  .j..t..g..|..D].
-00002e30: 007d 0300 7c03 006a 0700 5e02 0071 2501  .}..|..j..^..q%.
-00002e40: 8301 007c 0000 6a08 0083 0200 0164 0000  ...|..j......d..
-00002e50: 5328 1400 0000 4e73 0800 0000 4765 6e65  S(....Ns....Gene
-00002e60: 2833 3329 7308 0000 0047 656e 6528 3134  (33)s....Gene(14
-00002e70: 2973 0800 0000 4765 6e65 2833 3129 7308  )s....Gene(31)s.
-00002e80: 0000 0047 656e 6528 3531 2973 0800 0000  ...Gene(51)s....
-00002e90: 4765 6e65 2831 3329 7308 0000 0047 656e  Gene(13)s....Gen
-00002ea0: 6528 3131 2973 0800 0000 4765 6e65 2831  e(11)s....Gene(1
-00002eb0: 3229 7308 0000 0047 656e 6528 3233 2973  2)s....Gene(23)s
-00002ec0: 0800 0000 4765 6e65 2832 3129 7307 0000  ....Gene(21)s...
-00002ed0: 0047 656e 6528 3229 7308 0000 0047 656e  .Gene(2)s....Gen
-00002ee0: 6528 3334 2973 0700 0000 4765 6e65 2831  e(34)s....Gene(1
-00002ef0: 2973 0800 0000 4765 6e65 2833 3229 7307  )s....Gene(32)s.
-00002f00: 0000 0047 656e 6528 3529 7308 0000 0047  ...Gene(5)s....G
-00002f10: 656e 6528 3232 2973 0700 0000 4765 6e65  ene(22)s....Gene
-00002f20: 2833 2973 0800 0000 4765 6e65 2834 3129  (3)s....Gene(41)
-00002f30: 7308 0000 0047 656e 6528 3533 2973 0800  s....Gene(53)s..
-00002f40: 0000 4765 6e65 2834 3329 280a 0000 0052  ..Gene(43)(....R
-00002f50: 8b00 0000 7415 0000 0067 6574 5f6c 6973  ....t....get_lis
-00002f60: 745f 6578 7461 6e74 5f67 656e 6573 52ae  t_extant_genesR.
-00002f70: 0000 0052 1000 0000 528d 0000 0052 9800  ...R....R....R..
-00002f80: 0000 520c 0000 0074 0900 0000 756e 6971  ..R....t....uniq
-00002f90: 7565 5f69 6452 8f00 0000 529a 0000 0028  ue_idR....R....(
-00002fa0: 0400 0000 5224 0000 0052 5500 0000 7408  ....R$...RU...t.
-00002fb0: 0000 0065 7870 6563 7465 6474 0100 0000  ...expectedt....
-00002fc0: 6728 0000 0000 2800 0000 0073 4400 0000  g(....(....sD...
-00002fd0: 2f55 7365 7273 2f61 646d 696e 2f57 6f72  /Users/admin/Wor
-00002fe0: 6b2f 7072 6f6a 6563 742f 4465 7373 696d  k/project/Dessim
-00002ff0: 6f7a 2f70 7968 616d 2d64 6576 2f70 7968  oz/pyham-dev/pyh
-00003000: 616d 2f74 6573 7473 2f74 6573 745f 6861  am/tests/test_ha
-00003010: 6d2e 7079 741a 0000 0074 6573 745f 6765  m.pyt....test_ge
-00003020: 745f 6c69 7374 5f65 7874 616e 745f 6765  t_list_extant_ge
-00003030: 6e65 735b 0100 0073 1c00 0000 0002 0f01  nes[...s........
-00003040: 1801 1801 0f01 1602 0f01 1801 1801 0f01  ................
-00003050: 1606 0f01 2f02 0f01 6301 0000 0003 0000  ..../...c.......
-00003060: 0005 0000 0043 0000 0073 a501 0000 7c00  .....C...s....|.
-00003070: 006a 0000 6a01 0083 0000 7d01 0069 1300  .j..j.....}..i..
-00003080: 6401 0064 0200 3664 0300 6404 0036 6405  d..d..6d..d..6d.
-00003090: 0064 0600 3664 0700 6408 0036 6409 0064  .d..6d..d..6d..d
-000030a0: 0a00 3664 0b00 640c 0036 640d 0064 0e00  ..6d..d..6d..d..
-000030b0: 3664 0f00 6410 0036 6411 0064 1200 3664  6d..d..6d..d..6d
-000030c0: 1300 6414 0036 6415 0064 1600 3664 1700  ..d..6d..d..6d..
-000030d0: 6418 0036 6419 0064 1a00 3664 1b00 641c  d..6d..d..6d..d.
-000030e0: 0036 641d 0064 1e00 3664 1f00 6420 0036  .6d..d..6d..d .6
-000030f0: 6421 0064 2200 3664 2300 6424 0036 6425  d!.d".6d#.d$.6d%
-00003100: 0064 2600 367d 0200 7c00 006a 0200 7403  .d&.6}..|..j..t.
-00003110: 007c 0100 8301 007c 0200 8302 0001 7c00  .|.....|......|.
-00003120: 006a 0400 6a01 0083 0000 7d01 0069 1300  .j..j.....}..i..
-00003130: 6401 0064 0200 3664 0300 6404 0036 6405  d..d..6d..d..6d.
-00003140: 0064 0600 3664 0700 6408 0036 6409 0064  .d..6d..d..6d..d
-00003150: 0a00 3664 0b00 640c 0036 640d 0064 0e00  ..6d..d..6d..d..
-00003160: 3664 0f00 6410 0036 6411 0064 1200 3664  6d..d..6d..d..6d
-00003170: 1300 6414 0036 6415 0064 1600 3664 1700  ..d..6d..d..6d..
-00003180: 6418 0036 6419 0064 1a00 3664 1b00 641c  d..6d..d..6d..d.
-00003190: 0036 641d 0064 1e00 3664 1f00 6420 0036  .6d..d..6d..d .6
-000031a0: 6421 0064 2200 3664 2300 6424 0036 6425  d!.d".6d#.d$.6d%
-000031b0: 0064 2600 367d 0200 7c00 006a 0200 7403  .d&.6}..|..j..t.
-000031c0: 007c 0100 8301 007c 0200 8302 0001 7c00  .|.....|......|.
-000031d0: 006a 0500 6a01 0083 0000 7d01 007c 0000  .j..j.....}..|..
-000031e0: 6a02 0074 0300 7c01 0083 0100 6904 0064  j..t..|.....i..d
-000031f0: 1f00 6420 0036 640f 0064 1000 3664 0500  ..d .6d..d..6d..
-00003200: 6406 0036 6407 0064 0800 3683 0200 0164  d..6d..d..6....d
-00003210: 0000 5328 2700 0000 4e73 0800 0000 4765  ..S('...Ns....Ge
-00003220: 6e65 2833 3429 527c 0000 0073 0800 0000  ne(34)R|...s....
-00003230: 4765 6e65 2833 3329 527a 0000 0073 0700  Gene(33)Rz...s..
-00003240: 0000 4765 6e65 2832 2952 6900 0000 7308  ..Gene(2)Ri...s.
-00003250: 0000 0047 656e 6528 3132 2952 6c00 0000  ...Gene(12)Rl...
-00003260: 7307 0000 0047 656e 6528 3529 7401 0000  s....Gene(5)t...
-00003270: 0035 7308 0000 0047 656e 6528 3131 2952  .5s....Gene(11)R
-00003280: 7200 0000 7307 0000 0047 656e 6528 3129  r...s....Gene(1)
-00003290: 5271 0000 0073 0800 0000 4765 6e65 2832  Rq...s....Gene(2
-000032a0: 3229 526b 0000 0073 0700 0000 4765 6e65  2)Rk...s....Gene
-000032b0: 2833 2952 7700 0000 7308 0000 0047 656e  (3)Rw...s....Gen
-000032c0: 6528 3431 2952 7500 0000 7308 0000 0047  e(41)Ru...s....G
-000032d0: 656e 6528 3531 2952 7600 0000 7308 0000  ene(51)Rv...s...
-000032e0: 0047 656e 6528 3533 2952 7b00 0000 7308  .Gene(53)R{...s.
-000032f0: 0000 0047 656e 6528 3134 2952 7d00 0000  ...Gene(14)R}...
-00003300: 7308 0000 0047 656e 6528 3133 2952 7800  s....Gene(13)Rx.
-00003310: 0000 7308 0000 0047 656e 6528 3433 2974  ..s....Gene(43)t
-00003320: 0200 0000 3433 7308 0000 0047 656e 6528  ....43s....Gene(
-00003330: 3332 2952 6a00 0000 7308 0000 0047 656e  32)Rj...s....Gen
-00003340: 6528 3233 2952 7900 0000 7308 0000 0047  e(23)Ry...s....G
-00003350: 656e 6528 3231 2952 7300 0000 7308 0000  ene(21)Rs...s...
-00003360: 0047 656e 6528 3331 2952 7400 0000 2806  .Gene(31)Rt...(.
-00003370: 0000 0052 8b00 0000 5254 0000 0052 b000  ...R....RT...R..
-00003380: 0000 520a 0000 0052 8d00 0000 5298 0000  ..R....R....R...
-00003390: 0028 0300 0000 5224 0000 0052 5500 0000  .(....R$...RU...
-000033a0: 52bb 0000 0028 0000 0000 2800 0000 0073  R....(....(....s
-000033b0: 4400 0000 2f55 7365 7273 2f61 646d 696e  D.../Users/admin
-000033c0: 2f57 6f72 6b2f 7072 6f6a 6563 742f 4465  /Work/project/De
-000033d0: 7373 696d 6f7a 2f70 7968 616d 2d64 6576  ssimoz/pyham-dev
-000033e0: 2f70 7968 616d 2f74 6573 7473 2f74 6573  /pyham/tests/tes
-000033f0: 745f 6861 6d2e 7079 741a 0000 0074 6573  t_ham.pyt....tes
-00003400: 745f 6765 745f 6469 6374 5f65 7874 616e  t_get_dict_extan
-00003410: 745f 6765 6e65 7373 0100 0073 1e00 0000  t_geness...s....
-00003420: 0002 0f01 2601 2a01 2a01 1101 1602 0f01  ....&.*.*.......
-00003430: 2601 2a01 2301 0701 1101 1606 0f01 6301  &.*.#.........c.
-00003440: 0000 0004 0000 0008 0000 0043 0000 0073  ...........C...s
-00003450: 3b01 0000 7c00 006a 0000 7401 0083 0100  ;...|..j..t.....
-00003460: 8f15 0001 7c00 006a 0200 6a03 0064 0100  ....|..j..j..d..
-00003470: 8301 0001 5764 0000 5158 7c00 006a 0000  ....Wd..QX|..j..
-00003480: 7401 0083 0100 8f15 0001 7c00 006a 0200  t.........|..j..
-00003490: 6a03 0064 0200 8301 0001 5764 0000 5158  j..d......Wd..QX
-000034a0: 7c00 006a 0000 7401 0083 0100 8f15 0001  |..j..t.........
-000034b0: 7c00 006a 0200 6a03 0064 0300 8301 0001  |..j..j..d......
-000034c0: 5764 0000 5158 7c00 006a 0200 6a03 0064  Wd..QX|..j..j..d
-000034d0: 0400 8301 007d 0100 7c00 006a 0400 7c01  .....}..|..j..|.
-000034e0: 006a 0500 6404 0083 0200 017c 0000 6a06  .j..d......|..j.
-000034f0: 006a 0300 6404 0083 0100 7d01 007c 0000  .j..d.....}..|..
-00003500: 6a04 007c 0100 6a05 0064 0400 8302 0001  j..|..j..d......
-00003510: 7839 007c 0000 6a07 0044 5d2e 007d 0200  x9.|..j..D]..}..
-00003520: 7c00 006a 0800 6a03 007c 0200 8301 007d  |..j..j..|.....}
-00003530: 0300 7c00 006a 0400 7409 007c 0300 8301  ..|..j..t..|....
-00003540: 007c 0200 8302 0001 71c6 0057 783c 007c  .|......q..Wx<.|
-00003550: 0000 6a0a 0044 5d31 007d 0200 7c00 006a  ..j..D]1.}..|..j
-00003560: 0800 6a03 007c 0200 8301 007d 0300 7c00  ..j..|.....}..|.
-00003570: 006a 0400 740b 007c 0300 6a0c 0083 0100  .j..t..|..j.....
-00003580: 6405 0083 0200 0171 0201 5764 0000 5328  d......q..Wd..S(
-00003590: 0600 0000 4e52 1200 0000 7403 0000 0061  ....NR....t....a
-000035a0: 6263 6901 0000 0052 4d00 0000 6900 0000  bci....RM...i...
-000035b0: 0028 0d00 0000 522c 0000 0052 9f00 0000  .(....R,...R....
-000035c0: 528b 0000 0052 5600 0000 52a1 0000 0052  R....RV...R....R
-000035d0: 4c00 0000 528d 0000 0052 8e00 0000 5298  L...R....R....R.
-000035e0: 0000 0052 0400 0000 5292 0000 0052 b500  ...R....R....R..
-000035f0: 0000 5255 0000 0028 0400 0000 5224 0000  ..RU...(....R$..
-00003600: 0052 8b00 0000 7405 0000 0067 6e61 6d65  .R....t....gname
-00003610: 7406 0000 0067 656e 6f6d 6528 0000 0000  t....genome(....
-00003620: 2800 0000 0073 4400 0000 2f55 7365 7273  (....sD.../Users
-00003630: 2f61 646d 696e 2f57 6f72 6b2f 7072 6f6a  /admin/Work/proj
-00003640: 6563 742f 4465 7373 696d 6f7a 2f70 7968  ect/Dessimoz/pyh
-00003650: 616d 2d64 6576 2f70 7968 616d 2f74 6573  am-dev/pyham/tes
-00003660: 7473 2f74 6573 745f 6861 6d2e 7079 741e  ts/test_ham.pyt.
-00003670: 0000 0074 6573 745f 6765 745f 6578 7461  ...test_get_exta
-00003680: 6e74 5f67 656e 6f6d 655f 6279 5f6e 616d  nt_genome_by_nam
-00003690: 658d 0100 0073 2000 0000 0002 1001 1602  e....s .........
-000036a0: 1001 1602 1001 1602 1201 1302 1201 1305  ................
-000036b0: 1001 1201 1a02 1001 1201 6301 0000 0003  ..........c.....
-000036c0: 0000 0006 0000 0043 0000 0073 7e00 0000  .......C...s~...
-000036d0: 7c00 006a 0000 6a01 0083 0000 7d01 0064  |..j..j.....}..d
-000036e0: 0100 6402 0064 0300 6404 0064 0500 6406  ..d..d..d..d..d.
-000036f0: 0068 0600 7d02 007c 0000 6a02 0074 0300  .h..}..|..j..t..
-00003700: 7c01 0083 0100 7c02 0083 0200 017c 0000  |.....|......|..
-00003710: 6a04 006a 0100 8300 007d 0100 6401 0064  j..j.....}..d..d
-00003720: 0200 6403 0064 0400 6405 0064 0600 6806  ..d..d..d..d..h.
-00003730: 007d 0200 7c00 006a 0200 7403 007c 0100  .}..|..j..t..|..
-00003740: 8301 007c 0200 8302 0001 6400 0053 2807  ...|......d..S(.
-00003750: 0000 004e 5250 0000 0052 4d00 0000 524f  ...NRP...RM...RO
-00003760: 0000 0052 4e00 0000 5251 0000 0052 6800  ...RN...RQ...Rh.
-00003770: 0000 2805 0000 0052 8b00 0000 7417 0000  ..(....R....t...
-00003780: 0067 6574 5f6c 6973 745f 6578 7461 6e74  .get_list_extant
-00003790: 5f67 656e 6f6d 6573 52ae 0000 0052 1000  _genomesR....R..
-000037a0: 0000 528d 0000 0028 0300 0000 5224 0000  ..R....(....R$..
-000037b0: 0074 0300 0000 6c65 6752 bb00 0000 2800  .t....legR....(.
-000037c0: 0000 0028 0000 0000 7344 0000 002f 5573  ...(....sD.../Us
-000037d0: 6572 732f 6164 6d69 6e2f 576f 726b 2f70  ers/admin/Work/p
-000037e0: 726f 6a65 6374 2f44 6573 7369 6d6f 7a2f  roject/Dessimoz/
-000037f0: 7079 6861 6d2d 6465 762f 7079 6861 6d2f  pyham-dev/pyham/
-00003800: 7465 7374 732f 7465 7374 5f68 616d 2e70  tests/test_ham.p
-00003810: 7974 1c00 0000 7465 7374 5f67 6574 5f6c  yt....test_get_l
-00003820: 6973 745f 6578 7461 6e74 5f67 656e 6f6d  ist_extant_genom
-00003830: 6573 a901 0000 730c 0000 0000 020f 0118  es....s.........
-00003840: 0116 020f 0118 0163 0100 0000 0400 0000  .......c........
-00003850: 0600 0000 4300 0000 73be 0000 007c 0000  ....C...s....|..
-00003860: 6a00 0074 0100 8301 008f 1500 017c 0000  j..t.........|..
-00003870: 6a02 006a 0300 6401 0083 0100 0157 6400  j..j..d......Wd.
-00003880: 0051 587c 0000 6a02 006a 0300 6402 0083  .QX|..j..j..d...
-00003890: 0100 7d01 007c 0000 6a04 007c 0100 6a05  ..}..|..j..|..j.
-000038a0: 0064 0200 8302 0001 7c00 006a 0600 6a03  .d......|..j..j.
-000038b0: 0064 0300 8301 007d 0200 7c00 006a 0400  .d.....}..|..j..
-000038c0: 7c02 006a 0500 6403 0083 0200 017c 0000  |..j..d......|..
-000038d0: 6a06 006a 0300 6404 0083 0100 7d03 007c  j..j..d.....}..|
-000038e0: 0000 6a04 007c 0300 6a05 0064 0400 8302  ..j..|..j..d....
-000038f0: 0001 7c00 006a 0700 6a03 0064 0400 8301  ..|..j..j..d....
-00003900: 007d 0300 7c00 006a 0400 7c03 006a 0500  .}..|..j..|..j..
-00003910: 6404 0083 0200 0164 0000 5328 0500 0000  d......d..S(....
-00003920: 4e52 1200 0000 7408 0000 004d 616d 6d61  NR....t....Mamma
-00003930: 6c69 6173 0b00 0000 4d4f 5553 452f 5241  lias....MOUSE/RA
-00003940: 544e 4f52 4f00 0000 2808 0000 0052 2c00  TNORO...(....R,.
-00003950: 0000 529f 0000 0052 8b00 0000 7411 0000  ..R....R....t...
-00003960: 0067 6574 5f74 6178 6f6e 5f62 795f 6e61  .get_taxon_by_na
-00003970: 6d65 52a1 0000 0052 4c00 0000 528c 0000  meR....RL...R...
-00003980: 0052 8d00 0000 2804 0000 0052 2400 0000  .R....(....R$...
-00003990: 7407 0000 006d 616d 6d61 6c73 7407 0000  t....mammalst...
-000039a0: 0072 6f64 656e 7473 5259 0000 0028 0000  .rodentsRY...(..
-000039b0: 0000 2800 0000 0073 4400 0000 2f55 7365  ..(....sD.../Use
-000039c0: 7273 2f61 646d 696e 2f57 6f72 6b2f 7072  rs/admin/Work/pr
-000039d0: 6f6a 6563 742f 4465 7373 696d 6f7a 2f70  oject/Dessimoz/p
-000039e0: 7968 616d 2d64 6576 2f70 7968 616d 2f74  yham-dev/pyham/t
-000039f0: 6573 7473 2f74 6573 745f 6861 6d2e 7079  ests/test_ham.py
-00003a00: 7416 0000 0074 6573 745f 6765 745f 7461  t....test_get_ta
-00003a10: 786f 6e5f 6279 5f6e 616d 65b5 0100 0073  xon_by_name....s
-00003a20: 1400 0000 0002 1001 1603 1201 1302 1201  ................
-00003a30: 1303 1201 1304 1201 6301 0000 0004 0000  ........c.......
-00003a40: 0006 0000 0043 0000 0073 aa00 0000 7c00  .....C...s....|.
-00003a50: 006a 0000 6a01 0064 0100 8301 007d 0100  .j..j..d.....}..
-00003a60: 7c00 006a 0000 6a02 007c 0100 8301 007d  |..j..j..|.....}
-00003a70: 0200 7c00 006a 0300 7c02 006a 0400 6401  ..|..j..|..j..d.
-00003a80: 0083 0200 017c 0000 6a05 006a 0100 6401  .....|..j..j..d.
-00003a90: 0083 0100 7d01 007c 0000 6a05 006a 0200  ....}..|..j..j..
-00003aa0: 7c01 0083 0100 7d02 007c 0000 6a03 007c  |.....}..|..j..|
-00003ab0: 0200 6a04 0064 0100 8302 0001 7c00 006a  ..j..d......|..j
-00003ac0: 0600 7407 0083 0100 8f27 0001 7c00 006a  ..t......'..|..j
-00003ad0: 0800 6a01 0064 0200 8301 007d 0300 7c00  ..j..d.....}..|.
-00003ae0: 006a 0000 6a02 007c 0300 8301 0001 5764  .j..j..|......Wd
-00003af0: 0000 5158 6400 0053 2803 0000 004e 52c8  ..QXd..S(....NR.
-00003b00: 0000 0074 0a00 0000 5665 7274 6562 7261  ...t....Vertebra
-00003b10: 7461 2809 0000 0052 8b00 0000 52c9 0000  ta(....R....R...
-00003b20: 0074 1d00 0000 6765 745f 616e 6365 7374  .t....get_ancest
-00003b30: 7261 6c5f 6765 6e6f 6d65 5f62 795f 7461  ral_genome_by_ta
-00003b40: 786f 6e52 a100 0000 524c 0000 0052 8d00  xonR....RL...R..
-00003b50: 0000 522c 0000 0052 9f00 0000 5298 0000  ..R,...R....R...
-00003b60: 0028 0400 0000 5224 0000 0074 0b00 0000  .(....R$...t....
-00003b70: 6d61 6d6d 616c 735f 7461 7852 ca00 0000  mammals_taxR....
-00003b80: 740e 0000 0076 6572 7465 6272 6174 655f  t....vertebrate_
-00003b90: 7461 7828 0000 0000 2800 0000 0073 4400  tax(....(....sD.
-00003ba0: 0000 2f55 7365 7273 2f61 646d 696e 2f57  ../Users/admin/W
-00003bb0: 6f72 6b2f 7072 6f6a 6563 742f 4465 7373  ork/project/Dess
-00003bc0: 696d 6f7a 2f70 7968 616d 2d64 6576 2f70  imoz/pyham-dev/p
-00003bd0: 7968 616d 2f74 6573 7473 2f74 6573 745f  yham/tests/test_
-00003be0: 6861 6d2e 7079 7422 0000 0074 6573 745f  ham.pyt"...test_
-00003bf0: 6765 745f 616e 6365 7374 7261 6c5f 6765  get_ancestral_ge
-00003c00: 6e6f 6d65 5f62 795f 7461 786f 6ecc 0100  nome_by_taxon...
-00003c10: 0073 1200 0000 0002 1201 1201 1302 1201  .s..............
-00003c20: 1201 1306 1001 1201 6301 0000 0003 0000  ........c.......
-00003c30: 0006 0000 0043 0000 0073 9900 0000 7c00  .....C...s....|.
-00003c40: 006a 0000 6a01 0064 0100 8301 007d 0100  .j..j..d.....}..
-00003c50: 7c00 006a 0200 7c01 006a 0300 6401 0083  |..j..|..j..d...
-00003c60: 0200 017c 0000 6a04 006a 0100 6401 0083  ...|..j..j..d...
-00003c70: 0100 7d01 007c 0000 6a02 007c 0100 6a03  ..}..|..j..|..j.
-00003c80: 0064 0100 8302 0001 7c00 006a 0500 6a01  .d......|..j..j.
-00003c90: 0064 0200 8301 007d 0200 7c00 006a 0200  .d.....}..|..j..
-00003ca0: 7c02 006a 0300 6402 0083 0200 017c 0000  |..j..d......|..
-00003cb0: 6a06 0074 0700 8301 008f 1500 017c 0000  j..t.........|..
-00003cc0: 6a08 006a 0100 6403 0083 0100 0157 6400  j..j..d......Wd.
-00003cd0: 0051 5864 0000 5328 0400 0000 4e52 c800  .QXd..S(....NR..
-00003ce0: 0000 730b 0000 004d 4f55 5345 2f52 4154  ..s....MOUSE/RAT
-00003cf0: 4e4f 52cd 0000 0028 0900 0000 528b 0000  NOR....(....R...
-00003d00: 0074 1c00 0000 6765 745f 616e 6365 7374  .t....get_ancest
-00003d10: 7261 6c5f 6765 6e6f 6d65 5f62 795f 6e61  ral_genome_by_na
-00003d20: 6d65 52a1 0000 0052 4c00 0000 528d 0000  meR....RL...R...
-00003d30: 0052 8c00 0000 522c 0000 0052 9f00 0000  .R....R,...R....
-00003d40: 5298 0000 0028 0300 0000 5224 0000 0052  R....(....R$...R
-00003d50: ca00 0000 52cb 0000 0028 0000 0000 2800  ....R....(....(.
-00003d60: 0000 0073 4400 0000 2f55 7365 7273 2f61  ...sD.../Users/a
-00003d70: 646d 696e 2f57 6f72 6b2f 7072 6f6a 6563  dmin/Work/projec
-00003d80: 742f 4465 7373 696d 6f7a 2f70 7968 616d  t/Dessimoz/pyham
-00003d90: 2d64 6576 2f70 7968 616d 2f74 6573 7473  -dev/pyham/tests
-00003da0: 2f74 6573 745f 6861 6d2e 7079 7421 0000  /test_ham.pyt!..
-00003db0: 0074 6573 745f 6765 745f 616e 6365 7374  .test_get_ancest
-00003dc0: 7261 6c5f 6765 6e6f 6d65 5f62 795f 6e61  ral_genome_by_na
-00003dd0: 6d65 de01 0000 7310 0000 0000 0212 0113  me....s.........
-00003de0: 0212 0113 0212 0113 0610 0163 0100 0000  ...........c....
-00003df0: 0300 0000 0700 0000 4300 0000 736c 0000  ........C...sl..
-00003e00: 007c 0000 6a00 006a 0100 8300 007d 0100  .|..j..j.....}..
-00003e10: 7c00 006a 0200 7403 007c 0100 8301 0064  |..j..t..|.....d
-00003e20: 0100 6402 0064 0300 6404 0064 0500 6805  ..d..d..d..d..h.
-00003e30: 0083 0200 017c 0000 6a04 006a 0100 8300  .....|..j..j....
-00003e40: 007d 0200 7c00 006a 0200 7403 007c 0200  .}..|..j..t..|..
-00003e50: 8301 0064 0600 6407 0064 0800 6409 0064  ...d..d..d..d..d
-00003e60: 0a00 6805 0083 0200 0164 0000 5328 0b00  ..h......d..S(..
-00003e70: 0000 4e74 1000 0000 4575 6172 6368 6f6e  ..Nt....Euarchon
-00003e80: 746f 676c 6972 6573 52cd 0000 0052 c800  togliresR....R..
-00003e90: 0000 7408 0000 0050 7269 6d61 7465 7374  ..t....Primatest
-00003ea0: 0700 0000 526f 6465 6e74 7373 1700 0000  ....Rodentss....
-00003eb0: 4855 4d41 4e2f 5041 4e54 522f 4d4f 5553  HUMAN/PANTR/MOUS
-00003ec0: 452f 5241 544e 4f73 2300 0000 5845 4e54  E/RATNOs#...XENT
-00003ed0: 522f 4855 4d41 4e2f 5041 4e54 522f 4d4f  R/HUMAN/PANTR/MO
-00003ee0: 5553 452f 5241 544e 4f2f 4341 4e46 4173  USE/RATNO/CANFAs
-00003ef0: 1d00 0000 4855 4d41 4e2f 5041 4e54 522f  ....HUMAN/PANTR/
-00003f00: 4d4f 5553 452f 5241 544e 4f2f 4341 4e46  MOUSE/RATNO/CANF
-00003f10: 4173 0b00 0000 4855 4d41 4e2f 5041 4e54  As....HUMAN/PANT
-00003f20: 5273 0b00 0000 4d4f 5553 452f 5241 544e  Rs....MOUSE/RATN
-00003f30: 4f28 0500 0000 528b 0000 0074 1a00 0000  O(....R....t....
-00003f40: 6765 745f 6c69 7374 5f61 6e63 6573 7472  get_list_ancestr
-00003f50: 616c 5f67 656e 6f6d 6573 52ae 0000 0052  al_genomesR....R
-00003f60: 1000 0000 528c 0000 0028 0300 0000 5224  ....R....(....R$
-00003f70: 0000 0074 0300 0000 6c61 6774 0b00 0000  ...t....lagt....
-00003f80: 6c61 675f 6e6f 5f6e 616d 6528 0000 0000  lag_no_name(....
-00003f90: 2800 0000 0073 4400 0000 2f55 7365 7273  (....sD.../Users
-00003fa0: 2f61 646d 696e 2f57 6f72 6b2f 7072 6f6a  /admin/Work/proj
-00003fb0: 6563 742f 4465 7373 696d 6f7a 2f70 7968  ect/Dessimoz/pyh
-00003fc0: 616d 2d64 6576 2f70 7968 616d 2f74 6573  am-dev/pyham/tes
-00003fd0: 7473 2f74 6573 745f 6861 6d2e 7079 741f  ts/test_ham.pyt.
-00003fe0: 0000 0074 6573 745f 6765 745f 6c69 7374  ...test_get_list
-00003ff0: 5f61 6e63 6573 7472 616c 5f67 656e 6f6d  _ancestral_genom
-00004000: 6573 f001 0000 7308 0000 0000 020f 0125  es....s........%
-00004010: 020f 0163 0100 0000 0600 0000 0900 0000  ...c............
-00004020: 4300 0000 736f 0100 007c 0000 6a00 006a  C...so...|..j..j
-00004030: 0100 6401 0064 0200 8300 017d 0100 7c00  ..d..d.....}..|.
-00004040: 006a 0000 6a01 0064 0100 6403 0083 0001  .j..j..d..d.....
-00004050: 7d02 007c 0000 6a02 0074 0300 8301 008f  }..|..j..t......
-00004060: 1800 017c 0000 6a00 006a 0400 7c02 0068  ...|..j..j..|..h
-00004070: 0100 8301 0001 5764 0000 5158 7c00 006a  ......Wd..QX|..j
-00004080: 0200 7405 0083 0100 8f1b 0001 7c00 006a  ..t.........|..j
-00004090: 0000 6a04 007c 0200 6404 0068 0200 8301  ..j..|..d..h....
-000040a0: 0001 5764 0000 5158 7c00 006a 0000 6a04  ..Wd..QX|..j..j.
-000040b0: 007c 0100 7c02 0068 0200 8301 007d 0300  .|..|..h.....}..
-000040c0: 7c00 006a 0600 6405 007c 0300 6a07 0083  |..j..d..|..j...
-000040d0: 0200 017c 0000 6a00 006a 0400 7c03 007c  ...|..j..j..|..|
-000040e0: 0200 6802 0083 0100 7d04 007c 0000 6a06  ..h.....}..|..j.
-000040f0: 0064 0500 7c04 006a 0700 8302 0001 7c00  .d..|..j......|.
-00004100: 006a 0800 6a01 0064 0100 6402 0083 0001  .j..j..d..d.....
-00004110: 7d01 007c 0000 6a08 006a 0100 6401 0064  }..|..j..j..d..d
-00004120: 0300 8300 017d 0200 7c00 006a 0800 6a04  .....}..|..j..j.
-00004130: 007c 0100 7c02 0068 0200 8301 007d 0300  .|..|..h.....}..
-00004140: 7c00 006a 0600 6405 007c 0300 6a07 0083  |..j..d..|..j...
-00004150: 0200 017c 0000 6a02 0074 0900 8301 008f  ...|..j..t......
-00004160: 3000 017c 0000 6a08 006a 0100 6401 0064  0..|..j..j..d..d
-00004170: 0600 8300 017d 0500 7c00 006a 0800 6a04  .....}..|..j..j.
-00004180: 007c 0100 7c05 0068 0200 8301 0001 5764  .|..|..h......Wd
-00004190: 0000 5158 6400 0053 2807 0000 004e 524c  ..QXd..S(....NRL
-000041a0: 0000 0052 4d00 0000 524f 0000 0052 5700  ...RM...RO...RW.
-000041b0: 0000 52d4 0000 0052 4e00 0000 280a 0000  ..R....RN...(...
-000041c0: 0052 8b00 0000 5256 0000 0052 2c00 0000  .R....RV...R,...
-000041d0: 740a 0000 0056 616c 7565 4572 726f 7252  t....ValueErrorR
-000041e0: 5c00 0000 522d 0000 0052 a100 0000 524c  \...R-...R....RL
-000041f0: 0000 0052 9800 0000 529f 0000 0028 0600  ...R....R....(..
-00004200: 0000 5224 0000 0052 5700 0000 5259 0000  ..R$...RW...RY..
-00004210: 0074 1000 0000 6575 6172 6368 6f6e 746f  .t....euarchonto
-00004220: 676c 6972 6573 7411 0000 0065 7561 7263  glirest....euarc
-00004230: 686f 6e74 6f67 6c69 7265 7332 5258 0000  hontoglires2RX..
-00004240: 0028 0000 0000 2800 0000 0073 4400 0000  .(....(....sD...
-00004250: 2f55 7365 7273 2f61 646d 696e 2f57 6f72  /Users/admin/Wor
-00004260: 6b2f 7072 6f6a 6563 742f 4465 7373 696d  k/project/Dessim
-00004270: 6f7a 2f70 7968 616d 2d64 6576 2f70 7968  oz/pyham-dev/pyh
-00004280: 616d 2f74 6573 7473 2f74 6573 745f 6861  am/tests/test_ha
-00004290: 6d2e 7079 742f 0000 0074 6573 745f 6765  m.pyt/...test_ge
-000042a0: 745f 616e 6365 7374 7261 6c5f 6765 6e6f  t_ancestral_geno
-000042b0: 6d65 5f62 795f 6d72 6361 5f6f 665f 6765  me_by_mrca_of_ge
-000042c0: 6e6f 6d65 5f73 6574 f801 0000 7322 0000  nome_set....s"..
-000042d0: 0000 0215 0115 0210 0119 0210 011c 0218  ................
-000042e0: 0113 0318 0113 0615 0115 0218 0113 0210  ................
-000042f0: 0115 0128 1200 0000 5249 0000 0052 4a00  ...(....RI...RJ.
-00004300: 0000 5228 0000 0052 a600 0000 52ac 0000  ..R(...R....R...
-00004310: 0052 af00 0000 52b1 0000 0052 b200 0000  .R....R....R....
-00004320: 52b8 0000 0052 bd00 0000 52c0 0000 0052  R....R....R....R
-00004330: c400 0000 52c7 0000 0052 cc00 0000 52d1  ....R....R....R.
-00004340: 0000 0052 d300 0000 52da 0000 0052 de00  ...R....R....R..
-00004350: 0000 2800 0000 0028 0000 0000 2800 0000  ..(....(....(...
-00004360: 0073 4400 0000 2f55 7365 7273 2f61 646d  .sD.../Users/adm
-00004370: 696e 2f57 6f72 6b2f 7072 6f6a 6563 742f  in/Work/project/
-00004380: 4465 7373 696d 6f7a 2f70 7968 616d 2d64  Dessimoz/pyham-d
-00004390: 6576 2f70 7968 616d 2f74 6573 7473 2f74  ev/pyham/tests/t
-000043a0: 6573 745f 6861 6d2e 7079 5263 0000 0081  est_ham.pyRc....
-000043b0: 0000 0073 2000 0000 0602 092f 0927 091d  ...s ....../.'..
-000043c0: 090e 0913 091d 0927 0918 091a 091c 090c  .......'........
-000043d0: 0917 0912 0912 0908 740e 0000 0048 414d  ........t....HAM
-000043e0: 5465 7374 5072 6976 6174 6563 0000 0000  TestPrivatec....
-000043f0: 0000 0000 0100 0000 4200 0000 7311 0000  ........B...s...
-00004400: 0065 0000 5a01 0064 0000 8400 005a 0200  .e..Z..d.....Z..
-00004410: 5253 2801 0000 0063 0100 0000 0700 0000  RS(....c........
-00004420: 0d00 0000 4300 0000 73bb 0100 0074 0000  ....C...s....t..
-00004430: 6a01 006a 0200 7400 006a 0100 6a03 0074  j..j..t..j..j..t
-00004440: 0400 8301 0064 0100 8302 007d 0100 7405  .....d.....}..t.
-00004450: 006a 0600 7c01 0064 0200 6403 0083 0101  .j..|..d..d.....
-00004460: 7d02 0074 0000 6a01 006a 0200 7400 006a  }..t..j..j..t..j
-00004470: 0100 6a03 0074 0400 8301 0064 0100 8302  ..j..t.....d....
-00004480: 007d 0300 7405 006a 0600 7c03 0064 0200  .}..t..j..|..d..
-00004490: 6403 0083 0101 7d04 0074 0000 6a01 006a  d.....}..t..j..j
-000044a0: 0200 7400 006a 0100 6a03 0074 0400 8301  ..t..j..j..t....
-000044b0: 0064 0400 8302 007d 0500 7407 006a 0800  .d.....}..t..j..
-000044c0: 7c02 007c 0500 8302 007c 0000 5f09 0074  |..|.....|.._..t
-000044d0: 0700 6a08 007c 0400 7c05 0083 0200 7c00  ..j..|..|.....|.
-000044e0: 005f 0a00 6405 0064 0600 6407 0064 0800  ._..d..d..d..d..
-000044f0: 6804 007c 0000 5f0b 0064 0900 640a 0064  h..|.._..d..d..d
-00004500: 0b00 640c 0068 0400 7c00 005f 0c00 640d  ..d..h..|.._..d.
-00004510: 0064 0e00 640f 0064 1000 6804 007c 0000  .d..d..d..h..|..
-00004520: 5f0d 0064 0900 6801 007c 0000 5f0e 0064  _..d..h..|.._..d
-00004530: 1100 6412 0068 0200 7c00 005f 0f00 6413  ..d..h..|.._..d.
-00004540: 0064 1400 6415 0064 1600 6417 0064 1800  .d..d..d..d..d..
-00004550: 6419 0064 1a00 641b 0064 1c00 641d 0064  d..d..d..d..d..d
-00004560: 1e00 641f 0068 0d00 7c00 005f 1000 6420  ..d..h..|.._..d 
-00004570: 0064 2100 6422 0064 2300 6424 0064 2500  .d!.d".d#.d$.d%.
-00004580: 6426 0064 2700 6428 0064 2900 642a 0064  d&.d'.d(.d).d*.d
-00004590: 2b00 642c 0068 0d00 7c00 005f 1100 6413  +.d,.h..|.._..d.
-000045a0: 0064 1900 6802 007c 0000 5f12 0074 0700  .d..h..|.._..t..
-000045b0: 6a13 0083 0000 7d06 007c 0600 6a14 0064  j.....}..|..j..d
-000045c0: 2d00 6701 0083 0100 0174 0700 6a08 007c  -.g......t..j..|
-000045d0: 0200 7c05 0064 2e00 7c06 0083 0201 7c00  ..|..d..|.....|.
-000045e0: 005f 1500 6400 0053 282f 0000 004e 7313  ._..d..S(/...Ns.
-000045f0: 0000 002e 2f64 6174 612f 7369 6d70 6c65  ..../data/simple
-00004600: 4578 2e6e 776b 5213 0000 0052 1400 0000  Ex.nwkR....R....
-00004610: 7318 0000 002e 2f64 6174 612f 7369 6d70  s...../data/simp
-00004620: 6c65 4578 2e6f 7274 686f 786d 6c52 4d00  leEx.orthoxmlRM.
-00004630: 0000 524f 0000 0052 6800 0000 5251 0000  ..RO...Rh...RQ..
-00004640: 0052 6900 0000 526a 0000 0052 6b00 0000  .Ri...Rj...Rk...
-00004650: 526c 0000 0052 6d00 0000 526e 0000 0052  Rl...Rm...Rn...R
-00004660: 6f00 0000 5270 0000 0052 4e00 0000 5250  o...Rp...RN...RP
-00004670: 0000 0052 7100 0000 5272 0000 0052 7300  ...Rq...Rr...Rs.
-00004680: 0000 5274 0000 0052 7500 0000 5276 0000  ..Rt...Ru...Rv..
-00004690: 0052 7700 0000 5278 0000 0052 7900 0000  .Rw...Rx...Ry...
-000046a0: 527a 0000 0052 7b00 0000 527c 0000 0052  Rz...R{...R|...R
-000046b0: 7d00 0000 527e 0000 0052 7f00 0000 5280  }...R~...R....R.
-000046c0: 0000 0052 8100 0000 5282 0000 0052 8300  ...R....R....R..
-000046d0: 0000 5284 0000 0052 8500 0000 5286 0000  ..R....R....R...
-000046e0: 0052 8700 0000 5288 0000 0052 8900 0000  .R....R....R....
-000046f0: 528a 0000 0069 0200 0000 523f 0000 0028  R....i....R?...(
-00004700: 1600 0000 5218 0000 0052 1900 0000 521a  ....R....R....R.
-00004710: 0000 0052 1b00 0000 521c 0000 0052 0000  ...R....R....R..
-00004720: 0000 521d 0000 0052 0100 0000 522e 0000  ..R....R....R...
-00004730: 0052 8b00 0000 528c 0000 0052 8e00 0000  .R....R....R....
-00004740: 528f 0000 0052 9000 0000 5291 0000 0052  R....R....R....R
-00004750: 9200 0000 5293 0000 0052 9400 0000 5295  ....R....R....R.
-00004760: 0000 0052 9600 0000 5297 0000 0052 9800  ...R....R....R..
-00004770: 0000 2807 0000 0052 2400 0000 5225 0000  ..(....R$...R%..
-00004780: 0052 1e00 0000 529b 0000 0052 9c00 0000  .R....R....R....
-00004790: 5220 0000 0052 9d00 0000 2800 0000 0028  R ...R....(....(
-000047a0: 0000 0000 7344 0000 002f 5573 6572 732f  ....sD.../Users/
-000047b0: 6164 6d69 6e2f 576f 726b 2f70 726f 6a65  admin/Work/proje
-000047c0: 6374 2f44 6573 7369 6d6f 7a2f 7079 6861  ct/Dessimoz/pyha
-000047d0: 6d2d 6465 762f 7079 6861 6d2f 7465 7374  m-dev/pyham/test
-000047e0: 732f 7465 7374 5f68 616d 2e70 7952 2800  s/test_ham.pyR(.
-000047f0: 0000 1b02 0000 7326 0000 0000 0221 0115  ......s&.....!..
-00004800: 0221 0115 0221 0315 0315 0415 0115 0115  .!...!..........
-00004810: 010c 010f 0130 0115 011b 010f 010c 0110  .....0..........
-00004820: 0128 0300 0000 5249 0000 0052 4a00 0000  .(....RI...RJ...
-00004830: 5228 0000 0028 0000 0000 2800 0000 0028  R(...(....(....(
-00004840: 0000 0000 7344 0000 002f 5573 6572 732f  ....sD.../Users/
-00004850: 6164 6d69 6e2f 576f 726b 2f70 726f 6a65  admin/Work/proje
-00004860: 6374 2f44 6573 7369 6d6f 7a2f 7079 6861  ct/Dessimoz/pyha
-00004870: 6d2d 6465 762f 7079 6861 6d2f 7465 7374  m-dev/pyham/test
-00004880: 732f 7465 7374 5f68 616d 2e70 7952 df00  s/test_ham.pyR..
-00004890: 0000 1902 0000 7302 0000 0006 0274 0800  ......s......t..
-000048a0: 0000 5f5f 6d61 696e 5f5f 280f 0000 0074  ..__main__(....t
-000048b0: 0800 0000 756e 6974 7465 7374 7405 0000  ....unittestt...
-000048c0: 0070 7968 616d 5200 0000 0052 0100 0000  .pyhamR....R....
-000048d0: 5232 0000 0052 1800 0000 520a 0000 0052  R2...R....R....R
-000048e0: 1000 0000 7408 0000 0054 6573 7443 6173  ....t....TestCas
-000048f0: 6552 1100 0000 524b 0000 0052 6300 0000  eR....RK...Rc...
-00004900: 52df 0000 0052 4900 0000 7404 0000 006d  R....RI...t....m
-00004910: 6169 6e28 0000 0000 2800 0000 0028 0000  ain(....(....(..
-00004920: 0000 7344 0000 002f 5573 6572 732f 6164  ..sD.../Users/ad
-00004930: 6d69 6e2f 576f 726b 2f70 726f 6a65 6374  min/Work/project
-00004940: 2f44 6573 7369 6d6f 7a2f 7079 6861 6d2d  /Dessimoz/pyham-
-00004950: 6465 762f 7079 6861 6d2f 7465 7374 732f  dev/pyham/tests/
-00004960: 7465 7374 5f68 616d 2e70 7974 0800 0000  test_ham.pyt....
-00004970: 3c6d 6f64 756c 653e 0100 0000 731a 0000  <module>....s...
-00004980: 000c 0110 0110 010c 010c 0309 0609 0719  ................
-00004990: 4c19 2019 ff00 9919 210c 01              L. .....!..
+000001e0: 0076 2800 0000 0028 0000 0000 7331 0000  .v(....(....s1..
+000001f0: 002f 5573 6572 732f 6164 7269 6161 6c2f  ./Users/adriaal/
+00000200: 5265 706f 7369 746f 7269 6573 2f48 414d  Repositories/HAM
+00000210: 2f74 6573 7473 2f74 6573 745f 6861 6d2e  /tests/test_ham.
+00000220: 7079 7413 0000 005f 7374 725f 6469 6374  pyt...._str_dict
+00000230: 5f6f 6e65 5f76 616c 7565 0800 0000 730a  _one_value....s.
+00000240: 0000 0000 0113 011d 0119 0114 0163 0100  .............c..
+00000250: 0000 0300 0000 0400 0000 4300 0000 7334  ..........C...s4
+00000260: 0000 0067 0000 7d01 0078 2100 7c00 0044  ...g..}..x!.|..D
+00000270: 5d19 007d 0200 7c01 006a 0000 7401 007c  ]..}..|..j..t..|
+00000280: 0200 8301 0083 0100 0171 0d00 5774 0200  .........q..Wt..
+00000290: 7c01 0083 0100 5328 0100 0000 4e28 0300  |.....S(....N(..
+000002a0: 0000 7406 0000 0061 7070 656e 6452 0400  ..t....appendR..
+000002b0: 0000 7403 0000 0073 6574 2803 0000 0074  ..t....set(....t
+000002c0: 0500 0000 6172 7261 7974 0f00 0000 6172  ....arrayt....ar
+000002d0: 7261 795f 636f 6e76 6572 7465 6474 0100  ray_convertedt..
+000002e0: 0000 6528 0000 0000 2800 0000 0073 3100  ..e(....(....s1.
+000002f0: 0000 2f55 7365 7273 2f61 6472 6961 616c  ../Users/adriaal
+00000300: 2f52 6570 6f73 6974 6f72 6965 732f 4841  /Repositories/HA
+00000310: 4d2f 7465 7374 732f 7465 7374 5f68 616d  M/tests/test_ham
+00000320: 2e70 7974 0a00 0000 5f73 7472 5f61 7272  .pyt...._str_arr
+00000330: 6179 0e00 0000 7308 0000 0000 0106 010d  ay....s.........
+00000340: 0117 0174 0c00 0000 4841 4d54 6573 7453  ...t....HAMTestS
+00000350: 6574 5570 6300 0000 0000 0000 0001 0000  etUpc...........
+00000360: 0042 0000 0073 4700 0000 6500 005a 0100  .B...sG...e..Z..
+00000370: 6400 0084 0000 5a02 0064 0100 8400 005a  d.....Z..d.....Z
+00000380: 0300 6402 0084 0000 5a04 0064 0300 8400  ..d.....Z..d....
+00000390: 005a 0500 6404 0084 0000 5a06 0064 0500  .Z..d.....Z..d..
+000003a0: 8400 005a 0700 6406 0084 0000 5a08 0052  ...Z..d.....Z..R
+000003b0: 5328 0700 0000 6301 0000 0004 0000 0006  S(....c.........
+000003c0: 0000 0043 0000 0073 c700 0000 6401 007c  ...C...s....d..|
+000003d0: 0000 5f00 0064 0200 7c00 005f 0100 7402  .._..d..|.._..t.
+000003e0: 006a 0300 6a04 0074 0200 6a03 006a 0500  .j..j..t..j..j..
+000003f0: 7406 0083 0100 6403 0083 0200 7d01 0074  t.....d.....}..t
+00000400: 0700 6a08 007c 0100 6404 0064 0500 8301  ..j..|..d..d....
+00000410: 017c 0000 5f09 0074 0200 6a03 006a 0400  .|.._..t..j..j..
+00000420: 7402 006a 0300 6a05 0074 0600 8301 0064  t..j..j..t.....d
+00000430: 0600 8302 007c 0000 5f0a 0074 0200 6a03  .....|.._..t..j.
+00000440: 006a 0400 7402 006a 0300 6a05 0074 0600  .j..t..j..j..t..
+00000450: 8301 0064 0700 8302 007c 0000 5f0b 0074  ...d.....|.._..t
+00000460: 0c00 7c00 006a 0b00 6408 0083 0200 8f1c  ..|..j..d.......
+00000470: 007d 0200 7c02 006a 0d00 8300 007d 0300  .}..|..j.....}..
+00000480: 7c03 007c 0000 5f0e 0057 6400 0051 5864  |..|.._..Wd..QXd
+00000490: 0000 5328 0900 0000 4e74 0000 0000 7309  ..S(....Nt....s.
+000004a0: 0000 0028 412c 4229 7830 2e34 7313 0000  ...(A,B)x0.4s...
+000004b0: 002e 2f64 6174 612f 7369 6d70 6c65 4578  ../data/simpleEx
+000004c0: 2e6e 776b 7404 0000 0074 7970 6574 0300  .nwkt....typet..
+000004d0: 0000 6e77 6b73 1800 0000 2e2f 6461 7461  ..nwks...../data
+000004e0: 2f73 696d 706c 6545 782e 7068 796c 6f78  /simpleEx.phylox
+000004f0: 6d6c 7318 0000 002e 2f64 6174 612f 7369  mls...../data/si
+00000500: 6d70 6c65 4578 2e6f 7274 686f 786d 6c74  mpleEx.orthoxmlt
+00000510: 0100 0000 7228 0f00 0000 740d 0000 006e  ....r(....t....n
+00000520: 776b 5f73 7472 5f65 6d70 7479 740d 0000  wk_str_emptyt...
+00000530: 006e 776b 5f73 7472 5f77 726f 6e67 7402  .nwk_str_wrongt.
+00000540: 0000 006f 7374 0400 0000 7061 7468 7404  ...ost....patht.
+00000550: 0000 006a 6f69 6e74 0700 0000 6469 726e  ...joint....dirn
+00000560: 616d 6574 0800 0000 5f5f 6669 6c65 5f5f  amet....__file__
+00000570: 5200 0000 0074 1100 0000 6765 745f 6e65  R....t....get_ne
+00000580: 7769 636b 5f73 7472 696e 6774 0700 0000  wick_stringt....
+00000590: 6e77 6b5f 7374 7274 0d00 0000 7068 796c  nwk_strt....phyl
+000005a0: 6f78 6d6c 5f66 696c 6574 0d00 0000 6f72  oxml_filet....or
+000005b0: 7468 6f78 6d6c 5f70 6174 6874 0400 0000  thoxml_patht....
+000005c0: 6f70 656e 7404 0000 0072 6561 6474 0f00  opent....readt..
+000005d0: 0000 6f72 7468 6f78 6d6c 5f73 7472 696e  ..orthoxml_strin
+000005e0: 6728 0400 0000 7404 0000 0073 656c 6674  g(....t....selft
+000005f0: 0800 0000 6e77 6b5f 7061 7468 740d 0000  ....nwk_patht...
+00000600: 006f 7274 686f 786d 6c5f 6669 6c65 7404  .orthoxml_filet.
+00000610: 0000 0064 6174 6128 0000 0000 2800 0000  ...data(....(...
+00000620: 0073 3100 0000 2f55 7365 7273 2f61 6472  .s1.../Users/adr
+00000630: 6961 616c 2f52 6570 6f73 6974 6f72 6965  iaal/Repositorie
+00000640: 732f 4841 4d2f 7465 7374 732f 7465 7374  s/HAM/tests/test
+00000650: 5f68 616d 2e70 7974 0500 0000 7365 7455  _ham.pyt....setU
+00000660: 7017 0000 0073 1200 0000 0001 0901 0901  p....s..........
+00000670: 2101 1802 2402 2402 1501 0c01 6301 0000  !...$.$.....c...
+00000680: 0001 0000 0008 0000 0043 0000 0073 5000  .........C...sP.
+00000690: 0000 7c00 006a 0000 7401 0083 0100 8f15  ..|..j..t.......
+000006a0: 0001 7402 006a 0300 6401 0064 0200 8300  ..t..j..d..d....
+000006b0: 0101 5764 0000 5158 7c00 006a 0000 7401  ..Wd..QX|..j..t.
+000006c0: 0083 0100 8f15 0001 7402 006a 0300 6401  ........t..j..d.
+000006d0: 0064 0300 8300 0101 5764 0000 5158 6400  .d......Wd..QXd.
+000006e0: 0053 2804 0000 004e 740d 0000 0075 7365  .S(....Nt....use
+000006f0: 5f64 6174 615f 6672 6f6d 7403 0000 0078  _data_fromt....x
+00000700: 7878 7403 0000 006f 6d61 2804 0000 0074  xxt....oma(....t
+00000710: 0c00 0000 6173 7365 7274 5261 6973 6573  ....assertRaises
+00000720: 7409 0000 0054 7970 6545 7272 6f72 5201  t....TypeErrorR.
+00000730: 0000 0074 0300 0000 4861 6d28 0100 0000  ...t....Ham(....
+00000740: 5224 0000 0028 0000 0000 2800 0000 0073  R$...(....(....s
+00000750: 3100 0000 2f55 7365 7273 2f61 6472 6961  1.../Users/adria
+00000760: 616c 2f52 6570 6f73 6974 6f72 6965 732f  al/Repositories/
+00000770: 4841 4d2f 7465 7374 732f 7465 7374 5f68  HAM/tests/test_h
+00000780: 616d 2e70 7974 1500 0000 7465 7374 5f6c  am.pyt....test_l
+00000790: 6f61 645f 6672 6f6d 5f73 6572 7665 7225  oad_from_server%
+000007a0: 0000 0073 0800 0000 0003 1001 1603 1001  ...s............
+000007b0: 6301 0000 0001 0000 000a 0000 0043 0000  c............C..
+000007c0: 0073 7a00 0000 7c00 006a 0000 7401 006a  .sz...|..j..t..j
+000007d0: 0200 6a03 006a 0400 8301 008f 2100 0174  ..j..j......!..t
+000007e0: 0500 6a06 007c 0000 6a07 007c 0000 6a08  ..j..|..j..|..j.
+000007f0: 0064 0100 6402 0083 0201 0157 6400 0051  .d..d......Wd..Q
+00000800: 587c 0000 6a00 0074 0100 6a02 006a 0300  X|..j..t..j..j..
+00000810: 6a04 0083 0100 8f21 0001 7405 006a 0600  j......!..t..j..
+00000820: 7c00 006a 0900 7c00 006a 0800 6401 0064  |..j..|..j..d..d
+00000830: 0200 8302 0101 5764 0000 5158 6400 0053  ......Wd..QXd..S
+00000840: 2803 0000 004e 740d 0000 0074 7970 655f  (....Nt....type_
+00000850: 686f 675f 6669 6c65 7408 0000 006f 7274  hog_filet....ort
+00000860: 686f 786d 6c28 0a00 0000 522c 0000 0074  hoxml(....R,...t
+00000870: 0400 0000 6574 6533 7406 0000 0070 6172  ....ete3t....par
+00000880: 7365 7274 0600 0000 6e65 7769 636b 740b  sert....newickt.
+00000890: 0000 004e 6577 6963 6b45 7272 6f72 5201  ...NewickErrorR.
+000008a0: 0000 0052 2e00 0000 5216 0000 0052 2000  ...R....R....R .
+000008b0: 0000 5217 0000 0028 0100 0000 5224 0000  ..R....(....R$..
+000008c0: 0028 0000 0000 2800 0000 0073 3100 0000  .(....(....s1...
+000008d0: 2f55 7365 7273 2f61 6472 6961 616c 2f52  /Users/adriaal/R
+000008e0: 6570 6f73 6974 6f72 6965 732f 4841 4d2f  epositories/HAM/
+000008f0: 7465 7374 732f 7465 7374 5f68 616d 2e70  tests/test_ham.p
+00000900: 7974 1500 0000 7465 7374 5f77 726f 6e67  yt....test_wrong
+00000910: 5f6e 6577 6963 6b5f 7374 723b 0000 0073  _newick_str;...s
+00000920: 0800 0000 0002 1901 2202 1901 6301 0000  ........"...c...
+00000930: 0001 0000 000d 0000 0043 0000 0073 6a00  .........C...sj.
+00000940: 0000 7c00 006a 0000 7401 0083 0100 8f2d  ..|..j..t......-
+00000950: 0001 7402 006a 0300 7c00 006a 0400 7c00  ..t..j..|..j..|.
+00000960: 006a 0500 6401 0064 0200 6403 0064 0400  .j..d..d..d..d..
+00000970: 6405 0064 0600 8302 0301 5764 0000 5158  d..d......Wd..QX
+00000980: 7402 006a 0300 7c00 006a 0400 7c00 006a  t..j..|..j..|..j
+00000990: 0500 6401 0064 0200 6403 0064 0400 6405  ..d..d..d..d..d.
+000009a0: 0064 0700 8302 0301 6400 0053 2808 0000  .d......d..S(...
+000009b0: 004e 5230 0000 0052 3100 0000 740b 0000  .NR0...R1...t...
+000009c0: 0074 7265 655f 666f 726d 6174 7408 0000  .tree_formatt...
+000009d0: 0070 6879 6c6f 786d 6c74 1600 0000 7068  .phyloxmlt....ph
+000009e0: 796c 6f78 6d6c 5f6c 6561 665f 6e61 6d65  yloxml_leaf_name
+000009f0: 5f74 6167 7404 0000 004e 6f6e 6574 0a00  _tagt....Nonet..
+00000a00: 0000 636c 6164 655f 6e61 6d65 2806 0000  ..clade_name(...
+00000a10: 0052 2c00 0000 522d 0000 0052 0100 0000  .R,...R-...R....
+00000a20: 522e 0000 0052 1f00 0000 5220 0000 0028  R....R....R ...(
+00000a30: 0100 0000 5224 0000 0028 0000 0000 2800  ....R$...(....(.
+00000a40: 0000 0073 3100 0000 2f55 7365 7273 2f61  ...s1.../Users/a
+00000a50: 6472 6961 616c 2f52 6570 6f73 6974 6f72  driaal/Repositor
+00000a60: 6965 732f 4841 4d2f 7465 7374 732f 7465  ies/HAM/tests/te
+00000a70: 7374 5f68 616d 2e70 7974 1100 0000 7465  st_ham.pyt....te
+00000a80: 7374 5f70 6879 6c6f 786d 6c5f 7461 6743  st_phyloxml_tagC
+00000a90: 0000 0073 0600 0000 0002 1001 2e02 6301  ...s..........c.
+00000aa0: 0000 0001 0000 000b 0000 0043 0000 0073  ...........C...s
+00000ab0: 9a00 0000 7c00 006a 0000 7401 0083 0100  ....|..j..t.....
+00000ac0: 8f21 0001 7402 006a 0300 7c00 006a 0400  .!..t..j..|..j..
+00000ad0: 7c00 006a 0500 6401 0064 0200 8302 0101  |..j..d..d......
+00000ae0: 5764 0000 5158 7c00 006a 0000 7401 0083  Wd..QX|..j..t...
+00000af0: 0100 8f21 0001 7402 006a 0300 7c00 006a  ...!..t..j..|..j
+00000b00: 0400 7c00 006a 0500 6401 0064 0300 8302  ..|..j..d..d....
+00000b10: 0101 5764 0000 5158 7c00 006a 0000 7401  ..Wd..QX|..j..t.
+00000b20: 0083 0100 8f21 0001 7402 006a 0300 7c00  .....!..t..j..|.
+00000b30: 006a 0400 7c00 006a 0500 6401 0064 0000  .j..|..j..d..d..
+00000b40: 8302 0101 5764 0000 5158 6400 0053 2804  ....Wd..QXd..S(.
+00000b50: 0000 004e 5230 0000 0074 0200 0000 7873  ...NR0...t....xs
+00000b60: 5212 0000 0028 0700 0000 522c 0000 0052  R....(....R,...R
+00000b70: 2d00 0000 5201 0000 0052 2e00 0000 521e  -...R....R....R.
+00000b80: 0000 0052 2000 0000 523a 0000 0028 0100  ...R ...R:...(..
+00000b90: 0000 5224 0000 0028 0000 0000 2800 0000  ..R$...(....(...
+00000ba0: 0073 3100 0000 2f55 7365 7273 2f61 6472  .s1.../Users/adr
+00000bb0: 6961 616c 2f52 6570 6f73 6974 6f72 6965  iaal/Repositorie
+00000bc0: 732f 4841 4d2f 7465 7374 732f 7465 7374  s/HAM/tests/test
+00000bd0: 5f68 616d 2e70 7974 1800 0000 7465 7374  _ham.pyt....test
+00000be0: 5f77 726f 6e67 5f74 7970 655f 686f 675f  _wrong_type_hog_
+00000bf0: 6669 6c65 4a00 0000 730c 0000 0000 0210  fileJ...s.......
+00000c00: 0122 0210 0122 0210 0163 0100 0000 0100  ."..."...c......
+00000c10: 0000 0900 0000 4300 0000 7336 0000 007c  ......C...s6...|
+00000c20: 0000 6a00 0074 0100 8301 008f 2100 0174  ..j..t......!..t
+00000c30: 0200 6a03 007c 0000 6a04 007c 0000 6a05  ..j..|..j..|..j.
+00000c40: 0064 0100 6402 0083 0201 0157 6400 0051  .d..d......Wd..Q
+00000c50: 5864 0000 5328 0300 0000 4e74 0d00 0000  Xd..S(....Nt....
+00000c60: 6669 6c74 6572 5f6f 626a 6563 7474 0100  filter_objectt..
+00000c70: 0000 7828 0600 0000 522c 0000 0052 2d00  ..x(....R,...R-.
+00000c80: 0000 5201 0000 0052 2e00 0000 521e 0000  ..R....R....R...
+00000c90: 0052 2000 0000 2801 0000 0052 2400 0000  .R ...(....R$...
+00000ca0: 2800 0000 0028 0000 0000 7331 0000 002f  (....(....s1.../
+00000cb0: 5573 6572 732f 6164 7269 6161 6c2f 5265  Users/adriaal/Re
+00000cc0: 706f 7369 746f 7269 6573 2f48 414d 2f74  positories/HAM/t
+00000cd0: 6573 7473 2f74 6573 745f 6861 6d2e 7079  ests/test_ham.py
+00000ce0: 7411 0000 0074 6573 745f 7772 6f6e 675f  t....test_wrong_
+00000cf0: 6669 6c74 6572 5500 0000 7304 0000 0000  filterU...s.....
+00000d00: 0110 0163 0100 0000 0100 0000 0b00 0000  ...c............
+00000d10: 4300 0000 736e 0000 0074 0000 6a01 0064  C...sn...t..j..d
+00000d20: 0100 7c00 006a 0200 6402 007c 0000 6a03  ..|..j..d..|..j.
+00000d30: 0064 0300 6404 0064 0500 7404 0083 0004  .d..d..d..t.....
+00000d40: 7c00 005f 0500 7c00 006a 0600 7407 0083  |.._..|..j..t...
+00000d50: 0100 8f2c 0001 7400 006a 0100 6401 007c  ...,..t..j..d..|
+00000d60: 0000 6a02 0064 0200 7c00 006a 0300 6403  ..j..d..|..j..d.
+00000d70: 0064 0400 8300 037c 0000 5f05 0057 6400  .d.....|.._..Wd.
+00000d80: 0051 5864 0000 5328 0600 0000 4e74 0900  .QXd..S(....Nt..
+00000d90: 0000 7472 6565 5f66 696c 6574 0800 0000  ..tree_filet....
+00000da0: 686f 675f 6669 6c65 5230 0000 0052 3100  hog_fileR0...R1.
+00000db0: 0000 7412 0000 006f 7274 686f 584d 4c5f  ..t....orthoXML_
+00000dc0: 6173 5f73 7472 696e 6728 0800 0000 5201  as_string(....R.
+00000dd0: 0000 0052 2e00 0000 521e 0000 0052 2300  ...R....R....R#.
+00000de0: 0000 7404 0000 0054 7275 6574 0c00 0000  ..t....Truet....
+00000df0: 6861 6d5f 616e 616c 7973 6973 522c 0000  ham_analysisR,..
+00000e00: 0074 0700 0000 494f 4572 726f 7228 0100  .t....IOError(..
+00000e10: 0000 5224 0000 0028 0000 0000 2800 0000  ..R$...(....(...
+00000e20: 0073 3100 0000 2f55 7365 7273 2f61 6472  .s1.../Users/adr
+00000e30: 6961 616c 2f52 6570 6f73 6974 6f72 6965  iaal/Repositorie
+00000e40: 732f 4841 4d2f 7465 7374 732f 7465 7374  s/HAM/tests/test
+00000e50: 5f68 616d 2e70 7974 1700 0000 7465 7374  _ham.pyt....test
+00000e60: 5f6f 7274 686f 786d 6c5f 6173 5f73 7472  _orthoxml_as_str
+00000e70: 696e 6759 0000 0073 0600 0000 0002 2d02  ingY...s......-.
+00000e80: 1001 2809 0000 0074 0800 0000 5f5f 6e61  ..(....t....__na
+00000e90: 6d65 5f5f 740a 0000 005f 5f6d 6f64 756c  me__t....__modul
+00000ea0: 655f 5f52 2800 0000 522f 0000 0052 3600  e__R(...R/...R6.
+00000eb0: 0000 523c 0000 0052 3e00 0000 5241 0000  ..R<...R>...RA..
+00000ec0: 0052 4800 0000 2800 0000 0028 0000 0000  .RH...(....(....
+00000ed0: 2800 0000 0073 3100 0000 2f55 7365 7273  (....s1.../Users
+00000ee0: 2f61 6472 6961 616c 2f52 6570 6f73 6974  /adriaal/Reposit
+00000ef0: 6f72 6965 732f 4841 4d2f 7465 7374 732f  ories/HAM/tests/
+00000f00: 7465 7374 5f68 616d 2e70 7952 1100 0000  test_ham.pyR....
+00000f10: 1500 0000 730e 0000 0006 0209 0e09 1609  ....s...........
+00000f20: 0809 0709 0b09 0474 0700 0000 4841 4d54  .......t....HAMT
+00000f30: 6573 7463 0000 0000 0000 0000 0100 0000  estc............
+00000f40: 4200 0000 7323 0000 0065 0000 5a01 0064  B...s#...e..Z..d
+00000f50: 0000 8400 005a 0200 6401 0084 0000 5a03  .....Z..d.....Z.
+00000f60: 0064 0200 8400 005a 0400 5253 2803 0000  .d.....Z..RS(...
+00000f70: 0063 0100 0000 0400 0000 0700 0000 4300  .c............C.
+00000f80: 0000 7339 0100 0074 0000 6a01 006a 0200  ..s9...t..j..j..
+00000f90: 7400 006a 0100 6a03 0074 0400 8301 0064  t..j..j..t.....d
+00000fa0: 0100 8302 007d 0100 7405 006a 0600 7c01  .....}..t..j..|.
+00000fb0: 0064 0200 6403 0083 0101 7d02 0074 0000  .d..d.....}..t..
+00000fc0: 6a01 006a 0200 7400 006a 0100 6a03 0074  j..j..t..j..j..t
+00000fd0: 0400 8301 0064 0400 8302 007d 0300 7407  .....d.....}..t.
+00000fe0: 006a 0800 6405 007c 0200 6406 007c 0300  .j..d..|..d..|..
+00000ff0: 6407 0064 0800 8300 037c 0000 5f09 007c  d..d.....|.._..|
+00001000: 0000 6a09 006a 0a00 8300 007c 0000 5f0b  ..j..j.....|.._.
+00001010: 007c 0000 6a09 006a 0c00 8300 007c 0000  .|..j..j.....|..
+00001020: 5f0d 007c 0000 6a09 006a 0e00 6409 0064  _..|..j..j..d..d
+00001030: 0a00 8300 017c 0000 5f0f 007c 0000 6a09  .....|.._..|..j.
+00001040: 006a 0e00 6409 0064 0b00 8300 017c 0000  .j..d..d.....|..
+00001050: 5f10 007c 0000 6a09 006a 0e00 6409 0064  _..|..j..j..d..d
+00001060: 0c00 8300 017c 0000 5f11 007c 0000 6a09  .....|.._..|..j.
+00001070: 006a 0e00 6409 0064 0d00 8300 017c 0000  .j..d..d.....|..
+00001080: 5f12 007c 0000 6a09 006a 0e00 6409 0064  _..|..j..j..d..d
+00001090: 0e00 8300 017c 0000 5f13 007c 0000 6a09  .....|.._..|..j.
+000010a0: 006a 1400 7c00 006a 0f00 7c00 006a 1000  .j..|..j..|..j..
+000010b0: 6802 0083 0100 7c00 005f 1500 6400 0053  h.....|.._..d..S
+000010c0: 280f 0000 004e 7313 0000 002e 2f64 6174  (....Ns...../dat
+000010d0: 612f 7369 6d70 6c65 4578 2e6e 776b 5213  a/simpleEx.nwkR.
+000010e0: 0000 0052 1400 0000 7318 0000 002e 2f64  ...R....s...../d
+000010f0: 6174 612f 7369 6d70 6c65 4578 2e6f 7274  ata/simpleEx.ort
+00001100: 686f 786d 6c52 4200 0000 5243 0000 0052  hoxmlRB...RC...R
+00001110: 3000 0000 5231 0000 0074 0400 0000 6e61  0...R1...t....na
+00001120: 6d65 7405 0000 0048 554d 414e 7405 0000  met....HUMANt...
+00001130: 0058 454e 5452 7405 0000 004d 4f55 5345  .XENTRt....MOUSE
+00001140: 7405 0000 0052 4154 4e4f 7405 0000 0050  t....RATNOt....P
+00001150: 414e 5452 2816 0000 0052 1800 0000 5219  ANTR(....R....R.
+00001160: 0000 0052 1a00 0000 521b 0000 0052 1c00  ...R....R....R..
+00001170: 0000 5200 0000 0052 1d00 0000 5201 0000  ..R....R....R...
+00001180: 0052 2e00 0000 5246 0000 0074 1700 0000  .R....RF...t....
+00001190: 6765 745f 6469 6374 5f74 6f70 5f6c 6576  get_dict_top_lev
+000011a0: 656c 5f68 6f67 7374 0400 0000 686f 6773  el_hogst....hogs
+000011b0: 7415 0000 0067 6574 5f64 6963 745f 6578  t....get_dict_ex
+000011c0: 7461 6e74 5f67 656e 6573 7405 0000 0067  tant_genest....g
+000011d0: 656e 6573 7419 0000 0067 6574 5f65 7874  enest....get_ext
+000011e0: 616e 745f 6765 6e6f 6d65 5f62 795f 6e61  ant_genome_by_na
+000011f0: 6d65 7405 0000 0068 756d 616e 7404 0000  met....humant...
+00001200: 0066 726f 6774 0500 0000 6d6f 7573 6574  .frogt....mouset
+00001210: 0300 0000 7261 7474 0500 0000 6368 696d  ....ratt....chim
+00001220: 7074 2a00 0000 6765 745f 616e 6365 7374  pt*...get_ancest
+00001230: 7261 6c5f 6765 6e6f 6d65 5f62 795f 6d72  ral_genome_by_mr
+00001240: 6361 5f6f 665f 6765 6e6f 6d65 5f73 6574  ca_of_genome_set
+00001250: 740b 0000 0076 6572 7465 6272 6174 6573  t....vertebrates
+00001260: 2804 0000 0052 2400 0000 5225 0000 0074  (....R$...R%...t
+00001270: 0800 0000 7472 6565 5f73 7472 5220 0000  ....tree_strR ..
+00001280: 0028 0000 0000 2800 0000 0073 3100 0000  .(....(....s1...
+00001290: 2f55 7365 7273 2f61 6472 6961 616c 2f52  /Users/adriaal/R
+000012a0: 6570 6f73 6974 6f72 6965 732f 4841 4d2f  epositories/HAM/
+000012b0: 7465 7374 732f 7465 7374 5f68 616d 2e70  tests/test_ham.p
+000012c0: 7952 2800 0000 6300 0000 7318 0000 0000  yR(...c...s.....
+000012d0: 0121 0115 0221 0221 0112 0112 0218 0118  .!...!.!........
+000012e0: 0118 0118 0118 0163 0100 0000 0100 0000  .......c........
+000012f0: 0700 0000 4300 0000 7330 0000 007c 0000  ....C...s0...|..
+00001300: 6a00 0074 0100 8301 008f 1b00 017c 0000  j..t.........|..
+00001310: 6a02 006a 0300 6400 007c 0000 6a05 0083  j..j..d..|..j...
+00001320: 0200 0157 6400 0051 5864 0000 5328 0100  ...Wd..QXd..S(..
+00001330: 0000 4e28 0600 0000 522c 0000 0052 2d00  ..N(....R,...R-.
+00001340: 0000 5246 0000 0074 1a00 0000 636f 6d70  ..RF...t....comp
+00001350: 6172 655f 6765 6e6f 6d65 735f 7665 7274  are_genomes_vert
+00001360: 6963 616c 6c79 523a 0000 0052 5b00 0000  icallyR:...R[...
+00001370: 2801 0000 0052 2400 0000 2800 0000 0028  (....R$...(....(
+00001380: 0000 0000 7331 0000 002f 5573 6572 732f  ....s1.../Users/
+00001390: 6164 7269 6161 6c2f 5265 706f 7369 746f  adriaal/Reposito
+000013a0: 7269 6573 2f48 414d 2f74 6573 7473 2f74  ries/HAM/tests/t
+000013b0: 6573 745f 6861 6d2e 7079 7429 0000 0074  est_ham.pyt)...t
+000013c0: 6573 745f 636f 6d70 6172 655f 6c65 7665  est_compare_leve
+000013d0: 6c5f 636f 7272 6563 745f 696e 7075 745f  l_correct_input_
+000013e0: 7665 7274 6963 616c 7400 0000 7304 0000  verticalt...s...
+000013f0: 0000 0310 0163 0100 0000 0100 0000 0700  .....c..........
+00001400: 0000 4300 0000 7330 0000 007c 0000 6a00  ..C...s0...|..j.
+00001410: 0074 0100 8301 008f 1b00 017c 0000 6a02  .t.........|..j.
+00001420: 006a 0300 6400 007c 0000 6a05 0083 0200  .j..d..|..j.....
+00001430: 0157 6400 0051 5864 0000 5328 0100 0000  .Wd..QXd..S(....
+00001440: 4e28 0600 0000 522c 0000 0052 2d00 0000  N(....R,...R-...
+00001450: 5246 0000 0074 1700 0000 636f 6d70 6172  RF...t....compar
+00001460: 655f 6765 6e6f 6d65 735f 6c61 7465 7261  e_genomes_latera
+00001470: 6c52 3a00 0000 525b 0000 0028 0100 0000  lR:...R[...(....
+00001480: 5224 0000 0028 0000 0000 2800 0000 0073  R$...(....(....s
+00001490: 3100 0000 2f55 7365 7273 2f61 6472 6961  1.../Users/adria
+000014a0: 616c 2f52 6570 6f73 6974 6f72 6965 732f  al/Repositories/
+000014b0: 4841 4d2f 7465 7374 732f 7465 7374 5f68  HAM/tests/test_h
+000014c0: 616d 2e70 7974 2800 0000 7465 7374 5f63  am.pyt(...test_c
+000014d0: 6f6d 7061 7265 5f6c 6576 656c 5f63 6f72  ompare_level_cor
+000014e0: 7265 6374 5f69 6e70 7574 5f6c 6174 6572  rect_input_later
+000014f0: 616c 7a00 0000 7304 0000 0000 0310 0128  alz...s........(
+00001500: 0500 0000 5249 0000 0052 4a00 0000 5228  ....RI...RJ...R(
+00001510: 0000 0052 6000 0000 5262 0000 0028 0000  ...R`...Rb...(..
+00001520: 0000 2800 0000 0028 0000 0000 7331 0000  ..(....(....s1..
+00001530: 002f 5573 6572 732f 6164 7269 6161 6c2f  ./Users/adriaal/
+00001540: 5265 706f 7369 746f 7269 6573 2f48 414d  Repositories/HAM
+00001550: 2f74 6573 7473 2f74 6573 745f 6861 6d2e  /tests/test_ham.
+00001560: 7079 524b 0000 0061 0000 0073 0600 0000  pyRK...a...s....
+00001570: 0602 0911 0906 740c 0000 0048 414d 5465  ......t....HAMTe
+00001580: 7374 5175 6572 7963 0000 0000 0000 0000  stQueryc........
+00001590: 0100 0000 4200 0000 7398 0000 0065 0000  ....B...s....e..
+000015a0: 5a01 0064 0000 8400 005a 0200 6401 0084  Z..d.....Z..d...
+000015b0: 0000 5a03 0064 0200 8400 005a 0400 6403  ..Z..d.....Z..d.
+000015c0: 0084 0000 5a05 0064 0400 8400 005a 0600  ....Z..d.....Z..
+000015d0: 6405 0084 0000 5a07 0064 0600 8400 005a  d.....Z..d.....Z
+000015e0: 0800 6407 0084 0000 5a09 0064 0800 8400  ..d.....Z..d....
+000015f0: 005a 0a00 6409 0084 0000 5a0b 0064 0a00  .Z..d.....Z..d..
+00001600: 8400 005a 0c00 640b 0084 0000 5a0d 0064  ...Z..d.....Z..d
+00001610: 0c00 8400 005a 0e00 640d 0084 0000 5a0f  .....Z..d.....Z.
+00001620: 0064 0e00 8400 005a 1000 640f 0084 0000  .d.....Z..d.....
+00001630: 5a11 0052 5328 1000 0000 6301 0000 000a  Z..RS(....c.....
+00001640: 0000 000e 0000 0043 0000 0073 9002 0000  .......C...s....
+00001650: 7400 006a 0100 6a02 0074 0000 6a01 006a  t..j..j..t..j..j
+00001660: 0300 7404 0083 0100 6401 0083 0200 7d01  ..t.....d.....}.
+00001670: 0074 0500 6a06 007c 0100 6402 0064 0300  .t..j..|..d..d..
+00001680: 8301 017d 0200 7400 006a 0100 6a02 0074  ...}..t..j..j..t
+00001690: 0000 6a01 006a 0300 7404 0083 0100 6401  ..j..j..t.....d.
+000016a0: 0083 0200 7d03 0074 0500 6a06 007c 0300  ....}..t..j..|..
+000016b0: 6402 0064 0300 8301 017d 0400 7400 006a  d..d.....}..t..j
+000016c0: 0100 6a02 0074 0000 6a01 006a 0300 7404  ..j..t..j..j..t.
+000016d0: 0083 0100 6404 0083 0200 7d05 0074 0000  ....d.....}..t..
+000016e0: 6a01 006a 0200 7400 006a 0100 6a03 0074  j..j..t..j..j..t
+000016f0: 0400 8301 0064 0500 8302 007d 0600 7407  .....d.....}..t.
+00001700: 007c 0600 6406 0083 0200 8f1c 007d 0700  .|..d........}..
+00001710: 7c07 006a 0800 8300 007d 0800 7c08 007c  |..j.....}..|..|
+00001720: 0000 5f09 0057 6400 0051 5874 0a00 6a0b  .._..Wd..QXt..j.
+00001730: 007c 0200 7c06 0064 0700 740c 0083 0201  .|..|..d..t.....
+00001740: 7c00 005f 0d00 740a 006a 0b00 7c04 007c  |.._..t..j..|..|
+00001750: 0600 8302 007c 0000 5f0e 0074 0a00 6a0b  .....|.._..t..j.
+00001760: 007c 0500 7c06 0064 0700 740c 0064 0800  .|..|..d..t..d..
+00001770: 6409 0064 0a00 640b 0064 0c00 640d 0083  d..d..d..d..d...
+00001780: 0204 7c00 005f 0f00 640e 0064 0f00 6410  ..|.._..d..d..d.
+00001790: 0064 1100 6804 007c 0000 5f10 0064 1200  .d..h..|.._..d..
+000017a0: 6413 0064 1400 6415 0068 0400 7c00 005f  d..d..d..h..|.._
+000017b0: 1100 6416 0064 1700 6418 0064 1900 6804  ..d..d..d..d..h.
+000017c0: 007c 0000 5f12 0064 1200 6801 007c 0000  .|.._..d..h..|..
+000017d0: 5f13 0064 1a00 641b 0068 0200 7c00 005f  _..d..d..h..|.._
+000017e0: 1400 641c 0064 1d00 641e 0064 1f00 6420  ..d..d..d..d..d 
+000017f0: 0064 2100 6422 0064 2300 6424 0064 2500  .d!.d".d#.d$.d%.
+00001800: 6426 0064 2700 6428 0068 0d00 7c00 005f  d&.d'.d(.h..|.._
+00001810: 1500 6429 0064 2a00 642b 0064 2c00 642d  ..d).d*.d+.d,.d-
+00001820: 0064 2e00 642f 0064 3000 6431 0064 3200  .d..d/.d0.d1.d2.
+00001830: 6433 0064 3400 6435 0068 0d00 7c00 005f  d3.d4.d5.h..|.._
+00001840: 1600 641c 0064 2200 6802 007c 0000 5f17  ..d..d".h..|.._.
+00001850: 0074 0a00 6a18 0083 0000 7d09 007c 0900  .t..j.....}..|..
+00001860: 6a19 0064 3600 6701 0083 0100 0174 0a00  j..d6.g......t..
+00001870: 6a0b 007c 0200 7c06 0064 3700 7c09 0064  j..|..|..d7.|..d
+00001880: 0700 740c 0083 0202 7c00 005f 1a00 740a  ..t.....|.._..t.
+00001890: 006a 0b00 7c02 007c 0000 6a09 0064 0700  .j..|..|..j..d..
+000018a0: 740c 0064 3800 740c 0083 0202 7c00 005f  t..d8.t.....|.._
+000018b0: 1b00 740a 006a 0b00 7c02 007c 0000 6a09  ..t..j..|..|..j.
+000018c0: 0064 3700 7c09 0064 0700 740c 0064 3800  .d7.|..d..t..d8.
+000018d0: 740c 0083 0203 7c00 005f 1c00 6400 0053  t.....|.._..d..S
+000018e0: 2839 0000 004e 7313 0000 002e 2f64 6174  (9...Ns...../dat
+000018f0: 612f 7369 6d70 6c65 4578 2e6e 776b 5213  a/simpleEx.nwkR.
+00001900: 0000 0052 1400 0000 7318 0000 002e 2f64  ...R....s...../d
+00001910: 6174 612f 7369 6d70 6c65 4578 2e70 6879  ata/simpleEx.phy
+00001920: 6c6f 786d 6c73 1800 0000 2e2f 6461 7461  loxmls...../data
+00001930: 2f73 696d 706c 6545 782e 6f72 7468 6f78  /simpleEx.orthox
+00001940: 6d6c 5215 0000 0074 1100 0000 7573 655f  mlR....t....use_
+00001950: 696e 7465 726e 616c 5f6e 616d 6552 3700  internal_nameR7.
+00001960: 0000 5238 0000 0074 1a00 0000 7068 796c  ..R8...t....phyl
+00001970: 6f78 6d6c 5f69 6e74 6572 6e61 6c5f 6e61  oxml_internal_na
+00001980: 6d65 5f74 6167 7418 0000 0074 6178 6f6e  me_tagt....taxon
+00001990: 6f6d 795f 7363 6965 6e74 6966 6963 5f6e  omy_scientific_n
+000019a0: 616d 6552 3900 0000 740d 0000 0074 6178  ameR9...t....tax
+000019b0: 6f6e 6f6d 795f 636f 6465 524d 0000 0052  onomy_codeRM...R
+000019c0: 4f00 0000 7405 0000 0043 414e 4641 5251  O...t....CANFARQ
+000019d0: 0000 0074 0100 0000 3274 0200 0000 3332  ...t....2t....32
+000019e0: 7402 0000 0032 3274 0200 0000 3132 7406  t....22t....12t.
+000019f0: 0000 0048 554d 414e 3274 0600 0000 4d4f  ...HUMAN2t....MO
+00001a00: 5553 4532 7406 0000 0043 414e 4641 3274  USE2t....CANFA2t
+00001a10: 0600 0000 5041 4e54 5232 524e 0000 0052  ....PANTR2RN...R
+00001a20: 5000 0000 7401 0000 0031 7402 0000 0031  P...t....1t....1
+00001a30: 3174 0200 0000 3231 7402 0000 0033 3174  1t....21t....31t
+00001a40: 0200 0000 3431 7402 0000 0035 3174 0100  ....41t....51t..
+00001a50: 0000 3374 0200 0000 3133 7402 0000 0032  ..3t....13t....2
+00001a60: 3374 0200 0000 3333 7402 0000 0035 3374  3t....33t....53t
+00001a70: 0200 0000 3334 7402 0000 0031 3474 0600  ....34t....14t..
+00001a80: 0000 4855 4d41 4e31 7406 0000 0050 414e  ..HUMAN1t....PAN
+00001a90: 5452 3174 0600 0000 4341 4e46 4131 7406  TR1t....CANFA1t.
+00001aa0: 0000 004d 4f55 5345 3174 0600 0000 5241  ...MOUSE1t....RA
+00001ab0: 544e 4f31 7406 0000 0058 454e 5452 3174  TNO1t....XENTR1t
+00001ac0: 0600 0000 4855 4d41 4e33 7406 0000 0050  ....HUMAN3t....P
+00001ad0: 414e 5452 3374 0600 0000 4341 4e46 4133  ANTR3t....CANFA3
+00001ae0: 7406 0000 004d 4f55 5345 3374 0600 0000  t....MOUSE3t....
+00001af0: 5845 4e54 5233 7406 0000 004d 4f55 5345  XENTR3t....MOUSE
+00001b00: 3474 0600 0000 5041 4e54 5234 6902 0000  4t....PANTR4i...
+00001b10: 0052 3f00 0000 5244 0000 0028 1d00 0000  .R?...RD...(....
+00001b20: 5218 0000 0052 1900 0000 521a 0000 0052  R....R....R....R
+00001b30: 1b00 0000 521c 0000 0052 0000 0000 521d  ....R....R....R.
+00001b40: 0000 0052 2100 0000 5222 0000 0052 2300  ...R!...R"...R#.
+00001b50: 0000 5201 0000 0052 2e00 0000 5245 0000  ..R....R....RE..
+00001b60: 0074 0100 0000 6874 0200 0000 686e 7403  .t....ht....hnt.
+00001b70: 0000 0068 7078 740d 0000 0066 696c 7465  ...hpxt....filte
+00001b80: 725f 6765 6e6f 6d65 740c 0000 0066 696c  r_genomet....fil
+00001b90: 7465 725f 6765 6e65 7374 1000 0000 6669  ter_genest....fi
+00001ba0: 6c74 6572 5f67 656e 6573 5f65 7874 740b  lter_genes_extt.
+00001bb0: 0000 0066 696c 7465 725f 686f 6773 7410  ...filter_hogst.
+00001bc0: 0000 006e 6f5f 6669 6c74 6572 5f67 656e  ...no_filter_gen
+00001bd0: 6f6d 6574 0f00 0000 6e6f 5f66 696c 7465  omet....no_filte
+00001be0: 725f 6765 6e65 7374 1300 0000 6e6f 5f66  r_genest....no_f
+00001bf0: 696c 7465 725f 6765 6e65 735f 6578 7474  ilter_genes_extt
+00001c00: 0e00 0000 6e6f 5f66 696c 7465 725f 686f  ....no_filter_ho
+00001c10: 6773 740c 0000 0050 6172 7365 7246 696c  gst....ParserFil
+00001c20: 7465 7274 1200 0000 6164 645f 686f 6773  tert....add_hogs
+00001c30: 5f76 6961 5f68 6f67 4964 7402 0000 0068  _via_hogIdt....h
+00001c40: 6674 0700 0000 6873 7472 696e 6774 0800  ft....hstringt..
+00001c50: 0000 6866 7374 7269 6e67 280a 0000 0052  ..hfstring(....R
+00001c60: 2400 0000 5225 0000 0052 1e00 0000 7410  $...R%...R....t.
+00001c70: 0000 006e 776b 5f70 6174 685f 6e6f 5f6e  ...nwk_path_no_n
+00001c80: 616d 6574 0f00 0000 6e77 6b5f 7374 725f  amet....nwk_str_
+00001c90: 6e6f 5f6e 616d 6552 1f00 0000 5220 0000  no_nameR....R ..
+00001ca0: 0052 2600 0000 5227 0000 0074 0100 0000  .R&...R'...t....
+00001cb0: 6628 0000 0000 2800 0000 0073 3100 0000  f(....(....s1...
+00001cc0: 2f55 7365 7273 2f61 6472 6961 616c 2f52  /Users/adriaal/R
+00001cd0: 6570 6f73 6974 6f72 6965 732f 4841 4d2f  epositories/HAM/
+00001ce0: 7465 7374 732f 7465 7374 5f68 616d 2e70  tests/test_ham.p
+00001cf0: 7952 2800 0000 8300 0000 7336 0000 0000  yR(.......s6....
+00001d00: 0121 0115 0221 0115 0221 0221 0212 010c  .!...!...!.!....
+00001d10: 010f 031b 0315 032d 0315 0115 0115 010c  .......-........
+00001d20: 010f 0130 0115 011b 010f 010c 0110 0121  ...0...........!
+00001d30: 0318 010c 0363 0100 0000 0400 0000 0900  .....c..........
+00001d40: 0000 4300 0000 73a0 0100 007c 0000 6a00  ..C...s....|..j.
+00001d50: 0074 0100 8301 008f 1500 017c 0000 6a02  .t.........|..j.
+00001d60: 006a 0300 6401 0083 0100 0157 6400 0051  .j..d......Wd..Q
+00001d70: 587c 0000 6a02 006a 0300 6402 0083 0100  X|..j..j..d.....
+00001d80: 7d01 007c 0000 6a04 0074 0500 7c01 0083  }..|..j..t..|...
+00001d90: 0100 6403 0083 0200 017c 0000 6a02 006a  ..d......|..j..j
+00001da0: 0300 6404 0083 0100 7d01 007c 0000 6a04  ..d.....}..|..j.
+00001db0: 0074 0500 7c01 0083 0100 6403 0083 0200  .t..|.....d.....
+00001dc0: 017c 0000 6a06 006a 0300 6404 0083 0100  .|..j..j..d.....
+00001dd0: 7d01 007c 0000 6a04 0074 0500 7c01 0083  }..|..j..t..|...
+00001de0: 0100 6403 0083 0200 017c 0000 6a07 006a  ..d......|..j..j
+00001df0: 0300 6404 0083 0100 7d01 007c 0000 6a04  ..d.....}..|..j.
+00001e00: 0074 0500 7c01 0083 0100 6403 0083 0200  .t..|.....d.....
+00001e10: 0178 7300 7c00 006a 0800 445d 6800 7d02  .xs.|..j..D]h.}.
+00001e20: 007c 0000 6a09 006a 0300 7c02 0083 0100  .|..j..j..|.....
+00001e30: 7d03 007c 0000 6a04 0074 0500 7c03 0083  }..|..j..t..|...
+00001e40: 0100 6405 006a 0a00 7c02 0083 0100 8302  ..d..j..|.......
+00001e50: 0001 7c00 006a 0b00 6a03 007c 0200 8301  ..|..j..j..|....
+00001e60: 007d 0300 7c00 006a 0400 7405 007c 0300  .}..|..j..t..|..
+00001e70: 8301 0064 0500 6a0a 007c 0200 8301 0083  ...d..j..|......
+00001e80: 0200 0171 d000 5778 5d00 7c00 006a 0c00  ...q..Wx].|..j..
+00001e90: 445d 5200 7d02 007c 0000 6a00 0074 0100  D]R.}..|..j..t..
+00001ea0: 8301 008f 1500 017c 0000 6a09 006a 0300  .......|..j..j..
+00001eb0: 7c02 0083 0100 0157 6400 0051 587c 0000  |......Wd..QX|..
+00001ec0: 6a00 0074 0100 8301 008f 1500 017c 0000  j..t.........|..
+00001ed0: 6a0b 006a 0300 7c02 0083 0100 0157 6400  j..j..|......Wd.
+00001ee0: 0051 5871 4601 5764 0000 5328 0600 0000  .QXqF.Wd..S(....
+00001ef0: 4e74 0100 0000 6452 7700 0000 7308 0000  Nt....dRw...s...
+00001f00: 003c 484f 4728 3329 3e69 0300 0000 7309  .<HOG(3)>i....s.
+00001f10: 0000 003c 484f 4728 7b7d 293e 280d 0000  ...<HOG({})>(...
+00001f20: 0052 2c00 0000 7408 0000 004b 6579 4572  .R,...t....KeyEr
+00001f30: 726f 7252 8b00 0000 740d 0000 0067 6574  rorR....t....get
+00001f40: 5f68 6f67 5f62 795f 6964 740b 0000 0061  _hog_by_idt....a
+00001f50: 7373 6572 7445 7175 616c 5204 0000 0052  ssertEqualR....R
+00001f60: 9900 0000 528d 0000 0052 9100 0000 5298  ....R....R....R.
+00001f70: 0000 0074 0600 0000 666f 726d 6174 529a  ...t....formatR.
+00001f80: 0000 0052 9500 0000 2804 0000 0052 2400  ...R....(....R$.
+00001f90: 0000 7404 0000 0068 6f67 3374 0600 0000  ..t....hog3t....
+00001fa0: 686f 675f 6964 7403 0000 0068 6f67 2800  hog_idt....hog(.
+00001fb0: 0000 0028 0000 0000 7331 0000 002f 5573  ...(....s1.../Us
+00001fc0: 6572 732f 6164 7269 6161 6c2f 5265 706f  ers/adriaal/Repo
+00001fd0: 7369 746f 7269 6573 2f48 414d 2f74 6573  sitories/HAM/tes
+00001fe0: 7473 2f74 6573 745f 6861 6d2e 7079 7412  ts/test_ham.pyt.
+00001ff0: 0000 0074 6573 745f 6765 745f 686f 675f  ...test_get_hog_
+00002000: 6279 5f69 64b2 0000 0073 2800 0000 0003  by_id....s(.....
+00002010: 1001 1603 1201 1603 1201 1602 1201 1602  ................
+00002020: 1201 1607 1001 1201 1f02 1201 2302 1001  ............#...
+00002030: 1001 1602 1001 6301 0000 0006 0000 0008  ......c.........
+00002040: 0000 0043 0000 0073 3201 0000 7c00 006a  ...C...s2...|..j
+00002050: 0000 6a01 0064 0100 8301 007d 0100 7c00  ..j..d.....}..|.
+00002060: 006a 0000 6a02 007c 0100 8301 007d 0200  .j..j..|.....}..
+00002070: 7c00 006a 0300 7404 007c 0200 8301 0064  |..j..t..|.....d
+00002080: 0200 8302 0001 7c00 006a 0500 6a02 007c  ......|..j..j..|
+00002090: 0100 8301 007d 0200 7c00 006a 0300 7404  .....}..|..j..t.
+000020a0: 007c 0200 8301 0064 0200 8302 0001 7c00  .|.....d......|.
+000020b0: 006a 0600 7407 0083 0100 8f15 0001 7c00  .j..t.........|.
+000020c0: 006a 0000 6a02 0064 0300 8301 0001 5764  .j..j..d......Wd
+000020d0: 0000 5158 7857 007c 0000 6a08 0044 5d4c  ..QXxW.|..j..D]L
+000020e0: 007d 0300 7c00 006a 0900 6a01 007c 0300  .}..|..j..j..|..
+000020f0: 8301 007d 0400 7c00 006a 0900 6a02 007c  ...}..|..j..j..|
+00002100: 0400 8301 007d 0500 7c00 006a 0300 7404  .....}..|..j..t.
+00002110: 007c 0500 8301 0064 0400 6a0a 007c 0500  .|.....d..j..|..
+00002120: 6a0b 0083 0100 8302 0001 7192 0057 7849  j.........q..WxI
+00002130: 007c 0000 6a0c 0044 5d3e 007d 0300 7c00  .|..j..D]>.}..|.
+00002140: 006a 0600 7407 0083 0100 8f27 0001 7c00  .j..t......'..|.
+00002150: 006a 0900 6a01 007c 0300 8301 007d 0400  .j..j..|.....}..
+00002160: 7c00 006a 0900 6a02 007c 0400 8301 0001  |..j..j..|......
+00002170: 5764 0000 5158 71ec 0057 6400 0053 2805  Wd..QXq..Wd..S(.
+00002180: 0000 004e 5277 0000 0073 0800 0000 3c48  ...NRw...s....<H
+00002190: 4f47 2833 293e 7404 0000 0067 656e 6573  OG(3)>t....genes
+000021a0: 0900 0000 3c48 4f47 287b 7d29 3e28 0d00  ....<HOG({})>(..
+000021b0: 0000 528b 0000 0074 0e00 0000 6765 745f  ..R....t....get_
+000021c0: 6765 6e65 5f62 795f 6964 740f 0000 0067  gene_by_idt....g
+000021d0: 6574 5f68 6f67 5f62 795f 6765 6e65 52a1  et_hog_by_geneR.
+000021e0: 0000 0052 0400 0000 528d 0000 0052 2c00  ...R....R....R,.
+000021f0: 0000 529f 0000 0052 8f00 0000 5298 0000  ..R....R....R...
+00002200: 0052 a200 0000 52a4 0000 0052 9300 0000  .R....R....R....
+00002210: 2806 0000 0052 2400 0000 7405 0000 0067  (....R$...t....g
+00002220: 656e 6533 52a3 0000 0074 0700 0000 6765  ene3R....t....ge
+00002230: 6e65 5f69 6452 a700 0000 52a5 0000 0028  ne_idR....R....(
+00002240: 0000 0000 2800 0000 0073 3100 0000 2f55  ....(....s1.../U
+00002250: 7365 7273 2f61 6472 6961 616c 2f52 6570  sers/adriaal/Rep
+00002260: 6f73 6974 6f72 6965 732f 4841 4d2f 7465  ositories/HAM/te
+00002270: 7374 732f 7465 7374 5f68 616d 2e70 7974  sts/test_ham.pyt
+00002280: 1400 0000 7465 7374 5f67 6574 5f68 6f67  ....test_get_hog
+00002290: 5f62 795f 6765 6e65 d900 0000 731e 0000  _by_gene....s...
+000022a0: 0000 0212 0312 0116 0212 0116 0310 0116  ................
+000022b0: 0610 0112 0112 0126 0210 0110 0112 0163  .......&.......c
+000022c0: 0100 0000 0200 0000 0500 0000 4300 0000  ............C...
+000022d0: 7388 0000 007c 0000 6a00 006a 0100 8300  s....|..j..j....
+000022e0: 007d 0100 7c00 006a 0200 7403 007c 0100  .}..|..j..t..|..
+000022f0: 8301 0064 0100 6402 0064 0300 6803 0083  ...d..d..d..h...
+00002300: 0200 017c 0000 6a04 006a 0100 8300 007d  ...|..j..j.....}
+00002310: 0100 7c00 006a 0200 7403 007c 0100 8301  ..|..j..t..|....
+00002320: 0064 0100 6402 0064 0300 6803 0083 0200  .d..d..d..h.....
+00002330: 017c 0000 6a05 006a 0100 8300 007d 0100  .|..j..j.....}..
+00002340: 7c00 006a 0200 7403 007c 0100 8301 0064  |..j..t..|.....d
+00002350: 0100 6801 0083 0200 0164 0000 5328 0400  ..h......d..S(..
+00002360: 0000 4e73 0800 0000 3c48 4f47 2832 293e  ..Ns....<HOG(2)>
+00002370: 7308 0000 003c 484f 4728 3129 3e73 0800  s....<HOG(1)>s..
+00002380: 0000 3c48 4f47 2833 293e 2806 0000 0052  ..<HOG(3)>(....R
+00002390: 8b00 0000 7417 0000 0067 6574 5f6c 6973  ....t....get_lis
+000023a0: 745f 746f 705f 6c65 7665 6c5f 686f 6773  t_top_level_hogs
+000023b0: 740e 0000 0061 7373 6572 7453 6574 4571  t....assertSetEq
+000023c0: 7561 6c52 1000 0000 528d 0000 0052 9800  ualR....R....R..
+000023d0: 0000 2802 0000 0052 2400 0000 5253 0000  ..(....R$...RS..
+000023e0: 0028 0000 0000 2800 0000 0073 3100 0000  .(....(....s1...
+000023f0: 2f55 7365 7273 2f61 6472 6961 616c 2f52  /Users/adriaal/R
+00002400: 6570 6f73 6974 6f72 6965 732f 4841 4d2f  epositories/HAM/
+00002410: 7465 7374 732f 7465 7374 5f68 616d 2e70  tests/test_ham.p
+00002420: 7974 1c00 0000 7465 7374 5f67 6574 5f6c  yt....test_get_l
+00002430: 6973 745f 746f 705f 6c65 7665 6c5f 686f  ist_top_level_ho
+00002440: 6773 f600 0000 730c 0000 0000 010f 011f  gs....s.........
+00002450: 020f 011f 060f 0163 0100 0000 0200 0000  .......c........
+00002460: 0500 0000 4300 0000 73d0 0000 007c 0000  ....C...s....|..
+00002470: 6a00 006a 0100 8300 007d 0100 7c00 006a  j..j.....}..|..j
+00002480: 0200 7403 007c 0100 8301 0069 0300 6401  ..t..|.....i..d.
+00002490: 0064 0200 3664 0300 6404 0036 6405 0064  .d..6d..d..6d..d
+000024a0: 0600 3683 0200 017c 0000 6a04 006a 0100  ..6....|..j..j..
+000024b0: 8300 007d 0100 7c00 006a 0200 7403 007c  ...}..|..j..t..|
+000024c0: 0100 8301 0069 0300 6401 0064 0200 3664  .....i..d..d..6d
+000024d0: 0300 6404 0036 6405 0064 0600 3683 0200  ..d..6d..d..6...
+000024e0: 017c 0000 6a05 006a 0100 8300 007d 0100  .|..j..j.....}..
+000024f0: 7c00 006a 0200 7403 007c 0100 8301 0069  |..j..t..|.....i
+00002500: 0100 6401 0064 0200 3683 0200 017c 0000  ..d..d..6....|..
+00002510: 6a06 006a 0100 8300 007d 0100 7c00 006a  j..j.....}..|..j
+00002520: 0200 7403 007c 0100 8301 0069 0100 6401  ..t..|.....i..d.
+00002530: 0064 0200 3683 0200 0164 0000 5328 0700  .d..6....d..S(..
+00002540: 0000 4e73 0800 0000 3c48 4f47 2832 293e  ..Ns....<HOG(2)>
+00002550: 5269 0000 0073 0800 0000 3c48 4f47 2831  Ri...s....<HOG(1
+00002560: 293e 5271 0000 0073 0800 0000 3c48 4f47  )>Rq...s....<HOG
+00002570: 2833 293e 5277 0000 0028 0700 0000 528b  (3)>Rw...(....R.
+00002580: 0000 0052 5200 0000 740f 0000 0061 7373  ...RR...t....ass
+00002590: 6572 7444 6963 7445 7175 616c 520a 0000  ertDictEqualR...
+000025a0: 0052 8d00 0000 5298 0000 0052 9a00 0000  .R....R....R....
+000025b0: 2802 0000 0052 2400 0000 5253 0000 0028  (....R$...RS...(
+000025c0: 0000 0000 2800 0000 0073 3100 0000 2f55  ....(....s1.../U
+000025d0: 7365 7273 2f61 6472 6961 616c 2f52 6570  sers/adriaal/Rep
+000025e0: 6f73 6974 6f72 6965 732f 4841 4d2f 7465  ositories/HAM/te
+000025f0: 7374 732f 7465 7374 5f68 616d 2e70 7974  sts/test_ham.pyt
+00002600: 1c00 0000 7465 7374 5f67 6574 5f64 6963  ....test_get_dic
+00002610: 745f 746f 705f 6c65 7665 6c5f 686f 6773  t_top_level_hogs
+00002620: 0401 0000 7310 0000 0000 010f 012b 020f  ....s........+..
+00002630: 012b 060f 011d 020f 0163 0100 0000 0400  .+.......c......
+00002640: 0000 0800 0000 4300 0000 7321 0100 007c  ......C...s!...|
+00002650: 0000 6a00 0074 0100 8301 008f 1500 017c  ..j..t.........|
+00002660: 0000 6a02 006a 0300 6401 0083 0100 0157  ..j..j..d......W
+00002670: 6400 0051 587c 0000 6a02 006a 0300 6402  d..QX|..j..j..d.
+00002680: 0083 0100 7d01 007c 0000 6a04 0074 0500  ....}..|..j..t..
+00002690: 7c01 0083 0100 6403 0083 0200 017c 0000  |.....d......|..
+000026a0: 6a06 006a 0300 6402 0083 0100 7d01 007c  j..j..d.....}..|
+000026b0: 0000 6a04 0074 0500 7c01 0083 0100 6403  ..j..t..|.....d.
+000026c0: 0083 0200 017c 0000 6a02 006a 0300 6404  .....|..j..j..d.
+000026d0: 0083 0100 7d01 007c 0000 6a04 0074 0500  ....}..|..j..t..
+000026e0: 7c01 0083 0100 6403 0083 0200 0178 4200  |.....d......xB.
+000026f0: 7c00 006a 0700 445d 3700 7d02 007c 0000  |..j..D]7.}..|..
+00002700: 6a08 006a 0300 7c02 0083 0100 7d03 007c  j..j..|.....}..|
+00002710: 0000 6a04 0074 0500 7c03 0083 0100 6405  ..j..t..|.....d.
+00002720: 006a 0900 7c02 0083 0100 8302 0001 71a8  .j..|.........q.
+00002730: 0057 7837 007c 0000 6a0a 0044 5d2c 007d  .Wx7.|..j..D],.}
+00002740: 0200 7c00 006a 0000 7401 0083 0100 8f15  ..|..j..t.......
+00002750: 0001 7c00 006a 0800 6a03 007c 0200 8301  ..|..j..j..|....
+00002760: 0001 5764 0000 5158 71ed 0057 6400 0053  ..Wd..QXq..Wd..S
+00002770: 2806 0000 004e 529e 0000 0052 7700 0000  (....NR....Rw...
+00002780: 7307 0000 0047 656e 6528 3329 6903 0000  s....Gene(3)i...
+00002790: 0073 0800 0000 4765 6e65 287b 7d29 280b  .s....Gene({})(.
+000027a0: 0000 0052 2c00 0000 529f 0000 0052 8b00  ...R,...R....R..
+000027b0: 0000 52a8 0000 0052 a100 0000 5204 0000  ..R....R....R...
+000027c0: 0052 8d00 0000 5291 0000 0052 9800 0000  .R....R....R....
+000027d0: 52a2 0000 0052 9300 0000 2804 0000 0052  R....R....(....R
+000027e0: 2400 0000 52aa 0000 0052 ab00 0000 52a7  $...R....R....R.
+000027f0: 0000 0028 0000 0000 2800 0000 0073 3100  ...(....(....s1.
+00002800: 0000 2f55 7365 7273 2f61 6472 6961 616c  ../Users/adriaal
+00002810: 2f52 6570 6f73 6974 6f72 6965 732f 4841  /Repositories/HA
+00002820: 4d2f 7465 7374 732f 7465 7374 5f68 616d  M/tests/test_ham
+00002830: 2e70 7974 1300 0000 7465 7374 5f67 6574  .pyt....test_get
+00002840: 5f67 656e 655f 6279 5f69 6417 0100 0073  _gene_by_id....s
+00002850: 1c00 0000 0003 1001 1603 1201 1602 1201  ................
+00002860: 1603 1201 1606 1001 1201 2302 1001 1001  ..........#.....
+00002870: 6301 0000 0004 0000 0008 0000 0043 0000  c............C..
+00002880: 0073 9301 0000 7c00 006a 0000 7401 0083  .s....|..j..t...
+00002890: 0100 8f15 0001 7c00 006a 0200 6a03 0064  ......|..j..j..d
+000028a0: 0100 8301 0001 5764 0000 5158 7c00 006a  ......Wd..QX|..j
+000028b0: 0200 6a03 0064 0200 8301 0064 0300 197d  ..j..d.....d...}
+000028c0: 0100 7c00 006a 0400 7405 007c 0100 8301  ..|..j..t..|....
+000028d0: 0064 0400 8302 0001 7c00 006a 0200 6a03  .d......|..j..j.
+000028e0: 0064 0500 8301 0064 0300 197d 0100 7c00  .d.....d...}..|.
+000028f0: 006a 0400 7405 007c 0100 8301 0064 0400  .j..t..|.....d..
+00002900: 8302 0001 7c00 006a 0600 6a03 0064 0500  ....|..j..j..d..
+00002910: 8301 0064 0300 197d 0100 7c00 006a 0400  ...d...}..|..j..
+00002920: 7405 007c 0100 8301 0064 0400 8302 0001  t..|.....d......
+00002930: 7c00 006a 0700 6a03 0064 0200 8301 0064  |..j..j..d.....d
+00002940: 0300 197d 0100 7c00 006a 0400 7405 007c  ...}..|..j..t..|
+00002950: 0100 8301 0064 0400 8302 0001 7c00 006a  .....d......|..j
+00002960: 0700 6a03 0064 0500 8301 0064 0300 197d  ..j..d.....d...}
+00002970: 0100 7c00 006a 0400 7405 007c 0100 8301  ..|..j..t..|....
+00002980: 0064 0400 8302 0001 7850 007c 0000 6a08  .d......xP.|..j.
+00002990: 0044 5d45 007d 0200 7c00 006a 0900 6a03  .D]E.}..|..j..j.
+000029a0: 007c 0200 8301 007d 0300 7c00 006a 0400  .|.....}..|..j..
+000029b0: 740a 007c 0300 8301 0064 0600 8302 0001  t..|.....d......
+000029c0: 7c00 006a 0400 7c03 0064 0300 196a 0b00  |..j..|..d...j..
+000029d0: 7c02 0083 0200 0171 0c01 5778 3700 7c00  |......q..Wx7.|.
+000029e0: 006a 0c00 445d 2c00 7d02 007c 0000 6a00  .j..D],.}..|..j.
+000029f0: 0074 0100 8301 008f 1500 017c 0000 6a09  .t.........|..j.
+00002a00: 006a 0300 7c02 0083 0100 0157 6400 0051  .j..|......Wd..Q
+00002a10: 5871 5f01 5764 0000 5328 0700 0000 4e52  Xq_.Wd..S(....NR
+00002a20: 9e00 0000 5270 0000 0069 0000 0000 7308  ....Rp...i....s.
+00002a30: 0000 0047 656e 6528 3132 2974 0700 0000  ...Gene(12)t....
+00002a40: 5041 4e54 5267 3269 0100 0000 280d 0000  PANTRg2i....(...
+00002a50: 0052 2c00 0000 529f 0000 0052 8b00 0000  .R,...R....R....
+00002a60: 7418 0000 0067 6574 5f67 656e 6573 5f62  t....get_genes_b
+00002a70: 795f 6578 7465 726e 616c 5f69 6452 a100  y_external_idR..
+00002a80: 0000 5204 0000 0052 9900 0000 528d 0000  ..R....R....R...
+00002a90: 0052 9000 0000 5298 0000 0074 0300 0000  .R....R....t....
+00002aa0: 6c65 6e74 0700 0000 7072 6f74 5f69 6452  lent....prot_idR
+00002ab0: 9400 0000 2804 0000 0052 2400 0000 7406  ....(....R$...t.
+00002ac0: 0000 0067 656e 6531 3252 ab00 0000 5255  ...gene12R....RU
+00002ad0: 0000 0028 0000 0000 2800 0000 0073 3100  ...(....(....s1.
+00002ae0: 0000 2f55 7365 7273 2f61 6472 6961 616c  ../Users/adriaal
+00002af0: 2f52 6570 6f73 6974 6f72 6965 732f 4841  /Repositories/HA
+00002b00: 4d2f 7465 7374 732f 7465 7374 5f68 616d  M/tests/test_ham
+00002b10: 2e70 7974 1d00 0000 7465 7374 5f67 6574  .pyt....test_get
+00002b20: 5f67 656e 6573 5f62 795f 6578 7465 726e  _genes_by_extern
+00002b30: 616c 5f69 6434 0100 0073 2600 0000 0003  al_id4...s&.....
+00002b40: 1001 1603 1601 1603 1601 1602 1601 1603  ................
+00002b50: 1601 1603 1601 1607 1001 1201 1601 1b02  ................
+00002b60: 1001 1001 6301 0000 0004 0000 0013 0000  ....c...........
+00002b70: 0043 0000 0073 4801 0000 7c00 006a 0000  .C...sH...|..j..
+00002b80: 6a01 0083 0000 7d01 0064 0100 6402 0064  j.....}..d..d..d
+00002b90: 0300 6404 0064 0500 6406 0064 0700 6408  ..d..d..d..d..d.
+00002ba0: 0064 0900 640a 0064 0b00 640c 0064 0d00  .d..d..d..d..d..
+00002bb0: 640e 0064 0f00 6410 0064 1100 6412 0064  d..d..d..d..d..d
+00002bc0: 1300 6813 007d 0200 7c00 006a 0200 7403  ..h..}..|..j..t.
+00002bd0: 007c 0100 8301 007c 0200 8302 0001 7c00  .|.....|......|.
+00002be0: 006a 0400 6a01 0083 0000 7d01 0064 0100  .j..j.....}..d..
+00002bf0: 6402 0064 0300 6404 0064 0500 6406 0064  d..d..d..d..d..d
+00002c00: 0700 6408 0064 0900 640a 0064 0b00 640c  ..d..d..d..d..d.
+00002c10: 0064 0d00 640e 0064 0f00 6410 0064 1100  .d..d..d..d..d..
+00002c20: 6412 0064 1300 6813 007d 0200 7c00 006a  d..d..h..}..|..j
+00002c30: 0200 7403 007c 0100 8301 007c 0200 8302  ..t..|.....|....
+00002c40: 0001 7c00 006a 0500 6a01 0083 0000 7d01  ..|..j..j.....}.
+00002c50: 007c 0000 6a02 0074 0600 6700 007c 0100  .|..j..t..g..|..
+00002c60: 445d 0f00 7d03 007c 0300 6a07 005e 0200  D]..}..|..j..^..
+00002c70: 71e7 0083 0100 7c00 006a 0800 8302 0001  q.....|..j......
+00002c80: 7c00 006a 0900 6a01 0083 0000 7d01 007c  |..j..j.....}..|
+00002c90: 0000 6a02 0074 0600 6700 007c 0100 445d  ..j..t..g..|..D]
+00002ca0: 0f00 7d03 007c 0300 6a07 005e 0200 7125  ..}..|..j..^..q%
+00002cb0: 0183 0100 7c00 006a 0800 8302 0001 6400  ....|..j......d.
+00002cc0: 0053 2814 0000 004e 7308 0000 0047 656e  .S(....Ns....Gen
+00002cd0: 6528 3333 2973 0800 0000 4765 6e65 2831  e(33)s....Gene(1
+00002ce0: 3429 7308 0000 0047 656e 6528 3331 2973  4)s....Gene(31)s
+00002cf0: 0800 0000 4765 6e65 2835 3129 7308 0000  ....Gene(51)s...
+00002d00: 0047 656e 6528 3133 2973 0800 0000 4765  .Gene(13)s....Ge
+00002d10: 6e65 2831 3129 7308 0000 0047 656e 6528  ne(11)s....Gene(
+00002d20: 3132 2973 0800 0000 4765 6e65 2832 3329  12)s....Gene(23)
+00002d30: 7308 0000 0047 656e 6528 3231 2973 0700  s....Gene(21)s..
+00002d40: 0000 4765 6e65 2832 2973 0800 0000 4765  ..Gene(2)s....Ge
+00002d50: 6e65 2833 3429 7307 0000 0047 656e 6528  ne(34)s....Gene(
+00002d60: 3129 7308 0000 0047 656e 6528 3332 2973  1)s....Gene(32)s
+00002d70: 0700 0000 4765 6e65 2835 2973 0800 0000  ....Gene(5)s....
+00002d80: 4765 6e65 2832 3229 7307 0000 0047 656e  Gene(22)s....Gen
+00002d90: 6528 3329 7308 0000 0047 656e 6528 3431  e(3)s....Gene(41
+00002da0: 2973 0800 0000 4765 6e65 2835 3329 7308  )s....Gene(53)s.
+00002db0: 0000 0047 656e 6528 3433 2928 0a00 0000  ...Gene(43)(....
+00002dc0: 528b 0000 0074 1500 0000 6765 745f 6c69  R....t....get_li
+00002dd0: 7374 5f65 7874 616e 745f 6765 6e65 7352  st_extant_genesR
+00002de0: ae00 0000 5210 0000 0052 8d00 0000 5298  ....R....R....R.
+00002df0: 0000 0052 0c00 0000 7409 0000 0075 6e69  ...R....t....uni
+00002e00: 7175 655f 6964 528f 0000 0052 9a00 0000  que_idR....R....
+00002e10: 2804 0000 0052 2400 0000 5255 0000 0074  (....R$...RU...t
+00002e20: 0800 0000 6578 7065 6374 6564 7401 0000  ....expectedt...
+00002e30: 0067 2800 0000 0028 0000 0000 7331 0000  .g(....(....s1..
+00002e40: 002f 5573 6572 732f 6164 7269 6161 6c2f  ./Users/adriaal/
+00002e50: 5265 706f 7369 746f 7269 6573 2f48 414d  Repositories/HAM
+00002e60: 2f74 6573 7473 2f74 6573 745f 6861 6d2e  /tests/test_ham.
+00002e70: 7079 741a 0000 0074 6573 745f 6765 745f  pyt....test_get_
+00002e80: 6c69 7374 5f65 7874 616e 745f 6765 6e65  list_extant_gene
+00002e90: 735b 0100 0073 1c00 0000 0002 0f01 1801  s[...s..........
+00002ea0: 1801 0f01 1602 0f01 1801 1801 0f01 1606  ................
+00002eb0: 0f01 2f02 0f01 6301 0000 0003 0000 0005  ../...c.........
+00002ec0: 0000 0043 0000 0073 a501 0000 7c00 006a  ...C...s....|..j
+00002ed0: 0000 6a01 0083 0000 7d01 0069 1300 6401  ..j.....}..i..d.
+00002ee0: 0064 0200 3664 0300 6404 0036 6405 0064  .d..6d..d..6d..d
+00002ef0: 0600 3664 0700 6408 0036 6409 0064 0a00  ..6d..d..6d..d..
+00002f00: 3664 0b00 640c 0036 640d 0064 0e00 3664  6d..d..6d..d..6d
+00002f10: 0f00 6410 0036 6411 0064 1200 3664 1300  ..d..6d..d..6d..
+00002f20: 6414 0036 6415 0064 1600 3664 1700 6418  d..6d..d..6d..d.
+00002f30: 0036 6419 0064 1a00 3664 1b00 641c 0036  .6d..d..6d..d..6
+00002f40: 641d 0064 1e00 3664 1f00 6420 0036 6421  d..d..6d..d .6d!
+00002f50: 0064 2200 3664 2300 6424 0036 6425 0064  .d".6d#.d$.6d%.d
+00002f60: 2600 367d 0200 7c00 006a 0200 7403 007c  &.6}..|..j..t..|
+00002f70: 0100 8301 007c 0200 8302 0001 7c00 006a  .....|......|..j
+00002f80: 0400 6a01 0083 0000 7d01 0069 1300 6401  ..j.....}..i..d.
+00002f90: 0064 0200 3664 0300 6404 0036 6405 0064  .d..6d..d..6d..d
+00002fa0: 0600 3664 0700 6408 0036 6409 0064 0a00  ..6d..d..6d..d..
+00002fb0: 3664 0b00 640c 0036 640d 0064 0e00 3664  6d..d..6d..d..6d
+00002fc0: 0f00 6410 0036 6411 0064 1200 3664 1300  ..d..6d..d..6d..
+00002fd0: 6414 0036 6415 0064 1600 3664 1700 6418  d..6d..d..6d..d.
+00002fe0: 0036 6419 0064 1a00 3664 1b00 641c 0036  .6d..d..6d..d..6
+00002ff0: 641d 0064 1e00 3664 1f00 6420 0036 6421  d..d..6d..d .6d!
+00003000: 0064 2200 3664 2300 6424 0036 6425 0064  .d".6d#.d$.6d%.d
+00003010: 2600 367d 0200 7c00 006a 0200 7403 007c  &.6}..|..j..t..|
+00003020: 0100 8301 007c 0200 8302 0001 7c00 006a  .....|......|..j
+00003030: 0500 6a01 0083 0000 7d01 007c 0000 6a02  ..j.....}..|..j.
+00003040: 0074 0300 7c01 0083 0100 6904 0064 1f00  .t..|.....i..d..
+00003050: 6420 0036 640f 0064 1000 3664 0500 6406  d .6d..d..6d..d.
+00003060: 0036 6407 0064 0800 3683 0200 0164 0000  .6d..d..6....d..
+00003070: 5328 2700 0000 4e73 0800 0000 4765 6e65  S('...Ns....Gene
+00003080: 2833 3429 527c 0000 0073 0800 0000 4765  (34)R|...s....Ge
+00003090: 6e65 2833 3329 527a 0000 0073 0700 0000  ne(33)Rz...s....
+000030a0: 4765 6e65 2832 2952 6900 0000 7308 0000  Gene(2)Ri...s...
+000030b0: 0047 656e 6528 3132 2952 6c00 0000 7307  .Gene(12)Rl...s.
+000030c0: 0000 0047 656e 6528 3529 7401 0000 0035  ...Gene(5)t....5
+000030d0: 7308 0000 0047 656e 6528 3131 2952 7200  s....Gene(11)Rr.
+000030e0: 0000 7307 0000 0047 656e 6528 3129 5271  ..s....Gene(1)Rq
+000030f0: 0000 0073 0800 0000 4765 6e65 2832 3229  ...s....Gene(22)
+00003100: 526b 0000 0073 0700 0000 4765 6e65 2833  Rk...s....Gene(3
+00003110: 2952 7700 0000 7308 0000 0047 656e 6528  )Rw...s....Gene(
+00003120: 3431 2952 7500 0000 7308 0000 0047 656e  41)Ru...s....Gen
+00003130: 6528 3531 2952 7600 0000 7308 0000 0047  e(51)Rv...s....G
+00003140: 656e 6528 3533 2952 7b00 0000 7308 0000  ene(53)R{...s...
+00003150: 0047 656e 6528 3134 2952 7d00 0000 7308  .Gene(14)R}...s.
+00003160: 0000 0047 656e 6528 3133 2952 7800 0000  ...Gene(13)Rx...
+00003170: 7308 0000 0047 656e 6528 3433 2974 0200  s....Gene(43)t..
+00003180: 0000 3433 7308 0000 0047 656e 6528 3332  ..43s....Gene(32
+00003190: 2952 6a00 0000 7308 0000 0047 656e 6528  )Rj...s....Gene(
+000031a0: 3233 2952 7900 0000 7308 0000 0047 656e  23)Ry...s....Gen
+000031b0: 6528 3231 2952 7300 0000 7308 0000 0047  e(21)Rs...s....G
+000031c0: 656e 6528 3331 2952 7400 0000 2806 0000  ene(31)Rt...(...
+000031d0: 0052 8b00 0000 5254 0000 0052 b000 0000  .R....RT...R....
+000031e0: 520a 0000 0052 8d00 0000 5298 0000 0028  R....R....R....(
+000031f0: 0300 0000 5224 0000 0052 5500 0000 52bb  ....R$...RU...R.
+00003200: 0000 0028 0000 0000 2800 0000 0073 3100  ...(....(....s1.
+00003210: 0000 2f55 7365 7273 2f61 6472 6961 616c  ../Users/adriaal
+00003220: 2f52 6570 6f73 6974 6f72 6965 732f 4841  /Repositories/HA
+00003230: 4d2f 7465 7374 732f 7465 7374 5f68 616d  M/tests/test_ham
+00003240: 2e70 7974 1a00 0000 7465 7374 5f67 6574  .pyt....test_get
+00003250: 5f64 6963 745f 6578 7461 6e74 5f67 656e  _dict_extant_gen
+00003260: 6573 7301 0000 731e 0000 0000 020f 0126  ess...s........&
+00003270: 012a 012a 0111 0116 020f 0126 012a 0123  .*.*.......&.*.#
+00003280: 0107 0111 0116 060f 0163 0100 0000 0400  .........c......
+00003290: 0000 0800 0000 4300 0000 733b 0100 007c  ......C...s;...|
+000032a0: 0000 6a00 0074 0100 8301 008f 1500 017c  ..j..t.........|
+000032b0: 0000 6a02 006a 0300 6401 0083 0100 0157  ..j..j..d......W
+000032c0: 6400 0051 587c 0000 6a00 0074 0100 8301  d..QX|..j..t....
+000032d0: 008f 1500 017c 0000 6a02 006a 0300 6402  .....|..j..j..d.
+000032e0: 0083 0100 0157 6400 0051 587c 0000 6a00  .....Wd..QX|..j.
+000032f0: 0074 0100 8301 008f 1500 017c 0000 6a02  .t.........|..j.
+00003300: 006a 0300 6403 0083 0100 0157 6400 0051  .j..d......Wd..Q
+00003310: 587c 0000 6a02 006a 0300 6404 0083 0100  X|..j..j..d.....
+00003320: 7d01 007c 0000 6a04 007c 0100 6a05 0064  }..|..j..|..j..d
+00003330: 0400 8302 0001 7c00 006a 0600 6a03 0064  ......|..j..j..d
+00003340: 0400 8301 007d 0100 7c00 006a 0400 7c01  .....}..|..j..|.
+00003350: 006a 0500 6404 0083 0200 0178 3900 7c00  .j..d......x9.|.
+00003360: 006a 0700 445d 2e00 7d02 007c 0000 6a08  .j..D]..}..|..j.
+00003370: 006a 0300 7c02 0083 0100 7d03 007c 0000  .j..|.....}..|..
+00003380: 6a04 0074 0900 7c03 0083 0100 7c02 0083  j..t..|.....|...
+00003390: 0200 0171 c600 5778 3c00 7c00 006a 0a00  ...q..Wx<.|..j..
+000033a0: 445d 3100 7d02 007c 0000 6a08 006a 0300  D]1.}..|..j..j..
+000033b0: 7c02 0083 0100 7d03 007c 0000 6a04 0074  |.....}..|..j..t
+000033c0: 0b00 7c03 006a 0c00 8301 0064 0500 8302  ..|..j.....d....
+000033d0: 0001 7102 0157 6400 0053 2806 0000 004e  ..q..Wd..S(....N
+000033e0: 5212 0000 0074 0300 0000 6162 6369 0100  R....t....abci..
+000033f0: 0000 524d 0000 0069 0000 0000 280d 0000  ..RM...i....(...
+00003400: 0052 2c00 0000 529f 0000 0052 8b00 0000  .R,...R....R....
+00003410: 5256 0000 0052 a100 0000 524c 0000 0052  RV...R....RL...R
+00003420: 8d00 0000 528e 0000 0052 9800 0000 5204  ....R....R....R.
+00003430: 0000 0052 9200 0000 52b5 0000 0052 5500  ...R....R....RU.
+00003440: 0000 2804 0000 0052 2400 0000 528b 0000  ..(....R$...R...
+00003450: 0074 0500 0000 676e 616d 6574 0600 0000  .t....gnamet....
+00003460: 6765 6e6f 6d65 2800 0000 0028 0000 0000  genome(....(....
+00003470: 7331 0000 002f 5573 6572 732f 6164 7269  s1.../Users/adri
+00003480: 6161 6c2f 5265 706f 7369 746f 7269 6573  aal/Repositories
+00003490: 2f48 414d 2f74 6573 7473 2f74 6573 745f  /HAM/tests/test_
+000034a0: 6861 6d2e 7079 741e 0000 0074 6573 745f  ham.pyt....test_
+000034b0: 6765 745f 6578 7461 6e74 5f67 656e 6f6d  get_extant_genom
+000034c0: 655f 6279 5f6e 616d 658d 0100 0073 2000  e_by_name....s .
+000034d0: 0000 0002 1001 1602 1001 1602 1001 1602  ................
+000034e0: 1201 1302 1201 1305 1001 1201 1a02 1001  ................
+000034f0: 1201 6301 0000 0003 0000 0006 0000 0043  ..c............C
+00003500: 0000 0073 7e00 0000 7c00 006a 0000 6a01  ...s~...|..j..j.
+00003510: 0083 0000 7d01 0064 0100 6402 0064 0300  ....}..d..d..d..
+00003520: 6404 0064 0500 6406 0068 0600 7d02 007c  d..d..d..h..}..|
+00003530: 0000 6a02 0074 0300 7c01 0083 0100 7c02  ..j..t..|.....|.
+00003540: 0083 0200 017c 0000 6a04 006a 0100 8300  .....|..j..j....
+00003550: 007d 0100 6401 0064 0200 6403 0064 0400  .}..d..d..d..d..
+00003560: 6405 0064 0600 6806 007d 0200 7c00 006a  d..d..h..}..|..j
+00003570: 0200 7403 007c 0100 8301 007c 0200 8302  ..t..|.....|....
+00003580: 0001 6400 0053 2807 0000 004e 5250 0000  ..d..S(....NRP..
+00003590: 0052 4d00 0000 524f 0000 0052 4e00 0000  .RM...RO...RN...
+000035a0: 5251 0000 0052 6800 0000 2805 0000 0052  RQ...Rh...(....R
+000035b0: 8b00 0000 7417 0000 0067 6574 5f6c 6973  ....t....get_lis
+000035c0: 745f 6578 7461 6e74 5f67 656e 6f6d 6573  t_extant_genomes
+000035d0: 52ae 0000 0052 1000 0000 528d 0000 0028  R....R....R....(
+000035e0: 0300 0000 5224 0000 0074 0300 0000 6c65  ....R$...t....le
+000035f0: 6752 bb00 0000 2800 0000 0028 0000 0000  gR....(....(....
+00003600: 7331 0000 002f 5573 6572 732f 6164 7269  s1.../Users/adri
+00003610: 6161 6c2f 5265 706f 7369 746f 7269 6573  aal/Repositories
+00003620: 2f48 414d 2f74 6573 7473 2f74 6573 745f  /HAM/tests/test_
+00003630: 6861 6d2e 7079 741c 0000 0074 6573 745f  ham.pyt....test_
+00003640: 6765 745f 6c69 7374 5f65 7874 616e 745f  get_list_extant_
+00003650: 6765 6e6f 6d65 73a9 0100 0073 0c00 0000  genomes....s....
+00003660: 0002 0f01 1801 1602 0f01 1801 6301 0000  ............c...
+00003670: 0004 0000 0006 0000 0043 0000 0073 be00  .........C...s..
+00003680: 0000 7c00 006a 0000 7401 0083 0100 8f15  ..|..j..t.......
+00003690: 0001 7c00 006a 0200 6a03 0064 0100 8301  ..|..j..j..d....
+000036a0: 0001 5764 0000 5158 7c00 006a 0200 6a03  ..Wd..QX|..j..j.
+000036b0: 0064 0200 8301 007d 0100 7c00 006a 0400  .d.....}..|..j..
+000036c0: 7c01 006a 0500 6402 0083 0200 017c 0000  |..j..d......|..
+000036d0: 6a06 006a 0300 6403 0083 0100 7d02 007c  j..j..d.....}..|
+000036e0: 0000 6a04 007c 0200 6a05 0064 0300 8302  ..j..|..j..d....
+000036f0: 0001 7c00 006a 0600 6a03 0064 0400 8301  ..|..j..j..d....
+00003700: 007d 0300 7c00 006a 0400 7c03 006a 0500  .}..|..j..|..j..
+00003710: 6404 0083 0200 017c 0000 6a07 006a 0300  d......|..j..j..
+00003720: 6404 0083 0100 7d03 007c 0000 6a04 007c  d.....}..|..j..|
+00003730: 0300 6a05 0064 0400 8302 0001 6400 0053  ..j..d......d..S
+00003740: 2805 0000 004e 5212 0000 0074 0800 0000  (....NR....t....
+00003750: 4d61 6d6d 616c 6961 730b 0000 004d 4f55  Mammalias....MOU
+00003760: 5345 2f52 4154 4e4f 524f 0000 0028 0800  SE/RATNORO...(..
+00003770: 0000 522c 0000 0052 9f00 0000 528b 0000  ..R,...R....R...
+00003780: 0074 1100 0000 6765 745f 7461 786f 6e5f  .t....get_taxon_
+00003790: 6279 5f6e 616d 6552 a100 0000 524c 0000  by_nameR....RL..
+000037a0: 0052 8c00 0000 528d 0000 0028 0400 0000  .R....R....(....
+000037b0: 5224 0000 0074 0700 0000 6d61 6d6d 616c  R$...t....mammal
+000037c0: 7374 0700 0000 726f 6465 6e74 7352 5900  st....rodentsRY.
+000037d0: 0000 2800 0000 0028 0000 0000 7331 0000  ..(....(....s1..
+000037e0: 002f 5573 6572 732f 6164 7269 6161 6c2f  ./Users/adriaal/
+000037f0: 5265 706f 7369 746f 7269 6573 2f48 414d  Repositories/HAM
+00003800: 2f74 6573 7473 2f74 6573 745f 6861 6d2e  /tests/test_ham.
+00003810: 7079 7416 0000 0074 6573 745f 6765 745f  pyt....test_get_
+00003820: 7461 786f 6e5f 6279 5f6e 616d 65b5 0100  taxon_by_name...
+00003830: 0073 1400 0000 0002 1001 1603 1201 1302  .s..............
+00003840: 1201 1303 1201 1304 1201 6301 0000 0004  ..........c.....
+00003850: 0000 0006 0000 0043 0000 0073 aa00 0000  .......C...s....
+00003860: 7c00 006a 0000 6a01 0064 0100 8301 007d  |..j..j..d.....}
+00003870: 0100 7c00 006a 0000 6a02 007c 0100 8301  ..|..j..j..|....
+00003880: 007d 0200 7c00 006a 0300 7c02 006a 0400  .}..|..j..|..j..
+00003890: 6401 0083 0200 017c 0000 6a05 006a 0100  d......|..j..j..
+000038a0: 6401 0083 0100 7d01 007c 0000 6a05 006a  d.....}..|..j..j
+000038b0: 0200 7c01 0083 0100 7d02 007c 0000 6a03  ..|.....}..|..j.
+000038c0: 007c 0200 6a04 0064 0100 8302 0001 7c00  .|..j..d......|.
+000038d0: 006a 0600 7407 0083 0100 8f27 0001 7c00  .j..t......'..|.
+000038e0: 006a 0800 6a01 0064 0200 8301 007d 0300  .j..j..d.....}..
+000038f0: 7c00 006a 0000 6a02 007c 0300 8301 0001  |..j..j..|......
+00003900: 5764 0000 5158 6400 0053 2803 0000 004e  Wd..QXd..S(....N
+00003910: 52c8 0000 0074 0a00 0000 5665 7274 6562  R....t....Verteb
+00003920: 7261 7461 2809 0000 0052 8b00 0000 52c9  rata(....R....R.
+00003930: 0000 0074 1d00 0000 6765 745f 616e 6365  ...t....get_ance
+00003940: 7374 7261 6c5f 6765 6e6f 6d65 5f62 795f  stral_genome_by_
+00003950: 7461 786f 6e52 a100 0000 524c 0000 0052  taxonR....RL...R
+00003960: 8d00 0000 522c 0000 0052 9f00 0000 5298  ....R,...R....R.
+00003970: 0000 0028 0400 0000 5224 0000 0074 0b00  ...(....R$...t..
+00003980: 0000 6d61 6d6d 616c 735f 7461 7852 ca00  ..mammals_taxR..
+00003990: 0000 740e 0000 0076 6572 7465 6272 6174  ..t....vertebrat
+000039a0: 655f 7461 7828 0000 0000 2800 0000 0073  e_tax(....(....s
+000039b0: 3100 0000 2f55 7365 7273 2f61 6472 6961  1.../Users/adria
+000039c0: 616c 2f52 6570 6f73 6974 6f72 6965 732f  al/Repositories/
+000039d0: 4841 4d2f 7465 7374 732f 7465 7374 5f68  HAM/tests/test_h
+000039e0: 616d 2e70 7974 2200 0000 7465 7374 5f67  am.pyt"...test_g
+000039f0: 6574 5f61 6e63 6573 7472 616c 5f67 656e  et_ancestral_gen
+00003a00: 6f6d 655f 6279 5f74 6178 6f6e cc01 0000  ome_by_taxon....
+00003a10: 7312 0000 0000 0212 0112 0113 0212 0112  s...............
+00003a20: 0113 0610 0112 0163 0100 0000 0300 0000  .......c........
+00003a30: 0600 0000 4300 0000 7399 0000 007c 0000  ....C...s....|..
+00003a40: 6a00 006a 0100 6401 0083 0100 7d01 007c  j..j..d.....}..|
+00003a50: 0000 6a02 007c 0100 6a03 0064 0100 8302  ..j..|..j..d....
+00003a60: 0001 7c00 006a 0400 6a01 0064 0100 8301  ..|..j..j..d....
+00003a70: 007d 0100 7c00 006a 0200 7c01 006a 0300  .}..|..j..|..j..
+00003a80: 6401 0083 0200 017c 0000 6a05 006a 0100  d......|..j..j..
+00003a90: 6402 0083 0100 7d02 007c 0000 6a02 007c  d.....}..|..j..|
+00003aa0: 0200 6a03 0064 0200 8302 0001 7c00 006a  ..j..d......|..j
+00003ab0: 0600 7407 0083 0100 8f15 0001 7c00 006a  ..t.........|..j
+00003ac0: 0800 6a01 0064 0300 8301 0001 5764 0000  ..j..d......Wd..
+00003ad0: 5158 6400 0053 2804 0000 004e 52c8 0000  QXd..S(....NR...
+00003ae0: 0073 0b00 0000 4d4f 5553 452f 5241 544e  .s....MOUSE/RATN
+00003af0: 4f52 cd00 0000 2809 0000 0052 8b00 0000  OR....(....R....
+00003b00: 741c 0000 0067 6574 5f61 6e63 6573 7472  t....get_ancestr
+00003b10: 616c 5f67 656e 6f6d 655f 6279 5f6e 616d  al_genome_by_nam
+00003b20: 6552 a100 0000 524c 0000 0052 8d00 0000  eR....RL...R....
+00003b30: 528c 0000 0052 2c00 0000 529f 0000 0052  R....R,...R....R
+00003b40: 9800 0000 2803 0000 0052 2400 0000 52ca  ....(....R$...R.
+00003b50: 0000 0052 cb00 0000 2800 0000 0028 0000  ...R....(....(..
+00003b60: 0000 7331 0000 002f 5573 6572 732f 6164  ..s1.../Users/ad
+00003b70: 7269 6161 6c2f 5265 706f 7369 746f 7269  riaal/Repositori
+00003b80: 6573 2f48 414d 2f74 6573 7473 2f74 6573  es/HAM/tests/tes
+00003b90: 745f 6861 6d2e 7079 7421 0000 0074 6573  t_ham.pyt!...tes
+00003ba0: 745f 6765 745f 616e 6365 7374 7261 6c5f  t_get_ancestral_
+00003bb0: 6765 6e6f 6d65 5f62 795f 6e61 6d65 de01  genome_by_name..
+00003bc0: 0000 7310 0000 0000 0212 0113 0212 0113  ..s.............
+00003bd0: 0212 0113 0610 0163 0100 0000 0300 0000  .......c........
+00003be0: 0700 0000 4300 0000 736c 0000 007c 0000  ....C...sl...|..
+00003bf0: 6a00 006a 0100 8300 007d 0100 7c00 006a  j..j.....}..|..j
+00003c00: 0200 7403 007c 0100 8301 0064 0100 6402  ..t..|.....d..d.
+00003c10: 0064 0300 6404 0064 0500 6805 0083 0200  .d..d..d..h.....
+00003c20: 017c 0000 6a04 006a 0100 8300 007d 0200  .|..j..j.....}..
+00003c30: 7c00 006a 0200 7403 007c 0200 8301 0064  |..j..t..|.....d
+00003c40: 0600 6407 0064 0800 6409 0064 0a00 6805  ..d..d..d..d..h.
+00003c50: 0083 0200 0164 0000 5328 0b00 0000 4e74  .....d..S(....Nt
+00003c60: 1000 0000 4575 6172 6368 6f6e 746f 676c  ....Euarchontogl
+00003c70: 6972 6573 52cd 0000 0052 c800 0000 7408  iresR....R....t.
+00003c80: 0000 0050 7269 6d61 7465 7374 0700 0000  ...Primatest....
+00003c90: 526f 6465 6e74 7373 1700 0000 4855 4d41  Rodentss....HUMA
+00003ca0: 4e2f 5041 4e54 522f 4d4f 5553 452f 5241  N/PANTR/MOUSE/RA
+00003cb0: 544e 4f73 2300 0000 5845 4e54 522f 4855  TNOs#...XENTR/HU
+00003cc0: 4d41 4e2f 5041 4e54 522f 4d4f 5553 452f  MAN/PANTR/MOUSE/
+00003cd0: 5241 544e 4f2f 4341 4e46 4173 1d00 0000  RATNO/CANFAs....
+00003ce0: 4855 4d41 4e2f 5041 4e54 522f 4d4f 5553  HUMAN/PANTR/MOUS
+00003cf0: 452f 5241 544e 4f2f 4341 4e46 4173 0b00  E/RATNO/CANFAs..
+00003d00: 0000 4855 4d41 4e2f 5041 4e54 5273 0b00  ..HUMAN/PANTRs..
+00003d10: 0000 4d4f 5553 452f 5241 544e 4f28 0500  ..MOUSE/RATNO(..
+00003d20: 0000 528b 0000 0074 1a00 0000 6765 745f  ..R....t....get_
+00003d30: 6c69 7374 5f61 6e63 6573 7472 616c 5f67  list_ancestral_g
+00003d40: 656e 6f6d 6573 52ae 0000 0052 1000 0000  enomesR....R....
+00003d50: 528c 0000 0028 0300 0000 5224 0000 0074  R....(....R$...t
+00003d60: 0300 0000 6c61 6774 0b00 0000 6c61 675f  ....lagt....lag_
+00003d70: 6e6f 5f6e 616d 6528 0000 0000 2800 0000  no_name(....(...
+00003d80: 0073 3100 0000 2f55 7365 7273 2f61 6472  .s1.../Users/adr
+00003d90: 6961 616c 2f52 6570 6f73 6974 6f72 6965  iaal/Repositorie
+00003da0: 732f 4841 4d2f 7465 7374 732f 7465 7374  s/HAM/tests/test
+00003db0: 5f68 616d 2e70 7974 1f00 0000 7465 7374  _ham.pyt....test
+00003dc0: 5f67 6574 5f6c 6973 745f 616e 6365 7374  _get_list_ancest
+00003dd0: 7261 6c5f 6765 6e6f 6d65 73f0 0100 0073  ral_genomes....s
+00003de0: 0800 0000 0002 0f01 2502 0f01 6301 0000  ........%...c...
+00003df0: 0006 0000 0009 0000 0043 0000 0073 6f01  .........C...so.
+00003e00: 0000 7c00 006a 0000 6a01 0064 0100 6402  ..|..j..j..d..d.
+00003e10: 0083 0001 7d01 007c 0000 6a00 006a 0100  ....}..|..j..j..
+00003e20: 6401 0064 0300 8300 017d 0200 7c00 006a  d..d.....}..|..j
+00003e30: 0200 7403 0083 0100 8f18 0001 7c00 006a  ..t.........|..j
+00003e40: 0000 6a04 007c 0200 6801 0083 0100 0157  ..j..|..h......W
+00003e50: 6400 0051 587c 0000 6a02 0074 0500 8301  d..QX|..j..t....
+00003e60: 008f 1b00 017c 0000 6a00 006a 0400 7c02  .....|..j..j..|.
+00003e70: 0064 0400 6802 0083 0100 0157 6400 0051  .d..h......Wd..Q
+00003e80: 587c 0000 6a00 006a 0400 7c01 007c 0200  X|..j..j..|..|..
+00003e90: 6802 0083 0100 7d03 007c 0000 6a06 0064  h.....}..|..j..d
+00003ea0: 0500 7c03 006a 0700 8302 0001 7c00 006a  ..|..j......|..j
+00003eb0: 0000 6a04 007c 0300 7c02 0068 0200 8301  ..j..|..|..h....
+00003ec0: 007d 0400 7c00 006a 0600 6405 007c 0400  .}..|..j..d..|..
+00003ed0: 6a07 0083 0200 017c 0000 6a08 006a 0100  j......|..j..j..
+00003ee0: 6401 0064 0200 8300 017d 0100 7c00 006a  d..d.....}..|..j
+00003ef0: 0800 6a01 0064 0100 6403 0083 0001 7d02  ..j..d..d.....}.
+00003f00: 007c 0000 6a08 006a 0400 7c01 007c 0200  .|..j..j..|..|..
+00003f10: 6802 0083 0100 7d03 007c 0000 6a06 0064  h.....}..|..j..d
+00003f20: 0500 7c03 006a 0700 8302 0001 7c00 006a  ..|..j......|..j
+00003f30: 0200 7409 0083 0100 8f30 0001 7c00 006a  ..t......0..|..j
+00003f40: 0800 6a01 0064 0100 6406 0083 0001 7d05  ..j..d..d.....}.
+00003f50: 007c 0000 6a08 006a 0400 7c01 007c 0500  .|..j..j..|..|..
+00003f60: 6802 0083 0100 0157 6400 0051 5864 0000  h......Wd..QXd..
+00003f70: 5328 0700 0000 4e52 4c00 0000 524d 0000  S(....NRL...RM..
+00003f80: 0052 4f00 0000 5257 0000 0052 d400 0000  .RO...RW...R....
+00003f90: 524e 0000 0028 0a00 0000 528b 0000 0052  RN...(....R....R
+00003fa0: 5600 0000 522c 0000 0074 0a00 0000 5661  V...R,...t....Va
+00003fb0: 6c75 6545 7272 6f72 525c 0000 0052 2d00  lueErrorR\...R-.
+00003fc0: 0000 52a1 0000 0052 4c00 0000 5298 0000  ..R....RL...R...
+00003fd0: 0052 9f00 0000 2806 0000 0052 2400 0000  .R....(....R$...
+00003fe0: 5257 0000 0052 5900 0000 7410 0000 0065  RW...RY...t....e
+00003ff0: 7561 7263 686f 6e74 6f67 6c69 7265 7374  uarchontoglirest
+00004000: 1100 0000 6575 6172 6368 6f6e 746f 676c  ....euarchontogl
+00004010: 6972 6573 3252 5800 0000 2800 0000 0028  ires2RX...(....(
+00004020: 0000 0000 7331 0000 002f 5573 6572 732f  ....s1.../Users/
+00004030: 6164 7269 6161 6c2f 5265 706f 7369 746f  adriaal/Reposito
+00004040: 7269 6573 2f48 414d 2f74 6573 7473 2f74  ries/HAM/tests/t
+00004050: 6573 745f 6861 6d2e 7079 742f 0000 0074  est_ham.pyt/...t
+00004060: 6573 745f 6765 745f 616e 6365 7374 7261  est_get_ancestra
+00004070: 6c5f 6765 6e6f 6d65 5f62 795f 6d72 6361  l_genome_by_mrca
+00004080: 5f6f 665f 6765 6e6f 6d65 5f73 6574 f801  _of_genome_set..
+00004090: 0000 7322 0000 0000 0215 0115 0210 0119  ..s"............
+000040a0: 0210 011c 0218 0113 0318 0113 0615 0115  ................
+000040b0: 0218 0113 0210 0115 0128 1200 0000 5249  .........(....RI
+000040c0: 0000 0052 4a00 0000 5228 0000 0052 a600  ...RJ...R(...R..
+000040d0: 0000 52ac 0000 0052 af00 0000 52b1 0000  ..R....R....R...
+000040e0: 0052 b200 0000 52b8 0000 0052 bd00 0000  .R....R....R....
+000040f0: 52c0 0000 0052 c400 0000 52c7 0000 0052  R....R....R....R
+00004100: cc00 0000 52d1 0000 0052 d300 0000 52da  ....R....R....R.
+00004110: 0000 0052 de00 0000 2800 0000 0028 0000  ...R....(....(..
+00004120: 0000 2800 0000 0073 3100 0000 2f55 7365  ..(....s1.../Use
+00004130: 7273 2f61 6472 6961 616c 2f52 6570 6f73  rs/adriaal/Repos
+00004140: 6974 6f72 6965 732f 4841 4d2f 7465 7374  itories/HAM/test
+00004150: 732f 7465 7374 5f68 616d 2e70 7952 6300  s/test_ham.pyRc.
+00004160: 0000 8100 0000 7320 0000 0006 0209 2f09  ......s ....../.
+00004170: 2709 1d09 0e09 1309 1d09 2709 1809 1a09  '.........'.....
+00004180: 1c09 0c09 1709 1209 1209 0874 0e00 0000  ...........t....
+00004190: 4841 4d54 6573 7450 7269 7661 7465 6300  HAMTestPrivatec.
+000041a0: 0000 0000 0000 0001 0000 0042 0000 0073  ...........B...s
+000041b0: 1100 0000 6500 005a 0100 6400 0084 0000  ....e..Z..d.....
+000041c0: 5a02 0052 5328 0100 0000 6301 0000 0007  Z..RS(....c.....
+000041d0: 0000 000d 0000 0043 0000 0073 bb01 0000  .......C...s....
+000041e0: 7400 006a 0100 6a02 0074 0000 6a01 006a  t..j..j..t..j..j
+000041f0: 0300 7404 0083 0100 6401 0083 0200 7d01  ..t.....d.....}.
+00004200: 0074 0500 6a06 007c 0100 6402 0064 0300  .t..j..|..d..d..
+00004210: 8301 017d 0200 7400 006a 0100 6a02 0074  ...}..t..j..j..t
+00004220: 0000 6a01 006a 0300 7404 0083 0100 6401  ..j..j..t.....d.
+00004230: 0083 0200 7d03 0074 0500 6a06 007c 0300  ....}..t..j..|..
+00004240: 6402 0064 0300 8301 017d 0400 7400 006a  d..d.....}..t..j
+00004250: 0100 6a02 0074 0000 6a01 006a 0300 7404  ..j..t..j..j..t.
+00004260: 0083 0100 6404 0083 0200 7d05 0074 0700  ....d.....}..t..
+00004270: 6a08 007c 0200 7c05 0083 0200 7c00 005f  j..|..|.....|.._
+00004280: 0900 7407 006a 0800 7c04 007c 0500 8302  ..t..j..|..|....
+00004290: 007c 0000 5f0a 0064 0500 6406 0064 0700  .|.._..d..d..d..
+000042a0: 6408 0068 0400 7c00 005f 0b00 6409 0064  d..h..|.._..d..d
+000042b0: 0a00 640b 0064 0c00 6804 007c 0000 5f0c  ..d..d..h..|.._.
+000042c0: 0064 0d00 640e 0064 0f00 6410 0068 0400  .d..d..d..d..h..
+000042d0: 7c00 005f 0d00 6409 0068 0100 7c00 005f  |.._..d..h..|.._
+000042e0: 0e00 6411 0064 1200 6802 007c 0000 5f0f  ..d..d..h..|.._.
+000042f0: 0064 1300 6414 0064 1500 6416 0064 1700  .d..d..d..d..d..
+00004300: 6418 0064 1900 641a 0064 1b00 641c 0064  d..d..d..d..d..d
+00004310: 1d00 641e 0064 1f00 680d 007c 0000 5f10  ..d..d..h..|.._.
+00004320: 0064 2000 6421 0064 2200 6423 0064 2400  .d .d!.d".d#.d$.
+00004330: 6425 0064 2600 6427 0064 2800 6429 0064  d%.d&.d'.d(.d).d
+00004340: 2a00 642b 0064 2c00 680d 007c 0000 5f11  *.d+.d,.h..|.._.
+00004350: 0064 1300 6419 0068 0200 7c00 005f 1200  .d..d..h..|.._..
+00004360: 7407 006a 1300 8300 007d 0600 7c06 006a  t..j.....}..|..j
+00004370: 1400 642d 0067 0100 8301 0001 7407 006a  ..d-.g......t..j
+00004380: 0800 7c02 007c 0500 642e 007c 0600 8302  ..|..|..d..|....
+00004390: 017c 0000 5f15 0064 0000 5328 2f00 0000  .|.._..d..S(/...
+000043a0: 4e73 1300 0000 2e2f 6461 7461 2f73 696d  Ns...../data/sim
+000043b0: 706c 6545 782e 6e77 6b52 1300 0000 5214  pleEx.nwkR....R.
+000043c0: 0000 0073 1800 0000 2e2f 6461 7461 2f73  ...s...../data/s
+000043d0: 696d 706c 6545 782e 6f72 7468 6f78 6d6c  impleEx.orthoxml
+000043e0: 524d 0000 0052 4f00 0000 5268 0000 0052  RM...RO...Rh...R
+000043f0: 5100 0000 5269 0000 0052 6a00 0000 526b  Q...Ri...Rj...Rk
+00004400: 0000 0052 6c00 0000 526d 0000 0052 6e00  ...Rl...Rm...Rn.
+00004410: 0000 526f 0000 0052 7000 0000 524e 0000  ..Ro...Rp...RN..
+00004420: 0052 5000 0000 5271 0000 0052 7200 0000  .RP...Rq...Rr...
+00004430: 5273 0000 0052 7400 0000 5275 0000 0052  Rs...Rt...Ru...R
+00004440: 7600 0000 5277 0000 0052 7800 0000 5279  v...Rw...Rx...Ry
+00004450: 0000 0052 7a00 0000 527b 0000 0052 7c00  ...Rz...R{...R|.
+00004460: 0000 527d 0000 0052 7e00 0000 527f 0000  ..R}...R~...R...
+00004470: 0052 8000 0000 5281 0000 0052 8200 0000  .R....R....R....
+00004480: 5283 0000 0052 8400 0000 5285 0000 0052  R....R....R....R
+00004490: 8600 0000 5287 0000 0052 8800 0000 5289  ....R....R....R.
+000044a0: 0000 0052 8a00 0000 6902 0000 0052 3f00  ...R....i....R?.
+000044b0: 0000 2816 0000 0052 1800 0000 5219 0000  ..(....R....R...
+000044c0: 0052 1a00 0000 521b 0000 0052 1c00 0000  .R....R....R....
+000044d0: 5200 0000 0052 1d00 0000 5201 0000 0052  R....R....R....R
+000044e0: 2e00 0000 528b 0000 0052 8c00 0000 528e  ....R....R....R.
+000044f0: 0000 0052 8f00 0000 5290 0000 0052 9100  ...R....R....R..
+00004500: 0000 5292 0000 0052 9300 0000 5294 0000  ..R....R....R...
+00004510: 0052 9500 0000 5296 0000 0052 9700 0000  .R....R....R....
+00004520: 5298 0000 0028 0700 0000 5224 0000 0052  R....(....R$...R
+00004530: 2500 0000 521e 0000 0052 9b00 0000 529c  %...R....R....R.
+00004540: 0000 0052 2000 0000 529d 0000 0028 0000  ...R ...R....(..
+00004550: 0000 2800 0000 0073 3100 0000 2f55 7365  ..(....s1.../Use
+00004560: 7273 2f61 6472 6961 616c 2f52 6570 6f73  rs/adriaal/Repos
+00004570: 6974 6f72 6965 732f 4841 4d2f 7465 7374  itories/HAM/test
+00004580: 732f 7465 7374 5f68 616d 2e70 7952 2800  s/test_ham.pyR(.
+00004590: 0000 1b02 0000 7326 0000 0000 0221 0115  ......s&.....!..
+000045a0: 0221 0115 0221 0315 0315 0415 0115 0115  .!...!..........
+000045b0: 010c 010f 0130 0115 011b 010f 010c 0110  .....0..........
+000045c0: 0128 0300 0000 5249 0000 0052 4a00 0000  .(....RI...RJ...
+000045d0: 5228 0000 0028 0000 0000 2800 0000 0028  R(...(....(....(
+000045e0: 0000 0000 7331 0000 002f 5573 6572 732f  ....s1.../Users/
+000045f0: 6164 7269 6161 6c2f 5265 706f 7369 746f  adriaal/Reposito
+00004600: 7269 6573 2f48 414d 2f74 6573 7473 2f74  ries/HAM/tests/t
+00004610: 6573 745f 6861 6d2e 7079 52df 0000 0019  est_ham.pyR.....
+00004620: 0200 0073 0200 0000 0602 7408 0000 005f  ...s......t...._
+00004630: 5f6d 6169 6e5f 5f28 0f00 0000 7408 0000  _main__(....t...
+00004640: 0075 6e69 7474 6573 7474 0500 0000 7079  .unittestt....py
+00004650: 6861 6d52 0000 0000 5201 0000 0052 3200  hamR....R....R2.
+00004660: 0000 5218 0000 0052 0a00 0000 5210 0000  ..R....R....R...
+00004670: 0074 0800 0000 5465 7374 4361 7365 5211  .t....TestCaseR.
+00004680: 0000 0052 4b00 0000 5263 0000 0052 df00  ...RK...Rc...R..
+00004690: 0000 5249 0000 0074 0400 0000 6d61 696e  ..RI...t....main
+000046a0: 2800 0000 0028 0000 0000 2800 0000 0073  (....(....(....s
+000046b0: 3100 0000 2f55 7365 7273 2f61 6472 6961  1.../Users/adria
+000046c0: 616c 2f52 6570 6f73 6974 6f72 6965 732f  al/Repositories/
+000046d0: 4841 4d2f 7465 7374 732f 7465 7374 5f68  HAM/tests/test_h
+000046e0: 616d 2e70 7974 0800 0000 3c6d 6f64 756c  am.pyt....<modul
+000046f0: 653e 0100 0000 731a 0000 000c 0110 0110  e>....s.........
+00004700: 010c 010c 0309 0609 0719 4c19 2019 ff00  ..........L. ...
+00004710: 9919 210c 01                             ..!..
```

### Comparing `pyham-1.1.8/docs/index.rst` & `pyham-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/docs/Makefile` & `pyham-1.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/setup.py` & `pyham-1.1.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import os
 import sys
 from io import open
 
 
 name = 'pyham'
-requirements = ['ete3', 'six', 'lxml', 'future','coreapi']
+requirements = ['ete3 >= 3.1', 'six', 'lxml', 'future']
 if sys.version_info > (3, 3):
     # ete3 uses some py3 incompatible types if scipy is not present 
     requirements.extend(['scipy'])  
 
 __version__ = "Undefined"
 for line in open('{}/__init__.py'.format(name.lower())):
     if line.startswith('__version__'):
@@ -43,19 +43,21 @@
          'Intended Audience :: Developers',
          'Intended Audience :: Science/Research',
          'Topic :: Scientific/Engineering :: Bio-Informatics',
          'License :: OSI Approved :: MIT License',
          'Programming Language :: Python :: 2',
          'Programming Language :: Python :: 2.7',
          'Programming Language :: Python :: 3',
-         'Programming Language :: Python :: 3.4',
          'Programming Language :: Python :: 3.5',
          'Programming Language :: Python :: 3.6',
+         'Programming Language :: Python :: 3.7',
+         'Programming Language :: Python :: 3.8',
+         'Programming Language :: Python :: 3.9',
          ],
 
     packages=find_packages(exclude=[]),
     install_requires=requirements,
     extras_require={
-        'test': ['noise'],
-        'dev': ['noise', 'sphinx', 'wheel', 'twine', 'fabric', 'fabric3'],
+        'test': ['nose'],
+        'dev': ['nose', 'sphinx', 'wheel', 'twine', 'fabric', 'fabric3'],
     }
 )
```

### Comparing `pyham-1.1.8/pyham.egg-info/PKG-INFO` & `pyham-1.1.9/pyham.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyham
-Version: 1.1.8
+Version: 1.1.9
 Summary: A tool to analyse Hierarchical Orthologous Groups (HOGs)
 Home-page: http://lab.dessimoz.org/ham
 Author: Dessimoz Lab - Laboratory of Computational Evolutionary Biology and Genomics
 Author-email: adrian.altenhoff@inf.ethz.ch
 License: MIT
 Description: pyHam: A Tool to Analyze Hierarchical Orthologous Groups (HOGs)
         ===============================================================
@@ -116,12 +116,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dev
 Provides-Extra: test
```

### Comparing `pyham-1.1.8/pyham.egg-info/SOURCES.txt` & `pyham-1.1.9/pyham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/README.rst` & `pyham-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/pyham/ham.py` & `pyham-1.1.9/pyham/ham.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from __future__ import absolute_import
 from __future__ import unicode_literals
 from __future__ import print_function
 from __future__ import division
+
+import gzip
+import re
 from builtins import map
 from builtins import open
 from builtins import str
 from future import standard_library
 standard_library.install_aliases()
 
 from xml.etree.ElementTree import XMLParser
@@ -14,16 +17,16 @@
 from . import parsers
 from . import mapper
 from . import abstractgene
 from .TreeProfile import TreeProfile
 import logging
 import copy
 import io
-import coreapi
-from urllib.request import urlopen
+
+
 
 
 logger = logging.getLogger(__name__)
 
 
 class ParserFilter(object):
     """
@@ -128,15 +131,16 @@
         | taxonomy: (:obj:`pyham.mapper.Taxonomy`): :obj:`pyham.pyham.Taxonomy` build and used by :obj:`pyham.pyham.Ham` instance.
         | orthoXML_as_string (:obj:`Bool`) If set to true, hog_file is a string of an orthoxml file. Defaults to False.
 
     """
 
     def __init__(self, tree_file=None, hog_file=None, type_hog_file="orthoxml", filter_object=None, use_internal_name=False,\
                  orthoXML_as_string=False, tree_format='newick_string', phyloxml_internal_name_tag='taxonomy_scientific_name', \
-                 phyloxml_leaf_name_tag='taxonomy_scientific_name', use_data_from=None, query_database=None):
+                 phyloxml_leaf_name_tag='taxonomy_scientific_name', use_data_from=None, query_database=None,
+                 species_resolve_mode=None):
         """
 
         Args:
             | tree_file (:obj:`str`): Path to the file that contained the taxonomy information.
             | hog_file (:obj:`str`): Path to the file that contained the HOGs information.
             | type_hog_file (:obj:`str`, optional): File type of the hog_file. Can be "orthoxml or "hdf5". Defaults to "orthoxml".
             | filter_object (:obj:`pyham.pyham.ParserFilter`, optional): :obj:`pyham.pyham.ParserFilter` used during the instantiation of pyham.pyham.Ham. Defaults to None.
@@ -147,56 +151,40 @@
             | phyloxml_internal_name_tag (:obj:`str`) tag to use in the phyloxml to name the ancestral species (internal nodes). Defaults will use taxonomy.scientific_name to populate species names.
             available options: 'clade_name', 'taxonomy_scientific_name', 'taxonomy_code'. Beware than missing species names will stop pyham working.
             | use_data_from (:obj:`str`) if specified,  use data from a remote databaseto populate pyHam. Defaults to None. Options: 'oma'.
             | query_database (:obj:`str`) if use_data_from is specified, use this as a query to fetch the orthoxml and \
             tree information for the related query hog (gene family). For 'oma', this correspond to the oma gene id (e.g. 'HUMAN12' or 'CHIMP1435').
         """
 
-        if use_data_from!=None:
+        if use_data_from is not None:
             if query_database is None:
-                raise TypeError(
-                    "query_database argument can't be empty.")
+                raise TypeError("query_database argument can't be empty.")
 
             if use_data_from == 'oma':
 
-                # Initialize a client & load the schema document
-                client = coreapi.Client()
-                schema = client.get("https://omabrowser.org/api/docs")
-
-                # Get the gene data
-                try:
-
-                    action_gene = ["protein", "read"]
-                    params_gene = {
-                        "entry_id": query_database,
-                    }
-
-                    gene = client.action(schema, action_gene, params=params_gene)
-                    top_level = gene['hog_levels'][-1]
-
-                except coreapi.exceptions.ErrorMessage as exc:
-                    raise TypeError("{} is not a valid oma Id".format(query_database))
-
-                # Get the phyloxml data
-                action_phy = ["taxonomy", "read"]
-                params_phy = {
-                    "type": 'phyloxml',
-                    "root_id": top_level,
-                }
-
-                open_tax = client.action(schema, action_phy, params=params_phy)
+                import requests
+                protein_url = "https://omabrowser.org/api/protein/{}/".format(query_database)
+                res = requests.get(protein_url)
+                if not res.ok:
+                    res.raise_for_status()
+                gene = res.json()
+                top_level = gene['hog_levels'][-1]
+
+                rep_tax = requests.get("https://omabrowser.org/api/taxonomy/{}/".format(top_level),
+                                       params={"type": "phyloxml"})
+                if not rep_tax.ok:
+                    rep_tax.raise_for_status()
 
                 self.tree_file = 'taxonomy_from_oma_open_at_{}.phyloxml'.format(top_level)
-
                 with open(self.tree_file, 'w') as f:
-                    f.write(open_tax.read().decode())
+                    f.write(rep_tax.text)
 
                 # Get the phyloxml data
-                oma_url = 'https://omabrowser.org/oma/hogs/{}/orthoxml'.format(gene['omaid'])
-                self.hog_file = urlopen(oma_url).read().decode('utf-8')
+                oma_url = 'https://omabrowser.org/oma/hog/{}/orthoxml/'.format(gene['oma_hog_id'])
+                self.hog_file = requests.get(oma_url).text
                 self.hog_file_type = type_hog_file
 
                 self.orthoXML_as_string = True
                 use_internal_name = True
                 tree_format = 'phyloxml'
 
             elif use_data_from == 'ensembl':
@@ -231,15 +219,15 @@
 
         # Taxonomy
 
         accepted_tag_phyloxml = ['clade_name', 'taxonomy_scientific_name', 'taxonomy_code']
 
         if phyloxml_leaf_name_tag not in accepted_tag_phyloxml or phyloxml_internal_name_tag not in accepted_tag_phyloxml:
             raise TypeError("{} is an invalid type phyloxml tag name")
-
+        self.species_resolve_mode = species_resolve_mode
         self.taxonomy = tax.Taxonomy(self.tree_file, tree_format=tree_format, use_internal_name=use_internal_name, phyloxml_leaf_name_tag=phyloxml_leaf_name_tag, phyloxml_internal_name_tag=phyloxml_internal_name_tag)
         logger.info('Build taxonomy: completed.')
 
         # Misc. information
         self.top_level_hogs = None
         self.extant_gene_map = None
         self.external_id_mapper = None
@@ -252,28 +240,30 @@
             if self.filter_obj is not None:
 
                 if self.orthoXML_as_string == True:
                     with io.StringIO(self.hog_file)  as orthoxml_file:
                         self.filter_obj.buildFilter(orthoxml_file, self.hog_file_type)
 
                 else:
-                    with open(self.hog_file, 'r') as orthoxml_file:
+                    open_ = gzip.open if self.hog_file.endswith('.gz') else open
+                    with open_(self.hog_file, 'rt') as orthoxml_file:
                         self.filter_obj.buildFilter(orthoxml_file, self.hog_file_type)
 
                 logger.info('Filtering Indexing of Orthoxml done: {} top level hogs and {} extant genes will be extract.'.format(
                                 len(self.filter_obj.hogsId),
                                 len(self.filter_obj.geneUniqueId)))
 
             if self.orthoXML_as_string == True:
                 with io.StringIO(self.hog_file) as orthoxml_file:
                     self.top_level_hogs, self.extant_gene_map, self.external_id_mapper = self._build_hogs_and_genes(orthoxml_file, filter_object=self.filter_obj)
 
             else:
                 # This is the actual parser to build HOG/Gene and related Genomes.
-                with open(self.hog_file, 'r') as orthoxml_file:
+                open_ = gzip.open if self.hog_file.endswith('.gz') else open
+                with open_(self.hog_file, 'rt') as orthoxml_file:
                     self.top_level_hogs, self.extant_gene_map, self.external_id_mapper = self._build_hogs_and_genes(orthoxml_file, filter_object=self.filter_obj)
 
             logger.info('Parse Orthoxml: {} top level hogs and {} extant genes extract.'.format(len(self.top_level_hogs),len(self.extant_gene_map)))
 
         elif self.hog_file_type == "hdf5":
             # Looping through all orthoXML within the hdf5
             #   for each run self.build_...
@@ -874,14 +864,25 @@
         """
 
         nodes_founded = self.taxonomy.tree.search_nodes(name=kwargs['name'])
 
         if len(nodes_founded) == 1:
 
             node = nodes_founded[0]
+            if len(node.children) > 0 and self.species_resolve_mode == "OMA":
+                cand = []
+                for child in node.children:
+                    if len(child.name) == 5 and re.match(r'[A-Z][A-Z0-9]{4}', child.name) is not None:
+                        cand.append(child)
+                if len(cand) == 1:
+                    node = cand[0]
+                    kwargs['name'] = node.name
+            if len(node.children) > 0:
+                raise TypeError("species name '{}' maps to an ancestral name, not a leaf of the taxonomy"
+                                .format(kwargs["name"]))
 
             if "genome" in node.features:
                 return node.genome
 
             else:
                 extant_genome = ExtantGenome(**kwargs)
                 self.taxonomy.add_genome_to_node(node, extant_genome)
```

### Comparing `pyham-1.1.8/pyham/TreeProfile.py` & `pyham-1.1.9/pyham/TreeProfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import json
 
 logger = logging.getLogger(__name__)
 
 
 class TreeProfile(object):
     """
-    Object that map on each node of the Ham species tree the related evolutionary information such as the number of 
+    Object that map on each node of the Ham species tree the related evolutionary information such as the number of
     genes the related genome contains or the number of evolutionary events (duplications, genes loss or gain of genes)
     that occurs between the parent node and itself. This can be either applied to the full Ham comparative genomic setup
     or for a specific HOG.
 
     Attributes:
         | pyham (:obj:`pyham.pyham.Ham`): :obj:`set` of HOG ids used by the FilterOrthoXMLParser.
         | hog (:obj:`pyham.abstractgene.HOG`, optional): If specified, compute TreeProfile on a single HOGs. Defaults is None.
@@ -35,15 +35,15 @@
 
         elif isinstance(hog, HOG):
             self.treemap = self.computeTP_hog(hog)
         else:
             raise TypeError("Invalid argument {} for HOG".format(hog))
 
     def computeTP_hog(self, hog):
-        """  
+        """
         Create the treeMap object (ete3 Etree object with annotated nodes) that contained the following features for
         each nodes (representing an AbstractGene):
             - nbr_genes: numbers of HOG/Gene the genome contains. For leaves, it also counts the singletons.
             - dupl: numbers of HOGs that have arose by duplication in between this node and its parent.
             - retained: numbers of HOGs that have stay retained (in term of copy numbers) in between this node and
             its parent.
             - lost: numbers of HOGs that have been lost in between this node and its parent.
@@ -68,15 +68,16 @@
         # create a dictionary that map node with related hogs/genes
         levelGroups = {}
         for lvl in treeMap.traverse():
             levelGroups[lvl.name]=[]
 
         # add all of subhog to the related level in levelGroups
         for subhog in hog.get_all_descendant_hogs():
-            levelGroups[subhog.genome.name].append(subhog)
+            if subhog.genome.name in levelGroups:
+                levelGroups[subhog.genome.name].append(subhog)
 
         # add empty extant genome to levelGroups
         for extantGenome in treeMap.get_leaves():
             levelGroups[extantGenome.name] = []
 
         # add genes to related extant genome in levelGroups
         for species, genes in hog.get_all_descendant_genes_clustered_by_species().items():
@@ -126,26 +127,26 @@
             lvl.add_feature("retained", cpt_ident)
             lvl.add_feature("nbr_events", nbr_ev)
             lvl.add_feature("duplication", cpt_duplication)
 
         return treeMap
 
     def compute_tree_profile_full(self):
-        """  
+        """
         Create the treeMap object (ete3 Etree object with annotated nodes) that contained the following features for
         each nodes (the root node contains only nbr_genes):
             - nbr_genes: numbers of HOG/Gene the genome contains. For leaves, it also counts the singletons.
             - dupl: numbers of HOGs that have arose by duplication in between this node and its parent.
             - lost: numbers of HOGs that have been lost in between this node and its parent.
             - gain: numbers of HOGs that have "emerged" at this node.
             - retained: numbers of HOGs that have stay retained (in term of copy numbers) in between this node and
             its parent.
-            
+
         In order to get all those node informations, the HOGMap between each node and its parent is computed.
-            
+
         Returns:
             TreeMap
         """
 
         def _add_annot(node, nbr, dupl, lost, gain, retained, duplication, nbr_ev):
             node.add_feature("nbr_genes", nbr)
             node.add_feature("nbr_events", nbr_ev)
@@ -189,19 +190,19 @@
 
                 _add_annot(node, nbr, nbr_duplicate, len(hogmap.LOSS), len(hogmap.GAIN), len(hogmap.RETAINED.keys()), hogmap.number_duplication, nbr_ev)
 
         return treeMap
 
     def export(self, output, layout_function=None, display_internal_histogram=True):
 
-        """  
+        """
         Method to export the tree profile object as figure (available format .SVG, .PDF, .PNG).
-        
+
         -- Some magic going there --
-        
+
         Args:
             | output (:obj:`str`): output file name. The extension of output will set the format of the figure (SVG, .PDF, .PNG)
             | layout_function (:obj:`function`, optional): custom layout_fn for ete3 TreeStyle.
             | display_internal_histogram (:obj:`Boolean`, optional): Display internal node as histogram or raw text with numbers. Defaults to True.
         """
 
         from ete3 import TreeStyle, TextFace, NodeStyle, BarChartFace
@@ -286,15 +287,15 @@
             ts.legend.add_face(BarChartFace(_values_legend, deviations=None, width=w_legend, height=25, colors=_color_scheme, labels=_label_legend, min_value=0, max_value=max_genes, label_fsize=6, scale_fsize=6),column=0)
             ts.legend_position = 3
 
         self.treemap.render(output,tree_style=ts)
 
     def export_as_html(self, output ):
 
-        """  
+        """
         Method to export the tree profile object as an interactive tool embedded into a html file.
 
 
         Args:
             | output (:obj:`str`): output file name. If filename finish by .html, a double click load the file into your default browser.
         """
 
@@ -349,29 +350,29 @@
             <script type="text/javascript" src="https://cdn.rawgit.com/DessimozLab/phylo-io/5e89fafc3b1746b22da33c20b2af621d5807b6fb/www/js/FileSaver.min.js"></script>
             <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.0.8/css/solid.css" integrity="sha384-v2Tw72dyUXeU3y4aM2Y0tBJQkGfplr39mxZqlTBDUZAb9BGoC40+rdFCG0m10lXk" crossorigin="anonymous">
             <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.0.8/css/fontawesome.css" integrity="sha384-q3jl8XQu1OpdLgGFvNRnPdj5VIlCvgsDQTQB6owSOHWlAurxul7f+JpUOVdAiJ5P" crossorigin="anonymous">
             <link rel="stylesheet" type="text/css" href="https://cdn.rawgit.com/DessimozLab/phylo-io/5e89fafc3b1746b22da33c20b2af621d5807b6fb/www/css/bootstrap.min.css">
             <link rel="stylesheet" type="text/css" href="https://cdn.rawgit.com/DessimozLab/phylo-io/5e89fafc3b1746b22da33c20b2af621d5807b6fb/www/css/bootstrap-theme.min.css">
             <link rel="stylesheet" type="text/css" href="https://cdn.rawgit.com/DessimozLab/phylo-io/5e89fafc3b1746b22da33c20b2af621d5807b6fb/www/css/style.css">
             <style>
-            
+
             text {{stroke: none;}}
-            
+
             #help_modal_button {{
                 position: fixed;
                 right: 10px;
                 margin-right: 10px; /*magic number */
                 bottom: 10px;
                 z-index: 99;
             }}
-            
+
             </style>
         </head>
         <body id="phylo">
-        
+
         <!-- Modal -->
         <div class="modal  fade bs-example-modal-lg" id="myModal" tabindex="-1" role="dialog" aria-labelledby="myModalLabel">
             <div class="modal-dialog modal-lg" role="document">
                 <div class="modal-content">
                     <div class="modal-header">
                         <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
                         <h4 class="modal-title" id="myModalLabel">Tree profile help</h4>
@@ -388,17 +389,17 @@
         </div>
 
 
         <!-- Button trigger modal -->
         <button id="help_modal_button" type="button" class="btn btn-sm" data-toggle="modal" data-target="#myModal">
             Help
         </button>
-        
-        
-        
+
+
+
         <div id="vis-container1" style="width: 100%; height: 100%;">
         <div id="scale-1"> </div>
         </div>
         <script type="text/javascript">
             var treecomp = TreeCompare().init({{
                 enableScale: true,
                 scaleColor: "black",
```

### Comparing `pyham-1.1.8/pyham/mapper.py` & `pyham-1.1.9/pyham/mapper.py`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/pyham/abstractgene.py` & `pyham-1.1.9/pyham/abstractgene.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         Attributes:
             | arose_by_duplication (:obj:`Bool`): True if this AbstractGene arose by a duplication from its parent.
             | ** kwargs: dictionary of attribute and value required to create the: obj:`pyham.abstractgene.AbstractGene`.
         """
 
         self.parent = None
         self.genome = None
+        self._properties = {}
         self.arose_by_duplication = arose_by_duplication
 
     @abc.abstractmethod
     def set_genome(self, genome):
         """Set the genome attribute using the given :obj:`Genome`."""
         pass
 
@@ -132,14 +133,20 @@
 
         for e in rlist:
             if e == self:
                 raise KeyError("get level cannot return itself".format())
 
         return rlist
 
+    def add_property(self, name, value):
+        self._properties[name] = value
+
+    def __getitem__(self, item):
+        return self._properties[item]
+
 
 class HOG(AbstractGene):
 
     """  
     HOG class represents ancestral genes. An AbstractGene is defined the genome it belongs to and its child/parent
     AbstractGene. Only top level HOG doesn't have parent attribute (set to None).
```

### Comparing `pyham-1.1.8/pyham/parsers.py` & `pyham-1.1.9/pyham/parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,16 +69,16 @@
 
     def _build_gene(self, attrib):
         gene = abstractgene.Gene(**attrib)
         gene.set_genome(self.current_species)
         self.current_species.add_gene(gene)
         self.extant_gene_map[gene.unique_id] = gene
         for type, Id in attrib.items():
-            if type is not "id":
-                self.external_id_mapper.setdefault(Id,[]).append(gene.unique_id)
+            if type != "id":
+                self.external_id_mapper.setdefault(Id, []).append(gene.unique_id)
 
     def _build_hog(self, attrib):
 
         hog = abstractgene.HOG(arose_by_duplication=False, **attrib)
 
         if self.in_paralogGroup == len(self.hog_stack):
             self.paralogyNode.add_child(hog)
@@ -131,19 +131,18 @@
                 self._build_hog(attrib)
 
 
 
         elif tag == "{http://orthoXML.org/2011/}orthologGroup" and self.skip_this_hog is True:
             self.hog_stack.append(0)
 
-        elif tag == "{http://orthoXML.org/2011/}property" and attrib['name'] == "TaxRange":
-            #self.hog_stack[-1].set_genome(attrib["value"])
-            pass
+        elif tag == "{http://orthoXML.org/2011/}property" and not self.skip_this_hog:
+            self.hog_stack[-1].add_property(attrib["name"], attrib["value"])
 
-        elif tag == "{http://orthoXML.org/2011/}score" and self.skip_this_hog is False:
+        elif tag == "{http://orthoXML.org/2011/}score" and not self.skip_this_hog:
             self.hog_stack[-1].score(attrib['id'], float(attrib['value']))
 
     def end(self, tag):
 
         if tag == "{http://orthoXML.org/2011/}species":
             logger.info("Species {} created. ".format(self.current_species.name))
             self.current_species = None
@@ -165,99 +164,105 @@
 
             # get the latest hog
             hog = self.hog_stack.pop()
 
             if self.skip_this_hog:
                 if len(self.hog_stack) == 0:
                     self.skip_this_hog = False
-
             else:
-
-                # get the ancestral genome related to this hog based on it's children
-                if len(set([child.genome for child in hog.children])) == 1:
-                    ancestral_genome = self.ham_object._get_ancestral_genome_by_taxon(hog.children[0].genome.taxon.up)
-
-                else:
-                    ancestral_genome = self.ham_object._get_ancestral_genome_by_mrca_of_hog_children_genomes(hog)
-
-                hog.set_genome(ancestral_genome)
-                ancestral_genome.taxon.genome.add_gene(hog)
-
-                # get all child clustered by dup if any
-                child_by_duplication = defaultdict(list)
-                for child in hog.children:
-                    if child.arose_by_duplication != False:
-                        child_by_duplication[child.arose_by_duplication].append(child)
-
-                # For each duplication
-                for duplication, children in child_by_duplication.items():
-
-                    # add MRCA hog if its missing
-                    if duplication.MRCA != hog.genome:
-
-                        # create the MRCA hog
-                        mrcahog = abstractgene.HOG()
-                        mrcahog.set_genome(duplication.MRCA)
-                        duplication.MRCA.add_gene(mrcahog)
-
-                        hog.add_child(mrcahog)
-
-                        # add missing level down (from mrcaHOG to duplicated child)
-                        for child in children:
-                            hog.remove_child(child)
-                            mrcahog.add_child(child)
-
-                            change = self.ham_object.taxonomy.get_path_up(child.genome.taxon, mrcahog.genome.taxon)
-                            self.ham_object._add_missing_taxon(child, mrcahog, change)
-
-                        duplication.set_parent(mrcahog)
-
-                        for x in list(duplication.children):
-                            duplication.remove_child(x)
-
-                        for y in list(mrcahog.children):
-                            duplication.add_child(y)
-
-                    # Otherwise simply add missing taxa between hog and duplicated child
+                try:
+                    # get the ancestral genome related to this hog based on it's children
+                    if len(set([child.genome for child in hog.children])) == 1:
+                        try:
+                            if hog['TaxRange'] == hog.children[0].genome.name:
+                                # remove this hog structure.
+                                for child in hog.children:
+                                    child.parent = hog.parent
+                                hog.parent.children.remove(hog)
+                                hog.parent.children.extend(hog.children)
+                                if hog.arose_by_duplication != False:
+                                    dupl_node = hog.arose_by_duplication
+                                    dupl_node.remove_child(hog)
+                                    for child in hog.children:
+                                        dupl_node.add_child(child)
+                                    self.paralog_stack[-1]['depth'] -= 1
+                                return
+                        except KeyError:
+                            pass
+                        ancestral_genome = self.ham_object._get_ancestral_genome_by_taxon(hog.children[0].genome.taxon.up)
                     else:
+                        ancestral_genome = self.ham_object._get_ancestral_genome_by_mrca_of_hog_children_genomes(hog)
 
-                        duplication.set_parent(hog)
-
-                        for child_direct in children:
-
-                            change = self.ham_object.taxonomy.get_path_up(child_direct.genome.taxon, hog.genome.taxon)
-                            self.ham_object._add_missing_taxon(child_direct, hog, change)
-
-                            duplication.remove_child(child_direct)
-                            duplication.add_child(hog.children[-1])
-
-                    #duplication.children = list(set(duplication.children)) # this should be fix by add list() to duplication.children
-
-                hog_genome = hog.genome
-                change = {} # {child -> [intermediate level]}
-
-                # for all children of this hog find missing level
-                for child in hog.children:
-                    child_genome = child.genome
-                    if hog_genome.taxon.depth != child_genome.taxon.depth - 1:
-                        change[child] = self.ham_object.taxonomy.get_path_up(child_genome.taxon, hog_genome.taxon)
-
-                # and add them if required
-                for hog_child, missing in change.items():
-                    self.ham_object._add_missing_taxon(hog_child, hog, missing)
-
-
-                if len(self.hog_stack) == 0:
-
-                    self.toplevel_hogs[hog.hog_id] = hog
-
-                    self.cpt += 1
+                    hog.set_genome(ancestral_genome)
+                    ancestral_genome.taxon.genome.add_gene(hog)
 
-                    if self.cpt % 500 == 0:
-                        logger.info("{} HOGs parsed. ".format(self.cpt))
+                    # get all child clustered by dup if any
+                    child_by_duplication = defaultdict(list)
+                    for child in hog.children:
+                        if child.arose_by_duplication != False:
+                            child_by_duplication[child.arose_by_duplication].append(child)
+
+                    # For each duplication
+                    for duplication, children in child_by_duplication.items():
+
+                        # add MRCA hog if its missing
+                        if duplication.MRCA != hog.genome:
+
+                            # create the MRCA hog
+                            mrcahog = abstractgene.HOG()
+                            mrcahog.set_genome(duplication.MRCA)
+                            duplication.MRCA.add_gene(mrcahog)
+
+                            hog.add_child(mrcahog)
+
+                            # add missing level down (from mrcaHOG to duplicated child)
+                            for child in children:
+                                hog.remove_child(child)
+                                mrcahog.add_child(child)
+
+                                change = self.ham_object.taxonomy.get_path_up(child.genome.taxon, mrcahog.genome.taxon)
+                                self.ham_object._add_missing_taxon(child, mrcahog, change)
+
+                            duplication.set_parent(mrcahog)
+                            for x in list(duplication.children):
+                                duplication.remove_child(x)
+                            for y in list(mrcahog.children):
+                                duplication.add_child(y)
+
+                        # Otherwise simply add missing taxa between hog and duplicated child
+                        else:
+                            duplication.set_parent(hog)
+                            for child_direct in children:
+                                change = self.ham_object.taxonomy.get_path_up(child_direct.genome.taxon, hog.genome.taxon)
+                                self.ham_object._add_missing_taxon(child_direct, hog, change)
+
+                                duplication.remove_child(child_direct)
+                                duplication.add_child(hog.children[-1])
+
+                    hog_genome = hog.genome
+                    change = {} # {child -> [intermediate level]}
+
+                    # for all children of this hog find missing level
+                    for child in hog.children:
+                        child_genome = child.genome
+                        if hog_genome.taxon.depth != child_genome.taxon.depth - 1:
+                            change[child] = self.ham_object.taxonomy.get_path_up(child_genome.taxon, hog_genome.taxon)
+
+                    # and add them if required
+                    for hog_child, missing in change.items():
+                        self.ham_object._add_missing_taxon(hog_child, hog, missing)
+
+                    if len(self.hog_stack) == 0:
+                        self.toplevel_hogs[hog.hog_id] = hog
+                        self.cpt += 1
+                        if self.cpt % 500 == 0:
+                            logger.info("{} HOGs parsed. ".format(self.cpt))
+                except Exception as e:
+                    logger.error("cannot parse HOG '{}': {}".format(hog.hog_id, e))
+                    raise
 
     def data(self, data):
         # Ignore data inside nodes
         pass
 
     def close(self):
         # Nothing special to do here
```

### Comparing `pyham-1.1.8/pyham/iham.py` & `pyham-1.1.9/pyham/iham.py`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/pyham/utils.py` & `pyham-1.1.9/pyham/utils.py`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/pyham/taxonomy.py` & `pyham-1.1.9/pyham/taxonomy.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,20 +239,20 @@
                     "Node {} in the phyloxml file {} have no taxonomy scientific code  to populate the species name".format(
                         node, self.tree_file))
 
     def _build_tree(self, tree_file, tree_format):
 
         if tree_format == 'newick_string':
             self.tree_str = tree_file
-            return ete3.Tree(self.tree_str, format=1)
+            return ete3.Tree(self.tree_str, quoted_node_names=True, format=1)
 
         elif tree_format == 'newick':
             with open(tree_file, 'r') as nwk_file:
                 self.tree_str = nwk_file.read()
-            return ete3.Tree(self.tree_str, format=1)
+            return ete3.Tree(self.tree_str, quoted_node_names=True, format=1)
 
         elif tree_format == 'phyloxml':
             from ete3 import Phyloxml
             project = Phyloxml()
             project.build_from_file(tree_file)
             self.tree_str = None
```

### Comparing `pyham-1.1.8/pyham/genome.py` & `pyham-1.1.9/pyham/genome.py`

 * *Files identical despite different names*

### Comparing `pyham-1.1.8/LICENSE.txt` & `pyham-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

