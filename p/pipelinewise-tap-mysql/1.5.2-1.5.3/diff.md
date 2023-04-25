# Comparing `tmp/pipelinewise-tap-mysql-1.5.2.tar.gz` & `tmp/pipelinewise-tap-mysql-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipelinewise-tap-mysql-1.5.2.tar", last modified: Fri Aug 12 07:31:47 2022, max compression
+gzip compressed data, was "pipelinewise-tap-mysql-1.5.3.tar", last modified: Tue Apr 25 09:51:10 2023, max compression
```

## Comparing `pipelinewise-tap-mysql-1.5.2.tar` & `pipelinewise-tap-mysql-1.5.3.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 07:31:47.064501 pipelinewise-tap-mysql-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (121)    32393 2022-08-12 07:31:38.000000 pipelinewise-tap-mysql-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    23093 2022-08-12 07:31:47.064501 pipelinewise-tap-mysql-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    22642 2022-08-12 07:31:38.000000 pipelinewise-tap-mysql-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 07:31:47.064501 pipelinewise-tap-mysql-1.5.2/pipelinewise_tap_mysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    23093 2022-08-12 07:31:46.000000 pipelinewise-tap-mysql-1.5.2/pipelinewise_tap_mysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-08-12 07:31:46.000000 pipelinewise-tap-mysql-1.5.2/pipelinewise_tap_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-12 07:31:46.000000 pipelinewise-tap-mysql-1.5.2/pipelinewise_tap_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-08-12 07:31:46.000000 pipelinewise-tap-mysql-1.5.2/pipelinewise_tap_mysql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-08-12 07:31:46.000000 pipelinewise-tap-mysql-1.5.2/pipelinewise_tap_mysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-12 07:31:46.000000 pipelinewise-tap-mysql-1.5.2/pipelinewise_tap_mysql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-12 07:31:47.064501 pipelinewise-tap-mysql-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1207 2022-08-12 07:31:38.000000 pipelinewise-tap-mysql-1.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 07:31:47.064501 pipelinewise-tap-mysql-1.5.2/tap_mysql/
--rw-r--r--   0 runner    (1001) docker     (121)    17929 2022-08-12 07:31:38.000000 pipelinewise-tap-mysql-1.5.2/tap_mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6564 2022-08-12 07:31:38.000000 pipelinewise-tap-mysql-1.5.2/tap_mysql/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)    13865 2022-08-12 07:31:38.000000 pipelinewise-tap-mysql-1.5.2/tap_mysql/discover_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-08-12 07:31:38.000000 pipelinewise-tap-mysql-1.5.2/tap_mysql/stream_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-12 07:31:47.064501 pipelinewise-tap-mysql-1.5.2/tap_mysql/sync_strategies/
--rw-r--r--   0 runner    (1001) docker     (121)    35585 2022-08-12 07:31:38.000000 pipelinewise-tap-mysql-1.5.2/tap_mysql/sync_strategies/binlog.py
--rw-r--r--   0 runner    (1001) docker     (121)     7678 2022-08-12 07:31:38.000000 pipelinewise-tap-mysql-1.5.2/tap_mysql/sync_strategies/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     6855 2022-08-12 07:31:38.000000 pipelinewise-tap-mysql-1.5.2/tap_mysql/sync_strategies/full_table.py
--rw-r--r--   0 runner    (1001) docker     (121)     3064 2022-08-12 07:31:38.000000 pipelinewise-tap-mysql-1.5.2/tap_mysql/sync_strategies/incremental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:51:10.762766 pipelinewise-tap-mysql-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    32393 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-04-25 09:51:10.762766 pipelinewise-tap-mysql-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22726 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:51:10.762766 pipelinewise-tap-mysql-1.5.3/pipelinewise_tap_mysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-04-25 09:51:10.000000 pipelinewise-tap-mysql-1.5.3/pipelinewise_tap_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-25 09:51:10.000000 pipelinewise-tap-mysql-1.5.3/pipelinewise_tap_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 09:51:10.000000 pipelinewise-tap-mysql-1.5.3/pipelinewise_tap_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-25 09:51:10.000000 pipelinewise-tap-mysql-1.5.3/pipelinewise_tap_mysql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-25 09:51:10.000000 pipelinewise-tap-mysql-1.5.3/pipelinewise_tap_mysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 09:51:10.000000 pipelinewise-tap-mysql-1.5.3/pipelinewise_tap_mysql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 09:51:10.762766 pipelinewise-tap-mysql-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:51:10.762766 pipelinewise-tap-mysql-1.5.3/tap_mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)    17929 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/tap_mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/tap_mysql/binlogstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/tap_mysql/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/tap_mysql/discover_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/tap_mysql/stream_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:51:10.762766 pipelinewise-tap-mysql-1.5.3/tap_mysql/sync_strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/tap_mysql/sync_strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35207 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/tap_mysql/sync_strategies/binlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/tap_mysql/sync_strategies/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/tap_mysql/sync_strategies/full_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/tap_mysql/sync_strategies/incremental.py
```

### Comparing `pipelinewise-tap-mysql-1.5.2/LICENSE` & `pipelinewise-tap-mysql-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.2/PKG-INFO` & `pipelinewise-tap-mysql-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipelinewise-tap-mysql
-Version: 1.5.2
+Version: 1.5.3
 Summary: Singer.io tap for extracting data from MySQL & MariaDB - PipelineWise compatible
 Home-page: https://github.com/transferwise/pipelinewise-tap-mysql
 Author: Wise
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -73,32 +73,32 @@
 
 ### Create the configuration file
 
 Create a config file containing the database connection credentials, see [sample](config.json.sample).
 
 List of config parameters:
 
-| Parameter    | type                          | required | default                                                                                                                                                           | description                                                                                                               |
-|--------------|-------------------------------|----------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|
-| host         | string                        | yes      | -                                                                                                                                                                 | mysql/mariadb host                                                                                                        |
-| port         | int                           | yes      | -                                                                                                                                                                 | mysql/mariadb port                                                                                                        |
-| user         | string                        | yes      | -                                                                                                                                                                 | db username                                                                                                               |
-| password     | string                        | yes      | -                                                                                                                                                                 | db password                                                                                                               |
-| cursorclass  | string                        | No       | `pymysql.cursors.SSCursor`                                                                                                                                        | set cursorclass used by PyMYSQL                                                                                           |
-| database     | string                        | No       | -                                                                                                                                                                 | Database to use, None to not use a particular one. Used by PyMYSQL                                                        |
-| server_id    | int                           | False    | Randomly generated int                                                                                                                                            | Used as the slave id when this tap is connecting to the server                                                            |
-| filter_db    | string                        | False    | -                                                                                                                                                                 | Comma separated list of schemas to extract tables only from particular schemas and to improve data extraction performance |
-| use_gtid     | bool                          | False    | False                                                    <br/>                                                                                                         | Flag to enable log based replication using GTID               |
-| engine       | string ('mysql' or 'mariadb') | False    | 'mysql'                                                                                                                                                           | Indicate which flavor the server is, used for LOG_BASED with GTID                                                         |
-| ssl          | string ("true")               | No       | False                                                                                                                                                             | Enable SSL connection                                                                                                     |
-| ssl_ca       | string                        | No       | -                                                                                                                                                                 | for self-signed SSL                                                                                                       |
-| ssl_cert     | string                        | No       | -                                                                                                                                                                 | for self-signed SSL                                                                                                       |
-| ssl_key      | string                        | No       | -                                                                                                                                                                 | for self-signed SSL                                                                                                       |
-| internal_hostname  | string | No       | -                                                                                                                                                                 | Override match hostname for google cloud                                                                                  |
-| session_sqls | List of strings               | No       | ```['SET @@session.time_zone="+0:00"', 'SET @@session.wait_timeout=28800', 'SET @@session.net_read_timeout=3600', 'SET @@session.innodb_lock_wait_timeout=3600']``` | Set session variables dynamically.                                                                                        |
+| Parameter         | type                          | required | default                                                                                                                                                           | description                                                                                                               |
+|-------------------|-------------------------------|----------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|
+| host              | string                        | yes      | -                                                                                                                                                                 | mysql/mariadb host                                                                                                        |
+| port              | int                           | yes      | -                                                                                                                                                                 | mysql/mariadb port                                                                                                        |
+| user              | string                        | yes      | -                                                                                                                                                                 | db username                                                                                                               |
+| password          | string                        | yes      | -                                                                                                                                                                 | db password                                                                                                               |
+| cursorclass       | string                        | No       | `pymysql.cursors.SSCursor`                                                                                                                                        | set cursorclass used by PyMYSQL                                                                                           |
+| database          | string                        | No       | -                                                                                                                                                                 | Database to use, None to not use a particular one. Used by PyMYSQL                                                        |
+| server_id         | int                           | False    | Randomly generated int                                                                                                                                            | Used as the slave id when this tap is connecting to the server                                                            |
+| filter_dbs        | string                        | False    | -                                                                                                                                                                 | Comma separated list of schemas to extract tables only from particular schemas and to improve data extraction performance |
+| use_gtid          | bool                          | False    | False                                                    <br/>                                                                                                         | Flag to enable log based replication using GTID               |
+| engine            | string ('mysql' or 'mariadb') | False    | 'mysql'                                                                                                                                                           | Indicate which flavor the server is, used for LOG_BASED with GTID                                                         |
+| ssl               | string ("true")               | No       | False                                                                                                                                                             | Enable SSL connection                                                                                                     |
+| ssl_ca            | string                        | No       | -                                                                                                                                                                 | for self-signed SSL                                                                                                       |
+| ssl_cert          | string                        | No       | -                                                                                                                                                                 | for self-signed SSL                                                                                                       |
+| ssl_key           | string                        | No       | -                                                                                                                                                                 | for self-signed SSL                                                                                                       |
+| internal_hostname | string | No       | -                                                                                                                                                                 | Override match hostname for google cloud                                                                                  |
+| session_sqls      | List of strings               | No       | ```['SET @@session.time_zone="+0:00"', 'SET @@session.wait_timeout=28800', 'SET @@session.net_read_timeout=3600', 'SET @@session.innodb_lock_wait_timeout=3600']``` | Set session variables dynamically.                                                                                        |
 
 
 ### Discovery mode
 
 The tap can be invoked in discovery mode to find the available tables and
 columns in the database:
```

### Comparing `pipelinewise-tap-mysql-1.5.2/README.md` & `pipelinewise-tap-mysql-1.5.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -61,32 +61,32 @@
 
 ### Create the configuration file
 
 Create a config file containing the database connection credentials, see [sample](config.json.sample).
 
 List of config parameters:
 
-| Parameter    | type                          | required | default                                                                                                                                                           | description                                                                                                               |
-|--------------|-------------------------------|----------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|
-| host         | string                        | yes      | -                                                                                                                                                                 | mysql/mariadb host                                                                                                        |
-| port         | int                           | yes      | -                                                                                                                                                                 | mysql/mariadb port                                                                                                        |
-| user         | string                        | yes      | -                                                                                                                                                                 | db username                                                                                                               |
-| password     | string                        | yes      | -                                                                                                                                                                 | db password                                                                                                               |
-| cursorclass  | string                        | No       | `pymysql.cursors.SSCursor`                                                                                                                                        | set cursorclass used by PyMYSQL                                                                                           |
-| database     | string                        | No       | -                                                                                                                                                                 | Database to use, None to not use a particular one. Used by PyMYSQL                                                        |
-| server_id    | int                           | False    | Randomly generated int                                                                                                                                            | Used as the slave id when this tap is connecting to the server                                                            |
-| filter_db    | string                        | False    | -                                                                                                                                                                 | Comma separated list of schemas to extract tables only from particular schemas and to improve data extraction performance |
-| use_gtid     | bool                          | False    | False                                                    <br/>                                                                                                         | Flag to enable log based replication using GTID               |
-| engine       | string ('mysql' or 'mariadb') | False    | 'mysql'                                                                                                                                                           | Indicate which flavor the server is, used for LOG_BASED with GTID                                                         |
-| ssl          | string ("true")               | No       | False                                                                                                                                                             | Enable SSL connection                                                                                                     |
-| ssl_ca       | string                        | No       | -                                                                                                                                                                 | for self-signed SSL                                                                                                       |
-| ssl_cert     | string                        | No       | -                                                                                                                                                                 | for self-signed SSL                                                                                                       |
-| ssl_key      | string                        | No       | -                                                                                                                                                                 | for self-signed SSL                                                                                                       |
-| internal_hostname  | string | No       | -                                                                                                                                                                 | Override match hostname for google cloud                                                                                  |
-| session_sqls | List of strings               | No       | ```['SET @@session.time_zone="+0:00"', 'SET @@session.wait_timeout=28800', 'SET @@session.net_read_timeout=3600', 'SET @@session.innodb_lock_wait_timeout=3600']``` | Set session variables dynamically.                                                                                        |
+| Parameter         | type                          | required | default                                                                                                                                                           | description                                                                                                               |
+|-------------------|-------------------------------|----------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|
+| host              | string                        | yes      | -                                                                                                                                                                 | mysql/mariadb host                                                                                                        |
+| port              | int                           | yes      | -                                                                                                                                                                 | mysql/mariadb port                                                                                                        |
+| user              | string                        | yes      | -                                                                                                                                                                 | db username                                                                                                               |
+| password          | string                        | yes      | -                                                                                                                                                                 | db password                                                                                                               |
+| cursorclass       | string                        | No       | `pymysql.cursors.SSCursor`                                                                                                                                        | set cursorclass used by PyMYSQL                                                                                           |
+| database          | string                        | No       | -                                                                                                                                                                 | Database to use, None to not use a particular one. Used by PyMYSQL                                                        |
+| server_id         | int                           | False    | Randomly generated int                                                                                                                                            | Used as the slave id when this tap is connecting to the server                                                            |
+| filter_dbs        | string                        | False    | -                                                                                                                                                                 | Comma separated list of schemas to extract tables only from particular schemas and to improve data extraction performance |
+| use_gtid          | bool                          | False    | False                                                    <br/>                                                                                                         | Flag to enable log based replication using GTID               |
+| engine            | string ('mysql' or 'mariadb') | False    | 'mysql'                                                                                                                                                           | Indicate which flavor the server is, used for LOG_BASED with GTID                                                         |
+| ssl               | string ("true")               | No       | False                                                                                                                                                             | Enable SSL connection                                                                                                     |
+| ssl_ca            | string                        | No       | -                                                                                                                                                                 | for self-signed SSL                                                                                                       |
+| ssl_cert          | string                        | No       | -                                                                                                                                                                 | for self-signed SSL                                                                                                       |
+| ssl_key           | string                        | No       | -                                                                                                                                                                 | for self-signed SSL                                                                                                       |
+| internal_hostname | string | No       | -                                                                                                                                                                 | Override match hostname for google cloud                                                                                  |
+| session_sqls      | List of strings               | No       | ```['SET @@session.time_zone="+0:00"', 'SET @@session.wait_timeout=28800', 'SET @@session.net_read_timeout=3600', 'SET @@session.innodb_lock_wait_timeout=3600']``` | Set session variables dynamically.                                                                                        |
 
 
 ### Discovery mode
 
 The tap can be invoked in discovery mode to find the available tables and
 columns in the database:
```

### Comparing `pipelinewise-tap-mysql-1.5.2/pipelinewise_tap_mysql.egg-info/PKG-INFO` & `pipelinewise-tap-mysql-1.5.3/pipelinewise_tap_mysql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipelinewise-tap-mysql
-Version: 1.5.2
+Version: 1.5.3
 Summary: Singer.io tap for extracting data from MySQL & MariaDB - PipelineWise compatible
 Home-page: https://github.com/transferwise/pipelinewise-tap-mysql
 Author: Wise
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -73,32 +73,32 @@
 
 ### Create the configuration file
 
 Create a config file containing the database connection credentials, see [sample](config.json.sample).
 
 List of config parameters:
 
-| Parameter    | type                          | required | default                                                                                                                                                           | description                                                                                                               |
-|--------------|-------------------------------|----------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|
-| host         | string                        | yes      | -                                                                                                                                                                 | mysql/mariadb host                                                                                                        |
-| port         | int                           | yes      | -                                                                                                                                                                 | mysql/mariadb port                                                                                                        |
-| user         | string                        | yes      | -                                                                                                                                                                 | db username                                                                                                               |
-| password     | string                        | yes      | -                                                                                                                                                                 | db password                                                                                                               |
-| cursorclass  | string                        | No       | `pymysql.cursors.SSCursor`                                                                                                                                        | set cursorclass used by PyMYSQL                                                                                           |
-| database     | string                        | No       | -                                                                                                                                                                 | Database to use, None to not use a particular one. Used by PyMYSQL                                                        |
-| server_id    | int                           | False    | Randomly generated int                                                                                                                                            | Used as the slave id when this tap is connecting to the server                                                            |
-| filter_db    | string                        | False    | -                                                                                                                                                                 | Comma separated list of schemas to extract tables only from particular schemas and to improve data extraction performance |
-| use_gtid     | bool                          | False    | False                                                    <br/>                                                                                                         | Flag to enable log based replication using GTID               |
-| engine       | string ('mysql' or 'mariadb') | False    | 'mysql'                                                                                                                                                           | Indicate which flavor the server is, used for LOG_BASED with GTID                                                         |
-| ssl          | string ("true")               | No       | False                                                                                                                                                             | Enable SSL connection                                                                                                     |
-| ssl_ca       | string                        | No       | -                                                                                                                                                                 | for self-signed SSL                                                                                                       |
-| ssl_cert     | string                        | No       | -                                                                                                                                                                 | for self-signed SSL                                                                                                       |
-| ssl_key      | string                        | No       | -                                                                                                                                                                 | for self-signed SSL                                                                                                       |
-| internal_hostname  | string | No       | -                                                                                                                                                                 | Override match hostname for google cloud                                                                                  |
-| session_sqls | List of strings               | No       | ```['SET @@session.time_zone="+0:00"', 'SET @@session.wait_timeout=28800', 'SET @@session.net_read_timeout=3600', 'SET @@session.innodb_lock_wait_timeout=3600']``` | Set session variables dynamically.                                                                                        |
+| Parameter         | type                          | required | default                                                                                                                                                           | description                                                                                                               |
+|-------------------|-------------------------------|----------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|
+| host              | string                        | yes      | -                                                                                                                                                                 | mysql/mariadb host                                                                                                        |
+| port              | int                           | yes      | -                                                                                                                                                                 | mysql/mariadb port                                                                                                        |
+| user              | string                        | yes      | -                                                                                                                                                                 | db username                                                                                                               |
+| password          | string                        | yes      | -                                                                                                                                                                 | db password                                                                                                               |
+| cursorclass       | string                        | No       | `pymysql.cursors.SSCursor`                                                                                                                                        | set cursorclass used by PyMYSQL                                                                                           |
+| database          | string                        | No       | -                                                                                                                                                                 | Database to use, None to not use a particular one. Used by PyMYSQL                                                        |
+| server_id         | int                           | False    | Randomly generated int                                                                                                                                            | Used as the slave id when this tap is connecting to the server                                                            |
+| filter_dbs        | string                        | False    | -                                                                                                                                                                 | Comma separated list of schemas to extract tables only from particular schemas and to improve data extraction performance |
+| use_gtid          | bool                          | False    | False                                                    <br/>                                                                                                         | Flag to enable log based replication using GTID               |
+| engine            | string ('mysql' or 'mariadb') | False    | 'mysql'                                                                                                                                                           | Indicate which flavor the server is, used for LOG_BASED with GTID                                                         |
+| ssl               | string ("true")               | No       | False                                                                                                                                                             | Enable SSL connection                                                                                                     |
+| ssl_ca            | string                        | No       | -                                                                                                                                                                 | for self-signed SSL                                                                                                       |
+| ssl_cert          | string                        | No       | -                                                                                                                                                                 | for self-signed SSL                                                                                                       |
+| ssl_key           | string                        | No       | -                                                                                                                                                                 | for self-signed SSL                                                                                                       |
+| internal_hostname | string | No       | -                                                                                                                                                                 | Override match hostname for google cloud                                                                                  |
+| session_sqls      | List of strings               | No       | ```['SET @@session.time_zone="+0:00"', 'SET @@session.wait_timeout=28800', 'SET @@session.net_read_timeout=3600', 'SET @@session.innodb_lock_wait_timeout=3600']``` | Set session variables dynamically.                                                                                        |
 
 
 ### Discovery mode
 
 The tap can be invoked in discovery mode to find the available tables and
 columns in the database:
```

### Comparing `pipelinewise-tap-mysql-1.5.2/setup.py` & `pipelinewise-tap-mysql-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='pipelinewise-tap-mysql',
-      version='1.5.2',
+      version='1.5.3',
       description='Singer.io tap for extracting data from MySQL & MariaDB - PipelineWise compatible',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Wise',
       url='https://github.com/transferwise/pipelinewise-tap-mysql',
       classifiers=[
           'License :: OSI Approved :: GNU Affero General Public License v3',
```

### Comparing `pipelinewise-tap-mysql-1.5.2/tap_mysql/__init__.py` & `pipelinewise-tap-mysql-1.5.3/tap_mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.2/tap_mysql/connection.py` & `pipelinewise-tap-mysql-1.5.3/tap_mysql/connection.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.2/tap_mysql/discover_utils.py` & `pipelinewise-tap-mysql-1.5.3/tap_mysql/discover_utils.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.2/tap_mysql/stream_utils.py` & `pipelinewise-tap-mysql-1.5.3/tap_mysql/stream_utils.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.2/tap_mysql/sync_strategies/binlog.py` & `pipelinewise-tap-mysql-1.5.3/tap_mysql/sync_strategies/binlog.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,32 +8,31 @@
 import socket
 import pymysql.connections
 import pymysql.err
 import pytz
 import singer
 import tzlocal
 
-import tap_mysql.sync_strategies.common as common
-import tap_mysql.connection as connection
-
 from typing import Dict, Set, Union, Optional, Any, Tuple
 from plpygis import Geometry
-from pymysqlreplication import BinLogStreamReader
 from pymysqlreplication.constants import FIELD_TYPE
 from pymysqlreplication.event import RotateEvent, MariadbGtidEvent, GtidEvent
 from pymysqlreplication.row_event import (
     DeleteRowsEvent,
     UpdateRowsEvent,
     WriteRowsEvent,
 )
-
 from singer import utils, Schema, metadata
-from tap_mysql.stream_utils import write_schema_message
-from tap_mysql.discover_utils import discover_catalog, desired_columns, should_run_discovery
+
+from tap_mysql import connection
+from tap_mysql.binlogstream import CustomBinlogStreamReader
 from tap_mysql.connection import connect_with_backoff, make_connection_wrapper, MySQLConnection
+from tap_mysql.discover_utils import discover_catalog, desired_columns, should_run_discovery
+from tap_mysql.stream_utils import write_schema_message
+from tap_mysql.sync_strategies import common
 
 LOGGER = singer.get_logger('tap_mysql')
 
 SDC_DELETED_AT = "_sdc_deleted_at"
 UPDATE_BOOKMARK_PERIOD = 1000
 BOOKMARK_KEYS = {'log_file', 'log_pos', 'version', 'gtid'}
 
@@ -178,18 +177,26 @@
                 LOGGER.info('Using GTID %s for state bookmark', gtid_to_use)
                 return gtid_to_use
 
     raise Exception(f'No suitable GTID was found for server {server}.')
 
 
 def json_bytes_to_string(data):
-    if isinstance(data, bytes):  return data.decode()
-    if isinstance(data, dict):   return dict(map(json_bytes_to_string, data.items()))
-    if isinstance(data, tuple):  return tuple(map(json_bytes_to_string, data))
-    if isinstance(data, list):   return list(map(json_bytes_to_string, data))
+    if isinstance(data, bytes):
+        return data.decode()
+
+    if isinstance(data, dict):
+        return dict(map(json_bytes_to_string, data.items()))
+
+    if isinstance(data, tuple):
+        return tuple(map(json_bytes_to_string, data))
+
+    if isinstance(data, list):
+        return list(map(json_bytes_to_string, data))
+
     return data
 
 
 # pylint: disable=too-many-locals
 def row_to_singer_record(catalog_entry, version, db_column_map, row, time_extracted):
     row_to_persist = {}
 
@@ -580,15 +587,15 @@
 
     return set(binlog_columns_filtered).difference(schema_properties)
 
 
 # pylint: disable=R1702,R0915
 def _run_binlog_sync(
         mysql_conn: MySQLConnection,
-        reader: BinLogStreamReader,
+        reader: CustomBinlogStreamReader,
         binlog_streams_map: Dict,
         state: Dict,
         config: Dict,
         end_log_file: str,
         end_log_pos: int):
 
     processed_rows_events = 0
@@ -635,15 +642,15 @@
             state = update_bookmarks(state,
                                      binlog_streams_map,
                                      binlog_event.next_binlog,
                                      binlog_event.position,
                                      gtid_pos
                                      )
 
-        elif isinstance(binlog_event, MariadbGtidEvent) or isinstance(binlog_event, GtidEvent):
+        elif isinstance(binlog_event, (MariadbGtidEvent, GtidEvent)):
             gtid_pos = binlog_event.gtid
 
             LOGGER.debug('%s: gtid=%s',
                          binlog_event.__class__.__name__,
                          gtid_pos)
 
             state = update_bookmarks(state,
@@ -782,15 +789,15 @@
 
 
 def create_binlog_stream_reader(
         config: Dict,
         log_file: Optional[str],
         log_pos: Optional[int],
         gtid_pos: Optional[str]
-) -> BinLogStreamReader:
+) -> CustomBinlogStreamReader:
     """
     Create an instance of BinlogStreamReader with the right config
 
     Args:
         config: dictionary of the content of tap config.json
         log_file: binlog file name to start replication from (Optional if using gtid)
         log_pos: binlog pos to start replication from (Optional if using gtid)
@@ -813,16 +820,16 @@
         'is_mariadb': connection.MARIADB_ENGINE == engine,
         'server_id': server_id,  # slave server ID
         'report_slave': socket.gethostname() or 'pipelinewise',  # this is so this slave appears in SHOW SLAVE HOSTS;
         'only_events': [WriteRowsEvent, UpdateRowsEvent, DeleteRowsEvent],
     }
 
     # only fetch events pertaining to the schemas in filter db.
-    if config.get('filter_db'):
-        kwargs['only_schemas'] = config['filter_db'].split(',')
+    if config.get('filter_dbs'):
+        kwargs['only_schemas'] = config['filter_dbs'].split(',')
 
     if config['use_gtid']:
 
         if not gtid_pos:
             raise ValueError(f'gtid_pos is empty "{gtid_pos}"! Cannot start logical replication from empty gtid.')
 
         LOGGER.info("Starting logical replication from GTID '%s' on engine '%s'", gtid_pos, engine)
@@ -840,15 +847,15 @@
 
         # When not using GTID, we want to listen in for rotate events, and start from given log position and file
         kwargs['only_events'].append(RotateEvent)
         kwargs['log_file'] = log_file
         kwargs['log_pos'] = log_pos
         kwargs['resume_stream'] = True
 
-    return BinLogStreamReader(**kwargs)
+    return CustomBinlogStreamReader(**kwargs)
 
 
 def sync_binlog_stream(
         mysql_conn: MySQLConnection,
         config: Dict,
         binlog_streams_map: Dict[str, Any],
         state: Dict) -> None:
@@ -877,22 +884,14 @@
         reader = create_binlog_stream_reader(config, log_file, log_pos, gtid)
 
         end_log_file, end_log_pos = fetch_current_log_file_and_pos(mysql_conn)
         LOGGER.info('Current Master binlog file and pos: %s %s', end_log_file, end_log_pos)
 
         _run_binlog_sync(mysql_conn, reader, binlog_streams_map, state, config, end_log_file, end_log_pos)
 
-    except pymysql.err.OperationalError as ex:
-        if ex.args[0] == 1236:
-            LOGGER.error('Cannot resume logical replication from given GTID %s! This GTID might date back to before '
-                         'the new primary has been setup, connect to old primary and consume all binlog events to get '
-                         'a newer GTID then switch back.', gtid)
-
-        raise
-
     finally:
         # BinLogStreamReader doesn't implement the `with` methods
         # So, try/finally will close the chain from the top
         if reader:
             reader.close()
 
     singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
```

### Comparing `pipelinewise-tap-mysql-1.5.2/tap_mysql/sync_strategies/common.py` & `pipelinewise-tap-mysql-1.5.3/tap_mysql/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.2/tap_mysql/sync_strategies/full_table.py` & `pipelinewise-tap-mysql-1.5.3/tap_mysql/sync_strategies/full_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 # pylint: disable=too-many-locals,missing-function-docstring
 
 import singer
 
 from singer import metadata
 
-import tap_mysql.sync_strategies.binlog as binlog
-import tap_mysql.sync_strategies.common as common
+from tap_mysql.sync_strategies import binlog
+from tap_mysql.sync_strategies import common
 
 from tap_mysql.connection import connect_with_backoff
 
 LOGGER = singer.get_logger('tap_mysql')
 
 
 def generate_bookmark_keys(catalog_entry):
@@ -98,25 +98,21 @@
                                         'max_pk_values')
 
     last_pk_fetched = singer.get_bookmark(state,
                                           catalog_entry.tap_stream_id,
                                           'last_pk_fetched')
 
     if last_pk_fetched:
-        pk_comparisons = ["({} > {} AND {} <= {})".format(common.escape(pk),
-                                                          last_pk_fetched[pk],
-                                                          common.escape(pk),
-                                                          max_pk_values[pk])
-                          for pk in key_properties]
+        pk_comparisons = [
+            f"({common.escape(pk)} > {last_pk_fetched[pk]} AND {common.escape(pk)} <= {max_pk_values[pk]})"
+            for pk in key_properties]
     else:
-        pk_comparisons = ["{} <= {}".format(common.escape(pk), max_pk_values[pk])
-                          for pk in key_properties]
+        pk_comparisons = [f"{common.escape(pk)} <= {max_pk_values[pk]}" for pk in key_properties]
 
-    sql = " WHERE {} ORDER BY {} ASC".format(" AND ".join(pk_comparisons),
-                                             ", ".join(escaped_columns))
+    sql = f' WHERE {" AND ".join(pk_comparisons)} ORDER BY {", ".join(escaped_columns)} ASC'
 
     return sql
 
 
 def sync_table(mysql_conn, catalog_entry, state, columns, stream_version):
     common.whitelist_bookmark_keys(generate_bookmark_keys(catalog_entry), catalog_entry.tap_stream_id, state)
 
@@ -163,14 +159,15 @@
 
                     pk_clause = generate_pk_clause(catalog_entry, state)
 
                     select_sql += pk_clause
 
             params = {}
 
+            # pylint:disable=duplicate-code
             common.sync_query(cur,
                               catalog_entry,
                               state,
                               select_sql,
                               columns,
                               stream_version,
                               params)
```

### Comparing `pipelinewise-tap-mysql-1.5.2/tap_mysql/sync_strategies/incremental.py` & `pipelinewise-tap-mysql-1.5.3/tap_mysql/sync_strategies/incremental.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # pylint: disable=missing-function-docstring
 
 import pendulum
 import singer
 from singer import metadata
 
 from tap_mysql.connection import connect_with_backoff
-import tap_mysql.sync_strategies.common as common
+from tap_mysql.sync_strategies import common
 
 
 BOOKMARK_KEYS = {'replication_key', 'replication_key_value', 'version'}
 
 
 def sync_table(mysql_conn, catalog_entry, state, columns):
     common.whitelist_bookmark_keys(BOOKMARK_KEYS, catalog_entry.tap_stream_id, state)
@@ -59,15 +59,15 @@
                     replication_key_value = pendulum.parse(replication_key_value)
 
                 select_sql += f" WHERE `{replication_key_metadata}` >= %(replication_key_value)s " \
                               f"ORDER BY `{replication_key_metadata}` ASC"
 
                 params['replication_key_value'] = replication_key_value
             elif replication_key_metadata is not None:
-                select_sql += ' ORDER BY `{}` ASC'.format(replication_key_metadata)
+                select_sql += f' ORDER BY `{replication_key_metadata}` ASC'
 
             common.sync_query(cur,
                               catalog_entry,
                               state,
                               select_sql,
                               columns,
                               stream_version,
```

