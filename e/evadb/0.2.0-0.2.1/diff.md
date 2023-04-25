# Comparing `tmp/evadb-0.2.0.tar.gz` & `tmp/evadb-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evadb-0.2.0.tar", last modified: Mon Apr 17 14:50:18 2023, max compression
+gzip compressed data, was "evadb-0.2.1.tar", last modified: Tue Apr 25 13:20:56 2023, max compression
```

## Comparing `evadb-0.2.0.tar` & `evadb-0.2.1.tar`

### file list

```diff
@@ -1,461 +1,461 @@
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.503700 evadb-0.2.0/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    11357 2023-04-02 17:27:27.000000 evadb-0.2.0/LICENSE.txt
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12958 2023-04-17 14:50:18.503700 evadb-0.2.0/PKG-INFO
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10710 2023-04-02 17:27:27.000000 evadb-0.2.0/README.md
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.459699 evadb-0.2.0/eva/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      645 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.463699 evadb-0.2.0/eva/binder/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/binder/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4937 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/binder/binder_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12003 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/binder/statement_binder.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8000 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/binder/statement_binder_context.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.463699 evadb-0.2.0/eva/catalog/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    17810 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/catalog/catalog_manager.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3076 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/catalog/catalog_type.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5695 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/catalog/catalog_utils.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.463699 evadb-0.2.0/eva/catalog/models/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      886 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/models/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1499 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/models/association_models.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3752 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/models/base_model.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5110 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/models/column_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3274 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/models/index_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2997 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/models/table_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3532 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/models/udf_cache_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4429 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/catalog/models/udf_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2262 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/models/udf_cost_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4722 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/models/udf_io_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2668 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/models/udf_metadata_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2127 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/schema_utils.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.463699 evadb-0.2.0/eva/catalog/services/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/services/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1167 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/services/base_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2873 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/services/column_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2887 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/services/index_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4571 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/services/table_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3669 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/services/udf_cache_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3078 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/services/udf_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2826 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/services/udf_cost_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2476 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/services/udf_io_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1936 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/catalog/services/udf_metadata_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2857 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/catalog/sql_config.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.463699 evadb-0.2.0/eva/configuration/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/configuration/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4025 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/configuration/bootstrap_environment.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4374 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/configuration/configuration_manager.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1402 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/configuration/constants.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      840 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/constants.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      756 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/eva.yml
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1553 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/eva_cmd_client.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2399 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/eva_server.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.467699 evadb-0.2.0/eva/executor/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      615 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2137 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/abstract_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2214 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/executor/apply_and_merge_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1418 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/create_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5728 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/create_index_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3866 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/create_mat_view_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4777 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/executor/create_udf_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4738 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/delete_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2504 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/drop_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2010 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/drop_udf_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3013 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/executor/execution_context.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3043 2023-04-06 17:08:11.000000 evadb-0.2.0/eva/executor/executor_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1523 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/explain_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3507 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/executor/faiss_index_scan_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1591 2023-04-06 17:08:11.000000 evadb-0.2.0/eva/executor/function_scan_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1759 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/executor/groupby_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1800 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/hash_join_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2255 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/insert_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1616 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/join_build_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1661 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/lateral_join_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1583 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/executor/limit_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3086 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/load_csv_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1579 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/load_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4944 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/load_multimedia_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1488 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/executor/nested_loop_join_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4183 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/executor/orderby_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8071 2023-04-06 17:08:11.000000 evadb-0.2.0/eva/executor/plan_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1644 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/pp_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1277 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/executor/predicate_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1272 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/project_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1186 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/rename_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1413 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/sample_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1812 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/seq_scan_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1870 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/show_info_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2274 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/executor/storage_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1264 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/executor/union_executor.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.467699 evadb-0.2.0/eva/experimental/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      619 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/experimental/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.467699 evadb-0.2.0/eva/experimental/ray/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      610 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/experimental/ray/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.467699 evadb-0.2.0/eva/experimental/ray/executor/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      619 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/experimental/ray/executor/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3521 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/experimental/ray/executor/exchange_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1431 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/experimental/ray/executor/ray_stage.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.467699 evadb-0.2.0/eva/experimental/ray/optimizer/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/experimental/ray/optimizer/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.467699 evadb-0.2.0/eva/experimental/ray/optimizer/rules/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      626 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/experimental/ray/optimizer/rules/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4176 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/experimental/ray/optimizer/rules/rules.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.471699 evadb-0.2.0/eva/experimental/ray/planner/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      618 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/experimental/ray/planner/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1380 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/experimental/ray/planner/exchange_plan.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.471699 evadb-0.2.0/eva/expression/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      617 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/expression/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5469 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/expression/abstract_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3974 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/expression/aggregation_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1618 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/expression/arithmetic_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4351 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/expression/comparison_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2542 2023-04-13 06:13:25.000000 evadb-0.2.0/eva/expression/constant_value_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10440 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/expression/expression_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10151 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/expression/function_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3055 2023-04-17 01:45:56.000000 evadb-0.2.0/eva/expression/logical_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4685 2023-04-13 06:13:17.000000 evadb-0.2.0/eva/expression/tuple_value_expression.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.471699 evadb-0.2.0/eva/models/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      633 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/models/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.471699 evadb-0.2.0/eva/models/catalog/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/models/catalog/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1332 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/models/catalog/frame_info.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      857 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/models/catalog/properties.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.471699 evadb-0.2.0/eva/models/server/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/models/server/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1809 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/models/server/response.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.471699 evadb-0.2.0/eva/models/storage/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/models/storage/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    14837 2023-04-06 16:06:01.000000 evadb-0.2.0/eva/models/storage/batch.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.471699 evadb-0.2.0/eva/optimizer/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3260 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/binder.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2129 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/cost_model.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3450 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/group.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2669 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/group_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4335 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/memo.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    35842 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/optimizer/operators.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3838 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/optimizer_context.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      982 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/optimizer_task_stack.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12579 2023-04-06 17:08:11.000000 evadb-0.2.0/eva/optimizer/optimizer_tasks.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10128 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/optimizer_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5700 2023-04-06 17:08:11.000000 evadb-0.2.0/eva/optimizer/plan_generator.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1169 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/property.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.475699 evadb-0.2.0/eva/optimizer/rules/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/rules/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1016 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/optimizer/rules/pattern.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    41137 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/optimizer/rules/rules.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7023 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/optimizer/rules/rules_base.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7573 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/optimizer/rules/rules_manager.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13132 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/optimizer/statement_to_opr_convertor.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.475699 evadb-0.2.0/eva/parser/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1360 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/alias.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2672 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/create_index_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2788 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/create_mat_view_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4838 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/create_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4882 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/parser/create_udf_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2048 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/delete_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1767 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/drop_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1793 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/drop_udf_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    19228 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/parser/eva.lark
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.475699 evadb-0.2.0/eva/parser/evaql/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    65109 2022-12-14 06:32:03.000000 evadb-0.2.0/eva/parser/evaql/evaql_lexer.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)   408798 2022-12-14 06:32:04.000000 evadb-0.2.0/eva/parser/evaql/evaql_parser.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    44890 2022-12-14 06:32:04.000000 evadb-0.2.0/eva/parser/evaql/evaql_parserListener.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    26541 2022-12-14 06:32:04.000000 evadb-0.2.0/eva/parser/evaql/evaql_parserVisitor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1384 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/explain_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2922 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/insert_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1717 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_parser.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.479699 evadb-0.2.0/eva/parser/lark_visitor/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2655 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2150 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_common_clauses_ids.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10304 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_create_statements.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1404 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_delete_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1202 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_drop_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1006 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_explain_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4672 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_expressions.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5959 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_functions.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2465 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_insert_statements.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2057 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_load_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      932 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_rename_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2121 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_select_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1091 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_show_statements.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     9468 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/lark_visitor/_table_sources.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3214 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/load_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1228 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/parser.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2007 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/rename_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5921 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/select_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1460 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/show_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1052 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/parser/statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8639 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/parser/table_ref.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1679 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/parser/types.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.483699 evadb-0.2.0/eva/plan_nodes/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      614 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1689 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/abstract_join_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3453 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/plan_nodes/abstract_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1455 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/abstract_scan_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1930 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/apply_and_merge_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2401 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/create_index_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2076 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/create_mat_view_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2200 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/create_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3603 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/create_udf_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1951 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/delete_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1660 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/drop_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1532 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/drop_udf_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1033 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/explain_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2355 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/faiss_index_scan_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1755 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/function_scan_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1499 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/groupby_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1712 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/hash_join_build_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2179 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/hash_join_probe_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2023 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/insert_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1408 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/lateral_join_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1468 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/limit_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2710 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/load_data_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1510 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/nested_loop_join_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1564 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/orderby_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1177 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/pp_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1245 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/predicate_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1249 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/project_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1616 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/rename_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1469 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/sample_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1760 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/seq_scan_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1201 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/show_info_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4419 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/plan_nodes/storage_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1420 2023-04-05 18:07:02.000000 evadb-0.2.0/eva/plan_nodes/types.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1245 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/plan_nodes/union_plan.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.483699 evadb-0.2.0/eva/readers/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/readers/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2320 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/readers/abstract_reader.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2651 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/readers/csv_reader.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5617 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/readers/decord_reader.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.483699 evadb-0.2.0/eva/readers/image/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/readers/image/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1007 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/readers/image/opencv_image_reader.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.483699 evadb-0.2.0/eva/server/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      623 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/server/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3284 2023-04-03 16:26:49.000000 evadb-0.2.0/eva/server/command_handler.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3502 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/server/db_api.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3276 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/server/interpreter.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2866 2023-04-06 05:12:11.000000 evadb-0.2.0/eva/server/server.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.483699 evadb-0.2.0/eva/storage/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/storage/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5659 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/storage/abstract_media_storage_engine.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2385 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/storage/abstract_storage_engine.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1694 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/storage/image_storage_engine.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8881 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/storage/sqlite_storage_engine.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1688 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/storage/storage_engine.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2243 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/storage/video_storage_engine.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.483699 evadb-0.2.0/eva/third_party/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      605 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/third_party/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.483699 evadb-0.2.0/eva/third_party/huggingface/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      619 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/third_party/huggingface/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1506 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/third_party/huggingface/binder.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5776 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/third_party/huggingface/create.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1453 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/third_party/huggingface/model.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.487700 evadb-0.2.0/eva/udfs/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.487700 evadb-0.2.0/eva/udfs/abstract/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      625 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/abstract/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2441 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/abstract/abstract_udf.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3096 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/udfs/abstract/hf_abstract_udf.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3843 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/abstract/pytorch_abstract_udf.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3464 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/asl_action_recognition.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.487700 evadb-0.2.0/eva/udfs/decorators/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/decorators/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2185 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/decorators/decorators.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.487700 evadb-0.2.0/eva/udfs/decorators/io_descriptors/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/decorators/io_descriptors/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2754 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/decorators/io_descriptors/abstract_types.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3375 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/decorators/io_descriptors/data_types.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1437 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/udfs/decorators/utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5675 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/decorators/yolo_object_detection_decorators.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5478 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/emotion_detector.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2539 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/face_detector.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5110 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/fastrcnn_object_detector.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1822 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/feature_extractor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1028 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/gpu_compatible.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2200 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/mvit_action_recognition.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.487700 evadb-0.2.0/eva/udfs/ndarray/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      638 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/ndarray/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2568 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/ndarray/array_count.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1647 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/ndarray/crop.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1179 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/ndarray/fuzzy_join.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1557 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/ndarray/open.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1782 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/ndarray/similarity.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2750 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/ocr_extractor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2471 2023-04-05 15:01:02.000000 evadb-0.2.0/eva/udfs/toxicity_classifier.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6764 2023-04-12 18:47:51.000000 evadb-0.2.0/eva/udfs/udf_bootstrap_queries.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5043 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/udfs/yolo_object_detector.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.487700 evadb-0.2.0/eva/utils/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      611 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/utils/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      909 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/utils/errors.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6957 2023-04-13 06:12:12.000000 evadb-0.2.0/eva/utils/generic_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1837 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/utils/kv_cache.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      985 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/utils/logging_manager.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1562 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/utils/s3_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1692 2023-04-02 17:27:27.000000 evadb-0.2.0/eva/utils/stats.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      711 2023-04-17 02:39:30.000000 evadb-0.2.0/eva/version.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.487700 evadb-0.2.0/evadb.egg-info/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12958 2023-04-17 14:50:18.000000 evadb-0.2.0/evadb.egg-info/PKG-INFO
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13538 2023-04-17 14:50:18.000000 evadb-0.2.0/evadb.egg-info/SOURCES.txt
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)        1 2023-04-17 14:50:18.000000 evadb-0.2.0/evadb.egg-info/dependency_links.txt
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       89 2023-04-17 14:50:18.000000 evadb-0.2.0/evadb.egg-info/entry_points.txt
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1087 2023-04-17 14:50:18.000000 evadb-0.2.0/evadb.egg-info/requires.txt
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       21 2023-04-17 14:50:18.000000 evadb-0.2.0/evadb.egg-info/top_level.txt
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       90 2023-04-02 17:27:27.000000 evadb-0.2.0/pyproject.toml
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       38 2023-04-17 14:50:18.503700 evadb-0.2.0/setup.cfg
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4093 2023-04-13 06:12:12.000000 evadb-0.2.0/setup.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.491700 evadb-0.2.0/test/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.491700 evadb-0.2.0/test/benchmark_tests/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/benchmark_tests/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1172 2023-04-02 17:27:27.000000 evadb-0.2.0/test/benchmark_tests/conftest.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3294 2023-04-02 17:27:27.000000 evadb-0.2.0/test/benchmark_tests/test_benchmark_pytorch.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.491700 evadb-0.2.0/test/binder/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/binder/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2032 2023-04-02 17:27:27.000000 evadb-0.2.0/test/binder/test_binder_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    14016 2023-04-02 17:27:27.000000 evadb-0.2.0/test/binder/test_statement_binder.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7961 2023-04-02 17:27:27.000000 evadb-0.2.0/test/binder/test_statement_binder_context.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1796 2023-04-02 17:27:27.000000 evadb-0.2.0/test/binder/test_statement_binder_python37.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.491700 evadb-0.2.0/test/catalog/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.491700 evadb-0.2.0/test/catalog/models/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/models/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7234 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/models/test_models.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.491700 evadb-0.2.0/test/catalog/services/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/services/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1918 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/services/test_column_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4745 2023-04-13 06:12:12.000000 evadb-0.2.0/test/catalog/services/test_index_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3639 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/services/test_table_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3639 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/services/test_udf_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3210 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/services/test_udf_cost_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3035 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/services/test_udf_io_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7560 2023-04-05 15:01:02.000000 evadb-0.2.0/test/catalog/test_catalog_manager.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1402 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/test_column_type.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1910 2023-04-02 17:27:27.000000 evadb-0.2.0/test/catalog/test_sqlalchemy.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.491700 evadb-0.2.0/test/configuration/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/configuration/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1490 2023-04-02 17:27:27.000000 evadb-0.2.0/test/configuration/test_bootstrap_environment.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1690 2023-04-02 17:27:27.000000 evadb-0.2.0/test/configuration/test_configuration_manager.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.495700 evadb-0.2.0/test/executor/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1106 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/test_abstract_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2441 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/test_create_mat_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3987 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/test_create_udf_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4227 2023-04-06 05:12:11.000000 evadb-0.2.0/test/executor/test_execution_context.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1275 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/test_executor_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4650 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/test_limit_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3890 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/test_load_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2884 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/test_orderby_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10986 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/test_plan_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1397 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/test_pp_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1817 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/test_sample_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2752 2023-04-06 17:08:11.000000 evadb-0.2.0/test/executor/test_seq_scan_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      847 2023-04-02 17:27:27.000000 evadb-0.2.0/test/executor/utils.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.495700 evadb-0.2.0/test/expression/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/expression/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3722 2023-04-02 17:27:27.000000 evadb-0.2.0/test/expression/test_abstract_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5149 2023-04-02 17:27:27.000000 evadb-0.2.0/test/expression/test_aggregation.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2975 2023-04-02 17:27:27.000000 evadb-0.2.0/test/expression/test_arithmetic.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5578 2023-04-02 17:27:27.000000 evadb-0.2.0/test/expression/test_comparison.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2867 2023-04-02 17:27:27.000000 evadb-0.2.0/test/expression/test_expression_tree.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7555 2023-04-02 17:27:27.000000 evadb-0.2.0/test/expression/test_expression_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2685 2023-04-02 17:27:27.000000 evadb-0.2.0/test/expression/test_function_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10242 2023-04-13 06:25:00.000000 evadb-0.2.0/test/expression/test_logical.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.495700 evadb-0.2.0/test/integration_tests/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/integration_tests/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3587 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_array_count.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7647 2023-04-02 17:27:27.000000 evadb-0.2.0/test/integration_tests/test_create_index_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1091 2023-04-02 17:27:27.000000 evadb-0.2.0/test/integration_tests/test_create_table_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5160 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_delete_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4839 2023-04-05 15:01:02.000000 evadb-0.2.0/test/integration_tests/test_drop_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2454 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_error_handling_with_ray.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4088 2023-04-13 06:12:12.000000 evadb-0.2.0/test/integration_tests/test_explain_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3183 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_fuzzy_join.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7790 2023-04-13 06:12:12.000000 evadb-0.2.0/test/integration_tests/test_huggingface_udfs.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3896 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_insert_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2956 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_like.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    19262 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_load_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5233 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_mat_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2660 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_open.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10184 2023-04-12 18:47:51.000000 evadb-0.2.0/test/integration_tests/test_optimizer_rules.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12724 2023-04-12 18:47:51.000000 evadb-0.2.0/test/integration_tests/test_pytorch.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2953 2023-04-02 17:27:27.000000 evadb-0.2.0/test/integration_tests/test_rename_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7580 2023-04-12 18:47:51.000000 evadb-0.2.0/test/integration_tests/test_reuse.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5210 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_s3_load_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    29003 2023-04-06 17:08:11.000000 evadb-0.2.0/test/integration_tests/test_select_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3873 2023-04-13 06:12:12.000000 evadb-0.2.0/test/integration_tests/test_show_info_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12289 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_similarity.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12062 2023-04-06 05:12:11.000000 evadb-0.2.0/test/integration_tests/test_udf_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      852 2023-04-02 17:27:27.000000 evadb-0.2.0/test/markers.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.499700 evadb-0.2.0/test/models/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/models/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.499700 evadb-0.2.0/test/models/catalog/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/models/catalog/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1010 2023-04-02 17:27:27.000000 evadb-0.2.0/test/models/catalog/test_frame_info.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.499700 evadb-0.2.0/test/models/storage/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/models/storage/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5919 2023-04-05 15:01:02.000000 evadb-0.2.0/test/models/storage/test_batch.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.499700 evadb-0.2.0/test/optimizer/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/optimizer/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.499700 evadb-0.2.0/test/optimizer/rules/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/optimizer/rules/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    11728 2023-04-12 18:47:51.000000 evadb-0.2.0/test/optimizer/rules/test_rules.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4195 2023-04-02 17:27:27.000000 evadb-0.2.0/test/optimizer/test_binder.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4377 2023-04-06 05:12:11.000000 evadb-0.2.0/test/optimizer/test_cascade_optimizer.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4406 2023-04-02 17:27:27.000000 evadb-0.2.0/test/optimizer/test_cost_model.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2689 2023-04-02 17:27:27.000000 evadb-0.2.0/test/optimizer/test_group.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1996 2023-04-02 17:27:27.000000 evadb-0.2.0/test/optimizer/test_memo.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1034 2023-04-02 17:27:27.000000 evadb-0.2.0/test/optimizer/test_optimizer_context.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6122 2023-04-13 06:12:12.000000 evadb-0.2.0/test/optimizer/test_optimizer_task.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2000 2023-04-02 17:27:27.000000 evadb-0.2.0/test/optimizer/test_optimizer_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13335 2023-04-12 18:47:51.000000 evadb-0.2.0/test/optimizer/test_statement_to_opr_convertor.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.499700 evadb-0.2.0/test/parser/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/parser/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    36051 2023-04-02 17:27:27.000000 evadb-0.2.0/test/parser/test_parser.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4843 2023-04-02 17:27:27.000000 evadb-0.2.0/test/parser/test_parser_statements.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.499700 evadb-0.2.0/test/plan_nodes/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/plan_nodes/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6292 2023-04-02 17:27:27.000000 evadb-0.2.0/test/plan_nodes/test_plan.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.499700 evadb-0.2.0/test/readers/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/readers/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1688 2023-04-02 17:27:27.000000 evadb-0.2.0/test/readers/test_csv_reader.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7288 2023-04-05 15:01:02.000000 evadb-0.2.0/test/readers/test_decord_reader.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.499700 evadb-0.2.0/test/server/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/server/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1268 2023-04-02 17:27:27.000000 evadb-0.2.0/test/server/test_command_handler.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5057 2023-04-02 17:27:27.000000 evadb-0.2.0/test/server/test_db_api.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2581 2023-04-02 17:27:27.000000 evadb-0.2.0/test/server/test_interpreter.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2066 2023-04-02 17:27:27.000000 evadb-0.2.0/test/server/test_server.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.499700 evadb-0.2.0/test/storage/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/storage/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4001 2023-04-02 17:27:27.000000 evadb-0.2.0/test/storage/test_sqlite_storage_engine.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4023 2023-04-02 17:27:27.000000 evadb-0.2.0/test/storage/test_video_storage.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1801 2023-04-02 17:27:27.000000 evadb-0.2.0/test/test_eva_cmd_client.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1294 2023-04-02 17:27:27.000000 evadb-0.2.0/test/test_eva_imports.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1810 2023-04-02 17:27:27.000000 evadb-0.2.0/test/test_eva_server.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.503700 evadb-0.2.0/test/udfs/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      638 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.503700 evadb-0.2.0/test/udfs/decorators/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/decorators/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.503700 evadb-0.2.0/test/udfs/decorators/io_descriptors/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/decorators/io_descriptors/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7430 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/decorators/io_descriptors/test_descriptors.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2134 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/decorators/test_decorators.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.503700 evadb-0.2.0/test/udfs/ndarray/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      648 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/ndarray/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      849 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/ndarray/test_array_count.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2410 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/ndarray/test_crop.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2374 2023-04-13 06:12:12.000000 evadb-0.2.0/test/udfs/ndarray/test_open.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4330 2023-04-13 06:12:12.000000 evadb-0.2.0/test/udfs/test_abstract_udf.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2154 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/test_emotion_detector.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3345 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/test_facenet_udf.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2548 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/test_fastrcnn_object_detector.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2689 2023-04-02 17:27:27.000000 evadb-0.2.0/test/udfs/test_yolo_object_detector.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    16108 2023-04-13 06:12:12.000000 evadb-0.2.0/test/util.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.503700 evadb-0.2.0/test/utils/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.0/test/utils/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4196 2023-04-13 06:12:12.000000 evadb-0.2.0/test/utils/test_generic_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2256 2023-04-02 17:27:27.000000 evadb-0.2.0/test/utils/test_timer.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2181 2023-04-13 06:12:12.000000 evadb-0.2.0/test/utils/test_xdist.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-17 14:50:18.503700 evadb-0.2.0/third_party/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-02 17:27:27.000000 evadb-0.2.0/third_party/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.094514 evadb-0.2.1/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    11357 2023-04-02 17:27:27.000000 evadb-0.2.1/LICENSE.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    15197 2023-04-25 13:20:56.094514 evadb-0.2.1/PKG-INFO
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12629 2023-04-24 23:48:03.000000 evadb-0.2.1/README.md
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.046513 evadb-0.2.1/eva/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      645 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.050513 evadb-0.2.1/eva/binder/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/binder/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4937 2023-04-12 18:47:51.000000 evadb-0.2.1/eva/binder/binder_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12003 2023-04-13 06:12:12.000000 evadb-0.2.1/eva/binder/statement_binder.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8000 2023-04-05 15:01:02.000000 evadb-0.2.1/eva/binder/statement_binder_context.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.050513 evadb-0.2.1/eva/catalog/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    17810 2023-04-05 15:01:02.000000 evadb-0.2.1/eva/catalog/catalog_manager.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3076 2023-04-05 15:01:02.000000 evadb-0.2.1/eva/catalog/catalog_type.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5695 2023-04-05 15:01:02.000000 evadb-0.2.1/eva/catalog/catalog_utils.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.050513 evadb-0.2.1/eva/catalog/models/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      886 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/models/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1499 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/models/association_models.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3752 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/models/base_model.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5110 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/models/column_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3274 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/models/index_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2997 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/models/table_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3532 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/models/udf_cache_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4429 2023-04-13 06:12:12.000000 evadb-0.2.1/eva/catalog/models/udf_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2262 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/models/udf_cost_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4722 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/models/udf_io_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2668 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/models/udf_metadata_catalog.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2127 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/schema_utils.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.050513 evadb-0.2.1/eva/catalog/services/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/services/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1167 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/services/base_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2873 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/services/column_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2887 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/services/index_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4571 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/services/table_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3669 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/services/udf_cache_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3078 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/services/udf_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2826 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/services/udf_cost_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2476 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/services/udf_io_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1936 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/catalog/services/udf_metadata_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2857 2023-04-13 06:12:12.000000 evadb-0.2.1/eva/catalog/sql_config.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.050513 evadb-0.2.1/eva/configuration/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/configuration/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4025 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/configuration/bootstrap_environment.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4374 2023-04-13 06:12:12.000000 evadb-0.2.1/eva/configuration/configuration_manager.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1402 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/configuration/constants.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      840 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/constants.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      756 2023-04-06 05:12:11.000000 evadb-0.2.1/eva/eva.yml
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1553 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/eva_cmd_client.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2399 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/eva_server.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.054513 evadb-0.2.1/eva/executor/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      615 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2137 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/abstract_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2214 2023-04-12 18:47:51.000000 evadb-0.2.1/eva/executor/apply_and_merge_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1418 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/create_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5728 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/create_index_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3866 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/create_mat_view_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4777 2023-04-13 06:12:12.000000 evadb-0.2.1/eva/executor/create_udf_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4738 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/delete_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2504 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/drop_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2010 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/drop_udf_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3013 2023-04-06 05:12:11.000000 evadb-0.2.1/eva/executor/execution_context.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3043 2023-04-06 17:08:11.000000 evadb-0.2.1/eva/executor/executor_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1523 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/explain_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3507 2023-04-06 05:12:11.000000 evadb-0.2.1/eva/executor/faiss_index_scan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1591 2023-04-06 17:08:11.000000 evadb-0.2.1/eva/executor/function_scan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1759 2023-04-06 05:12:11.000000 evadb-0.2.1/eva/executor/groupby_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1800 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/hash_join_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2255 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/insert_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1616 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/join_build_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1661 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/lateral_join_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1583 2023-04-06 05:12:11.000000 evadb-0.2.1/eva/executor/limit_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3086 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/load_csv_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1579 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/load_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4944 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/load_multimedia_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1488 2023-04-06 05:12:11.000000 evadb-0.2.1/eva/executor/nested_loop_join_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4183 2023-04-06 05:12:11.000000 evadb-0.2.1/eva/executor/orderby_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8071 2023-04-06 17:08:11.000000 evadb-0.2.1/eva/executor/plan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1644 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/pp_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1277 2023-04-06 05:12:11.000000 evadb-0.2.1/eva/executor/predicate_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1272 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/project_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1186 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/rename_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1413 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/sample_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1812 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/seq_scan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1870 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/show_info_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2274 2023-04-05 15:01:02.000000 evadb-0.2.1/eva/executor/storage_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1264 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/executor/union_executor.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.054513 evadb-0.2.1/eva/experimental/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      619 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/experimental/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.058513 evadb-0.2.1/eva/experimental/ray/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      610 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/experimental/ray/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.058513 evadb-0.2.1/eva/experimental/ray/executor/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      619 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/experimental/ray/executor/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3521 2023-04-06 05:12:11.000000 evadb-0.2.1/eva/experimental/ray/executor/exchange_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1431 2023-04-06 05:12:11.000000 evadb-0.2.1/eva/experimental/ray/executor/ray_stage.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.058513 evadb-0.2.1/eva/experimental/ray/optimizer/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/experimental/ray/optimizer/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.058513 evadb-0.2.1/eva/experimental/ray/optimizer/rules/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      626 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/experimental/ray/optimizer/rules/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4176 2023-04-06 05:12:11.000000 evadb-0.2.1/eva/experimental/ray/optimizer/rules/rules.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.058513 evadb-0.2.1/eva/experimental/ray/planner/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      618 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/experimental/ray/planner/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1380 2023-04-06 05:12:11.000000 evadb-0.2.1/eva/experimental/ray/planner/exchange_plan.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.058513 evadb-0.2.1/eva/expression/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      617 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/expression/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5469 2023-04-12 18:47:51.000000 evadb-0.2.1/eva/expression/abstract_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3974 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/expression/aggregation_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1618 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/expression/arithmetic_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4351 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/expression/comparison_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2542 2023-04-13 06:13:25.000000 evadb-0.2.1/eva/expression/constant_value_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10440 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/expression/expression_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10151 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/expression/function_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3055 2023-04-17 01:45:56.000000 evadb-0.2.1/eva/expression/logical_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4685 2023-04-13 06:13:17.000000 evadb-0.2.1/eva/expression/tuple_value_expression.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.058513 evadb-0.2.1/eva/models/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      633 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/models/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.058513 evadb-0.2.1/eva/models/catalog/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/models/catalog/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1332 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/models/catalog/frame_info.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      857 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/models/catalog/properties.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.058513 evadb-0.2.1/eva/models/server/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/models/server/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1809 2023-04-05 15:01:02.000000 evadb-0.2.1/eva/models/server/response.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.058513 evadb-0.2.1/eva/models/storage/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/models/storage/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    14837 2023-04-06 16:06:01.000000 evadb-0.2.1/eva/models/storage/batch.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.062513 evadb-0.2.1/eva/optimizer/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/optimizer/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3260 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/optimizer/binder.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2129 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/optimizer/cost_model.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3450 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/optimizer/group.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2669 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/optimizer/group_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4335 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/optimizer/memo.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    35842 2023-04-12 18:47:51.000000 evadb-0.2.1/eva/optimizer/operators.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3838 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/optimizer/optimizer_context.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      982 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/optimizer/optimizer_task_stack.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12579 2023-04-06 17:08:11.000000 evadb-0.2.1/eva/optimizer/optimizer_tasks.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10128 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/optimizer/optimizer_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5700 2023-04-06 17:08:11.000000 evadb-0.2.1/eva/optimizer/plan_generator.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1169 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/optimizer/property.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.062513 evadb-0.2.1/eva/optimizer/rules/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/optimizer/rules/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1016 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/optimizer/rules/pattern.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    41137 2023-04-24 23:47:21.000000 evadb-0.2.1/eva/optimizer/rules/rules.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7023 2023-04-12 18:47:51.000000 evadb-0.2.1/eva/optimizer/rules/rules_base.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7573 2023-04-12 18:47:51.000000 evadb-0.2.1/eva/optimizer/rules/rules_manager.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13132 2023-04-12 18:47:51.000000 evadb-0.2.1/eva/optimizer/statement_to_opr_convertor.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.062513 evadb-0.2.1/eva/parser/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1360 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/alias.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2672 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/create_index_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2788 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/create_mat_view_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4838 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/create_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4882 2023-04-13 06:12:12.000000 evadb-0.2.1/eva/parser/create_udf_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2048 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/delete_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1767 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/drop_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1793 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/drop_udf_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    19228 2023-04-13 06:12:12.000000 evadb-0.2.1/eva/parser/eva.lark
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.066514 evadb-0.2.1/eva/parser/evaql/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    65109 2022-12-14 06:32:03.000000 evadb-0.2.1/eva/parser/evaql/evaql_lexer.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)   408798 2022-12-14 06:32:04.000000 evadb-0.2.1/eva/parser/evaql/evaql_parser.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    44890 2022-12-14 06:32:04.000000 evadb-0.2.1/eva/parser/evaql/evaql_parserListener.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    26541 2022-12-14 06:32:04.000000 evadb-0.2.1/eva/parser/evaql/evaql_parserVisitor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1384 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/explain_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2922 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/insert_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1717 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/lark_parser.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.066514 evadb-0.2.1/eva/parser/lark_visitor/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2655 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/lark_visitor/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2150 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/lark_visitor/_common_clauses_ids.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10304 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/lark_visitor/_create_statements.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1404 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/lark_visitor/_delete_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1202 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/lark_visitor/_drop_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1006 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/lark_visitor/_explain_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4672 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/lark_visitor/_expressions.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5959 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/lark_visitor/_functions.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2465 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/lark_visitor/_insert_statements.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2057 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/lark_visitor/_load_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      932 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/lark_visitor/_rename_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2121 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/lark_visitor/_select_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1091 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/lark_visitor/_show_statements.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     9468 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/lark_visitor/_table_sources.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3214 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/load_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1228 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/parser.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2007 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/rename_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5921 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/select_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1460 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/show_statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1052 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/parser/statement.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8639 2023-04-05 15:01:02.000000 evadb-0.2.1/eva/parser/table_ref.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1679 2023-04-12 18:47:51.000000 evadb-0.2.1/eva/parser/types.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.070514 evadb-0.2.1/eva/plan_nodes/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      614 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1689 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/abstract_join_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3453 2023-04-06 05:12:11.000000 evadb-0.2.1/eva/plan_nodes/abstract_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1455 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/abstract_scan_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1930 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/apply_and_merge_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2401 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/create_index_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2076 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/create_mat_view_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2200 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/create_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3603 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/create_udf_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1951 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/delete_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1660 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/drop_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1532 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/drop_udf_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1033 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/explain_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2355 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/faiss_index_scan_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1755 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/function_scan_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1499 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/groupby_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1712 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/hash_join_build_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2179 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/hash_join_probe_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2023 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/insert_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1408 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/lateral_join_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1468 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/limit_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2710 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/load_data_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1510 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/nested_loop_join_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1564 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/orderby_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1177 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/pp_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1245 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/predicate_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1249 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/project_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1616 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/rename_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1469 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/sample_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1760 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/seq_scan_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1201 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/show_info_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4419 2023-04-05 15:01:02.000000 evadb-0.2.1/eva/plan_nodes/storage_plan.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1420 2023-04-05 18:07:02.000000 evadb-0.2.1/eva/plan_nodes/types.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1245 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/plan_nodes/union_plan.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.070514 evadb-0.2.1/eva/readers/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/readers/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2320 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/readers/abstract_reader.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2651 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/readers/csv_reader.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5617 2023-04-05 15:01:02.000000 evadb-0.2.1/eva/readers/decord_reader.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.070514 evadb-0.2.1/eva/readers/image/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/readers/image/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1007 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/readers/image/opencv_image_reader.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.070514 evadb-0.2.1/eva/server/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      623 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/server/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3284 2023-04-03 16:26:49.000000 evadb-0.2.1/eva/server/command_handler.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3502 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/server/db_api.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3276 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/server/interpreter.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2866 2023-04-06 05:12:11.000000 evadb-0.2.1/eva/server/server.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.074514 evadb-0.2.1/eva/storage/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/storage/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5659 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/storage/abstract_media_storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2385 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/storage/abstract_storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1694 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/storage/image_storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8881 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/storage/sqlite_storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1688 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/storage/storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2243 2023-04-05 15:01:02.000000 evadb-0.2.1/eva/storage/video_storage_engine.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.074514 evadb-0.2.1/eva/third_party/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      605 2023-04-13 06:12:12.000000 evadb-0.2.1/eva/third_party/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.074514 evadb-0.2.1/eva/third_party/huggingface/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      619 2023-04-13 06:12:12.000000 evadb-0.2.1/eva/third_party/huggingface/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1506 2023-04-13 06:12:12.000000 evadb-0.2.1/eva/third_party/huggingface/binder.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5776 2023-04-13 06:12:12.000000 evadb-0.2.1/eva/third_party/huggingface/create.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1453 2023-04-13 06:12:12.000000 evadb-0.2.1/eva/third_party/huggingface/model.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.074514 evadb-0.2.1/eva/udfs/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.074514 evadb-0.2.1/eva/udfs/abstract/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      625 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/abstract/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2441 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/abstract/abstract_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3096 2023-04-13 06:12:12.000000 evadb-0.2.1/eva/udfs/abstract/hf_abstract_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3843 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/abstract/pytorch_abstract_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3464 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/asl_action_recognition.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.074514 evadb-0.2.1/eva/udfs/decorators/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/decorators/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2185 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/decorators/decorators.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.074514 evadb-0.2.1/eva/udfs/decorators/io_descriptors/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/decorators/io_descriptors/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2754 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/decorators/io_descriptors/abstract_types.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3375 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/decorators/io_descriptors/data_types.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1437 2023-04-12 18:47:51.000000 evadb-0.2.1/eva/udfs/decorators/utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5675 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/decorators/yolo_object_detection_decorators.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5478 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/emotion_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2539 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/face_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5110 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/fastrcnn_object_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1822 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/feature_extractor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1028 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/gpu_compatible.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2200 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/mvit_action_recognition.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.078514 evadb-0.2.1/eva/udfs/ndarray/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      638 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/ndarray/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2568 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/ndarray/array_count.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1647 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/ndarray/crop.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1179 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/ndarray/fuzzy_join.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1557 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/ndarray/open.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1782 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/ndarray/similarity.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2750 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/ocr_extractor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6764 2023-04-12 18:47:51.000000 evadb-0.2.1/eva/udfs/udf_bootstrap_queries.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5043 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/udfs/yolo_object_detector.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.078514 evadb-0.2.1/eva/utils/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      611 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/utils/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      909 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/utils/errors.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6957 2023-04-13 06:12:12.000000 evadb-0.2.1/eva/utils/generic_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1837 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/utils/kv_cache.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      985 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/utils/logging_manager.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1562 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/utils/s3_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1692 2023-04-02 17:27:27.000000 evadb-0.2.1/eva/utils/stats.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      711 2023-04-25 13:04:53.000000 evadb-0.2.1/eva/version.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.078514 evadb-0.2.1/evadb.egg-info/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    15197 2023-04-25 13:20:55.000000 evadb-0.2.1/evadb.egg-info/PKG-INFO
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13535 2023-04-25 13:20:56.000000 evadb-0.2.1/evadb.egg-info/SOURCES.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)        1 2023-04-25 13:20:55.000000 evadb-0.2.1/evadb.egg-info/dependency_links.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       89 2023-04-25 13:20:55.000000 evadb-0.2.1/evadb.egg-info/entry_points.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1069 2023-04-25 13:20:55.000000 evadb-0.2.1/evadb.egg-info/requires.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       21 2023-04-25 13:20:55.000000 evadb-0.2.1/evadb.egg-info/top_level.txt
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       90 2023-04-02 17:27:27.000000 evadb-0.2.1/pyproject.toml
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       38 2023-04-25 13:20:56.094514 evadb-0.2.1/setup.cfg
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4032 2023-04-25 12:50:32.000000 evadb-0.2.1/setup.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.078514 evadb-0.2.1/test/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.078514 evadb-0.2.1/test/benchmark_tests/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/benchmark_tests/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1172 2023-04-02 17:27:27.000000 evadb-0.2.1/test/benchmark_tests/conftest.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1504 2023-04-18 07:04:09.000000 evadb-0.2.1/test/benchmark_tests/plot.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3294 2023-04-24 23:47:21.000000 evadb-0.2.1/test/benchmark_tests/test_benchmark_pytorch.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.078514 evadb-0.2.1/test/binder/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/binder/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2032 2023-04-02 17:27:27.000000 evadb-0.2.1/test/binder/test_binder_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    14016 2023-04-02 17:27:27.000000 evadb-0.2.1/test/binder/test_statement_binder.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7961 2023-04-02 17:27:27.000000 evadb-0.2.1/test/binder/test_statement_binder_context.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1796 2023-04-02 17:27:27.000000 evadb-0.2.1/test/binder/test_statement_binder_python37.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.078514 evadb-0.2.1/test/catalog/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/catalog/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.078514 evadb-0.2.1/test/catalog/models/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/catalog/models/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7234 2023-04-02 17:27:27.000000 evadb-0.2.1/test/catalog/models/test_models.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.082514 evadb-0.2.1/test/catalog/services/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/catalog/services/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1918 2023-04-02 17:27:27.000000 evadb-0.2.1/test/catalog/services/test_column_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4745 2023-04-13 06:12:12.000000 evadb-0.2.1/test/catalog/services/test_index_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3639 2023-04-02 17:27:27.000000 evadb-0.2.1/test/catalog/services/test_table_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3639 2023-04-02 17:27:27.000000 evadb-0.2.1/test/catalog/services/test_udf_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3210 2023-04-02 17:27:27.000000 evadb-0.2.1/test/catalog/services/test_udf_cost_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3035 2023-04-02 17:27:27.000000 evadb-0.2.1/test/catalog/services/test_udf_io_catalog_service.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7560 2023-04-05 15:01:02.000000 evadb-0.2.1/test/catalog/test_catalog_manager.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1402 2023-04-02 17:27:27.000000 evadb-0.2.1/test/catalog/test_column_type.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1910 2023-04-02 17:27:27.000000 evadb-0.2.1/test/catalog/test_sqlalchemy.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.082514 evadb-0.2.1/test/configuration/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/configuration/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1490 2023-04-02 17:27:27.000000 evadb-0.2.1/test/configuration/test_bootstrap_environment.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1690 2023-04-02 17:27:27.000000 evadb-0.2.1/test/configuration/test_configuration_manager.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.082514 evadb-0.2.1/test/executor/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/executor/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1106 2023-04-02 17:27:27.000000 evadb-0.2.1/test/executor/test_abstract_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2441 2023-04-02 17:27:27.000000 evadb-0.2.1/test/executor/test_create_mat_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3987 2023-04-02 17:27:27.000000 evadb-0.2.1/test/executor/test_create_udf_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4227 2023-04-06 05:12:11.000000 evadb-0.2.1/test/executor/test_execution_context.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1275 2023-04-02 17:27:27.000000 evadb-0.2.1/test/executor/test_executor_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4650 2023-04-02 17:27:27.000000 evadb-0.2.1/test/executor/test_limit_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3890 2023-04-02 17:27:27.000000 evadb-0.2.1/test/executor/test_load_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2884 2023-04-02 17:27:27.000000 evadb-0.2.1/test/executor/test_orderby_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10986 2023-04-02 17:27:27.000000 evadb-0.2.1/test/executor/test_plan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1397 2023-04-02 17:27:27.000000 evadb-0.2.1/test/executor/test_pp_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1817 2023-04-02 17:27:27.000000 evadb-0.2.1/test/executor/test_sample_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2752 2023-04-06 17:08:11.000000 evadb-0.2.1/test/executor/test_seq_scan_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      847 2023-04-02 17:27:27.000000 evadb-0.2.1/test/executor/utils.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.082514 evadb-0.2.1/test/expression/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/expression/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3722 2023-04-02 17:27:27.000000 evadb-0.2.1/test/expression/test_abstract_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5149 2023-04-02 17:27:27.000000 evadb-0.2.1/test/expression/test_aggregation.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2975 2023-04-02 17:27:27.000000 evadb-0.2.1/test/expression/test_arithmetic.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5578 2023-04-02 17:27:27.000000 evadb-0.2.1/test/expression/test_comparison.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2867 2023-04-02 17:27:27.000000 evadb-0.2.1/test/expression/test_expression_tree.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7555 2023-04-02 17:27:27.000000 evadb-0.2.1/test/expression/test_expression_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2685 2023-04-02 17:27:27.000000 evadb-0.2.1/test/expression/test_function_expression.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10242 2023-04-13 06:25:00.000000 evadb-0.2.1/test/expression/test_logical.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.086514 evadb-0.2.1/test/integration_tests/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/integration_tests/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3587 2023-04-06 05:12:11.000000 evadb-0.2.1/test/integration_tests/test_array_count.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7647 2023-04-02 17:27:27.000000 evadb-0.2.1/test/integration_tests/test_create_index_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1091 2023-04-02 17:27:27.000000 evadb-0.2.1/test/integration_tests/test_create_table_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5160 2023-04-06 05:12:11.000000 evadb-0.2.1/test/integration_tests/test_delete_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4839 2023-04-05 15:01:02.000000 evadb-0.2.1/test/integration_tests/test_drop_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2454 2023-04-06 05:12:11.000000 evadb-0.2.1/test/integration_tests/test_error_handling_with_ray.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4088 2023-04-13 06:12:12.000000 evadb-0.2.1/test/integration_tests/test_explain_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3183 2023-04-06 05:12:11.000000 evadb-0.2.1/test/integration_tests/test_fuzzy_join.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7790 2023-04-13 06:12:12.000000 evadb-0.2.1/test/integration_tests/test_huggingface_udfs.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3896 2023-04-06 05:12:11.000000 evadb-0.2.1/test/integration_tests/test_insert_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2956 2023-04-06 05:12:11.000000 evadb-0.2.1/test/integration_tests/test_like.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    19262 2023-04-06 05:12:11.000000 evadb-0.2.1/test/integration_tests/test_load_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5233 2023-04-06 05:12:11.000000 evadb-0.2.1/test/integration_tests/test_mat_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2660 2023-04-06 05:12:11.000000 evadb-0.2.1/test/integration_tests/test_open.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10184 2023-04-12 18:47:51.000000 evadb-0.2.1/test/integration_tests/test_optimizer_rules.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    11219 2023-04-25 12:50:32.000000 evadb-0.2.1/test/integration_tests/test_pytorch.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2953 2023-04-02 17:27:27.000000 evadb-0.2.1/test/integration_tests/test_rename_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7580 2023-04-12 18:47:51.000000 evadb-0.2.1/test/integration_tests/test_reuse.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5210 2023-04-06 05:12:11.000000 evadb-0.2.1/test/integration_tests/test_s3_load_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    29003 2023-04-06 17:08:11.000000 evadb-0.2.1/test/integration_tests/test_select_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3873 2023-04-13 06:12:12.000000 evadb-0.2.1/test/integration_tests/test_show_info_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12289 2023-04-06 05:12:11.000000 evadb-0.2.1/test/integration_tests/test_similarity.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12062 2023-04-06 05:12:11.000000 evadb-0.2.1/test/integration_tests/test_udf_executor.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      852 2023-04-02 17:27:27.000000 evadb-0.2.1/test/markers.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.086514 evadb-0.2.1/test/models/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/models/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.086514 evadb-0.2.1/test/models/catalog/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/models/catalog/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1010 2023-04-02 17:27:27.000000 evadb-0.2.1/test/models/catalog/test_frame_info.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.086514 evadb-0.2.1/test/models/storage/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/models/storage/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5919 2023-04-05 15:01:02.000000 evadb-0.2.1/test/models/storage/test_batch.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.090515 evadb-0.2.1/test/optimizer/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/optimizer/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.090515 evadb-0.2.1/test/optimizer/rules/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/optimizer/rules/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    11728 2023-04-12 18:47:51.000000 evadb-0.2.1/test/optimizer/rules/test_rules.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4195 2023-04-02 17:27:27.000000 evadb-0.2.1/test/optimizer/test_binder.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4377 2023-04-06 05:12:11.000000 evadb-0.2.1/test/optimizer/test_cascade_optimizer.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4406 2023-04-02 17:27:27.000000 evadb-0.2.1/test/optimizer/test_cost_model.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2689 2023-04-02 17:27:27.000000 evadb-0.2.1/test/optimizer/test_group.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1996 2023-04-02 17:27:27.000000 evadb-0.2.1/test/optimizer/test_memo.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1034 2023-04-02 17:27:27.000000 evadb-0.2.1/test/optimizer/test_optimizer_context.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6122 2023-04-13 06:12:12.000000 evadb-0.2.1/test/optimizer/test_optimizer_task.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2000 2023-04-02 17:27:27.000000 evadb-0.2.1/test/optimizer/test_optimizer_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13335 2023-04-12 18:47:51.000000 evadb-0.2.1/test/optimizer/test_statement_to_opr_convertor.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.090515 evadb-0.2.1/test/parser/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/parser/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    36051 2023-04-02 17:27:27.000000 evadb-0.2.1/test/parser/test_parser.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4843 2023-04-02 17:27:27.000000 evadb-0.2.1/test/parser/test_parser_statements.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.090515 evadb-0.2.1/test/plan_nodes/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/plan_nodes/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6292 2023-04-02 17:27:27.000000 evadb-0.2.1/test/plan_nodes/test_plan.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.090515 evadb-0.2.1/test/readers/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/readers/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1688 2023-04-02 17:27:27.000000 evadb-0.2.1/test/readers/test_csv_reader.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7288 2023-04-05 15:01:02.000000 evadb-0.2.1/test/readers/test_decord_reader.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.090515 evadb-0.2.1/test/server/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/server/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1268 2023-04-02 17:27:27.000000 evadb-0.2.1/test/server/test_command_handler.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5057 2023-04-02 17:27:27.000000 evadb-0.2.1/test/server/test_db_api.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2581 2023-04-02 17:27:27.000000 evadb-0.2.1/test/server/test_interpreter.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2066 2023-04-02 17:27:27.000000 evadb-0.2.1/test/server/test_server.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.090515 evadb-0.2.1/test/storage/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/storage/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4001 2023-04-02 17:27:27.000000 evadb-0.2.1/test/storage/test_sqlite_storage_engine.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4023 2023-04-02 17:27:27.000000 evadb-0.2.1/test/storage/test_video_storage.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1801 2023-04-02 17:27:27.000000 evadb-0.2.1/test/test_eva_cmd_client.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1294 2023-04-02 17:27:27.000000 evadb-0.2.1/test/test_eva_imports.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1810 2023-04-02 17:27:27.000000 evadb-0.2.1/test/test_eva_server.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.090515 evadb-0.2.1/test/udfs/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      638 2023-04-02 17:27:27.000000 evadb-0.2.1/test/udfs/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.090515 evadb-0.2.1/test/udfs/decorators/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/udfs/decorators/__init__.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.090515 evadb-0.2.1/test/udfs/decorators/io_descriptors/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/udfs/decorators/io_descriptors/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7430 2023-04-02 17:27:27.000000 evadb-0.2.1/test/udfs/decorators/io_descriptors/test_descriptors.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2134 2023-04-02 17:27:27.000000 evadb-0.2.1/test/udfs/decorators/test_decorators.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.090515 evadb-0.2.1/test/udfs/ndarray/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      648 2023-04-02 17:27:27.000000 evadb-0.2.1/test/udfs/ndarray/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      849 2023-04-02 17:27:27.000000 evadb-0.2.1/test/udfs/ndarray/test_array_count.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2410 2023-04-02 17:27:27.000000 evadb-0.2.1/test/udfs/ndarray/test_crop.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2374 2023-04-13 06:12:12.000000 evadb-0.2.1/test/udfs/ndarray/test_open.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4330 2023-04-13 06:12:12.000000 evadb-0.2.1/test/udfs/test_abstract_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2154 2023-04-02 17:27:27.000000 evadb-0.2.1/test/udfs/test_emotion_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3345 2023-04-02 17:27:27.000000 evadb-0.2.1/test/udfs/test_facenet_udf.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2548 2023-04-02 17:27:27.000000 evadb-0.2.1/test/udfs/test_fastrcnn_object_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2689 2023-04-02 17:27:27.000000 evadb-0.2.1/test/udfs/test_yolo_object_detector.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    16108 2023-04-13 06:12:12.000000 evadb-0.2.1/test/util.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.094514 evadb-0.2.1/test/utils/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-04-02 17:27:27.000000 evadb-0.2.1/test/utils/__init__.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4196 2023-04-13 06:12:12.000000 evadb-0.2.1/test/utils/test_generic_utils.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2256 2023-04-02 17:27:27.000000 evadb-0.2.1/test/utils/test_timer.py
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2181 2023-04-13 06:12:12.000000 evadb-0.2.1/test/utils/test_xdist.py
+drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-25 13:20:56.094514 evadb-0.2.1/third_party/
+-rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-02 17:27:27.000000 evadb-0.2.1/third_party/__init__.py
```

### Comparing `evadb-0.2.0/LICENSE.txt` & `evadb-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/PKG-INFO` & `evadb-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: evadb
-Version: 0.2.0
+Version: 0.2.1
 Summary: EVA Video Database System (Think MySQL for videos).
 Home-page: https://github.com/georgia-tech-db/eva
 Author: Georgia Tech Database Group
 Author-email: georgia.tech.db@gmail.com
 License: Apache License 2.0
 Download-URL: https://github.com/georgia-tech-db/eva
 Description: <div >
           <a href="https://evadb.readthedocs.io/">
             <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-banner.png" alt="EVA" width="1000px" margin-left="-5px">
           </a>
           <div>
                 <h3>Try It Out!</h3>
+                <a href="https://github.com/georgia-tech-db/eva">
+                    <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/v1.json" alt="Logo"/>
+                </a>
                 <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
                     <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EVA on Colab"/>
                 </a>
                 <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
                     <img alt="Slack" src="https://img.shields.io/badge/slack-eva-ff69b4.svg?logo=slack">
                 </a>    
                 <a href="https://github.com/georgia-tech-db/eva/discussions">
@@ -26,120 +29,153 @@
                 <img alt="License" src="https://img.shields.io/badge/license-Apache%202-brightgreen.svg?logo=apache"/>
                 <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.7%20|%203.8%20|%203.9%20|%203.10-brightgreen"/>
             </div>
         </div>
         
         # EVA AI-Relational Database System
         
-        EVA is an open-source **AI-relational database with first-class support for deep learning models**. It aims to support AI-powered database applications that operate on both structured (tables) and unstructured data (videos, text, podcasts, PDFs, etc.) with deep learning models.
+        - â¡ï¸ 10-100x faster AI pipelines using SQL-like queries 
+        - ð° Save money spent on GPU-driven inference
+        - ð¦ Built-in caching to avoid re-running deep learning models across queries
+        - ð Over 20 AI-centric query optimization rules
+        - â¨ï¸ First-party integrations for PyTorch and HuggingFace models
+        - ð Installable via pip
+        - ð¤ Fully implemented in Python
+        
+        EVA is an open-source **AI-relational database with first-class support for deep learning models**. It supports next-generation AI-powered database applications that operate on structured (tables) and unstructured data (videos, text, podcasts, PDFs, etc.) with deep learning models.
         
-        EVA accelerates AI pipelines using a collection of optimizations inspired by relational database systems including function caching, sampling, and cost-based operator reordering. It comes with a wide range of models for analyzing unstructured data including image classification, object detection, OCR, face detection, etc. It is fully implemented in Python, and licensed under the Apache license.
+        EVA accelerates AI pipelines by 10-100x using a collection of optimizations inspired by relational database systems, including function caching, sampling, and cost-based predicate reordering. It comes with a wide range of models for analyzing unstructured data, including models for image classification, object detection, OCR, text sentiment classification, face detection, etc. It is fully implemented in Python and licensed under the Apache license.
         
-        EVA supports a AI-oriented query language for analysing unstructured data. Here are some illustrative applications:
+        EVA supports an AI-oriented query language tailored for analyzing unstructured data. Here are some illustrative applications:
         
          * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
          * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection </a>
          * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
-         * <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recogizing license plates </a>
+         * <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates </a>
          * <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
          
-        If you are wondering why you might need a AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/video.html#">Video Database Systems</a>. It describes how EVA lets you easily make use of deep learning models and you can save money spent on inference on large image or video datasets.
+        If you are wondering why you might need an AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/video.html#">Video Database Systems</a>. It describes how EVA lets you easily use deep learning models and save money spent on GPU-driven inference on large image or video datasets.
         
         The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different computer vision tasks: image classification, object detection, action recognition, and how you can easily extend EVA to support your custom deep learning model in the form of user-defined functions.
         
-        The <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/index.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab, where you can run the code by yourself.
+        The <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/index.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab to run the code.
         
         ## Why EVA? ##
         
         <details>
           <summary><b>Easily combine SQL and Deep Learning to build next-generation database applications</b></summary>
           Easily query videos in user-facing applications with a SQL-like interface for commonly used computer vision models.
         </details>
         
         <details>
           <summary><b>Speed up queries and save money spent on model inference</b></summary>
-          EVA comes with a collection of built-in sampling, caching, and filtering optimizations inspired by time-tested relational database systems.
+          EVA has built-in sampling, caching, and filtering optimizations inspired by time-tested relational database systems.
         </details>
         
         <details>
           <summary><b>Extensible by design to support custom deep learning models </b></summary>
-          EVA has first-class support for user-defined functions that wrap around your deep learning models in PyTorch.
+          EVA has first-class support for user-defined functions that wrap around your deep learning models in PyTorch and HuggingFace.
         </details>
         
         ## Links
         * [Documentation](https://evadb.readthedocs.io/)
         * [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
         * [Join Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
         * [Demo](https://ada-00.cc.gatech.edu/eva/playground)
         
         ## Quick Start
         
-        1. To install EVA, we recommend using the pip package manager (EVA supports Python versions 3.7+).
+        - Install EVA using the pip package manager. EVA supports Python versions 3.7+.
         
         ```shell
         pip install evadb
         ```
         
-        2. EVA is based on a client-server architecture. It works in Jupyter notebooks (illustrative notebooks are available in the [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb) folder) and also supports a terminal-based client. To start the EVA server and a terminal-based client, use the following commands:
+        - To start and connect to an EVA server in a Jupyter notebook, check out this [illustrative emotion analysis notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb):
         ```shell
-        eva_server &   # launch server
-        eva_client     # launch client
+        cursor = connect_to_server()
         ```
         
-        3. Load a video onto the EVA server from the client (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) video as an example):
+        - Load a video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration):
         
         ```mysql
-        LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO MyVideo;
+        LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO UADETRAC;
         ```
         
-        4. That's it! You can now run queries over the loaded video:
+        - That's it! You can now run queries over the loaded video:
         
         ```mysql
-        SELECT id, data FROM MyVideo WHERE id < 5;
+        SELECT id, data FROM UADETRAC WHERE id < 5;
         ```
         
-        5. Search for frames in the video that contain a car
+        - Search for frames in the video that contain a car
         
         ```mysql
-        SELECT id, data FROM MyVideo WHERE ['car'] <@ FastRCNNObjectDetector(data).labels;
+        SELECT id, data FROM UADETRAC WHERE ['car'] <@ YoloV5(data).labels;
         ```
         | Source Video  | Query Result |
         |---------------|--------------|
         |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
         
-        6. Search for frames in the video that contain a pedestrian and a car
+        - Search for frames in the video that contain a pedestrian and a car
         
         ```mysql
-        SELECT id, data FROM MyVideo WHERE ['pedestrian', 'car'] <@ FastRCNNObjectDetector(data).labels;
+        SELECT id, data FROM UADETRAC WHERE ['pedestrian', 'car'] <@ YoloV5(data).labels;
         ```
         
-        7. Search for frames in the video with more than 3 cars
+        - Search for frames with more than three cars
         
         ```mysql
-        SELECT id, data FROM MyVideo WHERE ArrayCount(FastRCNNObjectDetector(data).labels, 'car') > 3;
+        SELECT id, data FROM UADETRAC WHERE ArrayCount(YoloV5(data).labels, 'car') > 3;
         ```
         
-        8. You can create a new user-defined function (UDF) that wraps around your custom vision model or an off-the-shelf model like FastRCNN:
+        - You can **create a custom user-defined function (UDF)** that wraps around a fine-tuned or off-the-shelf deep learning model:
         ```mysql
         CREATE UDF IF NOT EXISTS MyUDF
         INPUT  (frame NDARRAY UINT8(3, ANYDIM, ANYDIM))
         OUTPUT (labels NDARRAY STR(ANYDIM), bboxes NDARRAY FLOAT32(ANYDIM, 4),
                 scores NDARRAY FLOAT32(ANYDIM))
         TYPE  Classification
         IMPL  'eva/udfs/fastrcnn_object_detector.py';
         ```
         
-        9. You can combine multiple user-defined functions in a single query to accomplish more complicated tasks.
+        - **Compose multiple user-defined functions in a single query** to accomplish complicated AI pipelines.
         ```mysql
            -- Analyse emotions of faces in a video
            SELECT id, bbox, EmotionDetector(Crop(data, bbox)) 
            FROM MyVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)  
            WHERE id < 15;
         ```
         
+        - Besides making it easy to write queries for complex AI pipelines, EVA **speeds up query execution using its AI-centric query optimizer**. Two illustrative  optimizations are:
+        
+           ð¾ **Caching**: EVA automatically caches and reuses previous query results (especially model inference results), eliminating redundant computation and reducing query processing time.
+        
+           ð¯ **Predicate Reordering**: EVA optimizes the order in which the query predicates are evaluated (e.g., runs the faster, more selective model first), leading to faster queries and lower inference costs.
+        
+        Consider these two exploratory queries on a dataset of dog images:
+        <img align="right" style="display:inline;" width="40%" src="https://github.com/georgia-tech-db/eva/blob/master/data/assets/eva_performance_comparison.png?raw=true"></a>
+        
+        ```mysql
+          -- Query 1: Find all images of black-colored dogs
+          SELECT id, bbox FROM dogs 
+          JOIN LATERAL UNNEST(YoloV5(data)) AS Obj(label, bbox, score) 
+          WHERE Obj.label = 'dog' 
+            AND Color(Crop(data, bbox)) = 'black'; 
+        
+          -- Query 2: Find all Great Danes that are black-colored
+          SELECT id, bbox FROM dogs 
+          JOIN LATERAL UNNEST(YoloV5(data)) AS Obj(label, bbox, score) 
+          WHERE Obj.label = 'dog' 
+            AND DogBreedClassifier(Crop(data, bbox)) = 'great dane' 
+            AND Color(Crop(data, bbox)) = 'black';
+        ```
+        
+        By reusing the results of the first query and reordering the predicates based on available cached results, EVA runs up the second query **10x faster**!
+        
         ## Illustrative EVA Applications 
         
         ### Traffic Analysis (Object Detection Model)
         | Source Video  | Query Result |
         |---------------|--------------|
         |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
         
@@ -181,22 +217,21 @@
         ## Contributing to EVA
         
         [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb)
         [![CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva)
         [![Coverage Status](https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master)](https://coveralls.io/github/georgia-tech-db/eva?branch=master)
         [![Documentation Status](https://readthedocs.org/projects/evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/index.html)
         
-        We welcome all kinds of contributions to EVA.
-        To file a bug or request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
+        EVA is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EVA are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
         
-        For more information on contributing to EVA, see our
+        For more information, see our
         [contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
         
         ## License
-        Copyright (c) 2018-2023 [Georgia Tech Database Group](http://db.cc.gatech.edu/)
+        Copyright (c) 2018-2023 [Georgia Tech Database Group](http://db.cc.gatech.edu/).
         Licensed under [Apache License](LICENSE).
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,107 +1,128 @@
-Metadata-Version: 2.1 Name: evadb Version: 0.2.0 Summary: EVA Video Database
+Metadata-Version: 2.1 Name: evadb Version: 0.2.1 Summary: EVA Video Database
 System (Think MySQL for videos). Home-page: https://github.com/georgia-tech-db/
 eva Author: Georgia Tech Database Group Author-email: georgia.tech.db@gmail.com
 License: Apache License 2.0 Download-URL: https://github.com/georgia-tech-db/
 eva Description:
 [EVA]
 **** Try It Out! ****
-[Open_EVA_on_Colab] [Slack] [Discuss_on_Github!] [PyPI] [License] [Python
-Versions]
-# EVA AI-Relational Database System EVA is an open-source **AI-relational
-database with first-class support for deep learning models**. It aims to
-support AI-powered database applications that operate on both structured
-(tables) and unstructured data (videos, text, podcasts, PDFs, etc.) with deep
-learning models. EVA accelerates AI pipelines using a collection of
-optimizations inspired by relational database systems including function
-caching, sampling, and cost-based operator reordering. It comes with a wide
-range of models for analyzing unstructured data including image classification,
-object detection, OCR, face detection, etc. It is fully implemented in Python,
-and licensed under the Apache license. EVA supports a AI-oriented query
-language for analysing unstructured data. Here are some illustrative
+[Logo] [Open_EVA_on_Colab] [Slack] [Discuss_on_Github!] [PyPI] [License]
+[Python Versions]
+# EVA AI-Relational Database System - Ã¢ÂÂ¡Ã¯Â¸Â 10-100x faster AI pipelines
+using SQL-like queries - Ã°ÂÂÂ° Save money spent on GPU-driven inference -
+Ã°ÂÂÂ¦ Built-in caching to avoid re-running deep learning models across
+queries - Ã°ÂÂÂ Over 20 AI-centric query optimization rules - Ã¢ÂÂ¨Ã¯Â¸Â
+First-party integrations for PyTorch and HuggingFace models - Ã°ÂÂÂ
+Installable via pip - Ã°ÂÂ¤Â Fully implemented in Python EVA is an open-
+source **AI-relational database with first-class support for deep learning
+models**. It supports next-generation AI-powered database applications that
+operate on structured (tables) and unstructured data (videos, text, podcasts,
+PDFs, etc.) with deep learning models. EVA accelerates AI pipelines by 10-100x
+using a collection of optimizations inspired by relational database systems,
+including function caching, sampling, and cost-based predicate reordering. It
+comes with a wide range of models for analyzing unstructured data, including
+models for image classification, object detection, OCR, text sentiment
+classification, face detection, etc. It is fully implemented in Python and
+licensed under the Apache license. EVA supports an AI-oriented query language
+tailored for analyzing unstructured data. Here are some illustrative
 applications: * Examining_the_emotion_palette_of_actors_in_a_movie * Analysing
 traffic_flow_at_an_intersection * Classifying_images_based_on_their_content *
-Recogizing_license_plates * Analysing_toxicity_of_social_media_memes If you are
-wondering why you might need a AI-relational database system, start with the
-page on Video_Database_Systems. It describes how EVA lets you easily make use
-of deep learning models and you can save money spent on inference on large
+Recognizing_license_plates * Analysing_toxicity_of_social_media_memes If you
+are wondering why you might need an AI-relational database system, start with
+the page on Video_Database_Systems. It describes how EVA lets you easily use
+deep learning models and save money spent on GPU-driven inference on large
 image or video datasets. The Getting_Started page shows how you can use EVA for
 different computer vision tasks: image classification, object detection, action
 recognition, and how you can easily extend EVA to support your custom deep
 learning model in the form of user-defined functions. The User_Guides section
 contains Jupyter Notebooks that demonstrate how to use various features of EVA.
-Each notebook includes a link to Google Colab, where you can run the code by
-yourself. ## Why EVA? ##  Easily combine SQL and Deep Learning to build next-
-generation database applications Easily query videos in user-facing
-applications with a SQL-like interface for commonly used computer vision
-models.   Speed up queries and save money spent on model inference EVA comes
-with a collection of built-in sampling, caching, and filtering optimizations
-inspired by time-tested relational database systems.   Extensible by design to
-support custom deep learning models EVA has first-class support for user-
-defined functions that wrap around your deep learning models in PyTorch.  ##
-Links * [Documentation](https://evadb.readthedocs.io/) * [Tutorials](https://
-github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
-* [Join Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-
-PlJ4iawLdurDv~aIAq90Dg) * [Demo](https://ada-00.cc.gatech.edu/eva/playground)
-## Quick Start 1. To install EVA, we recommend using the pip package manager
-(EVA supports Python versions 3.7+). ```shell pip install evadb ``` 2. EVA is
-based on a client-server architecture. It works in Jupyter notebooks
-(illustrative notebooks are available in the [Tutorials](https://github.com/
-georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb) folder)
-and also supports a terminal-based client. To start the EVA server and a
-terminal-based client, use the following commands: ```shell eva_server & #
-launch server eva_client # launch client ``` 3. Load a video onto the EVA
-server from the client (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4)
-video as an example): ```mysql LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO
-MyVideo; ``` 4. That's it! You can now run queries over the loaded video:
-```mysql SELECT id, data FROM MyVideo WHERE id < 5; ``` 5. Search for frames in
-the video that contain a car ```mysql SELECT id, data FROM MyVideo WHERE
-['car'] <@ FastRCNNObjectDetector(data).labels; ``` | Source Video | Query
-Result | |---------------|--------------| |[Source Video] |[Query Result] | 6.
-Search for frames in the video that contain a pedestrian and a car ```mysql
-SELECT id, data FROM MyVideo WHERE ['pedestrian', 'car'] <@
-FastRCNNObjectDetector(data).labels; ``` 7. Search for frames in the video with
-more than 3 cars ```mysql SELECT id, data FROM MyVideo WHERE ArrayCount
-(FastRCNNObjectDetector(data).labels, 'car') > 3; ``` 8. You can create a new
-user-defined function (UDF) that wraps around your custom vision model or an
-off-the-shelf model like FastRCNN: ```mysql CREATE UDF IF NOT EXISTS MyUDF
-INPUT (frame NDARRAY UINT8(3, ANYDIM, ANYDIM)) OUTPUT (labels NDARRAY STR
-(ANYDIM), bboxes NDARRAY FLOAT32(ANYDIM, 4), scores NDARRAY FLOAT32(ANYDIM))
-TYPE Classification IMPL 'eva/udfs/fastrcnn_object_detector.py'; ``` 9. You can
-combine multiple user-defined functions in a single query to accomplish more
-complicated tasks. ```mysql -- Analyse emotions of faces in a video SELECT id,
-bbox, EmotionDetector(Crop(data, bbox)) FROM MyVideo JOIN LATERAL UNNEST
-(FaceDetector(data)) AS Face(bbox, conf) WHERE id < 15; ``` ## Illustrative EVA
-Applications ### Traffic Analysis (Object Detection Model) | Source Video |
-Query Result | |---------------|--------------| |[Source Video] |[Query Result]
-| ### MNIST Digit Recognition (Image Classification Model) | Source Video |
-Query Result | |---------------|--------------| |[Source Video] |[Query Result]
-| ### Movie Analysis (Face Detection + Emotion Classfication Models) | Source
-Video | Query Result | |---------------|--------------| |[Source Video] |[Query
-Result] | ### [License Plate Recognition](https://github.com/georgia-tech-db/
-eva-application-template) (Plate Detection + OCR Extraction Models) | Query
-Result | |--------------| [Query Result] | ### [Meme Toxicity Classification]
-(https://github.com/georgia-tech-db/toxicity-classification) (OCR Extraction +
-Toxicity Classification Models) | Query Result | |--------------| [Query
-Result] | ## Community Join the EVA community on [Slack](https://
-join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) to
-ask questions and to share your ideas for improving EVA. [EVA_Slack_Channel]
-### Architecture Diagram of EVA [EVA Architecture Diagram] ## Contributing to
-EVA [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://
-pypi.org/project/evadb) [![CI Status](https://circleci.com/gh/georgia-tech-db/
-eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva) [![Coverage
-Status](https://coveralls.io/repos/github/georgia-tech-db/eva/
-badge.svg?branch=master)](https://coveralls.io/github/georgia-tech-db/
-eva?branch=master) [![Documentation Status](https://readthedocs.org/projects/
-evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/
-index.html) We welcome all kinds of contributions to EVA. To file a bug or
-request a feature, please use GitHub_issues. Pull_requests are welcome. For
-more information on contributing to EVA, see our [contribution guide](https://
-evadb.readthedocs.io/en/stable/source/contribute/index.html). ## License
-Copyright (c) 2018-2023 [Georgia Tech Database Group](http://db.cc.gatech.edu/
-) Licensed under [Apache License](LICENSE). Platform: UNKNOWN Classifier:
-Intended Audience :: Science/Research Classifier: Topic :: Scientific/
-Engineering :: Information Analysis Classifier: License :: OSI Approved ::
-Apache Software License Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha Classifier: Operating System :: OS
-Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Provides-Extra: dev
+Each notebook includes a link to Google Colab to run the code. ## Why EVA? ##
+Easily combine SQL and Deep Learning to build next-generation database
+applications Easily query videos in user-facing applications with a SQL-like
+interface for commonly used computer vision models.   Speed up queries and save
+money spent on model inference EVA has built-in sampling, caching, and
+filtering optimizations inspired by time-tested relational database systems.
+Extensible by design to support custom deep learning models EVA has first-class
+support for user-defined functions that wrap around your deep learning models
+in PyTorch and HuggingFace.  ## Links * [Documentation](https://
+evadb.readthedocs.io/) * [Tutorials](https://github.com/georgia-tech-db/eva/
+blob/master/tutorials/03-emotion-analysis.ipynb) * [Join Slack](https://
+join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) *
+[Demo](https://ada-00.cc.gatech.edu/eva/playground) ## Quick Start - Install
+EVA using the pip package manager. EVA supports Python versions 3.7+. ```shell
+pip install evadb ``` - To start and connect to an EVA server in a Jupyter
+notebook, check out this [illustrative emotion analysis notebook](https://
+github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-
+analysis.ipynb): ```shell cursor = connect_to_server() ``` - Load a video onto
+the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for
+illustration): ```mysql LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO
+UADETRAC; ``` - That's it! You can now run queries over the loaded video:
+```mysql SELECT id, data FROM UADETRAC WHERE id < 5; ``` - Search for frames in
+the video that contain a car ```mysql SELECT id, data FROM UADETRAC WHERE
+['car'] <@ YoloV5(data).labels; ``` | Source Video | Query Result | |----------
+-----|--------------| |[Source Video] |[Query Result] | - Search for frames in
+the video that contain a pedestrian and a car ```mysql SELECT id, data FROM
+UADETRAC WHERE ['pedestrian', 'car'] <@ YoloV5(data).labels; ``` - Search for
+frames with more than three cars ```mysql SELECT id, data FROM UADETRAC WHERE
+ArrayCount(YoloV5(data).labels, 'car') > 3; ``` - You can **create a custom
+user-defined function (UDF)** that wraps around a fine-tuned or off-the-shelf
+deep learning model: ```mysql CREATE UDF IF NOT EXISTS MyUDF INPUT (frame
+NDARRAY UINT8(3, ANYDIM, ANYDIM)) OUTPUT (labels NDARRAY STR(ANYDIM), bboxes
+NDARRAY FLOAT32(ANYDIM, 4), scores NDARRAY FLOAT32(ANYDIM)) TYPE Classification
+IMPL 'eva/udfs/fastrcnn_object_detector.py'; ``` - **Compose multiple user-
+defined functions in a single query** to accomplish complicated AI pipelines.
+```mysql -- Analyse emotions of faces in a video SELECT id, bbox,
+EmotionDetector(Crop(data, bbox)) FROM MyVideo JOIN LATERAL UNNEST(FaceDetector
+(data)) AS Face(bbox, conf) WHERE id < 15; ``` - Besides making it easy to
+write queries for complex AI pipelines, EVA **speeds up query execution using
+its AI-centric query optimizer**. Two illustrative optimizations are: Ã°ÂÂÂ¾
+**Caching**: EVA automatically caches and reuses previous query results
+(especially model inference results), eliminating redundant computation and
+reducing query processing time. Ã°ÂÂÂ¯ **Predicate Reordering**: EVA
+optimizes the order in which the query predicates are evaluated (e.g., runs the
+faster, more selective model first), leading to faster queries and lower
+inference costs. Consider these two exploratory queries on a dataset of dog
+images: [https://github.com/georgia-tech-db/eva/blob/master/data/assets/
+eva_performance_comparison.png?raw=true]
+ ```mysql -- Query 1: Find all images of black-colored dogs SELECT id, bbox
+FROM dogs JOIN LATERAL UNNEST(YoloV5(data)) AS Obj(label, bbox, score) WHERE
+Obj.label = 'dog' AND Color(Crop(data, bbox)) = 'black'; -- Query 2: Find all
+Great Danes that are black-colored SELECT id, bbox FROM dogs JOIN LATERAL
+UNNEST(YoloV5(data)) AS Obj(label, bbox, score) WHERE Obj.label = 'dog' AND
+DogBreedClassifier(Crop(data, bbox)) = 'great dane' AND Color(Crop(data, bbox))
+= 'black'; ``` By reusing the results of the first query and reordering the
+predicates based on available cached results, EVA runs up the second query
+**10x faster**! ## Illustrative EVA Applications ### Traffic Analysis (Object
+Detection Model) | Source Video | Query Result | |---------------|-------------
+-| |[Source Video] |[Query Result] | ### MNIST Digit Recognition (Image
+Classification Model) | Source Video | Query Result | |---------------|--------
+------| |[Source Video] |[Query Result] | ### Movie Analysis (Face Detection +
+Emotion Classfication Models) | Source Video | Query Result | |---------------
+|--------------| |[Source Video] |[Query Result] | ### [License Plate
+Recognition](https://github.com/georgia-tech-db/eva-application-template)
+(Plate Detection + OCR Extraction Models) | Query Result | |--------------|
+[Query Result] | ### [Meme Toxicity Classification](https://github.com/georgia-
+tech-db/toxicity-classification) (OCR Extraction + Toxicity Classification
+Models) | Query Result | |--------------| [Query Result] | ## Community Join
+the EVA community on [Slack](https://join.slack.com/t/eva-db/shared_invite/zt-
+1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) to ask questions and to share your ideas for
+improving EVA. [EVA_Slack_Channel] ### Architecture Diagram of EVA [EVA
+Architecture Diagram] ## Contributing to EVA [![PyPI Version](https://
+img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb) [![CI Status]
+(https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://
+circleci.com/gh/georgia-tech-db/eva) [![Coverage Status](https://coveralls.io/
+repos/github/georgia-tech-db/eva/badge.svg?branch=master)](https://
+coveralls.io/github/georgia-tech-db/eva?branch=master) [![Documentation Status]
+(https://readthedocs.org/projects/evadb/badge/?version=stable)](https://
+evadb.readthedocs.io/en/stable/index.html) EVA is the beneficiary of many
+[contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All
+kinds of contributions to EVA are appreciated. To file a bug or to request a
+feature, please use GitHub_issues. Pull_requests are welcome. For more
+information, see our [contribution guide](https://evadb.readthedocs.io/en/
+stable/source/contribute/index.html). ## License Copyright (c) 2018-2023
+[Georgia Tech Database Group](http://db.cc.gatech.edu/). Licensed under [Apache
+License](LICENSE). Platform: UNKNOWN Classifier: Intended Audience :: Science/
+Research Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Programming Language :: Python :: 3 Classifier: Development Status :: 3 - Alpha
+Classifier: Operating System :: OS Independent Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: dev
```

### Comparing `evadb-0.2.0/README.md` & `evadb-0.2.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 <div >
   <a href="https://evadb.readthedocs.io/">
     <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-banner.png" alt="EVA" width="1000px" margin-left="-5px">
   </a>
   <div>
         <h3>Try It Out!</h3>
+        <a href="https://github.com/georgia-tech-db/eva">
+            <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/v1.json" alt="Logo"/>
+        </a>
         <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
             <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EVA on Colab"/>
         </a>
         <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
             <img alt="Slack" src="https://img.shields.io/badge/slack-eva-ff69b4.svg?logo=slack">
         </a>    
         <a href="https://github.com/georgia-tech-db/eva/discussions">
@@ -17,120 +20,153 @@
         <img alt="License" src="https://img.shields.io/badge/license-Apache%202-brightgreen.svg?logo=apache"/>
         <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.7%20|%203.8%20|%203.9%20|%203.10-brightgreen"/>
     </div>
 </div>
 
 # EVA AI-Relational Database System
 
-EVA is an open-source **AI-relational database with first-class support for deep learning models**. It aims to support AI-powered database applications that operate on both structured (tables) and unstructured data (videos, text, podcasts, PDFs, etc.) with deep learning models.
+- ⚡️ 10-100x faster AI pipelines using SQL-like queries 
+- 💰 Save money spent on GPU-driven inference
+- 📦 Built-in caching to avoid re-running deep learning models across queries
+- 📏 Over 20 AI-centric query optimization rules
+- ⌨️ First-party integrations for PyTorch and HuggingFace models
+- 🐍 Installable via pip
+- 🤝 Fully implemented in Python
+
+EVA is an open-source **AI-relational database with first-class support for deep learning models**. It supports next-generation AI-powered database applications that operate on structured (tables) and unstructured data (videos, text, podcasts, PDFs, etc.) with deep learning models.
 
-EVA accelerates AI pipelines using a collection of optimizations inspired by relational database systems including function caching, sampling, and cost-based operator reordering. It comes with a wide range of models for analyzing unstructured data including image classification, object detection, OCR, face detection, etc. It is fully implemented in Python, and licensed under the Apache license.
+EVA accelerates AI pipelines by 10-100x using a collection of optimizations inspired by relational database systems, including function caching, sampling, and cost-based predicate reordering. It comes with a wide range of models for analyzing unstructured data, including models for image classification, object detection, OCR, text sentiment classification, face detection, etc. It is fully implemented in Python and licensed under the Apache license.
 
-EVA supports a AI-oriented query language for analysing unstructured data. Here are some illustrative applications:
+EVA supports an AI-oriented query language tailored for analyzing unstructured data. Here are some illustrative applications:
 
  * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
  * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection </a>
  * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
- * <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recogizing license plates </a>
+ * <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates </a>
  * <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
  
-If you are wondering why you might need a AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/video.html#">Video Database Systems</a>. It describes how EVA lets you easily make use of deep learning models and you can save money spent on inference on large image or video datasets.
+If you are wondering why you might need an AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/video.html#">Video Database Systems</a>. It describes how EVA lets you easily use deep learning models and save money spent on GPU-driven inference on large image or video datasets.
 
 The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different computer vision tasks: image classification, object detection, action recognition, and how you can easily extend EVA to support your custom deep learning model in the form of user-defined functions.
 
-The <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/index.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab, where you can run the code by yourself.
+The <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/index.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab to run the code.
 
 ## Why EVA? ##
 
 <details>
   <summary><b>Easily combine SQL and Deep Learning to build next-generation database applications</b></summary>
   Easily query videos in user-facing applications with a SQL-like interface for commonly used computer vision models.
 </details>
 
 <details>
   <summary><b>Speed up queries and save money spent on model inference</b></summary>
-  EVA comes with a collection of built-in sampling, caching, and filtering optimizations inspired by time-tested relational database systems.
+  EVA has built-in sampling, caching, and filtering optimizations inspired by time-tested relational database systems.
 </details>
 
 <details>
   <summary><b>Extensible by design to support custom deep learning models </b></summary>
-  EVA has first-class support for user-defined functions that wrap around your deep learning models in PyTorch.
+  EVA has first-class support for user-defined functions that wrap around your deep learning models in PyTorch and HuggingFace.
 </details>
 
 ## Links
 * [Documentation](https://evadb.readthedocs.io/)
 * [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
 * [Join Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
 * [Demo](https://ada-00.cc.gatech.edu/eva/playground)
 
 ## Quick Start
 
-1. To install EVA, we recommend using the pip package manager (EVA supports Python versions 3.7+).
+- Install EVA using the pip package manager. EVA supports Python versions 3.7+.
 
 ```shell
 pip install evadb
 ```
 
-2. EVA is based on a client-server architecture. It works in Jupyter notebooks (illustrative notebooks are available in the [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb) folder) and also supports a terminal-based client. To start the EVA server and a terminal-based client, use the following commands:
+- To start and connect to an EVA server in a Jupyter notebook, check out this [illustrative emotion analysis notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb):
 ```shell
-eva_server &   # launch server
-eva_client     # launch client
+cursor = connect_to_server()
 ```
 
-3. Load a video onto the EVA server from the client (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) video as an example):
+- Load a video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration):
 
 ```mysql
-LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO MyVideo;
+LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO UADETRAC;
 ```
 
-4. That's it! You can now run queries over the loaded video:
+- That's it! You can now run queries over the loaded video:
 
 ```mysql
-SELECT id, data FROM MyVideo WHERE id < 5;
+SELECT id, data FROM UADETRAC WHERE id < 5;
 ```
 
-5. Search for frames in the video that contain a car
+- Search for frames in the video that contain a car
 
 ```mysql
-SELECT id, data FROM MyVideo WHERE ['car'] <@ FastRCNNObjectDetector(data).labels;
+SELECT id, data FROM UADETRAC WHERE ['car'] <@ YoloV5(data).labels;
 ```
 | Source Video  | Query Result |
 |---------------|--------------|
 |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
 
-6. Search for frames in the video that contain a pedestrian and a car
+- Search for frames in the video that contain a pedestrian and a car
 
 ```mysql
-SELECT id, data FROM MyVideo WHERE ['pedestrian', 'car'] <@ FastRCNNObjectDetector(data).labels;
+SELECT id, data FROM UADETRAC WHERE ['pedestrian', 'car'] <@ YoloV5(data).labels;
 ```
 
-7. Search for frames in the video with more than 3 cars
+- Search for frames with more than three cars
 
 ```mysql
-SELECT id, data FROM MyVideo WHERE ArrayCount(FastRCNNObjectDetector(data).labels, 'car') > 3;
+SELECT id, data FROM UADETRAC WHERE ArrayCount(YoloV5(data).labels, 'car') > 3;
 ```
 
-8. You can create a new user-defined function (UDF) that wraps around your custom vision model or an off-the-shelf model like FastRCNN:
+- You can **create a custom user-defined function (UDF)** that wraps around a fine-tuned or off-the-shelf deep learning model:
 ```mysql
 CREATE UDF IF NOT EXISTS MyUDF
 INPUT  (frame NDARRAY UINT8(3, ANYDIM, ANYDIM))
 OUTPUT (labels NDARRAY STR(ANYDIM), bboxes NDARRAY FLOAT32(ANYDIM, 4),
         scores NDARRAY FLOAT32(ANYDIM))
 TYPE  Classification
 IMPL  'eva/udfs/fastrcnn_object_detector.py';
 ```
 
-9. You can combine multiple user-defined functions in a single query to accomplish more complicated tasks.
+- **Compose multiple user-defined functions in a single query** to accomplish complicated AI pipelines.
 ```mysql
    -- Analyse emotions of faces in a video
    SELECT id, bbox, EmotionDetector(Crop(data, bbox)) 
    FROM MyVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)  
    WHERE id < 15;
 ```
 
+- Besides making it easy to write queries for complex AI pipelines, EVA **speeds up query execution using its AI-centric query optimizer**. Two illustrative  optimizations are:
+
+   💾 **Caching**: EVA automatically caches and reuses previous query results (especially model inference results), eliminating redundant computation and reducing query processing time.
+
+   🎯 **Predicate Reordering**: EVA optimizes the order in which the query predicates are evaluated (e.g., runs the faster, more selective model first), leading to faster queries and lower inference costs.
+
+Consider these two exploratory queries on a dataset of dog images:
+<img align="right" style="display:inline;" width="40%" src="https://github.com/georgia-tech-db/eva/blob/master/data/assets/eva_performance_comparison.png?raw=true"></a>
+
+```mysql
+  -- Query 1: Find all images of black-colored dogs
+  SELECT id, bbox FROM dogs 
+  JOIN LATERAL UNNEST(YoloV5(data)) AS Obj(label, bbox, score) 
+  WHERE Obj.label = 'dog' 
+    AND Color(Crop(data, bbox)) = 'black'; 
+
+  -- Query 2: Find all Great Danes that are black-colored
+  SELECT id, bbox FROM dogs 
+  JOIN LATERAL UNNEST(YoloV5(data)) AS Obj(label, bbox, score) 
+  WHERE Obj.label = 'dog' 
+    AND DogBreedClassifier(Crop(data, bbox)) = 'great dane' 
+    AND Color(Crop(data, bbox)) = 'black';
+```
+
+By reusing the results of the first query and reordering the predicates based on available cached results, EVA runs up the second query **10x faster**!
+
 ## Illustrative EVA Applications 
 
 ### Traffic Analysis (Object Detection Model)
 | Source Video  | Query Result |
 |---------------|--------------|
 |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
 
@@ -172,16 +208,15 @@
 ## Contributing to EVA
 
 [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb)
 [![CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva)
 [![Coverage Status](https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master)](https://coveralls.io/github/georgia-tech-db/eva?branch=master)
 [![Documentation Status](https://readthedocs.org/projects/evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/index.html)
 
-We welcome all kinds of contributions to EVA.
-To file a bug or request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
+EVA is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EVA are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
 
-For more information on contributing to EVA, see our
+For more information, see our
 [contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
 
 ## License
-Copyright (c) 2018-2023 [Georgia Tech Database Group](http://db.cc.gatech.edu/)
+Copyright (c) 2018-2023 [Georgia Tech Database Group](http://db.cc.gatech.edu/).
 Licensed under [Apache License](LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,96 +1,117 @@
 [EVA]
 **** Try It Out! ****
-[Open_EVA_on_Colab] [Slack] [Discuss_on_Github!] [PyPI] [License] [Python
-Versions]
-# EVA AI-Relational Database System EVA is an open-source **AI-relational
-database with first-class support for deep learning models**. It aims to
-support AI-powered database applications that operate on both structured
-(tables) and unstructured data (videos, text, podcasts, PDFs, etc.) with deep
-learning models. EVA accelerates AI pipelines using a collection of
-optimizations inspired by relational database systems including function
-caching, sampling, and cost-based operator reordering. It comes with a wide
-range of models for analyzing unstructured data including image classification,
-object detection, OCR, face detection, etc. It is fully implemented in Python,
-and licensed under the Apache license. EVA supports a AI-oriented query
-language for analysing unstructured data. Here are some illustrative
-applications: * Examining_the_emotion_palette_of_actors_in_a_movie * Analysing
-traffic_flow_at_an_intersection * Classifying_images_based_on_their_content *
-Recogizing_license_plates * Analysing_toxicity_of_social_media_memes If you are
-wondering why you might need a AI-relational database system, start with the
-page on Video_Database_Systems. It describes how EVA lets you easily make use
-of deep learning models and you can save money spent on inference on large
-image or video datasets. The Getting_Started page shows how you can use EVA for
-different computer vision tasks: image classification, object detection, action
-recognition, and how you can easily extend EVA to support your custom deep
-learning model in the form of user-defined functions. The User_Guides section
-contains Jupyter Notebooks that demonstrate how to use various features of EVA.
-Each notebook includes a link to Google Colab, where you can run the code by
-yourself. ## Why EVA? ##  Easily combine SQL and Deep Learning to build next-
-generation database applications Easily query videos in user-facing
-applications with a SQL-like interface for commonly used computer vision
-models.   Speed up queries and save money spent on model inference EVA comes
-with a collection of built-in sampling, caching, and filtering optimizations
+[Logo] [Open_EVA_on_Colab] [Slack] [Discuss_on_Github!] [PyPI] [License]
+[Python Versions]
+# EVA AI-Relational Database System - â¡ï¸ 10-100x faster AI pipelines using
+SQL-like queries - ð° Save money spent on GPU-driven inference - ð¦ Built-
+in caching to avoid re-running deep learning models across queries - ð Over
+20 AI-centric query optimization rules - â¨ï¸ First-party integrations for
+PyTorch and HuggingFace models - ð Installable via pip - ð¤ Fully
+implemented in Python EVA is an open-source **AI-relational database with
+first-class support for deep learning models**. It supports next-generation AI-
+powered database applications that operate on structured (tables) and
+unstructured data (videos, text, podcasts, PDFs, etc.) with deep learning
+models. EVA accelerates AI pipelines by 10-100x using a collection of
+optimizations inspired by relational database systems, including function
+caching, sampling, and cost-based predicate reordering. It comes with a wide
+range of models for analyzing unstructured data, including models for image
+classification, object detection, OCR, text sentiment classification, face
+detection, etc. It is fully implemented in Python and licensed under the Apache
+license. EVA supports an AI-oriented query language tailored for analyzing
+unstructured data. Here are some illustrative applications: * Examining_the
+emotion_palette_of_actors_in_a_movie * Analysing_traffic_flow_at_an
+intersection * Classifying_images_based_on_their_content * Recognizing_license
+plates * Analysing_toxicity_of_social_media_memes If you are wondering why you
+might need an AI-relational database system, start with the page on Video
+Database_Systems. It describes how EVA lets you easily use deep learning models
+and save money spent on GPU-driven inference on large image or video datasets.
+The Getting_Started page shows how you can use EVA for different computer
+vision tasks: image classification, object detection, action recognition, and
+how you can easily extend EVA to support your custom deep learning model in the
+form of user-defined functions. The User_Guides section contains Jupyter
+Notebooks that demonstrate how to use various features of EVA. Each notebook
+includes a link to Google Colab to run the code. ## Why EVA? ##  Easily combine
+SQL and Deep Learning to build next-generation database applications Easily
+query videos in user-facing applications with a SQL-like interface for commonly
+used computer vision models.   Speed up queries and save money spent on model
+inference EVA has built-in sampling, caching, and filtering optimizations
 inspired by time-tested relational database systems.   Extensible by design to
 support custom deep learning models EVA has first-class support for user-
-defined functions that wrap around your deep learning models in PyTorch.  ##
-Links * [Documentation](https://evadb.readthedocs.io/) * [Tutorials](https://
-github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
-* [Join Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-
-PlJ4iawLdurDv~aIAq90Dg) * [Demo](https://ada-00.cc.gatech.edu/eva/playground)
-## Quick Start 1. To install EVA, we recommend using the pip package manager
-(EVA supports Python versions 3.7+). ```shell pip install evadb ``` 2. EVA is
-based on a client-server architecture. It works in Jupyter notebooks
-(illustrative notebooks are available in the [Tutorials](https://github.com/
-georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb) folder)
-and also supports a terminal-based client. To start the EVA server and a
-terminal-based client, use the following commands: ```shell eva_server & #
-launch server eva_client # launch client ``` 3. Load a video onto the EVA
-server from the client (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4)
-video as an example): ```mysql LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO
-MyVideo; ``` 4. That's it! You can now run queries over the loaded video:
-```mysql SELECT id, data FROM MyVideo WHERE id < 5; ``` 5. Search for frames in
-the video that contain a car ```mysql SELECT id, data FROM MyVideo WHERE
-['car'] <@ FastRCNNObjectDetector(data).labels; ``` | Source Video | Query
-Result | |---------------|--------------| |[Source Video] |[Query Result] | 6.
-Search for frames in the video that contain a pedestrian and a car ```mysql
-SELECT id, data FROM MyVideo WHERE ['pedestrian', 'car'] <@
-FastRCNNObjectDetector(data).labels; ``` 7. Search for frames in the video with
-more than 3 cars ```mysql SELECT id, data FROM MyVideo WHERE ArrayCount
-(FastRCNNObjectDetector(data).labels, 'car') > 3; ``` 8. You can create a new
-user-defined function (UDF) that wraps around your custom vision model or an
-off-the-shelf model like FastRCNN: ```mysql CREATE UDF IF NOT EXISTS MyUDF
-INPUT (frame NDARRAY UINT8(3, ANYDIM, ANYDIM)) OUTPUT (labels NDARRAY STR
-(ANYDIM), bboxes NDARRAY FLOAT32(ANYDIM, 4), scores NDARRAY FLOAT32(ANYDIM))
-TYPE Classification IMPL 'eva/udfs/fastrcnn_object_detector.py'; ``` 9. You can
-combine multiple user-defined functions in a single query to accomplish more
-complicated tasks. ```mysql -- Analyse emotions of faces in a video SELECT id,
-bbox, EmotionDetector(Crop(data, bbox)) FROM MyVideo JOIN LATERAL UNNEST
-(FaceDetector(data)) AS Face(bbox, conf) WHERE id < 15; ``` ## Illustrative EVA
-Applications ### Traffic Analysis (Object Detection Model) | Source Video |
-Query Result | |---------------|--------------| |[Source Video] |[Query Result]
-| ### MNIST Digit Recognition (Image Classification Model) | Source Video |
-Query Result | |---------------|--------------| |[Source Video] |[Query Result]
-| ### Movie Analysis (Face Detection + Emotion Classfication Models) | Source
-Video | Query Result | |---------------|--------------| |[Source Video] |[Query
-Result] | ### [License Plate Recognition](https://github.com/georgia-tech-db/
-eva-application-template) (Plate Detection + OCR Extraction Models) | Query
-Result | |--------------| [Query Result] | ### [Meme Toxicity Classification]
-(https://github.com/georgia-tech-db/toxicity-classification) (OCR Extraction +
-Toxicity Classification Models) | Query Result | |--------------| [Query
-Result] | ## Community Join the EVA community on [Slack](https://
-join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) to
-ask questions and to share your ideas for improving EVA. [EVA_Slack_Channel]
-### Architecture Diagram of EVA [EVA Architecture Diagram] ## Contributing to
-EVA [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://
-pypi.org/project/evadb) [![CI Status](https://circleci.com/gh/georgia-tech-db/
-eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva) [![Coverage
-Status](https://coveralls.io/repos/github/georgia-tech-db/eva/
-badge.svg?branch=master)](https://coveralls.io/github/georgia-tech-db/
-eva?branch=master) [![Documentation Status](https://readthedocs.org/projects/
-evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/
-index.html) We welcome all kinds of contributions to EVA. To file a bug or
-request a feature, please use GitHub_issues. Pull_requests are welcome. For
-more information on contributing to EVA, see our [contribution guide](https://
-evadb.readthedocs.io/en/stable/source/contribute/index.html). ## License
-Copyright (c) 2018-2023 [Georgia Tech Database Group](http://db.cc.gatech.edu/
-) Licensed under [Apache License](LICENSE).
+defined functions that wrap around your deep learning models in PyTorch and
+HuggingFace.  ## Links * [Documentation](https://evadb.readthedocs.io/) *
+[Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-
+emotion-analysis.ipynb) * [Join Slack](https://join.slack.com/t/eva-db/
+shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Demo](https://ada-
+00.cc.gatech.edu/eva/playground) ## Quick Start - Install EVA using the pip
+package manager. EVA supports Python versions 3.7+. ```shell pip install evadb
+``` - To start and connect to an EVA server in a Jupyter notebook, check out
+this [illustrative emotion analysis notebook](https://github.com/georgia-tech-
+db/eva/blob/master/tutorials/03-emotion-analysis.ipynb): ```shell cursor =
+connect_to_server() ``` - Load a video onto the EVA server (we use
+[ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration): ```mysql LOAD
+VIDEO "data/ua_detrac/ua_detrac.mp4" INTO UADETRAC; ``` - That's it! You can
+now run queries over the loaded video: ```mysql SELECT id, data FROM UADETRAC
+WHERE id < 5; ``` - Search for frames in the video that contain a car ```mysql
+SELECT id, data FROM UADETRAC WHERE ['car'] <@ YoloV5(data).labels; ``` |
+Source Video | Query Result | |---------------|--------------| |[Source Video]
+|[Query Result] | - Search for frames in the video that contain a pedestrian
+and a car ```mysql SELECT id, data FROM UADETRAC WHERE ['pedestrian', 'car'] <@
+YoloV5(data).labels; ``` - Search for frames with more than three cars ```mysql
+SELECT id, data FROM UADETRAC WHERE ArrayCount(YoloV5(data).labels, 'car') > 3;
+``` - You can **create a custom user-defined function (UDF)** that wraps around
+a fine-tuned or off-the-shelf deep learning model: ```mysql CREATE UDF IF NOT
+EXISTS MyUDF INPUT (frame NDARRAY UINT8(3, ANYDIM, ANYDIM)) OUTPUT (labels
+NDARRAY STR(ANYDIM), bboxes NDARRAY FLOAT32(ANYDIM, 4), scores NDARRAY FLOAT32
+(ANYDIM)) TYPE Classification IMPL 'eva/udfs/fastrcnn_object_detector.py'; ```
+- **Compose multiple user-defined functions in a single query** to accomplish
+complicated AI pipelines. ```mysql -- Analyse emotions of faces in a video
+SELECT id, bbox, EmotionDetector(Crop(data, bbox)) FROM MyVideo JOIN LATERAL
+UNNEST(FaceDetector(data)) AS Face(bbox, conf) WHERE id < 15; ``` - Besides
+making it easy to write queries for complex AI pipelines, EVA **speeds up query
+execution using its AI-centric query optimizer**. Two illustrative
+optimizations are: ð¾ **Caching**: EVA automatically caches and reuses
+previous query results (especially model inference results), eliminating
+redundant computation and reducing query processing time. ð¯ **Predicate
+Reordering**: EVA optimizes the order in which the query predicates are
+evaluated (e.g., runs the faster, more selective model first), leading to
+faster queries and lower inference costs. Consider these two exploratory
+queries on a dataset of dog images: [https://github.com/georgia-tech-db/eva/
+blob/master/data/assets/eva_performance_comparison.png?raw=true]
+ ```mysql -- Query 1: Find all images of black-colored dogs SELECT id, bbox
+FROM dogs JOIN LATERAL UNNEST(YoloV5(data)) AS Obj(label, bbox, score) WHERE
+Obj.label = 'dog' AND Color(Crop(data, bbox)) = 'black'; -- Query 2: Find all
+Great Danes that are black-colored SELECT id, bbox FROM dogs JOIN LATERAL
+UNNEST(YoloV5(data)) AS Obj(label, bbox, score) WHERE Obj.label = 'dog' AND
+DogBreedClassifier(Crop(data, bbox)) = 'great dane' AND Color(Crop(data, bbox))
+= 'black'; ``` By reusing the results of the first query and reordering the
+predicates based on available cached results, EVA runs up the second query
+**10x faster**! ## Illustrative EVA Applications ### Traffic Analysis (Object
+Detection Model) | Source Video | Query Result | |---------------|-------------
+-| |[Source Video] |[Query Result] | ### MNIST Digit Recognition (Image
+Classification Model) | Source Video | Query Result | |---------------|--------
+------| |[Source Video] |[Query Result] | ### Movie Analysis (Face Detection +
+Emotion Classfication Models) | Source Video | Query Result | |---------------
+|--------------| |[Source Video] |[Query Result] | ### [License Plate
+Recognition](https://github.com/georgia-tech-db/eva-application-template)
+(Plate Detection + OCR Extraction Models) | Query Result | |--------------|
+[Query Result] | ### [Meme Toxicity Classification](https://github.com/georgia-
+tech-db/toxicity-classification) (OCR Extraction + Toxicity Classification
+Models) | Query Result | |--------------| [Query Result] | ## Community Join
+the EVA community on [Slack](https://join.slack.com/t/eva-db/shared_invite/zt-
+1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) to ask questions and to share your ideas for
+improving EVA. [EVA_Slack_Channel] ### Architecture Diagram of EVA [EVA
+Architecture Diagram] ## Contributing to EVA [![PyPI Version](https://
+img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb) [![CI Status]
+(https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://
+circleci.com/gh/georgia-tech-db/eva) [![Coverage Status](https://coveralls.io/
+repos/github/georgia-tech-db/eva/badge.svg?branch=master)](https://
+coveralls.io/github/georgia-tech-db/eva?branch=master) [![Documentation Status]
+(https://readthedocs.org/projects/evadb/badge/?version=stable)](https://
+evadb.readthedocs.io/en/stable/index.html) EVA is the beneficiary of many
+[contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All
+kinds of contributions to EVA are appreciated. To file a bug or to request a
+feature, please use GitHub_issues. Pull_requests are welcome. For more
+information, see our [contribution guide](https://evadb.readthedocs.io/en/
+stable/source/contribute/index.html). ## License Copyright (c) 2018-2023
+[Georgia Tech Database Group](http://db.cc.gatech.edu/). Licensed under [Apache
+License](LICENSE).
```

### Comparing `evadb-0.2.0/eva/__init__.py` & `evadb-0.2.1/eva/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/binder/__init__.py` & `evadb-0.2.1/eva/binder/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/binder/binder_utils.py` & `evadb-0.2.1/eva/binder/binder_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/binder/statement_binder.py` & `evadb-0.2.1/eva/binder/statement_binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/binder/statement_binder_context.py` & `evadb-0.2.1/eva/binder/statement_binder_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/__init__.py` & `evadb-0.2.1/eva/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/catalog_manager.py` & `evadb-0.2.1/eva/catalog/catalog_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/catalog_type.py` & `evadb-0.2.1/eva/catalog/catalog_type.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/catalog_utils.py` & `evadb-0.2.1/eva/catalog/catalog_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/models/__init__.py` & `evadb-0.2.1/eva/catalog/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/models/association_models.py` & `evadb-0.2.1/eva/catalog/models/association_models.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/models/base_model.py` & `evadb-0.2.1/eva/catalog/models/base_model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/models/column_catalog.py` & `evadb-0.2.1/eva/catalog/models/column_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/models/index_catalog.py` & `evadb-0.2.1/eva/catalog/models/index_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/models/table_catalog.py` & `evadb-0.2.1/eva/catalog/models/table_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/models/udf_cache_catalog.py` & `evadb-0.2.1/eva/catalog/models/udf_cache_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/models/udf_catalog.py` & `evadb-0.2.1/eva/catalog/models/udf_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/models/udf_cost_catalog.py` & `evadb-0.2.1/eva/catalog/models/udf_cost_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/models/udf_io_catalog.py` & `evadb-0.2.1/eva/catalog/models/udf_io_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/models/udf_metadata_catalog.py` & `evadb-0.2.1/eva/catalog/models/udf_metadata_catalog.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/schema_utils.py` & `evadb-0.2.1/eva/catalog/schema_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/services/__init__.py` & `evadb-0.2.1/eva/catalog/services/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/services/base_service.py` & `evadb-0.2.1/eva/catalog/services/base_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/services/column_catalog_service.py` & `evadb-0.2.1/eva/catalog/services/column_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/services/index_catalog_service.py` & `evadb-0.2.1/eva/catalog/services/index_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/services/table_catalog_service.py` & `evadb-0.2.1/eva/catalog/services/table_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/services/udf_cache_catalog_service.py` & `evadb-0.2.1/eva/catalog/services/udf_cache_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/services/udf_catalog_service.py` & `evadb-0.2.1/eva/catalog/services/udf_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/services/udf_cost_catalog_service.py` & `evadb-0.2.1/eva/catalog/services/udf_cost_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/services/udf_io_catalog_service.py` & `evadb-0.2.1/eva/catalog/services/udf_io_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/services/udf_metadata_catalog_service.py` & `evadb-0.2.1/eva/catalog/services/udf_metadata_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/catalog/sql_config.py` & `evadb-0.2.1/eva/catalog/sql_config.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/configuration/__init__.py` & `evadb-0.2.1/eva/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/configuration/bootstrap_environment.py` & `evadb-0.2.1/eva/configuration/bootstrap_environment.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/configuration/configuration_manager.py` & `evadb-0.2.1/eva/configuration/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/configuration/constants.py` & `evadb-0.2.1/eva/configuration/constants.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/constants.py` & `evadb-0.2.1/eva/constants.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/eva.yml` & `evadb-0.2.1/eva/eva.yml`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/eva_cmd_client.py` & `evadb-0.2.1/eva/eva_cmd_client.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/eva_server.py` & `evadb-0.2.1/eva/eva_server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/__init__.py` & `evadb-0.2.1/eva/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/abstract_executor.py` & `evadb-0.2.1/eva/executor/abstract_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/apply_and_merge_executor.py` & `evadb-0.2.1/eva/executor/apply_and_merge_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/create_executor.py` & `evadb-0.2.1/eva/executor/create_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/create_index_executor.py` & `evadb-0.2.1/eva/executor/create_index_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/create_mat_view_executor.py` & `evadb-0.2.1/eva/executor/create_mat_view_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/create_udf_executor.py` & `evadb-0.2.1/eva/executor/create_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/delete_executor.py` & `evadb-0.2.1/eva/executor/delete_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/drop_executor.py` & `evadb-0.2.1/eva/executor/drop_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/drop_udf_executor.py` & `evadb-0.2.1/eva/executor/drop_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/execution_context.py` & `evadb-0.2.1/eva/executor/execution_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/executor_utils.py` & `evadb-0.2.1/eva/executor/executor_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/explain_executor.py` & `evadb-0.2.1/eva/executor/explain_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/faiss_index_scan_executor.py` & `evadb-0.2.1/eva/executor/faiss_index_scan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/function_scan_executor.py` & `evadb-0.2.1/eva/executor/function_scan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/groupby_executor.py` & `evadb-0.2.1/eva/executor/groupby_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/hash_join_executor.py` & `evadb-0.2.1/eva/executor/hash_join_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/insert_executor.py` & `evadb-0.2.1/eva/executor/insert_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/join_build_executor.py` & `evadb-0.2.1/eva/executor/join_build_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/lateral_join_executor.py` & `evadb-0.2.1/eva/executor/lateral_join_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/limit_executor.py` & `evadb-0.2.1/eva/executor/limit_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/load_csv_executor.py` & `evadb-0.2.1/eva/executor/load_csv_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/load_executor.py` & `evadb-0.2.1/eva/executor/load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/load_multimedia_executor.py` & `evadb-0.2.1/eva/executor/load_multimedia_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/nested_loop_join_executor.py` & `evadb-0.2.1/eva/executor/nested_loop_join_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/orderby_executor.py` & `evadb-0.2.1/eva/executor/orderby_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/plan_executor.py` & `evadb-0.2.1/eva/executor/plan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/pp_executor.py` & `evadb-0.2.1/eva/executor/pp_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/predicate_executor.py` & `evadb-0.2.1/eva/executor/predicate_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/project_executor.py` & `evadb-0.2.1/eva/executor/project_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/rename_executor.py` & `evadb-0.2.1/eva/executor/rename_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/sample_executor.py` & `evadb-0.2.1/eva/executor/sample_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/seq_scan_executor.py` & `evadb-0.2.1/eva/executor/seq_scan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/show_info_executor.py` & `evadb-0.2.1/eva/executor/show_info_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/storage_executor.py` & `evadb-0.2.1/eva/executor/storage_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/executor/union_executor.py` & `evadb-0.2.1/eva/executor/union_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/experimental/__init__.py` & `evadb-0.2.1/eva/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/experimental/ray/__init__.py` & `evadb-0.2.1/eva/experimental/ray/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/experimental/ray/executor/__init__.py` & `evadb-0.2.1/eva/experimental/ray/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/experimental/ray/executor/exchange_executor.py` & `evadb-0.2.1/eva/experimental/ray/executor/exchange_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/experimental/ray/executor/ray_stage.py` & `evadb-0.2.1/eva/experimental/ray/executor/ray_stage.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/experimental/ray/optimizer/__init__.py` & `evadb-0.2.1/eva/experimental/ray/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/experimental/ray/optimizer/rules/__init__.py` & `evadb-0.2.1/eva/experimental/ray/optimizer/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/experimental/ray/optimizer/rules/rules.py` & `evadb-0.2.1/eva/experimental/ray/optimizer/rules/rules.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/experimental/ray/planner/__init__.py` & `evadb-0.2.1/eva/experimental/ray/planner/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/experimental/ray/planner/exchange_plan.py` & `evadb-0.2.1/eva/experimental/ray/planner/exchange_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/expression/__init__.py` & `evadb-0.2.1/eva/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/expression/abstract_expression.py` & `evadb-0.2.1/eva/expression/abstract_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/expression/aggregation_expression.py` & `evadb-0.2.1/eva/expression/aggregation_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/expression/arithmetic_expression.py` & `evadb-0.2.1/eva/expression/arithmetic_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/expression/comparison_expression.py` & `evadb-0.2.1/eva/expression/comparison_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/expression/constant_value_expression.py` & `evadb-0.2.1/eva/expression/constant_value_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/expression/expression_utils.py` & `evadb-0.2.1/eva/expression/expression_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/expression/function_expression.py` & `evadb-0.2.1/eva/expression/function_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/expression/logical_expression.py` & `evadb-0.2.1/eva/expression/logical_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/expression/tuple_value_expression.py` & `evadb-0.2.1/eva/expression/tuple_value_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/models/__init__.py` & `evadb-0.2.1/eva/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/models/catalog/__init__.py` & `evadb-0.2.1/eva/models/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/models/catalog/frame_info.py` & `evadb-0.2.1/eva/models/catalog/frame_info.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/models/catalog/properties.py` & `evadb-0.2.1/eva/models/catalog/properties.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/models/server/__init__.py` & `evadb-0.2.1/eva/models/server/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/models/server/response.py` & `evadb-0.2.1/eva/models/server/response.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/models/storage/__init__.py` & `evadb-0.2.1/eva/models/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/models/storage/batch.py` & `evadb-0.2.1/eva/models/storage/batch.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/optimizer/__init__.py` & `evadb-0.2.1/eva/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/optimizer/binder.py` & `evadb-0.2.1/eva/optimizer/binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/optimizer/cost_model.py` & `evadb-0.2.1/eva/optimizer/cost_model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/optimizer/group.py` & `evadb-0.2.1/eva/optimizer/group.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/optimizer/group_expression.py` & `evadb-0.2.1/eva/optimizer/group_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/optimizer/memo.py` & `evadb-0.2.1/eva/optimizer/memo.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/optimizer/operators.py` & `evadb-0.2.1/eva/optimizer/operators.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/optimizer/optimizer_context.py` & `evadb-0.2.1/eva/optimizer/optimizer_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/optimizer/optimizer_task_stack.py` & `evadb-0.2.1/eva/optimizer/optimizer_task_stack.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/optimizer/optimizer_tasks.py` & `evadb-0.2.1/eva/optimizer/optimizer_tasks.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/optimizer/optimizer_utils.py` & `evadb-0.2.1/eva/optimizer/optimizer_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/optimizer/plan_generator.py` & `evadb-0.2.1/eva/optimizer/plan_generator.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/optimizer/property.py` & `evadb-0.2.1/eva/optimizer/property.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/optimizer/rules/__init__.py` & `evadb-0.2.1/eva/optimizer/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/optimizer/rules/pattern.py` & `evadb-0.2.1/eva/optimizer/rules/pattern.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/optimizer/rules/rules.py` & `evadb-0.2.1/eva/optimizer/rules/rules.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/optimizer/rules/rules_base.py` & `evadb-0.2.1/eva/optimizer/rules/rules_base.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/optimizer/rules/rules_manager.py` & `evadb-0.2.1/eva/optimizer/rules/rules_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/optimizer/statement_to_opr_convertor.py` & `evadb-0.2.1/eva/optimizer/statement_to_opr_convertor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/__init__.py` & `evadb-0.2.1/eva/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/alias.py` & `evadb-0.2.1/eva/parser/alias.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/create_index_statement.py` & `evadb-0.2.1/eva/parser/create_index_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/create_mat_view_statement.py` & `evadb-0.2.1/eva/parser/create_mat_view_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/create_statement.py` & `evadb-0.2.1/eva/parser/create_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/create_udf_statement.py` & `evadb-0.2.1/eva/parser/create_udf_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/delete_statement.py` & `evadb-0.2.1/eva/parser/delete_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/drop_statement.py` & `evadb-0.2.1/eva/parser/drop_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/drop_udf_statement.py` & `evadb-0.2.1/eva/parser/drop_udf_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/eva.lark` & `evadb-0.2.1/eva/parser/eva.lark`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/evaql/evaql_lexer.py` & `evadb-0.2.1/eva/parser/evaql/evaql_lexer.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/evaql/evaql_parser.py` & `evadb-0.2.1/eva/parser/evaql/evaql_parser.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/evaql/evaql_parserListener.py` & `evadb-0.2.1/eva/parser/evaql/evaql_parserListener.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/evaql/evaql_parserVisitor.py` & `evadb-0.2.1/eva/parser/evaql/evaql_parserVisitor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/explain_statement.py` & `evadb-0.2.1/eva/parser/explain_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/insert_statement.py` & `evadb-0.2.1/eva/parser/insert_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/lark_parser.py` & `evadb-0.2.1/eva/parser/lark_parser.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/lark_visitor/__init__.py` & `evadb-0.2.1/eva/parser/lark_visitor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/lark_visitor/_common_clauses_ids.py` & `evadb-0.2.1/eva/parser/lark_visitor/_common_clauses_ids.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/lark_visitor/_create_statements.py` & `evadb-0.2.1/eva/parser/lark_visitor/_create_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/lark_visitor/_delete_statement.py` & `evadb-0.2.1/eva/parser/lark_visitor/_delete_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/lark_visitor/_drop_statement.py` & `evadb-0.2.1/eva/parser/lark_visitor/_drop_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/lark_visitor/_explain_statement.py` & `evadb-0.2.1/eva/parser/lark_visitor/_explain_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/lark_visitor/_expressions.py` & `evadb-0.2.1/eva/parser/lark_visitor/_expressions.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/lark_visitor/_functions.py` & `evadb-0.2.1/eva/parser/lark_visitor/_functions.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/lark_visitor/_insert_statements.py` & `evadb-0.2.1/eva/parser/lark_visitor/_insert_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/lark_visitor/_load_statement.py` & `evadb-0.2.1/eva/parser/lark_visitor/_load_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/lark_visitor/_rename_statement.py` & `evadb-0.2.1/eva/parser/lark_visitor/_rename_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/lark_visitor/_select_statement.py` & `evadb-0.2.1/eva/parser/lark_visitor/_select_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/lark_visitor/_show_statements.py` & `evadb-0.2.1/eva/parser/lark_visitor/_show_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/lark_visitor/_table_sources.py` & `evadb-0.2.1/eva/parser/lark_visitor/_table_sources.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/load_statement.py` & `evadb-0.2.1/eva/parser/load_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/parser.py` & `evadb-0.2.1/eva/parser/parser.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/rename_statement.py` & `evadb-0.2.1/eva/parser/rename_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/select_statement.py` & `evadb-0.2.1/eva/parser/select_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/show_statement.py` & `evadb-0.2.1/eva/parser/show_statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/statement.py` & `evadb-0.2.1/eva/parser/statement.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/table_ref.py` & `evadb-0.2.1/eva/parser/table_ref.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/parser/types.py` & `evadb-0.2.1/eva/parser/types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/__init__.py` & `evadb-0.2.1/eva/plan_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/abstract_join_plan.py` & `evadb-0.2.1/eva/plan_nodes/abstract_join_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/abstract_plan.py` & `evadb-0.2.1/eva/plan_nodes/abstract_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/abstract_scan_plan.py` & `evadb-0.2.1/eva/plan_nodes/abstract_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/apply_and_merge_plan.py` & `evadb-0.2.1/eva/plan_nodes/apply_and_merge_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/create_index_plan.py` & `evadb-0.2.1/eva/plan_nodes/create_index_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/create_mat_view_plan.py` & `evadb-0.2.1/eva/plan_nodes/create_mat_view_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/create_plan.py` & `evadb-0.2.1/eva/plan_nodes/create_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/create_udf_plan.py` & `evadb-0.2.1/eva/plan_nodes/create_udf_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/delete_plan.py` & `evadb-0.2.1/eva/plan_nodes/delete_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/drop_plan.py` & `evadb-0.2.1/eva/plan_nodes/drop_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/drop_udf_plan.py` & `evadb-0.2.1/eva/plan_nodes/drop_udf_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/explain_plan.py` & `evadb-0.2.1/eva/plan_nodes/explain_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/faiss_index_scan_plan.py` & `evadb-0.2.1/eva/plan_nodes/faiss_index_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/function_scan_plan.py` & `evadb-0.2.1/eva/plan_nodes/function_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/groupby_plan.py` & `evadb-0.2.1/eva/plan_nodes/groupby_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/hash_join_build_plan.py` & `evadb-0.2.1/eva/plan_nodes/hash_join_build_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/hash_join_probe_plan.py` & `evadb-0.2.1/eva/plan_nodes/hash_join_probe_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/insert_plan.py` & `evadb-0.2.1/eva/plan_nodes/insert_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/lateral_join_plan.py` & `evadb-0.2.1/eva/plan_nodes/lateral_join_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/limit_plan.py` & `evadb-0.2.1/eva/plan_nodes/limit_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/load_data_plan.py` & `evadb-0.2.1/eva/plan_nodes/load_data_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/nested_loop_join_plan.py` & `evadb-0.2.1/eva/plan_nodes/nested_loop_join_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/orderby_plan.py` & `evadb-0.2.1/eva/plan_nodes/orderby_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/pp_plan.py` & `evadb-0.2.1/eva/plan_nodes/pp_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/predicate_plan.py` & `evadb-0.2.1/eva/plan_nodes/predicate_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/project_plan.py` & `evadb-0.2.1/eva/plan_nodes/project_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/rename_plan.py` & `evadb-0.2.1/eva/plan_nodes/rename_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/sample_plan.py` & `evadb-0.2.1/eva/plan_nodes/sample_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/seq_scan_plan.py` & `evadb-0.2.1/eva/plan_nodes/seq_scan_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/show_info_plan.py` & `evadb-0.2.1/eva/plan_nodes/show_info_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/storage_plan.py` & `evadb-0.2.1/eva/plan_nodes/storage_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/types.py` & `evadb-0.2.1/eva/plan_nodes/types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/plan_nodes/union_plan.py` & `evadb-0.2.1/eva/plan_nodes/union_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/readers/__init__.py` & `evadb-0.2.1/eva/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/readers/abstract_reader.py` & `evadb-0.2.1/eva/readers/abstract_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/readers/csv_reader.py` & `evadb-0.2.1/eva/readers/csv_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/readers/decord_reader.py` & `evadb-0.2.1/eva/readers/decord_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/readers/image/__init__.py` & `evadb-0.2.1/eva/readers/image/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/readers/image/opencv_image_reader.py` & `evadb-0.2.1/eva/readers/image/opencv_image_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/server/__init__.py` & `evadb-0.2.1/eva/server/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/server/command_handler.py` & `evadb-0.2.1/eva/server/command_handler.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/server/db_api.py` & `evadb-0.2.1/eva/server/db_api.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/server/interpreter.py` & `evadb-0.2.1/eva/server/interpreter.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/server/server.py` & `evadb-0.2.1/eva/server/server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/storage/__init__.py` & `evadb-0.2.1/eva/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/storage/abstract_media_storage_engine.py` & `evadb-0.2.1/eva/storage/abstract_media_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/storage/abstract_storage_engine.py` & `evadb-0.2.1/eva/storage/abstract_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/storage/image_storage_engine.py` & `evadb-0.2.1/eva/storage/image_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/storage/sqlite_storage_engine.py` & `evadb-0.2.1/eva/storage/sqlite_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/storage/storage_engine.py` & `evadb-0.2.1/eva/storage/storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/storage/video_storage_engine.py` & `evadb-0.2.1/eva/storage/video_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/third_party/__init__.py` & `evadb-0.2.1/eva/third_party/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/third_party/huggingface/__init__.py` & `evadb-0.2.1/eva/third_party/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/third_party/huggingface/binder.py` & `evadb-0.2.1/eva/third_party/huggingface/binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/third_party/huggingface/create.py` & `evadb-0.2.1/eva/third_party/huggingface/create.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/third_party/huggingface/model.py` & `evadb-0.2.1/eva/third_party/huggingface/model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/__init__.py` & `evadb-0.2.1/eva/udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/abstract/__init__.py` & `evadb-0.2.1/eva/udfs/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/abstract/abstract_udf.py` & `evadb-0.2.1/eva/udfs/abstract/abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/abstract/hf_abstract_udf.py` & `evadb-0.2.1/eva/udfs/abstract/hf_abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/abstract/pytorch_abstract_udf.py` & `evadb-0.2.1/eva/udfs/abstract/pytorch_abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/asl_action_recognition.py` & `evadb-0.2.1/eva/udfs/asl_action_recognition.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/decorators/__init__.py` & `evadb-0.2.1/eva/udfs/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/decorators/decorators.py` & `evadb-0.2.1/eva/udfs/decorators/decorators.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/decorators/io_descriptors/__init__.py` & `evadb-0.2.1/eva/udfs/decorators/io_descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/decorators/io_descriptors/abstract_types.py` & `evadb-0.2.1/eva/udfs/decorators/io_descriptors/abstract_types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/decorators/io_descriptors/data_types.py` & `evadb-0.2.1/eva/udfs/decorators/io_descriptors/data_types.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/decorators/utils.py` & `evadb-0.2.1/eva/udfs/decorators/utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/decorators/yolo_object_detection_decorators.py` & `evadb-0.2.1/eva/udfs/decorators/yolo_object_detection_decorators.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/emotion_detector.py` & `evadb-0.2.1/eva/udfs/emotion_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/face_detector.py` & `evadb-0.2.1/eva/udfs/face_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/fastrcnn_object_detector.py` & `evadb-0.2.1/eva/udfs/fastrcnn_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/feature_extractor.py` & `evadb-0.2.1/eva/udfs/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/gpu_compatible.py` & `evadb-0.2.1/eva/udfs/gpu_compatible.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/mvit_action_recognition.py` & `evadb-0.2.1/eva/udfs/mvit_action_recognition.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/ndarray/__init__.py` & `evadb-0.2.1/eva/udfs/ndarray/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/ndarray/array_count.py` & `evadb-0.2.1/eva/udfs/ndarray/array_count.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/ndarray/crop.py` & `evadb-0.2.1/eva/udfs/ndarray/crop.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/ndarray/fuzzy_join.py` & `evadb-0.2.1/eva/udfs/ndarray/fuzzy_join.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/ndarray/open.py` & `evadb-0.2.1/eva/udfs/ndarray/open.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/ndarray/similarity.py` & `evadb-0.2.1/eva/udfs/ndarray/similarity.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/ocr_extractor.py` & `evadb-0.2.1/eva/udfs/ocr_extractor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/udf_bootstrap_queries.py` & `evadb-0.2.1/eva/udfs/udf_bootstrap_queries.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/udfs/yolo_object_detector.py` & `evadb-0.2.1/eva/udfs/yolo_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/utils/__init__.py` & `evadb-0.2.1/eva/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/utils/errors.py` & `evadb-0.2.1/eva/utils/errors.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/utils/generic_utils.py` & `evadb-0.2.1/eva/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/utils/kv_cache.py` & `evadb-0.2.1/eva/utils/kv_cache.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/utils/logging_manager.py` & `evadb-0.2.1/eva/utils/logging_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/utils/s3_utils.py` & `evadb-0.2.1/eva/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/utils/stats.py` & `evadb-0.2.1/eva/utils/stats.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/eva/version.py` & `evadb-0.2.1/eva/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 _MAJOR = "0"
 _MINOR = "2"
-_REVISION = "0"
+_REVISION = "1"
 
 VERSION_SHORT = f"{_MAJOR}.{_MINOR}"
 VERSION = f"{_MAJOR}.{_MINOR}.{_REVISION}"
```

### Comparing `evadb-0.2.0/evadb.egg-info/PKG-INFO` & `evadb-0.2.1/evadb.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: evadb
-Version: 0.2.0
+Version: 0.2.1
 Summary: EVA Video Database System (Think MySQL for videos).
 Home-page: https://github.com/georgia-tech-db/eva
 Author: Georgia Tech Database Group
 Author-email: georgia.tech.db@gmail.com
 License: Apache License 2.0
 Download-URL: https://github.com/georgia-tech-db/eva
 Description: <div >
           <a href="https://evadb.readthedocs.io/">
             <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-banner.png" alt="EVA" width="1000px" margin-left="-5px">
           </a>
           <div>
                 <h3>Try It Out!</h3>
+                <a href="https://github.com/georgia-tech-db/eva">
+                    <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/v1.json" alt="Logo"/>
+                </a>
                 <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
                     <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EVA on Colab"/>
                 </a>
                 <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
                     <img alt="Slack" src="https://img.shields.io/badge/slack-eva-ff69b4.svg?logo=slack">
                 </a>    
                 <a href="https://github.com/georgia-tech-db/eva/discussions">
@@ -26,120 +29,153 @@
                 <img alt="License" src="https://img.shields.io/badge/license-Apache%202-brightgreen.svg?logo=apache"/>
                 <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.7%20|%203.8%20|%203.9%20|%203.10-brightgreen"/>
             </div>
         </div>
         
         # EVA AI-Relational Database System
         
-        EVA is an open-source **AI-relational database with first-class support for deep learning models**. It aims to support AI-powered database applications that operate on both structured (tables) and unstructured data (videos, text, podcasts, PDFs, etc.) with deep learning models.
+        - â¡ï¸ 10-100x faster AI pipelines using SQL-like queries 
+        - ð° Save money spent on GPU-driven inference
+        - ð¦ Built-in caching to avoid re-running deep learning models across queries
+        - ð Over 20 AI-centric query optimization rules
+        - â¨ï¸ First-party integrations for PyTorch and HuggingFace models
+        - ð Installable via pip
+        - ð¤ Fully implemented in Python
+        
+        EVA is an open-source **AI-relational database with first-class support for deep learning models**. It supports next-generation AI-powered database applications that operate on structured (tables) and unstructured data (videos, text, podcasts, PDFs, etc.) with deep learning models.
         
-        EVA accelerates AI pipelines using a collection of optimizations inspired by relational database systems including function caching, sampling, and cost-based operator reordering. It comes with a wide range of models for analyzing unstructured data including image classification, object detection, OCR, face detection, etc. It is fully implemented in Python, and licensed under the Apache license.
+        EVA accelerates AI pipelines by 10-100x using a collection of optimizations inspired by relational database systems, including function caching, sampling, and cost-based predicate reordering. It comes with a wide range of models for analyzing unstructured data, including models for image classification, object detection, OCR, text sentiment classification, face detection, etc. It is fully implemented in Python and licensed under the Apache license.
         
-        EVA supports a AI-oriented query language for analysing unstructured data. Here are some illustrative applications:
+        EVA supports an AI-oriented query language tailored for analyzing unstructured data. Here are some illustrative applications:
         
          * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
          * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection </a>
          * <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
-         * <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recogizing license plates </a>
+         * <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates </a>
          * <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
          
-        If you are wondering why you might need a AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/video.html#">Video Database Systems</a>. It describes how EVA lets you easily make use of deep learning models and you can save money spent on inference on large image or video datasets.
+        If you are wondering why you might need an AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/video.html#">Video Database Systems</a>. It describes how EVA lets you easily use deep learning models and save money spent on GPU-driven inference on large image or video datasets.
         
         The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different computer vision tasks: image classification, object detection, action recognition, and how you can easily extend EVA to support your custom deep learning model in the form of user-defined functions.
         
-        The <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/index.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab, where you can run the code by yourself.
+        The <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/index.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab to run the code.
         
         ## Why EVA? ##
         
         <details>
           <summary><b>Easily combine SQL and Deep Learning to build next-generation database applications</b></summary>
           Easily query videos in user-facing applications with a SQL-like interface for commonly used computer vision models.
         </details>
         
         <details>
           <summary><b>Speed up queries and save money spent on model inference</b></summary>
-          EVA comes with a collection of built-in sampling, caching, and filtering optimizations inspired by time-tested relational database systems.
+          EVA has built-in sampling, caching, and filtering optimizations inspired by time-tested relational database systems.
         </details>
         
         <details>
           <summary><b>Extensible by design to support custom deep learning models </b></summary>
-          EVA has first-class support for user-defined functions that wrap around your deep learning models in PyTorch.
+          EVA has first-class support for user-defined functions that wrap around your deep learning models in PyTorch and HuggingFace.
         </details>
         
         ## Links
         * [Documentation](https://evadb.readthedocs.io/)
         * [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
         * [Join Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
         * [Demo](https://ada-00.cc.gatech.edu/eva/playground)
         
         ## Quick Start
         
-        1. To install EVA, we recommend using the pip package manager (EVA supports Python versions 3.7+).
+        - Install EVA using the pip package manager. EVA supports Python versions 3.7+.
         
         ```shell
         pip install evadb
         ```
         
-        2. EVA is based on a client-server architecture. It works in Jupyter notebooks (illustrative notebooks are available in the [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb) folder) and also supports a terminal-based client. To start the EVA server and a terminal-based client, use the following commands:
+        - To start and connect to an EVA server in a Jupyter notebook, check out this [illustrative emotion analysis notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb):
         ```shell
-        eva_server &   # launch server
-        eva_client     # launch client
+        cursor = connect_to_server()
         ```
         
-        3. Load a video onto the EVA server from the client (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) video as an example):
+        - Load a video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration):
         
         ```mysql
-        LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO MyVideo;
+        LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO UADETRAC;
         ```
         
-        4. That's it! You can now run queries over the loaded video:
+        - That's it! You can now run queries over the loaded video:
         
         ```mysql
-        SELECT id, data FROM MyVideo WHERE id < 5;
+        SELECT id, data FROM UADETRAC WHERE id < 5;
         ```
         
-        5. Search for frames in the video that contain a car
+        - Search for frames in the video that contain a car
         
         ```mysql
-        SELECT id, data FROM MyVideo WHERE ['car'] <@ FastRCNNObjectDetector(data).labels;
+        SELECT id, data FROM UADETRAC WHERE ['car'] <@ YoloV5(data).labels;
         ```
         | Source Video  | Query Result |
         |---------------|--------------|
         |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
         
-        6. Search for frames in the video that contain a pedestrian and a car
+        - Search for frames in the video that contain a pedestrian and a car
         
         ```mysql
-        SELECT id, data FROM MyVideo WHERE ['pedestrian', 'car'] <@ FastRCNNObjectDetector(data).labels;
+        SELECT id, data FROM UADETRAC WHERE ['pedestrian', 'car'] <@ YoloV5(data).labels;
         ```
         
-        7. Search for frames in the video with more than 3 cars
+        - Search for frames with more than three cars
         
         ```mysql
-        SELECT id, data FROM MyVideo WHERE ArrayCount(FastRCNNObjectDetector(data).labels, 'car') > 3;
+        SELECT id, data FROM UADETRAC WHERE ArrayCount(YoloV5(data).labels, 'car') > 3;
         ```
         
-        8. You can create a new user-defined function (UDF) that wraps around your custom vision model or an off-the-shelf model like FastRCNN:
+        - You can **create a custom user-defined function (UDF)** that wraps around a fine-tuned or off-the-shelf deep learning model:
         ```mysql
         CREATE UDF IF NOT EXISTS MyUDF
         INPUT  (frame NDARRAY UINT8(3, ANYDIM, ANYDIM))
         OUTPUT (labels NDARRAY STR(ANYDIM), bboxes NDARRAY FLOAT32(ANYDIM, 4),
                 scores NDARRAY FLOAT32(ANYDIM))
         TYPE  Classification
         IMPL  'eva/udfs/fastrcnn_object_detector.py';
         ```
         
-        9. You can combine multiple user-defined functions in a single query to accomplish more complicated tasks.
+        - **Compose multiple user-defined functions in a single query** to accomplish complicated AI pipelines.
         ```mysql
            -- Analyse emotions of faces in a video
            SELECT id, bbox, EmotionDetector(Crop(data, bbox)) 
            FROM MyVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)  
            WHERE id < 15;
         ```
         
+        - Besides making it easy to write queries for complex AI pipelines, EVA **speeds up query execution using its AI-centric query optimizer**. Two illustrative  optimizations are:
+        
+           ð¾ **Caching**: EVA automatically caches and reuses previous query results (especially model inference results), eliminating redundant computation and reducing query processing time.
+        
+           ð¯ **Predicate Reordering**: EVA optimizes the order in which the query predicates are evaluated (e.g., runs the faster, more selective model first), leading to faster queries and lower inference costs.
+        
+        Consider these two exploratory queries on a dataset of dog images:
+        <img align="right" style="display:inline;" width="40%" src="https://github.com/georgia-tech-db/eva/blob/master/data/assets/eva_performance_comparison.png?raw=true"></a>
+        
+        ```mysql
+          -- Query 1: Find all images of black-colored dogs
+          SELECT id, bbox FROM dogs 
+          JOIN LATERAL UNNEST(YoloV5(data)) AS Obj(label, bbox, score) 
+          WHERE Obj.label = 'dog' 
+            AND Color(Crop(data, bbox)) = 'black'; 
+        
+          -- Query 2: Find all Great Danes that are black-colored
+          SELECT id, bbox FROM dogs 
+          JOIN LATERAL UNNEST(YoloV5(data)) AS Obj(label, bbox, score) 
+          WHERE Obj.label = 'dog' 
+            AND DogBreedClassifier(Crop(data, bbox)) = 'great dane' 
+            AND Color(Crop(data, bbox)) = 'black';
+        ```
+        
+        By reusing the results of the first query and reordering the predicates based on available cached results, EVA runs up the second query **10x faster**!
+        
         ## Illustrative EVA Applications 
         
         ### Traffic Analysis (Object Detection Model)
         | Source Video  | Query Result |
         |---------------|--------------|
         |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
         
@@ -181,22 +217,21 @@
         ## Contributing to EVA
         
         [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb)
         [![CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva)
         [![Coverage Status](https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master)](https://coveralls.io/github/georgia-tech-db/eva?branch=master)
         [![Documentation Status](https://readthedocs.org/projects/evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/index.html)
         
-        We welcome all kinds of contributions to EVA.
-        To file a bug or request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
+        EVA is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EVA are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
         
-        For more information on contributing to EVA, see our
+        For more information, see our
         [contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
         
         ## License
-        Copyright (c) 2018-2023 [Georgia Tech Database Group](http://db.cc.gatech.edu/)
+        Copyright (c) 2018-2023 [Georgia Tech Database Group](http://db.cc.gatech.edu/).
         Licensed under [Apache License](LICENSE).
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,107 +1,128 @@
-Metadata-Version: 2.1 Name: evadb Version: 0.2.0 Summary: EVA Video Database
+Metadata-Version: 2.1 Name: evadb Version: 0.2.1 Summary: EVA Video Database
 System (Think MySQL for videos). Home-page: https://github.com/georgia-tech-db/
 eva Author: Georgia Tech Database Group Author-email: georgia.tech.db@gmail.com
 License: Apache License 2.0 Download-URL: https://github.com/georgia-tech-db/
 eva Description:
 [EVA]
 **** Try It Out! ****
-[Open_EVA_on_Colab] [Slack] [Discuss_on_Github!] [PyPI] [License] [Python
-Versions]
-# EVA AI-Relational Database System EVA is an open-source **AI-relational
-database with first-class support for deep learning models**. It aims to
-support AI-powered database applications that operate on both structured
-(tables) and unstructured data (videos, text, podcasts, PDFs, etc.) with deep
-learning models. EVA accelerates AI pipelines using a collection of
-optimizations inspired by relational database systems including function
-caching, sampling, and cost-based operator reordering. It comes with a wide
-range of models for analyzing unstructured data including image classification,
-object detection, OCR, face detection, etc. It is fully implemented in Python,
-and licensed under the Apache license. EVA supports a AI-oriented query
-language for analysing unstructured data. Here are some illustrative
+[Logo] [Open_EVA_on_Colab] [Slack] [Discuss_on_Github!] [PyPI] [License]
+[Python Versions]
+# EVA AI-Relational Database System - Ã¢ÂÂ¡Ã¯Â¸Â 10-100x faster AI pipelines
+using SQL-like queries - Ã°ÂÂÂ° Save money spent on GPU-driven inference -
+Ã°ÂÂÂ¦ Built-in caching to avoid re-running deep learning models across
+queries - Ã°ÂÂÂ Over 20 AI-centric query optimization rules - Ã¢ÂÂ¨Ã¯Â¸Â
+First-party integrations for PyTorch and HuggingFace models - Ã°ÂÂÂ
+Installable via pip - Ã°ÂÂ¤Â Fully implemented in Python EVA is an open-
+source **AI-relational database with first-class support for deep learning
+models**. It supports next-generation AI-powered database applications that
+operate on structured (tables) and unstructured data (videos, text, podcasts,
+PDFs, etc.) with deep learning models. EVA accelerates AI pipelines by 10-100x
+using a collection of optimizations inspired by relational database systems,
+including function caching, sampling, and cost-based predicate reordering. It
+comes with a wide range of models for analyzing unstructured data, including
+models for image classification, object detection, OCR, text sentiment
+classification, face detection, etc. It is fully implemented in Python and
+licensed under the Apache license. EVA supports an AI-oriented query language
+tailored for analyzing unstructured data. Here are some illustrative
 applications: * Examining_the_emotion_palette_of_actors_in_a_movie * Analysing
 traffic_flow_at_an_intersection * Classifying_images_based_on_their_content *
-Recogizing_license_plates * Analysing_toxicity_of_social_media_memes If you are
-wondering why you might need a AI-relational database system, start with the
-page on Video_Database_Systems. It describes how EVA lets you easily make use
-of deep learning models and you can save money spent on inference on large
+Recognizing_license_plates * Analysing_toxicity_of_social_media_memes If you
+are wondering why you might need an AI-relational database system, start with
+the page on Video_Database_Systems. It describes how EVA lets you easily use
+deep learning models and save money spent on GPU-driven inference on large
 image or video datasets. The Getting_Started page shows how you can use EVA for
 different computer vision tasks: image classification, object detection, action
 recognition, and how you can easily extend EVA to support your custom deep
 learning model in the form of user-defined functions. The User_Guides section
 contains Jupyter Notebooks that demonstrate how to use various features of EVA.
-Each notebook includes a link to Google Colab, where you can run the code by
-yourself. ## Why EVA? ##  Easily combine SQL and Deep Learning to build next-
-generation database applications Easily query videos in user-facing
-applications with a SQL-like interface for commonly used computer vision
-models.   Speed up queries and save money spent on model inference EVA comes
-with a collection of built-in sampling, caching, and filtering optimizations
-inspired by time-tested relational database systems.   Extensible by design to
-support custom deep learning models EVA has first-class support for user-
-defined functions that wrap around your deep learning models in PyTorch.  ##
-Links * [Documentation](https://evadb.readthedocs.io/) * [Tutorials](https://
-github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
-* [Join Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-
-PlJ4iawLdurDv~aIAq90Dg) * [Demo](https://ada-00.cc.gatech.edu/eva/playground)
-## Quick Start 1. To install EVA, we recommend using the pip package manager
-(EVA supports Python versions 3.7+). ```shell pip install evadb ``` 2. EVA is
-based on a client-server architecture. It works in Jupyter notebooks
-(illustrative notebooks are available in the [Tutorials](https://github.com/
-georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb) folder)
-and also supports a terminal-based client. To start the EVA server and a
-terminal-based client, use the following commands: ```shell eva_server & #
-launch server eva_client # launch client ``` 3. Load a video onto the EVA
-server from the client (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4)
-video as an example): ```mysql LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO
-MyVideo; ``` 4. That's it! You can now run queries over the loaded video:
-```mysql SELECT id, data FROM MyVideo WHERE id < 5; ``` 5. Search for frames in
-the video that contain a car ```mysql SELECT id, data FROM MyVideo WHERE
-['car'] <@ FastRCNNObjectDetector(data).labels; ``` | Source Video | Query
-Result | |---------------|--------------| |[Source Video] |[Query Result] | 6.
-Search for frames in the video that contain a pedestrian and a car ```mysql
-SELECT id, data FROM MyVideo WHERE ['pedestrian', 'car'] <@
-FastRCNNObjectDetector(data).labels; ``` 7. Search for frames in the video with
-more than 3 cars ```mysql SELECT id, data FROM MyVideo WHERE ArrayCount
-(FastRCNNObjectDetector(data).labels, 'car') > 3; ``` 8. You can create a new
-user-defined function (UDF) that wraps around your custom vision model or an
-off-the-shelf model like FastRCNN: ```mysql CREATE UDF IF NOT EXISTS MyUDF
-INPUT (frame NDARRAY UINT8(3, ANYDIM, ANYDIM)) OUTPUT (labels NDARRAY STR
-(ANYDIM), bboxes NDARRAY FLOAT32(ANYDIM, 4), scores NDARRAY FLOAT32(ANYDIM))
-TYPE Classification IMPL 'eva/udfs/fastrcnn_object_detector.py'; ``` 9. You can
-combine multiple user-defined functions in a single query to accomplish more
-complicated tasks. ```mysql -- Analyse emotions of faces in a video SELECT id,
-bbox, EmotionDetector(Crop(data, bbox)) FROM MyVideo JOIN LATERAL UNNEST
-(FaceDetector(data)) AS Face(bbox, conf) WHERE id < 15; ``` ## Illustrative EVA
-Applications ### Traffic Analysis (Object Detection Model) | Source Video |
-Query Result | |---------------|--------------| |[Source Video] |[Query Result]
-| ### MNIST Digit Recognition (Image Classification Model) | Source Video |
-Query Result | |---------------|--------------| |[Source Video] |[Query Result]
-| ### Movie Analysis (Face Detection + Emotion Classfication Models) | Source
-Video | Query Result | |---------------|--------------| |[Source Video] |[Query
-Result] | ### [License Plate Recognition](https://github.com/georgia-tech-db/
-eva-application-template) (Plate Detection + OCR Extraction Models) | Query
-Result | |--------------| [Query Result] | ### [Meme Toxicity Classification]
-(https://github.com/georgia-tech-db/toxicity-classification) (OCR Extraction +
-Toxicity Classification Models) | Query Result | |--------------| [Query
-Result] | ## Community Join the EVA community on [Slack](https://
-join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) to
-ask questions and to share your ideas for improving EVA. [EVA_Slack_Channel]
-### Architecture Diagram of EVA [EVA Architecture Diagram] ## Contributing to
-EVA [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://
-pypi.org/project/evadb) [![CI Status](https://circleci.com/gh/georgia-tech-db/
-eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva) [![Coverage
-Status](https://coveralls.io/repos/github/georgia-tech-db/eva/
-badge.svg?branch=master)](https://coveralls.io/github/georgia-tech-db/
-eva?branch=master) [![Documentation Status](https://readthedocs.org/projects/
-evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/
-index.html) We welcome all kinds of contributions to EVA. To file a bug or
-request a feature, please use GitHub_issues. Pull_requests are welcome. For
-more information on contributing to EVA, see our [contribution guide](https://
-evadb.readthedocs.io/en/stable/source/contribute/index.html). ## License
-Copyright (c) 2018-2023 [Georgia Tech Database Group](http://db.cc.gatech.edu/
-) Licensed under [Apache License](LICENSE). Platform: UNKNOWN Classifier:
-Intended Audience :: Science/Research Classifier: Topic :: Scientific/
-Engineering :: Information Analysis Classifier: License :: OSI Approved ::
-Apache Software License Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha Classifier: Operating System :: OS
-Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Provides-Extra: dev
+Each notebook includes a link to Google Colab to run the code. ## Why EVA? ##
+Easily combine SQL and Deep Learning to build next-generation database
+applications Easily query videos in user-facing applications with a SQL-like
+interface for commonly used computer vision models.   Speed up queries and save
+money spent on model inference EVA has built-in sampling, caching, and
+filtering optimizations inspired by time-tested relational database systems.
+Extensible by design to support custom deep learning models EVA has first-class
+support for user-defined functions that wrap around your deep learning models
+in PyTorch and HuggingFace.  ## Links * [Documentation](https://
+evadb.readthedocs.io/) * [Tutorials](https://github.com/georgia-tech-db/eva/
+blob/master/tutorials/03-emotion-analysis.ipynb) * [Join Slack](https://
+join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) *
+[Demo](https://ada-00.cc.gatech.edu/eva/playground) ## Quick Start - Install
+EVA using the pip package manager. EVA supports Python versions 3.7+. ```shell
+pip install evadb ``` - To start and connect to an EVA server in a Jupyter
+notebook, check out this [illustrative emotion analysis notebook](https://
+github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-
+analysis.ipynb): ```shell cursor = connect_to_server() ``` - Load a video onto
+the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for
+illustration): ```mysql LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO
+UADETRAC; ``` - That's it! You can now run queries over the loaded video:
+```mysql SELECT id, data FROM UADETRAC WHERE id < 5; ``` - Search for frames in
+the video that contain a car ```mysql SELECT id, data FROM UADETRAC WHERE
+['car'] <@ YoloV5(data).labels; ``` | Source Video | Query Result | |----------
+-----|--------------| |[Source Video] |[Query Result] | - Search for frames in
+the video that contain a pedestrian and a car ```mysql SELECT id, data FROM
+UADETRAC WHERE ['pedestrian', 'car'] <@ YoloV5(data).labels; ``` - Search for
+frames with more than three cars ```mysql SELECT id, data FROM UADETRAC WHERE
+ArrayCount(YoloV5(data).labels, 'car') > 3; ``` - You can **create a custom
+user-defined function (UDF)** that wraps around a fine-tuned or off-the-shelf
+deep learning model: ```mysql CREATE UDF IF NOT EXISTS MyUDF INPUT (frame
+NDARRAY UINT8(3, ANYDIM, ANYDIM)) OUTPUT (labels NDARRAY STR(ANYDIM), bboxes
+NDARRAY FLOAT32(ANYDIM, 4), scores NDARRAY FLOAT32(ANYDIM)) TYPE Classification
+IMPL 'eva/udfs/fastrcnn_object_detector.py'; ``` - **Compose multiple user-
+defined functions in a single query** to accomplish complicated AI pipelines.
+```mysql -- Analyse emotions of faces in a video SELECT id, bbox,
+EmotionDetector(Crop(data, bbox)) FROM MyVideo JOIN LATERAL UNNEST(FaceDetector
+(data)) AS Face(bbox, conf) WHERE id < 15; ``` - Besides making it easy to
+write queries for complex AI pipelines, EVA **speeds up query execution using
+its AI-centric query optimizer**. Two illustrative optimizations are: Ã°ÂÂÂ¾
+**Caching**: EVA automatically caches and reuses previous query results
+(especially model inference results), eliminating redundant computation and
+reducing query processing time. Ã°ÂÂÂ¯ **Predicate Reordering**: EVA
+optimizes the order in which the query predicates are evaluated (e.g., runs the
+faster, more selective model first), leading to faster queries and lower
+inference costs. Consider these two exploratory queries on a dataset of dog
+images: [https://github.com/georgia-tech-db/eva/blob/master/data/assets/
+eva_performance_comparison.png?raw=true]
+ ```mysql -- Query 1: Find all images of black-colored dogs SELECT id, bbox
+FROM dogs JOIN LATERAL UNNEST(YoloV5(data)) AS Obj(label, bbox, score) WHERE
+Obj.label = 'dog' AND Color(Crop(data, bbox)) = 'black'; -- Query 2: Find all
+Great Danes that are black-colored SELECT id, bbox FROM dogs JOIN LATERAL
+UNNEST(YoloV5(data)) AS Obj(label, bbox, score) WHERE Obj.label = 'dog' AND
+DogBreedClassifier(Crop(data, bbox)) = 'great dane' AND Color(Crop(data, bbox))
+= 'black'; ``` By reusing the results of the first query and reordering the
+predicates based on available cached results, EVA runs up the second query
+**10x faster**! ## Illustrative EVA Applications ### Traffic Analysis (Object
+Detection Model) | Source Video | Query Result | |---------------|-------------
+-| |[Source Video] |[Query Result] | ### MNIST Digit Recognition (Image
+Classification Model) | Source Video | Query Result | |---------------|--------
+------| |[Source Video] |[Query Result] | ### Movie Analysis (Face Detection +
+Emotion Classfication Models) | Source Video | Query Result | |---------------
+|--------------| |[Source Video] |[Query Result] | ### [License Plate
+Recognition](https://github.com/georgia-tech-db/eva-application-template)
+(Plate Detection + OCR Extraction Models) | Query Result | |--------------|
+[Query Result] | ### [Meme Toxicity Classification](https://github.com/georgia-
+tech-db/toxicity-classification) (OCR Extraction + Toxicity Classification
+Models) | Query Result | |--------------| [Query Result] | ## Community Join
+the EVA community on [Slack](https://join.slack.com/t/eva-db/shared_invite/zt-
+1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) to ask questions and to share your ideas for
+improving EVA. [EVA_Slack_Channel] ### Architecture Diagram of EVA [EVA
+Architecture Diagram] ## Contributing to EVA [![PyPI Version](https://
+img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb) [![CI Status]
+(https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://
+circleci.com/gh/georgia-tech-db/eva) [![Coverage Status](https://coveralls.io/
+repos/github/georgia-tech-db/eva/badge.svg?branch=master)](https://
+coveralls.io/github/georgia-tech-db/eva?branch=master) [![Documentation Status]
+(https://readthedocs.org/projects/evadb/badge/?version=stable)](https://
+evadb.readthedocs.io/en/stable/index.html) EVA is the beneficiary of many
+[contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All
+kinds of contributions to EVA are appreciated. To file a bug or to request a
+feature, please use GitHub_issues. Pull_requests are welcome. For more
+information, see our [contribution guide](https://evadb.readthedocs.io/en/
+stable/source/contribute/index.html). ## License Copyright (c) 2018-2023
+[Georgia Tech Database Group](http://db.cc.gatech.edu/). Licensed under [Apache
+License](LICENSE). Platform: UNKNOWN Classifier: Intended Audience :: Science/
+Research Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Programming Language :: Python :: 3 Classifier: Development Status :: 3 - Alpha
+Classifier: Operating System :: OS Independent Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: dev
```

### Comparing `evadb-0.2.0/evadb.egg-info/SOURCES.txt` & `evadb-0.2.1/evadb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,14 @@
 eva/udfs/emotion_detector.py
 eva/udfs/face_detector.py
 eva/udfs/fastrcnn_object_detector.py
 eva/udfs/feature_extractor.py
 eva/udfs/gpu_compatible.py
 eva/udfs/mvit_action_recognition.py
 eva/udfs/ocr_extractor.py
-eva/udfs/toxicity_classifier.py
 eva/udfs/udf_bootstrap_queries.py
 eva/udfs/yolo_object_detector.py
 eva/udfs/abstract/__init__.py
 eva/udfs/abstract/abstract_udf.py
 eva/udfs/abstract/hf_abstract_udf.py
 eva/udfs/abstract/pytorch_abstract_udf.py
 eva/udfs/decorators/__init__.py
@@ -268,14 +267,15 @@
 test/markers.py
 test/test_eva_cmd_client.py
 test/test_eva_imports.py
 test/test_eva_server.py
 test/util.py
 test/benchmark_tests/__init__.py
 test/benchmark_tests/conftest.py
+test/benchmark_tests/plot.py
 test/benchmark_tests/test_benchmark_pytorch.py
 test/binder/__init__.py
 test/binder/test_binder_utils.py
 test/binder/test_statement_binder.py
 test/binder/test_statement_binder_context.py
 test/binder/test_statement_binder_python37.py
 test/catalog/__init__.py
```

### Comparing `evadb-0.2.0/evadb.egg-info/requires.txt` & `evadb-0.2.1/evadb.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Pillow>=8.4.0
 aenum>=2.2.0
-detoxify
 diskcache>=5.4.0
 easyocr>=1.5.0
-eva-decord==0.6.0
+eva-decord==0.6.1
 facenet-pytorch>=2.5.2
 faiss-cpu
 importlib-metadata<5.0
 ipython
 lark>=1.0.0
 numpy<=1.23.5,>=1.19.5
 opencv-python<4.6.0.66,>=4.5.4.60
@@ -23,18 +22,17 @@
 yolov5<=7.0.6
 
 [dev]
 Pillow>=8.4.0
 aenum>=2.2.0
 black>=23.1.0
 coveralls>=3.0.1
-detoxify
 diskcache>=5.4.0
 easyocr>=1.5.0
-eva-decord==0.6.0
+eva-decord==0.6.1
 facenet-pytorch>=2.5.2
 faiss-cpu
 flake8>=3.9.1
 importlib-metadata<5.0
 ipython
 ipywidgets>=7.7.2
 isort>=5.10.1
```

### Comparing `evadb-0.2.0/setup.py` & `evadb-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     "sqlalchemy-utils>=0.36.6",
     "lark>=1.0.0",
     "pyyaml>=5.1",
     "importlib-metadata<5.0",
     "ray>=1.13.0",
     "aenum>=2.2.0",
     "diskcache>=5.4.0",
-    "eva-decord==0.6.0"
+    "eva-decord==0.6.1"
 ]
 
 formatter_libs = ["black>=23.1.0", "isort>=5.10.1"]
 
 test_libs = [
     "pytest>=6.1.2",
     "pytest-cov>=2.11.1",
@@ -93,15 +93,14 @@
 
 ### NEEDED FOR A BATTERIES-LOADED EXPERIENCE
 udf_libs = [
     "facenet-pytorch>=2.5.2",  # FACE DETECTION
     "easyocr>=1.5.0",  # OCR EXTRACTION
     "ipython",
     "yolov5<=7.0.6",          # OBJECT DETECTION
-    "detoxify",               # TEXT TOXICITY CLASSIFICATION
     "thefuzz",                # FUZZY STRING MATCHINGz
     "transformers==4.27.4"    # HUGGINGFACE
 ]
 
 ### NEEDED FOR EXPERIMENTAL FEATURES
 experimental_libs = []
```

### Comparing `evadb-0.2.0/test/__init__.py` & `evadb-0.2.1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/benchmark_tests/__init__.py` & `evadb-0.2.1/test/benchmark_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/benchmark_tests/conftest.py` & `evadb-0.2.1/test/benchmark_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/benchmark_tests/test_benchmark_pytorch.py` & `evadb-0.2.1/test/benchmark_tests/test_benchmark_pytorch.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/binder/__init__.py` & `evadb-0.2.1/test/binder/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/binder/test_binder_utils.py` & `evadb-0.2.1/test/binder/test_binder_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/binder/test_statement_binder.py` & `evadb-0.2.1/test/binder/test_statement_binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/binder/test_statement_binder_context.py` & `evadb-0.2.1/test/binder/test_statement_binder_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/binder/test_statement_binder_python37.py` & `evadb-0.2.1/test/binder/test_statement_binder_python37.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/catalog/__init__.py` & `evadb-0.2.1/test/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/catalog/models/__init__.py` & `evadb-0.2.1/test/catalog/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/catalog/models/test_models.py` & `evadb-0.2.1/test/catalog/models/test_models.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/catalog/services/__init__.py` & `evadb-0.2.1/test/catalog/services/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/catalog/services/test_column_catalog_service.py` & `evadb-0.2.1/test/catalog/services/test_column_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/catalog/services/test_index_catalog_service.py` & `evadb-0.2.1/test/catalog/services/test_index_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/catalog/services/test_table_catalog_service.py` & `evadb-0.2.1/test/catalog/services/test_table_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/catalog/services/test_udf_catalog_service.py` & `evadb-0.2.1/test/catalog/services/test_udf_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/catalog/services/test_udf_cost_catalog_service.py` & `evadb-0.2.1/test/catalog/services/test_udf_cost_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/catalog/services/test_udf_io_catalog_service.py` & `evadb-0.2.1/test/catalog/services/test_udf_io_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/catalog/test_catalog_manager.py` & `evadb-0.2.1/test/catalog/test_catalog_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/catalog/test_column_type.py` & `evadb-0.2.1/test/catalog/test_column_type.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/catalog/test_sqlalchemy.py` & `evadb-0.2.1/test/catalog/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/configuration/__init__.py` & `evadb-0.2.1/test/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/configuration/test_bootstrap_environment.py` & `evadb-0.2.1/test/configuration/test_bootstrap_environment.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/configuration/test_configuration_manager.py` & `evadb-0.2.1/test/configuration/test_configuration_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/executor/__init__.py` & `evadb-0.2.1/test/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/executor/test_abstract_executor.py` & `evadb-0.2.1/test/executor/test_abstract_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/executor/test_create_mat_executor.py` & `evadb-0.2.1/test/executor/test_create_mat_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/executor/test_create_udf_executor.py` & `evadb-0.2.1/test/executor/test_create_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/executor/test_execution_context.py` & `evadb-0.2.1/test/executor/test_execution_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/executor/test_executor_utils.py` & `evadb-0.2.1/test/executor/test_executor_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/executor/test_limit_executor.py` & `evadb-0.2.1/test/executor/test_limit_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/executor/test_load_executor.py` & `evadb-0.2.1/test/executor/test_load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/executor/test_orderby_executor.py` & `evadb-0.2.1/test/executor/test_orderby_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/executor/test_plan_executor.py` & `evadb-0.2.1/test/executor/test_plan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/executor/test_pp_executor.py` & `evadb-0.2.1/test/executor/test_pp_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/executor/test_sample_executor.py` & `evadb-0.2.1/test/executor/test_sample_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/executor/test_seq_scan_executor.py` & `evadb-0.2.1/test/executor/test_seq_scan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/executor/utils.py` & `evadb-0.2.1/test/executor/utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/expression/__init__.py` & `evadb-0.2.1/test/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/expression/test_abstract_expression.py` & `evadb-0.2.1/test/expression/test_abstract_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/expression/test_aggregation.py` & `evadb-0.2.1/test/expression/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/expression/test_arithmetic.py` & `evadb-0.2.1/test/expression/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/expression/test_comparison.py` & `evadb-0.2.1/test/expression/test_comparison.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/expression/test_expression_tree.py` & `evadb-0.2.1/test/expression/test_expression_tree.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/expression/test_expression_utils.py` & `evadb-0.2.1/test/expression/test_expression_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/expression/test_function_expression.py` & `evadb-0.2.1/test/expression/test_function_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/expression/test_logical.py` & `evadb-0.2.1/test/expression/test_logical.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/__init__.py` & `evadb-0.2.1/test/integration_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_array_count.py` & `evadb-0.2.1/test/integration_tests/test_array_count.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_create_index_executor.py` & `evadb-0.2.1/test/integration_tests/test_create_index_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_create_table_executor.py` & `evadb-0.2.1/test/integration_tests/test_create_table_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_delete_executor.py` & `evadb-0.2.1/test/integration_tests/test_delete_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_drop_executor.py` & `evadb-0.2.1/test/integration_tests/test_drop_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_error_handling_with_ray.py` & `evadb-0.2.1/test/integration_tests/test_error_handling_with_ray.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_explain_executor.py` & `evadb-0.2.1/test/integration_tests/test_explain_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_fuzzy_join.py` & `evadb-0.2.1/test/integration_tests/test_fuzzy_join.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_huggingface_udfs.py` & `evadb-0.2.1/test/integration_tests/test_huggingface_udfs.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_insert_executor.py` & `evadb-0.2.1/test/integration_tests/test_insert_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_like.py` & `evadb-0.2.1/test/integration_tests/test_like.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_load_executor.py` & `evadb-0.2.1/test/integration_tests/test_load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_mat_executor.py` & `evadb-0.2.1/test/integration_tests/test_mat_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_open.py` & `evadb-0.2.1/test/integration_tests/test_open.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_optimizer_rules.py` & `evadb-0.2.1/test/integration_tests/test_optimizer_rules.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_pytorch.py` & `evadb-0.2.1/test/integration_tests/test_pytorch.py`

 * *Files 10% similar despite different names*

```diff
@@ -251,49 +251,14 @@
         self.assertEqual(len(actual_batch), 5)
 
         # non-trivial test case for MNIST
         res = actual_batch.frames
         self.assertTrue(res["ocrextractor.labels"][0][0] == "4")
         self.assertTrue(res["ocrextractor.scores"][2][0] > 0.9)
 
-    @pytest.mark.torchtest
-    @windows_skip_marker
-    def test_should_run_detoxify_on_text(self):
-        create_udf_query = """CREATE UDF IF NOT EXISTS OCRExtractor
-                  INPUT  (text NDARRAY STR(100))
-                  OUTPUT (labels NDARRAY STR(10),
-                          bboxes NDARRAY FLOAT32(ANYDIM, 4),
-                          scores NDARRAY FLOAT32(ANYDIM))
-                  TYPE  OCRExtraction
-                  IMPL  'eva/udfs/ocr_extractor.py';
-        """
-        execute_query_fetch_all(create_udf_query)
-
-        create_udf_query = """CREATE UDF IF NOT EXISTS ToxicityClassifier
-                  INPUT  (text NDARRAY STR(100))
-                  OUTPUT (labels NDARRAY STR(10))
-                  TYPE  Classification
-                  IMPL  'eva/udfs/toxicity_classifier.py';
-        """
-        execute_query_fetch_all(create_udf_query)
-
-        select_query = """SELECT name, OCRExtractor(data).labels,
-                                 ToxicityClassifier(OCRExtractor(data).labels)
-                        FROM MemeImages;"""
-        actual_batch = execute_query_fetch_all(select_query)
-
-        # non-trivial test case for Detoxify
-        res = actual_batch.frames
-        for i in range(2):
-            # Image can be reordered.
-            if "meme1" in res["memeimages.name"][i]:
-                self.assertTrue(res["toxicityclassifier.labels"][i] == "toxic")
-            else:
-                self.assertTrue(res["toxicityclassifier.labels"][i] == "not toxic")
-
     def test_check_unnest_with_predicate_on_yolo(self):
         query = """SELECT id, yolov5.label, yolov5.bbox, yolov5.score
                   FROM MyVideo
                   JOIN LATERAL UNNEST(YoloV5(data)) AS yolov5(label, bbox, score)
                   WHERE yolov5.label = 'car' AND id < 10;"""
 
         actual_batch = execute_query_fetch_all(query)
```

### Comparing `evadb-0.2.0/test/integration_tests/test_rename_executor.py` & `evadb-0.2.1/test/integration_tests/test_rename_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_reuse.py` & `evadb-0.2.1/test/integration_tests/test_reuse.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_s3_load_executor.py` & `evadb-0.2.1/test/integration_tests/test_s3_load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_select_executor.py` & `evadb-0.2.1/test/integration_tests/test_select_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_show_info_executor.py` & `evadb-0.2.1/test/integration_tests/test_show_info_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_similarity.py` & `evadb-0.2.1/test/integration_tests/test_similarity.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/integration_tests/test_udf_executor.py` & `evadb-0.2.1/test/integration_tests/test_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/markers.py` & `evadb-0.2.1/test/markers.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/models/__init__.py` & `evadb-0.2.1/test/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/models/catalog/__init__.py` & `evadb-0.2.1/test/models/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/models/catalog/test_frame_info.py` & `evadb-0.2.1/test/models/catalog/test_frame_info.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/models/storage/__init__.py` & `evadb-0.2.1/test/models/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/models/storage/test_batch.py` & `evadb-0.2.1/test/models/storage/test_batch.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/optimizer/__init__.py` & `evadb-0.2.1/test/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/optimizer/rules/__init__.py` & `evadb-0.2.1/test/optimizer/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/optimizer/rules/test_rules.py` & `evadb-0.2.1/test/optimizer/rules/test_rules.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/optimizer/test_binder.py` & `evadb-0.2.1/test/optimizer/test_binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/optimizer/test_cascade_optimizer.py` & `evadb-0.2.1/test/optimizer/test_cascade_optimizer.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/optimizer/test_cost_model.py` & `evadb-0.2.1/test/optimizer/test_cost_model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/optimizer/test_group.py` & `evadb-0.2.1/test/optimizer/test_group.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/optimizer/test_memo.py` & `evadb-0.2.1/test/optimizer/test_memo.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/optimizer/test_optimizer_context.py` & `evadb-0.2.1/test/optimizer/test_optimizer_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/optimizer/test_optimizer_task.py` & `evadb-0.2.1/test/optimizer/test_optimizer_task.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/optimizer/test_optimizer_utils.py` & `evadb-0.2.1/test/optimizer/test_optimizer_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/optimizer/test_statement_to_opr_convertor.py` & `evadb-0.2.1/test/optimizer/test_statement_to_opr_convertor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/parser/__init__.py` & `evadb-0.2.1/test/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/parser/test_parser.py` & `evadb-0.2.1/test/parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/parser/test_parser_statements.py` & `evadb-0.2.1/test/parser/test_parser_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/plan_nodes/__init__.py` & `evadb-0.2.1/test/plan_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/plan_nodes/test_plan.py` & `evadb-0.2.1/test/plan_nodes/test_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/readers/__init__.py` & `evadb-0.2.1/test/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/readers/test_csv_reader.py` & `evadb-0.2.1/test/readers/test_csv_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/readers/test_decord_reader.py` & `evadb-0.2.1/test/readers/test_decord_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/server/__init__.py` & `evadb-0.2.1/test/server/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/server/test_command_handler.py` & `evadb-0.2.1/test/server/test_command_handler.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/server/test_db_api.py` & `evadb-0.2.1/test/server/test_db_api.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/server/test_interpreter.py` & `evadb-0.2.1/test/server/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/server/test_server.py` & `evadb-0.2.1/test/server/test_server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/storage/__init__.py` & `evadb-0.2.1/test/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/storage/test_sqlite_storage_engine.py` & `evadb-0.2.1/test/storage/test_sqlite_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/storage/test_video_storage.py` & `evadb-0.2.1/test/storage/test_video_storage.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/test_eva_cmd_client.py` & `evadb-0.2.1/test/test_eva_cmd_client.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/test_eva_imports.py` & `evadb-0.2.1/test/test_eva_imports.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/test_eva_server.py` & `evadb-0.2.1/test/test_eva_server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/udfs/__init__.py` & `evadb-0.2.1/test/udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/udfs/decorators/__init__.py` & `evadb-0.2.1/test/udfs/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/udfs/decorators/io_descriptors/__init__.py` & `evadb-0.2.1/test/udfs/decorators/io_descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/udfs/decorators/io_descriptors/test_descriptors.py` & `evadb-0.2.1/test/udfs/decorators/io_descriptors/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/udfs/decorators/test_decorators.py` & `evadb-0.2.1/test/udfs/decorators/test_decorators.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/udfs/ndarray/__init__.py` & `evadb-0.2.1/test/udfs/ndarray/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/udfs/ndarray/test_array_count.py` & `evadb-0.2.1/test/udfs/ndarray/test_array_count.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/udfs/ndarray/test_crop.py` & `evadb-0.2.1/test/udfs/ndarray/test_crop.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/udfs/ndarray/test_open.py` & `evadb-0.2.1/test/udfs/ndarray/test_open.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/udfs/test_abstract_udf.py` & `evadb-0.2.1/test/udfs/test_abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/udfs/test_emotion_detector.py` & `evadb-0.2.1/test/udfs/test_emotion_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/udfs/test_facenet_udf.py` & `evadb-0.2.1/test/udfs/test_facenet_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/udfs/test_fastrcnn_object_detector.py` & `evadb-0.2.1/test/udfs/test_fastrcnn_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/udfs/test_yolo_object_detector.py` & `evadb-0.2.1/test/udfs/test_yolo_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/util.py` & `evadb-0.2.1/test/util.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/utils/__init__.py` & `evadb-0.2.1/test/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/utils/test_generic_utils.py` & `evadb-0.2.1/test/utils/test_generic_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/utils/test_timer.py` & `evadb-0.2.1/test/utils/test_timer.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.0/test/utils/test_xdist.py` & `evadb-0.2.1/test/utils/test_xdist.py`

 * *Files identical despite different names*

