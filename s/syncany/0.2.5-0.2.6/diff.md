# Comparing `tmp/syncany-0.2.5.tar.gz` & `tmp/syncany-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncany-0.2.5.tar", last modified: Thu Apr 20 08:44:39 2023, max compression
+gzip compressed data, was "syncany-0.2.6.tar", last modified: Tue Apr 25 09:43:43 2023, max compression
```

## Comparing `syncany-0.2.5.tar` & `syncany-0.2.6.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:39.483163 syncany-0.2.5/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2022-08-13 12:36:15.000000 syncany-0.2.5/LICENSE
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7103 2023-04-20 08:44:39.484190 syncany-0.2.5/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5832 2022-08-13 12:36:15.000000 syncany-0.2.5/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-04-20 08:44:39.494187 syncany-0.2.5/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1928 2023-04-20 03:39:41.000000 syncany-0.2.5/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:34.324661 syncany-0.2.5/syncany/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      607 2023-04-20 03:39:41.000000 syncany-0.2.5/syncany/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:35.054704 syncany-0.2.5/syncany/calculaters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3587 2023-04-20 05:48:06.000000 syncany-0.2.5/syncany/calculaters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    39302 2023-04-19 07:06:22.000000 syncany-0.2.5/syncany/calculaters/builtin.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4394 2023-03-24 09:30:00.000000 syncany-0.2.5/syncany/calculaters/calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7999 2023-03-27 08:30:23.000000 syncany-0.2.5/syncany/calculaters/convert_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4573 2023-03-23 03:10:08.000000 syncany-0.2.5/syncany/calculaters/datetime_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2255 2023-03-23 03:10:08.000000 syncany-0.2.5/syncany/calculaters/import_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3167 2023-03-23 03:10:08.000000 syncany-0.2.5/syncany/calculaters/textline_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    13697 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/calculaters/transform_calculater.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:36.043453 syncany-0.2.5/syncany/database/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4055 2023-03-28 03:25:41.000000 syncany-0.2.5/syncany/database/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8756 2023-03-24 06:27:35.000000 syncany-0.2.5/syncany/database/beanstalk.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    15303 2023-02-24 09:40:27.000000 syncany-0.2.5/syncany/database/clickhouse.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    15571 2023-03-25 11:28:20.000000 syncany-0.2.5/syncany/database/csv.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    10626 2023-02-23 11:47:13.000000 syncany-0.2.5/syncany/database/database.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12481 2023-02-24 09:33:28.000000 syncany-0.2.5/syncany/database/elasticsearch.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14331 2023-03-24 06:27:35.000000 syncany-0.2.5/syncany/database/excel.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14218 2023-02-22 05:00:17.000000 syncany-0.2.5/syncany/database/http.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    17931 2023-02-24 09:33:28.000000 syncany-0.2.5/syncany/database/influxdb.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    11892 2023-03-24 06:27:35.000000 syncany-0.2.5/syncany/database/json.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    11786 2023-03-24 06:27:35.000000 syncany-0.2.5/syncany/database/memory.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14344 2023-02-24 09:35:33.000000 syncany-0.2.5/syncany/database/mongodb.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14437 2023-02-24 09:28:32.000000 syncany-0.2.5/syncany/database/mysql.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14572 2023-02-24 09:33:28.000000 syncany-0.2.5/syncany/database/postgresql.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    17848 2023-03-24 06:27:35.000000 syncany-0.2.5/syncany/database/redis.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    13949 2023-03-28 03:39:46.000000 syncany-0.2.5/syncany/database/sqlite.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    15203 2023-02-24 09:28:33.000000 syncany-0.2.5/syncany/database/sqlserver.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    17813 2023-03-25 11:15:36.000000 syncany-0.2.5/syncany/database/textline.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      685 2022-08-23 12:03:29.000000 syncany-0.2.5/syncany/errors.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:36.216452 syncany-0.2.5/syncany/filters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      996 2023-03-25 04:34:57.000000 syncany-0.2.5/syncany/filters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    19439 2023-04-01 08:20:13.000000 syncany-0.2.5/syncany/filters/builtin.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      309 2022-08-13 12:36:15.000000 syncany-0.2.5/syncany/filters/filter.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1957 2023-02-16 02:10:09.000000 syncany-0.2.5/syncany/hook.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:36.590473 syncany-0.2.5/syncany/loaders/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      927 2023-03-25 04:34:57.000000 syncany-0.2.5/syncany/loaders/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1401 2023-02-10 08:39:32.000000 syncany-0.2.5/syncany/loaders/cache.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1148 2023-03-21 06:16:11.000000 syncany-0.2.5/syncany/loaders/const.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6106 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/loaders/db.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     9117 2023-03-30 02:17:02.000000 syncany-0.2.5/syncany/loaders/db_join.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1752 2023-02-24 04:31:16.000000 syncany-0.2.5/syncany/loaders/db_pull.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8751 2023-04-20 05:37:24.000000 syncany-0.2.5/syncany/loaders/loader.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      214 2022-08-13 12:36:15.000000 syncany-0.2.5/syncany/logger.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    13966 2023-03-24 04:36:02.000000 syncany-0.2.5/syncany/main.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:36.977243 syncany-0.2.5/syncany/outputers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1161 2023-03-25 04:34:57.000000 syncany-0.2.5/syncany/outputers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1491 2023-02-24 04:31:16.000000 syncany-0.2.5/syncany/outputers/db.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1920 2023-02-15 06:50:55.000000 syncany-0.2.5/syncany/outputers/db_delete_insert.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      887 2022-08-13 12:36:15.000000 syncany-0.2.5/syncany/outputers/db_insert.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5697 2023-03-18 13:41:32.000000 syncany-0.2.5/syncany/outputers/db_update_delete_insert.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4209 2023-03-18 13:41:32.000000 syncany-0.2.5/syncany/outputers/db_update_insert.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2864 2023-03-22 02:35:53.000000 syncany-0.2.5/syncany/outputers/outputer.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:37.258948 syncany-0.2.5/syncany/taskers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       52 2022-08-13 12:36:15.000000 syncany-0.2.5/syncany/taskers/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:37.716628 syncany-0.2.5/syncany/taskers/config/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1794 2023-03-25 04:34:57.000000 syncany-0.2.5/syncany/taskers/config/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      405 2022-08-23 12:07:09.000000 syncany-0.2.5/syncany/taskers/config/file_reader.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      937 2022-08-23 12:07:09.000000 syncany-0.2.5/syncany/taskers/config/http_reader.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      195 2022-08-13 12:36:15.000000 syncany-0.2.5/syncany/taskers/config/json_parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      208 2022-08-13 12:36:15.000000 syncany-0.2.5/syncany/taskers/config/parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      204 2022-08-23 11:55:44.000000 syncany-0.2.5/syncany/taskers/config/reader.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5006 2022-08-13 12:36:15.000000 syncany-0.2.5/syncany/taskers/config/yaml_parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1377 2023-02-24 02:44:01.000000 syncany-0.2.5/syncany/taskers/context.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:38.185759 syncany-0.2.5/syncany/taskers/core/
--rwxrwxrwx   0 snower    (1000) snower    (1000)    72944 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/taskers/core/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2192 2023-03-21 06:17:51.000000 syncany-0.2.5/syncany/taskers/core/loader_creater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      256 2022-08-13 12:36:15.000000 syncany-0.2.5/syncany/taskers/core/option.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2592 2023-02-10 08:39:32.000000 syncany-0.2.5/syncany/taskers/core/outputer_creater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4736 2022-08-13 12:36:15.000000 syncany-0.2.5/syncany/taskers/core/states.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    15689 2023-02-25 11:47:43.000000 syncany-0.2.5/syncany/taskers/core/valuer_compiler.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    40757 2023-03-24 06:10:54.000000 syncany-0.2.5/syncany/taskers/core/valuer_creater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      760 2023-02-25 12:43:51.000000 syncany-0.2.5/syncany/taskers/iterator.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      245 2022-08-13 12:36:15.000000 syncany-0.2.5/syncany/taskers/manager.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7122 2023-04-20 05:48:37.000000 syncany-0.2.5/syncany/taskers/tasker.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    11025 2023-04-20 03:35:47.000000 syncany-0.2.5/syncany/utils.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:39.439949 syncany-0.2.5/syncany/valuers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2098 2023-03-25 04:34:57.000000 syncany-0.2.5/syncany/valuers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4574 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/aggregate.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3714 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/assign.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5209 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/cache.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3956 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/calculate.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6445 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/call.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5526 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/case.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4729 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/condition.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      548 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/const.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2965 2023-03-30 01:52:08.000000 syncany-0.2.5/syncany/valuers/data.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5059 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/db_join.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2043 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/db_load.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1877 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/function.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6018 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/generator.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3468 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/inherit.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3379 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/let.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12327 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/loop.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7510 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/make.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    10283 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/match.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1247 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/schema.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4336 2023-03-29 08:52:57.000000 syncany-0.2.5/syncany/valuers/state.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6066 2023-03-30 01:52:08.000000 syncany-0.2.5/syncany/valuers/valuer.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-20 08:44:34.591915 syncany-0.2.5/syncany.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7103 2023-04-20 08:44:32.000000 syncany-0.2.5/syncany.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2889 2023-04-20 08:44:33.000000 syncany-0.2.5/syncany.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-20 08:44:32.000000 syncany-0.2.5/syncany.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       47 2023-04-20 08:44:32.000000 syncany-0.2.5/syncany.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2022-08-15 03:43:33.000000 syncany-0.2.5/syncany.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      371 2023-04-20 08:44:32.000000 syncany-0.2.5/syncany.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        8 2023-04-20 08:44:32.000000 syncany-0.2.5/syncany.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:43.802862 syncany-0.2.6/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2022-08-13 12:36:15.000000 syncany-0.2.6/LICENSE
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7103 2023-04-25 09:43:43.804884 syncany-0.2.6/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5832 2022-08-13 12:36:15.000000 syncany-0.2.6/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-04-25 09:43:43.814860 syncany-0.2.6/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1928 2023-04-21 09:56:25.000000 syncany-0.2.6/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:38.384634 syncany-0.2.6/syncany/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      607 2023-04-21 09:56:25.000000 syncany-0.2.6/syncany/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:39.166440 syncany-0.2.6/syncany/calculaters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4962 2023-04-25 03:51:51.000000 syncany-0.2.6/syncany/calculaters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    39302 2023-04-19 07:06:22.000000 syncany-0.2.6/syncany/calculaters/builtin.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4394 2023-03-24 09:30:00.000000 syncany-0.2.6/syncany/calculaters/calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7999 2023-03-27 08:30:23.000000 syncany-0.2.6/syncany/calculaters/convert_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4573 2023-03-23 03:10:08.000000 syncany-0.2.6/syncany/calculaters/datetime_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2328 2023-04-25 04:06:56.000000 syncany-0.2.6/syncany/calculaters/import_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3167 2023-03-23 03:10:08.000000 syncany-0.2.6/syncany/calculaters/textline_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    13907 2023-04-21 10:27:56.000000 syncany-0.2.6/syncany/calculaters/transform_calculater.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:40.173724 syncany-0.2.6/syncany/database/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5187 2023-04-25 03:51:51.000000 syncany-0.2.6/syncany/database/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8756 2023-03-24 06:27:35.000000 syncany-0.2.6/syncany/database/beanstalk.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    15594 2023-04-25 03:41:03.000000 syncany-0.2.6/syncany/database/clickhouse.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    15749 2023-04-25 02:15:32.000000 syncany-0.2.6/syncany/database/csv.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    10626 2023-02-23 11:47:13.000000 syncany-0.2.6/syncany/database/database.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12481 2023-02-24 09:33:28.000000 syncany-0.2.6/syncany/database/elasticsearch.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14490 2023-04-25 02:15:32.000000 syncany-0.2.6/syncany/database/excel.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14218 2023-02-22 05:00:17.000000 syncany-0.2.6/syncany/database/http.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    17931 2023-02-24 09:33:28.000000 syncany-0.2.6/syncany/database/influxdb.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12051 2023-04-25 02:15:32.000000 syncany-0.2.6/syncany/database/json.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    11954 2023-04-25 02:15:32.000000 syncany-0.2.6/syncany/database/memory.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14642 2023-04-25 03:15:38.000000 syncany-0.2.6/syncany/database/mongodb.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14723 2023-04-25 03:35:50.000000 syncany-0.2.6/syncany/database/mysql.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14858 2023-04-25 03:37:13.000000 syncany-0.2.6/syncany/database/postgresql.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    18023 2023-04-25 02:22:52.000000 syncany-0.2.6/syncany/database/redis.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    13949 2023-03-28 03:39:46.000000 syncany-0.2.6/syncany/database/sqlite.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    15489 2023-04-25 03:39:10.000000 syncany-0.2.6/syncany/database/sqlserver.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    17928 2023-04-23 08:27:57.000000 syncany-0.2.6/syncany/database/textline.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      685 2022-08-23 12:03:29.000000 syncany-0.2.6/syncany/errors.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:40.338267 syncany-0.2.6/syncany/filters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2275 2023-04-25 03:51:51.000000 syncany-0.2.6/syncany/filters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    19439 2023-04-01 08:20:13.000000 syncany-0.2.6/syncany/filters/builtin.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      309 2022-08-13 12:36:15.000000 syncany-0.2.6/syncany/filters/filter.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1957 2023-02-16 02:10:09.000000 syncany-0.2.6/syncany/hook.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:40.738422 syncany-0.2.6/syncany/loaders/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      927 2023-03-25 04:34:57.000000 syncany-0.2.6/syncany/loaders/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1401 2023-02-10 08:39:32.000000 syncany-0.2.6/syncany/loaders/cache.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1148 2023-03-21 06:16:11.000000 syncany-0.2.6/syncany/loaders/const.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6106 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/loaders/db.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     9117 2023-03-30 02:17:02.000000 syncany-0.2.6/syncany/loaders/db_join.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1752 2023-02-24 04:31:16.000000 syncany-0.2.6/syncany/loaders/db_pull.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8751 2023-04-20 05:37:24.000000 syncany-0.2.6/syncany/loaders/loader.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      214 2022-08-13 12:36:15.000000 syncany-0.2.6/syncany/logger.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    13966 2023-03-24 04:36:02.000000 syncany-0.2.6/syncany/main.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:41.161332 syncany-0.2.6/syncany/outputers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1161 2023-03-25 04:34:57.000000 syncany-0.2.6/syncany/outputers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1491 2023-02-24 04:31:16.000000 syncany-0.2.6/syncany/outputers/db.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1962 2023-04-25 03:15:38.000000 syncany-0.2.6/syncany/outputers/db_delete_insert.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      932 2023-04-25 03:15:38.000000 syncany-0.2.6/syncany/outputers/db_insert.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5697 2023-04-25 03:15:38.000000 syncany-0.2.6/syncany/outputers/db_update_delete_insert.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4210 2023-04-25 03:15:38.000000 syncany-0.2.6/syncany/outputers/db_update_insert.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2864 2023-03-22 02:35:53.000000 syncany-0.2.6/syncany/outputers/outputer.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:41.439635 syncany-0.2.6/syncany/taskers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       52 2022-08-13 12:36:15.000000 syncany-0.2.6/syncany/taskers/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:41.936438 syncany-0.2.6/syncany/taskers/config/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1794 2023-03-25 04:34:57.000000 syncany-0.2.6/syncany/taskers/config/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      405 2022-08-23 12:07:09.000000 syncany-0.2.6/syncany/taskers/config/file_reader.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      937 2022-08-23 12:07:09.000000 syncany-0.2.6/syncany/taskers/config/http_reader.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      195 2022-08-13 12:36:15.000000 syncany-0.2.6/syncany/taskers/config/json_parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      208 2022-08-13 12:36:15.000000 syncany-0.2.6/syncany/taskers/config/parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      204 2022-08-23 11:55:44.000000 syncany-0.2.6/syncany/taskers/config/reader.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5006 2022-08-13 12:36:15.000000 syncany-0.2.6/syncany/taskers/config/yaml_parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1377 2023-02-24 02:44:01.000000 syncany-0.2.6/syncany/taskers/context.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:42.425049 syncany-0.2.6/syncany/taskers/core/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    73072 2023-04-25 04:03:27.000000 syncany-0.2.6/syncany/taskers/core/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2192 2023-03-21 06:17:51.000000 syncany-0.2.6/syncany/taskers/core/loader_creater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      256 2022-08-13 12:36:15.000000 syncany-0.2.6/syncany/taskers/core/option.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2592 2023-02-10 08:39:32.000000 syncany-0.2.6/syncany/taskers/core/outputer_creater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4736 2022-08-13 12:36:15.000000 syncany-0.2.6/syncany/taskers/core/states.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    15689 2023-02-25 11:47:43.000000 syncany-0.2.6/syncany/taskers/core/valuer_compiler.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    40757 2023-03-24 06:10:54.000000 syncany-0.2.6/syncany/taskers/core/valuer_creater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      760 2023-02-25 12:43:51.000000 syncany-0.2.6/syncany/taskers/iterator.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      245 2022-08-13 12:36:15.000000 syncany-0.2.6/syncany/taskers/manager.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7122 2023-04-20 05:48:37.000000 syncany-0.2.6/syncany/taskers/tasker.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    11025 2023-04-20 03:35:47.000000 syncany-0.2.6/syncany/utils.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:43.748890 syncany-0.2.6/syncany/valuers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2098 2023-03-25 04:34:57.000000 syncany-0.2.6/syncany/valuers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4574 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/aggregate.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3714 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/assign.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5209 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/cache.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3956 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/calculate.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6445 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/call.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5526 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/case.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4729 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/condition.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      548 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/const.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2965 2023-03-30 01:52:08.000000 syncany-0.2.6/syncany/valuers/data.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5059 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/db_join.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2043 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/db_load.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1877 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/function.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6018 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/generator.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3468 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/inherit.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3379 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/let.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12327 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/loop.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7510 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/make.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    10283 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/match.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1247 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/schema.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4336 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/state.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6066 2023-03-30 01:52:08.000000 syncany-0.2.6/syncany/valuers/valuer.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:38.687664 syncany-0.2.6/syncany.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7103 2023-04-25 09:43:35.000000 syncany-0.2.6/syncany.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2889 2023-04-25 09:43:37.000000 syncany-0.2.6/syncany.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 09:43:35.000000 syncany-0.2.6/syncany.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       47 2023-04-25 09:43:36.000000 syncany-0.2.6/syncany.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2022-08-15 03:43:33.000000 syncany-0.2.6/syncany.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      371 2023-04-25 09:43:36.000000 syncany-0.2.6/syncany.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        8 2023-04-25 09:43:36.000000 syncany-0.2.6/syncany.egg-info/top_level.txt
```

### Comparing `syncany-0.2.5/LICENSE` & `syncany-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/PKG-INFO` & `syncany-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncany
-Version: 0.2.5
+Version: 0.2.6
 Summary: 简单易用的数据同步转换导出框架
 Home-page: https://github.com/snower/syncany
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # syncany
```

### Comparing `syncany-0.2.5/README.md` & `syncany-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/setup.py` & `syncany-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 18/8/6
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.2.5"
+version = "0.2.6"
 
 if os.path.exists("README.md"):
     if sys.version_info[0] >= 3:
         try:
             with open("README.md", encoding="utf-8") as fp:
                 long_description = fp.read()
         except Exception as e:
```

### Comparing `syncany-0.2.5/syncany/__init__.py` & `syncany-0.2.6/syncany/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # 18/8/6
 # create by: snower
 
-version = "0.2.5"
-version_info = (0, 2, 5)
+version = "0.2.6"
+version_info = (0, 2, 6)
 
 from .loaders import Loader, register_loader
 from .outputers import Outputer, register_outputer
 from .valuers import Valuer, register_valuer
 from .filters import Filter, register_filter
 from .database import DataBase, register_database
 from .calculaters import Calculater, TypeFormatCalculater, TypingCalculater, MathematicalCalculater, \
```

### Comparing `syncany-0.2.5/syncany/calculaters/builtin.py` & `syncany-0.2.6/syncany/calculaters/builtin.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/calculaters/calculater.py` & `syncany-0.2.6/syncany/calculaters/calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/calculaters/convert_calculater.py` & `syncany-0.2.6/syncany/calculaters/convert_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/calculaters/datetime_calculater.py` & `syncany-0.2.6/syncany/calculaters/datetime_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/calculaters/import_calculater.py` & `syncany-0.2.6/syncany/calculaters/import_calculater.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,16 @@
             attr_names = calculate_name.split(".")
             module_or_func = self._import_module
             for attr_name in attr_names:
                 if not hasattr(module_or_func, attr_name):
                     raise NotImplementedError("%s not implemented %s" % (self._import_module, calculate_name))
                 module_or_func = getattr(module_or_func, attr_name)
             if not callable(module_or_func):
+                if not args:
+                    return module_or_func
                 raise NotImplementedError("%s not callable %s" % (self._import_module, calculate_name))
         else:
             calculate_name = self.name
             if not callable(self._import_module):
                 raise NotImplementedError("%s not callable %s" % (self._import_module, self.name))
             module_or_func = self._import_module
```

### Comparing `syncany-0.2.5/syncany/calculaters/textline_calculater.py` & `syncany-0.2.6/syncany/calculaters/textline_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/calculaters/transform_calculater.py` & `syncany-0.2.6/syncany/calculaters/transform_calculater.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 class TransformCalculater(Calculater):
     def update_outputer_schema(self, keys):
         from ..taskers.tasker import current_tasker
         tasker = current_tasker()
         tasker.outputer.schema = {}
         for key in keys:
+            if not isinstance(key, str):
+                continue
             valuer = tasker.create_valuer(tasker.valuer_compiler.compile_data_valuer(key, None))
             if not valuer:
                 continue
             tasker.outputer.add_valuer(key, valuer)
 
 
 class TransformV4HCalculater(TransformCalculater):
@@ -48,15 +50,15 @@
             return []
 
         datas = args[0] if isinstance(args[0], list) else \
             ([args[0]] if isinstance(args[0], dict) else [])
         key, vkey = args[1], args[2]
         reserved_keys = [key, vkey]
         if len(args) >= 4:
-            reserved_keys.extend(list(set(args[3])) if isinstance(args[3], list) else [args[3]])
+            reserved_keys.extend(list({str(k) for k in args[3]}) if isinstance(args[3], list) else [str(args[3])])
         result, reserved_data = [], {key: None, vkey: None}
         for data in datas:
             for k, v in data.items():
                 if k not in reserved_keys:
                     continue
                 reserved_data[k] = v
             for k, v in data.items():
@@ -119,15 +121,15 @@
             hvalue, vvalue, vivalue = data[vhkey], (vvkey(data) if vvkey_callable else data[vvkey]), (data[vikey] if vikey in data else None)
             if (ivalue is None and rdata is None) or hvalue in rdata or (vikey is not None and vivalue != ivalue):
                 if rdata is not None:
                     result.append(rdata)
                 ivalue, rdata = vivalue, ({} if vikey is None else {vikey: vivalue})
             rdata[hvalue] = vvalue
             if hvalue not in vkeys:
-                vkeys.append(hvalue)
+                vkeys.append(str(hvalue))
         if rdata:
             result.append(rdata)
 
         self.update_outputer_schema(vkeys)
         return result
 
 
@@ -205,15 +207,15 @@
 
         result = []
         for vkey in vkeys:
             data = {vvkey: vkey}
             for hkey in hkeys:
                 data[hkey] = mdata[hkey][vkey] if hkey in mdata and vkey in mdata[hkey] else 0
             result.append(data)
-        self.update_outputer_schema([vvkey] + list(hkeys.keys()))
+        self.update_outputer_schema([str(vvkey)] + [str(hkey) for hkey in hkeys.keys()])
         return result
 
 
 class TransformH2VCalculater(TransformCalculater):
     """
     横向表转为纵向表
         参数1：横向表头
@@ -254,15 +256,15 @@
             for k, v in data.items():
                 if k == vkey:
                     continue
                 reserved_data[hkey] = k
                 if vvkey:
                     reserved_data[vvkey] = v
                 result.append(dict(**reserved_data))
-        self.update_outputer_schema(list(reserved_data.keys()))
+        self.update_outputer_schema([str(key) for key in reserved_data.keys()])
         return result
 
 
 class TransformUniqKVCalculater(TransformCalculater):
     """
     去重，重复行横向扩展
         参数1：重复字段key
@@ -305,38 +307,40 @@
                 for k in data:
                     if k in keys:
                         continue
                     keys.append(k)
                 uniq_datas[uvalue] = data
                 result.append(data)
 
-            uniq_data = uniq_datas[uvalue]
+            uniq_data, data_key = uniq_datas[uvalue], None
             if not vkey:
                 if kkey not in data:
                     continue
-                if data[kkey] not in uniq_data:
-                    uniq_data[data[kkey]] = 1
+                data_key = str(data[kkey])
+                if data_key not in uniq_data:
+                    uniq_data[data_key] = 1
                 else:
-                    uniq_data[data[kkey]] += 1
-                if data[kkey] not in keys:
-                    keys.append(data[kkey])
+                    uniq_data[data_key] += 1
+                if data_key not in keys:
+                    keys.append(data_key)
                 continue
 
             if kkey in data and vkey in data:
-                if data[vkey] is None and data[kkey] in uniq_data:
+                data_key = str(data[kkey])
+                if data[vkey] is None and data_key in uniq_data:
                     continue
                 if isinstance(data[vkey], (int, float)):
-                    if data[kkey] in uniq_data:
-                        uniq_data[data[kkey]] += data[vkey]
+                    if data_key in uniq_data:
+                        uniq_data[data_key] += data[vkey]
                     else:
-                        uniq_data[data[kkey]] = data[vkey]
+                        uniq_data[data_key] = data[vkey]
                 else:
-                    uniq_data[data[kkey]] = data[vkey]
-                if data[kkey] not in keys:
-                    keys.append(data[kkey])
+                    uniq_data[data_key] = data[vkey]
+                if data_key not in keys:
+                    keys.append(data_key)
 
         from ..taskers.tasker import current_tasker
         tasker = current_tasker()
         valuer = tasker.outputer.schema[vkey] if vkey else None
         for data in result:
             for key in keys:
                 if key in data:
```

### Comparing `syncany-0.2.5/syncany/database/__init__.py` & `syncany-0.2.6/syncany/database/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -*- coding: utf-8 -*-
 # 18/8/6
 # create by: snower
 
-from .database import DataBase
+import types
+from .database import DataBase, DatabaseFactory, DatabaseManager, DatabaseDriver, CacheBuilder, \
+    QueryBuilder, InsertBuilder, UpdateBuilder, DeleteBuilder
 from ..errors import DatabaseUnknownException
 
 DATABASES = {
     "memory": ".memory.MemoryDB",
     "textline": ".textline.TextLineDB",
     "mongo": ".mongodb.MongoDB",
     "mysql": ".mysql.MysqlDB",
@@ -69,18 +71,29 @@
             setattr(self.driver_instance, key, value)
 
     def build(self):
         if isinstance(DATABASES[self.driver_name], str):
             module_name, _, cls_name = DATABASES[self.driver_name].rpartition(".")
             if module_name[0] == ".":
                 module_name = module_name[1:]
-                module = __import__(module_name, globals(), globals(), [module_name], 1)
+                module = __import__(module_name, globals(), locals(), [module_name], 1)
+            elif "." in module_name:
+                from_module_name, _, module_name = module_name.rpartition(".")
+                module = __import__(from_module_name, globals(), locals(), [module_name])
             else:
-                module = __import__(module_name)
-            DATABASES[self.driver_name] = getattr(module, cls_name)
+                module = __import__(module_name, globals(), locals())
+            database_cls = getattr(module, cls_name)
+            if not isinstance(database_cls, type) or not issubclass(database_cls, DataBase):
+                raise TypeError("is not DataBase")
+            DATABASES[self.driver_name] = database_cls
+        elif isinstance(DATABASES[self.driver_name], (types.FunctionType, types.LambdaType)):
+            database_cls = DATABASES[self.driver_name]()
+            if not isinstance(database_cls, type) or not issubclass(database_cls, DataBase):
+                raise TypeError("is not DataBase")
+            DATABASES[self.driver_name] = database_cls
 
         if self.driver_instance is None:
             self.driver_instance = DATABASES[self.driver_name](self.manager, self.config)
             for key, value in self.update_attrs:
                 setattr(self.driver_instance, key, value)
         return self.driver_instance
 
@@ -99,17 +112,19 @@
         raise DatabaseUnknownException("%s is unknown database driver" % name)
     return DatabaseInstanceBuilder(name)
 
 
 def register_database(name, database=None):
     if database is None:
         def _(database):
-            if not issubclass(database, DataBase):
+            if not isinstance(database, str) and not callable(database) \
+                    and (not isinstance(database, type) or not issubclass(database, DataBase)):
                 raise TypeError("is not DataBase")
             DATABASES[name] = database
             return database
         return _
 
-    if not issubclass(database, DataBase):
+    if not isinstance(database, str) and not callable(database) \
+            and (not isinstance(database, type) or not issubclass(database, DataBase)):
         raise TypeError("is not DataBase")
     DATABASES[name] = database
     return database
```

### Comparing `syncany-0.2.5/syncany/database/beanstalk.py` & `syncany-0.2.6/syncany/database/beanstalk.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/database/clickhouse.py` & `syncany-0.2.6/syncany/database/clickhouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,15 +301,18 @@
     def filter_in(self, key, value):
         self.query.append('`' + key + "` in %s")
         self.query_values.append(value)
 
     def commit(self):
         db_name = self.name.split(".")
         db_name = ("`%s`.`%s`" % (self.db.db_name, ".".join(db_name[1:]))) if len(db_name) > 1 else ('`' + db_name[0] + '`')
-        sql = "ALTER TABLE %s DELETE WHERE %s" % (db_name, " AND ".join(self.query))
+        if not self.query and self.db.delete_all_truncate_table:
+            sql = "TRUNCATE TABLE %s" % db_name
+        else:
+            sql = "ALTER TABLE %s DELETE WHERE %s" % (db_name, " AND ".join(self.query))
         connection = self.db.ensure_connection()
         cursor = connection.cursor()
         try:
             cursor.execute(sql % self.db.escape_args(self.query_values))
         finally:
             cursor.close()
             self.db.release_connection()
@@ -358,14 +361,16 @@
     def __init__(self, manager, config):
         all_config = {}
         all_config.update(self.DEFAULT_CONFIG)
         all_config.update(config)
 
         self.db_name = all_config["database"] if "database" in all_config else all_config["name"]
         self.virtual_tables = all_config.pop("virtual_views") if "virtual_views" in all_config else []
+        self.delete_all_truncate_table = all_config.pop("delete_all_truncate_table") \
+            if "delete_all_truncate_table" in all_config else False
 
         super(ClickhouseDB, self).__init__(manager, all_config)
 
     def build_factory(self):
         try:
             from clickhouse_driver.util.escape import escape_param
         except ImportError:
```

### Comparing `syncany-0.2.5/syncany/database/csv.py` & `syncany-0.2.6/syncany/database/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                 datas.append(data)
                 if limit > 0 and len(datas) >= limit:
                     break
         return datas
 
     def commit(self):
         tasker_context, iterator_name, datas = TaskerContext.current(), None, None
-        if self.name not in self.db.csvs and not self.query and \
+        if self.name not in self.db.csvs and not self.query and tasker_context and \
                 (not self.orders or not tasker_context.tasker.config["orders"]) and self.limit:
             iterator_name = "csv::" + self.name
             iterator = tasker_context.get_iterator(iterator_name)
             if not iterator or iterator.offset != self.limit[0]:
                 fp = self.open_file(self.name)
                 if fp is not None:
                     iterator = TaskerFileIterator(fp, [])
@@ -100,18 +100,19 @@
             if iterator:
                 datas = self.csv_read(iterator.fp, iterator.fields, self.limit[1] - self.limit[0])
                 iterator.offset += len(datas)
                 return datas
 
         if self.limit and (self.query or self.orders):
             tasker_context = TaskerContext.current()
-            iterator_name = "csv::" + self.name
-            iterator = tasker_context.get_iterator(iterator_name)
-            if iterator and iterator.offset == self.limit[0]:
-                datas, iterator.offset = iterator.datas, self.limit[1]
+            if tasker_context:
+                iterator_name = "csv::" + self.name
+                iterator = tasker_context.get_iterator(iterator_name)
+                if iterator and iterator.offset == self.limit[0]:
+                    datas, iterator.offset = iterator.datas, self.limit[1]
 
         if not datas:
             if self.name not in self.db.csvs:
                 fp = self.open_file(self.name)
                 if fp is None:
                     return []
                 try:
@@ -137,15 +138,15 @@
                             break
                     if succed:
                         datas.append(data)
 
             if self.orders:
                 datas = sorted_by_keys(datas, keys=[(key, True if direct < 0 else False)
                                                     for key, direct in self.orders] if self.orders else None)
-            if self.limit and (self.query or self.orders):
+            if tasker_context and self.limit and (self.query or self.orders):
                 tasker_context.add_iterator(iterator_name, TaskerDataIterator(datas, self.limit[1]))
 
         if self.limit:
             datas = datas[self.limit[0]: self.limit[1]]
         return datas
 
     def verbose(self):
@@ -164,15 +165,16 @@
 
     def commit(self):
         csv_file = self.db.ensure_open_file(self.name)
         csv_file.fields = self.fields
         csv_file.datas.extend(self.datas)
         csv_file.changed = True
         tasker_context = TaskerContext.current()
-        tasker_context.remove_iterator("csv::" + self.name)
+        if tasker_context:
+            tasker_context.remove_iterator("csv::" + self.name)
 
     def verbose(self):
         return "datas(%d): \n%s" % (len(self.datas), human_repr_object(self.datas))
 
 
 class CsvUpdateBuilder(UpdateBuilder):
     def __init__(self, *args, **kwargs):
@@ -217,15 +219,16 @@
                 datas.append(self.update)
             else:
                 datas.append(data)
 
         csv_file.datas = datas
         csv_file.changed = True
         tasker_context = TaskerContext.current()
-        tasker_context.remove_iterator("csv::" + self.name)
+        if tasker_context:
+            tasker_context.remove_iterator("csv::" + self.name)
         return datas
 
     def verbose(self):
         return "filters: %s\nupdateDatas: %s" % (
             human_repr_object([(key, exp, value) for (key, exp), (value, cmp) in self.query.items()]),
             human_repr_object(self.diff_data))
 
@@ -270,15 +273,16 @@
 
             if not succed:
                 datas.append(data)
 
         csv_file.datas = datas
         csv_file.changed = True
         tasker_context = TaskerContext.current()
-        tasker_context.remove_iterator("csv::" + self.name)
+        if tasker_context:
+            tasker_context.remove_iterator("csv::" + self.name)
         return datas
 
     def verbose(self):
         return "filters: %s" % human_repr_object([(key, exp, value) for (key, exp), (value, cmp) in self.query.items()])
 
 
 class CsvFile(object):
```

### Comparing `syncany-0.2.5/syncany/database/database.py` & `syncany-0.2.6/syncany/database/database.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/database/elasticsearch.py` & `syncany-0.2.6/syncany/database/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/database/excel.py` & `syncany-0.2.6/syncany/database/excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,18 +59,19 @@
     def order_by(self, key, direct=1):
         self.orders.append((key, direct))
 
     def commit(self):
         tasker_context, iterator_name, datas = None, None, None
         if self.limit and (self.query or self.orders):
             tasker_context = TaskerContext.current()
-            iterator_name = "excel::" + self.name
-            iterator = tasker_context.get_iterator(iterator_name)
-            if iterator and iterator.offset == self.limit[0]:
-                datas, iterator.offset = iterator.datas, self.limit[1]
+            if tasker_context:
+                iterator_name = "excel::" + self.name
+                iterator = tasker_context.get_iterator(iterator_name)
+                if iterator and iterator.offset == self.limit[0]:
+                    datas, iterator.offset = iterator.datas, self.limit[1]
 
         if not datas:
             execl_sheet = self.db.ensure_open_file(self.name)
             if not self.query:
                 datas = execl_sheet.sheet_datas[:]
             else:
                 datas = []
@@ -85,15 +86,15 @@
                             break
                     if succed:
                         datas.append(data)
 
             if self.orders:
                 datas = sorted_by_keys(datas, keys=[(key, True if direct < 0 else False)
                                                     for key, direct in self.orders] if self.orders else None)
-            if self.limit and (self.query or self.orders):
+            if tasker_context and self.limit and (self.query or self.orders):
                 tasker_context.add_iterator(iterator_name, TaskerDataIterator(datas, self.limit[1]))
 
         if self.limit:
             datas = datas[self.limit[0]: self.limit[1]]
         return datas
 
     def verbose(self):
@@ -112,15 +113,16 @@
 
     def commit(self):
         execl_sheet = self.db.ensure_open_file(self.name)
         execl_sheet.sheet_descriptions = self.fields
         execl_sheet.sheet_datas.extend(self.datas)
         execl_sheet.changed = True
         tasker_context = TaskerContext.current()
-        tasker_context.remove_iterator("excel::" + self.name)
+        if tasker_context:
+            tasker_context.remove_iterator("excel::" + self.name)
 
     def verbose(self):
         return "datas(%d): \n%s" % (len(self.datas), human_repr_object(self.datas))
 
 
 class ExeclUpdateBuilder(UpdateBuilder):
     def __init__(self, *args, **kwargs):
@@ -165,15 +167,16 @@
                 datas.append(self.update)
             else:
                 datas.append(data)
 
         execl_sheet.sheet_datas = datas
         execl_sheet.changed = True
         tasker_context = TaskerContext.current()
-        tasker_context.remove_iterator("excel::" + self.name)
+        if tasker_context:
+            tasker_context.remove_iterator("excel::" + self.name)
         return datas
 
     def verbose(self):
         return "filters: %s\nupdateDatas: %s" % (
             human_repr_object([(key, exp, value) for (key, exp), (value, cmp) in self.query.items()]),
             human_repr_object(self.diff_data))
 
@@ -218,15 +221,16 @@
 
             if not succed:
                 datas.append(data)
 
         execl_sheet.sheet_datas = datas
         execl_sheet.changed = True
         tasker_context = TaskerContext.current()
-        tasker_context.remove_iterator("excel::" + self.name)
+        if tasker_context:
+            tasker_context.remove_iterator("excel::" + self.name)
         return datas
 
     def verbose(self):
         return "filters: %s" % human_repr_object([(key, exp, value) for (key, exp), (value, cmp) in self.query.items()])
 
 
 class ExeclSheet(object):
```

### Comparing `syncany-0.2.5/syncany/database/http.py` & `syncany-0.2.6/syncany/database/http.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/database/influxdb.py` & `syncany-0.2.6/syncany/database/influxdb.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/database/json.py` & `syncany-0.2.6/syncany/database/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,18 +55,19 @@
     def order_by(self, key, direct=1):
         self.orders.append((key, direct))
 
     def commit(self):
         tasker_context, iterator_name, datas = None, None, None
         if self.limit and (self.query or self.orders):
             tasker_context = TaskerContext.current()
-            iterator_name = "json::" + self.name
-            iterator = tasker_context.get_iterator(iterator_name)
-            if iterator and iterator.offset == self.limit[0]:
-                datas, iterator.offset = iterator.datas, self.limit[1]
+            if tasker_context:
+                iterator_name = "json::" + self.name
+                iterator = tasker_context.get_iterator(iterator_name)
+                if iterator and iterator.offset == self.limit[0]:
+                    datas, iterator.offset = iterator.datas, self.limit[1]
 
         if not datas:
             json_file = self.db.ensure_open_file(self.name)
             if not self.query:
                 datas = json_file.datas[:]
             else:
                 datas = []
@@ -81,15 +82,15 @@
                             break
                     if succed:
                         datas.append(data)
 
             if self.orders:
                 datas = sorted_by_keys(datas, keys=[(key, True if direct < 0 else False)
                                                     for key, direct in self.orders] if self.orders else None)
-            if self.limit and (self.query or self.orders):
+            if tasker_context and self.limit and (self.query or self.orders):
                 tasker_context.add_iterator(iterator_name, TaskerDataIterator(datas, self.limit[1]))
 
         if self.limit:
             datas = datas[self.limit[0]: self.limit[1]]
         return datas
 
     def verbose(self):
@@ -107,15 +108,16 @@
             self.datas = [self.datas]
 
     def commit(self):
         json_file = self.db.ensure_open_file(self.name)
         json_file.datas.extend(self.datas)
         json_file.changed = True
         tasker_context = TaskerContext.current()
-        tasker_context.remove_iterator("json::" + self.name)
+        if tasker_context:
+            tasker_context.remove_iterator("json::" + self.name)
 
     def verbose(self):
         return "datas(%d): \n%s" % (len(self.datas), human_repr_object(self.datas))
 
 
 class JsonUpdateBuilder(UpdateBuilder):
     def __init__(self, *args, **kwargs):
@@ -159,15 +161,16 @@
                 datas.append(self.update)
             else:
                 datas.append(data)
 
         json_file.datas = datas
         json_file.changed = True
         tasker_context = TaskerContext.current()
-        tasker_context.remove_iterator("json::" + self.name)
+        if tasker_context:
+            tasker_context.remove_iterator("json::" + self.name)
         return datas
 
     def verbose(self):
         return "filters: %s\nupdateDatas: %s" % (
             human_repr_object([(key, exp, value) for (key, exp), (value, cmp) in self.query.items()]),
             human_repr_object(self.diff_data))
 
@@ -212,15 +215,16 @@
 
             if not succed:
                 datas.append(data)
 
         json_file.datas = datas
         json_file.changed = True
         tasker_context = TaskerContext.current()
-        tasker_context.remove_iterator("json::" + self.name)
+        if tasker_context:
+            tasker_context.remove_iterator("json::" + self.name)
         return datas
 
     def verbose(self):
         return "filters: %s" % human_repr_object([(key, exp, value) for (key, exp), (value, cmp) in self.query.items()])
 
 
 class JsonFile(object):
```

### Comparing `syncany-0.2.5/syncany/database/memory.py` & `syncany-0.2.6/syncany/database/memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,18 +49,19 @@
     def order_by(self, key, direct=1):
         self.orders.append((key, direct))
 
     def commit(self):
         tasker_context, iterator, iterator_name, datas = None, None, None, None
         if self.limit and (self.query or self.orders):
             tasker_context = TaskerContext.current()
-            iterator_name = "memory::" + self.name
-            iterator = tasker_context.get_iterator(iterator_name)
-            if iterator and iterator.offset == self.limit[0]:
-                datas, iterator.offset = iterator.datas, self.limit[1]
+            if tasker_context:
+                iterator_name = "memory::" + self.name
+                iterator = tasker_context.get_iterator(iterator_name)
+                if iterator and iterator.offset == self.limit[0]:
+                    datas, iterator.offset = iterator.datas, self.limit[1]
 
         if not datas:
             if not self.query:
                 datas = self.db.memory_databases.get(self.name, [])[:]
             else:
                 datas = []
                 for data in self.db.memory_databases.get(self.name, []):
@@ -74,15 +75,15 @@
                             break
                     if succed:
                         datas.append(data)
 
             if self.orders:
                 datas = sorted_by_keys(datas, keys=[(key, True if direct < 0 else False)
                                                     for key, direct in self.orders] if self.orders else None)
-            if self.limit and (self.query or self.orders):
+            if tasker_context and self.limit and (self.query or self.orders):
                 tasker_context.add_iterator(iterator_name, TaskerDataIterator(datas, self.limit[1]))
 
         if self.limit:
             datas = datas[self.limit[0]: self.limit[1]]
 
         if not datas:
             db_keys = self.name.split(".")
@@ -118,15 +119,16 @@
             cache_keys = self.name.split(".")
             if len(cache_keys) == 2 or cache_keys[1][:2] == "--":
                 return
         datas = self.db.memory_databases.get(self.name, [])
         datas.extend(self.datas)
         self.db.memory_databases[self.name] = datas
         tasker_context = TaskerContext.current()
-        tasker_context.remove_iterator("memory::" + self.name)
+        if tasker_context:
+            tasker_context.remove_iterator("memory::" + self.name)
 
     def verbose(self):
         return "datas(%d): \n%s" % (len(self.datas), human_repr_object(self.datas))
 
 
 class MemoryUpdateBuilder(UpdateBuilder):
     def __init__(self, *args, **kwargs):
@@ -173,15 +175,16 @@
             if succed:
                 datas.append(self.update)
             else:
                 datas.append(data)
 
         self.db.memory_databases[self.name] = datas
         tasker_context = TaskerContext.current()
-        tasker_context.remove_iterator("memory::" + self.name)
+        if tasker_context:
+            tasker_context.remove_iterator("memory::" + self.name)
         return datas
 
     def verbose(self):
         return "filters: %s\nupdateDatas: %s" % (
             human_repr_object([(key, exp, value) for (key, exp), (value, cmp) in self.query.items()]),
             human_repr_object(self.diff_data))
 
@@ -214,15 +217,15 @@
     def commit(self):
         if ".--" in self.name:
             cache_keys = self.name.split(".")
             if len(cache_keys) == 2 or cache_keys[1][:2] == "--":
                 return
 
         if not self.query:
-            self.db.memory_databases[self.name] = []
+            self.db.memory_databases.pop(self.name, None)
             return []
 
         datas = []
         for data in self.db.memory_databases.get(self.name, []):
             succed = True
             for (key, exp), (value, cmp) in self.query.items():
                 if key not in data:
@@ -233,15 +236,16 @@
                     break
 
             if not succed:
                 datas.append(data)
 
         self.db.memory_databases[self.name] = datas
         tasker_context = TaskerContext.current()
-        tasker_context.remove_iterator("memory::" + self.name)
+        if tasker_context:
+            tasker_context.remove_iterator("memory::" + self.name)
         return datas
 
     def verbose(self):
         return "filters: %s" % human_repr_object([(key, exp, value) for (key, exp), (value, cmp) in self.query.items()])
 
 
 class MemoryCacheBuilder(CacheBuilder):
```

### Comparing `syncany-0.2.5/syncany/database/mongodb.py` & `syncany-0.2.6/syncany/database/mongodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,15 +309,17 @@
         if key not in self.query:
             self.query[key] = {}
         self.query[key]["$in"] = value
 
     def commit(self):
         connection = self.db.ensure_connection()
         try:
-            return connection[self.db_name][self.collection_name].remove(self.query, multi=True)
+            if not self.query and self.db.delete_all_drop_collection:
+                return connection[self.db_name][self.collection_name].drop()
+            return connection[self.db_name][self.collection_name].delete_many(self.query)
         finally:
             self.db.release_connection()
 
     def verbose(self):
         return "collection: %s\nquery: %s" % (self.collection_name, human_repr_object(self.query))
 
 
@@ -361,14 +363,16 @@
     def __init__(self, manager, config):
         all_config = {}
         all_config.update(self.DEFAULT_CONFIG)
         all_config.update(config)
 
         self.db_name = all_config.pop("db") if "db" in all_config else all_config["name"]
         self.virtual_collections = all_config.pop("virtual_views") if "virtual_views" in all_config else []
+        self.delete_all_drop_collection = all_config.pop("delete_all_drop_collection") \
+            if "delete_all_drop_collection" in all_config else False
 
         super(MongoDB, self).__init__(manager, all_config)
 
     def build_factory(self):
         return MongoDBFactory(self.get_config_key(), self.config)
 
     def ensure_connection(self):
```

### Comparing `syncany-0.2.5/syncany/database/mysql.py` & `syncany-0.2.6/syncany/database/mysql.py`

 * *Files 3% similar despite different names*

```diff
@@ -303,15 +303,18 @@
     def filter_in(self, key, value):
         self.query.append('`' + key + "` in %s")
         self.query_values.append(value)
 
     def commit(self):
         db_name = self.name.split(".")
         db_name = ("`%s`.`%s`" % (self.db.db_name, ".".join(db_name[1:]))) if len(db_name) > 1 else ('`' + db_name[0] + '`')
-        sql = "DELETE FROM %s WHERE %s" % (db_name, " AND ".join(self.query))
+        if not self.query and self.db.delete_all_truncate_table:
+            sql = "TRUNCATE TABLE %s" % db_name
+        else:
+            sql = "DELETE FROM %s WHERE %s" % (db_name, " AND ".join(self.query))
         connection = self.db.ensure_connection()
         cursor = connection.cursor(self.db.DictCursor)
         try:
             cursor.execute(sql, self.query_values)
         finally:
             cursor.close()
             connection.commit()
@@ -363,14 +366,16 @@
     def __init__(self, manager, config):
         all_config = {}
         all_config.update(self.DEFAULT_CONFIG)
         all_config.update(config)
 
         self.db_name = all_config["db"] if "db" in all_config else all_config["name"]
         self.virtual_tables = all_config.pop("virtual_views") if "virtual_views" in all_config else []
+        self.delete_all_truncate_table = all_config.pop("delete_all_truncate_table") \
+            if "delete_all_truncate_table" in all_config else False
 
         super(MysqlDB, self).__init__(manager, all_config)
 
     def build_factory(self):
         try:
             from pymysql.cursors import DictCursor
         except ImportError:
```

### Comparing `syncany-0.2.5/syncany/database/postgresql.py` & `syncany-0.2.6/syncany/database/postgresql.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,15 +302,18 @@
     def filter_in(self, key, value):
         self.query.append('"' + key + '" in %s')
         self.query_values.append(tuple(value))
 
     def commit(self):
         db_name = self.name.split(".")
         db_name = ('"%s"' % ".".join(db_name[1:])) if len(db_name) > 1 else ('"' + db_name[0] + '"')
-        sql = "DELETE FROM %s WHERE %s" % (db_name, " AND ".join(self.query))
+        if not self.query and self.db.delete_all_truncate_table:
+            sql = "TRUNCATE TABLE %s" % db_name
+        else:
+            sql = "DELETE FROM %s WHERE %s" % (db_name, " AND ".join(self.query))
         connection = self.db.ensure_connection()
         cursor = connection.cursor()
         try:
             cursor.execute(sql, self.query_values)
         finally:
             cursor.close()
             connection.commit()
@@ -369,14 +372,16 @@
 
         all_config = {}
         all_config.update(self.DEFAULT_CONFIG)
         all_config.update(config)
 
         self.db_name = all_config["dbname"] if "dbname" in all_config else all_config["name"]
         self.virtual_tables = all_config.pop("virtual_views") if "virtual_views" in all_config else []
+        self.delete_all_truncate_table = all_config.pop("delete_all_truncate_table") \
+            if "delete_all_truncate_table" in all_config else False
 
         super(PostgresqlDB, self).__init__(manager, all_config)
 
     def build_factory(self):
         try:
             from psycopg2.extras import DictCursor
         except ImportError:
```

### Comparing `syncany-0.2.5/syncany/database/redis.py` & `syncany-0.2.6/syncany/database/redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,18 +195,19 @@
     def order_by(self, key, direct=1):
         self.orders.append((key, direct))
 
     def commit(self):
         tasker_context, iterator, iterator_name, datas = None, None, None, None
         if self.limit and (self.query or self.orders):
             tasker_context = TaskerContext.current()
-            iterator_name = "redis::" + self.name
-            iterator = tasker_context.get_iterator(iterator_name)
-            if iterator and iterator.offset == self.limit[0]:
-                datas, iterator.offset = iterator.datas, self.limit[1]
+            if tasker_context:
+                iterator_name = "redis::" + self.name
+                iterator = tasker_context.get_iterator(iterator_name)
+                if iterator and iterator.offset == self.limit[0]:
+                    datas, iterator.offset = iterator.datas, self.limit[1]
 
         if not datas:
             try:
                 connection = self.db.ensure_connection()
                 load_datas = self.load_datas(connection)
                 if not self.query:
                     datas = load_datas[:]
@@ -223,15 +224,15 @@
                                 break
                         if succed:
                             datas.append(data)
 
                 if self.orders:
                     datas = sorted_by_keys(datas, keys=[(key, True if direct < 0 else False)
                                                         for key, direct in self.orders] if self.orders else None)
-                if self.limit and (self.query or self.orders):
+                if tasker_context and self.limit and (self.query or self.orders):
                     tasker_context.add_iterator(iterator_name, TaskerDataIterator(datas, self.limit[1]))
             finally:
                 self.db.release_connection()
 
         if self.limit:
             datas = datas[self.limit[0]: self.limit[1]]
         return datas
@@ -252,15 +253,16 @@
         try:
             connection = self.db.ensure_connection()
             self.save_datas(connection, self.primary_keys, self.datas, self.db.expire_seconds)
             return self.datas
         finally:
             self.db.release_connection()
             tasker_context = TaskerContext.current()
-            tasker_context.remove_iterator("redis::" + self.name)
+            if tasker_context:
+                tasker_context.remove_iterator("redis::" + self.name)
 
     def verbose(self):
         return "datas(%d): \n%s" % (len(self.datas), human_repr_object(self.datas))
 
 
 class RedisUpdateBuilder(UpdateBuilder, RedisCommand):
     def __init__(self, *args, **kwargs):
@@ -308,15 +310,16 @@
                     datas.append(data)
             self.delete_datas(connection)
             if datas:
                 self.save_datas(connection, self.primary_keys, datas, self.db.expire_seconds)
         finally:
             self.db.release_connection()
             tasker_context = TaskerContext.current()
-            tasker_context.remove_iterator("redis::" + self.name)
+            if tasker_context:
+                tasker_context.remove_iterator("redis::" + self.name)
 
     def verbose(self):
         return "filters: %s\nupdateDatas: %s" % (
             human_repr_object([(key, exp, value) for (key, exp), (value, cmp) in self.query.items()]),
             human_repr_object(self.diff_data))
 
 
@@ -369,15 +372,16 @@
 
             self.delete_datas(connection)
             if datas:
                 self.save_datas(connection, self.primary_keys, datas, self.db.expire_seconds)
         finally:
             self.db.release_connection()
             tasker_context = TaskerContext.current()
-            tasker_context.remove_iterator("redis::" + self.name)
+            if tasker_context:
+                tasker_context.remove_iterator("redis::" + self.name)
 
     def verbose(self):
         return "filters: %s" % human_repr_object([(key, exp, value) for (key, exp), (value, cmp) in self.query.items()])
 
 
 class RedisCacheBuilder(CacheBuilder):
     def __init__(self, *args, **kwargs):
```

### Comparing `syncany-0.2.5/syncany/database/sqlite.py` & `syncany-0.2.6/syncany/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/database/sqlserver.py` & `syncany-0.2.6/syncany/database/sqlserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -328,15 +328,18 @@
 
     def filter_in(self, key, value):
         self.query.append('[' + key + "] in %s")
         self.query_values.append(value)
 
     def commit(self):
         db_name = ("[%s].[%s].[%s]" % (self.db.db_name, self.dbo_name, self.table_name))
-        sql = "DELETE FROM %s WHERE %s" % (db_name, " AND ".join(self.query))
+        if not self.query and self.db.delete_all_truncate_table:
+            sql = "TRUNCATE TABLE %s" % db_name
+        else:
+            sql = "DELETE FROM %s WHERE %s" % (db_name, " AND ".join(self.query))
         connection = self.db.ensure_connection()
         cursor = connection.cursor(as_dict=True)
         try:
             cursor.execute(sql, tuple(self.query_values))
         finally:
             cursor.close()
             connection.commit()
@@ -387,14 +390,16 @@
     def __init__(self, manager, config):
         all_config = {}
         all_config.update(self.DEFAULT_CONFIG)
         all_config.update(config)
 
         self.db_name = all_config["database"] if "database" in all_config else all_config["name"]
         self.virtual_tables = all_config.pop("virtual_views") if "virtual_views" in all_config else []
+        self.delete_all_truncate_table = all_config.pop("delete_all_truncate_table") \
+            if "delete_all_truncate_table" in all_config else False
 
         super(SqlServerDB, self).__init__(manager, all_config)
 
     def build_factory(self):
         return SqlServerDBFactory(self.get_config_key(), self.config)
 
     def ensure_connection(self):
```

### Comparing `syncany-0.2.5/syncany/database/textline.py` & `syncany-0.2.6/syncany/database/textline.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,15 +204,15 @@
                 rdatas = self.text_read(fp)
         else:
             filename = os.path.join(self.db.config.get("path", "/"), ".".join(fileinfo[1:]))
             if not os.path.exists(filename):
                 return []
 
             tasker_context = TaskerContext.current()
-            if not self.query and (not self.orders or not tasker_context.tasker.config["orders"]) and self.limit:
+            if not self.query and tasker_context and (not self.orders or not tasker_context.tasker.config["orders"]) and self.limit:
                 iterator_name = "textline::" + self.name
                 iterator = tasker_context.get_iterator(iterator_name)
                 if not iterator or iterator.offset != self.limit[0]:
                     iterator = TaskerFileIterator(open(filename, "r", newline='', encoding=self.db.config.get("encoding", "utf-8")), [])
                     tasker_context.add_iterator(iterator_name, iterator)
                 if self.db.config.get("format") == "csv":
                     rdatas = self.csv_read(iterator.fp, iterator.fields, self.limit[1] - self.limit[0])
@@ -371,15 +371,16 @@
             elif self.db.config.get("format") == "txt":
                 self.text_write(fp)
             elif self.db.config.get("format") == "richtable":
                 self.rich_write(fp)
             else:
                 self.text_write(fp)
         tasker_context = TaskerContext.current()
-        tasker_context.remove_iterator("textline::" + self.name)
+        if tasker_context:
+            tasker_context.remove_iterator("textline::" + self.name)
 
     def verbose(self):
         return "datas(%d): \n%s" % (len(self.datas), human_repr_object(self.datas))
 
 
 class TextLineUpdateBuilder(UpdateBuilder):
     def __init__(self, *args, **kwargs):
@@ -404,15 +405,16 @@
         pass
 
     def filter_in(self, key, value):
         pass
 
     def commit(self):
         tasker_context = TaskerContext.current()
-        tasker_context.remove_iterator("textline::" + self.name)
+        if tasker_context:
+            tasker_context.remove_iterator("textline::" + self.name)
         return []
 
 
 class TextLineDeleteBuilder(DeleteBuilder):
     def __init__(self, *args, **kwargs):
         super(TextLineDeleteBuilder, self).__init__(*args, **kwargs)
 
@@ -435,15 +437,16 @@
         pass
 
     def filter_in(self, key, value):
         pass
 
     def commit(self):
         tasker_context = TaskerContext.current()
-        tasker_context.remove_iterator("textline::" + self.name)
+        if tasker_context:
+            tasker_context.remove_iterator("textline::" + self.name)
         return []
 
 
 class TextLineDB(DataBase):
     DEFAULT_CONFIG = {
         "encoding": os.environ.get("SYNCANYENCODING", "utf-8"),
         "sep": None,
```

### Comparing `syncany-0.2.5/syncany/errors.py` & `syncany-0.2.6/syncany/errors.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/filters/builtin.py` & `syncany-0.2.6/syncany/filters/builtin.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/hook.py` & `syncany-0.2.6/syncany/hook.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/loaders/__init__.py` & `syncany-0.2.6/syncany/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/loaders/cache.py` & `syncany-0.2.6/syncany/loaders/cache.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/loaders/const.py` & `syncany-0.2.6/syncany/loaders/const.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/loaders/db.py` & `syncany-0.2.6/syncany/loaders/db.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/loaders/db_join.py` & `syncany-0.2.6/syncany/loaders/db_join.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/loaders/db_pull.py` & `syncany-0.2.6/syncany/loaders/db_pull.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/loaders/loader.py` & `syncany-0.2.6/syncany/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/main.py` & `syncany-0.2.6/syncany/main.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/outputers/__init__.py` & `syncany-0.2.6/syncany/outputers/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/outputers/db.py` & `syncany-0.2.6/syncany/outputers/db.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/outputers/db_delete_insert.py` & `syncany-0.2.6/syncany/outputers/db_delete_insert.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,8 +50,10 @@
             insert.commit()
             self.outputer_state["insert_count"] += 1
 
     def store(self, datas):
         super(DBDeleteInsertOutputer, self).store(datas)
 
         self.remove()
-        self.insert(datas)
+        if not datas:
+            return
+        self.insert(datas)
```

### Comparing `syncany-0.2.5/syncany/outputers/db_insert.py` & `syncany-0.2.6/syncany/outputers/db_insert.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,8 +16,10 @@
         else:
             insert = self.db.insert(self.name, self.primary_keys, list(self.schema.keys()), datas)
             insert.commit()
             self.outputer_state["insert_count"] += 1
 
     def store(self, datas):
         super(DBInsertOutputer, self).store(datas)
-        self.insert(datas)
+        if not datas:
+            return
+        self.insert(datas)
```

### Comparing `syncany-0.2.5/syncany/outputers/db_update_delete_insert.py` & `syncany-0.2.6/syncany/outputers/db_update_delete_insert.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,10 +143,9 @@
             if primary_key in update_datas:
                 continue
 
             delete_datas.append(data)
 
         if delete_datas:
             self.remove(delete_datas)
-
         if insert_datas:
-            self.insert(insert_datas)
+            self.insert(insert_datas)
```

### Comparing `syncany-0.2.5/syncany/outputers/db_update_insert.py` & `syncany-0.2.6/syncany/outputers/db_update_insert.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -98,8 +98,8 @@
             primary_key = self.get_data_primary_key(data)
             if primary_key in self.load_data_keys:
                 self.update(data, self.load_data_keys[primary_key])
             else:
                 insert_datas.append(data)
 
         if insert_datas:
-            self.insert(insert_datas)
+            self.insert(insert_datas)
```

### Comparing `syncany-0.2.5/syncany/outputers/outputer.py` & `syncany-0.2.6/syncany/outputers/outputer.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/taskers/config/__init__.py` & `syncany-0.2.6/syncany/taskers/config/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/taskers/config/http_reader.py` & `syncany-0.2.6/syncany/taskers/config/http_reader.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/taskers/config/yaml_parser.py` & `syncany-0.2.6/syncany/taskers/config/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/taskers/context.py` & `syncany-0.2.6/syncany/taskers/context.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/taskers/core/__init__.py` & `syncany-0.2.6/syncany/taskers/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
             except NotImplementedError:
                 raise CacheUnknownException(name + " is unknown")
 
     def load_imports(self):
         for name, package in self.config["imports"].items():
             if not package or isinstance(package, (bool, int, float, list, tuple, set, dict)):
                 continue
-            module = __import__(package, {}, {}) if isinstance(package, str) else package
+            module = __import__(package, globals(), locals(), [package.rpartition(".")[-1]]) if isinstance(package, str) else package
             try:
                 if not self.find_calculater_driver(name):
                     self.register_calculater_driver(name, create_import_calculater(name, module))
             except CalculaterUnknownException:
                 self.register_calculater_driver(name, create_import_calculater(name, module))
 
     def load_sources(self):
@@ -1050,15 +1050,16 @@
             else:
                 self.loader.filter_limit(batch_count)
             self.loader.load(loader_timeout)
             load_count = len(self.loader.datas)
             self.loader.datas = self.run_queried_hooks(self.loader.datas)
             self.print_queryed_statistics(self.loader, self.status["statistics"]["loader"])
 
-            if self.outputer.is_dynamic_schema() and self.schema == ".*" and not self.config["querys"] and not self.intercepts:
+            if self.outputer.is_dynamic_schema() and self.schema == ".*" and not self.config["querys"] \
+                    and not self.intercepts and not self.hookers:
                 datas = self.loader.datas
             else:
                 datas = self.loader.get()
             datas = self.run_loaded_hooks(datas)
             self.print_loaded_statistics(self.join_loaders.values(), self.status["statistics"]["join_loaders"])
 
             if last_cursor_data:
@@ -1105,15 +1106,16 @@
         if "@limit" in self.arguments and self.arguments["@limit"] > 0:
             self.loader.filter_limit(self.arguments["@limit"])
         self.loader.load(loader_timeout)
         self.status["load_count"] = len(self.loader.datas)
         self.loader.datas = self.run_queried_hooks(self.loader.datas)
         self.print_queryed_statistics(self.loader, self.status["statistics"]["loader"])
 
-        if self.outputer.is_dynamic_schema() and self.schema == ".*" and not self.config["querys"] and not self.intercepts:
+        if self.outputer.is_dynamic_schema() and self.schema == ".*" and not self.config["querys"] \
+                and not self.intercepts and not self.hookers:
             datas = self.loader.datas
         else:
             datas = self.loader.get()
         datas = self.run_loaded_hooks(datas)
         self.print_loaded_statistics(self.join_loaders.values(), self.status["statistics"]["join_loaders"])
 
         self.outputer.store(datas)
```

### Comparing `syncany-0.2.5/syncany/taskers/core/loader_creater.py` & `syncany-0.2.6/syncany/taskers/core/loader_creater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/taskers/core/outputer_creater.py` & `syncany-0.2.6/syncany/taskers/core/outputer_creater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/taskers/core/states.py` & `syncany-0.2.6/syncany/taskers/core/states.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/taskers/core/valuer_compiler.py` & `syncany-0.2.6/syncany/taskers/core/valuer_compiler.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/taskers/core/valuer_creater.py` & `syncany-0.2.6/syncany/taskers/core/valuer_creater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/taskers/iterator.py` & `syncany-0.2.6/syncany/taskers/iterator.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/taskers/tasker.py` & `syncany-0.2.6/syncany/taskers/tasker.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/utils.py` & `syncany-0.2.6/syncany/utils.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/__init__.py` & `syncany-0.2.6/syncany/valuers/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/aggregate.py` & `syncany-0.2.6/syncany/valuers/aggregate.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/assign.py` & `syncany-0.2.6/syncany/valuers/assign.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/cache.py` & `syncany-0.2.6/syncany/valuers/cache.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/calculate.py` & `syncany-0.2.6/syncany/valuers/calculate.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/call.py` & `syncany-0.2.6/syncany/valuers/call.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/case.py` & `syncany-0.2.6/syncany/valuers/case.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/condition.py` & `syncany-0.2.6/syncany/valuers/condition.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/const.py` & `syncany-0.2.6/syncany/valuers/const.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/data.py` & `syncany-0.2.6/syncany/valuers/data.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/db_join.py` & `syncany-0.2.6/syncany/valuers/db_join.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/db_load.py` & `syncany-0.2.6/syncany/valuers/db_load.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/function.py` & `syncany-0.2.6/syncany/valuers/function.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/generator.py` & `syncany-0.2.6/syncany/valuers/generator.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/inherit.py` & `syncany-0.2.6/syncany/valuers/inherit.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/let.py` & `syncany-0.2.6/syncany/valuers/let.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/loop.py` & `syncany-0.2.6/syncany/valuers/loop.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/make.py` & `syncany-0.2.6/syncany/valuers/make.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/match.py` & `syncany-0.2.6/syncany/valuers/match.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/schema.py` & `syncany-0.2.6/syncany/valuers/schema.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/state.py` & `syncany-0.2.6/syncany/valuers/state.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany/valuers/valuer.py` & `syncany-0.2.6/syncany/valuers/valuer.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.5/syncany.egg-info/PKG-INFO` & `syncany-0.2.6/syncany.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncany
-Version: 0.2.5
+Version: 0.2.6
 Summary: 简单易用的数据同步转换导出框架
 Home-page: https://github.com/snower/syncany
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # syncany
```

### Comparing `syncany-0.2.5/syncany.egg-info/SOURCES.txt` & `syncany-0.2.6/syncany.egg-info/SOURCES.txt`

 * *Files identical despite different names*

