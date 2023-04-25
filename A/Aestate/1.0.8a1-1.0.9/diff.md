# Comparing `tmp/Aestate-1.0.8a1.tar.gz` & `tmp/Aestate-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Aestate-1.0.8a1.tar", last modified: Mon Sep 12 10:04:16 2022, max compression
+gzip compressed data, was "Aestate-1.0.9.tar", last modified: Tue Apr 25 06:55:03 2023, max compression
```

## Comparing `Aestate-1.0.8a1.tar` & `Aestate-1.0.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxrwx   0        0        0        0 2022-09-12 10:04:16.000000 Aestate-1.0.8a1/
-drwxrwxrwx   0        0        0        0 2022-09-12 10:04:15.000000 Aestate-1.0.8a1/Aestate.egg-info/
--rw-rw-rw-   0        0        0     9824 2022-09-12 10:04:15.000000 Aestate-1.0.8a1/Aestate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1408 2022-09-12 10:04:15.000000 Aestate-1.0.8a1/Aestate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-12 10:04:15.000000 Aestate-1.0.8a1/Aestate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2022-09-12 10:04:15.000000 Aestate-1.0.8a1/Aestate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2022-09-12 10:04:15.000000 Aestate-1.0.8a1/Aestate.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-09-12 10:04:15.000000 Aestate-1.0.8a1/Aestate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11556 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/LICENSE
--rw-rw-rw-   0        0        0     9824 2022-09-12 10:04:16.000000 Aestate-1.0.8a1/PKG-INFO
--rw-rw-rw-   0        0        0     9204 2022-09-10 18:26:17.000000 Aestate-1.0.8a1/README.md
-drwxrwxrwx   0        0        0        0 2022-09-12 10:04:15.000000 Aestate-1.0.8a1/aestate/
--rw-rw-rw-   0        0        0      396 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-12 10:04:16.000000 Aestate-1.0.8a1/aestate/ajson/
--rw-rw-rw-   0        0        0       53 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/ajson/__init__.py
--rw-rw-rw-   0        0        0    11743 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/ajson/ajson.py
-drwxrwxrwx   0        0        0        0 2022-09-12 10:04:16.000000 Aestate-1.0.8a1/aestate/base/
--rw-rw-rw-   0        0        0        0 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/base/__init__.py
--rw-rw-rw-   0        0        0      664 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/base/anno.py
--rw-rw-rw-   0        0        0     1504 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/base/manage.py
--rw-rw-rw-   0        0        0     1059 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/base/model.py
--rw-rw-rw-   0        0        0    10358 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/base/proxy.py
--rw-rw-rw-   0        0        0      416 2022-09-10 17:04:55.000000 Aestate-1.0.8a1/aestate/conf.py
-drwxrwxrwx   0        0        0        0 2022-09-12 10:04:16.000000 Aestate-1.0.8a1/aestate/dbs/
--rw-rw-rw-   0        0        0      156 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/dbs/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-12 10:04:16.000000 Aestate-1.0.8a1/aestate/dbs/_mssql/
--rw-rw-rw-   0        0        0    13957 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/dbs/_mssql/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-12 10:04:16.000000 Aestate-1.0.8a1/aestate/dbs/_mysql/
--rw-rw-rw-   0        0        0    17947 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/dbs/_mysql/__init__.py
--rw-rw-rw-   0        0        0     6609 2022-09-10 18:04:14.000000 Aestate-1.0.8a1/aestate/dbs/_mysql/tag.py
--rw-rw-rw-   0        0        0      255 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/dbs/base.py
-drwxrwxrwx   0        0        0        0 2022-09-12 10:04:16.000000 Aestate-1.0.8a1/aestate/exception/
--rw-rw-rw-   0        0        0     1446 2022-09-10 17:03:16.000000 Aestate-1.0.8a1/aestate/exception/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-12 10:04:16.000000 Aestate-1.0.8a1/aestate/i18n/
--rw-rw-rw-   0        0        0     3686 2022-09-12 10:01:38.000000 Aestate-1.0.8a1/aestate/i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-12 10:04:16.000000 Aestate-1.0.8a1/aestate/util/
--rw-rw-rw-   0        0        0     1298 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/util/CompulsoryRun.py
--rw-rw-rw-   0        0        0    12683 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/util/Log.py
--rw-rw-rw-   0        0        0      354 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/util/__init__.py
--rw-rw-rw-   0        0        0     6280 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/util/others.py
--rw-rw-rw-   0        0        0      779 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/util/sqlOpera.py
-drwxrwxrwx   0        0        0        0 2022-09-12 10:04:16.000000 Aestate-1.0.8a1/aestate/work/
--rw-rw-rw-   0        0        0     2853 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/work/Adapter.py
--rw-rw-rw-   0        0        0    10220 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/work/Annotation.py
--rw-rw-rw-   0        0        0     5402 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/work/AopContainer.py
--rw-rw-rw-   0        0        0    27175 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/work/Cache.py
--rw-rw-rw-   0        0        0     2708 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/work/Config.py
--rw-rw-rw-   0        0        0     5981 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/work/Manage.py
--rw-rw-rw-   0        0        0     9658 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/work/Modes.py
--rw-rw-rw-   0        0        0     4761 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/work/Serialize.py
--rw-rw-rw-   0        0        0      321 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/work/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-12 10:04:16.000000 Aestate-1.0.8a1/aestate/work/commands/
--rw-rw-rw-   0        0        0     5551 2022-09-12 10:04:00.000000 Aestate-1.0.8a1/aestate/work/commands/__init__.py
--rw-rw-rw-   0        0        0    18624 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/work/orm.py
-drwxrwxrwx   0        0        0        0 2022-09-12 10:04:16.000000 Aestate-1.0.8a1/aestate/work/proxy/
--rw-rw-rw-   0        0        0    10724 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/work/proxy/SqlOperaProxy.py
--rw-rw-rw-   0        0        0       17 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/work/proxy/__init__.py
--rw-rw-rw-   0        0        0     5112 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/work/repository.py
-drwxrwxrwx   0        0        0        0 2022-09-12 10:04:16.000000 Aestate-1.0.8a1/aestate/work/sql/
--rw-rw-rw-   0        0        0     7445 2022-09-10 18:04:14.000000 Aestate-1.0.8a1/aestate/work/sql/ExecuteSql.py
--rw-rw-rw-   0        0        0     5030 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/work/sql/ProxyOpera.py
--rw-rw-rw-   0        0        0       17 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/work/sql/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-12 10:04:16.000000 Aestate-1.0.8a1/aestate/work/xmlhandler/
--rw-rw-rw-   0        0        0     3776 2022-09-12 05:58:11.000000 Aestate-1.0.8a1/aestate/work/xmlhandler/XMLScriptBuilder.py
--rw-rw-rw-   0        0        0       17 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/work/xmlhandler/__init__.py
--rw-rw-rw-   0        0        0     1796 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/work/xmlhandler/base.py
--rw-rw-rw-   0        0        0      333 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/work/xmlhandler/final.py
--rw-rw-rw-   0        0        0    13722 2022-09-12 09:10:51.000000 Aestate-1.0.8a1/aestate/work/xmlhandler/nodes.py
--rw-rw-rw-   0        0        0     2077 2022-08-30 13:27:49.000000 Aestate-1.0.8a1/aestate/work/xmlhandler/utils.py
--rw-rw-rw-   0        0        0      108 2022-08-30 13:27:50.000000 Aestate-1.0.8a1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-09-12 10:04:16.000000 Aestate-1.0.8a1/setup.cfg
--rw-rw-rw-   0        0        0     1618 2022-09-10 18:05:51.000000 Aestate-1.0.8a1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.687219 Aestate-1.0.9/
+drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.641373 Aestate-1.0.9/Aestate.egg-info/
+-rw-rw-rw-   0        0        0     9903 2023-04-25 06:55:03.000000 Aestate-1.0.9/Aestate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1408 2023-04-25 06:55:03.000000 Aestate-1.0.9/Aestate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 06:55:03.000000 Aestate-1.0.9/Aestate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-25 06:55:03.000000 Aestate-1.0.9/Aestate.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-04-25 06:55:03.000000 Aestate-1.0.9/Aestate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-25 06:55:03.000000 Aestate-1.0.9/Aestate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11556 2023-03-09 03:30:52.000000 Aestate-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     9903 2023-04-25 06:55:03.687219 Aestate-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     9285 2023-04-25 06:54:22.000000 Aestate-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.643366 Aestate-1.0.9/aestate/
+-rw-rw-rw-   0        0        0      396 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.645359 Aestate-1.0.9/aestate/ajson/
+-rw-rw-rw-   0        0        0       53 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/ajson/__init__.py
+-rw-rw-rw-   0        0        0    11743 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/ajson/ajson.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.649346 Aestate-1.0.9/aestate/base/
+-rw-rw-rw-   0        0        0        0 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/base/__init__.py
+-rw-rw-rw-   0        0        0      664 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/base/anno.py
+-rw-rw-rw-   0        0        0     1504 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/base/manage.py
+-rw-rw-rw-   0        0        0     1059 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/base/model.py
+-rw-rw-rw-   0        0        0    10358 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/base/proxy.py
+-rw-rw-rw-   0        0        0      416 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/conf.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.651339 Aestate-1.0.9/aestate/dbs/
+-rw-rw-rw-   0        0        0      156 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/dbs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.652337 Aestate-1.0.9/aestate/dbs/_mssql/
+-rw-rw-rw-   0        0        0    13957 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/dbs/_mssql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.654328 Aestate-1.0.9/aestate/dbs/_mysql/
+-rw-rw-rw-   0        0        0    17947 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/dbs/_mysql/__init__.py
+-rw-rw-rw-   0        0        0     6609 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/dbs/_mysql/tag.py
+-rw-rw-rw-   0        0        0      255 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/dbs/base.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.657329 Aestate-1.0.9/aestate/exception/
+-rw-rw-rw-   0        0        0     1446 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/exception/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.658315 Aestate-1.0.9/aestate/i18n/
+-rw-rw-rw-   0        0        0     3573 2023-04-25 06:54:22.000000 Aestate-1.0.9/aestate/i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.663298 Aestate-1.0.9/aestate/util/
+-rw-rw-rw-   0        0        0     1298 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/util/CompulsoryRun.py
+-rw-rw-rw-   0        0        0    13156 2023-04-25 06:54:22.000000 Aestate-1.0.9/aestate/util/Log.py
+-rw-rw-rw-   0        0        0      354 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/util/__init__.py
+-rw-rw-rw-   0        0        0     6280 2023-04-25 02:31:39.000000 Aestate-1.0.9/aestate/util/others.py
+-rw-rw-rw-   0        0        0      779 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/util/sqlOpera.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.673265 Aestate-1.0.9/aestate/work/
+-rw-rw-rw-   0        0        0     2853 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/Adapter.py
+-rw-rw-rw-   0        0        0    10336 2023-04-25 06:54:22.000000 Aestate-1.0.9/aestate/work/Annotation.py
+-rw-rw-rw-   0        0        0     5402 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/AopContainer.py
+-rw-rw-rw-   0        0        0     1977 2023-04-25 06:54:22.000000 Aestate-1.0.9/aestate/work/Cache.py
+-rw-rw-rw-   0        0        0     2708 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/Config.py
+-rw-rw-rw-   0        0        0     5981 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/Manage.py
+-rw-rw-rw-   0        0        0     9658 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/Modes.py
+-rw-rw-rw-   0        0        0     4761 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/Serialize.py
+-rw-rw-rw-   0        0        0      321 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.674261 Aestate-1.0.9/aestate/work/commands/
+-rw-rw-rw-   0        0        0     5549 2023-04-25 06:54:22.000000 Aestate-1.0.9/aestate/work/commands/__init__.py
+-rw-rw-rw-   0        0        0    18717 2023-04-25 06:54:22.000000 Aestate-1.0.9/aestate/work/orm.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.677265 Aestate-1.0.9/aestate/work/proxy/
+-rw-rw-rw-   0        0        0    10724 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/proxy/SqlOperaProxy.py
+-rw-rw-rw-   0        0        0       17 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/proxy/__init__.py
+-rw-rw-rw-   0        0        0     5112 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/repository.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.680241 Aestate-1.0.9/aestate/work/sql/
+-rw-rw-rw-   0        0        0     6526 2023-04-25 06:54:22.000000 Aestate-1.0.9/aestate/work/sql/ExecuteSql.py
+-rw-rw-rw-   0        0        0     5030 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/sql/ProxyOpera.py
+-rw-rw-rw-   0        0        0       17 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/sql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 06:55:03.686222 Aestate-1.0.9/aestate/work/xmlhandler/
+-rw-rw-rw-   0        0        0     3776 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/xmlhandler/XMLScriptBuilder.py
+-rw-rw-rw-   0        0        0       17 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/xmlhandler/__init__.py
+-rw-rw-rw-   0        0        0     1796 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/xmlhandler/base.py
+-rw-rw-rw-   0        0        0      333 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/xmlhandler/final.py
+-rw-rw-rw-   0        0        0    13722 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/xmlhandler/nodes.py
+-rw-rw-rw-   0        0        0     2077 2023-03-09 03:30:52.000000 Aestate-1.0.9/aestate/work/xmlhandler/utils.py
+-rw-rw-rw-   0        0        0      108 2023-03-09 03:30:52.000000 Aestate-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 06:55:03.688215 Aestate-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1618 2023-03-09 03:30:52.000000 Aestate-1.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Aestate-1.0.8a1/Aestate.egg-info/PKG-INFO` & `Aestate-1.0.9/Aestate.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aestate
-Version: 1.0.8a1
+Version: 1.0.9
 Summary: Aestate framework for Python,You can see:https://gitee.com/aecode/aestate
 Home-page: https://gitee.com/aecode/aestate
 Author: CACode
 Author-email: cacode@163.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://gitee.com/aecode/aestate/issues
 Platform: UNKNOWN
@@ -191,15 +191,16 @@
 1. Java专业户：用xml、方法名和注解
 2. Python专业户：用Django模式和SQLAlchemy模式
 3. 纯萌新：老老实实写SQL，先把基础练好
 
 # 谁在使用 Aestate Framework 开发网站
 
 CACode： [https://cacode.ren](https://cacode.ren)  
-CocoZao 爬虫：[https://ccz.cacode.ren](https://ccz.cacode.ren)
+CocoZao 爬虫：[https://ccz.cacode.ren](https://ccz.cacode.ren)  
+还有很多很多个人开发者以及需要快速开发的外包工作者
 > 开源示例项目：[gitee/aestate-example](https://gitee.com/canotf/aestate-example)
 
 更多示例项目请前往
 > [👉 Go to canotf`s homepage on Gitee 👈](https://gitee.com/canotf)
 
 # 鸣谢
 
@@ -218,13 +219,14 @@
 </a>
 <a href="https://gitee.com/potuo">
 <img alt="Potuo" width="49%" src="https://svg.hamm.cn/gitee-user.svg?user=potuo"/>
 </a>
 <a href="https://gitee.com/zxiaosi">
 <img alt="Zxiaosi" width="49%" src="https://svg.hamm.cn/gitee-user.svg?user=zxiaosi"/>
 </a>
-<a href="https://gitee.com/zxiaosi">
+<a href="https://gitee.com/xierkz">
 <img alt="Xierkz" width="49%" src="https://svg.hamm.cn/gitee-user.svg?user=xierkz"/>
 </a>
-# CACode Development Team
+
+# Aestate Development Team
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Aestate Version: 1.0.8a1 Summary: Aestate framework
+Metadata-Version: 2.1 Name: Aestate Version: 1.0.9 Summary: Aestate framework
 for Python,You can see:https://gitee.com/aecode/aestate Home-page: https://
 gitee.com/aecode/aestate Author: CACode Author-email: cacode@163.com License:
 Apache License 2.0 Project-URL: Bug Tracker, https://gitee.com/aecode/aestate/
 issues Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Database Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
@@ -68,13 +68,14 @@
 (https://blog.csdn.net/qq_43059459) #
 æä½æ¹å¼å¤ªå¤äºä¸ä¸å­å­¦ä¸ä¼æä¹åï¼
 **Aestate**æäºç§æ¹å¼ï¼ä¸æ¯éè¦å¨é¨é½ä¼ï¼æå½æ¶åçæ¶ååªæ¯ä¸ºäºæå¾å¤è¯­è¨çæä½æ¹å¼ç¨Pythonå®ç°ï¼ç¶åè®©å¶ä»è¯­è¨è½¬Pythonçå¼åèè½å¤æ¾å°çæçæè§ï¼ä¾å¦
 1. Javaä¸ä¸æ·ï¼ç¨xmlãæ¹æ³ååæ³¨è§£ 2.
 Pythonä¸ä¸æ·ï¼ç¨Djangoæ¨¡å¼åSQLAlchemyæ¨¡å¼ 3.
 çº¯èæ°ï¼èèå®å®åSQLï¼åæåºç¡ç»å¥½ # è°å¨ä½¿ç¨ Aestate
 Framework å¼åç½ç« CACodeï¼ [https://cacode.ren](https://cacode.ren)
-CocoZao ç¬è«ï¼[https://ccz.cacode.ren](https://ccz.cacode.ren) >
+CocoZao ç¬è«ï¼[https://ccz.cacode.ren](https://ccz.cacode.ren)
+è¿æå¾å¤å¾å¤ä¸ªäººå¼åèä»¥åéè¦å¿«éå¼åçå¤åå·¥ä½è >
 å¼æºç¤ºä¾é¡¹ç®ï¼[gitee/aestate-example](https://gitee.com/canotf/aestate-
 example) æ´å¤ç¤ºä¾é¡¹ç®è¯·åå¾ > [ð Go to canotf`s homepage on Gitee
 ð](https://gitee.com/canotf) # é¸£è°¢ Cpython DBPool Simplejson Gitee #
-æè°¢æç® [Spacexzm] [Canotf] [Potuo] [Zxiaosi] [Xierkz] # CACode
+æè°¢æç® [Spacexzm] [Canotf] [Potuo] [Zxiaosi] [Xierkz] # Aestate
 Development Team
```

### Comparing `Aestate-1.0.8a1/Aestate.egg-info/SOURCES.txt` & `Aestate-1.0.9/Aestate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/LICENSE` & `Aestate-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/PKG-INFO` & `Aestate-1.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aestate
-Version: 1.0.8a1
+Version: 1.0.9
 Summary: Aestate framework for Python,You can see:https://gitee.com/aecode/aestate
 Home-page: https://gitee.com/aecode/aestate
 Author: CACode
 Author-email: cacode@163.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://gitee.com/aecode/aestate/issues
 Platform: UNKNOWN
@@ -191,15 +191,16 @@
 1. Java专业户：用xml、方法名和注解
 2. Python专业户：用Django模式和SQLAlchemy模式
 3. 纯萌新：老老实实写SQL，先把基础练好
 
 # 谁在使用 Aestate Framework 开发网站
 
 CACode： [https://cacode.ren](https://cacode.ren)  
-CocoZao 爬虫：[https://ccz.cacode.ren](https://ccz.cacode.ren)
+CocoZao 爬虫：[https://ccz.cacode.ren](https://ccz.cacode.ren)  
+还有很多很多个人开发者以及需要快速开发的外包工作者
 > 开源示例项目：[gitee/aestate-example](https://gitee.com/canotf/aestate-example)
 
 更多示例项目请前往
 > [👉 Go to canotf`s homepage on Gitee 👈](https://gitee.com/canotf)
 
 # 鸣谢
 
@@ -218,13 +219,14 @@
 </a>
 <a href="https://gitee.com/potuo">
 <img alt="Potuo" width="49%" src="https://svg.hamm.cn/gitee-user.svg?user=potuo"/>
 </a>
 <a href="https://gitee.com/zxiaosi">
 <img alt="Zxiaosi" width="49%" src="https://svg.hamm.cn/gitee-user.svg?user=zxiaosi"/>
 </a>
-<a href="https://gitee.com/zxiaosi">
+<a href="https://gitee.com/xierkz">
 <img alt="Xierkz" width="49%" src="https://svg.hamm.cn/gitee-user.svg?user=xierkz"/>
 </a>
-# CACode Development Team
+
+# Aestate Development Team
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Aestate Version: 1.0.8a1 Summary: Aestate framework
+Metadata-Version: 2.1 Name: Aestate Version: 1.0.9 Summary: Aestate framework
 for Python,You can see:https://gitee.com/aecode/aestate Home-page: https://
 gitee.com/aecode/aestate Author: CACode Author-email: cacode@163.com License:
 Apache License 2.0 Project-URL: Bug Tracker, https://gitee.com/aecode/aestate/
 issues Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Database Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
@@ -68,13 +68,14 @@
 (https://blog.csdn.net/qq_43059459) #
 æä½æ¹å¼å¤ªå¤äºä¸ä¸å­å­¦ä¸ä¼æä¹åï¼
 **Aestate**æäºç§æ¹å¼ï¼ä¸æ¯éè¦å¨é¨é½ä¼ï¼æå½æ¶åçæ¶ååªæ¯ä¸ºäºæå¾å¤è¯­è¨çæä½æ¹å¼ç¨Pythonå®ç°ï¼ç¶åè®©å¶ä»è¯­è¨è½¬Pythonçå¼åèè½å¤æ¾å°çæçæè§ï¼ä¾å¦
 1. Javaä¸ä¸æ·ï¼ç¨xmlãæ¹æ³ååæ³¨è§£ 2.
 Pythonä¸ä¸æ·ï¼ç¨Djangoæ¨¡å¼åSQLAlchemyæ¨¡å¼ 3.
 çº¯èæ°ï¼èèå®å®åSQLï¼åæåºç¡ç»å¥½ # è°å¨ä½¿ç¨ Aestate
 Framework å¼åç½ç« CACodeï¼ [https://cacode.ren](https://cacode.ren)
-CocoZao ç¬è«ï¼[https://ccz.cacode.ren](https://ccz.cacode.ren) >
+CocoZao ç¬è«ï¼[https://ccz.cacode.ren](https://ccz.cacode.ren)
+è¿æå¾å¤å¾å¤ä¸ªäººå¼åèä»¥åéè¦å¿«éå¼åçå¤åå·¥ä½è >
 å¼æºç¤ºä¾é¡¹ç®ï¼[gitee/aestate-example](https://gitee.com/canotf/aestate-
 example) æ´å¤ç¤ºä¾é¡¹ç®è¯·åå¾ > [ð Go to canotf`s homepage on Gitee
 ð](https://gitee.com/canotf) # é¸£è°¢ Cpython DBPool Simplejson Gitee #
-æè°¢æç® [Spacexzm] [Canotf] [Potuo] [Zxiaosi] [Xierkz] # CACode
+æè°¢æç® [Spacexzm] [Canotf] [Potuo] [Zxiaosi] [Xierkz] # Aestate
 Development Team
```

### Comparing `Aestate-1.0.8a1/README.md` & `Aestate-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,16 @@
 1. Java专业户：用xml、方法名和注解
 2. Python专业户：用Django模式和SQLAlchemy模式
 3. 纯萌新：老老实实写SQL，先把基础练好
 
 # 谁在使用 Aestate Framework 开发网站
 
 CACode： [https://cacode.ren](https://cacode.ren)  
-CocoZao 爬虫：[https://ccz.cacode.ren](https://ccz.cacode.ren)
+CocoZao 爬虫：[https://ccz.cacode.ren](https://ccz.cacode.ren)  
+还有很多很多个人开发者以及需要快速开发的外包工作者
 > 开源示例项目：[gitee/aestate-example](https://gitee.com/canotf/aestate-example)
 
 更多示例项目请前往
 > [👉 Go to canotf`s homepage on Gitee 👈](https://gitee.com/canotf)
 
 # 鸣谢
 
@@ -200,11 +201,12 @@
 </a>
 <a href="https://gitee.com/potuo">
 <img alt="Potuo" width="49%" src="https://svg.hamm.cn/gitee-user.svg?user=potuo"/>
 </a>
 <a href="https://gitee.com/zxiaosi">
 <img alt="Zxiaosi" width="49%" src="https://svg.hamm.cn/gitee-user.svg?user=zxiaosi"/>
 </a>
-<a href="https://gitee.com/zxiaosi">
+<a href="https://gitee.com/xierkz">
 <img alt="Xierkz" width="49%" src="https://svg.hamm.cn/gitee-user.svg?user=xierkz"/>
 </a>
-# CACode Development Team
+
+# Aestate Development Team
```

#### html2text {}

```diff
@@ -60,13 +60,14 @@
 (https://blog.csdn.net/qq_43059459) #
 æä½æ¹å¼å¤ªå¤äºä¸ä¸å­å­¦ä¸ä¼æä¹åï¼
 **Aestate**æäºç§æ¹å¼ï¼ä¸æ¯éè¦å¨é¨é½ä¼ï¼æå½æ¶åçæ¶ååªæ¯ä¸ºäºæå¾å¤è¯­è¨çæä½æ¹å¼ç¨Pythonå®ç°ï¼ç¶åè®©å¶ä»è¯­è¨è½¬Pythonçå¼åèè½å¤æ¾å°çæçæè§ï¼ä¾å¦
 1. Javaä¸ä¸æ·ï¼ç¨xmlãæ¹æ³ååæ³¨è§£ 2.
 Pythonä¸ä¸æ·ï¼ç¨Djangoæ¨¡å¼åSQLAlchemyæ¨¡å¼ 3.
 çº¯èæ°ï¼èèå®å®åSQLï¼åæåºç¡ç»å¥½ # è°å¨ä½¿ç¨ Aestate
 Framework å¼åç½ç« CACodeï¼ [https://cacode.ren](https://cacode.ren)
-CocoZao ç¬è«ï¼[https://ccz.cacode.ren](https://ccz.cacode.ren) >
+CocoZao ç¬è«ï¼[https://ccz.cacode.ren](https://ccz.cacode.ren)
+è¿æå¾å¤å¾å¤ä¸ªäººå¼åèä»¥åéè¦å¿«éå¼åçå¤åå·¥ä½è >
 å¼æºç¤ºä¾é¡¹ç®ï¼[gitee/aestate-example](https://gitee.com/canotf/aestate-
 example) æ´å¤ç¤ºä¾é¡¹ç®è¯·åå¾ > [ð Go to canotf`s homepage on Gitee
 ð](https://gitee.com/canotf) # é¸£è°¢ Cpython DBPool Simplejson Gitee #
-æè°¢æç® [Spacexzm] [Canotf] [Potuo] [Zxiaosi] [Xierkz] # CACode
+æè°¢æç® [Spacexzm] [Canotf] [Potuo] [Zxiaosi] [Xierkz] # Aestate
 Development Team
```

### Comparing `Aestate-1.0.8a1/aestate/ajson/ajson.py` & `Aestate-1.0.9/aestate/ajson/ajson.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/base/anno.py` & `Aestate-1.0.9/aestate/base/anno.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/base/manage.py` & `Aestate-1.0.9/aestate/base/manage.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/base/model.py` & `Aestate-1.0.9/aestate/base/model.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/base/proxy.py` & `Aestate-1.0.9/aestate/base/proxy.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/dbs/_mssql/__init__.py` & `Aestate-1.0.9/aestate/dbs/_mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/dbs/_mysql/__init__.py` & `Aestate-1.0.9/aestate/dbs/_mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/dbs/_mysql/tag.py` & `Aestate-1.0.9/aestate/dbs/_mysql/tag.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/exception/__init__.py` & `Aestate-1.0.9/aestate/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/i18n/__init__.py` & `Aestate-1.0.9/aestate/i18n/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -88,23 +88,21 @@
 
     def __init__(self):
         super(InfoI18n, self).__init__(langs={
             # 中文(简体,中国)
             0x804: {
                 "statement": "执行语句",
                 "parameters": "参数",
-                "cacheResult": "缓存结果",
-                "selectResult": "查询结果",
+                "selectResult": "行数",
                 "updateResult": "受影响行",
             },
             0x409: {
                 "statement": "Statement",
                 "parameters": "Parameters",
-                "cacheResult": "Cache Result",
-                "selectResult": "Select Result",
-                "updateResult": "Update Row",
+                "selectResult": "Total",
+                "updateResult": "Updates",
             }
         })
 
     @staticmethod
     def tt(name):
         return InfoI18n().t(name)
```

### Comparing `Aestate-1.0.8a1/aestate/util/CompulsoryRun.py` & `Aestate-1.0.9/aestate/util/CompulsoryRun.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/util/Log.py` & `Aestate-1.0.9/aestate/util/Log.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,35 +160,45 @@
         try:
             if obj is not None:
                 write_repr = others.fullname(obj)
             else:
                 write_repr = 'OBJECT IS NULL'
         except TypeError:
             write_repr = 'OBJECT CAN`T NOT PARSE'
+        # 时间
         t = datetime.datetime.utcnow().strftime('%Y-%m-%d %H:%M:%S.%f')
+        # 只输出文本
         pure_text = ' '.join([str(t), str(field.value), str(line), str(hex(id(obj))),
                               '[{}]'.format(task_name), str(write_repr), f" : {msg}"])
+
         t = ConsoleWrite.format_color(f"{t}".ljust(FieldsLength.DATETIME_FORMAT), ConsoleColor.FontColor.CYAN)
+        # 执行类型
         _field = ConsoleWrite.format_color(f"{field.value}".rjust(FieldsLength.INFO_FORMAT),
                                            ConsoleColor.FontColor.GREEN
                                            if field == LogStatus.Info
                                            else ConsoleColor.FontColor.RED
                                            if field == LogStatus.Error
                                            else ConsoleColor.FontColor.YELLOW
                                            if field == LogStatus.Warn
                                            else ConsoleColor.FontColor.YELLOW)
+        # 所在行数
         line = f"{line}".rjust(FieldsLength.LINE_FORMAT)
-        hex_id = ConsoleWrite.format_color(f" {str(hex(id(obj)))}", ConsoleColor.FontColor.PINK)
+        # 执行的类ID
+        hex_id = ConsoleWrite.format_color(f" {str(hex(id(obj))).upper()}", ConsoleColor.FontColor.PINK)
+        # 执行类型名称
         task_name = ConsoleWrite.format_color(f"{task_name}".rjust(FieldsLength.TASK_FORMAT),
                                               ConsoleColor.FontColor.PURPLE)
+        # 类
         write_repr = ConsoleWrite.format_color(write_repr,
                                                ConsoleColor.FontColor.LIGHT_GREEN
                                                if field != LogStatus.Error
                                                else ConsoleColor.FontColor.RED)
+        # 格式化消息颜色
         msg = ConsoleWrite.format_color(f" : {msg}", text_color)
+        # 组合消息
         info = "{}{}{}{}{}{}{}".format(t, _field, line, hex_id, ' [{}] '.format(task_name), write_repr, msg)
         if ned_text:
             return info, pure_text
         return info
 
     @staticmethod
     def log(msg, obj=None, line=sys._getframe().f_back.f_lineno, task_name='TEXT', LogObject=None,
@@ -365,8 +375,18 @@
         return instance
 
 
 class logging(object):
 
     @classmethod
     def gen(cls, _object) -> ALog:
+        """
+        使用实例化后的对象获取log日志对象
+        """
         return _object.log_obj
+
+    @classmethod
+    def gen_cls(cls, _class) -> ALog:
+        """
+        使用类获取log日志对象
+        """
+        return _class().log_obj
```

### Comparing `Aestate-1.0.8a1/aestate/util/others.py` & `Aestate-1.0.9/aestate/util/others.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/util/sqlOpera.py` & `Aestate-1.0.9/aestate/util/sqlOpera.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/work/Adapter.py` & `Aestate-1.0.9/aestate/work/Adapter.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/work/Annotation.py` & `Aestate-1.0.9/aestate/work/Annotation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import re
+
 from .AopContainer import AopModelObject
 from .Modes import EX_MODEL
 from .Serialize import QuerySet
 import os
 import inspect
 
 from .xmlhandler.nodes import ResultMapNode
@@ -64,41 +66,41 @@
 
         return _wrapper_
 
     return base_func
 
 
 def SelectAbst():
-    def mysql_rp(n, array) -> str:
+    def mysql_rp(n, array, obj) -> str:
         _name = array[len(array) - 1] if len(array) > 0 else ""
         rule = {
             'F': 'FROM',
             'find': "SELECT",
             'where': 'WHERE',
             'eq': "= #{%s}" % _name,
             'lt': '< #{%s}' % _name,
             'gt': '> #{%s}' % _name,
             'le': '<= #{%s}' % _name,
             'ge': '>= #{%s}' % _name,
             'in': 'in #{%s}' % _name,
             'like': 'like #{%s}' % _name,
-            'all': '*',
+            'all': ','.join([obj.orm.ParseUtil.parse_key(f) for f in obj.fields]),
         }
         return rule[n] if n in rule.keys() else n
 
     def base_func(func):
         def _wrapper_(*args, **kwargs):
             lines = list(args)
             if len(lines) == 0 and hasattr(func, 'instance') and not func.instance:
                 ALog.log_error(ExceptionI18n.tt(""))
             obj = lines[0]
             _name = func.__name__.split("_")
             S = []
             for i in _name:
-                d = mysql_rp(i, S)
+                d = mysql_rp(i, S, obj)
                 S.append(d if d != "FROM" else f"FROM {obj.__table_name__}")
 
             sql = ' '.join(S)
 
             # 查找参数
             sub_sql, new_args = TextUtil.replace_antlr(sql, **kwargs)
 
@@ -221,18 +223,17 @@
     return base_func
 
 
 def ReadXml(filename):
     """读取xml"""
 
     def set_to_field(cls):
-        sep = os.sep
-
         file_path = inspect.getfile(cls)
-        file_path = file_path[:file_path.rfind(sep)]
+        # 分割字符串得到当前路径
+        file_path = '/'.join(re.split(r'[/|\\]', file_path)[:-1])
         path = os.path.join(file_path, filename)
 
         setattr(cls, '_xml_file', path)
         xml = AestateXml.read_file(path)
         setattr(cls, 'xNode', xml)
         setattr(cls, '_xml_file_name', os.path.basename(path))
         return cls
```

### Comparing `Aestate-1.0.8a1/aestate/work/AopContainer.py` & `Aestate-1.0.9/aestate/work/AopContainer.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/work/Config.py` & `Aestate-1.0.9/aestate/work/Config.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/work/Manage.py` & `Aestate-1.0.9/aestate/work/Manage.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/work/Modes.py` & `Aestate-1.0.9/aestate/work/Modes.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/work/Serialize.py` & `Aestate-1.0.9/aestate/work/Serialize.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/work/commands/__init__.py` & `Aestate-1.0.9/aestate/work/commands/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- utf-8 -*-
 # encoding:utf-8
 # @Time: 2021/6/27 20:47
 # @Author: CACode
 # 版本有三种状态 正式版从1.0.0往后逐个加 1,对应版本的补丁为'a+补丁次数'
-__version__ = '1.0.8a1'
+__version__ = '1.0.9'
 __description__ = "Aestate framework for Python,You can see:https://gitee.com/aecode/aestate"
 __author__ = "CACode"
 __author_email__ = "cacode@163.com"
 __url__ = "https://gitee.com/aecode/aestate"
 __issues__ = 'https://gitee.com/aecode/aestate/issues'
 __license__ = 'Apache License 2.0'
 __project_name__ = 'Aestate'
```

### Comparing `Aestate-1.0.8a1/aestate/work/orm.py` & `Aestate-1.0.9/aestate/work/orm.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,15 @@
         查
         example:
             find('all')
             find('param1',asses=['p'],h_func=True)
         Attributes:
             asses:将对应的字段转成另一个别名,不需要转换的使用None标识
             h_func:不将字段转换成 `%s` 格式
+            poly:是否要在末尾加上[from table_name]，常用于使用加号连表时
         更新:
             如果args字段长度为0,默认为查找全部
         """
         self.exmode = AOrm.Mode.FIND
         self.args.append(self.sqlFields.find_str)
         # 如果有as字段
         alias = None
```

### Comparing `Aestate-1.0.8a1/aestate/work/proxy/SqlOperaProxy.py` & `Aestate-1.0.9/aestate/work/proxy/SqlOperaProxy.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/work/repository.py` & `Aestate-1.0.9/aestate/work/repository.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/work/sql/ExecuteSql.py` & `Aestate-1.0.9/aestate/work/sql/ExecuteSql.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import re
 import sys
 
 from aestate.exception import BaseSqlError
 from aestate.i18n import InfoI18n
 from aestate.util.Log import ALog
 from dbutils.pooled_db import PooledDB
-from aestate.work.Cache import SqlCacheManage, CacheStatus
 
 
 def parse_kwa(db, **kwargs):
     """
     解析并执行sql
 
     :param db:db_util对象
@@ -88,39 +87,27 @@
             params:需要填充的字段
             print_sql:是否打印sql语句
         :return:
         """
         db = self.get_conn()
         _l = sys._getframe().f_back.f_lineno
         try:
-            cursor = db.cursor()
-            sql = cursor.mogrify(kwargs['sql'], tuple(kwargs['params']) if 'params' in kwargs.keys() and kwargs[
-                'params'] else ())
-            # 判断和获取缓存
-            scm = SqlCacheManage()
-            if scm.status == CacheStatus.OPEN:
-                if sql in scm:
-                    values = scm.get(sql).get_value()
-                    msg = InfoI18n.tt("cacheResult") + ' ==> ' + (str(len(values)) if values is not None else '0')
-                    ALog.log(obj=db, line=_l, task_name='ASQL', msg=msg,
-                             LogObject=kwargs['log_obj'] if 'log_obj' in kwargs.keys() else None)
-                    return values
             cursor = parse_kwa(db=db, **kwargs)
             # 列名
             col = cursor.description
             data = cursor.fetchall()
             _result = []
             for data_index, data_value in enumerate(data):
                 _messy = {}
                 for item_index, item_value in enumerate(data_value):
                     _messy[col[item_index][0]] = item_value
                 _result.append(_messy)
             # 缓存
-            if scm.status == CacheStatus.OPEN:
-                scm.set(sql=sql, value=_result, instance=kwargs['instance'] if 'instance' in kwargs.keys() else None)
+            # if scm.status == CacheStatus.OPEN:
+            #     scm.set(sql=sql, value=_result, instance=kwargs['instance'] if 'instance' in kwargs.keys() else None)
 
             msg = InfoI18n.tt("selectResult") + ' ==> ' + (str(len(_result)) if _result is not None else '0')
             ALog.log(obj=db, line=_l, task_name='ASQL', msg=msg,
                      LogObject=kwargs['log_obj'] if 'log_obj' in kwargs.keys() else None)
             db.close()
             return _result
         except Exception as e:
@@ -139,16 +126,14 @@
             sql:处理过并加上%s的sql语句
             params:需要填充的字段
         :param many:是否为多行执行
         """
         db = self.get_conn()
         _l = sys._getframe().f_back.f_lineno
         try:
-            scm = SqlCacheManage()
-            scm.remove_by_instance(kwargs['instance'].get_tb_name() if 'instance' in kwargs.keys() else None)
             cursor = parse_kwa(db=db, many=many, **kwargs)
             db.commit()
             # 受影响行数
             rowcount = cursor.rowcount
             msg = InfoI18n.tt("updateResult") + ' ==> ' + str(rowcount)
             ALog.log(obj=db, line=_l, task_name='ASQL', msg=msg,
                      LogObject=kwargs['log_obj'] if 'log_obj' in kwargs.keys() else None)
```

### Comparing `Aestate-1.0.8a1/aestate/work/sql/ProxyOpera.py` & `Aestate-1.0.9/aestate/work/sql/ProxyOpera.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/work/xmlhandler/XMLScriptBuilder.py` & `Aestate-1.0.9/aestate/work/xmlhandler/XMLScriptBuilder.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/work/xmlhandler/base.py` & `Aestate-1.0.9/aestate/work/xmlhandler/base.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/work/xmlhandler/nodes.py` & `Aestate-1.0.9/aestate/work/xmlhandler/nodes.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/aestate/work/xmlhandler/utils.py` & `Aestate-1.0.9/aestate/work/xmlhandler/utils.py`

 * *Files identical despite different names*

### Comparing `Aestate-1.0.8a1/setup.py` & `Aestate-1.0.9/setup.py`

 * *Files identical despite different names*

