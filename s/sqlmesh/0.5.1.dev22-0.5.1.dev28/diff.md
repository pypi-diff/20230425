# Comparing `tmp/sqlmesh-0.5.1.dev22.tar.gz` & `tmp/sqlmesh-0.5.1.dev28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmesh-0.5.1.dev22.tar", last modified: Mon Apr 24 17:52:38 2023, max compression
+gzip compressed data, was "sqlmesh-0.5.1.dev28.tar", last modified: Mon Apr 24 23:32:11 2023, max compression
```

## Comparing `sqlmesh-0.5.1.dev22.tar` & `sqlmesh-0.5.1.dev28.tar`

### file list

```diff
@@ -1,734 +1,735 @@
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.807886 sqlmesh-0.5.1.dev22/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.617271 sqlmesh-0.5.1.dev22/.circleci/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1872 2023-04-17 00:43:26.000000 sqlmesh-0.5.1.dev22/.circleci/config.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4414 2023-04-17 00:43:26.000000 sqlmesh-0.5.1.dev22/.circleci/continue_config.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)       66 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/.dockerignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2152 2023-04-17 00:43:26.000000 sqlmesh-0.5.1.dev22/.gitignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1900 2023-03-27 22:28:21.000000 sqlmesh-0.5.1.dev22/.pre-commit-config.yaml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      234 2023-03-31 20:18:29.000000 sqlmesh-0.5.1.dev22/.readthedocs.yaml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      135 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/Dockerfile.api
--rw-r--r--   0 eakmanrq   (501) staff       (20)      383 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/Dockerfile.app
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11346 2023-03-21 00:57:17.000000 sqlmesh-0.5.1.dev22/LICENSE
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1855 2023-04-14 19:58:28.000000 sqlmesh-0.5.1.dev22/Makefile
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2202 2023-04-24 17:52:38.808010 sqlmesh-0.5.1.dev22/PKG-INFO
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1250 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/README.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1008 2023-04-24 17:50:28.000000 sqlmesh-0.5.1.dev22/docker-compose.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.619209 sqlmesh-0.5.1.dev22/docs/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.601480 sqlmesh-0.5.1.dev22/docs/_readthedocs/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.619483 sqlmesh-0.5.1.dev22/docs/_readthedocs/html/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-31 20:18:29.000000 sqlmesh-0.5.1.dev22/docs/_readthedocs/html/.keep
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9965 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/docs/comparisons.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.620820 sqlmesh-0.5.1.dev22/docs/concepts/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.621397 sqlmesh-0.5.1.dev22/docs/concepts/architecture/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1334 2023-03-27 03:14:49.000000 sqlmesh-0.5.1.dev22/docs/concepts/architecture/serialization.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1113 2023-03-27 03:14:49.000000 sqlmesh-0.5.1.dev22/docs/concepts/architecture/snapshots.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6689 2023-04-20 16:12:45.000000 sqlmesh-0.5.1.dev22/docs/concepts/audits.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3866 2023-03-27 03:14:49.000000 sqlmesh-0.5.1.dev22/docs/concepts/environments.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5952 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/docs/concepts/glossary.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)       13 2023-03-27 03:14:49.000000 sqlmesh-0.5.1.dev22/docs/concepts/hooks.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3027 2023-03-27 03:14:49.000000 sqlmesh-0.5.1.dev22/docs/concepts/macros.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.622480 sqlmesh-0.5.1.dev22/docs/concepts/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9934 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/docs/concepts/models/model_kinds.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7859 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/docs/concepts/models/overview.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7171 2023-03-27 03:14:56.000000 sqlmesh-0.5.1.dev22/docs/concepts/models/python_models.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4938 2023-03-27 03:14:56.000000 sqlmesh-0.5.1.dev22/docs/concepts/models/seed_models.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5356 2023-03-27 03:14:56.000000 sqlmesh-0.5.1.dev22/docs/concepts/models/sql_models.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6637 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/docs/concepts/overview.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.622646 sqlmesh-0.5.1.dev22/docs/concepts/plans/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    43124 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/docs/concepts/plans/model_versioning.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8973 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/docs/concepts/plans.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5699 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/docs/concepts/tests.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      607 2023-04-14 19:58:28.000000 sqlmesh-0.5.1.dev22/docs/development.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.624369 sqlmesh-0.5.1.dev22/docs/guides/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1943 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/docs/guides/connections.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1309 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/docs/guides/migrations.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10756 2023-04-06 22:49:28.000000 sqlmesh-0.5.1.dev22/docs/guides/models.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6133 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/docs/guides/multi_repo.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2142 2023-04-20 16:12:45.000000 sqlmesh-0.5.1.dev22/docs/guides/projects.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.625582 sqlmesh-0.5.1.dev22/docs/guides/scheduling/
--rw-r--r--   0 eakmanrq   (501) staff       (20)   740917 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/docs/guides/scheduling/airflow_successful_plan_apply.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   379880 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/docs/guides/scheduling/airflow_successful_setup.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5648 2023-03-27 03:14:49.000000 sqlmesh-0.5.1.dev22/docs/guides/scheduling.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1854 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/docs/guides/testing.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5517 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/docs/index.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      297 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/docs/installation.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.627955 sqlmesh-0.5.1.dev22/docs/integrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2905 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/docs/integrations/airflow.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7801 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/docs/integrations/dbt.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)    24125 2023-04-24 16:27:17.000000 sqlmesh-0.5.1.dev22/docs/integrations/engines.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      925 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/docs/integrations/github.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      217 2023-03-27 01:55:02.000000 sqlmesh-0.5.1.dev22/docs/integrations/overview.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      665 2023-03-28 15:29:23.000000 sqlmesh-0.5.1.dev22/docs/prerequisites.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10781 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/docs/quick_start.md
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.629805 sqlmesh-0.5.1.dev22/docs/reference/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6093 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/docs/reference/cli.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13607 2023-04-24 15:46:04.000000 sqlmesh-0.5.1.dev22/docs/reference/configuration.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4579 2023-04-20 16:12:45.000000 sqlmesh-0.5.1.dev22/docs/reference/notebook.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1127 2023-03-27 03:14:49.000000 sqlmesh-0.5.1.dev22/docs/reference/overview.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)       14 2023-03-27 03:14:49.000000 sqlmesh-0.5.1.dev22/docs/reference/python.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)       16 2023-03-27 03:14:49.000000 sqlmesh-0.5.1.dev22/docs/release_notes.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      122 2023-03-31 20:18:29.000000 sqlmesh-0.5.1.dev22/docs/requirements.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3249 2023-03-27 01:55:02.000000 sqlmesh-0.5.1.dev22/docs/sqlmesh.png
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.630094 sqlmesh-0.5.1.dev22/examples/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.631922 sqlmesh-0.5.1.dev22/examples/airflow/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1713 2023-04-08 22:07:58.000000 sqlmesh-0.5.1.dev22/examples/airflow/Dockerfile.template
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2164 2023-04-14 19:58:28.000000 sqlmesh-0.5.1.dev22/examples/airflow/Makefile
--rw-r--r--   0 eakmanrq   (501) staff       (20)      942 2023-01-20 19:02:18.000000 sqlmesh-0.5.1.dev22/examples/airflow/README.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/airflow/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.632236 sqlmesh-0.5.1.dev22/examples/airflow/dags/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      263 2023-03-21 21:04:44.000000 sqlmesh-0.5.1.dev22/examples/airflow/dags/sqlmesh_integration.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3515 2023-04-08 22:07:58.000000 sqlmesh-0.5.1.dev22/examples/airflow/docker_compose_decorator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)       12 2023-01-20 19:02:18.000000 sqlmesh-0.5.1.dev22/examples/airflow/requirements.txt
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.635138 sqlmesh-0.5.1.dev22/examples/airflow/spark_conf/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      872 2023-01-20 19:02:18.000000 sqlmesh-0.5.1.dev22/examples/airflow/spark_conf/hive-site.xml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      151 2023-01-20 19:02:18.000000 sqlmesh-0.5.1.dev22/examples/airflow/spark_conf/spark-defaults.conf
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.602778 sqlmesh-0.5.1.dev22/examples/multi/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.635509 sqlmesh-0.5.1.dev22/examples/multi/repo_1/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.635826 sqlmesh-0.5.1.dev22/examples/multi/repo_1/audits/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/examples/multi/repo_1/audits/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      108 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/examples/multi/repo_1/config.yaml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.636274 sqlmesh-0.5.1.dev22/examples/multi/repo_1/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/examples/multi/repo_1/macros/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/examples/multi/repo_1/macros/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.637049 sqlmesh-0.5.1.dev22/examples/multi/repo_1/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/examples/multi/repo_1/models/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)       63 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/examples/multi/repo_1/models/a.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       53 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/examples/multi/repo_1/models/b.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.637324 sqlmesh-0.5.1.dev22/examples/multi/repo_1/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/examples/multi/repo_1/tests/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.637538 sqlmesh-0.5.1.dev22/examples/multi/repo_2/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.637760 sqlmesh-0.5.1.dev22/examples/multi/repo_2/audits/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/examples/multi/repo_2/audits/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      113 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/examples/multi/repo_2/config.yaml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.638018 sqlmesh-0.5.1.dev22/examples/multi/repo_2/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/examples/multi/repo_2/macros/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/examples/multi/repo_2/macros/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.638663 sqlmesh-0.5.1.dev22/examples/multi/repo_2/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/examples/multi/repo_2/models/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)       64 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/examples/multi/repo_2/models/c.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       53 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/examples/multi/repo_2/models/d.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.638863 sqlmesh-0.5.1.dev22/examples/multi/repo_2/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/examples/multi/repo_2/tests/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.639460 sqlmesh-0.5.1.dev22/examples/sushi/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.5.1.dev22/examples/sushi/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.640528 sqlmesh-0.5.1.dev22/examples/sushi/audits/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      105 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi/audits/items.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      119 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi/audits/order_items.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      829 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/examples/sushi/config.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.640937 sqlmesh-0.5.1.dev22/examples/sushi/data/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-06 17:30:39.000000 sqlmesh-0.5.1.dev22/examples/sushi/data/.keep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      551 2023-01-20 19:02:18.000000 sqlmesh-0.5.1.dev22/examples/sushi/helper.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.641166 sqlmesh-0.5.1.dev22/examples/sushi/hooks/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi/hooks/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      247 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi/hooks/hooks.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.641617 sqlmesh-0.5.1.dev22/examples/sushi/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.5.1.dev22/examples/sushi/macros/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      702 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi/macros/macros.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.644491 sqlmesh-0.5.1.dev22/examples/sushi/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      916 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/examples/sushi/models/customer_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      204 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi/models/customers.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1910 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/examples/sushi/models/items.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1911 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/examples/sushi/models/order_items.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1642 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/examples/sushi/models/orders.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      346 2023-04-11 16:01:14.000000 sqlmesh-0.5.1.dev22/examples/sushi/models/top_waiters.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      465 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/examples/sushi/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      123 2023-02-17 23:03:10.000000 sqlmesh-0.5.1.dev22/examples/sushi/models/waiter_names.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      691 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/examples/sushi/models/waiter_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      197 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi/models/waiters.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.644664 sqlmesh-0.5.1.dev22/examples/sushi/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       88 2023-01-20 19:02:18.000000 sqlmesh-0.5.1.dev22/examples/sushi/seeds/waiter_names.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.644892 sqlmesh-0.5.1.dev22/examples/sushi/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1459 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi/tests/test_customer_revenue_by_day.yaml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.645894 sqlmesh-0.5.1.dev22/examples/sushi_dbt/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       15 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/.gitignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)       41 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/.user.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.646168 sqlmesh-0.5.1.dev22/examples/sushi_dbt/analyses/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/analyses/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      291 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/config.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      507 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/dbt_project.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.646422 sqlmesh-0.5.1.dev22/examples/sushi_dbt/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      941 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/macros/incremental.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       80 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/macros/log_value.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.647633 sqlmesh-0.5.1.dev22/examples/sushi_dbt/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1125 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/models/customer_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       80 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/models/customers.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      182 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/models/schema.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      309 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/models/top_waiters.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      389 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      752 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/models/waiter_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      186 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/models/waiters.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.603745 sqlmesh-0.5.1.dev22/examples/sushi_dbt/packages/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.647795 sqlmesh-0.5.1.dev22/examples/sushi_dbt/packages/customers/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.647971 sqlmesh-0.5.1.dev22/examples/sushi_dbt/packages/customers/analyses/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/packages/customers/analyses/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      663 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/packages/customers/dbt_project.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.648230 sqlmesh-0.5.1.dev22/examples/sushi_dbt/packages/customers/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      117 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/packages/customers/macros/current_engine.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       65 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/packages/customers/macros/distinct.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.648367 sqlmesh-0.5.1.dev22/examples/sushi_dbt/packages/customers/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/packages/customers/models/schema.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.648455 sqlmesh-0.5.1.dev22/examples/sushi_dbt/packages/customers/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/packages/customers/seeds/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.648539 sqlmesh-0.5.1.dev22/examples/sushi_dbt/packages/customers/snapshots/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/packages/customers/snapshots/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.648629 sqlmesh-0.5.1.dev22/examples/sushi_dbt/packages/customers/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/packages/customers/tests/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      783 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/profiles.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.659017 sqlmesh-0.5.1.dev22/examples/sushi_dbt/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2327 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/seeds/items.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10472 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/seeds/order_items.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9746 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/seeds/orders.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)       97 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/seeds/properties.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)       88 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/seeds/waiter_names.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.659274 sqlmesh-0.5.1.dev22/examples/sushi_dbt/snapshots/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/snapshots/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.659389 sqlmesh-0.5.1.dev22/examples/sushi_dbt/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.5.1.dev22/examples/sushi_dbt/tests/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.659610 sqlmesh-0.5.1.dev22/examples/wursthall/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/wursthall/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.604445 sqlmesh-0.5.1.dev22/examples/wursthall/audits/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.659867 sqlmesh-0.5.1.dev22/examples/wursthall/audits/db/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      141 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/wursthall/audits/db/order_f.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       66 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/wursthall/config.yaml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.660175 sqlmesh-0.5.1.dev22/examples/wursthall/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/wursthall/macros/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      618 2023-04-06 22:49:28.000000 sqlmesh-0.5.1.dev22/examples/wursthall/macros/macros.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.660435 sqlmesh-0.5.1.dev22/examples/wursthall/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/wursthall/models/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.661169 sqlmesh-0.5.1.dev22/examples/wursthall/models/db/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      433 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/examples/wursthall/models/db/customer_d.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      256 2023-04-06 22:49:28.000000 sqlmesh-0.5.1.dev22/examples/wursthall/models/db/item_d.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3161 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/examples/wursthall/models/db/order_f.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      542 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/examples/wursthall/models/db/order_item_f.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.662120 sqlmesh-0.5.1.dev22/examples/wursthall/models/src/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/wursthall/models/src/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1672 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/examples/wursthall/models/src/customer_details.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      120 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/wursthall/models/src/menu_item_details.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3434 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/examples/wursthall/models/src/order_item_details.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      892 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/wursthall/models/src/shared.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.604761 sqlmesh-0.5.1.dev22/examples/wursthall/seeds/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.662291 sqlmesh-0.5.1.dev22/examples/wursthall/seeds/src/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7416 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/wursthall/seeds/src/menu_item_details.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.662676 sqlmesh-0.5.1.dev22/examples/wursthall/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      888 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/wursthall/tests/test_customer_d.yaml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      955 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/examples/wursthall/tests/test_order_item_f.yaml
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2113 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/mkdocs.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.662863 sqlmesh-0.5.1.dev22/pdoc/
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)     1153 2023-03-28 16:31:06.000000 sqlmesh-0.5.1.dev22/pdoc/cli.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.663286 sqlmesh-0.5.1.dev22/pdoc/templates/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      131 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/pdoc/templates/module.html.jinja2
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.663619 sqlmesh-0.5.1.dev22/posts/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.667110 sqlmesh-0.5.1.dev22/posts/virtual_data_environments/
--rw-r--r--   0 eakmanrq   (501) staff       (20)   318753 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/posts/virtual_data_environments/change_categorization.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   274526 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/posts/virtual_data_environments/isolated_rigid_envs.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   163619 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/posts/virtual_data_environments/partial_breaking.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   298971 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/posts/virtual_data_environments/stateful_envs.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)   366545 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/posts/virtual_data_environments/virtual_envs.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)  1344487 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/posts/virtual_data_environments/virtual_envs_end_to_end.png
--rw-r--r--   0 eakmanrq   (501) staff       (20)    18696 2023-04-19 01:45:56.000000 sqlmesh-0.5.1.dev22/posts/virtual_data_environments.md
--rw-r--r--   0 eakmanrq   (501) staff       (20)      734 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/pytest.ini
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1393 2023-04-24 17:52:38.808519 sqlmesh-0.5.1.dev22/setup.cfg
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3158 2023-04-24 17:50:35.000000 sqlmesh-0.5.1.dev22/setup.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.671310 sqlmesh-0.5.1.dev22/sqlmesh/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        3 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/sqlmesh/.airflowignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3950 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      175 2023-04-24 17:52:38.000000 sqlmesh-0.5.1.dev22/sqlmesh/_version.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.673266 sqlmesh-0.5.1.dev22/sqlmesh/cli/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      898 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/cli/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4314 2023-04-06 22:49:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/cli/example_project.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9641 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/cli/main.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1433 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/cli/options.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.681118 sqlmesh-0.5.1.dev22/sqlmesh/core/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      586 2023-03-15 16:48:19.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/_typing.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.681922 sqlmesh-0.5.1.dev22/sqlmesh/core/audit/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      449 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/audit/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1071 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/audit/builtin.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8136 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/audit/definition.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.684291 sqlmesh-0.5.1.dev22/sqlmesh/core/config/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      668 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/config/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4412 2023-04-14 19:58:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/config/base.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1001 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/config/categorizer.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      940 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/config/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    21184 2023-04-24 16:27:17.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/config/connection.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3351 2023-04-20 16:12:45.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/config/loader.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1655 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/config/model.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5611 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/config/root.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8421 2023-04-24 15:25:03.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/config/scheduler.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    29242 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/console.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      735 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/constants.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    36030 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/context.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8612 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/context_diff.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    17626 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/dialect.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.688002 sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2626 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      762 2023-01-17 23:57:22.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/_typing.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    29021 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/base.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4191 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/base_postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4238 2023-04-14 22:30:56.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/base_spark.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15694 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/bigquery.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      402 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/databricks.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1939 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/databricks_api.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1971 2023-04-14 18:08:36.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/duckdb.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2149 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6650 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/redshift.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1181 2023-03-31 20:18:23.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/shared.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2658 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/snowflake.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4131 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/spark.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1815 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/environment.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      742 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/hooks.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    12521 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/loader.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    18920 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/macros.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.690054 sqlmesh-0.5.1.dev22/sqlmesh/core/model/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      594 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/model/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1746 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/model/cache.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1300 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/model/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2417 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/model/decorator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    47586 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/model/definition.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8168 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/model/kind.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    12453 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/model/meta.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2017 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/model/seed.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2314 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/notification_target.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.690730 sqlmesh-0.5.1.dev22/sqlmesh/core/plan/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      191 2022-12-27 18:08:03.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/plan/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    24916 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/plan/definition.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8075 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/plan/evaluator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    12623 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/renderer.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15386 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/scheduler.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    20418 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/schema_diff.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.691617 sqlmesh-0.5.1.dev22/sqlmesh/core/snapshot/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      527 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/snapshot/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1990 2023-03-27 01:55:02.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/snapshot/categorizer.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    32727 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/snapshot/definition.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    19093 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/snapshot/evaluator.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.697351 sqlmesh-0.5.1.dev22/sqlmesh/core/state_sync/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      692 2023-04-14 19:58:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/state_sync/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13080 2023-04-14 19:58:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/state_sync/base.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    12222 2023-04-14 19:58:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/state_sync/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    20048 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/state_sync/engine_adapter.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10834 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/test.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1412 2023-04-24 15:25:03.000000 sqlmesh-0.5.1.dev22/sqlmesh/core/user.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.700487 sqlmesh-0.5.1.dev22/sqlmesh/dbt/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       79 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/dbt/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9390 2023-04-14 22:30:56.000000 sqlmesh-0.5.1.dev22/sqlmesh/dbt/adapter.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15659 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/dbt/basemodel.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11231 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/dbt/builtin.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1969 2023-03-21 00:57:17.000000 sqlmesh-0.5.1.dev22/sqlmesh/dbt/column.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4749 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/dbt/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5143 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/dbt/context.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7950 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/dbt/loader.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9209 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/dbt/model.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13030 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/dbt/package.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3561 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/dbt/profile.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4772 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/dbt/project.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1080 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/dbt/seed.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3137 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/dbt/source.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    12439 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/dbt/target.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      291 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/dbt/util.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.700832 sqlmesh-0.5.1.dev22/sqlmesh/engines/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/sqlmesh/engines/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4437 2023-03-22 20:26:36.000000 sqlmesh-0.5.1.dev22/sqlmesh/engines/commands.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.701188 sqlmesh-0.5.1.dev22/sqlmesh/engines/spark/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/sqlmesh/engines/spark/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3414 2023-03-22 20:32:25.000000 sqlmesh-0.5.1.dev22/sqlmesh/engines/spark/app.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.701793 sqlmesh-0.5.1.dev22/sqlmesh/engines/spark/db_api/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/sqlmesh/engines/spark/db_api/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      148 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/sqlmesh/engines/spark/db_api/errors.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2571 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/engines/spark/db_api/spark_session.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.702007 sqlmesh-0.5.1.dev22/sqlmesh/integrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/sqlmesh/integrations/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.702671 sqlmesh-0.5.1.dev22/sqlmesh/integrations/github/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/sqlmesh/integrations/github/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2210 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/integrations/github/notification_operator_provider.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1726 2023-01-20 19:02:18.000000 sqlmesh-0.5.1.dev22/sqlmesh/integrations/github/notification_target.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1829 2023-01-18 17:26:59.000000 sqlmesh-0.5.1.dev22/sqlmesh/integrations/github/shared.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    13754 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/magics.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.703362 sqlmesh-0.5.1.dev22/sqlmesh/migrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-14 19:58:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/migrations/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1749 2023-04-14 19:58:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/migrations/v0001_init.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      103 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/migrations/v0002_remove_identify.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1183 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/migrations/v0003_move_batch_size.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/sqlmesh/py.typed
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.703584 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.705544 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-05 17:38:29.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4020 2023-04-14 19:58:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/api.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8053 2023-04-14 19:58:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/client.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3830 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/common.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    18799 2023-03-22 20:33:19.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/dag_generator.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.706404 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/hooks/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-15 19:26:11.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/hooks/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2132 2023-03-22 20:54:22.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/hooks/bigquery.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      868 2023-03-22 20:54:22.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/hooks/redshift.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8508 2023-03-22 20:33:52.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/integration.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.708866 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/operators/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/operators/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1444 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/operators/bigquery.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6307 2023-03-22 20:26:36.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/operators/databricks.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2549 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/operators/hwm_sensor.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      877 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/operators/notification.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1322 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/operators/postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1211 2023-01-20 20:10:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/operators/redshift.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1340 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/operators/snowflake.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5222 2023-03-22 20:26:36.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/operators/spark_submit.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11031 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/operators/targets.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4400 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/plan.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1292 2023-04-14 19:58:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/plugin.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4139 2023-04-14 19:58:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/state_sync.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5213 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/util.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.712591 sqlmesh-0.5.1.dev22/sqlmesh/utils/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4378 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/utils/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3593 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/utils/cache.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8053 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/utils/concurrency.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7530 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/utils/connection_pool.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      410 2022-12-30 00:03:50.000000 sqlmesh-0.5.1.dev22/sqlmesh/utils/conversions.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4329 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/utils/dag.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7549 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/sqlmesh/utils/date.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1244 2023-04-24 15:25:03.000000 sqlmesh-0.5.1.dev22/sqlmesh/utils/errors.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    16084 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/utils/jinja.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15093 2023-04-06 22:49:28.000000 sqlmesh-0.5.1.dev22/sqlmesh/utils/metaprogramming.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      888 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/utils/pandas.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1609 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/utils/pydantic.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1534 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/utils/rich.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6487 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/sqlmesh/utils/transactional_file.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1301 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/sqlmesh/utils/yaml.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.671990 sqlmesh-0.5.1.dev22/sqlmesh.egg-info/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2202 2023-04-24 17:52:38.000000 sqlmesh-0.5.1.dev22/sqlmesh.egg-info/PKG-INFO
--rw-r--r--   0 eakmanrq   (501) staff       (20)    21315 2023-04-24 17:52:38.000000 sqlmesh-0.5.1.dev22/sqlmesh.egg-info/SOURCES.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)        1 2023-04-24 17:52:38.000000 sqlmesh-0.5.1.dev22/sqlmesh.egg-info/dependency_links.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)      142 2023-04-24 17:52:38.000000 sqlmesh-0.5.1.dev22/sqlmesh.egg-info/entry_points.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)      838 2023-04-24 17:52:38.000000 sqlmesh-0.5.1.dev22/sqlmesh.egg-info/requires.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)       12 2023-04-24 17:52:38.000000 sqlmesh-0.5.1.dev22/sqlmesh.egg-info/top_level.txt
--rw-r--r--   0 eakmanrq   (501) staff       (20)    21020 2023-03-27 03:14:56.000000 sqlmesh-0.5.1.dev22/sqlmesh.svg
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.713134 sqlmesh-0.5.1.dev22/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/tests/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      285 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/tests/common_fixtures.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3741 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/tests/conftest.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.721453 sqlmesh-0.5.1.dev22/tests/core/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/tests/core/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.724269 sqlmesh-0.5.1.dev22/tests/core/engine_adapter/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/tests/core/engine_adapter/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    27881 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/tests/core/engine_adapter/test_base.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2114 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/tests/core/engine_adapter/test_base_postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1270 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/tests/core/engine_adapter/test_base_spark.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7171 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/tests/core/engine_adapter/test_bigquery.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1253 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/tests/core/engine_adapter/test_databricks.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2613 2023-01-17 20:15:22.000000 sqlmesh-0.5.1.dev22/tests/core/engine_adapter/test_duckdb.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1569 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/tests/core/engine_adapter/test_postgres.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8036 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/tests/core/engine_adapter/test_redshift.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3191 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/tests/core/engine_adapter/test_spark.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     7073 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/tests/core/test_audit.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6611 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/tests/core/test_config.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      850 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/core/test_connection_config.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10197 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/tests/core/test_context.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2749 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/tests/core/test_dialect.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      464 2022-12-28 16:53:44.000000 sqlmesh-0.5.1.dev22/tests/core/test_environment.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    26764 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/tests/core/test_integration.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5880 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/tests/core/test_macros.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    25301 2023-04-24 17:50:35.000000 sqlmesh-0.5.1.dev22/tests/core/test_model.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15280 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/tests/core/test_plan.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3824 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/tests/core/test_plan_evaluator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4557 2023-04-14 19:58:28.000000 sqlmesh-0.5.1.dev22/tests/core/test_scheduler.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    32235 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/tests/core/test_schema_diff.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      857 2023-01-06 18:44:22.000000 sqlmesh-0.5.1.dev22/tests/core/test_seed.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    28291 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/tests/core/test_snapshot.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9870 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/tests/core/test_snapshot_evaluator.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    21868 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/tests/core/test_state_sync.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.725169 sqlmesh-0.5.1.dev22/tests/dbt/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-16 20:33:14.000000 sqlmesh-0.5.1.dev22/tests/dbt/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      636 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/tests/dbt/conftest.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2537 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/tests/dbt/test_adapter.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    12939 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/tests/dbt/test_config.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    16968 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/tests/dbt/test_transformation.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.725452 sqlmesh-0.5.1.dev22/tests/engines/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/tests/engines/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.726021 sqlmesh-0.5.1.dev22/tests/engines/spark/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/tests/engines/spark/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      357 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/tests/engines/spark/conftest.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1503 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/tests/engines/spark/test_db_api.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.610768 sqlmesh-0.5.1.dev22/tests/fixtures/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.606771 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.727309 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.727564 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/analyses/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/analyses/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      291 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/config.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.606930 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/dbt_packages/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1055 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/dbt_project.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.727696 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/logs/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10264 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.728043 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      941 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/macros/incremental.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       80 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/macros/log_value.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.728884 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      247 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/models/schema.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      334 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/models/top_waiters.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      389 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/models/waiter_as_customer_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      863 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      196 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/models/waiters.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.607316 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.729043 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages/customers/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.729232 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages/customers/analyses/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages/customers/analyses/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)      663 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.729560 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages/customers/macros/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      117 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages/customers/macros/current_engine.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)       65 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages/customers/macros/distinct.sql
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.730465 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages/customers/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1155 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      108 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages/customers/models/customers.sql
--rw-r--r--   0 eakmanrq   (501) staff       (20)      193 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages/customers/models/schema.yml
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.730701 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages/customers/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages/customers/seeds/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.731159 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.731263 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages/customers/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages/customers/tests/.gitkeep
--rw-r--r--   0 eakmanrq   (501) staff       (20)       41 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)      540 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/profiles.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1250 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/seed_sources.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.731524 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/seeds/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       42 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/seeds/properties.yml
--rw-r--r--   0 eakmanrq   (501) staff       (20)       88 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/seeds/waiter_names.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.731688 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/snapshots/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/snapshots/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.732113 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/source_data/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2327 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/source_data/items.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10472 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/source_data/order_items.csv
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9746 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/source_data/orders.csv
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.732260 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/tests/.gitkeep
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.732564 sqlmesh-0.5.1.dev22/tests/fixtures/migrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9823 2023-04-14 19:58:28.000000 sqlmesh-0.5.1.dev22/tests/fixtures/migrations/environments.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)    25229 2023-04-14 19:58:28.000000 sqlmesh-0.5.1.dev22/tests/fixtures/migrations/snapshots.json
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.733011 sqlmesh-0.5.1.dev22/tests/integrations/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/tests/integrations/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.733281 sqlmesh-0.5.1.dev22/tests/integrations/github/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/tests/integrations/github/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.733619 sqlmesh-0.5.1.dev22/tests/integrations/github/fixtures/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      816 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/tests/integrations/github/fixtures/pull_request_review.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)      477 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/tests/integrations/github/test_notification_target.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.733797 sqlmesh-0.5.1.dev22/tests/schedulers/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/tests/schedulers/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.735005 sqlmesh-0.5.1.dev22/tests/schedulers/airflow/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/tests/schedulers/airflow/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1414 2023-01-20 19:02:18.000000 sqlmesh-0.5.1.dev22/tests/schedulers/airflow/conftest.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.743248 sqlmesh-0.5.1.dev22/tests/schedulers/airflow/operators/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/tests/schedulers/airflow/operators/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3866 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/tests/schedulers/airflow/operators/test_hwm_sensor.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4280 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/tests/schedulers/airflow/operators/test_targets.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9704 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/tests/schedulers/airflow/test_client.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1345 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/tests/schedulers/airflow/test_end_to_end.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6035 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/tests/schedulers/airflow/test_integration.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5785 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/tests/schedulers/airflow/test_plan.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.746344 sqlmesh-0.5.1.dev22/tests/utils/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/tests/utils/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1118 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/tests/utils/test_cache.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3580 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/tests/utils/test_concurrency.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6430 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/tests/utils/test_connection_pool.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1381 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/tests/utils/test_dag.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1818 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/tests/utils/test_date.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      551 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/tests/utils/test_filesystem.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5516 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/tests/utils/test_jinja.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5790 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/tests/utils/test_metaprogramming.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2501 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/tests/utils/test_pandas.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      518 2022-12-05 19:41:13.000000 sqlmesh-0.5.1.dev22/tests/utils/test_pydantic.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2911 2023-04-17 00:43:26.000000 sqlmesh-0.5.1.dev22/tests/utils/test_transactional_file.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1194 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/tests/utils/test_yaml.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.746621 sqlmesh-0.5.1.dev22/tests/web/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.5.1.dev22/tests/web/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)    16198 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/tests/web/test_main.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.746870 sqlmesh-0.5.1.dev22/web/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.5.1.dev22/web/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.751168 sqlmesh-0.5.1.dev22/web/client/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1104 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/web/client/.eslintrc.js
--rw-r--r--   0 eakmanrq   (501) staff       (20)       94 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/web/client/.gitignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)      129 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/web/client/.prettierignore
--rw-r--r--   0 eakmanrq   (501) staff       (20)      403 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/web/client/.prettierrc.js
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1076 2023-03-27 22:28:21.000000 sqlmesh-0.5.1.dev22/web/client/index.html
--rw-r--r--   0 eakmanrq   (501) staff       (20)    37689 2023-04-24 17:50:28.000000 sqlmesh-0.5.1.dev22/web/client/openapi.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)      330 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/web/client/orval.config.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)   408504 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/web/client/package-lock.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2389 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/web/client/package.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1642 2023-04-17 00:43:26.000000 sqlmesh-0.5.1.dev22/web/client/playwright.config.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)       82 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/web/client/postcss.config.js
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.611522 sqlmesh-0.5.1.dev22/web/client/public/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.751544 sqlmesh-0.5.1.dev22/web/client/public/favicons/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2473 2023-03-27 01:55:02.000000 sqlmesh-0.5.1.dev22/web/client/public/favicons/favicon.ico
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.752492 sqlmesh-0.5.1.dev22/web/client/src/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.753398 sqlmesh-0.5.1.dev22/web/client/src/api/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1236 2023-04-20 17:40:30.000000 sqlmesh-0.5.1.dev22/web/client/src/api/channels.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5243 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/web/client/src/api/index.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3247 2023-03-22 20:27:52.000000 sqlmesh-0.5.1.dev22/web/client/src/api/instance.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.611739 sqlmesh-0.5.1.dev22/web/client/src/assets/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.611838 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.756754 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Circular STD/
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74500 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74524 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74368 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    73964 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    68940 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    67284 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    74116 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    73916 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.769443 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    55004 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-Black.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    56384 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    57104 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-Bold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    62320 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    56652 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    61688 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    57680 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-Italic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    53148 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-Light.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    57060 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    56836 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-Medium.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    61460 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    52820 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-Roman.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    59176 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    63876 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    60768 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    81732 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    60992 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf
--rwxr-xr-x   0 eakmanrq   (501) staff       (20)    64792 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.772949 sqlmesh-0.5.1.dev22/web/client/src/context/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4126 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/web/client/src/context/context.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5719 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/web/client/src/context/editor.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      923 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/web/client/src/context/fileTree.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1129 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/web/client/src/context/lineage.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2661 2023-04-14 19:58:28.000000 sqlmesh-0.5.1.dev22/web/client/src/context/plan.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1562 2023-03-22 22:04:55.000000 sqlmesh-0.5.1.dev22/web/client/src/context/theme.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.773458 sqlmesh-0.5.1.dev22/web/client/src/hooks/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      308 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/web/client/src/hooks/useActiveFocus.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      817 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/web/client/src/hooks/useLocalStorage.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9363 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/web/client/src/index.css
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.612052 sqlmesh-0.5.1.dev22/web/client/src/library/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.613230 sqlmesh-0.5.1.dev22/web/client/src/library/components/
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.773660 sqlmesh-0.5.1.dev22/web/client/src/library/components/banner/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1705 2023-04-20 17:40:30.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/banner/Banner.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.773919 sqlmesh-0.5.1.dev22/web/client/src/library/components/button/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4517 2023-03-27 01:55:02.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/button/Button.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.774208 sqlmesh-0.5.1.dev22/web/client/src/library/components/button/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3516 2023-03-27 01:55:02.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/button/tests/Button.spec.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.774401 sqlmesh-0.5.1.dev22/web/client/src/library/components/divider/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      856 2023-03-22 22:04:55.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/divider/Divider.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.774635 sqlmesh-0.5.1.dev22/web/client/src/library/components/divider/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      632 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/divider/tests/Divider.spec.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.776658 sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1388 2023-03-27 01:55:02.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/Editor.css
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5397 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/Editor.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8015 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/EditorCode.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2718 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/EditorFooter.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1990 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/EditorIndicator.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9819 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/EditorInspector.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11303 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/EditorPreview.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3527 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/EditorTabs.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.777078 sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/extensions/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5880 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3987 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/extensions/index.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1538 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/help.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.785841 sqlmesh-0.5.1.dev22/web/client/src/library/components/fileTree/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10852 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/fileTree/Directory.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6045 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/fileTree/File.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2997 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/fileTree/FileTree.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)      562 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/fileTree/help.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.786438 sqlmesh-0.5.1.dev22/web/client/src/library/components/graph/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    14478 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/graph/Graph.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6392 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/graph/help.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.787268 sqlmesh-0.5.1.dev22/web/client/src/library/components/ide/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4342 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/ide/ActivePlan.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4870 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/ide/IDE.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    22356 2023-03-27 22:28:21.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/ide/RunPlan.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.788051 sqlmesh-0.5.1.dev22/web/client/src/library/components/input/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2087 2023-03-28 20:12:46.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/input/Input.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)      688 2023-03-22 22:04:55.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/input/InputToggle.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.788349 sqlmesh-0.5.1.dev22/web/client/src/library/components/loading/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      486 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/loading/Loading.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.788904 sqlmesh-0.5.1.dev22/web/client/src/library/components/logo/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2292 2023-03-22 22:04:55.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/logo/Spinner.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4637 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/logo/SqlMesh.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     8042 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/logo/Tobiko.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.789650 sqlmesh-0.5.1.dev22/web/client/src/library/components/modal/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1560 2023-03-22 22:04:55.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/modal/Modal.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1953 2023-03-27 01:55:02.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/modal/ModalConfirmation.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1447 2023-03-27 01:55:02.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/modal/ModalDrawer.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.792525 sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9269 2023-04-20 17:40:30.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/Plan.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     6775 2023-03-27 01:55:02.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/PlanActions.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1312 2023-03-28 20:12:46.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/PlanBackfillDates.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    10448 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/PlanChangePreview.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4920 2023-04-20 17:40:30.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/PlanHeader.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    15855 2023-04-20 17:40:30.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/PlanWizard.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     9926 2023-03-27 22:28:21.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/PlanWizardStepOptions.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)    12528 2023-04-20 17:40:30.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/context.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3444 2023-03-27 01:55:02.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/help.spec.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2155 2023-03-22 20:27:52.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/help.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2599 2023-04-20 17:40:30.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/hooks.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.792692 sqlmesh-0.5.1.dev22/web/client/src/library/components/progress/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      713 2023-03-27 01:55:02.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/progress/Progress.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.792901 sqlmesh-0.5.1.dev22/web/client/src/library/components/report/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1047 2023-04-20 17:40:30.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/report/ReportTestsErrors.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.793715 sqlmesh-0.5.1.dev22/web/client/src/library/components/root/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      526 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/root/Footer.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1921 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/root/Header.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)      247 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/root/Main.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)      443 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/root/Root.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.794042 sqlmesh-0.5.1.dev22/web/client/src/library/components/splitPane/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      788 2023-03-22 22:04:55.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/splitPane/SplitPane.css
--rw-r--r--   0 eakmanrq   (501) staff       (20)      541 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/splitPane/SplitPane.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.794273 sqlmesh-0.5.1.dev22/web/client/src/library/components/tasksOverview/
--rw-r--r--   0 eakmanrq   (501) staff       (20)    11713 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/tasksOverview/TasksOverview.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.794520 sqlmesh-0.5.1.dev22/web/client/src/library/components/toggle/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1453 2023-03-27 01:55:02.000000 sqlmesh-0.5.1.dev22/web/client/src/library/components/toggle/Toggle.tsx
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1197 2023-03-27 01:55:02.000000 sqlmesh-0.5.1.dev22/web/client/src/main.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.796044 sqlmesh-0.5.1.dev22/web/client/src/models/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1647 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/web/client/src/models/artifact.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3472 2023-04-06 22:49:28.000000 sqlmesh-0.5.1.dev22/web/client/src/models/directory.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4190 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/web/client/src/models/environment.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1760 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/web/client/src/models/file.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      173 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/web/client/src/models/index.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      766 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/web/client/src/models/initial.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      200 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/web/client/src/routes.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.796506 sqlmesh-0.5.1.dev22/web/client/src/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)       35 2023-01-20 19:02:18.000000 sqlmesh-0.5.1.dev22/web/client/src/tests/setup.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      541 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/web/client/src/tests/utils.tsx
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.796934 sqlmesh-0.5.1.dev22/web/client/src/types/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      467 2023-03-22 22:04:55.000000 sqlmesh-0.5.1.dev22/web/client/src/types/enum.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)      137 2023-03-22 22:04:55.000000 sqlmesh-0.5.1.dev22/web/client/src/types/index.d.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.797375 sqlmesh-0.5.1.dev22/web/client/src/utils/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4102 2023-03-27 01:55:02.000000 sqlmesh-0.5.1.dev22/web/client/src/utils/index.spec.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5245 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/web/client/src/utils/index.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.797574 sqlmesh-0.5.1.dev22/web/client/src/workers/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      113 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/web/client/src/workers/index.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.798366 sqlmesh-0.5.1.dev22/web/client/src/workers/sqlglot/
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1105 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/web/client/src/workers/sqlglot/sqlglot.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1578 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/web/client/src/workers/sqlglot/worker.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5842 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/web/client/tailwind.config.js
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.798531 sqlmesh-0.5.1.dev22/web/client/tests/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      170 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/web/client/tests/initial.spec.ts
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1141 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/web/client/tsconfig.json
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1297 2023-04-17 00:43:26.000000 sqlmesh-0.5.1.dev22/web/client/vite.config.ts
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.805623 sqlmesh-0.5.1.dev22/web/server/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-20 19:02:18.000000 sqlmesh-0.5.1.dev22/web/server/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.805857 sqlmesh-0.5.1.dev22/web/server/api/
--rw-r--r--   0 eakmanrq   (501) staff       (20)        0 2023-01-17 04:56:29.000000 sqlmesh-0.5.1.dev22/web/server/api/__init__.py
-drwxr-xr-x   0 eakmanrq   (501) staff       (20)        0 2023-04-24 17:52:38.807711 sqlmesh-0.5.1.dev22/web/server/api/endpoints/
--rw-r--r--   0 eakmanrq   (501) staff       (20)      784 2023-04-14 20:24:08.000000 sqlmesh-0.5.1.dev22/web/server/api/endpoints/__init__.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     4564 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/web/server/api/endpoints/commands.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      819 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/web/server/api/endpoints/context.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1858 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/web/server/api/endpoints/directories.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      721 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/web/server/api/endpoints/environments.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      637 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/web/server/api/endpoints/events.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5229 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/web/server/api/endpoints/files.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3283 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/web/server/api/endpoints/lineage.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      962 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/web/server/api/endpoints/models.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3628 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/web/server/api/endpoints/plan.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     3775 2023-04-20 17:40:30.000000 sqlmesh-0.5.1.dev22/web/server/console.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     1374 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/web/server/main.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     5777 2023-04-24 15:25:28.000000 sqlmesh-0.5.1.dev22/web/server/models.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)      260 2023-04-04 21:33:39.000000 sqlmesh-0.5.1.dev22/web/server/openapi.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2421 2023-04-24 17:50:28.000000 sqlmesh-0.5.1.dev22/web/server/settings.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2114 2023-03-17 21:52:31.000000 sqlmesh-0.5.1.dev22/web/server/sse.py
--rw-r--r--   0 eakmanrq   (501) staff       (20)     2461 2023-04-19 01:45:57.000000 sqlmesh-0.5.1.dev22/web/server/utils.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.414861 sqlmesh-0.5.1.dev28/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.270111 sqlmesh-0.5.1.dev28/.circleci/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1872 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev28/.circleci/config.yml
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4414 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev28/.circleci/continue_config.yml
+-rw-r--r--   0 izeigerman   (501) staff       (20)       66 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/.dockerignore
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2152 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev28/.gitignore
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1900 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev28/.pre-commit-config.yaml
+-rw-r--r--   0 izeigerman   (501) staff       (20)      234 2023-04-02 22:26:52.000000 sqlmesh-0.5.1.dev28/.readthedocs.yaml
+-rw-r--r--   0 izeigerman   (501) staff       (20)      135 2023-02-17 22:23:25.000000 sqlmesh-0.5.1.dev28/Dockerfile.api
+-rw-r--r--   0 izeigerman   (501) staff       (20)      383 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/Dockerfile.app
+-rw-r--r--   0 izeigerman   (501) staff       (20)    11346 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/LICENSE
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1855 2023-04-10 17:15:07.000000 sqlmesh-0.5.1.dev28/Makefile
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2037 2023-04-24 23:32:11.415022 sqlmesh-0.5.1.dev28/PKG-INFO
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1250 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev28/README.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1008 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/docker-compose.yml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.272660 sqlmesh-0.5.1.dev28/docs/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.251956 sqlmesh-0.5.1.dev28/docs/_readthedocs/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.272933 sqlmesh-0.5.1.dev28/docs/_readthedocs/html/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-02 22:26:52.000000 sqlmesh-0.5.1.dev28/docs/_readthedocs/html/.keep
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9965 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/docs/comparisons.md
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.274473 sqlmesh-0.5.1.dev28/docs/concepts/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.275122 sqlmesh-0.5.1.dev28/docs/concepts/architecture/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1334 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev28/docs/concepts/architecture/serialization.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1113 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev28/docs/concepts/architecture/snapshots.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6689 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/docs/concepts/audits.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3866 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev28/docs/concepts/environments.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5952 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/docs/concepts/glossary.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)       13 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev28/docs/concepts/hooks.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3027 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev28/docs/concepts/macros.md
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.275909 sqlmesh-0.5.1.dev28/docs/concepts/models/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9934 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/docs/concepts/models/model_kinds.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     7859 2023-04-21 23:38:26.000000 sqlmesh-0.5.1.dev28/docs/concepts/models/overview.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     7171 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev28/docs/concepts/models/python_models.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4938 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev28/docs/concepts/models/seed_models.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5356 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev28/docs/concepts/models/sql_models.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6637 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/docs/concepts/overview.md
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.276064 sqlmesh-0.5.1.dev28/docs/concepts/plans/
+-rw-r--r--   0 izeigerman   (501) staff       (20)    43124 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev28/docs/concepts/plans/model_versioning.png
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8973 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/docs/concepts/plans.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5699 2023-02-27 20:36:43.000000 sqlmesh-0.5.1.dev28/docs/concepts/tests.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)      607 2023-04-09 02:39:18.000000 sqlmesh-0.5.1.dev28/docs/development.md
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.279440 sqlmesh-0.5.1.dev28/docs/guides/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1943 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/docs/guides/connections.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1309 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/docs/guides/migrations.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)    10756 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/docs/guides/models.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6133 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/docs/guides/multi_repo.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2142 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/docs/guides/projects.md
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.281065 sqlmesh-0.5.1.dev28/docs/guides/scheduling/
+-rw-r--r--   0 izeigerman   (501) staff       (20)   740917 2023-02-24 17:54:11.000000 sqlmesh-0.5.1.dev28/docs/guides/scheduling/airflow_successful_plan_apply.png
+-rw-r--r--   0 izeigerman   (501) staff       (20)   379880 2023-02-24 17:54:11.000000 sqlmesh-0.5.1.dev28/docs/guides/scheduling/airflow_successful_setup.png
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5648 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev28/docs/guides/scheduling.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1854 2023-02-27 20:36:43.000000 sqlmesh-0.5.1.dev28/docs/guides/testing.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5517 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/docs/index.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)      297 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/docs/installation.md
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.283810 sqlmesh-0.5.1.dev28/docs/integrations/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2905 2023-04-03 17:47:07.000000 sqlmesh-0.5.1.dev28/docs/integrations/airflow.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     7801 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/docs/integrations/dbt.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)    24125 2023-04-24 17:39:27.000000 sqlmesh-0.5.1.dev28/docs/integrations/engines.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)      925 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/docs/integrations/github.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)      217 2023-03-25 06:07:32.000000 sqlmesh-0.5.1.dev28/docs/integrations/overview.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)      665 2023-03-29 18:25:45.000000 sqlmesh-0.5.1.dev28/docs/prerequisites.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)    10781 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/docs/quick_start.md
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.285078 sqlmesh-0.5.1.dev28/docs/reference/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6093 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev28/docs/reference/cli.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)    13607 2023-04-24 17:39:27.000000 sqlmesh-0.5.1.dev28/docs/reference/configuration.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4579 2023-04-20 18:21:56.000000 sqlmesh-0.5.1.dev28/docs/reference/notebook.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1127 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev28/docs/reference/overview.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)       14 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev28/docs/reference/python.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)       16 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev28/docs/release_notes.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)      122 2023-04-02 22:26:52.000000 sqlmesh-0.5.1.dev28/docs/requirements.txt
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3249 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/docs/sqlmesh.png
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.286658 sqlmesh-0.5.1.dev28/examples/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.5.1.dev28/examples/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.288519 sqlmesh-0.5.1.dev28/examples/airflow/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1713 2023-04-09 02:39:12.000000 sqlmesh-0.5.1.dev28/examples/airflow/Dockerfile.template
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2164 2023-04-09 02:39:18.000000 sqlmesh-0.5.1.dev28/examples/airflow/Makefile
+-rw-r--r--   0 izeigerman   (501) staff       (20)      942 2023-01-20 00:11:34.000000 sqlmesh-0.5.1.dev28/examples/airflow/README.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-27 21:18:46.000000 sqlmesh-0.5.1.dev28/examples/airflow/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.288781 sqlmesh-0.5.1.dev28/examples/airflow/dags/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      263 2023-03-09 17:15:39.000000 sqlmesh-0.5.1.dev28/examples/airflow/dags/sqlmesh_integration.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3515 2023-04-09 02:39:12.000000 sqlmesh-0.5.1.dev28/examples/airflow/docker_compose_decorator.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)       12 2023-01-20 00:11:34.000000 sqlmesh-0.5.1.dev28/examples/airflow/requirements.txt
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.289150 sqlmesh-0.5.1.dev28/examples/airflow/spark_conf/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      872 2023-01-20 00:11:34.000000 sqlmesh-0.5.1.dev28/examples/airflow/spark_conf/hive-site.xml
+-rw-r--r--   0 izeigerman   (501) staff       (20)      151 2023-01-20 00:11:34.000000 sqlmesh-0.5.1.dev28/examples/airflow/spark_conf/spark-defaults.conf
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.253408 sqlmesh-0.5.1.dev28/examples/multi/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.289488 sqlmesh-0.5.1.dev28/examples/multi/repo_1/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.289810 sqlmesh-0.5.1.dev28/examples/multi/repo_1/audits/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/examples/multi/repo_1/audits/.gitkeep
+-rw-r--r--   0 izeigerman   (501) staff       (20)      108 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/examples/multi/repo_1/config.yaml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.290117 sqlmesh-0.5.1.dev28/examples/multi/repo_1/macros/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/examples/multi/repo_1/macros/.gitkeep
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/examples/multi/repo_1/macros/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.290708 sqlmesh-0.5.1.dev28/examples/multi/repo_1/models/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/examples/multi/repo_1/models/.gitkeep
+-rw-r--r--   0 izeigerman   (501) staff       (20)       63 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/examples/multi/repo_1/models/a.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)       53 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/examples/multi/repo_1/models/b.sql
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.290996 sqlmesh-0.5.1.dev28/examples/multi/repo_1/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/examples/multi/repo_1/tests/.gitkeep
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.291163 sqlmesh-0.5.1.dev28/examples/multi/repo_2/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.291412 sqlmesh-0.5.1.dev28/examples/multi/repo_2/audits/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/examples/multi/repo_2/audits/.gitkeep
+-rw-r--r--   0 izeigerman   (501) staff       (20)      113 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/examples/multi/repo_2/config.yaml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.291734 sqlmesh-0.5.1.dev28/examples/multi/repo_2/macros/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/examples/multi/repo_2/macros/.gitkeep
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/examples/multi/repo_2/macros/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.292212 sqlmesh-0.5.1.dev28/examples/multi/repo_2/models/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/examples/multi/repo_2/models/.gitkeep
+-rw-r--r--   0 izeigerman   (501) staff       (20)       64 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/examples/multi/repo_2/models/c.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)       53 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/examples/multi/repo_2/models/d.sql
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.292413 sqlmesh-0.5.1.dev28/examples/multi/repo_2/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/examples/multi/repo_2/tests/.gitkeep
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.292860 sqlmesh-0.5.1.dev28/examples/sushi/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev28/examples/sushi/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.293493 sqlmesh-0.5.1.dev28/examples/sushi/audits/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      105 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev28/examples/sushi/audits/items.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      119 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev28/examples/sushi/audits/order_items.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      829 2023-04-21 21:07:50.000000 sqlmesh-0.5.1.dev28/examples/sushi/config.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.293707 sqlmesh-0.5.1.dev28/examples/sushi/data/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-24 21:30:36.000000 sqlmesh-0.5.1.dev28/examples/sushi/data/.keep
+-rw-r--r--   0 izeigerman   (501) staff       (20)      551 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev28/examples/sushi/helper.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.293988 sqlmesh-0.5.1.dev28/examples/sushi/hooks/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev28/examples/sushi/hooks/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      247 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev28/examples/sushi/hooks/hooks.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.294297 sqlmesh-0.5.1.dev28/examples/sushi/macros/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev28/examples/sushi/macros/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      702 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev28/examples/sushi/macros/macros.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.296397 sqlmesh-0.5.1.dev28/examples/sushi/models/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      916 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev28/examples/sushi/models/customer_revenue_by_day.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      204 2023-03-03 17:17:44.000000 sqlmesh-0.5.1.dev28/examples/sushi/models/customers.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1910 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev28/examples/sushi/models/items.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1911 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev28/examples/sushi/models/order_items.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1642 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev28/examples/sushi/models/orders.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      346 2023-03-25 04:59:10.000000 sqlmesh-0.5.1.dev28/examples/sushi/models/top_waiters.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      465 2023-04-24 18:34:50.000000 sqlmesh-0.5.1.dev28/examples/sushi/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      123 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev28/examples/sushi/models/waiter_names.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      691 2023-04-24 21:41:10.000000 sqlmesh-0.5.1.dev28/examples/sushi/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      197 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev28/examples/sushi/models/waiters.sql
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.296633 sqlmesh-0.5.1.dev28/examples/sushi/seeds/
+-rw-r--r--   0 izeigerman   (501) staff       (20)       88 2023-03-24 20:49:46.000000 sqlmesh-0.5.1.dev28/examples/sushi/seeds/waiter_names.csv
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.297067 sqlmesh-0.5.1.dev28/examples/sushi/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1459 2023-02-27 20:51:17.000000 sqlmesh-0.5.1.dev28/examples/sushi/tests/test_customer_revenue_by_day.yaml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.298996 sqlmesh-0.5.1.dev28/examples/sushi_dbt/
+-rw-r--r--   0 izeigerman   (501) staff       (20)       15 2023-02-17 22:23:25.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/.gitignore
+-rw-r--r--   0 izeigerman   (501) staff       (20)       41 2023-02-17 22:23:25.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/.user.yml
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-27 21:18:46.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.299339 sqlmesh-0.5.1.dev28/examples/sushi_dbt/analyses/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-20 00:11:34.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/analyses/.gitkeep
+-rw-r--r--   0 izeigerman   (501) staff       (20)      291 2023-03-14 18:30:53.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/config.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      507 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/dbt_project.yml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.299912 sqlmesh-0.5.1.dev28/examples/sushi_dbt/macros/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      941 2023-03-03 23:53:25.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/macros/incremental.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)       80 2023-02-28 16:05:24.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/macros/log_value.sql
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.301494 sqlmesh-0.5.1.dev28/examples/sushi_dbt/models/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1125 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/models/customer_revenue_by_day.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)       80 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/models/customers.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      182 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/models/schema.yml
+-rw-r--r--   0 izeigerman   (501) staff       (20)      309 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/models/top_waiters.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      389 2023-01-31 01:13:15.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      752 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      186 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/models/waiters.sql
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.255262 sqlmesh-0.5.1.dev28/examples/sushi_dbt/packages/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.301711 sqlmesh-0.5.1.dev28/examples/sushi_dbt/packages/customers/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.301964 sqlmesh-0.5.1.dev28/examples/sushi_dbt/packages/customers/analyses/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-03-09 19:19:03.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/packages/customers/analyses/.gitkeep
+-rw-r--r--   0 izeigerman   (501) staff       (20)      663 2023-03-09 19:19:03.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/packages/customers/dbt_project.yml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.302380 sqlmesh-0.5.1.dev28/examples/sushi_dbt/packages/customers/macros/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      117 2023-03-09 19:19:03.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/packages/customers/macros/current_engine.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)       65 2023-03-09 19:19:03.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/packages/customers/macros/distinct.sql
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.302570 sqlmesh-0.5.1.dev28/examples/sushi_dbt/packages/customers/models/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/packages/customers/models/schema.yml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.302722 sqlmesh-0.5.1.dev28/examples/sushi_dbt/packages/customers/seeds/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-03-09 19:19:03.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/packages/customers/seeds/.gitkeep
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.302869 sqlmesh-0.5.1.dev28/examples/sushi_dbt/packages/customers/snapshots/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-03-09 19:19:03.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/packages/customers/snapshots/.gitkeep
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.303001 sqlmesh-0.5.1.dev28/examples/sushi_dbt/packages/customers/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-03-09 19:19:03.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/packages/customers/tests/.gitkeep
+-rw-r--r--   0 izeigerman   (501) staff       (20)      783 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/profiles.yml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.303815 sqlmesh-0.5.1.dev28/examples/sushi_dbt/seeds/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2327 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/seeds/items.csv
+-rw-r--r--   0 izeigerman   (501) staff       (20)    10472 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/seeds/order_items.csv
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9746 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/seeds/orders.csv
+-rw-r--r--   0 izeigerman   (501) staff       (20)       97 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/seeds/properties.yml
+-rw-r--r--   0 izeigerman   (501) staff       (20)       88 2023-01-31 01:13:15.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/seeds/waiter_names.csv
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.304056 sqlmesh-0.5.1.dev28/examples/sushi_dbt/snapshots/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-20 00:11:34.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/snapshots/.gitkeep
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.304193 sqlmesh-0.5.1.dev28/examples/sushi_dbt/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-20 00:11:34.000000 sqlmesh-0.5.1.dev28/examples/sushi_dbt/tests/.gitkeep
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.304442 sqlmesh-0.5.1.dev28/examples/wursthall/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.5.1.dev28/examples/wursthall/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.256363 sqlmesh-0.5.1.dev28/examples/wursthall/audits/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.304731 sqlmesh-0.5.1.dev28/examples/wursthall/audits/db/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      141 2023-01-31 01:13:15.000000 sqlmesh-0.5.1.dev28/examples/wursthall/audits/db/order_f.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)       66 2023-01-25 18:34:48.000000 sqlmesh-0.5.1.dev28/examples/wursthall/config.yaml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.305075 sqlmesh-0.5.1.dev28/examples/wursthall/macros/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.5.1.dev28/examples/wursthall/macros/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      618 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/examples/wursthall/macros/macros.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.305224 sqlmesh-0.5.1.dev28/examples/wursthall/models/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.5.1.dev28/examples/wursthall/models/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.305919 sqlmesh-0.5.1.dev28/examples/wursthall/models/db/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      433 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev28/examples/wursthall/models/db/customer_d.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      256 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/examples/wursthall/models/db/item_d.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3161 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev28/examples/wursthall/models/db/order_f.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      542 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev28/examples/wursthall/models/db/order_item_f.sql
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.306992 sqlmesh-0.5.1.dev28/examples/wursthall/models/src/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-25 18:34:48.000000 sqlmesh-0.5.1.dev28/examples/wursthall/models/src/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1672 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev28/examples/wursthall/models/src/customer_details.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      120 2023-01-25 18:34:48.000000 sqlmesh-0.5.1.dev28/examples/wursthall/models/src/menu_item_details.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3434 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev28/examples/wursthall/models/src/order_item_details.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      892 2023-01-25 18:34:48.000000 sqlmesh-0.5.1.dev28/examples/wursthall/models/src/shared.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.256757 sqlmesh-0.5.1.dev28/examples/wursthall/seeds/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.307222 sqlmesh-0.5.1.dev28/examples/wursthall/seeds/src/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     7416 2023-01-25 18:34:48.000000 sqlmesh-0.5.1.dev28/examples/wursthall/seeds/src/menu_item_details.csv
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.307886 sqlmesh-0.5.1.dev28/examples/wursthall/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      888 2023-02-20 22:54:27.000000 sqlmesh-0.5.1.dev28/examples/wursthall/tests/test_customer_d.yaml
+-rw-r--r--   0 izeigerman   (501) staff       (20)      955 2023-02-20 22:54:27.000000 sqlmesh-0.5.1.dev28/examples/wursthall/tests/test_order_item_f.yaml
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2113 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/mkdocs.yml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.308083 sqlmesh-0.5.1.dev28/pdoc/
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)     1153 2023-03-29 18:25:45.000000 sqlmesh-0.5.1.dev28/pdoc/cli.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.308331 sqlmesh-0.5.1.dev28/pdoc/templates/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      131 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/pdoc/templates/module.html.jinja2
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.308621 sqlmesh-0.5.1.dev28/posts/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.312722 sqlmesh-0.5.1.dev28/posts/virtual_data_environments/
+-rw-r--r--   0 izeigerman   (501) staff       (20)   318753 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/posts/virtual_data_environments/change_categorization.png
+-rw-r--r--   0 izeigerman   (501) staff       (20)   274526 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/posts/virtual_data_environments/isolated_rigid_envs.png
+-rw-r--r--   0 izeigerman   (501) staff       (20)   163619 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/posts/virtual_data_environments/partial_breaking.png
+-rw-r--r--   0 izeigerman   (501) staff       (20)   298971 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/posts/virtual_data_environments/stateful_envs.png
+-rw-r--r--   0 izeigerman   (501) staff       (20)   366545 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/posts/virtual_data_environments/virtual_envs.png
+-rw-r--r--   0 izeigerman   (501) staff       (20)  1344487 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/posts/virtual_data_environments/virtual_envs_end_to_end.png
+-rw-r--r--   0 izeigerman   (501) staff       (20)    18696 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/posts/virtual_data_environments.md
+-rw-r--r--   0 izeigerman   (501) staff       (20)      734 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/pytest.ini
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1393 2023-04-24 23:32:11.415716 sqlmesh-0.5.1.dev28/setup.cfg
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3158 2023-04-24 23:28:42.000000 sqlmesh-0.5.1.dev28/setup.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.315621 sqlmesh-0.5.1.dev28/sqlmesh/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        3 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/sqlmesh/.airflowignore
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3950 2023-04-21 23:38:26.000000 sqlmesh-0.5.1.dev28/sqlmesh/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      175 2023-04-24 23:32:10.000000 sqlmesh-0.5.1.dev28/sqlmesh/_version.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.317603 sqlmesh-0.5.1.dev28/sqlmesh/cli/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      898 2023-04-21 23:38:26.000000 sqlmesh-0.5.1.dev28/sqlmesh/cli/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4314 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/sqlmesh/cli/example_project.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9641 2023-04-23 13:55:51.000000 sqlmesh-0.5.1.dev28/sqlmesh/cli/main.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1433 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/sqlmesh/cli/options.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.320255 sqlmesh-0.5.1.dev28/sqlmesh/core/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      586 2023-01-20 19:19:17.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/_typing.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.320889 sqlmesh-0.5.1.dev28/sqlmesh/core/audit/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      449 2023-01-27 03:51:22.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/audit/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1071 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/audit/builtin.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8136 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/audit/definition.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.322818 sqlmesh-0.5.1.dev28/sqlmesh/core/config/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      668 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/config/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4412 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/config/base.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1001 2023-02-22 17:05:23.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/config/categorizer.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      940 2023-02-08 20:28:46.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/config/common.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    21184 2023-04-24 17:39:27.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/config/connection.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3351 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/config/loader.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1655 2023-02-08 20:28:46.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/config/model.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5611 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/config/root.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8421 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/config/scheduler.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    29242 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/console.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      735 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/constants.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    36030 2023-04-24 23:28:13.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/context.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8612 2023-04-24 23:28:13.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/context_diff.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    17626 2023-03-24 20:30:06.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/dialect.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.326228 sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2626 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      762 2023-01-18 00:01:51.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/_typing.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    29021 2023-04-22 00:09:12.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/base.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4191 2023-04-22 00:43:39.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/base_postgres.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4238 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/base_spark.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    15694 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/bigquery.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      402 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/databricks.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1939 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/databricks_api.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1971 2023-03-01 20:53:43.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/duckdb.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2149 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/postgres.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6650 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/redshift.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1181 2023-03-01 20:53:43.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/shared.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2658 2023-03-01 00:12:50.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/snowflake.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4131 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/spark.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1815 2023-04-24 23:28:13.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/environment.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      742 2023-02-09 01:00:20.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/hooks.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    12521 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/loader.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    18920 2023-03-24 20:30:06.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/macros.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.329520 sqlmesh-0.5.1.dev28/sqlmesh/core/model/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      594 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/model/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1746 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/model/cache.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1300 2023-04-18 21:05:17.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/model/common.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2417 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/model/decorator.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    47685 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/model/definition.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8168 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/model/kind.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    13034 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/model/meta.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2017 2023-03-15 19:25:00.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/model/seed.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2314 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/notification_target.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.331166 sqlmesh-0.5.1.dev28/sqlmesh/core/plan/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      191 2022-12-27 15:59:10.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/plan/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    24916 2023-04-21 23:38:26.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/plan/definition.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8075 2023-04-24 23:28:13.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/plan/evaluator.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    12623 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/renderer.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    15386 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/scheduler.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    20418 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/schema_diff.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.332097 sqlmesh-0.5.1.dev28/sqlmesh/core/snapshot/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      527 2023-02-13 20:33:07.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/snapshot/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1990 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/snapshot/categorizer.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    32727 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/snapshot/definition.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    19214 2023-04-24 23:28:13.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/snapshot/evaluator.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.333042 sqlmesh-0.5.1.dev28/sqlmesh/core/state_sync/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      692 2023-04-10 17:15:07.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/state_sync/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    13080 2023-04-24 23:28:13.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/state_sync/base.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    12222 2023-04-24 23:28:13.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/state_sync/common.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    20048 2023-04-24 23:28:13.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/state_sync/engine_adapter.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    10834 2023-04-19 16:43:48.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/test.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1412 2022-12-24 00:00:07.000000 sqlmesh-0.5.1.dev28/sqlmesh/core/user.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.336695 sqlmesh-0.5.1.dev28/sqlmesh/dbt/
+-rw-r--r--   0 izeigerman   (501) staff       (20)       79 2023-03-13 19:40:14.000000 sqlmesh-0.5.1.dev28/sqlmesh/dbt/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9390 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev28/sqlmesh/dbt/adapter.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    16407 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev28/sqlmesh/dbt/basemodel.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    11231 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/sqlmesh/dbt/builtin.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1762 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev28/sqlmesh/dbt/column.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4771 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev28/sqlmesh/dbt/common.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5087 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev28/sqlmesh/dbt/context.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8044 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev28/sqlmesh/dbt/loader.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9807 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev28/sqlmesh/dbt/model.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    13257 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev28/sqlmesh/dbt/package.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3701 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev28/sqlmesh/dbt/profile.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4772 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/sqlmesh/dbt/project.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      928 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev28/sqlmesh/dbt/seed.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3137 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/sqlmesh/dbt/source.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    13503 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev28/sqlmesh/dbt/target.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      291 2023-03-02 18:36:40.000000 sqlmesh-0.5.1.dev28/sqlmesh/dbt/util.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.337086 sqlmesh-0.5.1.dev28/sqlmesh/engines/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/sqlmesh/engines/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4437 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/sqlmesh/engines/commands.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.337355 sqlmesh-0.5.1.dev28/sqlmesh/engines/spark/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/sqlmesh/engines/spark/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3414 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/sqlmesh/engines/spark/app.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.338171 sqlmesh-0.5.1.dev28/sqlmesh/engines/spark/db_api/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/sqlmesh/engines/spark/db_api/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      148 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/sqlmesh/engines/spark/db_api/errors.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2571 2023-02-14 21:38:26.000000 sqlmesh-0.5.1.dev28/sqlmesh/engines/spark/db_api/spark_session.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.338530 sqlmesh-0.5.1.dev28/sqlmesh/integrations/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/sqlmesh/integrations/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.339416 sqlmesh-0.5.1.dev28/sqlmesh/integrations/github/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/sqlmesh/integrations/github/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2210 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev28/sqlmesh/integrations/github/notification_operator_provider.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1726 2023-01-19 13:52:03.000000 sqlmesh-0.5.1.dev28/sqlmesh/integrations/github/notification_target.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1829 2023-01-18 20:54:37.000000 sqlmesh-0.5.1.dev28/sqlmesh/integrations/github/shared.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    13754 2023-04-21 23:38:26.000000 sqlmesh-0.5.1.dev28/sqlmesh/magics.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.340368 sqlmesh-0.5.1.dev28/sqlmesh/migrations/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-10 17:15:07.000000 sqlmesh-0.5.1.dev28/sqlmesh/migrations/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1749 2023-04-10 17:15:07.000000 sqlmesh-0.5.1.dev28/sqlmesh/migrations/v0001_init.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      103 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/sqlmesh/migrations/v0002_remove_identify.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1183 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev28/sqlmesh/migrations/v0003_move_batch_size.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      530 2023-04-24 22:14:08.000000 sqlmesh-0.5.1.dev28/sqlmesh/migrations/v0004_environmnent_add_finalized_at.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/sqlmesh/py.typed
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.340764 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.343028 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-04 00:12:26.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4020 2023-04-10 17:15:07.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/api.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8053 2023-04-10 17:15:07.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/client.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3830 2023-03-09 17:15:48.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/common.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    18799 2023-04-24 23:28:13.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/dag_generator.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.343618 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/hooks/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-16 21:08:59.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/hooks/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2132 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/hooks/bigquery.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      868 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/hooks/redshift.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8508 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/integration.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.346110 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/operators/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/operators/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1444 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/operators/bigquery.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6307 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/operators/databricks.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2549 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/operators/hwm_sensor.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      877 2023-01-31 17:31:24.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/operators/notification.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1322 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/operators/postgres.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1211 2023-01-20 19:19:17.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/operators/redshift.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1340 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/operators/snowflake.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5222 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/operators/spark_submit.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    11104 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/operators/targets.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4400 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/plan.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1292 2023-04-10 17:15:07.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/plugin.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4139 2023-04-10 17:15:07.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/state_sync.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5213 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/util.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.349603 sqlmesh-0.5.1.dev28/sqlmesh/utils/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4378 2023-04-21 19:57:49.000000 sqlmesh-0.5.1.dev28/sqlmesh/utils/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3593 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/sqlmesh/utils/cache.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8053 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev28/sqlmesh/utils/concurrency.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     7530 2023-02-14 22:10:01.000000 sqlmesh-0.5.1.dev28/sqlmesh/utils/connection_pool.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      410 2022-12-30 16:25:50.000000 sqlmesh-0.5.1.dev28/sqlmesh/utils/conversions.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4329 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev28/sqlmesh/utils/dag.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     7549 2023-04-18 02:34:51.000000 sqlmesh-0.5.1.dev28/sqlmesh/utils/date.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1244 2023-02-04 22:32:08.000000 sqlmesh-0.5.1.dev28/sqlmesh/utils/errors.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    16084 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/sqlmesh/utils/jinja.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    15093 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/sqlmesh/utils/metaprogramming.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      888 2023-03-07 23:18:33.000000 sqlmesh-0.5.1.dev28/sqlmesh/utils/pandas.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1609 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev28/sqlmesh/utils/pydantic.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1534 2023-01-25 18:09:57.000000 sqlmesh-0.5.1.dev28/sqlmesh/utils/rich.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6487 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/sqlmesh/utils/transactional_file.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1419 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev28/sqlmesh/utils/yaml.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.316754 sqlmesh-0.5.1.dev28/sqlmesh.egg-info/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2037 2023-04-24 23:32:10.000000 sqlmesh-0.5.1.dev28/sqlmesh.egg-info/PKG-INFO
+-rw-r--r--   0 izeigerman   (501) staff       (20)    21373 2023-04-24 23:32:11.000000 sqlmesh-0.5.1.dev28/sqlmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 izeigerman   (501) staff       (20)        1 2023-04-24 23:32:10.000000 sqlmesh-0.5.1.dev28/sqlmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 izeigerman   (501) staff       (20)      142 2023-04-24 23:32:10.000000 sqlmesh-0.5.1.dev28/sqlmesh.egg-info/entry_points.txt
+-rw-r--r--   0 izeigerman   (501) staff       (20)      838 2023-04-24 23:32:10.000000 sqlmesh-0.5.1.dev28/sqlmesh.egg-info/requires.txt
+-rw-r--r--   0 izeigerman   (501) staff       (20)       12 2023-04-24 23:32:10.000000 sqlmesh-0.5.1.dev28/sqlmesh.egg-info/top_level.txt
+-rw-r--r--   0 izeigerman   (501) staff       (20)    21020 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev28/sqlmesh.svg
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.350303 sqlmesh-0.5.1.dev28/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/tests/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      285 2023-02-07 17:58:48.000000 sqlmesh-0.5.1.dev28/tests/common_fixtures.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3741 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/tests/conftest.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.354725 sqlmesh-0.5.1.dev28/tests/core/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/tests/core/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.356821 sqlmesh-0.5.1.dev28/tests/core/engine_adapter/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/tests/core/engine_adapter/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    27881 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/tests/core/engine_adapter/test_base.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2114 2023-04-22 00:43:39.000000 sqlmesh-0.5.1.dev28/tests/core/engine_adapter/test_base_postgres.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1270 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/tests/core/engine_adapter/test_base_spark.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     7171 2023-03-07 23:18:33.000000 sqlmesh-0.5.1.dev28/tests/core/engine_adapter/test_bigquery.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1253 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/tests/core/engine_adapter/test_databricks.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2613 2023-02-14 20:17:36.000000 sqlmesh-0.5.1.dev28/tests/core/engine_adapter/test_duckdb.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1569 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/tests/core/engine_adapter/test_postgres.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8036 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/tests/core/engine_adapter/test_redshift.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3191 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/tests/core/engine_adapter/test_spark.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     7073 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev28/tests/core/test_audit.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6611 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev28/tests/core/test_config.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      850 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/core/test_connection_config.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    10197 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/tests/core/test_context.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2749 2023-02-17 22:23:25.000000 sqlmesh-0.5.1.dev28/tests/core/test_dialect.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      464 2022-12-28 17:42:44.000000 sqlmesh-0.5.1.dev28/tests/core/test_environment.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    26764 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev28/tests/core/test_integration.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5880 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/tests/core/test_macros.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    25301 2023-04-24 17:39:27.000000 sqlmesh-0.5.1.dev28/tests/core/test_model.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    15280 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/tests/core/test_plan.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3824 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/tests/core/test_plan_evaluator.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4557 2023-04-10 17:15:07.000000 sqlmesh-0.5.1.dev28/tests/core/test_scheduler.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    32235 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/tests/core/test_schema_diff.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      857 2023-01-06 17:16:27.000000 sqlmesh-0.5.1.dev28/tests/core/test_seed.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    28291 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev28/tests/core/test_snapshot.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9965 2023-04-24 23:28:13.000000 sqlmesh-0.5.1.dev28/tests/core/test_snapshot_evaluator.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    21868 2023-04-24 23:28:13.000000 sqlmesh-0.5.1.dev28/tests/core/test_state_sync.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.357816 sqlmesh-0.5.1.dev28/tests/dbt/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-16 16:43:18.000000 sqlmesh-0.5.1.dev28/tests/dbt/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      636 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/tests/dbt/conftest.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2537 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/tests/dbt/test_adapter.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    13195 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev28/tests/dbt/test_config.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    17098 2023-04-24 20:07:04.000000 sqlmesh-0.5.1.dev28/tests/dbt/test_transformation.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.358014 sqlmesh-0.5.1.dev28/tests/engines/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/tests/engines/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.358584 sqlmesh-0.5.1.dev28/tests/engines/spark/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/tests/engines/spark/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      357 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/tests/engines/spark/conftest.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1503 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/tests/engines/spark/test_db_api.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.261100 sqlmesh-0.5.1.dev28/tests/fixtures/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.259822 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.359841 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.360100 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/analyses/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/analyses/.gitkeep
+-rw-r--r--   0 izeigerman   (501) staff       (20)      291 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/config.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.259961 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/dbt_packages/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1055 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/dbt_project.yml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.360240 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/logs/
+-rw-r--r--   0 izeigerman   (501) staff       (20)    10264 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.360674 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/macros/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      941 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/macros/incremental.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)       80 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/macros/log_value.sql
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.361651 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/models/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      247 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/models/schema.yml
+-rw-r--r--   0 izeigerman   (501) staff       (20)      334 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/models/top_waiters.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      389 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/models/waiter_as_customer_by_day.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      863 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      196 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/models/waiters.sql
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.260296 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.361843 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages/customers/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.362095 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages/customers/analyses/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages/customers/analyses/.gitkeep
+-rw-r--r--   0 izeigerman   (501) staff       (20)      663 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.362582 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages/customers/macros/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      117 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages/customers/macros/current_engine.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)       65 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages/customers/macros/distinct.sql
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.363198 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages/customers/models/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1155 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      108 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages/customers/models/customers.sql
+-rw-r--r--   0 izeigerman   (501) staff       (20)      193 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages/customers/models/schema.yml
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.363395 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages/customers/seeds/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages/customers/seeds/.gitkeep
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.363547 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages/customers/snapshots/.gitkeep
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.363654 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages/customers/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages/customers/tests/.gitkeep
+-rw-r--r--   0 izeigerman   (501) staff       (20)       41 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages.yml
+-rw-r--r--   0 izeigerman   (501) staff       (20)      540 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/profiles.yml
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1250 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/seed_sources.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.363934 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/seeds/
+-rw-r--r--   0 izeigerman   (501) staff       (20)       42 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/seeds/properties.yml
+-rw-r--r--   0 izeigerman   (501) staff       (20)       88 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/seeds/waiter_names.csv
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.364103 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/snapshots/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/snapshots/.gitkeep
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.364527 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/source_data/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2327 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/source_data/items.csv
+-rw-r--r--   0 izeigerman   (501) staff       (20)    10472 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/source_data/order_items.csv
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9746 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/source_data/orders.csv
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.364698 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/tests/.gitkeep
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.364964 sqlmesh-0.5.1.dev28/tests/fixtures/migrations/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9823 2023-04-24 22:27:34.000000 sqlmesh-0.5.1.dev28/tests/fixtures/migrations/environments.json
+-rw-r--r--   0 izeigerman   (501) staff       (20)    25229 2023-04-10 17:15:07.000000 sqlmesh-0.5.1.dev28/tests/fixtures/migrations/snapshots.json
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.365341 sqlmesh-0.5.1.dev28/tests/integrations/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/tests/integrations/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.365827 sqlmesh-0.5.1.dev28/tests/integrations/github/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/tests/integrations/github/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.366204 sqlmesh-0.5.1.dev28/tests/integrations/github/fixtures/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      816 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/tests/integrations/github/fixtures/pull_request_review.json
+-rw-r--r--   0 izeigerman   (501) staff       (20)      477 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev28/tests/integrations/github/test_notification_target.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.366450 sqlmesh-0.5.1.dev28/tests/schedulers/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/tests/schedulers/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.367760 sqlmesh-0.5.1.dev28/tests/schedulers/airflow/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/tests/schedulers/airflow/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1414 2023-01-19 13:52:03.000000 sqlmesh-0.5.1.dev28/tests/schedulers/airflow/conftest.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.368304 sqlmesh-0.5.1.dev28/tests/schedulers/airflow/operators/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/tests/schedulers/airflow/operators/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3866 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev28/tests/schedulers/airflow/operators/test_hwm_sensor.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4280 2023-03-09 17:15:48.000000 sqlmesh-0.5.1.dev28/tests/schedulers/airflow/operators/test_targets.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9704 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/tests/schedulers/airflow/test_client.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1345 2023-04-21 23:58:46.000000 sqlmesh-0.5.1.dev28/tests/schedulers/airflow/test_end_to_end.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6035 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev28/tests/schedulers/airflow/test_integration.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5785 2023-03-02 21:54:32.000000 sqlmesh-0.5.1.dev28/tests/schedulers/airflow/test_plan.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.370772 sqlmesh-0.5.1.dev28/tests/utils/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/tests/utils/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1118 2023-04-24 13:57:39.000000 sqlmesh-0.5.1.dev28/tests/utils/test_cache.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3580 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev28/tests/utils/test_concurrency.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6430 2023-02-14 21:38:26.000000 sqlmesh-0.5.1.dev28/tests/utils/test_connection_pool.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1381 2023-02-14 17:01:23.000000 sqlmesh-0.5.1.dev28/tests/utils/test_dag.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1818 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/tests/utils/test_date.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      551 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/tests/utils/test_filesystem.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5516 2023-03-07 20:10:54.000000 sqlmesh-0.5.1.dev28/tests/utils/test_jinja.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5790 2023-03-03 23:53:25.000000 sqlmesh-0.5.1.dev28/tests/utils/test_metaprogramming.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2501 2023-03-07 23:18:33.000000 sqlmesh-0.5.1.dev28/tests/utils/test_pandas.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      518 2022-12-13 22:24:29.000000 sqlmesh-0.5.1.dev28/tests/utils/test_pydantic.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2911 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev28/tests/utils/test_transactional_file.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1194 2023-03-13 19:40:14.000000 sqlmesh-0.5.1.dev28/tests/utils/test_yaml.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.371114 sqlmesh-0.5.1.dev28/tests/web/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-19 13:52:03.000000 sqlmesh-0.5.1.dev28/tests/web/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)    16198 2023-04-24 23:28:13.000000 sqlmesh-0.5.1.dev28/tests/web/test_main.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.371235 sqlmesh-0.5.1.dev28/web/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-19 13:52:03.000000 sqlmesh-0.5.1.dev28/web/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.375503 sqlmesh-0.5.1.dev28/web/client/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1104 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/web/client/.eslintrc.js
+-rw-r--r--   0 izeigerman   (501) staff       (20)       94 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/web/client/.gitignore
+-rw-r--r--   0 izeigerman   (501) staff       (20)      129 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/web/client/.prettierignore
+-rw-r--r--   0 izeigerman   (501) staff       (20)      403 2023-02-14 21:38:26.000000 sqlmesh-0.5.1.dev28/web/client/.prettierrc.js
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1076 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev28/web/client/index.html
+-rw-r--r--   0 izeigerman   (501) staff       (20)    37689 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/web/client/openapi.json
+-rw-r--r--   0 izeigerman   (501) staff       (20)      330 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/web/client/orval.config.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)   408504 2023-04-22 00:03:34.000000 sqlmesh-0.5.1.dev28/web/client/package-lock.json
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2389 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/web/client/package.json
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1642 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev28/web/client/playwright.config.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)       82 2023-02-14 21:38:27.000000 sqlmesh-0.5.1.dev28/web/client/postcss.config.js
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.261911 sqlmesh-0.5.1.dev28/web/client/public/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.375721 sqlmesh-0.5.1.dev28/web/client/public/favicons/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2473 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/public/favicons/favicon.ico
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.376430 sqlmesh-0.5.1.dev28/web/client/src/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.377317 sqlmesh-0.5.1.dev28/web/client/src/api/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1236 2023-04-20 18:21:56.000000 sqlmesh-0.5.1.dev28/web/client/src/api/channels.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5243 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/web/client/src/api/index.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3247 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/src/api/instance.ts
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.262170 sqlmesh-0.5.1.dev28/web/client/src/assets/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.262282 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.380177 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Circular STD/
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    74500 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    74524 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    74368 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    73964 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    68940 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    67284 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    74116 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    73916 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.387330 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    55004 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-Black.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    56384 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    57104 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-Bold.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    62320 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    56652 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    61688 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    57680 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-Italic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    53148 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-Light.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    57060 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    56836 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-Medium.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    61460 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    52820 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-Roman.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    59176 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    63876 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    60768 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    81732 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    60992 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf
+-rwxr-xr-x   0 izeigerman   (501) staff       (20)    64792 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.389007 sqlmesh-0.5.1.dev28/web/client/src/context/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4126 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/web/client/src/context/context.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5719 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/web/client/src/context/editor.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)      923 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev28/web/client/src/context/fileTree.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1129 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/web/client/src/context/lineage.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2661 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/web/client/src/context/plan.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1562 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/src/context/theme.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.389691 sqlmesh-0.5.1.dev28/web/client/src/hooks/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      308 2023-03-02 00:19:27.000000 sqlmesh-0.5.1.dev28/web/client/src/hooks/useActiveFocus.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)      817 2023-02-27 20:28:04.000000 sqlmesh-0.5.1.dev28/web/client/src/hooks/useLocalStorage.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9363 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/web/client/src/index.css
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.262545 sqlmesh-0.5.1.dev28/web/client/src/library/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.264126 sqlmesh-0.5.1.dev28/web/client/src/library/components/
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.390049 sqlmesh-0.5.1.dev28/web/client/src/library/components/banner/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1705 2023-04-20 18:21:56.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/banner/Banner.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.390373 sqlmesh-0.5.1.dev28/web/client/src/library/components/button/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4517 2023-03-25 06:07:32.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/button/Button.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.390683 sqlmesh-0.5.1.dev28/web/client/src/library/components/button/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3516 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/button/tests/Button.spec.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.390901 sqlmesh-0.5.1.dev28/web/client/src/library/components/divider/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      856 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/divider/Divider.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.391138 sqlmesh-0.5.1.dev28/web/client/src/library/components/divider/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      632 2023-02-14 21:38:27.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/divider/tests/Divider.spec.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.393525 sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1388 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/Editor.css
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5397 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/Editor.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8015 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/EditorCode.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2718 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/EditorFooter.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1990 2023-04-02 22:26:52.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/EditorIndicator.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9819 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/EditorInspector.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)    11303 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/EditorPreview.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3527 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/EditorTabs.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.393973 sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/extensions/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5880 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3987 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/extensions/index.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1538 2023-04-02 22:26:52.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/help.ts
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.394802 sqlmesh-0.5.1.dev28/web/client/src/library/components/fileTree/
+-rw-r--r--   0 izeigerman   (501) staff       (20)    10852 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/fileTree/Directory.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6045 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/fileTree/File.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2997 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/fileTree/FileTree.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)      562 2023-04-02 22:26:52.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/fileTree/help.ts
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.395324 sqlmesh-0.5.1.dev28/web/client/src/library/components/graph/
+-rw-r--r--   0 izeigerman   (501) staff       (20)    14478 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/graph/Graph.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6392 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/graph/help.ts
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.396254 sqlmesh-0.5.1.dev28/web/client/src/library/components/ide/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4342 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/ide/ActivePlan.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4870 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/ide/IDE.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)    22356 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/ide/RunPlan.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.397100 sqlmesh-0.5.1.dev28/web/client/src/library/components/input/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2087 2023-03-29 18:25:45.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/input/Input.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)      688 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/input/InputToggle.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.397331 sqlmesh-0.5.1.dev28/web/client/src/library/components/loading/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      486 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/loading/Loading.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.398106 sqlmesh-0.5.1.dev28/web/client/src/library/components/logo/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2292 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/logo/Spinner.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4637 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/logo/SqlMesh.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     8042 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/logo/Tobiko.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.399018 sqlmesh-0.5.1.dev28/web/client/src/library/components/modal/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1560 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/modal/Modal.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1953 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/modal/ModalConfirmation.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1447 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/modal/ModalDrawer.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.401878 sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9269 2023-04-20 18:21:56.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/Plan.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     6775 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/PlanActions.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1312 2023-03-29 18:25:45.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/PlanBackfillDates.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)    10448 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/PlanChangePreview.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4920 2023-04-20 18:21:56.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/PlanHeader.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)    15855 2023-04-20 18:21:56.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/PlanWizard.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     9926 2023-03-28 05:23:20.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/PlanWizardStepOptions.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)    12528 2023-04-20 18:21:56.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/context.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3444 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/help.spec.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2155 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/help.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2599 2023-04-20 18:21:56.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/hooks.ts
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.402093 sqlmesh-0.5.1.dev28/web/client/src/library/components/progress/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      713 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/progress/Progress.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.402320 sqlmesh-0.5.1.dev28/web/client/src/library/components/report/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1047 2023-04-20 18:21:56.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/report/ReportTestsErrors.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.403107 sqlmesh-0.5.1.dev28/web/client/src/library/components/root/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      526 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/root/Footer.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1921 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/root/Header.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)      247 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/root/Main.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)      443 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/root/Root.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.403522 sqlmesh-0.5.1.dev28/web/client/src/library/components/splitPane/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      788 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/splitPane/SplitPane.css
+-rw-r--r--   0 izeigerman   (501) staff       (20)      541 2023-03-16 22:35:40.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/splitPane/SplitPane.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.403958 sqlmesh-0.5.1.dev28/web/client/src/library/components/tasksOverview/
+-rw-r--r--   0 izeigerman   (501) staff       (20)    11713 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/tasksOverview/TasksOverview.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.404449 sqlmesh-0.5.1.dev28/web/client/src/library/components/toggle/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1453 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/src/library/components/toggle/Toggle.tsx
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1197 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/src/main.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.406069 sqlmesh-0.5.1.dev28/web/client/src/models/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1647 2023-04-02 22:26:52.000000 sqlmesh-0.5.1.dev28/web/client/src/models/artifact.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3472 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/web/client/src/models/directory.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4190 2023-03-16 22:35:40.000000 sqlmesh-0.5.1.dev28/web/client/src/models/environment.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1760 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev28/web/client/src/models/file.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)      173 2023-02-14 21:38:27.000000 sqlmesh-0.5.1.dev28/web/client/src/models/index.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)      766 2023-02-14 21:38:27.000000 sqlmesh-0.5.1.dev28/web/client/src/models/initial.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)      200 2023-02-14 21:38:27.000000 sqlmesh-0.5.1.dev28/web/client/src/routes.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.406678 sqlmesh-0.5.1.dev28/web/client/src/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)       35 2023-01-20 18:11:03.000000 sqlmesh-0.5.1.dev28/web/client/src/tests/setup.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)      541 2023-03-16 22:35:40.000000 sqlmesh-0.5.1.dev28/web/client/src/tests/utils.tsx
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.407319 sqlmesh-0.5.1.dev28/web/client/src/types/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      467 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/src/types/enum.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)      137 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/src/types/index.d.ts
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.407994 sqlmesh-0.5.1.dev28/web/client/src/utils/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4102 2023-03-24 20:30:10.000000 sqlmesh-0.5.1.dev28/web/client/src/utils/index.spec.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5245 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev28/web/client/src/utils/index.ts
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.408301 sqlmesh-0.5.1.dev28/web/client/src/workers/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      113 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/web/client/src/workers/index.ts
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.408805 sqlmesh-0.5.1.dev28/web/client/src/workers/sqlglot/
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1105 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev28/web/client/src/workers/sqlglot/sqlglot.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1578 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/web/client/src/workers/sqlglot/worker.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5842 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev28/web/client/tailwind.config.js
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.409155 sqlmesh-0.5.1.dev28/web/client/tests/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      170 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/web/client/tests/initial.spec.ts
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1141 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/web/client/tsconfig.json
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1297 2023-04-17 20:03:35.000000 sqlmesh-0.5.1.dev28/web/client/vite.config.ts
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.411331 sqlmesh-0.5.1.dev28/web/server/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-19 13:52:03.000000 sqlmesh-0.5.1.dev28/web/server/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.411574 sqlmesh-0.5.1.dev28/web/server/api/
+-rw-r--r--   0 izeigerman   (501) staff       (20)        0 2023-01-17 03:45:08.000000 sqlmesh-0.5.1.dev28/web/server/api/__init__.py
+drwxr-xr-x   0 izeigerman   (501) staff       (20)        0 2023-04-24 23:32:11.414692 sqlmesh-0.5.1.dev28/web/server/api/endpoints/
+-rw-r--r--   0 izeigerman   (501) staff       (20)      784 2023-04-17 20:03:31.000000 sqlmesh-0.5.1.dev28/web/server/api/endpoints/__init__.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     4564 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/web/server/api/endpoints/commands.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      819 2023-02-27 20:28:04.000000 sqlmesh-0.5.1.dev28/web/server/api/endpoints/context.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1858 2023-02-17 22:23:25.000000 sqlmesh-0.5.1.dev28/web/server/api/endpoints/directories.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      721 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/web/server/api/endpoints/environments.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      637 2023-02-15 19:33:57.000000 sqlmesh-0.5.1.dev28/web/server/api/endpoints/events.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5229 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/web/server/api/endpoints/files.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3283 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/web/server/api/endpoints/lineage.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      962 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/web/server/api/endpoints/models.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3628 2023-04-19 17:07:52.000000 sqlmesh-0.5.1.dev28/web/server/api/endpoints/plan.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     3775 2023-04-20 18:21:56.000000 sqlmesh-0.5.1.dev28/web/server/console.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     1374 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/web/server/main.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     5777 2023-04-21 18:09:59.000000 sqlmesh-0.5.1.dev28/web/server/models.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)      260 2023-04-07 21:24:23.000000 sqlmesh-0.5.1.dev28/web/server/openapi.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2421 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/web/server/settings.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2114 2023-02-04 22:32:08.000000 sqlmesh-0.5.1.dev28/web/server/sse.py
+-rw-r--r--   0 izeigerman   (501) staff       (20)     2461 2023-04-18 13:21:08.000000 sqlmesh-0.5.1.dev28/web/server/utils.py
```

### Comparing `sqlmesh-0.5.1.dev22/.circleci/config.yml` & `sqlmesh-0.5.1.dev28/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/.circleci/continue_config.yml` & `sqlmesh-0.5.1.dev28/.circleci/continue_config.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/.gitignore` & `sqlmesh-0.5.1.dev28/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/.pre-commit-config.yaml` & `sqlmesh-0.5.1.dev28/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/LICENSE` & `sqlmesh-0.5.1.dev28/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/Makefile` & `sqlmesh-0.5.1.dev28/Makefile`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/PKG-INFO` & `sqlmesh-0.5.1.dev28/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,15 @@
 Metadata-Version: 2.1
 Name: sqlmesh
-Version: 0.5.1.dev22
+Version: 0.5.1.dev28
 Summary: UNKNOWN
 Home-page: https://github.com/TobikoData/sqlmesh
 Author: TobikoData Inc.
 Author-email: engineering@tobikodata.com
 License: Apache License 2.0
-Description: ![SQLMesh logo](sqlmesh.svg)
-        
-        SQLMesh is a DataOps framework that brings the benefits of DevOps to data teams. It enables data scientists, analysts, and engineers to efficiently run and deploy data transformations written in SQL or Python.
-        
-        For more information, check out the [website](https://sqlmesh.com) and [documentation](https://sqlmesh.readthedocs.io/en/stable/).
-        
-        ## Geting Started
-        Install SQLMesh through [pypi](https://pypi.org/project/sqlmesh/) by running:
-        
-        ```pip install sqlmesh```
-        
-        Follow the [tutorial](https://sqlmesh.readthedocs.io/en/stable/quick_start/) to learn how to use SQLMesh.
-        
-        ## Join our community
-        We'd love to join you on your data journey. Connect with us in the following ways:
-        
-        * Join the [Tobiko Slack community](https://join.slack.com/t/tobiko-data/shared_invite/zt-1ma66d79v-a4dbf4DUpLAQJ8ptQrJygg) to ask questions, or just to say hi!
-        * File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
-        * Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
-        
-        ## Contribution
-        Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
-        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -41,7 +18,33 @@
 Provides-Extra: databricks
 Provides-Extra: dev
 Provides-Extra: dbt
 Provides-Extra: postgres
 Provides-Extra: redshift
 Provides-Extra: snowflake
 Provides-Extra: web
+License-File: LICENSE
+
+![SQLMesh logo](sqlmesh.svg)
+
+SQLMesh is a DataOps framework that brings the benefits of DevOps to data teams. It enables data scientists, analysts, and engineers to efficiently run and deploy data transformations written in SQL or Python.
+
+For more information, check out the [website](https://sqlmesh.com) and [documentation](https://sqlmesh.readthedocs.io/en/stable/).
+
+## Geting Started
+Install SQLMesh through [pypi](https://pypi.org/project/sqlmesh/) by running:
+
+```pip install sqlmesh```
+
+Follow the [tutorial](https://sqlmesh.readthedocs.io/en/stable/quick_start/) to learn how to use SQLMesh.
+
+## Join our community
+We'd love to join you on your data journey. Connect with us in the following ways:
+
+* Join the [Tobiko Slack community](https://join.slack.com/t/tobiko-data/shared_invite/zt-1ma66d79v-a4dbf4DUpLAQJ8ptQrJygg) to ask questions, or just to say hi!
+* File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
+* Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
+
+## Contribution
+Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
+
+
```

### Comparing `sqlmesh-0.5.1.dev22/README.md` & `sqlmesh-0.5.1.dev28/README.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docker-compose.yml` & `sqlmesh-0.5.1.dev28/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/comparisons.md` & `sqlmesh-0.5.1.dev28/docs/comparisons.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/concepts/architecture/serialization.md` & `sqlmesh-0.5.1.dev28/docs/concepts/architecture/serialization.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/concepts/architecture/snapshots.md` & `sqlmesh-0.5.1.dev28/docs/concepts/architecture/snapshots.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/concepts/audits.md` & `sqlmesh-0.5.1.dev28/docs/concepts/audits.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/concepts/environments.md` & `sqlmesh-0.5.1.dev28/docs/concepts/environments.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/concepts/glossary.md` & `sqlmesh-0.5.1.dev28/docs/concepts/glossary.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/concepts/macros.md` & `sqlmesh-0.5.1.dev28/docs/concepts/macros.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/concepts/models/model_kinds.md` & `sqlmesh-0.5.1.dev28/docs/concepts/models/model_kinds.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/concepts/models/overview.md` & `sqlmesh-0.5.1.dev28/docs/concepts/models/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/concepts/models/python_models.md` & `sqlmesh-0.5.1.dev28/docs/concepts/models/python_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/concepts/models/seed_models.md` & `sqlmesh-0.5.1.dev28/docs/concepts/models/seed_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/concepts/models/sql_models.md` & `sqlmesh-0.5.1.dev28/docs/concepts/models/sql_models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/concepts/overview.md` & `sqlmesh-0.5.1.dev28/docs/concepts/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/concepts/plans/model_versioning.png` & `sqlmesh-0.5.1.dev28/docs/concepts/plans/model_versioning.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/concepts/plans.md` & `sqlmesh-0.5.1.dev28/docs/concepts/plans.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/concepts/tests.md` & `sqlmesh-0.5.1.dev28/docs/concepts/tests.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/development.md` & `sqlmesh-0.5.1.dev28/docs/development.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/guides/connections.md` & `sqlmesh-0.5.1.dev28/docs/guides/connections.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/guides/migrations.md` & `sqlmesh-0.5.1.dev28/docs/guides/migrations.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/guides/models.md` & `sqlmesh-0.5.1.dev28/docs/guides/models.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/guides/multi_repo.md` & `sqlmesh-0.5.1.dev28/docs/guides/multi_repo.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/guides/projects.md` & `sqlmesh-0.5.1.dev28/docs/guides/projects.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/guides/scheduling/airflow_successful_plan_apply.png` & `sqlmesh-0.5.1.dev28/docs/guides/scheduling/airflow_successful_plan_apply.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/guides/scheduling/airflow_successful_setup.png` & `sqlmesh-0.5.1.dev28/docs/guides/scheduling/airflow_successful_setup.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/guides/scheduling.md` & `sqlmesh-0.5.1.dev28/docs/guides/scheduling.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/guides/testing.md` & `sqlmesh-0.5.1.dev28/docs/guides/testing.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/index.md` & `sqlmesh-0.5.1.dev28/docs/index.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/integrations/airflow.md` & `sqlmesh-0.5.1.dev28/docs/integrations/airflow.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/integrations/dbt.md` & `sqlmesh-0.5.1.dev28/docs/integrations/dbt.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/integrations/engines.md` & `sqlmesh-0.5.1.dev28/docs/integrations/engines.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/integrations/github.md` & `sqlmesh-0.5.1.dev28/docs/integrations/github.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/prerequisites.md` & `sqlmesh-0.5.1.dev28/docs/prerequisites.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/quick_start.md` & `sqlmesh-0.5.1.dev28/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/reference/cli.md` & `sqlmesh-0.5.1.dev28/docs/reference/cli.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/reference/configuration.md` & `sqlmesh-0.5.1.dev28/docs/reference/configuration.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/reference/notebook.md` & `sqlmesh-0.5.1.dev28/docs/reference/notebook.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/reference/overview.md` & `sqlmesh-0.5.1.dev28/docs/reference/overview.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/docs/sqlmesh.png` & `sqlmesh-0.5.1.dev28/docs/sqlmesh.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/airflow/Dockerfile.template` & `sqlmesh-0.5.1.dev28/examples/airflow/Dockerfile.template`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/airflow/Makefile` & `sqlmesh-0.5.1.dev28/examples/airflow/Makefile`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/airflow/README.md` & `sqlmesh-0.5.1.dev28/examples/airflow/README.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/airflow/docker_compose_decorator.py` & `sqlmesh-0.5.1.dev28/examples/airflow/docker_compose_decorator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/airflow/spark_conf/hive-site.xml` & `sqlmesh-0.5.1.dev28/examples/airflow/spark_conf/hive-site.xml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/sushi/config.py` & `sqlmesh-0.5.1.dev28/examples/sushi/config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/sushi/helper.py` & `sqlmesh-0.5.1.dev28/examples/sushi/helper.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/sushi/macros/macros.py` & `sqlmesh-0.5.1.dev28/examples/sushi/macros/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/sushi/models/customer_revenue_by_day.sql` & `sqlmesh-0.5.1.dev28/examples/sushi/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/sushi/models/items.py` & `sqlmesh-0.5.1.dev28/examples/sushi/models/items.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/sushi/models/order_items.py` & `sqlmesh-0.5.1.dev28/examples/sushi/models/order_items.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/sushi/models/orders.py` & `sqlmesh-0.5.1.dev28/examples/sushi/models/orders.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/sushi/models/waiter_revenue_by_day.sql` & `sqlmesh-0.5.1.dev28/examples/sushi/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/sushi/tests/test_customer_revenue_by_day.yaml` & `sqlmesh-0.5.1.dev28/examples/sushi/tests/test_customer_revenue_by_day.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/sushi_dbt/macros/incremental.sql` & `sqlmesh-0.5.1.dev28/examples/sushi_dbt/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/sushi_dbt/models/customer_revenue_by_day.sql` & `sqlmesh-0.5.1.dev28/examples/sushi_dbt/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/sushi_dbt/models/waiter_revenue_by_day.sql` & `sqlmesh-0.5.1.dev28/examples/sushi_dbt/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/sushi_dbt/packages/customers/dbt_project.yml` & `sqlmesh-0.5.1.dev28/examples/sushi_dbt/packages/customers/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/sushi_dbt/profiles.yml` & `sqlmesh-0.5.1.dev28/examples/sushi_dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/sushi_dbt/seeds/items.csv` & `sqlmesh-0.5.1.dev28/examples/sushi_dbt/seeds/items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/sushi_dbt/seeds/order_items.csv` & `sqlmesh-0.5.1.dev28/examples/sushi_dbt/seeds/order_items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/sushi_dbt/seeds/orders.csv` & `sqlmesh-0.5.1.dev28/examples/sushi_dbt/seeds/orders.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/wursthall/macros/macros.py` & `sqlmesh-0.5.1.dev28/examples/wursthall/macros/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/wursthall/models/db/order_f.py` & `sqlmesh-0.5.1.dev28/examples/wursthall/models/db/order_f.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/wursthall/models/db/order_item_f.sql` & `sqlmesh-0.5.1.dev28/examples/wursthall/models/db/order_item_f.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/wursthall/models/src/customer_details.py` & `sqlmesh-0.5.1.dev28/examples/wursthall/models/src/customer_details.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/wursthall/models/src/order_item_details.py` & `sqlmesh-0.5.1.dev28/examples/wursthall/models/src/order_item_details.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/wursthall/models/src/shared.py` & `sqlmesh-0.5.1.dev28/examples/wursthall/models/src/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/wursthall/seeds/src/menu_item_details.csv` & `sqlmesh-0.5.1.dev28/examples/wursthall/seeds/src/menu_item_details.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/wursthall/tests/test_customer_d.yaml` & `sqlmesh-0.5.1.dev28/examples/wursthall/tests/test_customer_d.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/examples/wursthall/tests/test_order_item_f.yaml` & `sqlmesh-0.5.1.dev28/examples/wursthall/tests/test_order_item_f.yaml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/mkdocs.yml` & `sqlmesh-0.5.1.dev28/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/pdoc/cli.py` & `sqlmesh-0.5.1.dev28/pdoc/cli.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/posts/virtual_data_environments/change_categorization.png` & `sqlmesh-0.5.1.dev28/posts/virtual_data_environments/change_categorization.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/posts/virtual_data_environments/isolated_rigid_envs.png` & `sqlmesh-0.5.1.dev28/posts/virtual_data_environments/isolated_rigid_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/posts/virtual_data_environments/partial_breaking.png` & `sqlmesh-0.5.1.dev28/posts/virtual_data_environments/partial_breaking.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/posts/virtual_data_environments/stateful_envs.png` & `sqlmesh-0.5.1.dev28/posts/virtual_data_environments/stateful_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/posts/virtual_data_environments/virtual_envs.png` & `sqlmesh-0.5.1.dev28/posts/virtual_data_environments/virtual_envs.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/posts/virtual_data_environments/virtual_envs_end_to_end.png` & `sqlmesh-0.5.1.dev28/posts/virtual_data_environments/virtual_envs_end_to_end.png`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/posts/virtual_data_environments.md` & `sqlmesh-0.5.1.dev28/posts/virtual_data_environments.md`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/pytest.ini` & `sqlmesh-0.5.1.dev28/pytest.ini`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/setup.cfg` & `sqlmesh-0.5.1.dev28/setup.cfg`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/setup.py` & `sqlmesh-0.5.1.dev28/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         "hyperscript",
         "jinja2",
         "pandas",
         "pydantic>=1.9.1,<2.0.0",
         "requests",
         "rich",
         "ruamel.yaml",
-        "sqlglot~=11.5.6",
+        "sqlglot~=11.5.7",
         "fsspec",
     ],
     extras_require={
         "bigquery": [
             "google-cloud-bigquery[pandas]",
             "google-cloud-bigquery-storage",
         ],
```

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/__init__.py` & `sqlmesh-0.5.1.dev28/sqlmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/cli/__init__.py` & `sqlmesh-0.5.1.dev28/sqlmesh/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/cli/example_project.py` & `sqlmesh-0.5.1.dev28/sqlmesh/cli/example_project.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/cli/main.py` & `sqlmesh-0.5.1.dev28/sqlmesh/cli/main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/cli/options.py` & `sqlmesh-0.5.1.dev28/sqlmesh/cli/options.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/_typing.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/_typing.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/audit/builtin.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/audit/builtin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/audit/definition.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/audit/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/config/__init__.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/config/base.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/config/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/config/categorizer.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/config/categorizer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/config/common.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/config/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/config/connection.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/config/connection.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/config/loader.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/config/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/config/model.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/config/model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/config/root.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/config/root.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/config/scheduler.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/config/scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/console.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/console.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/constants.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/constants.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/context.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/context_diff.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/context_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/dialect.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/dialect.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/__init__.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/_typing.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/_typing.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/base.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/base_postgres.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/base_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/base_spark.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/base_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/bigquery.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/databricks_api.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/databricks_api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/duckdb.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/postgres.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/redshift.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/shared.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/snowflake.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/engine_adapter/spark.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/engine_adapter/spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/environment.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/environment.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/hooks.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/hooks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/loader.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/loader.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/macros.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/model/__init__.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/model/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/model/cache.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/model/cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/model/common.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/model/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/model/decorator.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/model/decorator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/model/definition.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/model/definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,17 +88,18 @@
             [croniter](https://github.com/kiorky/croniter) library.
         description: The optional model description.
         stamp: An optional arbitrary string sequence used to create new model versions without making
             changes to any of the functional components of the definition.
         start: The earliest date that the model will be backfilled for. If this is None,
             then the date is inferred by taking the most recent start date of its ancestors.
             The start date can be a static datetime or a relative datetime like "1 year ago"
-        batch_size: The maximum number of intervals that can be run per backfill job. If this is None,
+        batch_size: The maximum number of incremental intervals that can be run per backfill job. If this is None,
             then backfilling this model will do all of history in one job. If this is set, a model's backfill
             will be chunked such that each individual job will only contain jobs with max `batch_size` intervals.
+        lookback: The number of previous incremental intervals in the lookback window.
         storage_format: The storage format used to store the physical table, only applicable in certain engines.
             (eg. 'parquet')
         partitioned_by: The partition columns, only applicable in certain engines. (eg. (ds, hour))
         pre: Pre-hooks to run before the model executes.
         post: Post-hooks to run after the model executes.
         expressions: All of the expressions between the model definition and final query, used for setting certain variables or environments.
         python_env: Dictionary containing all global variables needed to render the model's macros.
```

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/model/kind.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/model/kind.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/model/meta.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/model/meta.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import typing as t
+from datetime import timedelta
 from enum import Enum
 
 from croniter import croniter
 from pydantic import Field, root_validator, validator
 from sqlglot import exp, maybe_parse
 
 import sqlmesh.core.dialect as d
@@ -253,14 +254,27 @@
 
     @property
     def lookback(self) -> int:
         """The incremental lookback window."""
         return (self.kind.lookback if isinstance(self.kind, _Incremental) else 0) or 0
 
     @property
+    def lookback_delta(self) -> timedelta:
+        """The incremental lookback time delta."""
+        if isinstance(self.kind, _Incremental):
+            interval_unit = self.interval_unit()
+            if interval_unit == IntervalUnit.DAY:
+                return timedelta(days=self.lookback)
+            if interval_unit == IntervalUnit.HOUR:
+                return timedelta(hours=self.lookback)
+            if interval_unit == IntervalUnit.MINUTE:
+                return timedelta(minutes=self.lookback)
+        return timedelta()
+
+    @property
     def batch_size(self) -> t.Optional[int]:
         """The maximal number of units in a single task for a backfill."""
         return self.kind.batch_size if isinstance(self.kind, _Incremental) else None
 
     def interval_unit(self, sample_size: int = 10) -> IntervalUnit:
         """Returns the IntervalUnit of the model
```

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/model/seed.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/model/seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/notification_target.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/notification_target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/plan/definition.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/plan/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/plan/evaluator.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/plan/evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/renderer.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/renderer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/scheduler.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/schema_diff.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/schema_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/snapshot/__init__.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/snapshot/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/snapshot/categorizer.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/snapshot/categorizer.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/snapshot/definition.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/snapshot/definition.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/snapshot/evaluator.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/snapshot/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,20 @@
 from contextlib import contextmanager
 
 from sqlglot import exp, select
 from sqlglot.executor import execute
 
 from sqlmesh.core.audit import BUILT_IN_AUDITS, AuditResult
 from sqlmesh.core.engine_adapter import EngineAdapter, TransactionType
-from sqlmesh.core.snapshot import Snapshot, SnapshotId, SnapshotInfoLike
+from sqlmesh.core.snapshot import (
+    Snapshot,
+    SnapshotChangeCategory,
+    SnapshotId,
+    SnapshotInfoLike,
+)
 from sqlmesh.utils.concurrency import concurrent_apply_to_snapshots
 from sqlmesh.utils.date import TimeLike
 from sqlmesh.utils.errors import AuditError, ConfigError, SQLMeshError
 
 if t.TYPE_CHECKING:
     from sqlmesh.core.engine_adapter._typing import DF, QueryOrDF
 
@@ -396,15 +401,18 @@
                     snapshot.model.columns_to_types,
                     storage_format=snapshot.model.storage_format,
                     partitioned_by=snapshot.model.partitioned_by,
                     partition_interval_unit=snapshot.model.interval_unit(),
                 )
 
     def _migrate_snapshot(self, snapshot: SnapshotInfoLike) -> None:
-        if not snapshot.is_materialized or snapshot.is_new_version:
+        if (
+            not snapshot.is_materialized
+            or snapshot.change_category != SnapshotChangeCategory.FORWARD_ONLY
+        ):
             return
 
         tmp_table_name = snapshot.table_name(is_dev=True)
         target_table_name = snapshot.table_name()
 
         logger.info(f"Altering table '{target_table_name}'")
         self.adapter.alter_table(target_table_name, tmp_table_name)
```

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/state_sync/__init__.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/state_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/state_sync/base.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/state_sync/base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/state_sync/common.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/state_sync/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/state_sync/engine_adapter.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/state_sync/engine_adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/test.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/test.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/core/user.py` & `sqlmesh-0.5.1.dev28/sqlmesh/core/user.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/dbt/adapter.py` & `sqlmesh-0.5.1.dev28/sqlmesh/dbt/adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/dbt/basemodel.py` & `sqlmesh-0.5.1.dev28/sqlmesh/dbt/basemodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from sqlmesh.dbt.adapter import ParsetimeAdapter
 from sqlmesh.dbt.column import (
     ColumnConfig,
     column_descriptions_to_sqlmesh,
     column_types_to_sqlmesh,
     yaml_to_columns,
 )
-from sqlmesh.dbt.common import GeneralConfig, QuotingConfig, SqlStr
+from sqlmesh.dbt.common import DbtConfig, GeneralConfig, QuotingConfig, SqlStr
 from sqlmesh.dbt.context import DbtContext
 from sqlmesh.utils import AttributeDict
 from sqlmesh.utils.conversions import ensure_bool
 from sqlmesh.utils.date import date_dict
 from sqlmesh.utils.errors import ConfigError
 from sqlmesh.utils.jinja import MacroReference, extract_macro_references
 from sqlmesh.utils.pydantic import PydanticModel
@@ -67,14 +67,25 @@
 
     TABLE = "table"
     VIEW = "view"
     INCREMENTAL = "incremental"
     EPHEMERAL = "ephemeral"
 
 
+class Hook(DbtConfig):
+    """
+    Args:
+        sql: The sql to execute.
+        transaction: bool indicating if the hook is executed in the same transaction as the model query.
+    """
+
+    sql: SqlStr
+    transaction: bool = True  # TODO not yet supported
+
+
 class BaseModelConfig(GeneralConfig):
     """
     Args:
         owner: The owner of the model.
         stamp: An optional arbitrary string sequence used to create new model versions without making
             changes to any of the functional components of the definition.
         storage_format: The storage format used to store the physical table, only applicable in certain engines.
@@ -101,36 +112,47 @@
     _dependencies: Dependencies = Dependencies()
     _variables: t.Dict[str, bool] = {}
 
     # DBT configuration fields
     database: t.Optional[str] = None
     schema_: t.Optional[str] = Field(None, alias="schema")
     alias: t.Optional[str] = None
-    pre_hook: t.List[SqlStr] = Field([], alias="pre-hook")
-    post_hook: t.List[SqlStr] = Field([], alias="post-hook")
+    pre_hook: t.List[Hook] = Field([], alias="pre-hook")
+    post_hook: t.List[Hook] = Field([], alias="post-hook")
     full_refresh: t.Optional[bool] = None
     grants: t.Dict[str, t.List[str]] = {}
     columns: t.Dict[str, ColumnConfig] = {}
     quoting: QuotingConfig = Field(default_factory=QuotingConfig)
 
     @validator("pre_hook", "post_hook", pre=True)
-    def _validate_hooks(cls, v: t.Union[str, t.List[t.Union[SqlStr, str]]]) -> t.List[SqlStr]:
-        return [SqlStr(val) for val in ensure_list(v)]
+    def _validate_hooks(cls, v: t.Union[str, t.List[t.Union[SqlStr, str]]]) -> t.List[Hook]:
+        hooks = []
+        for hook in ensure_list(v):
+            if isinstance(hook, Hook):
+                hooks.append(hook)
+            elif isinstance(hook, str):
+                hooks.append(Hook(sql=hook))
+            elif isinstance(hook, dict):
+                hooks.append(Hook(**hook))
+            else:
+                raise ConfigError(f"Invalid hook data: {hook}")
+
+        return hooks
 
     @validator("full_refresh", pre=True)
     def _validate_bool(cls, v: str) -> bool:
         return ensure_bool(v)
 
     @validator("grants", pre=True)
     def _validate_grants(cls, v: t.Dict[str, str]) -> t.Dict[str, t.List[str]]:
         return {key: ensure_list(value) for key, value in v.items()}
 
     @validator("columns", pre=True)
     def _validate_columns(cls, v: t.Any) -> t.Dict[str, ColumnConfig]:
-        if not isinstance(v, dict) or all(isinstance(col, ColumnConfig) for col in v.values()):
+        if isinstance(v, dict) and all(isinstance(col, ColumnConfig) for col in v.values()):
             return v
 
         return yaml_to_columns(v)
 
     _FIELD_UPDATE_STRATEGY: t.ClassVar[t.Dict[str, UpdateStrategy]] = {
         **GeneralConfig._FIELD_UPDATE_STRATEGY,
         **{
@@ -140,15 +162,21 @@
             "post-hook": UpdateStrategy.EXTEND,
             "columns": UpdateStrategy.KEY_EXTEND,
         },
     }
 
     @property
     def all_sql(self) -> SqlStr:
-        return SqlStr("\n".join(self.pre_hook + [self.sql_no_config] + self.post_hook))
+        return SqlStr(
+            "\n".join(
+                [hook.sql for hook in self.pre_hook]
+                + [self.sql_no_config]
+                + [hook.sql for hook in self.post_hook]
+            )
+        )
 
     @property
     def sql_no_config(self) -> SqlStr:
         return SqlStr("")
 
     @property
     def sql_embedded_config(self) -> SqlStr:
@@ -226,16 +254,16 @@
 
         return {
             "columns": column_types_to_sqlmesh(self.columns) or None,
             "column_descriptions_": column_descriptions_to_sqlmesh(self.columns) or None,
             "depends_on": {model_context.refs[ref] for ref in self._dependencies.refs},
             "jinja_macros": jinja_macros,
             "path": self.path,
-            "pre": [exp for hook in self.pre_hook for exp in d.parse(hook)],
-            "post": [exp for hook in self.post_hook for exp in d.parse(hook)],
+            "pre": [exp for hook in self.pre_hook for exp in d.parse(hook.sql)],
+            "post": [exp for hook in self.post_hook for exp in d.parse(hook.sql)],
             **optional_kwargs,
         }
 
     def render_config(self: BMC, context: DbtContext) -> BMC:
         rendered = super().render_config(context)
         rendered = ModelSqlRenderer(context, rendered).enriched_config
```

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/dbt/builtin.py` & `sqlmesh-0.5.1.dev28/sqlmesh/dbt/builtin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/dbt/column.py` & `sqlmesh-0.5.1.dev28/sqlmesh/dbt/column.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,19 +53,15 @@
 class ColumnConfig(GeneralConfig):
     """
     Column configuration for a DBT project
 
     Args:
         name: Name of the column
         data_type: The column's data type
-        description: User defined description of the column
-        meta: Meta data associated with the column
         quote: Boolean flag to use quoting for the column name
-        tests: Tests associated with this column
-        tags: Tags associated with this column
     """
 
     name: str
     data_type: t.Optional[str] = None
     quote: t.Optional[bool] = False
 
     @validator("quote", pre=True)
```

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/dbt/common.py` & `sqlmesh-0.5.1.dev28/sqlmesh/dbt/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "statement",
     "store_result",
     "target",
 }
 
 
 def load_yaml(source: str | Path) -> t.OrderedDict:
-    return load(source, render_jinja=False)
+    return load(source, render_jinja=False, allow_duplicate_keys=True)
 
 
 def parse_meta(v: t.Dict[str, t.Any]) -> t.Dict[str, t.Any]:
     for key, value in v.items():
         if isinstance(value, str):
             v[key] = try_str_to_bool(value)
 
@@ -75,15 +75,15 @@
         tags: List of tags that can be used for element grouping
         meta: Dictionary of metadata for the element
     """
 
     start: t.Optional[str] = None
     description: t.Optional[str] = None
     # TODO add test support
-    tests: t.Dict[str, t.Any] = {}
+    tests: t.List[t.Any] = []
     enabled: bool = True
     docs: t.Dict[str, t.Any] = {"show": True}
     persist_docs: t.Dict[str, t.Any] = {}
     tags: t.List[str] = []
     meta: t.Dict[str, t.Any] = {}
 
     @validator("enabled", pre=True)
```

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/dbt/context.py` & `sqlmesh-0.5.1.dev28/sqlmesh/dbt/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     _variables: t.Dict[str, t.Any] = field(default_factory=dict)
     _models: t.Dict[str, ModelConfig] = field(default_factory=dict)
     _seeds: t.Dict[str, SeedConfig] = field(default_factory=dict)
     _sources: t.Dict[str, SourceConfig] = field(default_factory=dict)
     _refs: t.Dict[str, str] = field(default_factory=dict)
 
-    _target: TargetConfig = field(default_factory=TargetConfig)
+    _target: t.Optional[TargetConfig] = None
 
     _jinja_environment: t.Optional[Environment] = None
 
     @property
     def dialect(self) -> str:
         return self.engine_adapter.dialect if self.engine_adapter is not None else ""
 
@@ -106,15 +106,15 @@
     @property
     def refs(self) -> t.Dict[str, str]:
         if not self._refs:
             self._refs = {k: v.model_name for k, v in {**self._seeds, **self._models}.items()}  # type: ignore
         return self._refs
 
     @property
-    def target(self) -> TargetConfig:
+    def target(self) -> t.Optional[TargetConfig]:
         return self._target
 
     @target.setter
     def target(self, value: TargetConfig) -> None:
         if not self.project_name:
             raise ConfigError("Project name must be set in the context in order to use a target.")
 
@@ -142,10 +142,10 @@
         output: t.Dict[str, JinjaGlobalAttribute] = {
             "vars": AttributeDict(self.variables),
             "refs": AttributeDict({k: v.relation_info for k, v in refs.items()}),
             "sources": AttributeDict({k: v.relation_info for k, v in self.sources.items()}),
         }
         if self.project_name is not None:
             output["project_name"] = self.project_name
-        if self._target is not None and self.project_name is not None:
-            output["target"] = self._target.target_jinja(self.project_name)
+        if self._target is not None:
+            output["target"] = self._target.attribute_dict()
         return output
```

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/dbt/loader.py` & `sqlmesh-0.5.1.dev28/sqlmesh/dbt/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from sqlmesh.core.model import Model, ModelCache
 from sqlmesh.dbt.basemodel import BaseModelConfig
 from sqlmesh.dbt.context import DbtContext
 from sqlmesh.dbt.model import ModelConfig
 from sqlmesh.dbt.profile import Profile
 from sqlmesh.dbt.project import Project
 from sqlmesh.dbt.seed import SeedConfig
+from sqlmesh.dbt.target import TargetConfig
 from sqlmesh.utils import UniqueKeyDict
 from sqlmesh.utils.cache import FileCache
 
 
 def sqlmesh_config(project_root: t.Optional[Path] = None, **kwargs: t.Any) -> Config:
     project_root = project_root or Path()
     context = DbtContext(project_root=project_root)
@@ -144,15 +145,16 @@
             yaml_max_mtimes: t.Dict[Path, float],
         ):
             self._loader = loader
             self._project = project
             self._macros_max_mtime = macros_max_mtime
             self._yaml_max_mtimes = yaml_max_mtimes
 
-            cache_path = loader._context.path / c.CACHE / project.context.target.name
+            target = t.cast(TargetConfig, project.context.target)
+            cache_path = loader._context.path / c.CACHE / target.name
             self._model_cache = ModelCache(cache_path)
             self._model_config_cache = FileCache(cache_path, ModelConfig, prefix="model_config")
             self._seed_config_cache = FileCache(cache_path, SeedConfig, prefix="seed_config")
 
         def get_or_load_model(self, target_path: Path, loader: t.Callable[[], Model]) -> Model:
             return self._model_cache.get_or_load(
                 self._cache_entry_name(target_path), self._cache_entry_id(target_path), loader
```

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/dbt/model.py` & `sqlmesh-0.5.1.dev28/sqlmesh/dbt/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,32 +43,34 @@
         time_column: The name of the time column
         partitioned_by: List of columns to partition by. time_column will automatically be
             included, if specified.
         cron: A cron string specifying how often the model should be refreshed, leveraging the
             [croniter](https://github.com/kiorky/croniter) library.
         dialect: The SQL dialect that the model's query is written in. By default,
             this is assumed to be the dialect of the context.
-        batch_size: The maximum number of intervals that can be run per backfill job. If this is None,
+        batch_size: The maximum number of incremental intervals that can be run per backfill job. If this is None,
             then backfilling this model will do all of history in one job. If this is set, a model's backfill
             will be chunked such that each individual job will only contain jobs with max `batch_size` intervals.
+        lookback: The number of previous incremental intervals in the lookback window.
         start: The earliest date that the model will be backfilled for
         cluster_by: Field(s) to use for clustering in data warehouses that support clustering
         incremental_strategy: Strategy used to build the incremental model
         materialized: How the model will be materialized in the database
         sql_header: SQL statement to inject above create table/view as
         unique_key: List of columns that define row uniqueness for the model
     """
 
     # sqlmesh fields
     sql: SqlStr = SqlStr("")
     time_column: t.Optional[str] = None
     partitioned_by: t.Optional[t.Union[t.List[str], str]] = None
     cron: t.Optional[str] = None
     dialect: t.Optional[str] = None
-    batch_size: t.Optional[int]
+    batch_size: t.Optional[int] = None
+    lookback: t.Optional[int] = None
 
     # DBT configuration fields
     start: t.Optional[str] = None
     cluster_by: t.Optional[t.List[str]] = None
     incremental_strategy: t.Optional[str] = None
     materialized: str = Materialization.VIEW.value
     sql_header: t.Optional[str] = None
@@ -118,37 +120,45 @@
         """
         materialization = self.model_materialization
         if materialization == Materialization.TABLE:
             return ModelKind(name=ModelKindName.FULL)
         if materialization == Materialization.VIEW:
             return ModelKind(name=ModelKindName.VIEW)
         if materialization == Materialization.INCREMENTAL:
+            incremental_kwargs = {}
+            for field in ("batch_size", "lookback"):
+                field_val = getattr(self, field, None) or self.meta.get(field, None)
+                if field_val:
+                    incremental_kwargs[field] = field_val
+
             if self.time_column:
                 strategy = self.incremental_strategy or target.default_incremental_strategy(
                     IncrementalByTimeRangeKind
                 )
                 if strategy not in INCREMENTAL_BY_TIME_STRATEGIES:
                     raise ConfigError(
                         f"SQLMesh IncrementalByTime is not compatible with '{strategy}'"
                         f" incremental strategy. Supported strategies include {collection_to_str(INCREMENTAL_BY_TIME_STRATEGIES)}."
                     )
-                return IncrementalByTimeRangeKind(time_column=self.time_column)
+                return IncrementalByTimeRangeKind(
+                    time_column=self.time_column, **incremental_kwargs
+                )
             if self.unique_key:
                 strategy = self.incremental_strategy or target.default_incremental_strategy(
                     IncrementalByUniqueKeyKind
                 )
                 if (
                     self.incremental_strategy
                     and strategy not in INCREMENTAL_BY_UNIQUE_KEY_STRATEGIES
                 ):
                     raise ConfigError(
                         f"{self.model_name}: SQLMesh IncrementalByUniqueKey is not compatible with '{strategy}'"
                         f" incremental strategy. Supported strategies include {collection_to_str(INCREMENTAL_BY_UNIQUE_KEY_STRATEGIES)}."
                     )
-                return IncrementalByUniqueKeyKind(unique_key=self.unique_key)
+                return IncrementalByUniqueKeyKind(unique_key=self.unique_key, **incremental_kwargs)
 
             raise ConfigError(
                 f"{self.model_name}: Incremental materialization requires either a "
                 f"time_column {collection_to_str(INCREMENTAL_BY_TIME_STRATEGIES)}) or a "
                 f"unique_key ({collection_to_str(INCREMENTAL_BY_UNIQUE_KEY_STRATEGIES.union(['none']))}) configuration."
             )
         if materialization == Materialization.EPHEMERAL:
@@ -204,19 +214,22 @@
         expressions = d.parse(self.sql_no_config)
         if not expressions:
             raise ConfigError(f"Model '{self.table_name}' must have a query.")
 
         optional_kwargs: t.Dict[str, t.Any] = {}
         if self.partitioned_by:
             optional_kwargs["partitioned_by"] = self.partitioned_by
-        for field in ("cron", "batch_size"):
+        for field in ["cron"]:
             field_val = getattr(self, field, None) or self.meta.get(field, None)
             if field_val:
                 optional_kwargs[field] = field_val
 
+        if not context.target:
+            raise ConfigError(f"Target required to load '{self.model_name}' into SQLMesh.")
+
         return create_sql_model(
             self.model_name,
             expressions[-1],
             dialect=self.model_dialect or model_context.dialect,
             kind=self.model_kind(context.target),
             start=self.start,
             statements=expressions[0:-1],
```

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/dbt/package.py` & `sqlmesh-0.5.1.dev28/sqlmesh/dbt/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     SqlStr,
     load_yaml,
 )
 from sqlmesh.dbt.context import DbtContext
 from sqlmesh.dbt.model import ModelConfig
 from sqlmesh.dbt.seed import SeedConfig
 from sqlmesh.dbt.source import SourceConfig
+from sqlmesh.dbt.target import TargetConfig
 from sqlmesh.utils.errors import ConfigError
 from sqlmesh.utils.jinja import MacroExtractor, MacroInfo
 from sqlmesh.utils.pydantic import PydanticModel
 
 if t.TYPE_CHECKING:
     C = t.TypeVar("C", bound=BaseConfig)
 
@@ -142,31 +143,33 @@
             scoped_configs[scope] = config
             for key, value in nested_config.items():
                 nested_scope = (*scope, key)
                 load_config(value, config, nested_scope, scoped_configs)
 
             return scoped_configs
 
+        target = self._context.target or self._create_empty_target()
+
         if "quoting" in yaml:
             quoting = QuotingConfig(**yaml["quoting"])
         else:
-            quoting = self._context.target.quoting
+            quoting = target.quoting
 
         scope = ()
         self.project_config.source_config = load_config(
             yaml.get("sources", {}), SourceConfig(quoting=quoting), scope
         )
         self.project_config.seed_config = load_config(
             yaml.get("seeds", {}),
-            SeedConfig(target_schema=self._context.target.schema_, quoting=quoting),
+            SeedConfig(target_schema=target.schema_, quoting=quoting),
             scope,
         )
         self.project_config.model_config = load_config(
             yaml.get("models", {}),
-            ModelConfig(target_schema=self._context.target.schema_, quoting=quoting),
+            ModelConfig(target_schema=target.schema_, quoting=quoting),
             scope,
         )
 
     def _load_models(
         self, models_dirs: t.List[Path]
     ) -> t.Tuple[t.Dict[str, ModelConfig], t.Dict[str, SourceConfig]]:
         """
@@ -304,15 +307,15 @@
             source_config = self._config_for_scope((*scope, source_name), scoped_configs)
 
             source_config.schema_ = source_name
             config_fields = source.get("config")
             if config_fields:
                 source_config = source_config.update_with(config_fields)
 
-            for table in source["tables"]:
+            for table in source.get("tables", []):
                 table_name = table["name"]
                 table_config = source_config.copy()
 
                 table_config.identifier = table_name
                 config_fields = source.get("config")
                 if config_fields:
                     table_config = table_config.update_with(config_fields)
@@ -356,7 +359,11 @@
         scope = (self._package_name, *path_from_root.parts[:-1])
         if path.match("*.sql") or path.match("*.csv"):
             scope = (*scope, path_from_root.stem)
         return scope
 
     def _config_for_scope(self, scope: Scope, configs: t.Dict[Scope, C]) -> C:
         return configs.get(scope) or self._config_for_scope(scope[0:-1], configs)
+
+    @classmethod
+    def _create_empty_target(cls) -> TargetConfig:
+        return TargetConfig(name="", database="", schema="", profile_name="")
```

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/dbt/profile.py` & `sqlmesh-0.5.1.dev28/sqlmesh/dbt/profile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import os
 import typing as t
 from pathlib import Path
 
 from sqlmesh.dbt.common import PROJECT_FILENAME, load_yaml
 from sqlmesh.dbt.context import DbtContext
 from sqlmesh.dbt.target import TargetConfig
 from sqlmesh.utils.errors import ConfigError
@@ -61,18 +62,20 @@
             raise ConfigError(f"{cls.PROFILE_FILE} not found.")
 
         target_name, target = cls._read_profile(profile_filepath, context, target_name)
         return Profile(profile_filepath, target_name, target)
 
     @classmethod
     def _find_profile(cls, project_root: Path) -> t.Optional[Path]:
-        # TODO Check environment variable
-        path = Path(project_root, cls.PROFILE_FILE)
+        dir = os.environ.get("DBT_PROFILES_DIR", "")
+        path = Path(project_root, dir, cls.PROFILE_FILE)
         if path.exists():
             return path
+        elif dir:
+            return None
 
         path = Path(Path.home(), ".dbt", cls.PROFILE_FILE)
         if path.exists():
             return path
 
         return None
 
@@ -95,10 +98,12 @@
 
         if target_name not in outputs:
             raise ConfigError(
                 f"Target '{target_name}' not specified in profiles for '{context.profile_name}'."
             )
 
         target_fields = load_yaml(context.render(dump_yaml(outputs[target_name])))
-        target = TargetConfig.load(target_name, target_fields)
+        target = TargetConfig.load(
+            {"name": target_name, "profile_name": context.profile_name, **target_fields}
+        )
 
         return (target_name, target)
```

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/dbt/project.py` & `sqlmesh-0.5.1.dev28/sqlmesh/dbt/project.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/dbt/source.py` & `sqlmesh-0.5.1.dev28/sqlmesh/dbt/source.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/dbt/target.py` & `sqlmesh-0.5.1.dev28/sqlmesh/dbt/target.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,65 +31,66 @@
 
 
 class TargetConfig(abc.ABC, DbtConfig):
     """
     Configuration for DBT profile target
 
     Args:
-        name: The name of this target
         type: The type of the data warehouse
-        schema_: The target schema for this project
+        name: The name of this target
+        database: Name of the database
+        schema_: Name of the schema
         threads: The number of threads to run on
     """
 
     # dbt
-    type: str = ""
-    name: str = ""
-    schema_: str = Field(default="", alias="schema")
+    type: str = "none"
+    name: str
+    database: str
+    schema_: str = Field(alias="schema")
     threads: int = 1
     profile_name: t.Optional[str] = None
 
     @classmethod
-    def load(cls, name: str, data: t.Dict[str, t.Any]) -> TargetConfig:
+    def load(cls, data: t.Dict[str, t.Any]) -> TargetConfig:
         """
         Loads the configuration from the yaml provided for a profile target
 
         Args:
             data: The yaml for the project's target output
 
         Returns:
             The configuration of the provided profile target
         """
         db_type = data["type"]
         if db_type == "databricks":
-            return DatabricksConfig(name=name, **data)
+            return DatabricksConfig(**data)
         elif db_type == "duckdb":
-            return DuckDbConfig(name=name, **data)
+            return DuckDbConfig(**data)
         elif db_type == "postgres":
-            return PostgresConfig(name=name, **data)
+            return PostgresConfig(**data)
         elif db_type == "redshift":
-            return RedshiftConfig(name=name, **data)
+            return RedshiftConfig(**data)
         elif db_type == "snowflake":
-            return SnowflakeConfig(name=name, **data)
+            return SnowflakeConfig(**data)
         elif db_type == "bigquery":
-            return BigQueryConfig(name=name, **data)
+            return BigQueryConfig(**data)
 
         raise ConfigError(f"{db_type} not supported.")
 
     def default_incremental_strategy(self, kind: IncrementalKind) -> str:
         """The default incremental strategy for the db"""
         raise NotImplementedError
 
     def to_sqlmesh(self) -> ConnectionConfig:
         """Converts target config to SQLMesh connection config"""
         raise NotImplementedError
 
-    def target_jinja(self, profile_name: str) -> AttributeDict:
+    def attribute_dict(self) -> AttributeDict:
         fields = self.dict().copy()
-        fields["profile_name"] = profile_name
         fields["target_name"] = self.name
         return AttributeDict(fields)
 
     @property
     def quoting(self) -> QuotingConfig:
         return QuotingConfig()
 
@@ -103,15 +104,17 @@
     Connection config for DuckDb target
 
     Args:
         path: Location of the database file. If not specified, an in memory database is used.
     """
 
     type: Literal["duckdb"] = "duckdb"
-    path: t.Optional[str] = None
+    database: str = "main"
+    schema_: str = Field(default="main", alias="schema")
+    path: str = ":memory:"
 
     def default_incremental_strategy(self, kind: IncrementalKind) -> str:
         return "delete+insert"
 
     def to_sqlmesh(self) -> ConnectionConfig:
         return DuckDBConnectionConfig(database=self.path, concurrent_tasks=self.threads)
 
@@ -119,15 +122,14 @@
 class SnowflakeConfig(TargetConfig):
     """
     Project connection and operational configuration for the Snowflake target
 
     Args:
         account: Snowflake account
         warehouse: Name of the warehouse
-        database: Name of the database
         user: Name of the user
         password: User's password
         role: Role of the user
         client_session_keep_alive: A boolean flag to extend the duration of the Snowflake session beyond 4 hours
         query_tag: tag for the query in Snowflake
         connect_retries: Number of times to retry if the Snowflake connector encounters an error
         connect_timeout: Number of seconds to wait between failed attempts
@@ -135,15 +137,14 @@
         retry_all: A boolean flag to retry on all Snowflake connector errors
     """
 
     # TODO add other forms of authentication
     type: Literal["snowflake"] = "snowflake"
     account: str
     warehouse: str
-    database: str
     user: str
     password: str
     role: t.Optional[str]
     client_session_keep_alive: bool = False
     query_tag: t.Optional[str]
     connect_retries: int = 0
     connect_timeout: int = 10
@@ -196,14 +197,23 @@
     keepalives_idle: int = 0
     connect_timeout: int = 10
     retries: int = 1  # Currently Unsupported by SQLMesh
     search_path: t.Optional[str] = None  # Currently Unsupported by SQLMesh
     role: t.Optional[str] = None
     sslmode: t.Optional[str] = None
 
+    @root_validator(pre=True)
+    def validate_database(
+        cls, values: t.Dict[str, t.Union[t.Tuple[str, ...], t.Optional[str], t.Dict[str, t.Any]]]
+    ) -> t.Dict[str, t.Union[t.Tuple[str, ...], t.Optional[str], t.Dict[str, t.Any]]]:
+        values["database"] = values.get("database") or values.get("dbname")
+        if not values["database"]:
+            raise ConfigError("Either database or dbname must be set")
+        return values
+
     def default_incremental_strategy(self, kind: IncrementalKind) -> str:
         return "delete+insert" if kind is IncrementalByUniqueKeyKind else "append"
 
     def to_sqlmesh(self) -> ConnectionConfig:
         return PostgresConnectionConfig(
             host=self.host,
             user=self.user,
@@ -244,21 +254,31 @@
     dbname: str
     keepalives_idle: int = 240
     connect_timeout: int = 10
     ra3_node: bool = True
     search_path: t.Optional[str] = None
     sslmode: t.Optional[str] = None
 
+    @root_validator(pre=True)
+    def validate_database(
+        cls, values: t.Dict[str, t.Union[t.Tuple[str, ...], t.Optional[str], t.Dict[str, t.Any]]]
+    ) -> t.Dict[str, t.Union[t.Tuple[str, ...], t.Optional[str], t.Dict[str, t.Any]]]:
+        values["database"] = values.get("database") or values.get("dbname")
+        if not values["database"]:
+            raise ConfigError("Either database or dbname must be set")
+        return values
+
     def default_incremental_strategy(self, kind: IncrementalKind) -> str:
         return "append"
 
     def to_sqlmesh(self) -> ConnectionConfig:
         return RedshiftConnectionConfig(
             user=self.user,
             password=self.password,
+            database=self.database,
             host=self.host,
             port=self.port,
             sslmode=self.sslmode,
             timeout=self.connect_timeout,
             concurrent_tasks=self.threads,
         )
 
@@ -268,21 +288,23 @@
     Project connection and operational configuration for the Databricks target
 
     Args:
         catalog: Catalog name to use for Unity Catalog
         host: The Databricks host to connect to
         http_path: The Databricks compute resources URL
         token: Personal access token
+        database: Name of the database. Not applicable for Databricks and ignored
     """
 
     type: Literal["databricks"] = "databricks"
     catalog: t.Optional[str] = None
     host: str
     http_path: str
     token: str
+    database: t.Optional[str] = None  # type: ignore
 
     def default_incremental_strategy(self, kind: IncrementalKind) -> str:
         return "merge"
 
     def to_sqlmesh(self) -> ConnectionConfig:
         return DatabricksSQLConnectionConfig(
             server_hostname=self.host,
@@ -293,15 +315,14 @@
 
 
 class BigQueryConfig(TargetConfig):
     """
     Project connection and operational configuration for the BigQuery target
 
     Args:
-        schema_: Overrides
         type: The type of the target (bigquery)
         method: The BigQuery authentication method to use
         project: The BigQuery project to connect to
         location: The BigQuery location to connect to
         keyfile: The path to the BigQuery keyfile
         keyfile_json: The BigQuery keyfile as a JSON string
         token: The BigQuery token
@@ -310,15 +331,14 @@
         client_secret: The BigQuery client secret
         token_uri: The BigQuery token URI
         scopes: The BigQuery scopes
     """
 
     type: Literal["bigquery"] = "bigquery"
     method: t.Optional[str] = BigQueryConnectionMethod.OAUTH
-    schema_: t.Optional[str] = Field(None, alias="schema")  # type: ignore
     dataset: t.Optional[str] = None
     project: t.Optional[str] = None
     location: t.Optional[str] = None
     keyfile: t.Optional[str] = None
     keyfile_json: t.Optional[t.Dict[str, t.Any]] = None
     token: t.Optional[str] = None
     refresh_token: t.Optional[str] = None
@@ -332,30 +352,33 @@
     )
     job_execution_timeout_seconds: t.Optional[int] = None
     job_retries: int = 1
     job_retry_deadline_seconds: t.Optional[int] = None
     priority: BigQueryPriority = BigQueryPriority.INTERACTIVE
     maximum_bytes_billed: t.Optional[int] = None
 
-    @root_validator
-    def validate_schema(
+    @root_validator(pre=True)
+    def validate_fields(
         cls, values: t.Dict[str, t.Union[t.Tuple[str, ...], t.Optional[str], t.Dict[str, t.Any]]]
     ) -> t.Dict[str, t.Union[t.Tuple[str, ...], t.Optional[str], t.Dict[str, t.Any]]]:
-        values["schema_"] = values.get("schema_") or values.get("dataset")
-        if not values["schema_"]:
+        values["schema"] = values.get("schema") or values.get("dataset")
+        if not values["schema"]:
             raise ConfigError("Either schema or dataset must be set")
+        values["database"] = values.get("database") or values.get("project")
+        if not values["database"]:
+            raise ConfigError("Either database or project must be set")
         return values
 
     def default_incremental_strategy(self, kind: IncrementalKind) -> str:
         return "merge"
 
     def to_sqlmesh(self) -> ConnectionConfig:
         return BigQueryConnectionConfig(
             method=self.method,
-            project=self.project,
+            project=self.database,
             location=self.location,
             concurrent_tasks=self.threads,
             keyfile=self.keyfile,
             keyfile_json=self.keyfile_json,
             token=self.token,
             refresh_token=self.refresh_token,
             client_id=self.client_id,
```

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/engines/commands.py` & `sqlmesh-0.5.1.dev28/sqlmesh/engines/commands.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/engines/spark/app.py` & `sqlmesh-0.5.1.dev28/sqlmesh/engines/spark/app.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/engines/spark/db_api/spark_session.py` & `sqlmesh-0.5.1.dev28/sqlmesh/engines/spark/db_api/spark_session.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/integrations/github/notification_operator_provider.py` & `sqlmesh-0.5.1.dev28/sqlmesh/integrations/github/notification_operator_provider.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/integrations/github/notification_target.py` & `sqlmesh-0.5.1.dev28/sqlmesh/integrations/github/notification_target.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/integrations/github/shared.py` & `sqlmesh-0.5.1.dev28/sqlmesh/integrations/github/shared.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/magics.py` & `sqlmesh-0.5.1.dev28/sqlmesh/magics.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/migrations/v0001_init.py` & `sqlmesh-0.5.1.dev28/sqlmesh/migrations/v0001_init.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/migrations/v0003_move_batch_size.py` & `sqlmesh-0.5.1.dev28/sqlmesh/migrations/v0003_move_batch_size.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/api.py` & `sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/client.py` & `sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/client.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/common.py` & `sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/common.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/dag_generator.py` & `sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/dag_generator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/hooks/bigquery.py` & `sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/hooks/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/hooks/redshift.py` & `sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/hooks/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/integration.py` & `sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/operators/bigquery.py` & `sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/operators/bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/operators/databricks.py` & `sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/operators/databricks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/operators/hwm_sensor.py` & `sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/operators/hwm_sensor.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/operators/notification.py` & `sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/operators/notification.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/operators/postgres.py` & `sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/operators/postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/operators/redshift.py` & `sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/operators/redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/operators/snowflake.py` & `sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/operators/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/operators/spark_submit.py` & `sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/operators/spark_submit.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/operators/targets.py` & `sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/operators/targets.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,18 @@
             start=self._get_start(context),
             end=self._get_end(context),
             latest=self._get_latest(context),
             is_dev=self.is_dev,
         )
 
     def _get_start(self, context: Context) -> TimeLike:
-        return self.start or context["dag_run"].data_interval_start
+        return (
+            self.start
+            or context["dag_run"].data_interval_start - self.snapshot.model.lookback_delta
+        )
 
     def _get_end(self, context: Context) -> TimeLike:
         return self.end or context["dag_run"].data_interval_end
 
     def _get_latest(self, context: Context) -> TimeLike:
         return self.latest or context["dag_run"].logical_date
```

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/plan.py` & `sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/plugin.py` & `sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/plugin.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/state_sync.py` & `sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/state_sync.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/schedulers/airflow/util.py` & `sqlmesh-0.5.1.dev28/sqlmesh/schedulers/airflow/util.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/utils/__init__.py` & `sqlmesh-0.5.1.dev28/sqlmesh/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/utils/cache.py` & `sqlmesh-0.5.1.dev28/sqlmesh/utils/cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/utils/concurrency.py` & `sqlmesh-0.5.1.dev28/sqlmesh/utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/utils/connection_pool.py` & `sqlmesh-0.5.1.dev28/sqlmesh/utils/connection_pool.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/utils/dag.py` & `sqlmesh-0.5.1.dev28/sqlmesh/utils/dag.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/utils/date.py` & `sqlmesh-0.5.1.dev28/sqlmesh/utils/date.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/utils/errors.py` & `sqlmesh-0.5.1.dev28/sqlmesh/utils/errors.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/utils/jinja.py` & `sqlmesh-0.5.1.dev28/sqlmesh/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/utils/metaprogramming.py` & `sqlmesh-0.5.1.dev28/sqlmesh/utils/metaprogramming.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/utils/pandas.py` & `sqlmesh-0.5.1.dev28/sqlmesh/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/utils/pydantic.py` & `sqlmesh-0.5.1.dev28/sqlmesh/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/utils/rich.py` & `sqlmesh-0.5.1.dev28/sqlmesh/utils/rich.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/utils/transactional_file.py` & `sqlmesh-0.5.1.dev28/sqlmesh/utils/transactional_file.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh/utils/yaml.py` & `sqlmesh-0.5.1.dev28/sqlmesh/utils/yaml.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,28 +13,33 @@
 
 JINJA_METHODS = {
     "env_var": lambda key, default=None: getenv(key, default),
 }
 
 
 def load(
-    source: str | Path, raise_if_empty: bool = True, render_jinja: bool = True
+    source: str | Path,
+    raise_if_empty: bool = True,
+    render_jinja: bool = True,
+    allow_duplicate_keys: bool = False,
 ) -> t.OrderedDict:
     """Loads a YAML object from either a raw string or a file."""
     path: t.Optional[Path] = None
 
     if isinstance(source, Path):
         path = source
         with open(source, "r", encoding="utf-8") as file:
             source = file.read()
 
     if render_jinja:
         source = ENVIRONMENT.from_string(source).render(JINJA_METHODS)
 
-    contents = YAML().load(source)
+    yaml = YAML()
+    yaml.allow_duplicate_keys = allow_duplicate_keys
+    contents = yaml.load(source)
     if contents is None:
         if raise_if_empty:
             error_path = f" '{path}'" if path else ""
             raise SQLMeshError(f"YAML source{error_path} can't be empty.")
         return OrderedDict()
 
     return contents
```

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh.egg-info/PKG-INFO` & `sqlmesh-0.5.1.dev28/sqlmesh.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,15 @@
 Metadata-Version: 2.1
 Name: sqlmesh
-Version: 0.5.1.dev22
+Version: 0.5.1.dev28
 Summary: UNKNOWN
 Home-page: https://github.com/TobikoData/sqlmesh
 Author: TobikoData Inc.
 Author-email: engineering@tobikodata.com
 License: Apache License 2.0
-Description: ![SQLMesh logo](sqlmesh.svg)
-        
-        SQLMesh is a DataOps framework that brings the benefits of DevOps to data teams. It enables data scientists, analysts, and engineers to efficiently run and deploy data transformations written in SQL or Python.
-        
-        For more information, check out the [website](https://sqlmesh.com) and [documentation](https://sqlmesh.readthedocs.io/en/stable/).
-        
-        ## Geting Started
-        Install SQLMesh through [pypi](https://pypi.org/project/sqlmesh/) by running:
-        
-        ```pip install sqlmesh```
-        
-        Follow the [tutorial](https://sqlmesh.readthedocs.io/en/stable/quick_start/) to learn how to use SQLMesh.
-        
-        ## Join our community
-        We'd love to join you on your data journey. Connect with us in the following ways:
-        
-        * Join the [Tobiko Slack community](https://join.slack.com/t/tobiko-data/shared_invite/zt-1ma66d79v-a4dbf4DUpLAQJ8ptQrJygg) to ask questions, or just to say hi!
-        * File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
-        * Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
-        
-        ## Contribution
-        Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
-        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -41,7 +18,33 @@
 Provides-Extra: databricks
 Provides-Extra: dev
 Provides-Extra: dbt
 Provides-Extra: postgres
 Provides-Extra: redshift
 Provides-Extra: snowflake
 Provides-Extra: web
+License-File: LICENSE
+
+![SQLMesh logo](sqlmesh.svg)
+
+SQLMesh is a DataOps framework that brings the benefits of DevOps to data teams. It enables data scientists, analysts, and engineers to efficiently run and deploy data transformations written in SQL or Python.
+
+For more information, check out the [website](https://sqlmesh.com) and [documentation](https://sqlmesh.readthedocs.io/en/stable/).
+
+## Geting Started
+Install SQLMesh through [pypi](https://pypi.org/project/sqlmesh/) by running:
+
+```pip install sqlmesh```
+
+Follow the [tutorial](https://sqlmesh.readthedocs.io/en/stable/quick_start/) to learn how to use SQLMesh.
+
+## Join our community
+We'd love to join you on your data journey. Connect with us in the following ways:
+
+* Join the [Tobiko Slack community](https://join.slack.com/t/tobiko-data/shared_invite/zt-1ma66d79v-a4dbf4DUpLAQJ8ptQrJygg) to ask questions, or just to say hi!
+* File an issue on our [GitHub](https://github.com/TobikoData/sqlmesh/issues/new).
+* Send us an email at [hello@tobikodata.com](hello@tobikodata.com) with your questions or feedback.
+
+## Contribution
+Contributions in the form of issues or pull requests are greatly appreciated. [Read more](https://sqlmesh.readthedocs.io/en/stable/development/) about how to develop for SQLMesh.
+
+
```

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh.egg-info/SOURCES.txt` & `sqlmesh-0.5.1.dev28/sqlmesh.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -271,14 +271,15 @@
 sqlmesh/integrations/github/notification_operator_provider.py
 sqlmesh/integrations/github/notification_target.py
 sqlmesh/integrations/github/shared.py
 sqlmesh/migrations/__init__.py
 sqlmesh/migrations/v0001_init.py
 sqlmesh/migrations/v0002_remove_identify.py
 sqlmesh/migrations/v0003_move_batch_size.py
+sqlmesh/migrations/v0004_environmnent_add_finalized_at.py
 sqlmesh/schedulers/__init__.py
 sqlmesh/schedulers/airflow/__init__.py
 sqlmesh/schedulers/airflow/api.py
 sqlmesh/schedulers/airflow/client.py
 sqlmesh/schedulers/airflow/common.py
 sqlmesh/schedulers/airflow/dag_generator.py
 sqlmesh/schedulers/airflow/integration.py
```

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh.egg-info/requires.txt` & `sqlmesh-0.5.1.dev28/sqlmesh.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 hyperscript
 jinja2
 pandas
 pydantic<2.0.0,>=1.9.1
 requests
 rich
 ruamel.yaml
-sqlglot~=11.5.6
+sqlglot~=11.5.7
 fsspec
 
 [bigquery]
 google-cloud-bigquery[pandas]
 google-cloud-bigquery-storage
 
 [databricks]
```

### Comparing `sqlmesh-0.5.1.dev22/sqlmesh.svg` & `sqlmesh-0.5.1.dev28/sqlmesh.svg`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/conftest.py` & `sqlmesh-0.5.1.dev28/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/engine_adapter/test_base.py` & `sqlmesh-0.5.1.dev28/tests/core/engine_adapter/test_base.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/engine_adapter/test_base_postgres.py` & `sqlmesh-0.5.1.dev28/tests/core/engine_adapter/test_base_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/engine_adapter/test_base_spark.py` & `sqlmesh-0.5.1.dev28/tests/core/engine_adapter/test_base_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/engine_adapter/test_bigquery.py` & `sqlmesh-0.5.1.dev28/tests/core/engine_adapter/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/engine_adapter/test_databricks.py` & `sqlmesh-0.5.1.dev28/tests/core/engine_adapter/test_databricks.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/engine_adapter/test_duckdb.py` & `sqlmesh-0.5.1.dev28/tests/core/engine_adapter/test_duckdb.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/engine_adapter/test_postgres.py` & `sqlmesh-0.5.1.dev28/tests/core/engine_adapter/test_postgres.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/engine_adapter/test_redshift.py` & `sqlmesh-0.5.1.dev28/tests/core/engine_adapter/test_redshift.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/engine_adapter/test_spark.py` & `sqlmesh-0.5.1.dev28/tests/core/engine_adapter/test_spark.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/test_audit.py` & `sqlmesh-0.5.1.dev28/tests/core/test_audit.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/test_config.py` & `sqlmesh-0.5.1.dev28/tests/core/test_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/test_connection_config.py` & `sqlmesh-0.5.1.dev28/tests/core/test_connection_config.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/test_context.py` & `sqlmesh-0.5.1.dev28/tests/core/test_context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/test_dialect.py` & `sqlmesh-0.5.1.dev28/tests/core/test_dialect.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/test_integration.py` & `sqlmesh-0.5.1.dev28/tests/core/test_integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/test_macros.py` & `sqlmesh-0.5.1.dev28/tests/core/test_macros.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/test_model.py` & `sqlmesh-0.5.1.dev28/tests/core/test_model.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/test_plan.py` & `sqlmesh-0.5.1.dev28/tests/core/test_plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/test_plan_evaluator.py` & `sqlmesh-0.5.1.dev28/tests/core/test_plan_evaluator.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/test_scheduler.py` & `sqlmesh-0.5.1.dev28/tests/core/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/test_schema_diff.py` & `sqlmesh-0.5.1.dev28/tests/core/test_schema_diff.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/test_seed.py` & `sqlmesh-0.5.1.dev28/tests/core/test_seed.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/test_snapshot.py` & `sqlmesh-0.5.1.dev28/tests/core/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/core/test_snapshot_evaluator.py` & `sqlmesh-0.5.1.dev28/tests/core/test_snapshot_evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     ModelKindName,
     SqlModel,
     load_model,
 )
 from sqlmesh.core.model.meta import IntervalUnit
 from sqlmesh.core.snapshot import (
     Snapshot,
+    SnapshotChangeCategory,
     SnapshotEvaluator,
     SnapshotFingerprint,
     SnapshotTableInfo,
 )
 from sqlmesh.utils.errors import ConfigError, SQLMeshError
 
 
@@ -231,14 +232,15 @@
     model = SqlModel(
         name="test_schema.test_model",
         kind=IncrementalByTimeRangeKind(time_column="a"),
         storage_format="parquet",
         query=parse_one("SELECT c, a FROM tbl WHERE ds BETWEEN @start_ds and @end_ds"),
     )
     snapshot = make_snapshot(model, physical_schema="physical_schema", version="1")
+    snapshot.change_category = SnapshotChangeCategory.FORWARD_ONLY
 
     evaluator.migrate([snapshot])
 
     cursor_mock.execute.assert_has_calls(
         [
             call("""ALTER TABLE physical_schema.test_schema__test_model__1 DROP COLUMN b"""),
             call("""ALTER TABLE physical_schema.test_schema__test_model__1 ADD COLUMN a INT"""),
```

### Comparing `sqlmesh-0.5.1.dev22/tests/core/test_state_sync.py` & `sqlmesh-0.5.1.dev28/tests/core/test_state_sync.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/dbt/conftest.py` & `sqlmesh-0.5.1.dev28/tests/dbt/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/dbt/test_adapter.py` & `sqlmesh-0.5.1.dev28/tests/dbt/test_adapter.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/dbt/test_config.py` & `sqlmesh-0.5.1.dev28/tests/dbt/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 import pytest
 from dbt.adapters.base import BaseRelation
 
 from sqlmesh.core.model import SqlModel
 from sqlmesh.dbt.context import DbtContext
-from sqlmesh.dbt.model import Materialization, ModelConfig
+from sqlmesh.dbt.model import IncrementalByUniqueKeyKind, Materialization, ModelConfig
 from sqlmesh.dbt.project import Project
 from sqlmesh.dbt.source import SourceConfig
 from sqlmesh.dbt.target import (
     BigQueryConfig,
     DatabricksConfig,
     DuckDbConfig,
     PostgresConfig,
@@ -100,37 +100,43 @@
 
 def test_to_sqlmesh_fields(sushi_test_project: Project):
     model_config = ModelConfig(
         alias="model",
         target_schema="schema",
         schema_="custom",
         database="database",
-        materialized=Materialization.TABLE,
+        materialized=Materialization.INCREMENTAL,
         description="test model",
         sql="SELECT 1 AS a FROM foo",
         start="Jan 1 2023",
         partitioned_by=["a"],
         cron="@hourly",
+        batch_size=5,
+        lookback=3,
+        unique_key=["a"],
         meta={"stamp": "bar", "dialect": "duckdb"},
         owner="Sally",
     )
     context = DbtContext(project_name="Foo")
-    context.target = DuckDbConfig(schema="foo")
+    context.target = DuckDbConfig(name="target", schema="foo")
     model = model_config.to_sqlmesh(context)
 
     assert isinstance(model, SqlModel)
     assert model.name == "database.schema_custom.model"
     assert model.description == "test model"
     assert model.query.sql() == "SELECT 1 AS a FROM foo"
     assert model.start == "Jan 1 2023"
     assert model.partitioned_by == ["a"]
     assert model.cron == "@hourly"
     assert model.stamp == "bar"
     assert model.dialect == "duckdb"
     assert model.owner == "Sally"
+    kind = t.cast(IncrementalByUniqueKeyKind, model.kind)
+    assert kind.batch_size == 5
+    assert kind.lookback == 3
 
 
 def test_model_config_sql_no_config():
     context = DbtContext()
     assert (
         ModelConfig(
             sql="""{{
@@ -269,20 +275,20 @@
     source = SourceConfig(identifier="bar", schema="foo")
     assert str(BaseRelation.create(**source.relation_info)) == '"foo"."bar"'
 
     source.quoting.schema_ = False
     assert str(BaseRelation.create(**source.relation_info)) == 'foo."bar"'
 
 
-def _test_warehouse_config(config_yaml: str, config_model: t.Type[TargetConfig], *params_path: str):
+def _test_warehouse_config(config_yaml: str, target_class: t.Type[TargetConfig], *params_path: str):
     config_dict = yaml_load(config_yaml)
     for path in params_path:
         config_dict = config_dict[path]
 
-    config = config_model(**config_dict)
+    config = target_class(**{"name": "dev", **config_dict})
 
     for key, value in config.dict().items():
         input_value = config_dict.get(key)
         if input_value is not None:
             assert input_value == value
```

### Comparing `sqlmesh-0.5.1.dev22/tests/dbt/test_transformation.py` & `sqlmesh-0.5.1.dev28/tests/dbt/test_transformation.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     assert (
         ModelConfig(target_schema="foo", path="models/bar.sql", schema_="baz").model_name
         == "foo_baz.bar"
     )
 
 
 def test_model_kind():
-    target = DuckDbConfig(schema="foo")
+    target = DuckDbConfig(name="target", schema="foo")
 
     assert ModelConfig(materialized=Materialization.TABLE).model_kind(target) == ModelKind(
         name=ModelKindName.FULL
     )
     assert ModelConfig(materialized=Materialization.VIEW).model_kind(target) == ModelKind(
         name=ModelKindName.VIEW
     )
@@ -135,15 +135,15 @@
         "zipcode": "Business zipcode",
     }
 
     assert column_types_to_sqlmesh(model.columns) == expected_column_types
     assert column_descriptions_to_sqlmesh(model.columns) == expected_column_descriptions
 
     context = DbtContext(project_name="Foo")
-    context.target = DuckDbConfig(schema="foo")
+    context.target = DuckDbConfig(name="target", schema="foo")
     sqlmesh_model = model.to_sqlmesh(context)
     assert sqlmesh_model.columns_to_types == expected_column_types
     assert sqlmesh_model.column_descriptions == expected_column_descriptions
 
 
 def test_seed_columns():
     seed = SeedConfig(
@@ -192,15 +192,15 @@
                 data_type="varchar({{ var('size') }})",
                 description="Business zipcode",
             ),
         },
     )
 
     context = DbtContext(project_name="Foo")
-    context.target = DuckDbConfig(schema="foo")
+    context.target = DuckDbConfig(name="target", schema="foo")
     context.variables = {"schema": "foo", "size": "5"}
     model._dependencies.sources = set(["package.table"])
     context.sources = {"package.table": SourceConfig(schema_="raw", name="baz")}
 
     rendered = model.render_config(context)
     assert rendered.pre_hook == model.pre_hook
     assert rendered.sql == model.sql
@@ -212,15 +212,16 @@
     sqlmesh_model = rendered.to_sqlmesh(context)
     assert str(sqlmesh_model.query) == model.sql
     assert str(sqlmesh_model.render_query()) == 'SELECT * FROM "raw"."baz" AS baz'
     assert sqlmesh_model.columns_to_types == column_types_to_sqlmesh(rendered.columns)
 
 
 def test_config_containing_missing_dependency():
-    context = DbtContext()
+    context = DbtContext(project_name="project")
+    context.target = DuckDbConfig(name="target", schema="foo")
     model = ModelConfig(sql="{{ config(pre_hook=\"{{ print(ref('bar')) }}\") }} SELECT 1 FROM a")
     with pytest.raises(ConfigError, match="'bar' was not found"):
         model.render_config(context).to_sqlmesh(context)
 
     model = ModelConfig(sql='{{ config(pre_hook="{{ get_table_name() }}") }} SELECT 1 FROM a')
     with pytest.raises(ConfigError, match="get_table_name"):
         model.render_config(context).to_sqlmesh(context)
```

### Comparing `sqlmesh-0.5.1.dev22/tests/engines/spark/test_db_api.py` & `sqlmesh-0.5.1.dev28/tests/engines/spark/test_db_api.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/dbt_project.yml` & `sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy` & `sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/logs/dbt.log.legacy`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/macros/incremental.sql` & `sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql` & `sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/models/waiter_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml` & `sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages/customers/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql` & `sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/packages/customers/models/customer_revenue_by_day.sql`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/profiles.yml` & `sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/profiles.yml`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/seed_sources.py` & `sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/seed_sources.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/source_data/items.csv` & `sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/source_data/items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/source_data/order_items.csv` & `sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/source_data/order_items.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/fixtures/dbt/sushi_test/source_data/orders.csv` & `sqlmesh-0.5.1.dev28/tests/fixtures/dbt/sushi_test/source_data/orders.csv`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/fixtures/migrations/environments.json` & `sqlmesh-0.5.1.dev28/tests/fixtures/migrations/environments.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/fixtures/migrations/snapshots.json` & `sqlmesh-0.5.1.dev28/tests/fixtures/migrations/snapshots.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/integrations/github/fixtures/pull_request_review.json` & `sqlmesh-0.5.1.dev28/tests/integrations/github/fixtures/pull_request_review.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/schedulers/airflow/conftest.py` & `sqlmesh-0.5.1.dev28/tests/schedulers/airflow/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/schedulers/airflow/operators/test_hwm_sensor.py` & `sqlmesh-0.5.1.dev28/tests/schedulers/airflow/operators/test_hwm_sensor.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/schedulers/airflow/operators/test_targets.py` & `sqlmesh-0.5.1.dev28/tests/schedulers/airflow/operators/test_targets.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/schedulers/airflow/test_client.py` & `sqlmesh-0.5.1.dev28/tests/schedulers/airflow/test_client.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/schedulers/airflow/test_end_to_end.py` & `sqlmesh-0.5.1.dev28/tests/schedulers/airflow/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/schedulers/airflow/test_integration.py` & `sqlmesh-0.5.1.dev28/tests/schedulers/airflow/test_integration.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/schedulers/airflow/test_plan.py` & `sqlmesh-0.5.1.dev28/tests/schedulers/airflow/test_plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/utils/test_cache.py` & `sqlmesh-0.5.1.dev28/tests/utils/test_cache.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/utils/test_concurrency.py` & `sqlmesh-0.5.1.dev28/tests/utils/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/utils/test_connection_pool.py` & `sqlmesh-0.5.1.dev28/tests/utils/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/utils/test_dag.py` & `sqlmesh-0.5.1.dev28/tests/utils/test_dag.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/utils/test_date.py` & `sqlmesh-0.5.1.dev28/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/utils/test_filesystem.py` & `sqlmesh-0.5.1.dev28/tests/utils/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/utils/test_jinja.py` & `sqlmesh-0.5.1.dev28/tests/utils/test_jinja.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/utils/test_metaprogramming.py` & `sqlmesh-0.5.1.dev28/tests/utils/test_metaprogramming.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/utils/test_pandas.py` & `sqlmesh-0.5.1.dev28/tests/utils/test_pandas.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/utils/test_pydantic.py` & `sqlmesh-0.5.1.dev28/tests/utils/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/utils/test_transactional_file.py` & `sqlmesh-0.5.1.dev28/tests/utils/test_transactional_file.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/utils/test_yaml.py` & `sqlmesh-0.5.1.dev28/tests/utils/test_yaml.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/tests/web/test_main.py` & `sqlmesh-0.5.1.dev28/tests/web/test_main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/.eslintrc.js` & `sqlmesh-0.5.1.dev28/web/client/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/index.html` & `sqlmesh-0.5.1.dev28/web/client/index.html`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/openapi.json` & `sqlmesh-0.5.1.dev28/web/client/openapi.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/package-lock.json` & `sqlmesh-0.5.1.dev28/web/client/package-lock.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/package.json` & `sqlmesh-0.5.1.dev28/web/client/package.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/playwright.config.ts` & `sqlmesh-0.5.1.dev28/web/client/playwright.config.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/public/favicons/favicon.ico` & `sqlmesh-0.5.1.dev28/web/client/public/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/api/channels.ts` & `sqlmesh-0.5.1.dev28/web/client/src/api/channels.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/api/index.ts` & `sqlmesh-0.5.1.dev28/web/client/src/api/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/api/instance.ts` & `sqlmesh-0.5.1.dev28/web/client/src/api/instance.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Circular STD/CircularStd-Black.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Circular STD/CircularStd-BlackItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Circular STD/CircularStd-Bold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Circular STD/CircularStd-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Circular STD/CircularStd-Book.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Circular STD/CircularStd-BookItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Circular STD/CircularStd-Medium.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Circular STD/CircularStd-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-Black.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-Black.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-BlackItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-Bold.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-Bold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-Extrabold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-ExtraboldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-Italic.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-Italic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-Light.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-Light.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-LightItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-Medium.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-Medium.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-MediumItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/Publico-Roman.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/Publico-Roman.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/PublicoText-Bold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/PublicoText-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/PublicoText-Italic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/PublicoText-Roman.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/PublicoText-Semibold.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf` & `sqlmesh-0.5.1.dev28/web/client/src/assets/fonts/Publico/PublicoText-SemiboldItalic.otf`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/context/context.ts` & `sqlmesh-0.5.1.dev28/web/client/src/context/context.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/context/editor.ts` & `sqlmesh-0.5.1.dev28/web/client/src/context/editor.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/context/fileTree.ts` & `sqlmesh-0.5.1.dev28/web/client/src/context/fileTree.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/context/lineage.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/context/lineage.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/context/plan.ts` & `sqlmesh-0.5.1.dev28/web/client/src/context/plan.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/context/theme.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/context/theme.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/hooks/useLocalStorage.ts` & `sqlmesh-0.5.1.dev28/web/client/src/hooks/useLocalStorage.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/index.css` & `sqlmesh-0.5.1.dev28/web/client/src/index.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/banner/Banner.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/banner/Banner.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/button/Button.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/button/Button.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/button/tests/Button.spec.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/button/tests/Button.spec.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/divider/Divider.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/divider/Divider.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/divider/tests/Divider.spec.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/divider/tests/Divider.spec.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/Editor.css` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/Editor.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/Editor.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/Editor.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/EditorCode.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/EditorCode.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/EditorFooter.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/EditorFooter.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/EditorIndicator.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/EditorIndicator.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/EditorInspector.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/EditorInspector.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/EditorPreview.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/EditorPreview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/EditorTabs.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/EditorTabs.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/extensions/SqlMeshDialect.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/extensions/index.ts` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/extensions/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/editor/help.ts` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/editor/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/fileTree/Directory.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/fileTree/Directory.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/fileTree/File.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/fileTree/File.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/fileTree/FileTree.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/fileTree/FileTree.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/fileTree/help.ts` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/fileTree/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/graph/Graph.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/graph/Graph.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/graph/help.ts` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/graph/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/ide/ActivePlan.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/ide/ActivePlan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/ide/IDE.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/ide/IDE.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/ide/RunPlan.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/ide/RunPlan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/input/Input.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/input/Input.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/input/InputToggle.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/input/InputToggle.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/logo/Spinner.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/logo/Spinner.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/logo/SqlMesh.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/logo/SqlMesh.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/logo/Tobiko.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/logo/Tobiko.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/modal/Modal.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/modal/Modal.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/modal/ModalConfirmation.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/modal/ModalConfirmation.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/modal/ModalDrawer.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/modal/ModalDrawer.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/Plan.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/Plan.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/PlanActions.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/PlanActions.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/PlanBackfillDates.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/PlanBackfillDates.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/PlanChangePreview.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/PlanChangePreview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/PlanHeader.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/PlanHeader.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/PlanWizard.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/PlanWizard.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/PlanWizardStepOptions.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/PlanWizardStepOptions.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/context.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/context.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/help.spec.ts` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/help.spec.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/help.ts` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/help.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/plan/hooks.ts` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/plan/hooks.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/progress/Progress.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/progress/Progress.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/report/ReportTestsErrors.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/report/ReportTestsErrors.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/root/Footer.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/root/Footer.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/root/Header.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/root/Header.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/splitPane/SplitPane.css` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/splitPane/SplitPane.css`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/splitPane/SplitPane.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/splitPane/SplitPane.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/tasksOverview/TasksOverview.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/tasksOverview/TasksOverview.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/library/components/toggle/Toggle.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/library/components/toggle/Toggle.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/main.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/main.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/models/artifact.ts` & `sqlmesh-0.5.1.dev28/web/client/src/models/artifact.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/models/directory.ts` & `sqlmesh-0.5.1.dev28/web/client/src/models/directory.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/models/environment.ts` & `sqlmesh-0.5.1.dev28/web/client/src/models/environment.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/models/file.ts` & `sqlmesh-0.5.1.dev28/web/client/src/models/file.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/models/initial.ts` & `sqlmesh-0.5.1.dev28/web/client/src/models/initial.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/tests/utils.tsx` & `sqlmesh-0.5.1.dev28/web/client/src/tests/utils.tsx`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/utils/index.spec.ts` & `sqlmesh-0.5.1.dev28/web/client/src/utils/index.spec.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/utils/index.ts` & `sqlmesh-0.5.1.dev28/web/client/src/utils/index.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/workers/sqlglot/sqlglot.py` & `sqlmesh-0.5.1.dev28/web/client/src/workers/sqlglot/sqlglot.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/src/workers/sqlglot/worker.ts` & `sqlmesh-0.5.1.dev28/web/client/src/workers/sqlglot/worker.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/tailwind.config.js` & `sqlmesh-0.5.1.dev28/web/client/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/tsconfig.json` & `sqlmesh-0.5.1.dev28/web/client/tsconfig.json`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/client/vite.config.ts` & `sqlmesh-0.5.1.dev28/web/client/vite.config.ts`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/server/api/endpoints/__init__.py` & `sqlmesh-0.5.1.dev28/web/server/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/server/api/endpoints/commands.py` & `sqlmesh-0.5.1.dev28/web/server/api/endpoints/commands.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/server/api/endpoints/context.py` & `sqlmesh-0.5.1.dev28/web/server/api/endpoints/context.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/server/api/endpoints/directories.py` & `sqlmesh-0.5.1.dev28/web/server/api/endpoints/directories.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/server/api/endpoints/environments.py` & `sqlmesh-0.5.1.dev28/web/server/api/endpoints/environments.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/server/api/endpoints/events.py` & `sqlmesh-0.5.1.dev28/web/server/api/endpoints/events.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/server/api/endpoints/files.py` & `sqlmesh-0.5.1.dev28/web/server/api/endpoints/files.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/server/api/endpoints/lineage.py` & `sqlmesh-0.5.1.dev28/web/server/api/endpoints/lineage.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/server/api/endpoints/models.py` & `sqlmesh-0.5.1.dev28/web/server/api/endpoints/models.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/server/api/endpoints/plan.py` & `sqlmesh-0.5.1.dev28/web/server/api/endpoints/plan.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/server/console.py` & `sqlmesh-0.5.1.dev28/web/server/console.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/server/main.py` & `sqlmesh-0.5.1.dev28/web/server/main.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/server/models.py` & `sqlmesh-0.5.1.dev28/web/server/models.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/server/settings.py` & `sqlmesh-0.5.1.dev28/web/server/settings.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/server/sse.py` & `sqlmesh-0.5.1.dev28/web/server/sse.py`

 * *Files identical despite different names*

### Comparing `sqlmesh-0.5.1.dev22/web/server/utils.py` & `sqlmesh-0.5.1.dev28/web/server/utils.py`

 * *Files identical despite different names*

