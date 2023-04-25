# Comparing `tmp/arkindex-base-worker-0.3.3rc1.tar.gz` & `tmp/arkindex-base-worker-0.3.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkindex-base-worker-0.3.3rc1.tar", last modified: Thu Apr 13 07:20:02 2023, max compression
+gzip compressed data, was "arkindex-base-worker-0.3.3rc2.tar", last modified: Tue Apr 25 08:57:11 2023, max compression
```

## Comparing `arkindex-base-worker-0.3.3rc1.tar` & `arkindex-base-worker-0.3.3rc2.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:20:02.570545 arkindex-base-worker-0.3.3rc1/
--rw-r--r--   0 root         (0) root         (0)      248 2023-04-13 07:20:02.570545 arkindex-base-worker-0.3.3rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:20:02.566545 arkindex-base-worker-0.3.3rc1/arkindex_base_worker.egg-info/
--rw-r--r--   0 root         (0) root         (0)      248 2023-04-13 07:20:02.000000 arkindex-base-worker-0.3.3rc1/arkindex_base_worker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1304 2023-04-13 07:20:02.000000 arkindex-base-worker-0.3.3rc1/arkindex_base_worker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 07:20:02.000000 arkindex-base-worker-0.3.3rc1/arkindex_base_worker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      318 2023-04-13 07:20:02.000000 arkindex-base-worker-0.3.3rc1/arkindex_base_worker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-13 07:20:02.000000 arkindex-base-worker-0.3.3rc1/arkindex_base_worker.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:20:02.566545 arkindex-base-worker-0.3.3rc1/arkindex_worker/
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10890 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/cache.py
--rw-rw-rw-   0 root         (0) root         (0)    15338 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/git.py
--rw-rw-rw-   0 root         (0) root         (0)    13490 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/image.py
--rw-rw-rw-   0 root         (0) root         (0)     9619 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/models.py
--rw-rw-rw-   0 root         (0) root         (0)     8012 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/reporting.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:20:02.566545 arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/
--rw-rw-rw-   0 root         (0) root         (0)    11662 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15723 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/base.py
--rw-rw-rw-   0 root         (0) root         (0)    10935 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/classification.py
--rw-rw-rw-   0 root         (0) root         (0)    19034 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/element.py
--rw-rw-rw-   0 root         (0) root         (0)    14657 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/entity.py
--rw-rw-rw-   0 root         (0) root         (0)     6657 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11714 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/training.py
--rw-rw-rw-   0 root         (0) root         (0)    19105 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/transcription.py
--rw-rw-rw-   0 root         (0) root         (0)     1460 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/version.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-04-13 07:20:02.570545 arkindex-base-worker-0.3.3rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      783 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:20:02.570545 arkindex-base-worker-0.3.3rc1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17535 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    21312 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_base_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     8699 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    12961 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_element.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:20:02.570545 arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    32744 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_classifications.py
--rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    52801 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_elements.py
--rw-rw-rw-   0 root         (0) root         (0)    36695 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_entities.py
--rw-rw-rw-   0 root         (0) root         (0)    18023 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     8330 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_training.py
--rw-rw-rw-   0 root         (0) root         (0)    69404 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_transcriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10239 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_worker.py
--rw-rw-rw-   0 root         (0) root         (0)    14944 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_git.py
--rw-rw-rw-   0 root         (0) root         (0)    14356 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_image.py
--rw-rw-rw-   0 root         (0) root         (0)     8224 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_merge.py
--rw-rw-rw-   0 root         (0) root         (0)     8802 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_reporting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:57:11.720569 arkindex-base-worker-0.3.3rc2/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-04-25 08:57:11.720569 arkindex-base-worker-0.3.3rc2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:57:11.716569 arkindex-base-worker-0.3.3rc2/arkindex_base_worker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-04-25 08:57:11.000000 arkindex-base-worker-0.3.3rc2/arkindex_base_worker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-04-25 08:57:11.000000 arkindex-base-worker-0.3.3rc2/arkindex_base_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 08:57:11.000000 arkindex-base-worker-0.3.3rc2/arkindex_base_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      318 2023-04-25 08:57:11.000000 arkindex-base-worker-0.3.3rc2/arkindex_base_worker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-25 08:57:11.000000 arkindex-base-worker-0.3.3rc2/arkindex_base_worker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:57:11.716569 arkindex-base-worker-0.3.3rc2/arkindex_worker/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10871 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    15338 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/git.py
+-rw-rw-rw-   0 root         (0) root         (0)    13466 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     9619 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     8012 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/reporting.py
+-rw-rw-rw-   0 root         (0) root         (0)     5507 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:57:11.716569 arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/
+-rw-rw-rw-   0 root         (0) root         (0)    11662 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15968 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10935 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)    19034 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/element.py
+-rw-rw-rw-   0 root         (0) root         (0)    14657 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/entity.py
+-rw-rw-rw-   0 root         (0) root         (0)     6657 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    10374 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/training.py
+-rw-rw-rw-   0 root         (0) root         (0)    19105 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/transcription.py
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-04-25 08:57:11.720569 arkindex-base-worker-0.3.3rc2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      768 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:57:11.720569 arkindex-base-worker-0.3.3rc2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17541 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    21333 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_base_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     8705 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    12961 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_element.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 08:57:11.720569 arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    32744 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_classifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    52786 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_elements.py
+-rw-rw-rw-   0 root         (0) root         (0)    36695 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)    18023 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     8292 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_training.py
+-rw-rw-rw-   0 root         (0) root         (0)    69404 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_transcriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10239 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)    14944 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_git.py
+-rw-rw-rw-   0 root         (0) root         (0)    14353 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     8406 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_merge.py
+-rw-rw-rw-   0 root         (0) root         (0)     8802 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_reporting.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-04-25 08:50:41.000000 arkindex-base-worker-0.3.3rc2/tests/test_utils.py
```

### Comparing `arkindex-base-worker-0.3.3rc1/arkindex_base_worker.egg-info/SOURCES.txt` & `arkindex-base-worker-0.3.3rc2/arkindex_base_worker.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 arkindex_base_worker.egg-info/top_level.txt
 arkindex_worker/__init__.py
 arkindex_worker/cache.py
 arkindex_worker/git.py
 arkindex_worker/image.py
 arkindex_worker/models.py
 arkindex_worker/reporting.py
+arkindex_worker/utils.py
 arkindex_worker/worker/__init__.py
 arkindex_worker/worker/base.py
 arkindex_worker/worker/classification.py
 arkindex_worker/worker/element.py
 arkindex_worker/worker/entity.py
 arkindex_worker/worker/metadata.py
 arkindex_worker/worker/training.py
@@ -26,14 +27,15 @@
 tests/test_base_worker.py
 tests/test_cache.py
 tests/test_element.py
 tests/test_git.py
 tests/test_image.py
 tests/test_merge.py
 tests/test_reporting.py
+tests/test_utils.py
 tests/test_elements_worker/__init__.py
 tests/test_elements_worker/test_classifications.py
 tests/test_elements_worker/test_cli.py
 tests/test_elements_worker/test_elements.py
 tests/test_elements_worker/test_entities.py
 tests/test_elements_worker/test_metadata.py
 tests/test_elements_worker/test_training.py
```

### Comparing `arkindex-base-worker-0.3.3rc1/arkindex_worker/cache.py` & `arkindex-base-worker-0.3.3rc2/arkindex_worker/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 On methods that support caching, the database will be used for all reads,
 and writes will go both to the Arkindex API and the database,
 reducing network usage.
 """
 
 import json
-import os
 import sqlite3
 from pathlib import Path
 from typing import Optional, Union
 
 from peewee import (
     BooleanField,
     CharField,
@@ -168,15 +167,15 @@
     """
     Cache transcription table
     """
 
     id = UUIDField(primary_key=True)
     element = ForeignKeyField(CachedElement, backref="transcriptions")
     text = TextField()
-    confidence = FloatField()
+    confidence = FloatField(null=True)
     orientation = CharField(max_length=50)
     # Needed to filter transcriptions with cache
     worker_version_id = UUIDField(null=True)
     worker_run_id = UUIDField(null=True)
 
     class Meta:
         database = db
@@ -246,15 +245,15 @@
     CachedClassification,
     CachedEntity,
     CachedTranscriptionEntity,
 ]
 SQL_VERSION = 2
 
 
-def init_cache_db(path: str):
+def init_cache_db(path: Path):
     """
     Create the cache database on the given path
     :param path: Where the new database should be created
     """
     db.init(
         path,
         pragmas={
@@ -300,54 +299,54 @@
 
             assert (
                 version == SQL_VERSION
             ), f"The SQLite database {cache_path} does not have the correct cache version, it should be {SQL_VERSION}"
 
 
 def retrieve_parents_cache_path(
-    parent_ids: list, data_dir: str = "/data", chunk: int = None
+    parent_ids: list, data_dir: Path = Path("/data"), chunk: int = None
 ) -> list:
     """
     Retrieve the path of the given parent's in the
     :param parent_ids: List of element IDs to search
     :param data_dir: Base folder where to look for
     :param chunk: Index of the chunk of the db that might contain the paths
     :return: The corresponding list of paths
     """
     assert isinstance(parent_ids, list)
-    assert os.path.isdir(data_dir)
+    assert data_dir.is_dir()
 
     # Handle possible chunk in parent task name
     # This is needed to support the init_elements databases
     filenames = [
         "db.sqlite",
     ]
     if chunk is not None:
         filenames.append(f"db_{chunk}.sqlite")
 
     # Find all the paths for these databases
     return list(
         filter(
-            lambda p: os.path.isfile(p),
+            lambda p: p.is_file(),
             [
-                os.path.join(data_dir, parent, name)
+                Path(data_dir, parent, name)
                 for parent in parent_ids
                 for name in filenames
             ],
         )
     )
 
 
-def merge_parents_cache(paths: list, current_database: str):
+def merge_parents_cache(paths: list, current_database: Path):
     """
     Merge all the potential parent task's databases into the existing local one
     :param paths: Path to cache databases
     :param current_database: Path to the current database
     """
-    assert os.path.exists(current_database)
+    assert current_database.exists()
 
     if not paths:
         logger.info("No parents cache to use")
         return
 
     # Open a connection on current database
     connection = sqlite3.connect(current_database)
```

### Comparing `arkindex-base-worker-0.3.3rc1/arkindex_worker/git.py` & `arkindex-base-worker-0.3.3rc2/arkindex_worker/git.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc1/arkindex_worker/image.py` & `arkindex-base-worker-0.3.3rc2/arkindex_worker/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 """
 Helper methods to download and open IIIF images, and manage polygons.
 """
-import os
 from collections import namedtuple
 from io import BytesIO
 from math import ceil
 from pathlib import Path
 from typing import TYPE_CHECKING, List, Optional, Union
 
 import requests
@@ -30,15 +29,15 @@
 # See http://docs.python-requests.org/en/master/user/advanced/#timeouts
 DOWNLOAD_TIMEOUT = (30, 60)
 
 BoundingBox = namedtuple("BoundingBox", ["x", "y", "width", "height"])
 
 
 def open_image(
-    path: Union[str, Path],
+    path: str,
     mode: Optional[str] = "RGB",
     rotation_angle: Optional[int] = 0,
     mirrored: Optional[bool] = False,
 ) -> Image:
     """
     Open an image from a path or a URL.
 
@@ -54,15 +53,15 @@
        the mode's default color to be added for padding.
     :param mirrored: Whether or not to mirror the image horizontally.
     :returns: A Pillow image.
     """
     if (
         path.startswith("http://")
         or path.startswith("https://")
-        or not os.path.exists(path)
+        or not Path(path).exists()
     ):
         image = download_image(path)
     else:
         try:
             image = Image.open(path)
         except (IOError, ValueError):
             image = download_image(path)
```

### Comparing `arkindex-base-worker-0.3.3rc1/arkindex_worker/models.py` & `arkindex-base-worker-0.3.3rc2/arkindex_worker/models.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc1/arkindex_worker/reporting.py` & `arkindex-base-worker-0.3.3rc2/arkindex_worker/reporting.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/__init__.py` & `arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/base.py` & `arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             help="Alternative configuration file when running without a Worker Version ID",
             type=open,
         )
         self.parser.add_argument(
             "-d",
             "--database",
             help="Alternative SQLite database to use for worker caching",
-            type=str,
+            type=Path,
             default=None,
         )
         self.parser.add_argument(
             "-v",
             "--verbose",
             "--debug",
             help="Display more information on events and errors",
@@ -112,23 +112,25 @@
 
         # Setup workdir either in Ponos environment or on host's home
         if os.environ.get("PONOS_DATA"):
             self.work_dir = Path(os.environ["PONOS_DATA"], "current")
         else:
             # We use the official XDG convention to store file for developers
             # https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html
-            xdg_data_home = os.environ.get(
-                "XDG_DATA_HOME", os.path.expanduser("~/.local/share")
-            )
-            self.work_dir = Path(xdg_data_home, "arkindex")
+            xdg_data_home = os.environ.get("XDG_DATA_HOME", "~/.local/share")
+            self.work_dir = Path(xdg_data_home, "arkindex").expanduser()
             self.work_dir.mkdir(parents=True, exist_ok=True)
 
-        # Store task ID. This is only available when running in production
+        # Store task ID and chunk index. This is only available when running in production
         # through a ponos agent
         self.task_id = os.environ.get("PONOS_TASK")
+        self.task_chunk = os.environ.get("ARKINDEX_TASK_CHUNK")
+
+        # Store task data directory.
+        self.task_data_dir = Path(os.environ.get("PONOS_DATA", "/data"))
 
         self.worker_run_id = os.environ.get("ARKINDEX_WORKER_RUN_ID")
         if not self.worker_run_id:
             logger.warning(
                 "Missing ARKINDEX_WORKER_RUN_ID environment variable, worker is in read-only mode"
             )
 
@@ -141,14 +143,18 @@
         self.user_configuration = {}
         self.model_configuration = {}
         self.support_cache = support_cache
         # use_cache will be updated in configure() if the cache is supported and if there
         # is at least one available sqlite database either given or in the parent tasks
         self.use_cache = False
 
+        # task_parents will be updated in configure() if the cache is supported and if there
+        # is at least one available sqlite database either given or in the parent tasks
+        self.task_parents = []
+
         # Define API Client
         self.setup_api_client()
 
     @property
     def is_read_only(self) -> bool:
         """
         Whether or not the worker can publish data.
@@ -198,15 +204,15 @@
                 "'ARKINDEX_CORPUS_ID' was not set in the environment. Any API request involving a `corpus_id` will fail."
             )
 
         # Define model_version_id from environment
         self.model_version_id = os.environ.get("ARKINDEX_MODEL_VERSION_ID")
 
         # Load all required secrets
-        self.secrets = {name: self.load_secret(name) for name in required_secrets}
+        self.secrets = {name: self.load_secret(Path(name)) for name in required_secrets}
 
     def configure(self):
         """
         Setup the necessary configuration needed using CLI args and environment variables.
         This is the method called when running a worker on Arkindex.
         """
         assert not self.is_read_only
@@ -274,34 +280,32 @@
         Setup the necessary attribute when using the cache system of `Base-Worker`.
         """
         paths = None
         if self.support_cache and self.args.database is not None:
             self.use_cache = True
         elif self.support_cache and self.task_id:
             task = self.request("RetrieveTaskFromAgent", id=self.task_id)
+            self.task_parents = task["parents"]
             paths = retrieve_parents_cache_path(
-                task["parents"],
-                data_dir=os.environ.get("PONOS_DATA", "/data"),
-                chunk=os.environ.get("ARKINDEX_TASK_CHUNK"),
+                self.task_parents,
+                data_dir=self.task_data_dir,
+                chunk=self.task_chunk,
             )
             self.use_cache = len(paths) > 0
 
         if self.use_cache:
             if self.args.database is not None:
-                assert os.path.isfile(
-                    self.args.database
+                assert (
+                    self.args.database.is_file()
                 ), f"Database in {self.args.database} does not exist"
                 self.cache_path = self.args.database
             else:
-                cache_dir = os.path.join(
-                    os.environ.get("PONOS_DATA", "/data"), self.task_id
-                )
-                assert os.path.isdir(cache_dir), f"Missing task cache in {cache_dir}"
-                self.cache_path = os.path.join(cache_dir, "db.sqlite")
-
+                cache_dir = self.task_data_dir / self.task_id
+                assert cache_dir.is_dir(), f"Missing task cache in {cache_dir}"
+                self.cache_path = cache_dir / "db.sqlite"
             init_cache_db(self.cache_path)
 
             if self.args.database is not None:
                 check_version(self.cache_path)
             else:
                 create_version_table()
 
@@ -309,26 +313,26 @@
 
             # Merging parents caches (if there are any) in the current task local cache, unless the database got overridden
             if self.args.database is None and paths is not None:
                 merge_parents_cache(paths, self.cache_path)
         else:
             logger.debug("Cache is disabled")
 
-    def load_secret(self, name: str):
+    def load_secret(self, name: Path):
         """
         Load a Ponos secret by name.
 
         :param name: Name of the Ponos secret.
         :raises Exception: When the secret cannot be loaded from the API nor the local secrets directory.
         """
         secret = None
 
         # Load from the backend
         try:
-            resp = self.request("RetrieveSecret", name=name)
+            resp = self.request("RetrieveSecret", name=str(name))
             secret = resp["content"]
             logging.info(f"Loaded API secret {name}")
         except ErrorResponse as e:
             logger.warning(f"Secret {name} not available: {e.content}")
 
         # Load from local developer storage
         base_dir = Path(os.environ.get("XDG_CONFIG_HOME") or "~/.config").expanduser()
@@ -347,17 +351,16 @@
             except Exception as e:
                 logger.error(f"Local secret {name} is not available as {path}: {e}")
 
         if secret is None:
             raise Exception(f"Secret {name} is not available on the API nor locally")
 
         # Parse secret payload, according to its extension
-        _, ext = os.path.splitext(os.path.basename(name))
         try:
-            ext = ext.lower()
+            ext = name.suffix.lower()
             if ext == ".json":
                 return json.loads(secret)
             elif ext in (".yaml", ".yml"):
                 return yaml.safe_load(secret)
         except Exception as e:
             logger.error(f"Failed to parse secret {name}: {e}")
```

### Comparing `arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/classification.py` & `arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/classification.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/element.py` & `arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/element.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/entity.py` & `arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/entity.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/metadata.py` & `arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/metadata.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/training.py` & `arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/training.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 # -*- coding: utf-8 -*-
 """
 BaseWorker methods for training.
 """
 
 import functools
-import hashlib
-import os
-import tarfile
-import tempfile
 from contextlib import contextmanager
 from pathlib import Path
 from typing import NewType, Optional, Tuple, Union
 from uuid import UUID
 
 import requests
-import zstandard as zstd
 from apistar.exceptions import ErrorResponse
 
 from arkindex_worker import logger
+from arkindex_worker.utils import close_delete_file, create_tar_archive, zstd_compress
 
-CHUNK_SIZE = 1024
-
-DirPath = NewType("DirPath", str)
+DirPath = NewType("DirPath", Path)
 """Path to a directory"""
 
 Hash = NewType("Hash", str)
 """MD5 Hash"""
 
 FileSize = NewType("FileSize", int)
 """File size"""
@@ -39,62 +33,27 @@
     Yield its location, its hash, its size and its content's hash.
 
     :param path: Create a compressed tar archive from the files
     :returns: The location of the created archive, its hash, its size and its content's hash
     """
     assert path.is_dir(), "create_archive needs a directory"
 
-    compressor = zstd.ZstdCompressor(level=3)
-    content_hasher = hashlib.md5()
-    archive_hasher = hashlib.md5()
-
-    # Remove extension from the model filename
-    _, path_to_tar_archive = tempfile.mkstemp(prefix="teklia-", suffix=".tar")
-
-    # Create an uncompressed tar archive with all the needed files
-    # Files hierarchy ifs kept in the archive.
-    file_list = []
-    with tarfile.open(path_to_tar_archive, "w") as tar:
-        for p in path.glob("**/*"):
-            x = p.relative_to(path)
-            tar.add(p, arcname=x, recursive=False)
-            # Only keep files when computing the hash
-            if p.is_file():
-                file_list.append(p)
-
-    # Sort by path
-    file_list.sort()
-    # Compute hash of the files
-    for file_path in file_list:
-        with open(file_path, "rb") as file_data:
-            for chunk in iter(lambda: file_data.read(CHUNK_SIZE), b""):
-                content_hasher.update(chunk)
-
-    _, path_to_zst_archive = tempfile.mkstemp(prefix="teklia-", suffix=".tar.zst")
+    tar_descriptor, tar_archive, content_hash = create_tar_archive(path)
 
     # Compress the archive
-    with open(path_to_zst_archive, "wb") as archive_file:
-        with open(path_to_tar_archive, "rb") as model_data:
-            for model_chunk in iter(lambda: model_data.read(CHUNK_SIZE), b""):
-                compressed_chunk = compressor.compress(model_chunk)
-                archive_hasher.update(compressed_chunk)
-                archive_file.write(compressed_chunk)
+    zstd_descriptor, zstd_archive, archive_hash = zstd_compress(tar_archive)
 
     # Remove the tar archive
-    os.remove(path_to_tar_archive)
+    close_delete_file(tar_descriptor, tar_archive)
 
     # Get content hash, archive size and hash
-    hash = content_hasher.hexdigest()
-    size = os.path.getsize(path_to_zst_archive)
-    archive_hash = archive_hasher.hexdigest()
-
-    yield path_to_zst_archive, hash, size, archive_hash
+    yield zstd_archive, content_hash, zstd_archive.stat().st_size, archive_hash
 
     # Remove the zstd archive
-    os.remove(path_to_zst_archive)
+    close_delete_file(zstd_descriptor, zstd_archive)
 
 
 def build_clean_payload(**kwargs):
     """
     Remove null attributes from an API body payload
     """
     return {key: value for key, value in kwargs.items() if value is not None}
@@ -263,15 +222,15 @@
             ),
         )
         logger.info(
             f"Model version ({self.model_version['id']}) was successfully updated"
         )
 
     @skip_if_read_only
-    def upload_to_s3(self, archive_path: str) -> None:
+    def upload_to_s3(self, archive_path: Path) -> None:
         """
         Upload the archive of the model's files to an Amazon s3 compatible storage
         """
 
         assert (
             self.model_version
         ), "You must create the model version before uploading an archive."
@@ -282,15 +241,15 @@
         s3_put_url = self.model_version.get("s3_put_url")
         assert (
             s3_put_url
         ), "S3 PUT URL is not set, please ensure you have the right to validate a model version."
 
         logger.info("Uploading to s3...")
         # Upload the archive on s3
-        with open(archive_path, "rb") as archive:
+        with archive_path.open("rb") as archive:
             r = requests.put(
                 url=s3_put_url,
                 data=archive,
                 headers={"Content-Type": "application/zstd"},
             )
         r.raise_for_status()
```

### Comparing `arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/transcription.py` & `arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/transcription.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/version.py` & `arkindex-base-worker-0.3.3rc2/arkindex_worker/worker/version.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc1/setup.py` & `arkindex-base-worker-0.3.3rc2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-import os.path
+from pathlib import Path
 
 from setuptools import find_packages, setup
 
 
-def requirements(path):
-    assert os.path.exists(path), "Missing requirements {}".format(path)
-    with open(path) as f:
+def requirements(path: Path):
+    assert path.exists(), "Missing requirements {}".format(path)
+    with path.open() as f:
         return list(map(str.strip, f.read().splitlines()))
 
 
 with open("VERSION") as f:
     VERSION = f.read()
 
-install_requires = requirements("requirements.txt")
-
 setup(
     name="arkindex-base-worker",
     version=VERSION,
     description="Base Worker to easily build Arkindex ML workflows",
     author="Teklia",
     author_email="contact@teklia.com",
     url="https://teklia.com",
     python_requires=">=3.7",
-    install_requires=install_requires,
-    extras_require={"docs": requirements("docs-requirements.txt")},
+    install_requires=requirements(Path("requirements.txt")),
+    extras_require={"docs": requirements(Path("docs-requirements.txt"))},
     packages=find_packages(),
 )
```

### Comparing `arkindex-base-worker-0.3.3rc1/tests/conftest.py` & `arkindex-base-worker-0.3.3rc2/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -431,26 +431,26 @@
         confidence=0.42,
         orientation=TextOrientation.HorizontalLeftToRight,
         worker_version_id=None,
     )
 
 
 @pytest.fixture(scope="function")
-def mock_databases(tmpdir):
+def mock_databases(tmp_path):
     """
     Initialize several temporary databases
     to help testing the merge algorithm
     """
     out = {}
     for name in ("target", "first", "second", "conflict", "chunk_42"):
         # Build a local database in sub directory
         # for each name required
         filename = "db_42.sqlite" if name == "chunk_42" else "db.sqlite"
-        path = tmpdir / name / filename
-        (tmpdir / name).mkdir()
+        path = tmp_path / name / filename
+        (tmp_path / name).mkdir()
         local_db = SqliteDatabase(path)
         with local_db.bind_ctx(MODELS + [Version]):
             # Create tables on the current local database
             # by binding temporarily the models on that database
             local_db.create_tables([Version])
             Version.create(version=SQL_VERSION)
             local_db.create_tables(MODELS)
```

### Comparing `arkindex-base-worker-0.3.3rc1/tests/test_base_worker.py` & `arkindex-base-worker-0.3.3rc2/tests/test_base_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # -*- coding: utf-8 -*-
 import json
 import logging
-import os
 import sys
 from pathlib import Path
 
 import gnupg
 import pytest
 
 from arkindex.mock import MockApiClient
@@ -13,29 +12,29 @@
 from arkindex_worker.worker import BaseWorker
 from arkindex_worker.worker.base import ModelNotFoundError
 
 
 def test_init_default_local_share(monkeypatch):
     worker = BaseWorker()
 
-    assert str(worker.work_dir) == os.path.expanduser("~/.local/share/arkindex")
+    assert worker.work_dir == Path("~/.local/share/arkindex").expanduser()
 
 
 def test_init_default_xdg_data_home(monkeypatch):
     path = str(Path(__file__).absolute().parent)
     monkeypatch.setenv("XDG_DATA_HOME", path)
     worker = BaseWorker()
 
     assert str(worker.work_dir) == f"{path}/arkindex"
 
 
 def test_init_with_local_cache(monkeypatch):
     worker = BaseWorker(support_cache=True)
 
-    assert str(worker.work_dir) == os.path.expanduser("~/.local/share/arkindex")
+    assert worker.work_dir == Path("~/.local/share/arkindex").expanduser()
     assert worker.support_cache is True
 
 
 def test_init_var_ponos_data_given(monkeypatch):
     path = str(Path(__file__).absolute().parent)
     monkeypatch.setenv("PONOS_DATA", path)
     worker = BaseWorker()
@@ -500,27 +499,27 @@
 def test_load_missing_secret():
     worker = BaseWorker()
     worker.api_client = MockApiClient()
 
     with pytest.raises(
         Exception, match="Secret missing/secret is not available on the API nor locally"
     ):
-        worker.load_secret("missing/secret")
+        worker.load_secret(Path("missing/secret"))
 
 
 def test_load_remote_secret():
     worker = BaseWorker()
     worker.api_client = MockApiClient()
     worker.api_client.add_response(
         "RetrieveSecret",
         name="testRemote",
         response={"content": "this is a secret value !"},
     )
 
-    assert worker.load_secret("testRemote") == "this is a secret value !"
+    assert worker.load_secret(Path("testRemote")) == "this is a secret value !"
 
     # The one mocked call has been used
     assert len(worker.api_client.history) == 1
     assert len(worker.api_client.responses) == 0
 
 
 def test_load_json_secret():
@@ -528,15 +527,15 @@
     worker.api_client = MockApiClient()
     worker.api_client.add_response(
         "RetrieveSecret",
         name="path/to/file.json",
         response={"content": '{"key": "value", "number": 42}'},
     )
 
-    assert worker.load_secret("path/to/file.json") == {
+    assert worker.load_secret(Path("path/to/file.json")) == {
         "key": "value",
         "number": 42,
     }
 
     # The one mocked call has been used
     assert len(worker.api_client.history) == 1
     assert len(worker.api_client.responses) == 0
@@ -558,47 +557,47 @@
 struct:
  level:
    X
 """
         },
     )
 
-    assert worker.load_secret("path/to/file.yaml") == {
+    assert worker.load_secret(Path("path/to/file.yaml")) == {
         "aList": ["A", "B", "C"],
         "somekey": "value",
         "struct": {"level": "X"},
     }
 
     # The one mocked call has been used
     assert len(worker.api_client.history) == 1
     assert len(worker.api_client.responses) == 0
 
 
-def test_load_local_secret(monkeypatch, tmpdir):
+def test_load_local_secret(monkeypatch, tmp_path):
     # Setup arkindex config dir in a temp directory
-    monkeypatch.setenv("XDG_CONFIG_HOME", str(tmpdir))
+    monkeypatch.setenv("XDG_CONFIG_HOME", str(tmp_path))
 
     # Write a dummy secret
-    secrets_dir = tmpdir / "arkindex" / "secrets"
-    os.makedirs(secrets_dir)
+    secrets_dir = tmp_path / "arkindex" / "secrets"
+    secrets_dir.mkdir(parents=True)
     secret = secrets_dir / "testLocal"
     secret.write_text("this is a local secret value", encoding="utf-8")
 
     # Mock GPG decryption
     class GpgDecrypt(object):
         def __init__(self, fd):
             self.ok = True
             self.data = fd.read()
 
     monkeypatch.setattr(gnupg.GPG, "decrypt_file", lambda gpg, f: GpgDecrypt(f))
 
     worker = BaseWorker()
     worker.api_client = MockApiClient()
 
-    assert worker.load_secret("testLocal") == "this is a local secret value"
+    assert worker.load_secret(Path("testLocal")) == "this is a local secret value"
 
     # The remote api is checked first
     assert len(worker.api_client.history) == 1
     assert worker.api_client.history[0].operation == "RetrieveSecret"
 
 
 def test_find_model_directory_ponos(monkeypatch):
```

### Comparing `arkindex-base-worker-0.3.3rc1/tests/test_cache.py` & `arkindex-base-worker-0.3.3rc2/tests/test_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-import os
+from pathlib import Path
 from uuid import UUID
 
 import pytest
 from peewee import OperationalError
 
 from arkindex_worker.cache import (
     SQL_VERSION,
@@ -22,18 +22,18 @@
     with pytest.raises(OperationalError) as e:
         init_cache_db("path/not/found.sqlite")
 
     assert str(e.value) == "unable to open database file"
 
 
 def test_init(tmp_path):
-    db_path = f"{tmp_path}/db.sqlite"
+    db_path = Path(f"{tmp_path}/db.sqlite")
     init_cache_db(db_path)
 
-    assert os.path.isfile(db_path)
+    assert db_path.is_file()
 
 
 def test_create_tables_existing_table(tmp_path):
     db_path = f"{tmp_path}/db.sqlite"
 
     # Create the tables once…
     init_cache_db(db_path)
@@ -59,15 +59,15 @@
     create_tables()
 
     expected_schema = """CREATE TABLE "classifications" ("id" TEXT NOT NULL PRIMARY KEY, "element_id" TEXT NOT NULL, "class_name" TEXT NOT NULL, "confidence" REAL NOT NULL, "state" VARCHAR(10) NOT NULL, "worker_run_id" TEXT, FOREIGN KEY ("element_id") REFERENCES "elements" ("id"))
 CREATE TABLE "elements" ("id" TEXT NOT NULL PRIMARY KEY, "parent_id" TEXT, "type" VARCHAR(50) NOT NULL, "image_id" TEXT, "polygon" text, "rotation_angle" INTEGER NOT NULL, "mirrored" INTEGER NOT NULL, "initial" INTEGER NOT NULL, "worker_version_id" TEXT, "worker_run_id" TEXT, "confidence" REAL, FOREIGN KEY ("image_id") REFERENCES "images" ("id"))
 CREATE TABLE "entities" ("id" TEXT NOT NULL PRIMARY KEY, "type" VARCHAR(50) NOT NULL, "name" TEXT NOT NULL, "validated" INTEGER NOT NULL, "metas" text, "worker_run_id" TEXT)
 CREATE TABLE "images" ("id" TEXT NOT NULL PRIMARY KEY, "width" INTEGER NOT NULL, "height" INTEGER NOT NULL, "url" TEXT NOT NULL)
 CREATE TABLE "transcription_entities" ("transcription_id" TEXT NOT NULL, "entity_id" TEXT NOT NULL, "offset" INTEGER NOT NULL CHECK (offset >= 0), "length" INTEGER NOT NULL CHECK (length > 0), "worker_run_id" TEXT, "confidence" REAL, PRIMARY KEY ("transcription_id", "entity_id"), FOREIGN KEY ("transcription_id") REFERENCES "transcriptions" ("id"), FOREIGN KEY ("entity_id") REFERENCES "entities" ("id"))
-CREATE TABLE "transcriptions" ("id" TEXT NOT NULL PRIMARY KEY, "element_id" TEXT NOT NULL, "text" TEXT NOT NULL, "confidence" REAL NOT NULL, "orientation" VARCHAR(50) NOT NULL, "worker_version_id" TEXT, "worker_run_id" TEXT, FOREIGN KEY ("element_id") REFERENCES "elements" ("id"))"""
+CREATE TABLE "transcriptions" ("id" TEXT NOT NULL PRIMARY KEY, "element_id" TEXT NOT NULL, "text" TEXT NOT NULL, "confidence" REAL, "orientation" VARCHAR(50) NOT NULL, "worker_version_id" TEXT, "worker_run_id" TEXT, FOREIGN KEY ("element_id") REFERENCES "elements" ("id"))"""
 
     actual_schema = "\n".join(
         [
             row[0]
             for row in db.connection()
             .execute("SELECT sql FROM sqlite_master WHERE type = 'table' ORDER BY name")
             .fetchall()
```

### Comparing `arkindex-base-worker-0.3.3rc1/tests/test_element.py` & `arkindex-base-worker-0.3.3rc2/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_classifications.py` & `arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_classifications.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_cli.py` & `arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_cli.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_elements.py` & `arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,39 +228,39 @@
 
     mocker.patch(
         "arkindex_worker.worker.base.argparse.ArgumentParser.parse_args",
         return_value=Namespace(
             element=["volumeid", "pageid"],
             verbose=False,
             elements_list=None,
-            database=str(database_path),
+            database=database_path,
             dev=False,
         ),
     )
 
     worker = ElementsWorker(support_cache=True)
     worker.configure()
 
     assert worker.use_cache is True
-    assert worker.cache_path == str(database_path)
+    assert worker.cache_path == database_path
 
 
 def test_database_arg_cache_missing_version_table(
     mocker, mock_elements_worker, tmp_path
 ):
     database_path = tmp_path / "my_database.sqlite"
     database_path.touch()
 
     mocker.patch(
         "arkindex_worker.worker.base.argparse.ArgumentParser.parse_args",
         return_value=Namespace(
             element=["volumeid", "pageid"],
             verbose=False,
             elements_list=None,
-            database=str(database_path),
+            database=database_path,
             dev=False,
         ),
     )
 
     worker = ElementsWorker(support_cache=True)
     with pytest.raises(AssertionError) as e:
         worker.configure()
```

### Comparing `arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_entities.py` & `arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_entities.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_metadata.py` & `arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_metadata.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_training.py` & `arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 import logging
-import os
 import sys
 
 import pytest
 import responses
 
 from arkindex.mock import MockApiClient
 from arkindex_worker.worker import BaseWorker
@@ -49,39 +48,39 @@
 
     with create_archive(path=model_file_dir) as (
         zst_archive_path,
         hash,
         size,
         archive_hash,
     ):
-        assert os.path.exists(zst_archive_path), "The archive was not created"
+        assert zst_archive_path.exists(), "The archive was not created"
         assert (
             hash == "c5aedde18a768757351068b840c8c8f9"
         ), "Hash was not properly computed"
         assert 300 < size < 700
 
-    assert not os.path.exists(zst_archive_path), "Auto removal failed"
+    assert not zst_archive_path.exists(), "Auto removal failed"
 
 
 def test_create_archive_with_subfolder(model_file_dir_with_subfolder):
     """Create an archive when the model's file is in a folder containing a subfolder"""
 
     with create_archive(path=model_file_dir_with_subfolder) as (
         zst_archive_path,
         hash,
         size,
         archive_hash,
     ):
-        assert os.path.exists(zst_archive_path), "The archive was not created"
+        assert zst_archive_path.exists(), "The archive was not created"
         assert (
             hash == "3e453881404689e6e125144d2db3e605"
         ), "Hash was not properly computed"
         assert 300 < size < 1500
 
-    assert not os.path.exists(zst_archive_path), "Auto removal failed"
+    assert not zst_archive_path.exists(), "Auto removal failed"
 
 
 def test_handle_s3_uploading_errors(mock_training_worker, model_file_dir):
     s3_endpoint_url = "http://s3.localhost.com"
     responses.add_passthru(s3_endpoint_url)
     responses.add(responses.Response(method="PUT", url=s3_endpoint_url, status=400))
     file_path = model_file_dir / "model_file.pth"
```

### Comparing `arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_transcriptions.py` & `arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_transcriptions.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_worker.py` & `arkindex-base-worker-0.3.3rc2/tests/test_elements_worker/test_worker.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc1/tests/test_git.py` & `arkindex-base-worker-0.3.3rc2/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.3rc1/tests/test_image.py` & `arkindex-base-worker-0.3.3rc2/tests/test_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,20 +126,19 @@
         ("path/to/something", True),
         ("/absolute/path/to/something", True),
     ),
 )
 def test_open_image(path, is_local, monkeypatch):
     """Check if the path triggers a local load or a remote one"""
 
-    monkeypatch.setattr("os.path.exists", lambda x: True)
+    monkeypatch.setattr(Path, "exists", lambda x: True)
     monkeypatch.setattr(Image, "open", lambda x: Image.new("RGB", (1, 10)))
     monkeypatch.setattr(
         "arkindex_worker.image.download_image", lambda x: Image.new("RGB", (10, 1))
     )
-
     image = open_image(path)
 
     if is_local:
         assert image.size == (1, 10)
     else:
         assert image.size == (10, 1)
```

### Comparing `arkindex-base-worker-0.3.3rc1/tests/test_merge.py` & `arkindex-base-worker-0.3.3rc2/tests/test_merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,29 +73,29 @@
                 UUID("11111111-1111-1111-1111-111111111111"),
                 UUID("22222222-2222-2222-2222-222222222222"),
             ],
         ),
     ),
 )
 def test_merge_databases(
-    mock_databases, tmpdir, parents, expected_elements, expected_transcriptions
+    mock_databases, tmp_path, parents, expected_elements, expected_transcriptions
 ):
     """Test multiple database merge scenarios"""
 
     # We always start with an empty database
     with mock_databases["target"]["db"].bind_ctx(MODELS):
         assert CachedImage.select().count() == 0
         assert CachedElement.select().count() == 0
         assert CachedTranscription.select().count() == 0
         assert CachedClassification.select().count() == 0
         assert CachedEntity.select().count() == 0
         assert CachedTranscriptionEntity.select().count() == 0
 
     # Retrieve parents databases paths
-    paths = retrieve_parents_cache_path(parents, data_dir=tmpdir)
+    paths = retrieve_parents_cache_path(parents, data_dir=tmp_path)
 
     # Merge all requested parents databases into our target
     merge_parents_cache(paths, mock_databases["target"]["path"])
 
     # The target now should have the expected elements and transcriptions
     with mock_databases["target"]["db"].bind_ctx(MODELS):
         assert CachedImage.select().count() == 0
@@ -108,38 +108,38 @@
             e.id for e in CachedElement.select().order_by("id")
         ] == expected_elements
         assert [
             t.id for t in CachedTranscription.select().order_by("id")
         ] == expected_transcriptions
 
 
-def test_merge_chunk(mock_databases, tmpdir, monkeypatch):
+def test_merge_chunk(mock_databases, tmp_path, monkeypatch):
     """
     Check the db merge algorithm support two parents
     and one of them has a chunk
     """
     # At first we have nothing in target
     with mock_databases["target"]["db"].bind_ctx(MODELS):
         assert CachedImage.select().count() == 0
         assert CachedElement.select().count() == 0
         assert CachedTranscription.select().count() == 0
         assert CachedClassification.select().count() == 0
         assert CachedEntity.select().count() == 0
         assert CachedTranscriptionEntity.select().count() == 0
 
     # Check filenames
-    assert mock_databases["chunk_42"]["path"].basename == "db_42.sqlite"
-    assert mock_databases["second"]["path"].basename == "db.sqlite"
+    assert mock_databases["chunk_42"]["path"].name == "db_42.sqlite"
+    assert mock_databases["second"]["path"].name == "db.sqlite"
 
     paths = retrieve_parents_cache_path(
         [
             "chunk_42",
             "first",
         ],
-        data_dir=tmpdir,
+        data_dir=tmp_path,
         chunk="42",
     )
     merge_parents_cache(paths, mock_databases["target"]["path"])
 
     # The target should now have 3 elements and 0 transcription
     with mock_databases["target"]["db"].bind_ctx(MODELS):
         assert CachedImage.select().count() == 0
@@ -152,42 +152,46 @@
             UUID("42424242-4242-4242-4242-424242424242"),
             UUID("12341234-1234-1234-1234-123412341234"),
             UUID("56785678-5678-5678-5678-567856785678"),
         ]
 
 
 def test_merge_from_worker(
-    responses, mock_base_worker_with_cache, mock_databases, tmpdir, monkeypatch
+    responses, mock_base_worker_with_cache, mock_databases, tmp_path, monkeypatch
 ):
     """
     High level merge from the base worker
     """
     responses.add(
         responses.GET,
         "http://testserver/api/v1/task/my_task/from-agent/",
         status=200,
         json={"parents": ["first", "second"]},
     )
-
     # At first we have nothing in target
     with mock_databases["target"]["db"].bind_ctx(MODELS):
         assert CachedImage.select().count() == 0
         assert CachedElement.select().count() == 0
         assert CachedTranscription.select().count() == 0
         assert CachedClassification.select().count() == 0
         assert CachedEntity.select().count() == 0
         assert CachedTranscriptionEntity.select().count() == 0
 
     # Configure worker with a specific data directory
-    monkeypatch.setenv("PONOS_DATA", str(tmpdir))
+    mock_base_worker_with_cache.task_data_dir = tmp_path
+
     # Create the task's output dir, so that it can create its own database
-    (tmpdir / "my_task").mkdir()
+    (tmp_path / "my_task").mkdir()
     mock_base_worker_with_cache.args = mock_base_worker_with_cache.parser.parse_args()
     mock_base_worker_with_cache.configure()
     mock_base_worker_with_cache.configure_cache()
+    # Store parent tasks IDs as attribute
+    assert mock_base_worker_with_cache.task_parents == ["first", "second"]
+
+    assert mock_base_worker_with_cache.use_cache
 
     # Then we have 2 elements and a transcription
     assert CachedImage.select().count() == 0
     assert CachedElement.select().count() == 3
     assert CachedTranscription.select().count() == 1
     assert CachedClassification.select().count() == 0
     assert CachedEntity.select().count() == 0
@@ -198,30 +202,30 @@
         UUID("42424242-4242-4242-4242-424242424242"),
     ]
     assert [t.id for t in CachedTranscription.select().order_by("id")] == [
         UUID("11111111-1111-1111-1111-111111111111"),
     ]
 
 
-def test_merge_conflicting_versions(mock_databases, tmpdir):
+def test_merge_conflicting_versions(mock_databases, tmp_path):
     """
     Merging databases with differing versions should not be allowed
     """
 
     with mock_databases["second"]["db"].bind_ctx([Version]):
         assert Version.get() == Version(version=SQL_VERSION)
         fake_version = 420
         Version.update(version=fake_version).execute()
         assert Version.get() == Version(version=fake_version)
 
     with mock_databases["target"]["db"].bind_ctx([Version]):
         assert Version.get() == Version(version=SQL_VERSION)
 
     # Retrieve parents databases paths
-    paths = retrieve_parents_cache_path(["first", "second"], data_dir=tmpdir)
+    paths = retrieve_parents_cache_path(["first", "second"], data_dir=tmp_path)
 
     # Merge all requested parents databases into our target, the "second" parent have a differing version
     with pytest.raises(AssertionError) as e:
         merge_parents_cache(paths, mock_databases["target"]["path"])
 
     assert (
         str(e.value)
```

### Comparing `arkindex-base-worker-0.3.3rc1/tests/test_reporting.py` & `arkindex-base-worker-0.3.3rc2/tests/test_reporting.py`

 * *Files identical despite different names*

