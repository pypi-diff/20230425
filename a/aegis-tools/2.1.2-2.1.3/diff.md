# Comparing `tmp/aegis-tools-2.1.2.tar.gz` & `tmp/aegis-tools-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aegis-tools-2.1.2.tar", last modified: Mon Apr 17 16:13:28 2023, max compression
+gzip compressed data, was "aegis-tools-2.1.3.tar", last modified: Mon Apr 24 22:50:27 2023, max compression
```

## Comparing `aegis-tools-2.1.2.tar` & `aegis-tools-2.1.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-17 16:13:28.613039 aegis-tools-2.1.2/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/LICENSE
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/MANIFEST.in
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-04-17 16:13:28.613039 aegis-tools-2.1.2/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/README.md
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-17 16:13:28.593039 aegis-tools-2.1.2/aegis/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/aegis/__init__.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    17334 2022-11-21 05:05:18.000000 aegis-tools-2.1.2/aegis/aegis_.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    18100 2022-11-21 04:55:50.000000 aegis-tools-2.1.2/aegis/build.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2380 2023-01-12 20:56:01.000000 aegis-tools-2.1.2/aegis/config.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    25757 2023-04-02 20:38:42.000000 aegis-tools-2.1.2/aegis/database.py
--rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    25692 2023-04-04 22:56:26.000000 aegis-tools-2.1.2/aegis/hydra.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     6919 2023-04-04 23:19:50.000000 aegis-tools-2.1.2/aegis/mailer.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    42189 2023-04-17 16:11:36.000000 aegis-tools-2.1.2/aegis/model.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-17 16:13:28.601039 aegis-tools-2.1.2/aegis/sql/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.1.2/aegis/sql/auditing-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4271 2023-02-05 03:12:16.000000 aegis-tools-2.1.2/aegis/sql/auditing-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/aegis/sql/build-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.1.2/aegis/sql/build-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/aegis/sql/cache_system.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.1.2/aegis/sql/email_system-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-03-13 22:09:08.000000 aegis-tools-2.1.2/aegis/sql/google_signin.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/aegis/sql/hydra-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/aegis/sql/hydra-pgsql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/aegis/sql/member_auth.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/aegis/sql/monitor-mysql.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/aegis/sql/reports.sql
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    31593 2023-04-02 17:41:52.000000 aegis-tools-2.1.2/aegis/stdlib.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-17 16:13:28.609039 aegis-tools-2.1.2/aegis/templates/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3083 2023-03-11 00:56:38.000000 aegis-tools-2.1.2/aegis/templates/build.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.1.2/aegis/templates/build_confirm.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.1.2/aegis/templates/build_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.1.2/aegis/templates/build_view.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/aegis/templates/error_message.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3297 2023-03-26 04:29:07.000000 aegis-tools-2.1.2/aegis/templates/frame.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2107 2023-03-11 00:53:08.000000 aegis-tools-2.1.2/aegis/templates/hydra.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.1.2/aegis/templates/hydra_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1660 2023-03-11 00:55:55.000000 aegis-tools-2.1.2/aegis/templates/hydra_queue.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.1.2/aegis/templates/index.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.1.2/aegis/templates/report.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.1.2/aegis/templates/report_form.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.1.2/aegis/templates/reports.html
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.1.2/aegis/templates/w3.css
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.1.2/aegis/threadpool.py
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    73096 2023-04-14 17:14:23.000000 aegis-tools-2.1.2/aegis/webapp.py
-drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-17 16:13:28.609039 aegis-tools-2.1.2/aegis_tools.egg-info/
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-04-17 16:13:28.000000 aegis-tools-2.1.2/aegis_tools.egg-info/PKG-INFO
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2023-04-17 16:13:28.000000 aegis-tools-2.1.2/aegis_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2023-04-17 16:13:28.000000 aegis-tools-2.1.2/aegis_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2023-04-17 16:13:28.000000 aegis-tools-2.1.2/aegis_tools.egg-info/entry_points.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2023-04-17 16:13:28.000000 aegis-tools-2.1.2/aegis_tools.egg-info/requires.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2023-04-17 16:13:28.000000 aegis-tools-2.1.2/aegis_tools.egg-info/top_level.txt
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2023-04-17 16:13:28.613039 aegis-tools-2.1.2/setup.cfg
--rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1676 2023-04-17 16:13:05.000000 aegis-tools-2.1.2/setup.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-24 22:50:27.214832 aegis-tools-2.1.3/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1073 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/LICENSE
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/MANIFEST.in
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-04-24 22:50:27.214832 aegis-tools-2.1.3/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      881 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/README.md
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-24 22:50:27.198832 aegis-tools-2.1.3/aegis/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       57 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/aegis/__init__.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    17334 2022-11-21 05:05:18.000000 aegis-tools-2.1.3/aegis/aegis_.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    18100 2022-11-21 04:55:50.000000 aegis-tools-2.1.3/aegis/build.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2380 2023-01-12 20:56:01.000000 aegis-tools-2.1.3/aegis/config.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    25757 2023-04-02 20:38:42.000000 aegis-tools-2.1.3/aegis/database.py
+-rwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)    25692 2023-04-04 22:56:26.000000 aegis-tools-2.1.3/aegis/hydra.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     7276 2023-04-24 22:47:56.000000 aegis-tools-2.1.3/aegis/mailer.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    42189 2023-04-17 16:11:36.000000 aegis-tools-2.1.3/aegis/model.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-24 22:50:27.206832 aegis-tools-2.1.3/aegis/sql/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1089 2022-11-22 01:51:27.000000 aegis-tools-2.1.3/aegis/sql/auditing-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     4271 2023-02-05 03:12:16.000000 aegis-tools-2.1.3/aegis/sql/auditing-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1051 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/aegis/sql/build-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1672 2022-11-16 03:24:54.000000 aegis-tools-2.1.3/aegis/sql/build-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      450 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/aegis/sql/cache_system.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1839 2023-04-02 17:24:35.000000 aegis-tools-2.1.3/aegis/sql/email_system-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1252 2023-03-13 22:09:08.000000 aegis-tools-2.1.3/aegis/sql/google_signin.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3409 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/aegis/sql/hydra-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3195 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/aegis/sql/hydra-pgsql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1535 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/aegis/sql/member_auth.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      616 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/aegis/sql/monitor-mysql.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      579 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/aegis/sql/reports.sql
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    31593 2023-04-24 21:25:57.000000 aegis-tools-2.1.3/aegis/stdlib.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-24 22:50:27.214832 aegis-tools-2.1.3/aegis/templates/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3083 2023-03-11 00:56:38.000000 aegis-tools-2.1.3/aegis/templates/build.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1549 2023-03-11 00:57:54.000000 aegis-tools-2.1.3/aegis/templates/build_confirm.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1187 2023-03-11 00:57:33.000000 aegis-tools-2.1.3/aegis/templates/build_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1217 2023-03-11 01:00:56.000000 aegis-tools-2.1.3/aegis/templates/build_view.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      253 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/aegis/templates/error_message.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     3297 2023-03-26 04:29:07.000000 aegis-tools-2.1.3/aegis/templates/frame.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2107 2023-03-11 00:53:08.000000 aegis-tools-2.1.3/aegis/templates/hydra.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2652 2023-03-11 00:52:58.000000 aegis-tools-2.1.3/aegis/templates/hydra_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1660 2023-03-11 00:55:55.000000 aegis-tools-2.1.3/aegis/templates/hydra_queue.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      109 2023-03-11 01:02:04.000000 aegis-tools-2.1.3/aegis/templates/index.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1954 2023-03-26 04:27:55.000000 aegis-tools-2.1.3/aegis/templates/report.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1909 2023-03-20 03:03:26.000000 aegis-tools-2.1.3/aegis/templates/report_form.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      745 2023-03-20 02:52:01.000000 aegis-tools-2.1.3/aegis/templates/reports.html
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    23427 2023-03-11 00:09:55.000000 aegis-tools-2.1.3/aegis/templates/w3.css
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     2681 2022-10-24 18:25:55.000000 aegis-tools-2.1.3/aegis/threadpool.py
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)    73127 2023-04-24 22:16:45.000000 aegis-tools-2.1.3/aegis/webapp.py
+drwxrwxr-x   0 mdagosta  (1000) mdagosta  (1000)        0 2023-04-24 22:50:27.214832 aegis-tools-2.1.3/aegis_tools.egg-info/
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)      808 2023-04-24 22:50:27.000000 aegis-tools-2.1.3/aegis_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1176 2023-04-24 22:50:27.000000 aegis-tools-2.1.3/aegis_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        1 2023-04-24 22:50:27.000000 aegis-tools-2.1.3/aegis_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       45 2023-04-24 22:50:27.000000 aegis-tools-2.1.3/aegis_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       85 2023-04-24 22:50:27.000000 aegis-tools-2.1.3/aegis_tools.egg-info/requires.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)        6 2023-04-24 22:50:27.000000 aegis-tools-2.1.3/aegis_tools.egg-info/top_level.txt
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)       38 2023-04-24 22:50:27.214832 aegis-tools-2.1.3/setup.cfg
+-rw-rw-r--   0 mdagosta  (1000) mdagosta  (1000)     1676 2023-04-24 22:50:08.000000 aegis-tools-2.1.3/setup.py
```

### Comparing `aegis-tools-2.1.2/LICENSE` & `aegis-tools-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/PKG-INFO` & `aegis-tools-2.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.1.2
+Version: 2.1.3
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.1.2/README.md` & `aegis-tools-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/aegis_.py` & `aegis-tools-2.1.3/aegis/aegis_.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/build.py` & `aegis-tools-2.1.3/aegis/build.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/config.py` & `aegis-tools-2.1.3/aegis/config.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/database.py` & `aegis-tools-2.1.3/aegis/database.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/hydra.py` & `aegis-tools-2.1.3/aegis/hydra.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/mailer.py` & `aegis-tools-2.1.3/aegis/mailer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # E-mail utilities
 #
 # A lot is adapted from https://mg.pov.lt/blog/unicode-emails-in-python
 
 
 # Python Imports
 import datetime
+import email.charset
 import email.header
 import email.mime.multipart
 import email.mime.text
 import email.utils
 import json
 import logging
 import smtplib
@@ -20,14 +21,17 @@
 import pytz
 import tornado.template
 
 # Project Imports
 import config
 
 
+# Use Quoted-printable encoding instead of base64 since it's far more legible at a glance! From https://bugs.python.org/issue12552
+email.charset.add_charset('utf-8', email.charset.SHORTEST, email.charset.QP)
+
 class Mailer(object):
     template_registry = {}
 
 
     @classmethod
     def register_template(cls, domain, email_type_name, function):
         cls.template_registry.setdefault(domain, {})
@@ -83,22 +87,22 @@
         if not handler:
             host_config = config.hostnames[kwargs['domain']]
             template_loader = tornado.template.Loader(host_config['template_path'])
             plain = ''
             html = ''
             try:
                 plain = template_loader.load(template+'.txt').generate(**email_opts)
-            except:
-                logging.exception("Couldn't render plaintext email for template: %s" % template)
-                pass
+            except FileNotFoundError as ex:
+                if kwargs.get('debug'):
+                    logging.exception("Couldn't render plaintext email for template: %s" % template)
             try:
                 html = template_loader.load(template+'.html').generate(**email_opts)
-            except:
-                logging.exception("Couldn't render HTML email for template: %s" % template)
-                pass
+            except FileNotFoundError as ex:
+                if kwargs.get('debug'):
+                    logging.exception("Couldn't render HTML email for template: %s" % template)
         else:
             plain = handler.render_string('%s.txt' % template, **email_opts)
             html =  handler.render_string('%s.html' % template, **email_opts)
         body = {'plain': plain, 'html': html}
         reply_to = kwargs.get('reply_to', from_email)
         service_sender = kwargs.get('service_sender', from_email)
         return cls.encode_email(from_email, to_addrs, subject, body, reply_to, service_sender)
@@ -137,17 +141,18 @@
         # It's a mouthful to convert this to Pacific time
         email_data['send_dttm_str'] = email_tracking['send_dttm'].astimezone(pytz.timezone('US/Pacific')).strftime('%b %d, %Y, %-H:%-M %p')
         email_data['options'] = options
         email_data['current_year'] = datetime.date.today().year
         email_data['email_tracking_id'] = email_tracking_id
         email_data['email_uuid'] = email_tracking['email_uuid']
         email_template = 'email/%s' % email_type['template_name']
+        #kwargs['debug'] = True
         email_msg = cls.render_email(None, email_data['from_addr'], email_data['to_addr'], email_data['subject'], email_template, email_data, **kwargs)
         if email_msg:
-            logging.warning(email_msg)
+            #logging.warning(email_msg)
             sent = cls.sendmail(from_email['email'], to_email['email'], email_msg)
             # Record email_tracking as sent
             if sent:
                 email_tracking.mark_sent(dbconn=dbconn)
             return True
         return False
```

### Comparing `aegis-tools-2.1.2/aegis/model.py` & `aegis-tools-2.1.3/aegis/model.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/sql/auditing-mysql.sql` & `aegis-tools-2.1.3/aegis/sql/auditing-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/sql/auditing-pgsql.sql` & `aegis-tools-2.1.3/aegis/sql/auditing-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/sql/build-mysql.sql` & `aegis-tools-2.1.3/aegis/sql/build-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/sql/build-pgsql.sql` & `aegis-tools-2.1.3/aegis/sql/build-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/sql/email_system-pgsql.sql` & `aegis-tools-2.1.3/aegis/sql/email_system-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/sql/google_signin.sql` & `aegis-tools-2.1.3/aegis/sql/google_signin.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/sql/hydra-mysql.sql` & `aegis-tools-2.1.3/aegis/sql/hydra-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/sql/hydra-pgsql.sql` & `aegis-tools-2.1.3/aegis/sql/hydra-pgsql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/sql/member_auth.sql` & `aegis-tools-2.1.3/aegis/sql/member_auth.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/sql/monitor-mysql.sql` & `aegis-tools-2.1.3/aegis/sql/monitor-mysql.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/sql/reports.sql` & `aegis-tools-2.1.3/aegis/sql/reports.sql`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/stdlib.py` & `aegis-tools-2.1.3/aegis/stdlib.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/templates/build.html` & `aegis-tools-2.1.3/aegis/templates/build.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/templates/build_confirm.html` & `aegis-tools-2.1.3/aegis/templates/build_confirm.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/templates/build_form.html` & `aegis-tools-2.1.3/aegis/templates/build_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/templates/build_view.html` & `aegis-tools-2.1.3/aegis/templates/build_view.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/templates/frame.html` & `aegis-tools-2.1.3/aegis/templates/frame.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/templates/hydra.html` & `aegis-tools-2.1.3/aegis/templates/hydra.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/templates/hydra_form.html` & `aegis-tools-2.1.3/aegis/templates/hydra_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/templates/hydra_queue.html` & `aegis-tools-2.1.3/aegis/templates/hydra_queue.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/templates/report.html` & `aegis-tools-2.1.3/aegis/templates/report.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/templates/report_form.html` & `aegis-tools-2.1.3/aegis/templates/report_form.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/templates/reports.html` & `aegis-tools-2.1.3/aegis/templates/reports.html`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/templates/w3.css` & `aegis-tools-2.1.3/aegis/templates/w3.css`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/threadpool.py` & `aegis-tools-2.1.3/aegis/threadpool.py`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/aegis/webapp.py` & `aegis-tools-2.1.3/aegis/webapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -775,15 +775,15 @@
         email_tracking = aegis.model.EmailTracking.get_params(aegis.stdlib.validate_int(self.request.args['t']), self.request.args['e'])
         if not email_tracking:
             return
         if not email_tracking['deliver_dttm']:
             email_tracking.mark_delivered()
         if not email_tracking['open_dttm']:
             email_tracking.mark_opened()
-        if not email_tracking['click_dttm']:
+        if self.request.args.get('c') and not email_tracking['click_dttm']:
             email_tracking.mark_clicked()
         # Mark email and member verified
         email = aegis.model.Email.get_id(email_tracking['to_email_id'])
         if email:
             email.mark_verified()
             if email['member_id'] and email['member_id'] == self.get_member_id():
                 self.get_current_user().mark_verified()
```

### Comparing `aegis-tools-2.1.2/aegis_tools.egg-info/PKG-INFO` & `aegis-tools-2.1.3/aegis_tools.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aegis-tools
-Version: 2.1.2
+Version: 2.1.3
 Summary: Aegis is a set of battle-tested tools and tricks to help everyone make better software
 Home-page: https://github.com/mdagosta/aegis
 Author: Michael D'Agosta
 Author-email: mdagosta@codebug.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aegis-tools-2.1.2/aegis_tools.egg-info/SOURCES.txt` & `aegis-tools-2.1.3/aegis_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aegis-tools-2.1.2/setup.py` & `aegis-tools-2.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 
 import os
 import setuptools
 
 setuptools.setup (
     name = 'aegis-tools',
-    version = '2.1.2',
+    version = '2.1.3',
     description = 'Aegis is a set of battle-tested tools and tricks to help everyone make better software',
     long_description = 'A combination of tools and framework, Aegis has multiple different uses. You can import it and use the thoroughly made and tested functions. You can use it as a natural extension for the tornado web framework. And you can use it to quickly create a new web application with the structure already built-in, and follow along.',
     author = "Michael D'Agosta",
     author_email = 'mdagosta@codebug.com',
     url = 'https://github.com/mdagosta/aegis',
     python_requires='>=3.6',
     packages = ['aegis'],
```

