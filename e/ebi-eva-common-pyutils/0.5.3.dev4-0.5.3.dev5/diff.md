# Comparing `tmp/ebi_eva_common_pyutils-0.5.3.dev4.tar.gz` & `tmp/ebi_eva_common_pyutils-0.5.3.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebi_eva_common_pyutils-0.5.3.dev4.tar", last modified: Sun Apr 23 11:26:01 2023, max compression
+gzip compressed data, was "ebi_eva_common_pyutils-0.5.3.dev5.tar", last modified: Tue Apr 25 06:17:51 2023, max compression
```

## Comparing `ebi_eva_common_pyutils-0.5.3.dev4.tar` & `ebi_eva_common_pyutils-0.5.3.dev5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 11:26:01.152649 ebi_eva_common_pyutils-0.5.3.dev4/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1492 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev4/CHANGELOG.md
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    11357 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev4/LICENSE
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       28 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev4/MANIFEST.in
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      545 2023-04-23 11:26:01.152649 ebi_eva_common_pyutils-0.5.3.dev4/PKG-INFO
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1434 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev4/README.md
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 11:26:01.148649 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4984 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/archive_directory.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 11:26:01.148649 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/assembly/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       66 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/assembly/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1481 2023-04-23 08:50:32.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/assembly/assembly.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2151 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/command_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1192 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/common_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2242 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/config.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     7838 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/config_utils.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 11:26:01.148649 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/contig_alias/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/contig_alias/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3056 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/contig_alias/contig_alias.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1452 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/ena_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1375 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/file_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4990 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/logger.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    15607 2023-04-23 11:24:40.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/metadata_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3589 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/mongo_utils.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 11:26:01.148649 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/mongodb/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       72 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/mongodb/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     9676 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/mongodb/mongo_database.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4009 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/ncbi_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2285 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/network_utils.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 11:26:01.148649 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/nextflow/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      120 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/nextflow/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    10114 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4398 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/pg_utils.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 11:26:01.152649 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/reference/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      134 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/reference/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    12162 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/reference/assembly.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3911 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/reference/sequence.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     9540 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/spring_properties.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 11:26:01.152649 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/taxonomy/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/taxonomy/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2259 2023-04-23 09:52:55.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/taxonomy/taxonomy.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 11:26:01.152649 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/variation/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/variation/__init__.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3515 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/variation/assembly_utils.py
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     5230 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/variation/contig_utils.py
-drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 11:26:01.148649 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils.egg-info/
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      545 2023-04-23 11:26:01.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1702 2023-04-23 11:26:01.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        1 2023-04-23 11:26:01.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       81 2023-04-23 11:26:01.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils.egg-info/requires.txt
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       23 2023-04-23 11:26:01.000000 ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils.egg-info/top_level.txt
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      225 2023-04-23 11:26:01.152649 ebi_eva_common_pyutils-0.5.3.dev4/setup.cfg
--rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      912 2023-04-23 11:25:36.000000 ebi_eva_common_pyutils-0.5.3.dev4/setup.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-25 06:17:51.066863 ebi_eva_common_pyutils-0.5.3.dev5/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1492 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev5/CHANGELOG.md
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    11357 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev5/LICENSE
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       28 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev5/MANIFEST.in
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      545 2023-04-25 06:17:51.066863 ebi_eva_common_pyutils-0.5.3.dev5/PKG-INFO
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1434 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev5/README.md
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-25 06:17:51.058863 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4984 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/archive_directory.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-25 06:17:51.062863 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/assembly/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       66 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/assembly/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1569 2023-04-23 12:01:06.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/assembly/assembly.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2151 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/command_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1192 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/common_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2242 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/config.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     7838 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/config_utils.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-25 06:17:51.062863 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/contig_alias/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/contig_alias/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3056 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/contig_alias/contig_alias.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1452 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/ena_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1375 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/file_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4990 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/logger.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    14950 2023-04-25 06:14:55.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/metadata_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3589 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/mongo_utils.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-25 06:17:51.062863 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/mongodb/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       72 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/mongodb/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     9676 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/mongodb/mongo_database.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4009 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/ncbi_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2285 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/network_utils.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-25 06:17:51.062863 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/nextflow/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      120 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/nextflow/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    10114 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     4398 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/pg_utils.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-25 06:17:51.062863 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/reference/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      134 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/reference/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)    12162 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/reference/assembly.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3911 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/reference/sequence.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     9540 2023-04-23 07:42:51.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/spring_properties.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-25 06:17:51.062863 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/taxonomy/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/taxonomy/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     2259 2023-04-23 09:52:55.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/taxonomy/taxonomy.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-25 06:17:51.062863 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/variation/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/variation/__init__.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     3515 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/variation/assembly_utils.py
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     5230 2023-04-23 07:42:33.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/variation/contig_utils.py
+drwxr-xr-x   0 sundarvenkata  (1002) biouser   (1000)        0 2023-04-25 06:17:51.062863 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils.egg-info/
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      545 2023-04-25 06:17:50.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)     1702 2023-04-25 06:17:50.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)        1 2023-04-25 06:17:50.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       81 2023-04-25 06:17:50.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils.egg-info/requires.txt
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)       23 2023-04-25 06:17:50.000000 ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils.egg-info/top_level.txt
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      225 2023-04-25 06:17:51.066863 ebi_eva_common_pyutils-0.5.3.dev5/setup.cfg
+-rw-r--r--   0 sundarvenkata  (1002) biouser   (1000)      912 2023-04-25 06:17:17.000000 ebi_eva_common_pyutils-0.5.3.dev5/setup.py
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/CHANGELOG.md` & `ebi_eva_common_pyutils-0.5.3.dev5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/LICENSE` & `ebi_eva_common_pyutils-0.5.3.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/PKG-INFO` & `ebi_eva_common_pyutils-0.5.3.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebi_eva_common_pyutils
-Version: 0.5.3.dev4
+Version: 0.5.3.dev5
 Summary: EBI EVA - Common Python Utilities
 Home-page: https://github.com/EBIVariation/eva-common-pyutils
 License: Apache
 Keywords: EBI,EVA,PYTHON,UTILITIES
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/README.md` & `ebi_eva_common_pyutils-0.5.3.dev5/README.md`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/archive_directory.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/archive_directory.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/assembly/assembly.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/assembly/assembly.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 from ebi_eva_common_pyutils.reference.assembly import NCBIAssembly
 from ebi_eva_common_pyutils.taxonomy.taxonomy import get_scientific_name_from_ensembl
 
 logging_config.add_stdout_handler()
 logger = logging_config.get_logger(__name__)
 
 
-def get_supported_asm_from_ensembl(tax_id: int) -> str:
+def get_supported_asm_from_ensembl(tax_id: int) -> str | None:
     logger.info(f'Query Ensembl for species name using taxonomy {tax_id}')
     scientific_name_api_param = get_scientific_name_from_ensembl(tax_id).lower().replace(' ', '_')
     ENSEMBL_REST_API_URL = "http://rest.ensembl.org/info/assembly/{0}?content-type=application/json".format(
         scientific_name_api_param)
     response = json_request(ENSEMBL_REST_API_URL)
-    assembly_accession = str(response.get('assembly_accession'))
-    return assembly_accession
+    assembly_accession_attribute = 'assembly_accession'
+    if assembly_accession_attribute in response:
+        return str(response.get('assembly_accession'))
+    return None
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/command_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/common_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/common_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/config.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/config.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/config_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/contig_alias/contig_alias.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/contig_alias/contig_alias.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/ena_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/ena_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/file_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/logger.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/logger.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/metadata_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/metadata_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -254,27 +254,14 @@
     cur = metadata_connection_handle.cursor()
     cur.execute('INSERT INTO evapro.taxonomy(taxonomy_id, common_name, scientific_name, taxonomy_code, eva_name) '
                 'VALUES (%s, %s, %s, %s, %s)',
                 (taxonomy_id, common_name, scientific_name, taxonomy_code, eva_species_name))
     logger.info('New taxonomy {} added'.format(taxonomy_id))
 
 
-def get_tax_submitted_with_asm_in_eva(metadata_connection_handle, assembly_accession: str) -> list[int]:
-    """
-    :param metadata_connection_handle: Connection handle to the metadata database
-    :param assembly_accession: Assembly accession
-    :return: List of taxonomies submitted to EVA where variants were called with the given assembly accession
-
-    """
-    get_tax_for_asm_query = "select distinct taxonomy_id from {0} where assembly_id = '{1}'".format(
-        SUPPORTED_ASSEMBLY_TRACKER_TABLE, assembly_accession)
-    result = get_all_results_for_query(metadata_connection_handle, get_tax_for_asm_query)
-    return [row[0] for row in result]
-
-
 def add_to_supported_assemblies(metadata_connection_handle, source_of_assembly: str, target_assembly: str,
                                 taxonomy_id: int):
     today = datetime.date.today().strftime('%Y-%m-%d')
     # First check if the current assembly is already target - if so don't do anything
     current_query = (
         f"SELECT assembly_id FROM evapro.supported_assembly_tracker "
         f"WHERE taxonomy_id={taxonomy_id} AND current=true;"
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/mongo_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/mongo_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/mongodb/mongo_database.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/mongodb/mongo_database.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/ncbi_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/ncbi_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/network_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/network_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/pg_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/pg_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/reference/assembly.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/reference/assembly.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/reference/sequence.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/reference/sequence.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/spring_properties.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/spring_properties.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/taxonomy/taxonomy.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/taxonomy/taxonomy.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/variation/assembly_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/variation/assembly_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils/variation/contig_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils/variation/contig_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils.egg-info/PKG-INFO` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebi-eva-common-pyutils
-Version: 0.5.3.dev4
+Version: 0.5.3.dev5
 Summary: EBI EVA - Common Python Utilities
 Home-page: https://github.com/EBIVariation/eva-common-pyutils
 License: Apache
 Keywords: EBI,EVA,PYTHON,UTILITIES
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/ebi_eva_common_pyutils.egg-info/SOURCES.txt` & `ebi_eva_common_pyutils-0.5.3.dev5/ebi_eva_common_pyutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev4/setup.py` & `ebi_eva_common_pyutils-0.5.3.dev5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages
 
 setup(
     name='ebi_eva_common_pyutils',
     scripts=[os.path.join(os.path.dirname(__file__), 'ebi_eva_common_pyutils', 'archive_directory.py')],
     packages=find_packages(),
-    version='0.5.3.dev4',
+    version='0.5.3.dev5',
     license='Apache',
     description='EBI EVA - Common Python Utilities',
     url='https://github.com/EBIVariation/eva-common-pyutils',
     keywords=['EBI', 'EVA', 'PYTHON', 'UTILITIES'],
     install_requires=['psycopg2-binary', 'requests', 'pymongo', 'lxml', 'pyyaml', 'cached-property', 'retry',
                       'networkx<=2.5'],
     classifiers=[
```

