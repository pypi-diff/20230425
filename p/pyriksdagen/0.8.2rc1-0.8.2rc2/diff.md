# Comparing `tmp/pyriksdagen-0.8.2rc1.tar.gz` & `tmp/pyriksdagen-0.8.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriksdagen-0.8.2rc1.tar", max compression
+gzip compressed data, was "pyriksdagen-0.8.2rc2.tar", max compression
```

## Comparing `pyriksdagen-0.8.2rc1.tar` & `pyriksdagen-0.8.2rc2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1249 2023-04-24 12:55:27.543987 pyriksdagen-0.8.2rc1/LICENSE
--rw-r--r--   0        0        0     3520 2023-04-24 12:55:27.543987 pyriksdagen-0.8.2rc1/README.md
--rw-r--r--   0        0        0      748 2023-04-24 12:58:08.311789 pyriksdagen-0.8.2rc1/pyproject.toml
--rw-r--r--   0        0        0     1107 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/LICENSE
--rw-r--r--   0        0        0       84 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/__init__.py
--rw-r--r--   0        0        0      225 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/alias.rq
--rw-r--r--   0        0        0      494 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/government.rq
--rw-r--r--   0        0        0      729 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/member_of_parliament.rq
--rw-r--r--   0        0        0      148 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/member_of_parliament.txt
--rw-r--r--   0        0        0     1380 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/minister.rq
--rw-r--r--   0        0        0      235 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/minister.txt
--rw-r--r--   0        0        0      262 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/name_location_specifier.rq
--rw-r--r--   0        0        0      484 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/party_affiliation.rq
--rw-r--r--   0        0        0      549 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/person.rq
--rw-r--r--   0        0        0      616 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/speaker.rq
--rw-r--r--   0        0        0      253 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/speaker.txt
--rw-r--r--   0        0        0      208 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/twitter.rq
--rw-r--r--   0        0        0      225 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/alias.rq
--rw-r--r--   0        0        0      482 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/government.rq
--rw-r--r--   0        0        0      722 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/member_of_parliament.rq
--rw-r--r--   0        0        0     1380 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/minister.rq
--rw-r--r--   0        0        0     1013 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/name_location_specifier.rq
--rw-r--r--   0        0        0     1230 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/party_affiliation.rq
--rw-r--r--   0        0        0     1412 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/person.rq
--rw-r--r--   0        0        0      616 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/speaker.rq
--rw-r--r--   0        0        0      959 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/twitter.rq
--rw-r--r--   0        0        0     2195 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/dataset.py
--rw-r--r--   0        0        0     6193 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/db.py
--rw-r--r--   0        0        0     9747 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/download.py
--rw-r--r--   0        0        0     6813 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/export.py
--rw-r--r--   0        0        0     4532 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/match_mp.py
--rw-r--r--   0        0        0     6915 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/metadata.py
--rw-r--r--   0        0        0    11120 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/mp.py
--rw-r--r--   0        0        0    16044 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/refine.py
--rwxr-xr-x   0        0        0      237 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/requirements.txt
--rw-r--r--   0        0        0     7053 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/segmentation.py
--rw-r--r--   0        0        0     5497 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/utils.py
--rw-r--r--   0        0        0     5265 2023-04-24 12:56:20.603911 pyriksdagen-0.8.2rc1/pyriksdagen/wikidata.py
--rw-r--r--   0        0        0     4647 1970-01-01 00:00:00.000000 pyriksdagen-0.8.2rc1/PKG-INFO
+-rw-r--r--   0        0        0     1249 2023-04-25 08:33:14.394206 pyriksdagen-0.8.2rc2/LICENSE
+-rw-r--r--   0        0        0     3520 2023-04-25 08:33:14.394206 pyriksdagen-0.8.2rc2/README.md
+-rw-r--r--   0        0        0      748 2023-04-25 08:36:02.272848 pyriksdagen-0.8.2rc2/pyproject.toml
+-rw-r--r--   0        0        0     1107 2023-04-25 08:34:02.550968 pyriksdagen-0.8.2rc2/pyriksdagen/LICENSE
+-rw-r--r--   0        0        0       84 2023-04-25 08:34:02.550968 pyriksdagen-0.8.2rc2/pyriksdagen/__init__.py
+-rw-r--r--   0        0        0      225 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries/alias.rq
+-rw-r--r--   0        0        0      494 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries/government.rq
+-rw-r--r--   0        0        0      729 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries/member_of_parliament.rq
+-rw-r--r--   0        0        0      148 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries/member_of_parliament.txt
+-rw-r--r--   0        0        0     1380 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries/minister.rq
+-rw-r--r--   0        0        0      235 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries/minister.txt
+-rw-r--r--   0        0        0      262 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries/name_location_specifier.rq
+-rw-r--r--   0        0        0      484 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries/party_affiliation.rq
+-rw-r--r--   0        0        0      549 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries/person.rq
+-rw-r--r--   0        0        0      616 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries/speaker.rq
+-rw-r--r--   0        0        0      253 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries/speaker.txt
+-rw-r--r--   0        0        0      208 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries/twitter.rq
+-rw-r--r--   0        0        0      225 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries_backup/alias.rq
+-rw-r--r--   0        0        0      482 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries_backup/government.rq
+-rw-r--r--   0        0        0      722 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries_backup/member_of_parliament.rq
+-rw-r--r--   0        0        0     1380 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries_backup/minister.rq
+-rw-r--r--   0        0        0     1013 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries_backup/name_location_specifier.rq
+-rw-r--r--   0        0        0     1230 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries_backup/party_affiliation.rq
+-rw-r--r--   0        0        0     1412 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries_backup/person.rq
+-rw-r--r--   0        0        0      616 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries_backup/speaker.rq
+-rw-r--r--   0        0        0      959 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/data/queries_backup/twitter.rq
+-rw-r--r--   0        0        0     2195 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/dataset.py
+-rw-r--r--   0        0        0     6193 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/db.py
+-rw-r--r--   0        0        0     9747 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/download.py
+-rw-r--r--   0        0        0     6813 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/export.py
+-rw-r--r--   0        0        0     4532 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/match_mp.py
+-rw-r--r--   0        0        0     6915 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/metadata.py
+-rw-r--r--   0        0        0    11120 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/mp.py
+-rw-r--r--   0        0        0    16044 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/refine.py
+-rwxr-xr-x   0        0        0      237 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/requirements.txt
+-rw-r--r--   0        0        0     7053 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/segmentation.py
+-rw-r--r--   0        0        0     5497 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/utils.py
+-rw-r--r--   0        0        0     5265 2023-04-25 08:34:02.554968 pyriksdagen-0.8.2rc2/pyriksdagen/wikidata.py
+-rw-r--r--   0        0        0     4647 1970-01-01 00:00:00.000000 pyriksdagen-0.8.2rc2/PKG-INFO
```

### Comparing `pyriksdagen-0.8.2rc1/LICENSE` & `pyriksdagen-0.8.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/README.md` & `pyriksdagen-0.8.2rc2/README.md`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyproject.toml` & `pyriksdagen-0.8.2rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyriksdagen"
-version = "0.8.2rc1"
+version = "0.8.2rc2"
 description = "Access the Riksdagen corpus"
 authors = ["ninpnin <vainoyrjanainen@icloud.com>"]
 repository = "https://github.com/welfare-state-analytics/riksdagen-corpus"
 readme = "README.md"
 license = "MIT"
 packages = [
     { include = "pyriksdagen", from = "" }
```

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/LICENSE` & `pyriksdagen-0.8.2rc2/pyriksdagen/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/member_of_parliament.rq` & `pyriksdagen-0.8.2rc2/pyriksdagen/data/queries/member_of_parliament.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/minister.rq` & `pyriksdagen-0.8.2rc2/pyriksdagen/data/queries/minister.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/person.rq` & `pyriksdagen-0.8.2rc2/pyriksdagen/data/queries/person.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries/speaker.rq` & `pyriksdagen-0.8.2rc2/pyriksdagen/data/queries/speaker.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/member_of_parliament.rq` & `pyriksdagen-0.8.2rc2/pyriksdagen/data/queries_backup/member_of_parliament.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/minister.rq` & `pyriksdagen-0.8.2rc2/pyriksdagen/data/queries_backup/minister.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/name_location_specifier.rq` & `pyriksdagen-0.8.2rc2/pyriksdagen/data/queries_backup/name_location_specifier.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/party_affiliation.rq` & `pyriksdagen-0.8.2rc2/pyriksdagen/data/queries_backup/party_affiliation.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/person.rq` & `pyriksdagen-0.8.2rc2/pyriksdagen/data/queries_backup/person.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/speaker.rq` & `pyriksdagen-0.8.2rc2/pyriksdagen/data/queries_backup/speaker.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/data/queries_backup/twitter.rq` & `pyriksdagen-0.8.2rc2/pyriksdagen/data/queries_backup/twitter.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/dataset.py` & `pyriksdagen-0.8.2rc2/pyriksdagen/dataset.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/db.py` & `pyriksdagen-0.8.2rc2/pyriksdagen/db.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/download.py` & `pyriksdagen-0.8.2rc2/pyriksdagen/download.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/export.py` & `pyriksdagen-0.8.2rc2/pyriksdagen/export.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/match_mp.py` & `pyriksdagen-0.8.2rc2/pyriksdagen/match_mp.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/metadata.py` & `pyriksdagen-0.8.2rc2/pyriksdagen/metadata.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/mp.py` & `pyriksdagen-0.8.2rc2/pyriksdagen/mp.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/refine.py` & `pyriksdagen-0.8.2rc2/pyriksdagen/refine.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/segmentation.py` & `pyriksdagen-0.8.2rc2/pyriksdagen/segmentation.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/utils.py` & `pyriksdagen-0.8.2rc2/pyriksdagen/utils.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/pyriksdagen/wikidata.py` & `pyriksdagen-0.8.2rc2/pyriksdagen/wikidata.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.8.2rc1/PKG-INFO` & `pyriksdagen-0.8.2rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyriksdagen
-Version: 0.8.2rc1
+Version: 0.8.2rc2
 Summary: Access the Riksdagen corpus
 Home-page: https://github.com/welfare-state-analytics/riksdagen-corpus
 License: MIT
 Author: ninpnin
 Author-email: vainoyrjanainen@icloud.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

