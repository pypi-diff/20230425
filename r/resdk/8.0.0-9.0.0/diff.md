# Comparing `tmp/resdk-8.0.0.tar.gz` & `tmp/resdk-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/resdk-8.0.0.tar", last modified: Tue Nov 20 10:23:48 2018, max compression
+gzip compressed data, was "dist/resdk-9.0.0.tar", last modified: Thu Feb 21 10:37:43 2019, max compression
```

## Comparing `resdk-8.0.0.tar` & `resdk-9.0.0.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 miha       (501) staff       (20)        0 2018-11-20 10:23:48.000000 resdk-8.0.0/
--rw-r--r--   0 miha       (501) staff       (20)     5425 2018-11-20 10:23:48.000000 resdk-8.0.0/PKG-INFO
--rw-------   0 miha       (501) staff       (20)    13018 2017-05-08 19:40:27.000000 resdk-8.0.0/.pylintrc
-drwxr-xr-x   0 miha       (501) staff       (20)        0 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk/
--rw-------   0 miha       (501) staff       (20)     5898 2017-05-08 19:40:27.000000 resdk-8.0.0/resdk/resdk_logger.py
--rw-r--r--   0 miha       (501) staff       (20)    17299 2018-11-20 10:01:14.000000 resdk-8.0.0/resdk/resolwe.py
-drwxr-xr-x   0 miha       (501) staff       (20)        0 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk/analysis/
--rw-r--r--   0 miha       (501) staff       (20)     1795 2018-05-28 10:52:27.000000 resdk-8.0.0/resdk/analysis/_register.py
--rw-r--r--   0 miha       (501) staff       (20)     4930 2018-09-20 10:34:28.000000 resdk-8.0.0/resdk/analysis/prepare_geo.py
--rw-r--r--   0 miha       (501) staff       (20)     4735 2018-09-20 10:34:28.000000 resdk-8.0.0/resdk/analysis/differential_expressions.py
--rw-------   0 miha       (501) staff       (20)     4375 2017-07-14 12:23:46.000000 resdk-8.0.0/resdk/analysis/alignment.py
--rw-r--r--   0 miha       (501) staff       (20)     3476 2018-10-15 21:08:36.000000 resdk-8.0.0/resdk/analysis/expressions.py
--rw-------   0 miha       (501) staff       (20)       60 2017-05-08 19:40:27.000000 resdk-8.0.0/resdk/analysis/__init__.py
--rw-------   0 miha       (501) staff       (20)     7392 2017-05-08 19:40:27.000000 resdk-8.0.0/resdk/analysis/plots.py
--rw-r--r--   0 miha       (501) staff       (20)     6167 2018-10-15 21:08:36.000000 resdk-8.0.0/resdk/analysis/chip_seq.py
--rw-r--r--   0 miha       (501) staff       (20)    11916 2018-10-15 21:08:36.000000 resdk-8.0.0/resdk/query.py
-drwxr-xr-x   0 miha       (501) staff       (20)        0 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk/resources/
--rw-r--r--   0 miha       (501) staff       (20)     1042 2018-09-20 10:34:28.000000 resdk-8.0.0/resdk/resources/descriptor.py
--rw-r--r--   0 miha       (501) staff       (20)     5186 2018-10-15 21:08:36.000000 resdk-8.0.0/resdk/resources/relation.py
--rw-r--r--   0 miha       (501) staff       (20)     3964 2018-10-15 21:08:36.000000 resdk-8.0.0/resdk/resources/user.py
-drwxr-xr-x   0 miha       (501) staff       (20)        0 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk/resources/kb/
--rw-r--r--   0 miha       (501) staff       (20)      251 2018-11-20 10:01:14.000000 resdk-8.0.0/resdk/resources/kb/__init__.py
--rw-r--r--   0 miha       (501) staff       (20)     1453 2018-09-20 10:34:28.000000 resdk-8.0.0/resdk/resources/kb/feature.py
--rw-r--r--   0 miha       (501) staff       (20)     1393 2018-09-20 10:34:28.000000 resdk-8.0.0/resdk/resources/kb/mapping.py
--rw-r--r--   0 miha       (501) staff       (20)     1567 2018-11-20 10:01:14.000000 resdk-8.0.0/resdk/resources/__init__.py
--rw-r--r--   0 miha       (501) staff       (20)     8529 2018-11-20 10:01:14.000000 resdk-8.0.0/resdk/resources/utils.py
--rw-r--r--   0 miha       (501) staff       (20)    13050 2018-11-20 10:01:14.000000 resdk-8.0.0/resdk/resources/sample.py
--rw-r--r--   0 miha       (501) staff       (20)     8392 2018-11-20 10:01:14.000000 resdk-8.0.0/resdk/resources/collection.py
--rw-r--r--   0 miha       (501) staff       (20)     8868 2018-08-09 09:23:51.000000 resdk-8.0.0/resdk/resources/permissions.py
--rw-r--r--   0 miha       (501) staff       (20)     3061 2018-10-15 21:08:36.000000 resdk-8.0.0/resdk/resources/process.py
--rw-r--r--   0 miha       (501) staff       (20)     7268 2018-09-20 10:34:28.000000 resdk-8.0.0/resdk/resources/base.py
--rw-r--r--   0 miha       (501) staff       (20)    13317 2018-11-20 10:01:14.000000 resdk-8.0.0/resdk/resources/data.py
--rw-r--r--   0 miha       (501) staff       (20)      113 2018-08-09 09:23:51.000000 resdk-8.0.0/resdk/constants.py
-drwxr-xr-x   0 miha       (501) staff       (20)        0 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk/tests/
-drwxr-xr-x   0 miha       (501) staff       (20)        0 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk/tests/unit/
--rw-r--r--   0 miha       (501) staff       (20)    21700 2018-11-20 10:01:14.000000 resdk-8.0.0/resdk/tests/unit/test_resolwe.py
--rw-r--r--   0 miha       (501) staff       (20)    11661 2018-09-20 10:34:28.000000 resdk-8.0.0/resdk/tests/unit/test_utils.py
--rw-------   0 miha       (501) staff       (20)      719 2017-07-17 07:43:01.000000 resdk-8.0.0/resdk/tests/unit/test_decorators.py
--rw-r--r--   0 miha       (501) staff       (20)     5906 2018-09-20 10:34:28.000000 resdk-8.0.0/resdk/tests/unit/test_collections_shortcuts.py
--rw-r--r--   0 miha       (501) staff       (20)     5123 2018-11-20 10:01:14.000000 resdk-8.0.0/resdk/tests/unit/test_sample.py
--rw-------   0 miha       (501) staff       (20)      783 2017-05-08 19:40:27.000000 resdk-8.0.0/resdk/tests/unit/test_exceptions.py
--rw-------   0 miha       (501) staff       (20)        0 2016-06-03 20:56:03.000000 resdk-8.0.0/resdk/tests/unit/__init__.py
--rw-------   0 miha       (501) staff       (20)      668 2016-11-21 08:52:36.000000 resdk-8.0.0/resdk/tests/unit/test_process.py
--rw-r--r--   0 miha       (501) staff       (20)     1491 2018-10-15 21:08:36.000000 resdk-8.0.0/resdk/tests/unit/test_users.py
--rw-r--r--   0 miha       (501) staff       (20)     9211 2018-10-15 21:08:36.000000 resdk-8.0.0/resdk/tests/unit/test_query.py
--rw-r--r--   0 miha       (501) staff       (20)    10689 2018-11-20 10:01:14.000000 resdk-8.0.0/resdk/tests/unit/test_data.py
--rw-r--r--   0 miha       (501) staff       (20)     6862 2018-11-20 10:01:14.000000 resdk-8.0.0/resdk/tests/unit/test_collections.py
--rw-r--r--   0 miha       (501) staff       (20)     9541 2018-09-20 10:34:28.000000 resdk-8.0.0/resdk/tests/unit/test_base.py
--rw-r--r--   0 miha       (501) staff       (20)     4707 2018-10-15 21:08:36.000000 resdk-8.0.0/resdk/tests/unit/test_relations.py
--rw-------   0 miha       (501) staff       (20)       30 2016-08-30 18:30:15.000000 resdk-8.0.0/resdk/tests/__init__.py
-drwxr-xr-x   0 miha       (501) staff       (20)        0 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk/tests/files/
--rw-------   0 miha       (501) staff       (20)    21168 2016-05-11 02:23:20.000000 resdk-8.0.0/resdk/tests/files/example.fastq
--rw-------   0 miha       (501) staff       (20)      758 2016-08-01 20:19:17.000000 resdk-8.0.0/resdk/tests/files/reads.fastq.gz
--rw-------   0 miha       (501) staff       (20)       10 2017-05-08 19:40:27.000000 resdk-8.0.0/resdk/tests/files/dummy_gtf.gtf
--rw-r--r--   0 miha       (501) staff       (20)       13 2018-05-28 10:52:27.000000 resdk-8.0.0/resdk/tests/files/dummy_expression.tab
--rw-r--r--   0 miha       (501) staff       (20)      939 2018-10-15 21:08:36.000000 resdk-8.0.0/resdk/tests/files/genome.fasta.gz
--rw-------   0 miha       (501) staff       (20)        9 2017-05-08 19:40:27.000000 resdk-8.0.0/resdk/tests/files/dummy_genome.fasta
--rw-r--r--   0 miha       (501) staff       (20)      143 2018-10-15 21:08:36.000000 resdk-8.0.0/resdk/tests/files/annotation.gtf.gz
--rw-------   0 miha       (501) staff       (20)        8 2017-05-08 19:40:27.000000 resdk-8.0.0/resdk/tests/files/dummy_reads.fastq
--rw-------   0 miha       (501) staff       (20)        6 2017-05-08 19:40:27.000000 resdk-8.0.0/resdk/tests/files/dummy_bam.bam
--rw-------   0 miha       (501) staff       (20)       12 2017-05-08 19:40:27.000000 resdk-8.0.0/resdk/tests/files/dummy_cuffquant.cxb
-drwxr-xr-x   0 miha       (501) staff       (20)        0 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk/tests/functional/
-drwxr-xr-x   0 miha       (501) staff       (20)        0 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk/tests/functional/analysis/
--rw-r--r--   0 miha       (501) staff       (20)     9945 2018-09-20 10:34:28.000000 resdk-8.0.0/resdk/tests/functional/analysis/e2e_chip_seq.py
--rw-------   0 miha       (501) staff       (20)        0 2017-05-08 19:40:27.000000 resdk-8.0.0/resdk/tests/functional/analysis/__init__.py
--rw-r--r--   0 miha       (501) staff       (20)     3248 2018-09-20 10:34:28.000000 resdk-8.0.0/resdk/tests/functional/analysis/e2e_alignment.py
--rw-r--r--   0 miha       (501) staff       (20)     3083 2018-10-15 21:08:36.000000 resdk-8.0.0/resdk/tests/functional/analysis/e2e_expressions.py
--rw-r--r--   0 miha       (501) staff       (20)     3948 2018-09-20 10:34:28.000000 resdk-8.0.0/resdk/tests/functional/analysis/e2e_differential_expressions.py
--rw-r--r--   0 miha       (501) staff       (20)     7634 2018-09-20 10:34:28.000000 resdk-8.0.0/resdk/tests/functional/analysis/e2e_prepare_geo.py
--rw-------   0 miha       (501) staff       (20)        0 2017-05-08 19:40:27.000000 resdk-8.0.0/resdk/tests/functional/__init__.py
-drwxr-xr-x   0 miha       (501) staff       (20)        0 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk/tests/functional/docs/
--rw-r--r--   0 miha       (501) staff       (20)     8535 2018-10-15 21:08:36.000000 resdk-8.0.0/resdk/tests/functional/docs/e2e_docs.py
-drwxr-xr-x   0 miha       (501) staff       (20)        0 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk/tests/functional/permissions/
--rw-------   0 miha       (501) staff       (20)     1549 2017-09-14 00:59:23.000000 resdk-8.0.0/resdk/tests/functional/permissions/e2e_permissions.py
-drwxr-xr-x   0 miha       (501) staff       (20)        0 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk/tests/functional/resolwe/
--rw-r--r--   0 miha       (501) staff       (20)     1252 2018-11-20 10:01:14.000000 resdk-8.0.0/resdk/tests/functional/resolwe/e2e_resolwe.py
--rw-r--r--   0 miha       (501) staff       (20)     7602 2018-10-15 21:08:36.000000 resdk-8.0.0/resdk/tests/functional/base.py
--rw-r--r--   0 miha       (501) staff       (20)      290 2018-10-15 21:08:36.000000 resdk-8.0.0/resdk/__init__.py
-drwxr-xr-x   0 miha       (501) staff       (20)        0 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk/utils/
--rw-------   0 miha       (501) staff       (20)       19 2017-07-17 07:43:01.000000 resdk-8.0.0/resdk/utils/__init__.py
--rw-------   0 miha       (501) staff       (20)      662 2017-07-17 07:43:01.000000 resdk-8.0.0/resdk/utils/decorators.py
-drwxr-xr-x   0 miha       (501) staff       (20)        0 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk/scripts/
--rw-r--r--   0 miha       (501) staff       (20)       60 2018-10-15 21:08:36.000000 resdk-8.0.0/resdk/scripts/__init__.py
--rw-r--r--   0 miha       (501) staff       (20)     3167 2018-05-07 12:06:48.000000 resdk-8.0.0/resdk/scripts/reads.py
-drwxr-xr-x   0 miha       (501) staff       (20)        0 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk/shortcuts/
--rw-------   0 miha       (501) staff       (20)      194 2017-04-01 18:44:57.000000 resdk-8.0.0/resdk/shortcuts/__init__.py
--rw-r--r--   0 miha       (501) staff       (20)     4132 2018-09-20 10:34:28.000000 resdk-8.0.0/resdk/shortcuts/collection.py
--rw-r--r--   0 miha       (501) staff       (20)      755 2018-11-20 10:22:03.000000 resdk-8.0.0/resdk/__about__.py
--rw-------   0 miha       (501) staff       (20)      877 2017-05-08 19:40:27.000000 resdk-8.0.0/resdk/exceptions.py
--rw-------   0 miha       (501) staff       (20)    11358 2016-04-01 01:31:46.000000 resdk-8.0.0/LICENSE
--rw-------   0 miha       (501) staff       (20)      330 2017-05-08 19:40:27.000000 resdk-8.0.0/MANIFEST.in
-drwxr-xr-x   0 miha       (501) staff       (20)        0 2018-11-20 10:23:48.000000 resdk-8.0.0/docs/
--rw-r--r--   0 miha       (501) staff       (20)     8420 2018-10-15 21:08:36.000000 resdk-8.0.0/docs/tutorial-create.rst
--rw-r--r--   0 miha       (501) staff       (20)     1968 2018-10-15 21:08:36.000000 resdk-8.0.0/docs/index.rst
--rw-r--r--   0 miha       (501) staff       (20)     1559 2018-02-16 11:39:37.000000 resdk-8.0.0/docs/contributing.rst
-drwxr-xr-x   0 miha       (501) staff       (20)        0 2018-11-20 10:23:48.000000 resdk-8.0.0/docs/images/
--rw-------   0 miha       (501) staff       (20)    44949 2016-05-31 20:00:51.000000 resdk-8.0.0/docs/images/input_schema.jpg
--rw-r--r--   0 miha       (501) staff       (20)    77678 2018-10-15 21:08:36.000000 resdk-8.0.0/docs/images/data-hierarchy-diagram.png
--rw-------   0 miha       (501) staff       (20)     3821 2017-07-17 12:16:37.000000 resdk-8.0.0/docs/images/define_sample_collection_relations-02.png
--rw-------   0 miha       (501) staff       (20)    35758 2016-05-31 20:00:51.000000 resdk-8.0.0/docs/images/resolwe_resdk.jpg
--rw-------   0 miha       (501) staff       (20)    10722 2017-07-17 12:16:37.000000 resdk-8.0.0/docs/images/define_sample_collection_relations-03.png
--rw-------   0 miha       (501) staff       (20)   163707 2016-05-31 20:00:51.000000 resdk-8.0.0/docs/images/collections_relation.jpg
--rw-------   0 miha       (501) staff       (20)     2775 2017-07-17 12:16:37.000000 resdk-8.0.0/docs/images/define_sample_collection_relations-01.png
--rw-r--r--   0 miha       (501) staff       (20)     5155 2018-10-15 21:08:36.000000 resdk-8.0.0/docs/tutorial-get.rst
--rw-------   0 miha       (501) staff       (20)     1978 2017-05-08 19:40:27.000000 resdk-8.0.0/docs/conf.py
--rw-r--r--   0 miha       (501) staff       (20)     4536 2018-10-15 21:08:36.000000 resdk-8.0.0/docs/tutorial-basics.rst
-drwxr-xr-x   0 miha       (501) staff       (20)        0 2018-11-20 10:23:48.000000 resdk-8.0.0/docs/files/
--rw-r--r--   0 miha       (501) staff       (20)     2547 2018-10-15 21:08:36.000000 resdk-8.0.0/docs/files/tutorial-create.py
--rw-r--r--   0 miha       (501) staff       (20)      370 2018-10-15 21:08:36.000000 resdk-8.0.0/docs/files/index.py
--rw-r--r--   0 miha       (501) staff       (20)      878 2018-10-15 21:08:36.000000 resdk-8.0.0/docs/files/start.py
--rw-r--r--   0 miha       (501) staff       (20)     1438 2018-10-15 21:08:36.000000 resdk-8.0.0/docs/files/tutorial-get.py
--rw-------   0 miha       (501) staff       (20)      205 2016-11-21 08:52:36.000000 resdk-8.0.0/docs/ref.rst
--rw-r--r--   0 miha       (501) staff       (20)      115 2018-10-15 21:08:36.000000 resdk-8.0.0/docs/tutorials.rst
--rw-r--r--   0 miha       (501) staff       (20)    15405 2018-11-20 10:22:03.000000 resdk-8.0.0/docs/CHANGELOG.rst
--rw-r--r--   0 miha       (501) staff       (20)     7031 2018-10-15 21:08:36.000000 resdk-8.0.0/docs/start.rst
--rw-r--r--   0 miha       (501) staff       (20)     2547 2018-10-15 21:08:36.000000 resdk-8.0.0/setup.py
--rw-------   0 miha       (501) staff       (20)     1277 2017-09-14 00:59:23.000000 resdk-8.0.0/tox.ini
--rw-r--r--   0 miha       (501) staff       (20)      516 2018-11-20 10:23:48.000000 resdk-8.0.0/setup.cfg
--rw-r--r--   0 miha       (501) staff       (20)     3553 2018-10-15 21:08:36.000000 resdk-8.0.0/README.rst
-drwxr-xr-x   0 miha       (501) staff       (20)        0 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk.egg-info/
--rw-r--r--   0 miha       (501) staff       (20)     5425 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk.egg-info/PKG-INFO
--rw-r--r--   0 miha       (501) staff       (20)        1 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk.egg-info/not-zip-safe
--rw-r--r--   0 miha       (501) staff       (20)     3122 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk.egg-info/SOURCES.txt
--rw-r--r--   0 miha       (501) staff       (20)       69 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk.egg-info/entry_points.txt
--rw-r--r--   0 miha       (501) staff       (20)      258 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk.egg-info/requires.txt
--rw-r--r--   0 miha       (501) staff       (20)        6 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk.egg-info/top_level.txt
--rw-r--r--   0 miha       (501) staff       (20)        1 2018-11-20 10:23:48.000000 resdk-8.0.0/resdk.egg-info/dependency_links.txt
+drwxr-xr-x   0 miha       (501) staff       (20)        0 2019-02-21 10:37:43.000000 resdk-9.0.0/
+-rw-r--r--   0 miha       (501) staff       (20)     5425 2019-02-21 10:37:43.000000 resdk-9.0.0/PKG-INFO
+-rw-------   0 miha       (501) staff       (20)    13018 2017-05-08 19:40:27.000000 resdk-9.0.0/.pylintrc
+drwxr-xr-x   0 miha       (501) staff       (20)        0 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk/
+-rw-------   0 miha       (501) staff       (20)     5898 2017-05-08 19:40:27.000000 resdk-9.0.0/resdk/resdk_logger.py
+-rw-r--r--   0 miha       (501) staff       (20)    17299 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/resolwe.py
+drwxr-xr-x   0 miha       (501) staff       (20)        0 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk/analysis/
+-rw-r--r--   0 miha       (501) staff       (20)     1795 2018-05-28 10:52:27.000000 resdk-9.0.0/resdk/analysis/_register.py
+-rw-r--r--   0 miha       (501) staff       (20)     4698 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/analysis/prepare_geo.py
+-rw-r--r--   0 miha       (501) staff       (20)     4735 2018-09-20 10:34:28.000000 resdk-9.0.0/resdk/analysis/differential_expressions.py
+-rw-------   0 miha       (501) staff       (20)     4375 2017-07-14 12:23:46.000000 resdk-9.0.0/resdk/analysis/alignment.py
+-rw-r--r--   0 miha       (501) staff       (20)     3476 2018-10-15 21:08:36.000000 resdk-9.0.0/resdk/analysis/expressions.py
+-rw-------   0 miha       (501) staff       (20)       60 2017-05-08 19:40:27.000000 resdk-9.0.0/resdk/analysis/__init__.py
+-rw-------   0 miha       (501) staff       (20)     7392 2017-05-08 19:40:27.000000 resdk-9.0.0/resdk/analysis/plots.py
+-rw-r--r--   0 miha       (501) staff       (20)     6167 2018-10-15 21:08:36.000000 resdk-9.0.0/resdk/analysis/chip_seq.py
+-rw-r--r--   0 miha       (501) staff       (20)    11512 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/query.py
+drwxr-xr-x   0 miha       (501) staff       (20)        0 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk/resources/
+-rw-r--r--   0 miha       (501) staff       (20)     1042 2018-09-20 10:34:28.000000 resdk-9.0.0/resdk/resources/descriptor.py
+-rw-r--r--   0 miha       (501) staff       (20)     5149 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/resources/relation.py
+-rw-r--r--   0 miha       (501) staff       (20)     3964 2018-10-15 21:08:36.000000 resdk-9.0.0/resdk/resources/user.py
+drwxr-xr-x   0 miha       (501) staff       (20)        0 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk/resources/kb/
+-rw-r--r--   0 miha       (501) staff       (20)      251 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/resources/kb/__init__.py
+-rw-r--r--   0 miha       (501) staff       (20)     1453 2018-09-20 10:34:28.000000 resdk-9.0.0/resdk/resources/kb/feature.py
+-rw-r--r--   0 miha       (501) staff       (20)     1393 2018-09-20 10:34:28.000000 resdk-9.0.0/resdk/resources/kb/mapping.py
+-rw-r--r--   0 miha       (501) staff       (20)     1567 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/resources/__init__.py
+-rw-r--r--   0 miha       (501) staff       (20)     9227 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/resources/utils.py
+-rw-r--r--   0 miha       (501) staff       (20)    13050 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/resources/sample.py
+-rw-r--r--   0 miha       (501) staff       (20)     8428 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/resources/collection.py
+-rw-r--r--   0 miha       (501) staff       (20)     8868 2018-08-09 09:23:51.000000 resdk-9.0.0/resdk/resources/permissions.py
+-rw-r--r--   0 miha       (501) staff       (20)     3061 2018-10-15 21:08:36.000000 resdk-9.0.0/resdk/resources/process.py
+-rw-r--r--   0 miha       (501) staff       (20)     8851 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/resources/base.py
+-rw-r--r--   0 miha       (501) staff       (20)    13708 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/resources/data.py
+-rw-r--r--   0 miha       (501) staff       (20)      163 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/constants.py
+drwxr-xr-x   0 miha       (501) staff       (20)        0 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk/tests/
+drwxr-xr-x   0 miha       (501) staff       (20)        0 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk/tests/unit/
+-rw-r--r--   0 miha       (501) staff       (20)    21700 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/tests/unit/test_resolwe.py
+-rw-r--r--   0 miha       (501) staff       (20)    12309 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/tests/unit/test_utils.py
+-rw-------   0 miha       (501) staff       (20)      719 2017-07-17 07:43:01.000000 resdk-9.0.0/resdk/tests/unit/test_decorators.py
+-rw-r--r--   0 miha       (501) staff       (20)     5906 2018-09-20 10:34:28.000000 resdk-9.0.0/resdk/tests/unit/test_collections_shortcuts.py
+-rw-r--r--   0 miha       (501) staff       (20)     5123 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/tests/unit/test_sample.py
+-rw-------   0 miha       (501) staff       (20)      783 2017-05-08 19:40:27.000000 resdk-9.0.0/resdk/tests/unit/test_exceptions.py
+-rw-------   0 miha       (501) staff       (20)        0 2016-06-03 20:56:03.000000 resdk-9.0.0/resdk/tests/unit/__init__.py
+-rw-------   0 miha       (501) staff       (20)      668 2016-11-21 08:52:36.000000 resdk-9.0.0/resdk/tests/unit/test_process.py
+-rw-r--r--   0 miha       (501) staff       (20)     1491 2018-10-15 21:08:36.000000 resdk-9.0.0/resdk/tests/unit/test_users.py
+-rw-r--r--   0 miha       (501) staff       (20)     9263 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/tests/unit/test_query.py
+-rw-r--r--   0 miha       (501) staff       (20)    10689 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/tests/unit/test_data.py
+-rw-r--r--   0 miha       (501) staff       (20)     6862 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/tests/unit/test_collections.py
+-rw-r--r--   0 miha       (501) staff       (20)     9541 2018-09-20 10:34:28.000000 resdk-9.0.0/resdk/tests/unit/test_base.py
+-rw-r--r--   0 miha       (501) staff       (20)     4707 2018-10-15 21:08:36.000000 resdk-9.0.0/resdk/tests/unit/test_relations.py
+-rw-------   0 miha       (501) staff       (20)       30 2016-08-30 18:30:15.000000 resdk-9.0.0/resdk/tests/__init__.py
+drwxr-xr-x   0 miha       (501) staff       (20)        0 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk/tests/files/
+-rw-------   0 miha       (501) staff       (20)    21168 2016-05-11 02:23:20.000000 resdk-9.0.0/resdk/tests/files/example.fastq
+-rw-------   0 miha       (501) staff       (20)      758 2016-08-01 20:19:17.000000 resdk-9.0.0/resdk/tests/files/reads.fastq.gz
+-rw-------   0 miha       (501) staff       (20)       10 2017-05-08 19:40:27.000000 resdk-9.0.0/resdk/tests/files/dummy_gtf.gtf
+-rw-r--r--   0 miha       (501) staff       (20)       13 2018-05-28 10:52:27.000000 resdk-9.0.0/resdk/tests/files/dummy_expression.tab
+-rw-r--r--   0 miha       (501) staff       (20)      939 2018-10-15 21:08:36.000000 resdk-9.0.0/resdk/tests/files/genome.fasta.gz
+-rw-------   0 miha       (501) staff       (20)        9 2017-05-08 19:40:27.000000 resdk-9.0.0/resdk/tests/files/dummy_genome.fasta
+-rw-r--r--   0 miha       (501) staff       (20)      143 2018-10-15 21:08:36.000000 resdk-9.0.0/resdk/tests/files/annotation.gtf.gz
+-rw-------   0 miha       (501) staff       (20)        8 2017-05-08 19:40:27.000000 resdk-9.0.0/resdk/tests/files/dummy_reads.fastq
+-rw-------   0 miha       (501) staff       (20)        6 2017-05-08 19:40:27.000000 resdk-9.0.0/resdk/tests/files/dummy_bam.bam
+-rw-------   0 miha       (501) staff       (20)       12 2017-05-08 19:40:27.000000 resdk-9.0.0/resdk/tests/files/dummy_cuffquant.cxb
+drwxr-xr-x   0 miha       (501) staff       (20)        0 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk/tests/functional/
+drwxr-xr-x   0 miha       (501) staff       (20)        0 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk/tests/functional/analysis/
+-rw-r--r--   0 miha       (501) staff       (20)     9945 2018-09-20 10:34:28.000000 resdk-9.0.0/resdk/tests/functional/analysis/e2e_chip_seq.py
+-rw-------   0 miha       (501) staff       (20)        0 2017-05-08 19:40:27.000000 resdk-9.0.0/resdk/tests/functional/analysis/__init__.py
+-rw-r--r--   0 miha       (501) staff       (20)     3248 2018-09-20 10:34:28.000000 resdk-9.0.0/resdk/tests/functional/analysis/e2e_alignment.py
+-rw-r--r--   0 miha       (501) staff       (20)     3083 2018-10-15 21:08:36.000000 resdk-9.0.0/resdk/tests/functional/analysis/e2e_expressions.py
+-rw-r--r--   0 miha       (501) staff       (20)     3948 2018-09-20 10:34:28.000000 resdk-9.0.0/resdk/tests/functional/analysis/e2e_differential_expressions.py
+-rw-r--r--   0 miha       (501) staff       (20)     7087 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/tests/functional/analysis/e2e_prepare_geo.py
+-rw-------   0 miha       (501) staff       (20)        0 2017-05-08 19:40:27.000000 resdk-9.0.0/resdk/tests/functional/__init__.py
+drwxr-xr-x   0 miha       (501) staff       (20)        0 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk/tests/functional/docs/
+-rw-r--r--   0 miha       (501) staff       (20)     8535 2018-10-15 21:08:36.000000 resdk-9.0.0/resdk/tests/functional/docs/e2e_docs.py
+drwxr-xr-x   0 miha       (501) staff       (20)        0 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk/tests/functional/permissions/
+-rw-------   0 miha       (501) staff       (20)     1549 2017-09-14 00:59:23.000000 resdk-9.0.0/resdk/tests/functional/permissions/e2e_permissions.py
+drwxr-xr-x   0 miha       (501) staff       (20)        0 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk/tests/functional/resolwe/
+-rw-r--r--   0 miha       (501) staff       (20)     1252 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/tests/functional/resolwe/e2e_resolwe.py
+-rw-r--r--   0 miha       (501) staff       (20)     7602 2018-10-15 21:08:36.000000 resdk-9.0.0/resdk/tests/functional/base.py
+-rw-r--r--   0 miha       (501) staff       (20)      290 2018-10-15 21:08:36.000000 resdk-9.0.0/resdk/__init__.py
+drwxr-xr-x   0 miha       (501) staff       (20)        0 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk/utils/
+-rw-------   0 miha       (501) staff       (20)       19 2017-07-17 07:43:01.000000 resdk-9.0.0/resdk/utils/__init__.py
+-rw-------   0 miha       (501) staff       (20)      662 2017-07-17 07:43:01.000000 resdk-9.0.0/resdk/utils/decorators.py
+drwxr-xr-x   0 miha       (501) staff       (20)        0 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk/scripts/
+-rw-r--r--   0 miha       (501) staff       (20)       60 2018-10-15 21:08:36.000000 resdk-9.0.0/resdk/scripts/__init__.py
+-rw-r--r--   0 miha       (501) staff       (20)     3167 2018-05-07 12:06:48.000000 resdk-9.0.0/resdk/scripts/reads.py
+drwxr-xr-x   0 miha       (501) staff       (20)        0 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk/shortcuts/
+-rw-------   0 miha       (501) staff       (20)      194 2017-04-01 18:44:57.000000 resdk-9.0.0/resdk/shortcuts/__init__.py
+-rw-r--r--   0 miha       (501) staff       (20)     4132 2018-09-20 10:34:28.000000 resdk-9.0.0/resdk/shortcuts/collection.py
+-rw-r--r--   0 miha       (501) staff       (20)      755 2019-02-21 10:36:39.000000 resdk-9.0.0/resdk/__about__.py
+-rw-------   0 miha       (501) staff       (20)      877 2017-05-08 19:40:27.000000 resdk-9.0.0/resdk/exceptions.py
+-rw-------   0 miha       (501) staff       (20)    11358 2016-04-01 01:31:46.000000 resdk-9.0.0/LICENSE
+-rw-------   0 miha       (501) staff       (20)      330 2017-05-08 19:40:27.000000 resdk-9.0.0/MANIFEST.in
+drwxr-xr-x   0 miha       (501) staff       (20)        0 2019-02-21 10:37:43.000000 resdk-9.0.0/docs/
+-rw-r--r--   0 miha       (501) staff       (20)     8420 2018-10-15 21:08:36.000000 resdk-9.0.0/docs/tutorial-create.rst
+-rw-r--r--   0 miha       (501) staff       (20)     1968 2018-10-15 21:08:36.000000 resdk-9.0.0/docs/index.rst
+-rw-r--r--   0 miha       (501) staff       (20)     1559 2018-02-16 11:39:37.000000 resdk-9.0.0/docs/contributing.rst
+drwxr-xr-x   0 miha       (501) staff       (20)        0 2019-02-21 10:37:43.000000 resdk-9.0.0/docs/images/
+-rw-------   0 miha       (501) staff       (20)    44949 2016-05-31 20:00:51.000000 resdk-9.0.0/docs/images/input_schema.jpg
+-rw-r--r--   0 miha       (501) staff       (20)    77678 2018-10-15 21:08:36.000000 resdk-9.0.0/docs/images/data-hierarchy-diagram.png
+-rw-------   0 miha       (501) staff       (20)     3821 2017-07-17 12:16:37.000000 resdk-9.0.0/docs/images/define_sample_collection_relations-02.png
+-rw-------   0 miha       (501) staff       (20)    35758 2016-05-31 20:00:51.000000 resdk-9.0.0/docs/images/resolwe_resdk.jpg
+-rw-------   0 miha       (501) staff       (20)    10722 2017-07-17 12:16:37.000000 resdk-9.0.0/docs/images/define_sample_collection_relations-03.png
+-rw-------   0 miha       (501) staff       (20)   163707 2016-05-31 20:00:51.000000 resdk-9.0.0/docs/images/collections_relation.jpg
+-rw-------   0 miha       (501) staff       (20)     2775 2017-07-17 12:16:37.000000 resdk-9.0.0/docs/images/define_sample_collection_relations-01.png
+-rw-r--r--   0 miha       (501) staff       (20)     5155 2018-10-15 21:08:36.000000 resdk-9.0.0/docs/tutorial-get.rst
+-rw-------   0 miha       (501) staff       (20)     1978 2017-05-08 19:40:27.000000 resdk-9.0.0/docs/conf.py
+-rw-r--r--   0 miha       (501) staff       (20)     4536 2018-10-15 21:08:36.000000 resdk-9.0.0/docs/tutorial-basics.rst
+drwxr-xr-x   0 miha       (501) staff       (20)        0 2019-02-21 10:37:43.000000 resdk-9.0.0/docs/files/
+-rw-r--r--   0 miha       (501) staff       (20)     2547 2018-10-15 21:08:36.000000 resdk-9.0.0/docs/files/tutorial-create.py
+-rw-r--r--   0 miha       (501) staff       (20)      370 2018-10-15 21:08:36.000000 resdk-9.0.0/docs/files/index.py
+-rw-r--r--   0 miha       (501) staff       (20)      878 2018-10-15 21:08:36.000000 resdk-9.0.0/docs/files/start.py
+-rw-r--r--   0 miha       (501) staff       (20)     1438 2018-10-15 21:08:36.000000 resdk-9.0.0/docs/files/tutorial-get.py
+-rw-------   0 miha       (501) staff       (20)      205 2016-11-21 08:52:36.000000 resdk-9.0.0/docs/ref.rst
+-rw-r--r--   0 miha       (501) staff       (20)      115 2018-10-15 21:08:36.000000 resdk-9.0.0/docs/tutorials.rst
+-rw-r--r--   0 miha       (501) staff       (20)    15938 2019-02-21 10:36:39.000000 resdk-9.0.0/docs/CHANGELOG.rst
+-rw-r--r--   0 miha       (501) staff       (20)     7031 2018-10-15 21:08:36.000000 resdk-9.0.0/docs/start.rst
+-rw-r--r--   0 miha       (501) staff       (20)     2597 2019-02-21 10:36:39.000000 resdk-9.0.0/setup.py
+-rw-------   0 miha       (501) staff       (20)     1277 2017-09-14 00:59:23.000000 resdk-9.0.0/tox.ini
+-rw-r--r--   0 miha       (501) staff       (20)      516 2019-02-21 10:37:43.000000 resdk-9.0.0/setup.cfg
+-rw-r--r--   0 miha       (501) staff       (20)     3553 2018-10-15 21:08:36.000000 resdk-9.0.0/README.rst
+drwxr-xr-x   0 miha       (501) staff       (20)        0 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk.egg-info/
+-rw-r--r--   0 miha       (501) staff       (20)     5425 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk.egg-info/PKG-INFO
+-rw-r--r--   0 miha       (501) staff       (20)        1 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk.egg-info/not-zip-safe
+-rw-r--r--   0 miha       (501) staff       (20)     3122 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk.egg-info/SOURCES.txt
+-rw-r--r--   0 miha       (501) staff       (20)       69 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk.egg-info/entry_points.txt
+-rw-r--r--   0 miha       (501) staff       (20)      286 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk.egg-info/requires.txt
+-rw-r--r--   0 miha       (501) staff       (20)        6 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk.egg-info/top_level.txt
+-rw-r--r--   0 miha       (501) staff       (20)        1 2019-02-21 10:37:43.000000 resdk-9.0.0/resdk.egg-info/dependency_links.txt
```

### Comparing `resdk-8.0.0/PKG-INFO` & `resdk-9.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resdk
-Version: 8.0.0
+Version: 9.0.0
 Summary: Resolwe SDK for Python
 Home-page: https://github.com/genialis/resolwe-bio-py
 Author: Genialis, Inc.
 Author-email: dev-team@genialis.com
 License: Apache License (2.0)
 Description: ======================
         Resolwe SDK for Python
@@ -122,10 +122,10 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
-Provides-Extra: docs
-Provides-Extra: package
 Provides-Extra: test
+Provides-Extra: package
+Provides-Extra: docs
```

### Comparing `resdk-8.0.0/.pylintrc` & `resdk-9.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/resdk_logger.py` & `resdk-9.0.0/resdk/resdk_logger.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/resolwe.py` & `resdk-9.0.0/resdk/resolwe.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/analysis/_register.py` & `resdk-9.0.0/resdk/analysis/_register.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/analysis/prepare_geo.py` & `resdk-9.0.0/resdk/analysis/prepare_geo.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,58 +39,48 @@
     on a single collection or a list of samples.
 
     :param resource: resource on which prepare_geo_chipseq will be run
     :param str name: name of the prepare GEO tarball and table
 
     """
     reads = []
-    macs14 = []
-    relations = []
+    macs = []
 
     samples = get_samples(resource)
     resolwe = get_resolwe(*samples)
     collection_ids = set()
 
     for sample in samples:
         reads.append(sample.get_reads().id)
 
         if sample.is_background:
             continue
 
         macs_list = sample.get_macs()
         if not macs_list:
-            raise ValueError(
-                "Sample {} has no `macs14` data object!".format(sample)
-            )
+            raise ValueError("Sample {} has no `macs` data object!".format(sample))
         elif len(macs_list) != 1:
-            raise ValueError(
-                "Sample {} has more than one `macs14` data objects!".format(sample)
-            )
+            raise ValueError("Sample {} has more than one `macs` data objects!".format(sample))
 
-        macs14.append(macs_list[0].id)
+        macs.append(macs_list[0].id)
 
         if sample.background:
             if sample.background not in samples:
                 raise ValueError(
                     "Background of the sample {} cannot be found in the resource you provided: "
                     "{}!".format(sample, resource)
                 )
 
-            relations.append(
-                ':'.join([sample.name, sample.background.name])
-            )
-
         collection_ids.add(get_resource_collection(sample))
 
     auto_name, collection = get_name_collection(collection_ids, resolwe)
 
     inputs = {
         'reads': reads,
-        'macs14': macs14,
-        'relations': relations,
+        'macs': macs,
         'name': name or auto_name,
     }
     geo = resolwe.get_or_run(slug='prepare-geo-chipseq', input=inputs)
 
     if collection:
         collection.add_data(geo)
```

### Comparing `resdk-8.0.0/resdk/analysis/differential_expressions.py` & `resdk-9.0.0/resdk/analysis/differential_expressions.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/analysis/alignment.py` & `resdk-9.0.0/resdk/analysis/alignment.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/analysis/expressions.py` & `resdk-9.0.0/resdk/analysis/expressions.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/analysis/plots.py` & `resdk-9.0.0/resdk/analysis/plots.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/analysis/chip_seq.py` & `resdk-9.0.0/resdk/analysis/chip_seq.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/query.py` & `resdk-9.0.0/resdk/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,56 +92,39 @@
             * created (=, __gte, __gt=, __lte=, __lt=, __year__gte=,
               __month__gte=,...)
             * modified (=, __gte, __gt=, __lte=, __lt=, __year__gte=,
               __month__gte=,...)
             * slug (=, __in=)
             * id (=, __in=)
 
-    Example usage:
-
-    .. code-block:: python
-
-        # Get a list of data objects with status set to OK.
-        res.data.filter(status='OK')
-
-        # Get a list of sample objects that contain data object 42 and
-        # were contributed by contributor with ID 1
-
-        res.collection.filter(data=42, contributor=1)
-
     """
 
     _cache = None
     _count = None  # number of objects in current query (without applied limit and offset)
     _limit = None
     _offset = None
-    _filters = collections.defaultdict(list)
+    _filters = None
 
     resolwe = None
     resource = None
+    slug_field = None
     endpoint = None
     api = None
     logger = None
 
-    def __init__(self, resolwe, resource, endpoint=None, slug_field='slug'):
+    def __init__(self, resolwe, resource, slug_field='slug'):
         """Initialize attributes."""
         self.resolwe = resolwe
         self.resource = resource
-
         self.slug_field = slug_field
+        self.endpoint = resource.query_endpoint or resource.endpoint
+        self.api = operator.attrgetter(self.endpoint)(resolwe.api)
 
-        # Determine the endpoint to use.
-        if endpoint is not None:
-            self.endpoint = endpoint
-        elif resource.query_endpoint is not None:
-            self.endpoint = resource.query_endpoint
-        else:
-            self.endpoint = resource.endpoint
+        self._filters = collections.defaultdict(list)
 
-        self.api = operator.attrgetter(self.endpoint)(resolwe.api)
         self.logger = logging.getLogger(__name__)
 
     def __getitem__(self, index):
         """Retrieve an item or slice from the set of results."""
         # pylint: disable=protected-access
         if not isinstance(index, (slice,) + six.integer_types):
             raise TypeError
@@ -191,22 +174,22 @@
     def __len__(self):
         """Return length of results of current query."""
         return self.count()
 
     def _clone(self):
         """Return copy of current object with empty cache."""
         # pylint: disable=protected-access
-        new_obj = ResolweQuery(self.resolwe, self.resource, self.endpoint)
+        new_obj = ResolweQuery(self.resolwe, self.resource)
         new_obj._filters = copy.deepcopy(self._filters)
         new_obj._limit = self._limit
         new_obj._offset = self._offset
         return new_obj
 
     def _add_filter(self, filter_):
-        """Add filter parameter."""
+        """Add filtering parameters."""
         for key, value in filter_.items():
             # 'sample' is called 'entity' in the backend.
             key = key.replace('sample', 'entity')
 
             if self.resource.query_method == 'GET':
                 self._filters[key].append(value)
             elif self.resource.query_method == 'POST':
@@ -229,15 +212,16 @@
     def _populate_resource(self, data):
         """Populate resource with given data."""
         return self.resource(resolwe=self.resolwe, **data)
 
     def _fetch(self):
         """Make request to the server and populate cache."""
         if self._cache is not None:
-            return  # already fetched
+            # Already fetched.
+            return
 
         filters = self._compose_filters()
         if self.resource.query_method == 'GET':
             items = self.api.get(**filters)
         elif self.resource.query_method == 'POST':
             items = self.api.post(filters)
         else:
@@ -315,21 +299,14 @@
     def create(self, **model_data):
         """Return new instance of current resource."""
         resource = self.resource(self.resolwe, **model_data)
         resource.save()
 
         return resource
 
-    def post(self, data):
-        """Post data to this endpoint.
-
-        :param dict data: Data dictionary to post
-        """
-        return self.api.post(data)  # pylint: disable=no-member
-
     def filter(self, **filters):
         """Return clone of current query with added given filters."""
         new_query = self._clone()
         new_query._add_filter(filters)  # pylint: disable=protected-access
         return new_query
 
     def delete(self, force=False):
@@ -350,10 +327,17 @@
         """Return copy of the current queryset.
 
         This is handy function to get newly created query without any
         filters.
         """
         return self._clone()
 
-    def search(self):
+    def search(self, text):
         """Full text search."""
-        raise NotImplementedError()
+        if not self.resource.full_search_paramater:
+            raise NotImplementedError()
+
+        new_query = self._clone()
+        # pylint: disable=protected-access
+        new_query._add_filter({self.resource.full_search_paramater: text})
+        # pylint: enable=protected-access
+        return new_query
```

### Comparing `resdk-8.0.0/resdk/resources/descriptor.py` & `resdk-9.0.0/resdk/resources/descriptor.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/resources/relation.py` & `resdk-9.0.0/resdk/resources/relation.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,16 @@
     :type resolwe: Resolwe object
     :param model_data: Resource model data
 
     """
 
     endpoint = 'relation'
 
-    READ_ONLY_FIELDS = (
-        'created', 'id', 'modified',
-    )
-    UPDATE_PROTECTED_FIELDS = (
-        'contributor', 'type',
+    UPDATE_PROTECTED_FIELDS = BaseResolweResource.UPDATE_PROTECTED_FIELDS + (
+        'type',
     )
     WRITABLE_FIELDS = BaseResolweResource.WRITABLE_FIELDS + (
         'collection', 'category', 'partitions', 'unit',
     )
 
     ALL_PERMISSIONS = ['view', 'edit', 'share', 'owner']
```

### Comparing `resdk-8.0.0/resdk/resources/user.py` & `resdk-9.0.0/resdk/resources/user.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/resources/kb/feature.py` & `resdk-9.0.0/resdk/resources/kb/feature.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/resources/kb/mapping.py` & `resdk-9.0.0/resdk/resources/kb/mapping.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/resources/__init__.py` & `resdk-9.0.0/resdk/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/resources/utils.py` & `resdk-9.0.0/resdk/resources/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 """Resource utility functions."""
 from __future__ import absolute_import, division, print_function, unicode_literals
 
+from datetime import datetime
+
+import pytz
+import tzlocal
+
+from resdk.constants import RESOLWE_DATETIME_FORMAT
+
 
 def iterate_fields(fields, schema):
     """Recursively iterate over all DictField sub-fields.
 
     :param fields: Field instance (e.g. input)
     :type fields: dict
     :param schema: Schema instance (e.g. input_schema)
@@ -257,7 +264,22 @@
     Raise an error if there is more than one.
     """
     resolwes = {res_obj.resolwe for res_obj in resources}
     if len(resolwes) != 1:
         raise TypeError('All input objects must be from the same `Resolwe` connection.')
 
     return list(resolwes)[0]
+
+
+def parse_resolwe_datetime(dtime):
+    """Convert string representation of time to local datetime.datetime object."""
+    if dtime:
+        # Get naive (=time-zone unaware) version of UTC time:
+        utc_naive = datetime.strptime(dtime[:-6], RESOLWE_DATETIME_FORMAT)
+        # Localize the time so it includes UTC timezone info:
+        utc_aware = pytz.utc.localize(utc_naive)
+        # Get name local time zone:
+        local_tz = tzlocal.get_localzone()
+        # Present time in the local time zone
+        local_time = utc_aware.astimezone(local_tz)
+
+        return local_time
```

### Comparing `resdk-8.0.0/resdk/resources/sample.py` & `resdk-9.0.0/resdk/resources/sample.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/resources/collection.py` & `resdk-9.0.0/resdk/resources/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 
     :param resolwe: Resolwe instance
     :type resolwe: Resolwe object
     :param model_data: Resource model data
 
     """
 
+    full_search_paramater = 'text'
+
     WRITABLE_FIELDS = BaseResolweResource.WRITABLE_FIELDS + (
         'description', 'descriptor', 'descriptor_schema', 'settings', 'tags',
     )
 
     ALL_PERMISSIONS = ['view', 'download', 'add', 'edit', 'share', 'owner']
 
     def __init__(self, resolwe, **model_data):
```

### Comparing `resdk-8.0.0/resdk/resources/permissions.py` & `resdk-9.0.0/resdk/resources/permissions.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/resources/process.py` & `resdk-9.0.0/resdk/resources/process.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/resources/base.py` & `resdk-9.0.0/resdk/resources/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import copy
 import logging
 import operator
 
 import six
 
 from .permissions import PermissionsManager
+from .utils import parse_resolwe_datetime
 
 
 class BaseResource(object):
     """Abstract resource.
 
     One and only one of the identifiers (slug, id or model_data)
     should be given.
@@ -21,14 +22,15 @@
     :param model_data: Resource model data
 
     """
 
     endpoint = None
     query_endpoint = None
     query_method = 'GET'
+    full_search_paramater = None
 
     READ_ONLY_FIELDS = (
         'id',
     )
     UPDATE_PROTECTED_FIELDS = ()
     WRITABLE_FIELDS = ()
 
@@ -142,15 +144,16 @@
                 and value != self._original_values[name]):
             raise ValueError("Can not change read only field {}".format(name))
 
         super(BaseResource, self).__setattr__(name, value)
 
     def __eq__(self, obj):
         """Evaluate if objects are the same."""
-        if self.__class__ == obj.__class__ and self.id == obj.id:
+        if (self.__class__ == obj.__class__ and self.resolwe.url == obj.resolwe.url
+                and self.id == obj.id):
             return True
         else:
             return False
 
 
 class BaseResolweResource(BaseResource):
     """Base class for Resolwe resources.
@@ -163,35 +166,29 @@
     :param model_data: Resource model data
 
     """
 
     _permissions = None
 
     READ_ONLY_FIELDS = BaseResource.READ_ONLY_FIELDS + (
-        'created', 'current_user_permissions', 'id', 'modified', 'version',
+        'current_user_permissions', 'id', 'version',
     )
     WRITABLE_FIELDS = (
         'name', 'slug',
     )
-    UPDATE_PROTECTED_FIELDS = (
-        'contributor',
-    )
 
     def __init__(self, resolwe, **model_data):
         """Initialize attributes."""
         self.logger = logging.getLogger(__name__)
 
-        #: user id of the contributor
-        self.contributor = None
-        #: date of creation
-        self.created = None
+        #: User object of the contributor (lazy loaded)
+        self._contributor = None
+
         #: current user permissions
         self.current_user_permissions = None
-        #: date of latest modification
-        self.modified = None
         #: name of resource
         self.name = None
         #: human-readable unique identifier
         self.slug = None
         #: resource version
         self.version = None
 
@@ -207,14 +204,53 @@
                 self.ALL_PERMISSIONS,
                 self.api(self.id),
                 self.resolwe
             )
 
         return self._permissions
 
+    @property
+    def contributor(self):
+        """Get contributor."""
+        if self.id is None:
+            raise ValueError('Instance must be saved before accessing `contributor` attribute.')
+        if self._contributor is None:
+            contributor_data = self._original_values.get('contributor', {})
+            try:
+                self._contributor = self.resolwe.user.get(id=contributor_data.get('id'))
+            except LookupError:
+                from . import User
+                # Normal user has only access to his user instance on user
+                # endpoint. Instead of returning None for all other
+                # contributors, data that is received in response is used to
+                # populate User resource.
+                self._contributor = User(
+                    self.resolwe,
+                    id=contributor_data.get('id'),
+                    username=contributor_data.get('username'),
+                    first_name=contributor_data.get('first_name'),
+                    last_name=contributor_data.get('last_name'),
+                )
+
+        return self._contributor
+
+    @property
+    def created(self):
+        """Creation time."""
+        if not self.id:
+            raise ValueError('Instance must be saved before acessing `created` attribute.')
+        return parse_resolwe_datetime(self._original_values['created'])
+
+    @property
+    def modified(self):
+        """Modification time."""
+        if not self.id:
+            raise ValueError('Instance must be saved before acessing `modified` attribute.')
+        return parse_resolwe_datetime(self._original_values['modified'])
+
     def update(self):
         """Clear permissions cache and update the object."""
         self.permissions.clear_cache()
 
         super(BaseResolweResource, self).update()
 
     def __repr__(self):
```

### Comparing `resdk-8.0.0/resdk/resources/data.py` & `resdk-9.0.0/resdk/resources/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 import six
 from six.moves.urllib.parse import urljoin  # pylint: disable=wrong-import-order
 
 from resdk.constants import CHUNK_SIZE
 
 from .base import BaseResolweResource
 from .descriptor import DescriptorSchema
-from .utils import flatten_field, get_descriptor_schema_id, is_descriptor_schema
+from .utils import (
+    flatten_field, get_descriptor_schema_id, is_descriptor_schema, parse_resolwe_datetime,
+)
 
 
 class Data(BaseResolweResource):
     """Resolwe Data resource.
 
     One and only one of the identifiers (slug, id or model_data)
     should be given.
@@ -24,20 +26,21 @@
     :param resolwe: Resolwe instance
     :type resolwe: Resolwe object
     :param model_data: Resource model data
 
     """
 
     endpoint = 'data'
+    full_search_paramater = 'text'
 
     READ_ONLY_FIELDS = BaseResolweResource.READ_ONLY_FIELDS + (
-        'checksum', 'descriptor_dirty', 'finished', 'process_cores', 'process_error',
-        'process_info', 'process_input_schema', 'process_memory', 'process_name',
-        'process_output_schema', 'process_progress', 'process_rc', 'process_slug', 'process_type',
-        'process_warning', 'output', 'size', 'started', 'status',
+        'checksum', 'descriptor_dirty', 'process_cores', 'process_error', 'process_info',
+        'process_input_schema', 'process_memory', 'process_name', 'process_output_schema',
+        'process_progress', 'process_rc', 'process_slug', 'process_type', 'process_warning',
+        'output', 'size', 'status',
     )
     UPDATE_PROTECTED_FIELDS = BaseResolweResource.UPDATE_PROTECTED_FIELDS + (
         'input', 'process',
     )
     WRITABLE_FIELDS = BaseResolweResource.WRITABLE_FIELDS + (
         'descriptor', 'descriptor_schema', 'tags',
     )
@@ -69,18 +72,14 @@
         self.process_output_schema = None
         #: actual output values
         self.output = None
         #: annotation data, with the form defined in descriptor_schema
         self.descriptor = None
         #: The ID of the process used in this data object
         self.process = None
-        #: start time of the process in data object
-        self.started = None
-        #: finish time of the process in data object
-        self.finished = None
         #: checksum field calculated on inputs
         self.checksum = None
         #: process status - Possible values: Uploading(UP), Resolving(RE),
         #: Waiting(WT), Processing(PR), Done(OK), Error(ER), Dirty (DR)
         self.status = None
         #: process progress in percentage
         self.process_progress = None
@@ -198,14 +197,28 @@
             dschema = DescriptorSchema(resolwe=self.resolwe, **dschema)
 
         self._descriptor_schema = get_descriptor_schema_id(dschema)
         # Save descriptor schema if already hydrated, otherwise it will be rerived in getter
         self._hydrated_descriptor_schema = dschema if is_descriptor_schema(dschema) else None
 
     @property
+    def started(self):
+        """Start time."""
+        if not self.id:
+            raise ValueError('Instance must be saved before acessing `started` attribute.')
+        return parse_resolwe_datetime(self._original_values['started'])
+
+    @property
+    def finished(self):
+        """Finish time."""
+        if not self.id:
+            raise ValueError('Instance must be saved before acessing `finished` attribute.')
+        return parse_resolwe_datetime(self._original_values['finished'])
+
+    @property
     def parents(self):
         """Get parents of this Data object."""
         if self.id is None:
             raise ValueError('Instance must be saved before accessing `parents` attribute.')
         if self._parents is None:
             self._parents = self.resolwe.data.filter(children=self.id)
```

### Comparing `resdk-8.0.0/resdk/tests/unit/test_resolwe.py` & `resdk-9.0.0/resdk/tests/unit/test_resolwe.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/unit/test_utils.py` & `resdk-9.0.0/resdk/tests/unit/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 Unit tests for resdk/resources/utils.py file.
 """
 # pylint: disable=missing-docstring, protected-access
 
 import unittest
 
+import pytz
 import six
 from mock import MagicMock, call, patch
 
 from resdk.resources import Collection, Data, Process, Relation, Sample
 from resdk.resources.utils import (
     _print_input_line, fill_spaces, find_field, flatten_field, get_collection_id, get_data_id,
     get_process_id, get_relation_id, get_resolwe, get_resource_collection, get_sample_id,
-    get_samples, iterate_fields, iterate_schema,
+    get_samples, iterate_fields, iterate_schema, parse_resolwe_datetime,
 )
 
 PROCESS_OUTPUT_SCHEMA = [
     {'name': "fastq", 'type': "basic:file:", 'label': "Reads file"},
     {'name': "bases", 'type': "basic:string:", 'label': "Number of bases"},
     {'name': "options", 'label': "Options", 'group': [
         {'name': "id", 'type': "basic:string:", 'label': "ID"},
@@ -309,10 +310,23 @@
         self.assertEqual(get_resolwe(relation, sample), resolwe_mock)
 
         relation = Relation(id=1, resolwe=MagicMock())
         sample = Sample(id=1, resolwe=MagicMock())
         with self.assertRaises(TypeError):
             get_resolwe(relation, sample)
 
+    @patch('resdk.resources.utils.tzlocal')
+    def test_parse_resolwe_datetime(self, tzlocal_mock):
+        tzlocal_mock.get_localzone.return_value = pytz.timezone('US/Hawaii')
+        dtime = parse_resolwe_datetime('2018-06-01T16:12:34.123456+02:00')
+        self.assertEqual(dtime.year, 2018)
+        self.assertEqual(dtime.month, 6)
+        self.assertEqual(dtime.day, 1)
+        self.assertEqual(dtime.hour, 6)
+        self.assertEqual(dtime.minute, 12)
+        self.assertEqual(dtime.second, 34)
+        self.assertEqual(dtime.microsecond, 123456)
+        self.assertEqual(dtime.tzinfo.zone, 'US/Hawaii')
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `resdk-8.0.0/resdk/tests/unit/test_decorators.py` & `resdk-9.0.0/resdk/tests/unit/test_decorators.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/unit/test_collections_shortcuts.py` & `resdk-9.0.0/resdk/tests/unit/test_collections_shortcuts.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/unit/test_sample.py` & `resdk-9.0.0/resdk/tests/unit/test_sample.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/unit/test_exceptions.py` & `resdk-9.0.0/resdk/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/unit/test_process.py` & `resdk-9.0.0/resdk/tests/unit/test_process.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/unit/test_users.py` & `resdk-9.0.0/resdk/tests/unit/test_users.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/unit/test_query.py` & `resdk-9.0.0/resdk/tests/unit/test_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,32 +13,22 @@
 
 class TestResolweQuery(unittest.TestCase):
 
     def test_init(self):
         resolwe = MagicMock()
         resource = MagicMock(endpoint='resolwe_endpoint', query_endpoint=None, query_method='GET')
 
-        query = ResolweQuery(resolwe, resource, 'endpoint')
-        self.assertEqual(query.resolwe, resolwe)
-        self.assertEqual(query.resource, resource)
-        self.assertEqual(query.endpoint, 'endpoint')
-
         query = ResolweQuery(resolwe, resource)
         self.assertEqual(query.resolwe, resolwe)
         self.assertEqual(query.resource, resource)
         self.assertEqual(query.endpoint, 'resolwe_endpoint')
 
         resource = MagicMock(endpoint='resolwe_endpoint', query_endpoint='query_endpoint',
                              query_method='GET')
 
-        query = ResolweQuery(resolwe, resource, 'endpoint')
-        self.assertEqual(query.resolwe, resolwe)
-        self.assertEqual(query.resource, resource)
-        self.assertEqual(query.endpoint, 'endpoint')
-
         query = ResolweQuery(resolwe, resource)
         self.assertEqual(query.resolwe, resolwe)
         self.assertEqual(query.resource, resource)
         self.assertEqual(query.endpoint, 'query_endpoint')
 
     def test_getitem_invalid(self):
         query = MagicMock(spec=ResolweQuery)
@@ -105,16 +95,22 @@
     def test_len(self):
         query = MagicMock(spec=ResolweQuery, **{'count.return_value': 3})
         query.__len__ = ResolweQuery.__len__
 
         self.assertEqual(len(query), 3)
 
     def test_clone(self):
-        query = MagicMock(spec=ResolweQuery, _cache=[1, 2, 3], _filters=defaultdict(list),
-                          _limit=2, _offset=3, endpoint='endpoint')
+        query = MagicMock(
+            spec=ResolweQuery,
+            resource=MagicMock(query_endpoint='foo'),
+            _cache=[1, 2, 3],
+            _filters=defaultdict(list),
+            _limit=2,
+            _offset=3,
+        )
 
         new_query = ResolweQuery._clone(query)
         self.assertEqual(new_query._cache, None)  # cache shouldnt be copied
         self.assertEqual(new_query._filters, {})
         self.assertEqual(new_query._limit, 2)
         self.assertEqual(new_query._offset, 3)
 
@@ -213,20 +209,14 @@
         with self.assertRaises(LookupError):
             ResolweQuery.get(query, 1)
 
         new_query.__iter__.return_value = ['object 1', 'object 2']
         with self.assertRaises(LookupError):
             ResolweQuery.get(query, 1)
 
-    def test_post(self):
-        query = MagicMock(spec=ResolweQuery)
-
-        ResolweQuery.post(query, {'id': 2, 'name': 'Test object'})
-        query.api.post.assert_called_once_with({'id': 2, 'name': 'Test object'})
-
     def test_filter(self):
         new_query = MagicMock(spec=ResolweQuery)
         query = MagicMock(spec=ResolweQuery, **{'_clone.return_value': new_query})
 
         result = ResolweQuery.filter(query, id=2)
         result._add_filter.assert_called_once_with({'id': 2})  # pylint: disable=no-member
         # make sure that original hasnt changed
@@ -235,16 +225,31 @@
     def test_all(self):
         new_query = MagicMock(spec=ResolweQuery)
         query = MagicMock(spec=ResolweQuery, **{'_clone.return_value': new_query})
 
         result = ResolweQuery.all(query)
         self.assertEqual(result, new_query)
 
-    def test_search(self):
-        query = MagicMock(spec=ResolweQuery)
+    def test_search_undefined(self):
+        resolwe = MagicMock()
+        resource = MagicMock(full_search_paramater=None, query_endpoint='endpoint')
+        query = ResolweQuery(resolwe, resource)
 
+        # If ``full_search_paramater`` is not defined, raise NotImplemented error.
         with self.assertRaises(NotImplementedError):
-            ResolweQuery.search(query)
+            query.search('foo bar')
+
+    def test_search(self):
+        resolwe = MagicMock()
+        resource = MagicMock(full_search_paramater='text', query_endpoint='endpoint',
+                             query_method='GET')
+        query = ResolweQuery(resolwe, resource)
+
+        new_query = query.search('foobar')
+        self.assertEqual(
+            list(new_query._filters.items()),
+            list({'text': ['foobar']}.items()),
+        )
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `resdk-8.0.0/resdk/tests/unit/test_data.py` & `resdk-9.0.0/resdk/tests/unit/test_data.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/unit/test_collections.py` & `resdk-9.0.0/resdk/tests/unit/test_collections.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/unit/test_base.py` & `resdk-9.0.0/resdk/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/unit/test_relations.py` & `resdk-9.0.0/resdk/tests/unit/test_relations.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/files/example.fastq` & `resdk-9.0.0/resdk/tests/files/example.fastq`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/files/reads.fastq.gz` & `resdk-9.0.0/resdk/tests/files/reads.fastq.gz`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/files/genome.fasta.gz` & `resdk-9.0.0/resdk/tests/files/genome.fasta.gz`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/functional/analysis/e2e_chip_seq.py` & `resdk-9.0.0/resdk/tests/functional/analysis/e2e_chip_seq.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/functional/analysis/e2e_alignment.py` & `resdk-9.0.0/resdk/tests/functional/analysis/e2e_alignment.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/functional/analysis/e2e_expressions.py` & `resdk-9.0.0/resdk/tests/functional/analysis/e2e_expressions.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/functional/analysis/e2e_differential_expressions.py` & `resdk-9.0.0/resdk/tests/functional/analysis/e2e_differential_expressions.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/functional/analysis/e2e_prepare_geo.py` & `resdk-9.0.0/resdk/tests/functional/analysis/e2e_prepare_geo.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,62 +41,52 @@
         relation = collection_3.create_background_relation('background1', samples[3], [samples[4]])
 
         # Run macs
         macs_1, macs_2 = collection_1.run_macs()
         macs_3 = relation.run_macs()[0]
         macs_4 = samples[5].run_macs(use_background=False)[0]
 
-        relations = [
-            "{}:{}".format(samples[1].name, samples[0].name),
-            "{}:{}".format(samples[2].name, samples[0].name),
-            "{}:{}".format(samples[4].name, samples[3].name)
-        ]
-
         reads_id = [read.id for read in reads]
         macs_id = [macs_1.id, macs_2.id, macs_3.id, macs_4.id]
 
         # Run on collection
         prepare_geo_chipseq = collection_1.run_prepare_geo_chipseq()
         self.assertEqual(prepare_geo_chipseq.input['reads'], reads_id[:3])
-        self.assertEqual(prepare_geo_chipseq.input['macs14'], macs_id[:2])
+        self.assertEqual(prepare_geo_chipseq.input['macs'], macs_id[:2])
         self.assertEqual(prepare_geo_chipseq.input['name'], collection_1.name)
-        self.assertEqual(prepare_geo_chipseq.input['relations'], relations[:2])
 
         # Second run with same parameters should return same objects
         prepare_geo_chipseq_2 = collection_1.run_prepare_geo_chipseq()
         self.assertEqual(prepare_geo_chipseq.id, prepare_geo_chipseq_2.id)
 
         # Run on a list of samples all in the same collection
         prepare_geo_chipseq = prepare_geo.prepare_geo_chipseq(samples[:3])
         self.assertEqual(prepare_geo_chipseq.id, prepare_geo_chipseq_2.id)
 
         # Run on samples that are in two different collections
         prepare_geo_chipseq = prepare_geo.prepare_geo_chipseq(samples[:3] + [samples[5]])
         self.assertEqual(prepare_geo_chipseq.input['reads'], reads_id[:3] + [reads_id[5]])
-        self.assertEqual(prepare_geo_chipseq.input['macs14'], macs_id[:2] + [macs_id[3]])
-        self.assertEqual(prepare_geo_chipseq.input['relations'], relations[:2])
+        self.assertEqual(prepare_geo_chipseq.input['macs'], macs_id[:2] + [macs_id[3]])
 
         # Run on all samples
         prepare_geo_chipseq = prepare_geo.prepare_geo_chipseq(samples)
         self.assertEqual(prepare_geo_chipseq.input['reads'], reads_id)
-        self.assertEqual(prepare_geo_chipseq.input['macs14'], macs_id)
-        self.assertEqual(prepare_geo_chipseq.input['relations'], relations)
+        self.assertEqual(prepare_geo_chipseq.input['macs'], macs_id)
 
         # Run only on samples that are not in a collection
         prepare_geo_chipseq = prepare_geo.prepare_geo_chipseq(samples[3:5])
         self.assertEqual(prepare_geo_chipseq.input['reads'], reads_id[3:5])
-        self.assertEqual(prepare_geo_chipseq.input['macs14'], [macs_id[2]])
-        self.assertEqual(prepare_geo_chipseq.input['relations'], [relations[2]])
+        self.assertEqual(prepare_geo_chipseq.input['macs'], [macs_id[2]])
 
-        # Run on a sample that has two macs14 data objects
+        # Run on a sample that has two macs data objects
         samples[1].add_data(macs_2)
         with self.assertRaises(ValueError):
             collection_1.run_prepare_geo_chipseq()
 
-        # Run on a sample that has no macs14 data object
+        # Run on a sample that has no macs data object
         samples[1].remove_data(macs_2)
         samples[1].remove_data(macs_1)
         with self.assertRaises(ValueError):
             collection_1.run_prepare_geo_chipseq()
 
         # Run on a sample whose background is not in the resource - sample_list
         with self.assertRaises(ValueError):
```

### Comparing `resdk-8.0.0/resdk/tests/functional/docs/e2e_docs.py` & `resdk-9.0.0/resdk/tests/functional/docs/e2e_docs.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/functional/permissions/e2e_permissions.py` & `resdk-9.0.0/resdk/tests/functional/permissions/e2e_permissions.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/functional/resolwe/e2e_resolwe.py` & `resdk-9.0.0/resdk/tests/functional/resolwe/e2e_resolwe.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/tests/functional/base.py` & `resdk-9.0.0/resdk/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/utils/decorators.py` & `resdk-9.0.0/resdk/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/scripts/reads.py` & `resdk-9.0.0/resdk/scripts/reads.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/shortcuts/collection.py` & `resdk-9.0.0/resdk/shortcuts/collection.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk/__about__.py` & `resdk-9.0.0/resdk/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #       interfere with a global variable __name__ denoting object's name.
 __title__ = 'resdk'
 __summary__ = 'Resolwe SDK for Python'
 __url__ = 'https://github.com/genialis/resolwe-bio-py'
 
 # Semantic versioning is used. For more information see:
 # https://packaging.python.org/en/latest/distributing/#semantic-versioning-preferred
-__version__ = '8.0.0'
+__version__ = '9.0.0'
 
 __author__ = 'Genialis, Inc.'
 __email__ = 'dev-team@genialis.com'
 
 __license__ = 'Apache License (2.0)'
 __copyright__ = '2015-2017, ' + __author__
```

### Comparing `resdk-8.0.0/resdk/exceptions.py` & `resdk-9.0.0/resdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/LICENSE` & `resdk-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/docs/tutorial-create.rst` & `resdk-9.0.0/docs/tutorial-create.rst`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/docs/index.rst` & `resdk-9.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/docs/contributing.rst` & `resdk-9.0.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/docs/images/input_schema.jpg` & `resdk-9.0.0/docs/images/input_schema.jpg`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/docs/images/data-hierarchy-diagram.png` & `resdk-9.0.0/docs/images/data-hierarchy-diagram.png`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/docs/images/define_sample_collection_relations-02.png` & `resdk-9.0.0/docs/images/define_sample_collection_relations-02.png`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/docs/images/resolwe_resdk.jpg` & `resdk-9.0.0/docs/images/resolwe_resdk.jpg`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/docs/images/define_sample_collection_relations-03.png` & `resdk-9.0.0/docs/images/define_sample_collection_relations-03.png`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/docs/images/collections_relation.jpg` & `resdk-9.0.0/docs/images/collections_relation.jpg`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/docs/images/define_sample_collection_relations-01.png` & `resdk-9.0.0/docs/images/define_sample_collection_relations-01.png`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/docs/tutorial-get.rst` & `resdk-9.0.0/docs/tutorial-get.rst`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/docs/conf.py` & `resdk-9.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/docs/tutorial-basics.rst` & `resdk-9.0.0/docs/tutorial-basics.rst`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/docs/files/tutorial-create.py` & `resdk-9.0.0/docs/files/tutorial-create.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/docs/files/start.py` & `resdk-9.0.0/docs/files/start.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/docs/files/tutorial-get.py` & `resdk-9.0.0/docs/files/tutorial-get.py`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/docs/CHANGELOG.rst` & `resdk-9.0.0/docs/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,32 @@
 Change Log
 ##########
 
 All notable changes to this project are documented in this file.
 
 
 ==================
+9.0.0 - 2019-02-19
+==================
+
+Changed
+-------
+* **BACKWARD INCOMPATIBLE:** Remove unused ``ResolweQuery.post`` method
+* Make contributor attribute a User object
+* Cast date-time attributes to datetime objects. This means, for example,
+  that ``created`` attribute is now Python datetime object instead of string.
+* Update prepare_geo_chipseq analysis to reflect process chnages
+
+Added
+-----
+* Implement full text search method in ``ResolweQuery`` for ``Data``,
+  ``Sample`` and ``Collection`` resources
+
+
+==================
 8.0.0 - 2018-11-20
 ==================
 
 Changed
 -------
 * **BACKWARD INCOMPATIBLE:** Rename argument ``file_type`` to ``field_name``
   in ``BaseCollection.download`` method
```

### Comparing `resdk-8.0.0/docs/start.rst` & `resdk-9.0.0/docs/start.rst`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/setup.py` & `resdk-9.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,16 @@
     zip_safe=False,
     install_requires=(
         'requests>=2.6.0',
         'slumber>=0.7.1',
         'six>=1.10.0',
         'pyyaml>=3.11',
         'wrapt>=1.10.8',
+        'pytz>=2018.4',
+        'tzlocal>=1.5.1',
     ),
     extras_require={
         'docs': [
             'sphinx>=1.4.1',
             'sphinx_rtd_theme>=0.1.9',
         ],
         'package': [
```

### Comparing `resdk-8.0.0/tox.ini` & `resdk-9.0.0/tox.ini`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/setup.cfg` & `resdk-9.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/README.rst` & `resdk-9.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `resdk-8.0.0/resdk.egg-info/PKG-INFO` & `resdk-9.0.0/resdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resdk
-Version: 8.0.0
+Version: 9.0.0
 Summary: Resolwe SDK for Python
 Home-page: https://github.com/genialis/resolwe-bio-py
 Author: Genialis, Inc.
 Author-email: dev-team@genialis.com
 License: Apache License (2.0)
 Description: ======================
         Resolwe SDK for Python
@@ -122,10 +122,10 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
-Provides-Extra: docs
-Provides-Extra: package
 Provides-Extra: test
+Provides-Extra: package
+Provides-Extra: docs
```

### Comparing `resdk-8.0.0/resdk.egg-info/SOURCES.txt` & `resdk-9.0.0/resdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

