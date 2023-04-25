# Comparing `tmp/mitzu-0.6.0rc1.tar.gz` & `tmp/mitzu-0.6.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitzu-0.6.0rc1.tar", max compression
+gzip compressed data, was "mitzu-0.6.0rc2.tar", max compression
```

## Comparing `mitzu-0.6.0rc1.tar` & `mitzu-0.6.0rc2.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     1082 2023-04-22 19:42:35.921651 mitzu-0.6.0rc1/LICENSE.txt
--rw-r--r--   0        0        0     2235 2023-04-22 19:42:35.921651 mitzu-0.6.0rc1/README.md
--rw-r--r--   0        0        0     6148 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/.DS_Store
--rw-r--r--   0        0        0      865 2023-04-22 19:43:38.102597 mitzu-0.6.0rc1/mitzu/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/__init__.py
--rw-r--r--   0        0        0     1762 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/adapter_factory.py
--rw-r--r--   0        0        0     5234 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/athena_adapter.py
--rw-r--r--   0        0        0     6072 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/databricks_adapter.py
--rw-r--r--   0        0        0     2261 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/file_adapter.py
--rw-r--r--   0        0        0     2563 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/generic_adapter.py
--rw-r--r--   0        0        0      723 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/helper.py
--rw-r--r--   0        0        0     3422 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/mysql_adapter.py
--rw-r--r--   0        0        0     2297 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/postgresql_adapter.py
--rw-r--r--   0        0        0     4085 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/redshift_adapter.py
--rw-r--r--   0        0        0     3344 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/snowflake_adapter.py
--rw-r--r--   0        0        0        0 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      660 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/__init__.py
--rw-r--r--   0        0        0      701 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5071 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6415 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
--rw-r--r--   0        0        0     9751 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1844 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
--rw-r--r--   0        0        0      672 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/__init__.py
--rw-r--r--   0        0        0      713 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5010 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6601 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
--rw-r--r--   0        0        0    10073 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1848 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
--rw-r--r--   0        0        0    39389 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy_adapter.py
--rw-r--r--   0        0        0     5009 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/adapters/sqlite_adapter.py
--rw-r--r--   0        0        0     6687 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/adapters/trino_adapter.py
--rw-r--r--   0        0        0     1760 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/helper.py
--rw-r--r--   0        0        0    54541 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/model.py
--rw-r--r--   0        0        0        0 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/notebook/__init__.py
--rw-r--r--   0        0        0     6818 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/notebook/model_loader.py
--rw-r--r--   0        0        0     5424 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/project_discovery.py
--rw-r--r--   0        0        0     2086 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/project_serialization.py
--rw-r--r--   0        0        0      785 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/samples/__init__.py
--rw-r--r--   0        0        0     3794 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/samples/data_ingestion.py
--rw-r--r--   0        0        0    10141 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/samples/sample_data_generator.py
--rw-r--r--   0        0        0    11435 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/serialization.py
--rw-r--r--   0        0        0        0 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/visualization/__init__.py
--rw-r--r--   0        0        0     7124 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/visualization/charts.py
--rw-r--r--   0        0        0     1854 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/visualization/common.py
--rw-r--r--   0        0        0      941 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/visualization/labels.py
--rw-r--r--   0        0        0     7547 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/visualization/plot.py
--rw-r--r--   0        0        0     5372 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/visualization/titles.py
--rw-r--r--   0        0        0     3181 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/visualization/tooltips.py
--rw-r--r--   0        0        0     3339 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/visualization/transform_conv.py
--rw-r--r--   0        0        0     1261 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/visualization/transform_retention.py
--rw-r--r--   0        0        0     6148 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/.DS_Store
--rw-r--r--   0        0        0        0 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/__init__.py
--rw-r--r--   0        0        0     5347 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/explore_page.css
--rw-r--r--   0        0        0   147145 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/favicon.ico
--rw-r--r--   0        0        0    46702 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/logo.png
--rw-r--r--   0        0        0    43472 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/mitzu-logo-light.svg
--rw-r--r--   0        0        0    49422 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/athena.png
--rw-r--r--   0        0        0    10321 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/clickhouse.png
--rw-r--r--   0        0        0   119554 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/databricks.png
--rw-r--r--   0        0        0     3008 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/mysql.png
--rw-r--r--   0        0        0     2446 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/pandas.png
--rw-r--r--   0        0        0     5338 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/postgresql.png
--rw-r--r--   0        0        0     8512 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/redshift.png
--rw-r--r--   0        0        0    93500 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/snowflake.png
--rw-r--r--   0        0        0    48681 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/sqlite.png
--rw-r--r--   0        0        0    34219 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/trino.png
--rw-r--r--   0        0        0    14499 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/auth/authorizer.py
--rw-r--r--   0        0        0     3557 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/auth/cognito.py
--rw-r--r--   0        0        0     1963 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/auth/decorator.py
--rw-r--r--   0        0        0     2777 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/auth/google.py
--rw-r--r--   0        0        0     7392 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/cache.py
--rw-r--r--   0        0        0     2966 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/caching_dataset_adapter.py
--rw-r--r--   0        0        0     2595 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/configs.py
--rw-r--r--   0        0        0     3382 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/dependencies.py
--rw-r--r--   0        0        0     4833 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/helper.py
--rw-r--r--   0        0        0     8355 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/model.py
--rw-r--r--   0        0        0      408 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/navbar.py
--rw-r--r--   0        0        0     6460 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/offcanvas.py
--rw-r--r--   0        0        0        0 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/connections/__init__.py
--rw-r--r--   0        0        0    15406 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/connections/manage_connections_component.py
--rw-r--r--   0        0        0     4195 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/connections_page.py
--rw-r--r--   0        0        0        0 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/dashboards/__init__.py
--rw-r--r--   0        0        0    21143 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
--rw-r--r--   0        0        0     9799 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/dashboards.py
--rw-r--r--   0        0        0    15447 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/edit_user.py
--rw-r--r--   0        0        0        0 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/__init__.py
--rw-r--r--   0        0        0     5299 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/complex_segment_handler.py
--rw-r--r--   0        0        0     6488 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/dates_selector_handler.py
--rw-r--r--   0        0        0     5564 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/event_segment_handler.py
--rw-r--r--   0        0        0    16412 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/explore_page.py
--rw-r--r--   0        0        0    10152 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/graph_handler.py
--rw-r--r--   0        0        0    11669 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/metric_config_handler.py
--rw-r--r--   0        0        0     2375 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/metric_segments_handler.py
--rw-r--r--   0        0        0     1565 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/metric_type_handler.py
--rw-r--r--   0        0        0     9783 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/simple_segment_handler.py
--rw-r--r--   0        0        0     4644 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/toolbar_handler.py
--rw-r--r--   0        0        0     1401 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore_project.py
--rw-r--r--   0        0        0     1708 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/home.py
--rw-r--r--   0        0        0     4123 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/login.py
--rw-r--r--   0        0        0     3928 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/manage_connection.py
--rw-r--r--   0        0        0     1315 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/manage_dashboard.py
--rw-r--r--   0        0        0    10034 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/manage_event_defs.py
--rw-r--r--   0        0        0    11710 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/manage_project.py
--rw-r--r--   0        0        0    10013 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/manage_saved_metrics.py
--rw-r--r--   0        0        0     1733 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/paths.py
--rw-r--r--   0        0        0        0 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/projects/__init__.py
--rw-r--r--   0        0        0    35869 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/projects/event_tables_config.py
--rw-r--r--   0        0        0      587 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/projects/helper.py
--rw-r--r--   0        0        0     9231 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/projects/manage_project_component.py
--rw-r--r--   0        0        0     4901 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/projects_page.py
--rw-r--r--   0        0        0     3304 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/users.py
--rw-r--r--   0        0        0        0 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/service/__init__.py
--rw-r--r--   0        0        0     2172 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/service/events_service.py
--rw-r--r--   0        0        0     5366 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/service/navbar_service.py
--rw-r--r--   0        0        0     2105 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/service/secret_service.py
--rw-r--r--   0        0        0     4710 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/service/user_service.py
--rw-r--r--   0        0        0    19970 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/storage.py
--rw-r--r--   0        0        0    25909 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/storage_model.py
--rw-r--r--   0        0        0      666 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/toast.py
--rw-r--r--   0        0        0     4266 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/webapp.py
--rw-r--r--   0        0        0     2965 2023-04-22 19:43:38.098597 mitzu-0.6.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 mitzu-0.6.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-25 11:40:58.478845 mitzu-0.6.0rc2/LICENSE.txt
+-rw-r--r--   0        0        0     2235 2023-04-25 11:40:58.478845 mitzu-0.6.0rc2/README.md
+-rw-r--r--   0        0        0     6148 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/.DS_Store
+-rw-r--r--   0        0        0      865 2023-04-25 11:42:10.543900 mitzu-0.6.0rc2/mitzu/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/__init__.py
+-rw-r--r--   0        0        0     1762 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/adapter_factory.py
+-rw-r--r--   0        0        0     5234 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/athena_adapter.py
+-rw-r--r--   0        0        0     6072 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/databricks_adapter.py
+-rw-r--r--   0        0        0     2261 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/file_adapter.py
+-rw-r--r--   0        0        0     2563 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/generic_adapter.py
+-rw-r--r--   0        0        0      723 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/helper.py
+-rw-r--r--   0        0        0     3422 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/mysql_adapter.py
+-rw-r--r--   0        0        0     2297 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/postgresql_adapter.py
+-rw-r--r--   0        0        0     4085 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/redshift_adapter.py
+-rw-r--r--   0        0        0     3344 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/snowflake_adapter.py
+-rw-r--r--   0        0        0        0 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      660 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/__init__.py
+-rw-r--r--   0        0        0      701 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5071 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6415 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0     9751 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1844 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
+-rw-r--r--   0        0        0      672 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/__init__.py
+-rw-r--r--   0        0        0      713 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5010 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6601 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0    10073 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1848 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
+-rw-r--r--   0        0        0    39389 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy_adapter.py
+-rw-r--r--   0        0        0     5009 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/sqlite_adapter.py
+-rw-r--r--   0        0        0     6687 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/adapters/trino_adapter.py
+-rw-r--r--   0        0        0     1760 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/helper.py
+-rw-r--r--   0        0        0    54541 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/model.py
+-rw-r--r--   0        0        0        0 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/notebook/__init__.py
+-rw-r--r--   0        0        0     6818 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/notebook/model_loader.py
+-rw-r--r--   0        0        0     5424 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/project_discovery.py
+-rw-r--r--   0        0        0     2086 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/project_serialization.py
+-rw-r--r--   0        0        0      785 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/samples/__init__.py
+-rw-r--r--   0        0        0     3794 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/samples/data_ingestion.py
+-rw-r--r--   0        0        0    10141 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/samples/sample_data_generator.py
+-rw-r--r--   0        0        0    11435 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/serialization.py
+-rw-r--r--   0        0        0        0 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/visualization/__init__.py
+-rw-r--r--   0        0        0     7124 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/visualization/charts.py
+-rw-r--r--   0        0        0     1854 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/visualization/common.py
+-rw-r--r--   0        0        0      941 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/visualization/labels.py
+-rw-r--r--   0        0        0     7547 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/visualization/plot.py
+-rw-r--r--   0        0        0     5372 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/visualization/titles.py
+-rw-r--r--   0        0        0     3181 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/visualization/tooltips.py
+-rw-r--r--   0        0        0     3339 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/visualization/transform_conv.py
+-rw-r--r--   0        0        0     1261 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/visualization/transform_retention.py
+-rw-r--r--   0        0        0     6148 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/webapp/.DS_Store
+-rw-r--r--   0        0        0        0 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/webapp/__init__.py
+-rw-r--r--   0        0        0     5347 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/webapp/assets/explore_page.css
+-rw-r--r--   0        0        0   147145 2023-04-25 11:40:58.934851 mitzu-0.6.0rc2/mitzu/webapp/assets/favicon.ico
+-rw-r--r--   0        0        0    46702 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/logo.png
+-rw-r--r--   0        0        0    43472 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/mitzu-logo-light.svg
+-rw-r--r--   0        0        0    49422 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/athena.png
+-rw-r--r--   0        0        0    10321 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/clickhouse.png
+-rw-r--r--   0        0        0   119554 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/databricks.png
+-rw-r--r--   0        0        0     3008 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/mysql.png
+-rw-r--r--   0        0        0     2446 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/pandas.png
+-rw-r--r--   0        0        0     5338 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/postgresql.png
+-rw-r--r--   0        0        0     8512 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/redshift.png
+-rw-r--r--   0        0        0    93500 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/snowflake.png
+-rw-r--r--   0        0        0    48681 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/sqlite.png
+-rw-r--r--   0        0        0    34219 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/trino.png
+-rw-r--r--   0        0        0    13355 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/auth/authorizer.py
+-rw-r--r--   0        0        0     3557 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/auth/cognito.py
+-rw-r--r--   0        0        0     1594 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/auth/decorator.py
+-rw-r--r--   0        0        0     2777 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/auth/google.py
+-rw-r--r--   0        0        0     7392 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/cache.py
+-rw-r--r--   0        0        0     2966 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/caching_dataset_adapter.py
+-rw-r--r--   0        0        0     2595 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/configs.py
+-rw-r--r--   0        0        0     2750 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/dependencies.py
+-rw-r--r--   0        0        0     4833 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/helper.py
+-rw-r--r--   0        0        0     8355 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/model.py
+-rw-r--r--   0        0        0      408 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/navbar.py
+-rw-r--r--   0        0        0     6112 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/offcanvas.py
+-rw-r--r--   0        0        0        0 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/connections/__init__.py
+-rw-r--r--   0        0        0    15406 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/connections/manage_connections_component.py
+-rw-r--r--   0        0        0     4195 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/connections_page.py
+-rw-r--r--   0        0        0        0 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/dashboards/__init__.py
+-rw-r--r--   0        0        0    21143 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
+-rw-r--r--   0        0        0     9799 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/dashboards.py
+-rw-r--r--   0        0        0    14789 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/edit_user.py
+-rw-r--r--   0        0        0        0 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/__init__.py
+-rw-r--r--   0        0        0     5299 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/complex_segment_handler.py
+-rw-r--r--   0        0        0     6488 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/dates_selector_handler.py
+-rw-r--r--   0        0        0     5564 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/event_segment_handler.py
+-rw-r--r--   0        0        0    16412 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/explore_page.py
+-rw-r--r--   0        0        0    10152 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/graph_handler.py
+-rw-r--r--   0        0        0    11669 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/metric_config_handler.py
+-rw-r--r--   0        0        0     2375 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/metric_segments_handler.py
+-rw-r--r--   0        0        0     1565 2023-04-25 11:40:58.938851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/metric_type_handler.py
+-rw-r--r--   0        0        0     9783 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/simple_segment_handler.py
+-rw-r--r--   0        0        0     4644 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore/toolbar_handler.py
+-rw-r--r--   0        0        0     1401 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/explore_project.py
+-rw-r--r--   0        0        0     1708 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/home.py
+-rw-r--r--   0        0        0     3894 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/login.py
+-rw-r--r--   0        0        0     4898 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/manage_connection.py
+-rw-r--r--   0        0        0     1315 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/manage_dashboard.py
+-rw-r--r--   0        0        0    10034 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/manage_event_defs.py
+-rw-r--r--   0        0        0    11756 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/manage_project.py
+-rw-r--r--   0        0        0    10013 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/manage_saved_metrics.py
+-rw-r--r--   0        0        0     1733 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/paths.py
+-rw-r--r--   0        0        0        0 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/projects/__init__.py
+-rw-r--r--   0        0        0    35893 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/projects/event_tables_config.py
+-rw-r--r--   0        0        0      587 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/projects/helper.py
+-rw-r--r--   0        0        0     9400 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/projects/manage_project_component.py
+-rw-r--r--   0        0        0     4901 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/projects_page.py
+-rw-r--r--   0        0        0     3146 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/pages/users.py
+-rw-r--r--   0        0        0        0 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/service/__init__.py
+-rw-r--r--   0        0        0     2172 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/service/events_service.py
+-rw-r--r--   0        0        0     5302 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/service/navbar_service.py
+-rw-r--r--   0        0        0     2105 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/service/secret_service.py
+-rw-r--r--   0        0        0     4710 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/service/user_service.py
+-rw-r--r--   0        0        0    20518 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/storage.py
+-rw-r--r--   0        0        0    25909 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/storage_model.py
+-rw-r--r--   0        0        0      666 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/toast.py
+-rw-r--r--   0        0        0     4141 2023-04-25 11:40:58.942851 mitzu-0.6.0rc2/mitzu/webapp/webapp.py
+-rw-r--r--   0        0        0     2965 2023-04-25 11:42:10.539900 mitzu-0.6.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 mitzu-0.6.0rc2/PKG-INFO
```

### Comparing `mitzu-0.6.0rc1/LICENSE.txt` & `mitzu-0.6.0rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/README.md` & `mitzu-0.6.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/.DS_Store` & `mitzu-0.6.0rc2/mitzu/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/__init__.py` & `mitzu-0.6.0rc2/mitzu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     TimeWindow,
     TimeGroup,
     DiscoverySettings,
     WebappSettings,
 )
 from mitzu.samples import get_sample_discovered_project
 
-__version__ = "0.6.0-rc.1"
+__version__ = "0.6.0-rc.2"
 
 
 __all__ = [
     "Connection",
     "ConnectionType",
     "Project",
     "EventDataTable",
```

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/adapter_factory.py` & `mitzu-0.6.0rc2/mitzu/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/athena_adapter.py` & `mitzu-0.6.0rc2/mitzu/adapters/athena_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/databricks_adapter.py` & `mitzu-0.6.0rc2/mitzu/adapters/databricks_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/file_adapter.py` & `mitzu-0.6.0rc2/mitzu/adapters/file_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/generic_adapter.py` & `mitzu-0.6.0rc2/mitzu/adapters/generic_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/helper.py` & `mitzu-0.6.0rc2/mitzu/adapters/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/mysql_adapter.py` & `mitzu-0.6.0rc2/mitzu/adapters/mysql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/postgresql_adapter.py` & `mitzu-0.6.0rc2/mitzu/adapters/postgresql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/redshift_adapter.py` & `mitzu-0.6.0rc2/mitzu/adapters/redshift_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/snowflake_adapter.py` & `mitzu-0.6.0rc2/mitzu/adapters/snowflake_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/__init__.py` & `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py` & `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py` & `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py` & `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py` & `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py` & `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/__init__.py` & `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py` & `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py` & `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py` & `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py` & `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py` & `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy_adapter.py` & `mitzu-0.6.0rc2/mitzu/adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/sqlite_adapter.py` & `mitzu-0.6.0rc2/mitzu/adapters/sqlite_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/adapters/trino_adapter.py` & `mitzu-0.6.0rc2/mitzu/adapters/trino_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/helper.py` & `mitzu-0.6.0rc2/mitzu/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/model.py` & `mitzu-0.6.0rc2/mitzu/model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/notebook/model_loader.py` & `mitzu-0.6.0rc2/mitzu/notebook/model_loader.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/project_discovery.py` & `mitzu-0.6.0rc2/mitzu/project_discovery.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/project_serialization.py` & `mitzu-0.6.0rc2/mitzu/project_serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/samples/__init__.py` & `mitzu-0.6.0rc2/mitzu/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/samples/data_ingestion.py` & `mitzu-0.6.0rc2/mitzu/samples/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/samples/sample_data_generator.py` & `mitzu-0.6.0rc2/mitzu/samples/sample_data_generator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/serialization.py` & `mitzu-0.6.0rc2/mitzu/serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/visualization/charts.py` & `mitzu-0.6.0rc2/mitzu/visualization/charts.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/visualization/common.py` & `mitzu-0.6.0rc2/mitzu/visualization/common.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/visualization/labels.py` & `mitzu-0.6.0rc2/mitzu/visualization/labels.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/visualization/plot.py` & `mitzu-0.6.0rc2/mitzu/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/visualization/titles.py` & `mitzu-0.6.0rc2/mitzu/visualization/titles.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/visualization/tooltips.py` & `mitzu-0.6.0rc2/mitzu/visualization/tooltips.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/visualization/transform_conv.py` & `mitzu-0.6.0rc2/mitzu/visualization/transform_conv.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/visualization/transform_retention.py` & `mitzu-0.6.0rc2/mitzu/visualization/transform_retention.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/.DS_Store` & `mitzu-0.6.0rc2/mitzu/webapp/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/assets/explore_page.css` & `mitzu-0.6.0rc2/mitzu/webapp/assets/explore_page.css`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/assets/favicon.ico` & `mitzu-0.6.0rc2/mitzu/webapp/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/assets/logo.png` & `mitzu-0.6.0rc2/mitzu/webapp/assets/logo.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/assets/mitzu-logo-light.svg` & `mitzu-0.6.0rc2/mitzu/webapp/assets/mitzu-logo-light.svg`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/athena.png` & `mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/athena.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/clickhouse.png` & `mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/databricks.png` & `mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/databricks.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/mysql.png` & `mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/mysql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/pandas.png` & `mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/pandas.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/postgresql.png` & `mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/postgresql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/redshift.png` & `mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/redshift.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/snowflake.png` & `mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/snowflake.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/sqlite.png` & `mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/sqlite.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/trino.png` & `mitzu-0.6.0rc2/mitzu/webapp/assets/warehouse/trino.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/auth/authorizer.py` & `mitzu-0.6.0rc2/mitzu/webapp/auth/authorizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,29 +77,29 @@
             oauth_config.jwt_algorithms,
             oauth_config.client_id,
         )
 
 
 @dataclass(frozen=True)
 class AuthConfig:
+    user_service: U.UserService
+
     token_cookie_name: str = field(default_factory=lambda: "auth-token")
     redirect_cookie_name: str = field(default_factory=lambda: "redirect-to")
 
     session_timeout: int = field(default_factory=lambda: 7 * 24 * 60 * 60)
     token_signing_key: str = field(default_factory=lambda: configs.AUTH_JWT_SECRET)
 
     oauth: Optional[OAuthConfig] = None
     token_validator: Optional[TokenValidator] = None
-    allowed_email_domain: Optional[str] = None
-
-    user_service: Optional[U.UserService] = None
 
 
 @dataclass(frozen=True)
 class OAuthAuthorizer:
+    _config: AuthConfig
 
     _authorized_url_prefixes: List[str] = field(
         default_factory=lambda: [
             P.UNAUTHORIZED_URL,
             configs.HEALTH_CHECK_PATH,
             "/assets/",
             "/_dash-update-component",
@@ -112,15 +112,14 @@
         default_factory=lambda: [
             P.UNAUTHORIZED_URL,
             P.SIGN_OUT_URL,
             configs.HEALTH_CHECK_PATH,
             "/assets/",
         ]
     )
-    _config: AuthConfig = field(default_factory=lambda: AuthConfig())
 
     @classmethod
     def create(cls, config: AuthConfig) -> OAuthAuthorizer:
         return OAuthAuthorizer(
             _config=config,
         )
 
@@ -204,26 +203,19 @@
 
     def _validate_token(self, token: str) -> Optional[Dict]:
         try:
             claims = jwt.decode(
                 token, self._config.token_signing_key, algorithms=[JWT_ALGORITHM]
             )
 
-            if self._config.user_service is not None:
-                user_id = claims["sub"]
-                user = self._config.user_service.get_user_by_id(user_id)
-                if user is None:
-                    raise Exception("User not found")
-                claims[JWT_CLAIM_ROLE] = user.role
-            elif JWT_CLAIM_ROLE in claims.keys():
-                claims[JWT_CLAIM_ROLE] = WM.Role(claims[JWT_CLAIM_ROLE])
-            else:
-                claims[
-                    JWT_CLAIM_ROLE
-                ] = WM.Role.MEMBER  # backward compatibility with old sessions
+            user_id = claims["sub"]
+            user = self._config.user_service.get_user_by_id(user_id)
+            if user is None:
+                raise Exception("User not found")
+            claims[JWT_CLAIM_ROLE] = user.role
             return claims
         except Exception as e:
             LOGGER.warning(f"Failed to validate token: {str(e)}")
             return None
 
     def _validate_foreign_token(self, token) -> Optional[str]:
         if not self._config.token_validator:
@@ -260,28 +252,17 @@
                         self._config.redirect_cookie_name, MITZU_WEBAPP_URL
                     )
 
                     user_email = self._validate_foreign_token(id_token)
                     if not user_email:
                         raise Exception("Unauthorized (Invalid jwt token)")
 
-                    if (
-                        self._config.allowed_email_domain is not None
-                        and not user_email.endswith(self._config.allowed_email_domain)
-                    ):
-                        raise Exception(
-                            f"User tried to login with not allowed email address: {user_email}"
-                        )
-
                     user_role = WM.Role.MEMBER
                     token_identity = user_email
-                    if (
-                        configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS
-                        and self._config.user_service is not None
-                    ):
+                    if configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS:
                         user = self._config.user_service.get_user_by_email(user_email)
                         if user is None:
                             raise Exception(
                                 f"User tried to login without having a local user: {user_email}"
                             )
                         user_role = user.role
                         token_identity = user.id
@@ -343,30 +324,25 @@
 
     def is_request_authorized(self, request: flask.Request) -> bool:
         auth_token = request.cookies.get(self._config.token_cookie_name)
         return auth_token is not None and self._validate_token(auth_token) is not None
 
     def get_current_user_role(self, request: flask.Request) -> Optional[WM.Role]:
         auth_token = request.cookies.get(self._config.token_cookie_name)
-        if self._config.user_service is None:
-            return WM.Role.MEMBER
 
         if auth_token is None:
             return None
 
         claims = self._validate_token(auth_token)
         if claims is None or JWT_CLAIM_ROLE not in claims.keys():
             return None
 
         return WM.Role(claims[JWT_CLAIM_ROLE])
 
     def login_local_user(self, email: str, password: str) -> bool:
-        if self._config.user_service is None:
-            raise ValueError("User service is not set for local auth")
-
         if configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS:
             raise ValueError("Password login is not enabled, need to use SSO")
 
         user = self._config.user_service.get_user_by_email_and_password(email, password)
         if user is None:
             return False
```

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/auth/cognito.py` & `mitzu-0.6.0rc2/mitzu/webapp/auth/cognito.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/auth/decorator.py` & `mitzu-0.6.0rc2/mitzu/webapp/auth/decorator.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,56 +11,47 @@
 def restricted(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         dependencies: DEPS.Dependencies = cast(
             DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
         )
 
-        if dependencies.authorizer is not None:
-            if dependencies.authorizer.is_request_authorized(flask.request):
-                return func(*args, **kwargs)
-            else:
-                raise PreventUpdate
-        else:
+        if dependencies.authorizer.is_request_authorized(flask.request):
             return func(*args, **kwargs)
+        else:
+            raise PreventUpdate
 
     return wrapper
 
 
 def restricted_for_admin(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         dependencies: DEPS.Dependencies = cast(
             DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
         )
 
-        if dependencies.authorizer is not None:
-            user_role = dependencies.authorizer.get_current_user_role(flask.request)
-            if user_role is None:
-                raise PreventUpdate
-
-            if user_role != WM.Role.ADMIN:
-                raise PreventUpdate
-            else:
-                return func(*args, **kwargs)
+        user_role = dependencies.authorizer.get_current_user_role(flask.request)
+        if user_role is None:
+            raise PreventUpdate
+
+        if user_role != WM.Role.ADMIN:
+            raise PreventUpdate
         else:
             return func(*args, **kwargs)
 
     return wrapper
 
 
 def restricted_layout(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         dependencies: DEPS.Dependencies = cast(
             DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
         )
 
-        if dependencies.authorizer is not None:
-            if dependencies.authorizer.is_request_authorized(flask.request):
-                return func(*args, **kwargs)
-            else:
-                return Location("url", href=P.UNAUTHORIZED_URL)
-        else:
+        if dependencies.authorizer.is_request_authorized(flask.request):
             return func(*args, **kwargs)
+        else:
+            return Location("url", href=P.UNAUTHORIZED_URL)
 
     return wrapper
```

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/auth/google.py` & `mitzu-0.6.0rc2/mitzu/webapp/auth/google.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/cache.py` & `mitzu-0.6.0rc2/mitzu/webapp/cache.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/caching_dataset_adapter.py` & `mitzu-0.6.0rc2/mitzu/webapp/caching_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/configs.py` & `mitzu-0.6.0rc2/mitzu/webapp/configs.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/dependencies.py` & `mitzu-0.6.0rc2/mitzu/webapp/dependencies.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Optional
 
 
 import mitzu.webapp.auth.authorizer as A
 import mitzu.webapp.cache as C
 import mitzu.webapp.configs as configs
 import mitzu.webapp.storage as S
 import mitzu.webapp.service.user_service as U
@@ -15,72 +14,57 @@
 
 CONFIG_KEY = "dependencies"
 
 
 @dataclass(frozen=True)
 class Dependencies:
 
-    authorizer: Optional[A.OAuthAuthorizer]
+    authorizer: A.OAuthAuthorizer
     storage: S.MitzuStorage
     queue: C.MitzuCache
     cache: C.MitzuCache
     events_service: E.EventsService
     navbar_service: NB.NavbarService
     secret_service: SS.SecretService
-    user_service: Optional[U.UserService] = None
+    user_service: U.UserService
 
     @classmethod
     def from_configs(cls) -> Dependencies:
         delegate_cache: C.MitzuCache
         if configs.STORAGE_REDIS_HOST is not None:
             delegate_cache = C.RedisMitzuCache(global_prefix=configs.CACHE_PREFIX)
         else:
             delegate_cache = C.DiskMitzuCache(
                 "cache", global_prefix=configs.CACHE_PREFIX
             )
         cache = C.RequestCache(delegate_cache)
         storage = S.MitzuStorage(connection_string=configs.STORAGE_CONNECTION_STRING)
 
-        authorizer = None
         oauth_config = None
-        user_service = None
-        create_user_service = False
         if configs.AUTH_BACKEND == "cognito":
             from mitzu.webapp.auth.cognito import Cognito
 
             oauth_config = Cognito.get_config()
-            create_user_service = configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS
         elif configs.AUTH_BACKEND == "google":
             from mitzu.webapp.auth.google import GoogleOAuth
 
             oauth_config = GoogleOAuth.get_config()
-            create_user_service = configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS
 
-        elif configs.AUTH_BACKEND == "local":
-            create_user_service = True
+        user_service = U.UserService(storage, root_password=configs.AUTH_ROOT_PASSWORD)
 
-        if create_user_service:
-            user_service = U.UserService(
-                storage, root_password=configs.AUTH_ROOT_PASSWORD
-            )
-
-        if oauth_config or user_service:
-            auth_config = A.AuthConfig(
-                oauth=oauth_config,
-                token_validator=A.JWTTokenValidator.create_from_oauth_config(
-                    oauth_config
-                )
-                if oauth_config is not None
-                else None,
-                allowed_email_domain=configs.AUTH_ALLOWED_EMAIL_DOMAIN,
-                token_signing_key=configs.AUTH_JWT_SECRET,
-                session_timeout=configs.AUTH_SESSION_TIMEOUT,
-                user_service=user_service,
-            )
-            authorizer = A.OAuthAuthorizer.create(auth_config)
+        auth_config = A.AuthConfig(
+            oauth=oauth_config,
+            token_validator=A.JWTTokenValidator.create_from_oauth_config(oauth_config)
+            if oauth_config is not None
+            else None,
+            token_signing_key=configs.AUTH_JWT_SECRET,
+            session_timeout=configs.AUTH_SESSION_TIMEOUT,
+            user_service=user_service,
+        )
+        authorizer = A.OAuthAuthorizer.create(auth_config)
 
         queue: C.MitzuCache
         if configs.QUEUE_REDIS_HOST is not None:
             queue = C.RedisMitzuCache()
         else:
             queue = C.DiskMitzuCache("queue")
```

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/helper.py` & `mitzu-0.6.0rc2/mitzu/webapp/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/model.py` & `mitzu-0.6.0rc2/mitzu/webapp/model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/offcanvas.py` & `mitzu-0.6.0rc2/mitzu/webapp/offcanvas.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,20 +36,14 @@
 EXPLORE_MENU_ITEM_CSS = "mb-1 w-100 text-start"
 
 
 def create_offcanvas(dependencies: DEPS.Dependencies) -> dbc.Offcanvas:
     project_ids = dependencies.storage.list_projects()
     project_id = project_ids[0] if len(project_ids) > 0 else None
 
-    show_users = False
-    show_sign_out = False
-    if dependencies.authorizer is not None:
-        show_sign_out = True
-        show_users = dependencies.authorizer._config.user_service is not None
-
     res = dbc.Offcanvas(
         children=[
             dbc.Row(
                 [
                     dbc.Col(
                         dcc.Link(
                             html.Img(
@@ -132,36 +126,30 @@
             html.Hr(className="mb-3"),
             dbc.Button(
                 [html.B(className="bi bi-person-circle me-1"), "Users"],
                 color=BUTTON_COLOR,
                 class_name=MENU_ITEM_CSS,
                 href=P.USERS_PATH,
                 id=USERS_BUTTON,
-            )
-            if show_users
-            else None,
+            ),
             dbc.Button(
                 [html.B(className="bi bi-person-circle me-1"), "My Account"],
                 color=BUTTON_COLOR,
                 class_name=MENU_ITEM_CSS,
                 href=P.create_path(P.USERS_HOME_PATH, user_id="my-account"),
                 id=MY_ACCOUNT_BUTTON,
-            )
-            if show_users
-            else None,
+            ),
             html.Hr(className="mb-3 d-none"),
             dbc.Button(
                 [html.B(className="bi bi-box-arrow-right me-1"), "Sign out"],
                 color="light",
                 class_name=MENU_ITEM_CSS,
                 href=P.SIGN_OUT_URL,
                 external_link=True,
-            )
-            if show_sign_out
-            else None,
+            ),
             html.Div(
                 f"v{version}",
                 className="position-absolute bottom-0 start-0 p-2",
                 style={"opacity": "0.5"},
             ),
         ],
         close_button=False,
```

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/connections/manage_connections_component.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/connections/manage_connections_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/connections_page.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/connections_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/dashboards/manage_dashboards_component.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/dashboards/manage_dashboards_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/dashboards.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/dashboards.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/edit_user.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/edit_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,19 +46,14 @@
 CHANGE_ROLE_RESPONSE_CONTAINER = "user_change_role_response_container"
 
 
 @restricted_layout
 def layout(user_id: str, **query_params) -> bc.Component:
     deps = cast(DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY))
     user_service = deps.user_service
-    if user_service is None:
-        raise ValueError("User service is not set")
-
-    if deps.authorizer is None:
-        raise ValueError("Authorizer is not set")
 
     logged_in_user_id = deps.authorizer.get_current_user_id()
     if logged_in_user_id is None:
         raise ValueError("Cannot determine logged in user id")
     logged_in_user = user_service.get_user_by_id(logged_in_user_id)
     if logged_in_user is None:
         raise ValueError("Logged in user is not found")
@@ -284,17 +279,14 @@
     prevent_initial_call=True,
 )
 @restricted_for_admin
 def create_new_user(n_clicks: int, email="", role="", password="", confirm_password=""):
     deps = cast(DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY))
     user_service = deps.user_service
 
-    if user_service is None:
-        raise ValueError("User service is not set")
-
     if configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS:
         # new user need a password other than empty string
         from uuid import uuid4
 
         password = str(uuid4())
         confirm_password = password
 
@@ -331,20 +323,14 @@
 def update_password(
     n_clicks: int, password="", confirm_password="", pathname: str = ""
 ):
     deps = cast(DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY))
 
     user_service = deps.user_service
 
-    if user_service is None:
-        raise ValueError("User service is not set")
-
-    if deps.authorizer is None:
-        raise ValueError("Authorizer is not set")
-
     try:
         logged_in_user_id = deps.authorizer.get_current_user_id()
         logged_in_user = user_service.get_user_by_id(logged_in_user_id)
 
         user_id = P.get_path_value(P.USERS_HOME_PATH, pathname, P.USER_PATH_PART)
         if logged_in_user is None:
             raise Exception("User is not signed in")
@@ -383,20 +369,14 @@
 )
 @restricted_for_admin
 def update_role(n_clicks: int, role="", pathname: str = ""):
     deps = cast(DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY))
 
     user_service = deps.user_service
 
-    if user_service is None:
-        raise ValueError("User service is not set")
-
-    if deps.authorizer is None:
-        raise ValueError("Authorizer is not set")
-
     try:
         logged_in_user_id = deps.authorizer.get_current_user_id()
 
         user_id = P.get_path_value(P.USERS_HOME_PATH, pathname, P.USER_PATH_PART)
         if logged_in_user_id is None:
             raise Exception("User is not signed in")
 
@@ -425,17 +405,14 @@
 )
 @restricted_for_admin
 def delete_user(n_clicks: int, pathname: str = ""):
     user_id = P.get_path_value(P.USERS_HOME_PATH, pathname, P.USER_PATH_PART)
     deps = cast(DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY))
     user_service = deps.user_service
 
-    if user_service is None:
-        raise ValueError("User service is not set")
-
     try:
         if user_id == "my-account":
             raise Exception("Own account cannot be deleted")
 
         user_service.delete_user(user_id)
         return {
             DELETE_RESPONSE_CONTAINER: "User deleted",
```

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/explore/complex_segment_handler.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/explore/complex_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/explore/dates_selector_handler.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/explore/dates_selector_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/explore/event_segment_handler.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/explore/event_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/explore/explore_page.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/explore/explore_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/explore/graph_handler.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/explore/graph_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/explore/metric_config_handler.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/explore/metric_config_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/explore/metric_segments_handler.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/explore/metric_segments_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/explore/metric_type_handler.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/explore/metric_type_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/explore/simple_segment_handler.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/explore/simple_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/explore/toolbar_handler.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/explore/toolbar_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/explore_project.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/explore_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/home.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/home.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/login.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/login.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,23 +136,14 @@
     prevent_initial_call=True,
 )
 def login(n_click: int, inputs: List[str]):
     authorizer = cast(
         DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
     ).authorizer
 
-    if authorizer is None:
-        return (
-            no_update,
-            html.P(
-                "Authorizer is not configured for local user login",
-                className="color-danger lead",
-            ),
-        )
-
     if authorizer.login_local_user(inputs[0], inputs[1]):
         return (P.HOME_PATH, "")
     return (
         no_update,
         html.P(
             "Bad credentials",
             className="text-danger lead text-center",
```

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/manage_connection.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/manage_connection.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,28 +9,30 @@
     Output,
     State,
     callback,
     ctx,
     html,
     no_update,
     register_page,
+    dcc,
 )
 
 import mitzu.helper as H
 import mitzu.model as M
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.navbar as NB
 import mitzu.webapp.pages.connections.manage_connections_component as MCC
 import mitzu.webapp.pages.paths as P
 from mitzu.webapp.auth.decorator import restricted, restricted_layout
-from mitzu.webapp.helper import MITZU_LOCATION
 
 CONNECTION_SAVE_BUTTON = "connection_save_button"
 CONNECTION_CLOSE_BUTTON = "connection_close_button"
+CONNECTION_LOCATION = "connection_location"
 SAVE_RESPONSE_CONTAINER = "save_response_container"
+CONNECTION_SAVE_AND_ADD_PROJECT_BUTTON = "connection_save_and_add_project"
 
 
 @restricted_layout
 def no_connection_layout():
     return layout(None)
 
 
@@ -46,14 +48,15 @@
     title = "Create new connection" if connection is None else "Manage connection"
 
     return dbc.Form(
         [
             NB.create_mitzu_navbar("create-connection-navbar"),
             dbc.Container(
                 children=[
+                    dcc.Location(id=CONNECTION_LOCATION),
                     html.H4(title),
                     html.Hr(),
                     MCC.create_manage_connection_component(connection),
                     html.Hr(),
                     html.Div(
                         [
                             dbc.Button(
@@ -62,16 +65,26 @@
                                 class_name="me-3",
                                 id=CONNECTION_CLOSE_BUTTON,
                                 href=P.CONNECTIONS_PATH,
                             ),
                             dbc.Button(
                                 [html.B(className="bi bi-check-circle"), " Save"],
                                 color="success",
+                                class_name="me-3",
                                 id=CONNECTION_SAVE_BUTTON,
                             ),
+                            dbc.Button(
+                                [
+                                    html.B(className="bi bi-plus-circle"),
+                                    " Save and add project",
+                                ],
+                                color="primary",
+                                class_name="me-3",
+                                id=CONNECTION_SAVE_AND_ADD_PROJECT_BUTTON,
+                            ),
                         ],
                         className="mb-3",
                     ),
                     html.Div(children=[], id=SAVE_RESPONSE_CONTAINER),
                 ],
                 class_name="mb-3",
             ),
@@ -93,36 +106,42 @@
     title="Mitzu - Manage Connection",
     layout=layout,
 )
 
 
 @callback(
     Output(SAVE_RESPONSE_CONTAINER, "children"),
+    Output(CONNECTION_LOCATION, "href"),
     Input(CONNECTION_SAVE_BUTTON, "n_clicks"),
+    Input(CONNECTION_SAVE_AND_ADD_PROJECT_BUTTON, "n_clicks"),
     State({"type": MCC.INDEX_TYPE, "index": ALL}, "value"),
-    State(MITZU_LOCATION, "pathname"),
     prevent_initial_call=True,
 )
 @restricted
 def save_button_clicked(
-    n_clicks: int, values: List[Any], pathname: str
+    save_button_clicks: int,
+    save_and_add_project_button_clicks: int,
+    values: List[Any],
 ) -> List[bc.Component]:
-    if n_clicks is None:
+    if save_button_clicks is None and save_and_add_project_button_clicks is None:
         return no_update
 
     vals = {}
-    for prop in ctx.args_grouping[1]:
+    for prop in ctx.args_grouping[2]:
         id_val = prop["id"]
         if id_val.get("type") == MCC.INDEX_TYPE:
             vals[id_val.get("index")] = prop["value"]
 
     connection = MCC.create_connection_from_values(vals)
     depenednecies: DEPS.Dependencies = cast(
         DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
     )
 
     invalid = MCC.validate_input_values(values=vals)
     if invalid is not None:
         return html.P(f"Invalid {H.value_to_label(invalid)}", className="lead")
     depenednecies.storage.set_connection(connection.id, connection)
 
-    return [html.P("Connection saved", className="lead")]
+    if ctx.triggered_id == CONNECTION_SAVE_BUTTON:
+        return [html.P("Connection saved", className="lead"), no_update]
+    else:
+        return [no_update, f"{P.PROJECTS_CREATE_PATH}?connection_id={connection.id}"]
```

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/manage_dashboard.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/manage_dashboard.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/manage_event_defs.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/manage_event_defs.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/manage_project.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/manage_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,16 +123,16 @@
         date_partition_field=(
             all_fields[date_partition_col] if date_partition_col else None
         ),
     )
 
 
 @restricted_layout
-def layout_create() -> bc.Component:
-    return layout(None)
+def layout_create(**query_params) -> bc.Component:
+    return layout(None, **query_params)
 
 
 @restricted_layout
 def layout(project_id: Optional[str] = None, **query_params) -> bc.Component:
     project: Optional[M.Project] = None
     dependencies: DEPS.Dependencies = cast(
         DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
@@ -158,15 +158,15 @@
                                     title, id=PROJECT_TITLE, className="card-title"
                                 ),
                                 width="auto",
                             )
                         ]
                     ),
                     html.Hr(),
-                    MPC.create_project_settings(project, dependencies),
+                    MPC.create_project_settings(project, dependencies, **query_params),
                     html.Hr(),
                     dbc.Button(
                         [html.B(className="bi bi-check-circle"), " Save"],
                         color="success",
                         id=SAVE_BUTTON,
                         class_name="d-inline-block me-3 mb-1",
                     ),
```

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/manage_saved_metrics.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/manage_saved_metrics.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/paths.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/paths.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/projects/event_tables_config.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/projects/event_tables_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -667,15 +667,16 @@
                 connection=connection,
                 event_data_tables=[],
                 project_name="dummy_project",
             )
             adapter = dummy_project.get_adapter()
 
             tables = [
-                {"label": s, "value": s} for s in adapter.list_tables(schema=schema)
+                {"label": s, "value": s}
+                for s in sorted(adapter.list_tables(schema=schema))
             ]
             return (tables, [], "Choose tables to add")
         except Exception as exc:
             traceback.print_exc()
             return ([], [], f"Something went wrong: {exc}")
     return ([], [], "Connection must be set first!")
```

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/projects/helper.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/projects/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/projects/manage_project_component.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/projects/manage_project_component.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 PROP_EXPLORE_AUTO_REFRESH = "auto_refresh"
 PROP_END_DATE_CONFIG = "default_end_date_config"
 PROP_CUSTOM_END_DATE_CONFIG = "custom_default_end_date"
 
 
 def create_project_settings(
-    project: Optional[M.Project], dependencies: DEPS.Dependencies
+    project: Optional[M.Project], dependencies: DEPS.Dependencies, **query_args
 ) -> bc.Component:
     return html.Div(
         [
             dbc.Form(
                 children=[
                     dbc.Accordion(
                         children=[
@@ -44,15 +44,15 @@
                                         [
                                             html.I(className="bi bi-gear me-1"),
                                             "Setup your project:",
                                         ],
                                         className="mb-3 lead",
                                     ),
                                     create_basic_project_settings(
-                                        project, dependencies
+                                        project, dependencies, **query_args
                                     ),
                                 ],
                                 title="Project Settings",
                             ),
                             dbc.AccordionItem(
                                 create_explore_settings(project),
                                 title="Explore Settings",
@@ -71,20 +71,25 @@
                 class_name="mt-3 ",
             ),
         ],
     )
 
 
 def create_basic_project_settings(
-    project: Optional[M.Project], dependencies: DEPS.Dependencies
+    project: Optional[M.Project], dependencies: DEPS.Dependencies, **query_args
 ) -> bc.Component:
     if project is not None:
         project_name = project.project_name
+        connection_id = project.connection.id
     else:
         project_name = None
+        connection_id = None
+
+    if connection_id is None:
+        connection_id = query_args.get("connection_id", None)
 
     con_ids = dependencies.storage.list_connections()
     connections = [dependencies.storage.get_connection(c_id) for c_id in con_ids]
     con_options = [{"label": c.connection_name, "value": c.id} for c in connections]
 
     return html.Div(
         [
@@ -108,15 +113,15 @@
                 maxlength=100,
             ),
             create_form_property_input(
                 property=PROP_CONNECTION,
                 index_type=PROJECT_INDEX_TYPE,
                 icon_cls="bi bi-link",
                 component_type=dmc.Select,
-                value=(project.connection.id if project is not None else None),
+                value=(connection_id),
                 data=con_options,
                 size="xs",
                 required=True,
             ),
             dbc.Row(
                 [
                     dbc.Col("", lg=3, sm=12, class_name="m-0"),
```

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/projects_page.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/projects_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/pages/users.py` & `mitzu-0.6.0rc2/mitzu/webapp/pages/users.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,20 +68,16 @@
     )
 
 
 @restricted_layout
 def layout(**query_params) -> bc.Component:
     deps = cast(DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY))
     user_service = deps.user_service
-    if user_service is None:
-        raise ValueError("User service is not set")
 
     authorizer = deps.authorizer
-    if authorizer is None:
-        raise ValueError("Authorizer is not set")
 
     is_admin = authorizer.get_current_user_role(flask.request) == WM.Role.ADMIN
 
     table = create_users_table(user_service)
 
     return html.Div(
         [
```

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/service/events_service.py` & `mitzu-0.6.0rc2/mitzu/webapp/service/events_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/service/navbar_service.py` & `mitzu-0.6.0rc2/mitzu/webapp/service/navbar_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,17 +81,14 @@
                 DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
             ).authorizer
 
             storage = cast(
                 DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
             ).storage
 
-            if authorizer is None:
-                return None
-
             user_id = authorizer.get_current_user_id()
             if user_id is None:
                 return None
 
             email = None
             if storage:
                 user = storage.get_user_by_id(user_id)
```

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/service/secret_service.py` & `mitzu-0.6.0rc2/mitzu/webapp/service/secret_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/service/user_service.py` & `mitzu-0.6.0rc2/mitzu/webapp/service/user_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/storage.py` & `mitzu-0.6.0rc2/mitzu/webapp/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,38 +75,53 @@
 
 class MitzuStorage:
     def __init__(
         self,
         connection_string: str = "sqlite://?check_same_thread=False",
     ) -> None:
         self._engine = SA.create_engine(connection_string)
-        if connection_string.startswith("sqlite"):
-            with self._engine.connect() as connection:
-                connection.execute("PRAGMA foreign_keys = ON;")
+        self._is_sqlite = connection_string.startswith("sqlite")
         self.__init_schema()
 
     @property
     def _session(self) -> Session:
         if flask.has_app_context():
             if "request_session_cache" not in flask.g:
                 session = SA.orm.sessionmaker(bind=self._engine)()
-                session.execute("PRAGMA foreign_keys = ON;")
-                session.commit()
+                if self._is_sqlite:
+                    session.execute("PRAGMA foreign_keys = ON;")
+                    session.commit()
                 flask.g.request_session_cache = session
                 return session
             else:
                 return flask.g.request_session_cache
         else:
             session = SA.orm.sessionmaker(bind=self._engine)()
-            session.execute("PRAGMA foreign_keys = ON;")
-            session.commit()
+            if self._is_sqlite:
+                session.execute("PRAGMA foreign_keys = ON;")
+                session.commit()
             return session
 
     def __init_schema(self):
-        SM.Base.metadata.create_all(self._engine)
+        tables = []
+        for storage_record in [
+            SM.UserStorageRecord,
+            SM.DiscoverySettingsStorageRecord,
+            SM.WebappSettingsStorageRecord,
+            SM.ConnectionStorageRecord,
+            SM.ProjectStorageRecord,
+            SM.EventDataTableStorageRecord,
+            SM.EventDefStorageRecord,
+            SM.SavedMetricStorageRecord,
+            SM.DashboardStorageRecord,
+            SM.DashboardMetricStorageRecord,
+        ]:
+            tables.append(SM.Base.metadata.tables[storage_record.__tablename__])
+
+        SM.Base.metadata.create_all(self._engine, tables=tables)
 
     def set_project(self, project_id: str, project: M.Project):
         self.set_connection(project.connection.id, project.connection)
         self.set_discovery_settings(
             project.discovery_settings.id, project.discovery_settings
         )
         self.set_webapp_settings(project.webapp_settings.id, project.webapp_settings)
```

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/storage_model.py` & `mitzu-0.6.0rc2/mitzu/webapp/storage_model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/toast.py` & `mitzu-0.6.0rc2/mitzu/webapp/toast.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc1/mitzu/webapp/webapp.py` & `mitzu-0.6.0rc2/mitzu/webapp/webapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,27 +59,25 @@
 
 
 def create_dash_app(dependencies: Optional[DEPS.Dependencies] = None) -> Dash:
     server = flask.Flask(__name__)
     if dependencies is None:
         dependencies = DEPS.Dependencies.from_configs()
 
-    if dependencies.authorizer is not None:
-
-        @server.before_request
-        def before_request():
-            request = flask.request
-            return dependencies.authorizer.authorize_request(request)
-
-        @server.after_request
-        def after_request(response: flask.Response):
-            request = flask.request
-            if dependencies is not None and dependencies.authorizer is not None:
-                return dependencies.authorizer.refresh_auth_token(request, response)
-            return response
+    @server.before_request
+    def before_request():
+        request = flask.request
+        return dependencies.authorizer.authorize_request(request)
+
+    @server.after_request
+    def after_request(response: flask.Response):
+        request = flask.request
+        if dependencies is not None:
+            return dependencies.authorizer.refresh_auth_token(request, response)
+        return response
 
     with server.app_context():
         flask.current_app.config[DEPS.CONFIG_KEY] = dependencies
         if configs.SETUP_SAMPLE_PROJECT:
             S.setup_sample_project(dependencies.storage)
 
     dependencies.navbar_service.register_navbar_item_provider(
```

### Comparing `mitzu-0.6.0rc1/pyproject.toml` & `mitzu-0.6.0rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mitzu"
-version = "0.6.0-rc.1"
+version = "0.6.0-rc.2"
 description = "Product analytics over your data warehouse"
 authors = ["Istvan Meszaros <istvan.meszaros.88@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mitzu.io"
 repository = "https://github.com/mitzu-io/mitzu"
 documentation = "https://mitzu.io/documentation/"
```

### Comparing `mitzu-0.6.0rc1/PKG-INFO` & `mitzu-0.6.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitzu
-Version: 0.6.0rc1
+Version: 0.6.0rc2
 Summary: Product analytics over your data warehouse
 Home-page: https://mitzu.io
 License: MIT
 Author: Istvan Meszaros
 Author-email: istvan.meszaros.88@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

