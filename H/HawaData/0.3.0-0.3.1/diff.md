# Comparing `tmp/HawaData-0.3.0.tar.gz` & `tmp/HawaData-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.3.0.tar", last modified: Mon Apr 17 08:29:53 2023, max compression
+gzip compressed data, was "HawaData-0.3.1.tar", last modified: Tue Apr 25 10:02:22 2023, max compression
```

## Comparing `HawaData-0.3.0.tar` & `HawaData-0.3.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.557623 HawaData-0.3.0/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.547461 HawaData-0.3.0/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     1964 2023-04-17 08:29:53.000000 HawaData-0.3.0/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      765 2023-04-17 08:29:53.000000 HawaData-0.3.0/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-04-17 08:29:53.000000 HawaData-0.3.0/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)      257 2023-04-17 08:29:53.000000 HawaData-0.3.0/HawaData.egg-info/requires.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)       10 2023-04-17 08:29:53.000000 HawaData-0.3.0/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     1964 2023-04-17 08:29:53.557365 HawaData-0.3.0/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.3.0/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.547853 HawaData-0.3.0/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.3.0/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.549631 HawaData-0.3.0/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.3.0/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2842 2022-12-11 02:48:15.000000 HawaData-0.3.0/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.3.0/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.3.0/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.550923 HawaData-0.3.0/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.3.0/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     8767 2023-04-17 08:29:21.000000 HawaData-0.3.0/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     4455 2023-04-17 08:27:12.000000 HawaData-0.3.0/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2691 2022-12-01 05:37:32.000000 HawaData-0.3.0/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.3.0/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.551828 HawaData-0.3.0/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.3.0/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.3.0/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.3.0/hawa/data/school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.552916 HawaData-0.3.0/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.3.0/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    22989 2023-04-13 07:01:46.000000 HawaData-0.3.0/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5252 2022-12-08 10:47:44.000000 HawaData-0.3.0/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-04-17 08:29:53.557703 HawaData-0.3.0/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      875 2022-12-02 07:10:09.000000 HawaData-0.3.0/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.554271 HawaData-0.3.0/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2022-12-01 08:54:31.000000 HawaData-0.3.0/test/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      654 2022-12-02 04:24:16.000000 HawaData-0.3.0/test/mock.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.554971 HawaData-0.3.0/test/test_common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:19.000000 HawaData-0.3.0/test/test_common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      770 2023-04-13 03:56:08.000000 HawaData-0.3.0/test/test_common/test_common_data.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.555807 HawaData-0.3.0/test/test_data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:40.000000 HawaData-0.3.0/test/test_data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1622 2023-04-17 08:15:54.000000 HawaData-0.3.0/test/test_data/test_school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-17 08:29:53.556750 HawaData-0.3.0/test/test_paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:31.000000 HawaData-0.3.0/test/test_paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      681 2023-03-29 04:15:57.000000 HawaData-0.3.0/test/test_paper/test_health_data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      491 2022-12-02 09:56:11.000000 HawaData-0.3.0/test/test_paper/test_mht_data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.3.0/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.205297 HawaData-0.3.1/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.192860 HawaData-0.3.1/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1996 2023-04-25 10:02:22.000000 HawaData-0.3.1/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      765 2023-04-25 10:02:22.000000 HawaData-0.3.1/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-04-25 10:02:22.000000 HawaData-0.3.1/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)      257 2023-04-25 10:02:22.000000 HawaData-0.3.1/HawaData.egg-info/requires.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)       10 2023-04-25 10:02:22.000000 HawaData-0.3.1/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1996 2023-04-25 10:02:22.205038 HawaData-0.3.1/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.3.1/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.193389 HawaData-0.3.1/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.3.1/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.195282 HawaData-0.3.1/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.3.1/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2842 2022-12-11 02:48:15.000000 HawaData-0.3.1/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.3.1/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.3.1/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.197136 HawaData-0.3.1/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.3.1/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     8767 2023-04-17 08:29:21.000000 HawaData-0.3.1/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5032 2023-04-25 09:59:36.000000 HawaData-0.3.1/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2710 2023-04-25 09:04:45.000000 HawaData-0.3.1/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.3.1/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.198620 HawaData-0.3.1/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.3.1/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.3.1/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.3.1/hawa/data/school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.200247 HawaData-0.3.1/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.3.1/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    22989 2023-04-13 07:01:46.000000 HawaData-0.3.1/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5252 2022-12-08 10:47:44.000000 HawaData-0.3.1/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-04-25 10:02:22.205375 HawaData-0.3.1/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      875 2022-12-02 07:10:09.000000 HawaData-0.3.1/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.201775 HawaData-0.3.1/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2022-12-01 08:54:31.000000 HawaData-0.3.1/test/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      654 2022-12-02 04:24:16.000000 HawaData-0.3.1/test/mock.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.202465 HawaData-0.3.1/test/test_common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:19.000000 HawaData-0.3.1/test/test_common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      770 2023-04-13 03:56:08.000000 HawaData-0.3.1/test/test_common/test_common_data.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.203296 HawaData-0.3.1/test/test_data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:40.000000 HawaData-0.3.1/test/test_data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1622 2023-04-17 08:15:54.000000 HawaData-0.3.1/test/test_data/test_school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-04-25 10:02:22.204477 HawaData-0.3.1/test/test_paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:37:31.000000 HawaData-0.3.1/test/test_paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      681 2023-03-29 04:15:57.000000 HawaData-0.3.1/test/test_paper/test_health_data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      491 2022-12-02 09:56:11.000000 HawaData-0.3.1/test/test_paper/test_mht_data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.3.1/test/test_query.py
```

### Comparing `HawaData-0.3.0/HawaData.egg-info/PKG-INFO` & `HawaData-0.3.1/HawaData.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.3.0
+Version: 0.3.1
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -71,7 +71,8 @@
 - 0.2.4 Filter users when length id <18
 - 0.2.5 Filter users when length id <18 true
 - 0.2.6 Fix rank dis
 - 0.2.7 Fix miss grade
 - 0.2.8 Fix miss grade all
 - 0.2.9 Fix miss grade again
 - 0.3.0 Fix more school when query school
+- 0.3.1 Update replace select *
```

### Comparing `HawaData-0.3.0/HawaData.egg-info/SOURCES.txt` & `HawaData-0.3.1/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.0/PKG-INFO` & `HawaData-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.3.0
+Version: 0.3.1
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -71,7 +71,8 @@
 - 0.2.4 Filter users when length id <18
 - 0.2.5 Filter users when length id <18 true
 - 0.2.6 Fix rank dis
 - 0.2.7 Fix miss grade
 - 0.2.8 Fix miss grade all
 - 0.2.9 Fix miss grade again
 - 0.3.0 Fix more school when query school
+- 0.3.1 Update replace select *
```

### Comparing `HawaData-0.3.0/README.md` & `HawaData-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.0/hawa/base/db.py` & `HawaData-0.3.1/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.0/hawa/base/init.py` & `HawaData-0.3.1/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.0/hawa/common/data.py` & `HawaData-0.3.1/hawa/common/data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.0/hawa/common/query.py` & `HawaData-0.3.1/hawa/common/query.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from collections import namedtuple
 
 import pandas as pd
-from loguru import logger
 
 from hawa.base.db import DbUtil
 from hawa.base.decos import singleton
 
 
 @singleton
 class DataQuery:
@@ -23,37 +22,37 @@
                 data = self.db.query_by_sql(sql=sql, mode='one')
                 meta_unit = MetaUnit(**data, short_name=data['name'])
             case _:
                 meta_unit = MetaUnit(id=0, name='全国', short_name='全国')
         return meta_unit
 
     def query_schools_all(self):
-        sql = f"select * from schools;"
+        sql = f"select id, name, short_name, created from schools;"
         return pd.read_sql(sql, self.db.conn)
 
     def query_schools_by_ids(self, school_ids: list[int]):
         if len(school_ids) == 0:
             return []
         elif len(school_ids) == 1:
-            sql = f"select * from schools where id={school_ids[0]};"
+            sql = f"select id, name, short_name, created from schools where id={school_ids[0]};"
         else:
-            sql = f"select * from schools where id in {tuple(school_ids)};"
+            sql = f"select id, name, short_name, created from schools where id in {tuple(school_ids)};"
         return pd.read_sql(sql, self.db.conn)
 
     def query_schools_by_startwith(self, startwith: int):
         param_len = len(str(startwith))
-        sql = f"select * from schools where left(id,{param_len})={startwith};"
+        sql = f"select id, name, short_name, created from schools where left(id,{param_len})={startwith};"
         return pd.read_sql(sql, self.db.conn)
 
     def query_papers(self, test_type: str = '', test_types: list[str] = None):
         """优先 test_types"""
         if test_types:
-            sql = f"select * from papers where test_type in {tuple(test_types)};"
+            sql = f"select id, name, grade, test_type, created from papers where test_type in {tuple(test_types)};"
         elif test_type:
-            sql = f"select * from papers where test_type='{test_type}';"
+            sql = f"select id, name, grade, test_type, created from papers where test_type='{test_type}';"
         else:
             raise
         return pd.read_sql(sql, self.db.conn)
 
     def query_cases(
             self, school_ids: list[int], paper_ids: list[int],
             valid_to_start: str, valid_to_end: str,
@@ -71,37 +70,42 @@
             school_sql = f"and cs.school_id={school_ids[0]}"
         else:
             school_sql = f"and cs.school_id in {tuple(school_ids)}"
 
         sql = f"select c.id,c.name,c.valid_from,c.valid_to,c.client_id,c.created," \
               f"c.paper_id,c.is_cleared " \
               f"from cases c " \
-              f"left join case_schools cs on c.id=cs.case_id " \
-              f"where valid_to between '{valid_to_start}' and '{valid_to_end}'" \
-              f" {school_sql} {paper_sql} and is_cleared=1;"
+              f"inner join case_schools cs on c.id=cs.case_id " \
+              f"where  is_cleared=1 and valid_to between '{valid_to_start}' and '{valid_to_end}'" \
+              f" {school_sql} {paper_sql};"
         cases = pd.read_sql(sql, self.db.conn).drop_duplicates(subset=['id'])
         return cases
 
     def query_answers(self, case_ids: list[int]):
+        answer_cols = "id, student_id, item_id, case_id, answer, score, created, valid"
         if len(case_ids) == 0:
             return []
         elif len(case_ids) == 1:
-            sql = f"select * from answers where case_id={case_ids[0]} and valid=1;"
+            sql = f"select {answer_cols} from answers where case_id={case_ids[0]} and valid=1;"
         else:
-            sql = f"select * from answers where case_id in {tuple(case_ids)} and valid=1;"
+            sql = f"select {answer_cols} from answers where case_id in {tuple(case_ids)} and valid=1;"
         answers = pd.read_sql(sql, self.db.conn).drop_duplicates(subset=['case_id', 'student_id', 'item_id'])
         return answers
 
     def query_students(self, student_ids: list[int]):
-        sql = f"select * from users where id in {tuple(student_ids)} and length(id)>=18;"
+        user_cols = "id, username, first_name, last_name, nickname, gender, role, source, created, " \
+                    "unit_id, client_id, extra"
+        sql = f"select {user_cols} from users where id in {tuple(student_ids)} and length(id)>=18;"
         students = pd.read_sql(sql, self.db.conn).drop_duplicates(subset=['id'])
         return students
 
     def query_items(self, item_ids: list[int]):
-        sql = f"select * from items where id in {tuple(item_ids)}"
+        item_cols = "id, item_text, choices, item_key, item_type, grade, test_type, pattern, " \
+                    "`source`, created"
+        sql = f"select {item_cols} from items where id in {tuple(item_ids)};"
         return pd.read_sql(sql, self.db.conn)
 
     def query_item_codes(self, item_ids: list[int]):
         item_code_sql = f'select ic.item_id,ic.code,ic.category,c.name ' \
                         f'from item_codes ic left join codebook c on ic.code = c.code ' \
                         f'where ic.item_id in {tuple(item_ids)};'
         item_codes = pd.read_sql(item_code_sql, self.db.conn)
```

### Comparing `HawaData-0.3.0/hawa/common/utils.py` & `HawaData-0.3.1/hawa/common/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     @property
     def dimensions(self):
         return self._get_fields(category='dimension')
 
     def _get_fields(self, category: str):
         data = pd.read_sql(
-            f"select * from codebook where category='{category}' and name<>'其他'", self.db.conn)
+            f"select code, category, name from codebook where category='{category}' and name<>'其他'", self.db.conn)
         return data['name'].to_list()
 
     def _get_field_names(self, category: str):
         codes = self._get_fields(category=category)
         return '、'.join(codes[:len(codes) - 1]) + f'与{codes[-1]}'
```

### Comparing `HawaData-0.3.0/hawa/config.py` & `HawaData-0.3.1/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.0/hawa/paper/health.py` & `HawaData-0.3.1/hawa/paper/health.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.0/hawa/paper/mht.py` & `HawaData-0.3.1/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.0/setup.py` & `HawaData-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.0/test/mock.py` & `HawaData-0.3.1/test/mock.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.0/test/test_common/test_common_data.py` & `HawaData-0.3.1/test/test_common/test_common_data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.0/test/test_data/test_school.py` & `HawaData-0.3.1/test/test_data/test_school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.0/test/test_paper/test_health_data.py` & `HawaData-0.3.1/test/test_paper/test_health_data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.3.0/test/test_query.py` & `HawaData-0.3.1/test/test_query.py`

 * *Files identical despite different names*

