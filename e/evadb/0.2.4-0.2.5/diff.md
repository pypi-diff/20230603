# Comparing `tmp/evadb-0.2.4.tar.gz` & `tmp/evadb-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evadb-0.2.4.tar", last modified: Thu May 18 03:49:40 2023, max compression
+gzip compressed data, was "evadb-0.2.5.tar", last modified: Sat Jun  3 02:07:23 2023, max compression
```

## Comparing `evadb-0.2.4.tar` & `evadb-0.2.5.tar`

### file list

```diff
@@ -1,467 +1,480 @@
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.467877 evadb-0.2.4/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    11357 2023-05-18 00:46:12.000000 evadb-0.2.4/LICENSE.txt
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    16362 2023-05-18 03:49:40.467877 evadb-0.2.4/PKG-INFO
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13729 2023-05-18 02:58:13.000000 evadb-0.2.4/README.md
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.423875 evadb-0.2.4/eva/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      645 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.423875 evadb-0.2.4/eva/binder/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/binder/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7778 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/binder/binder_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12413 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/binder/statement_binder.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7997 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/binder/statement_binder_context.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.423875 evadb-0.2.4/eva/catalog/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    18120 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/catalog_manager.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3022 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/catalog_type.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7200 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/catalog_utils.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.423875 evadb-0.2.4/eva/catalog/models/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      886 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1499 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/association_models.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4671 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/base_model.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5266 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/column_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3393 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/index_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2997 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/table_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3532 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/udf_cache_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4429 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/udf_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2262 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/udf_cost_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4722 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/udf_io_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2668 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/models/udf_metadata_catalog.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2127 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/schema_utils.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.423875 evadb-0.2.4/eva/catalog/services/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/services/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1167 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/services/base_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2873 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/services/column_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2899 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/services/index_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4571 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/services/table_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3669 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/services/udf_cache_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3078 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/services/udf_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2826 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/services/udf_cost_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2476 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/services/udf_io_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1936 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/services/udf_metadata_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3119 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/catalog/sql_config.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.427875 evadb-0.2.4/eva/configuration/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/configuration/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4298 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/configuration/bootstrap_environment.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4146 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/configuration/configuration_manager.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1403 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/configuration/constants.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      882 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/constants.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      787 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/eva.yml
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1997 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/eva_cmd_client.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2692 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/eva_server.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/executor/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      615 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2140 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/abstract_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1910 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/apply_and_merge_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1530 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/create_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5191 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/create_index_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3866 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/create_mat_view_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7642 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/create_udf_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4738 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/delete_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2557 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/drop_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2010 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/drop_udf_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3017 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/execution_context.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3958 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/executor_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1522 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/explain_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1591 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/function_scan_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1759 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/groupby_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1800 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/hash_join_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2255 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/insert_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1616 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/join_build_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1661 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/lateral_join_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1583 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/limit_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3086 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/load_csv_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1579 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/load_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6038 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/load_multimedia_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1488 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/nested_loop_join_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4183 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/orderby_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8075 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/plan_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1644 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/pp_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1277 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/predicate_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1272 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/project_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1186 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/rename_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1413 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/sample_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1812 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/seq_scan_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1870 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/show_info_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2274 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/storage_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1264 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/union_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3916 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/executor/vector_index_scan_executor.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/experimental/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      619 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/experimental/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/experimental/ray/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      610 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/experimental/ray/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/experimental/ray/executor/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      619 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/experimental/ray/executor/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3522 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/experimental/ray/executor/exchange_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1431 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/experimental/ray/executor/ray_stage.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/experimental/ray/optimizer/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/experimental/ray/optimizer/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/experimental/ray/optimizer/rules/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      626 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/experimental/ray/optimizer/rules/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4176 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/experimental/ray/optimizer/rules/rules.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/experimental/ray/planner/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      618 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/experimental/ray/planner/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1380 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/experimental/ray/planner/exchange_plan.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/expression/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      617 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/expression/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5559 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/expression/abstract_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3974 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/expression/aggregation_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1618 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/expression/arithmetic_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4351 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/expression/comparison_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2542 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/expression/constant_value_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10433 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/expression/expression_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10172 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/expression/function_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3055 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/expression/logical_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4685 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/expression/tuple_value_expression.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/models/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      633 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/models/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/models/catalog/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/models/catalog/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1332 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/models/catalog/frame_info.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      857 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/models/catalog/properties.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/models/server/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/models/server/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1961 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/models/server/response.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.431875 evadb-0.2.4/eva/models/storage/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/models/storage/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    14841 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/models/storage/batch.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.435876 evadb-0.2.4/eva/optimizer/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      620 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3259 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/binder.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2129 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/cost_model.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3450 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/group.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2669 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/group_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4335 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/memo.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    37333 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/operators.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3837 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/optimizer_context.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      982 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/optimizer_task_stack.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12582 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/optimizer_tasks.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10874 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/optimizer_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5897 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/plan_generator.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1169 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/property.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.435876 evadb-0.2.4/eva/optimizer/rules/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/rules/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1019 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/rules/pattern.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    45651 2023-05-18 02:58:13.000000 evadb-0.2.4/eva/optimizer/rules/rules.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7336 2023-05-18 02:58:13.000000 evadb-0.2.4/eva/optimizer/rules/rules_base.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7842 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/rules/rules_manager.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13590 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/optimizer/statement_to_opr_converter.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.435876 evadb-0.2.4/eva/parser/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1360 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/alias.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2740 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/create_index_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2788 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/create_mat_view_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4838 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/create_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4882 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/create_udf_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2048 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/delete_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1767 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/drop_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1793 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/drop_udf_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    19597 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/eva.lark
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1384 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/explain_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2922 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/insert_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1717 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_parser.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.439875 evadb-0.2.4/eva/parser/lark_visitor/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2655 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2161 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_common_clauses_ids.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10670 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_create_statements.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1404 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_delete_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1202 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_drop_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1006 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_explain_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4672 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_expressions.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6231 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_functions.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2465 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_insert_statements.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2057 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_load_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      932 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_rename_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2143 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_select_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1112 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_show_statements.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     9468 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/lark_visitor/_table_sources.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3214 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/load_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1228 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/parser.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2007 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/rename_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5921 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/select_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1460 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/show_statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1052 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/statement.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8639 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/table_ref.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1738 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/parser/types.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.443876 evadb-0.2.4/eva/plan_nodes/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      614 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1689 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/abstract_join_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3453 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/abstract_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1455 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/abstract_scan_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1930 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/apply_and_merge_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2469 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/create_index_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2076 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/create_mat_view_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2200 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/create_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3603 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/create_udf_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1951 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/delete_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1660 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/drop_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1532 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/drop_udf_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1033 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/explain_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1755 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/function_scan_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1499 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/groupby_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1712 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/hash_join_build_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2179 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/hash_join_probe_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2023 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/insert_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1408 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/lateral_join_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1468 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/limit_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2710 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/load_data_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1510 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/nested_loop_join_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1564 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/orderby_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1177 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/pp_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1245 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/predicate_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1249 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/project_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1616 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/rename_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1469 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/sample_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1760 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/seq_scan_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1201 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/show_info_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4419 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/storage_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1421 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/types.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1245 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/union_plan.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2720 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/plan_nodes/vector_index_scan_plan.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.443876 evadb-0.2.4/eva/readers/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/readers/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2320 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/readers/abstract_reader.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2648 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/readers/csv_reader.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5987 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/readers/decord_reader.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.443876 evadb-0.2.4/eva/readers/image/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/readers/image/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1067 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/readers/image/opencv_image_reader.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.443876 evadb-0.2.4/eva/server/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      623 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/server/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3284 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/server/command_handler.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3502 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/server/db_api.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3252 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/server/interpreter.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2954 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/server/server.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.443876 evadb-0.2.4/eva/storage/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/storage/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6133 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/storage/abstract_media_storage_engine.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2383 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/storage/abstract_storage_engine.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1717 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/storage/image_storage_engine.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8972 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/storage/sqlite_storage_engine.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1688 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/storage/storage_engine.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2496 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/storage/video_storage_engine.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.443876 evadb-0.2.4/eva/third_party/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      605 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/third_party/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.443876 evadb-0.2.4/eva/third_party/huggingface/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      612 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/third_party/huggingface/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1420 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/third_party/huggingface/binder.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6403 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/third_party/huggingface/create.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2615 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/third_party/huggingface/model.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.447876 evadb-0.2.4/eva/third_party/vector_stores/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      607 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/third_party/vector_stores/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3227 2023-05-18 02:58:13.000000 evadb-0.2.4/eva/third_party/vector_stores/faiss.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2960 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/third_party/vector_stores/qdrant.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1376 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/third_party/vector_stores/types.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1594 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/third_party/vector_stores/utils.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.447876 evadb-0.2.4/eva/udfs/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      616 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.447876 evadb-0.2.4/eva/udfs/abstract/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      625 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/abstract/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2442 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/abstract/abstract_udf.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3945 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/abstract/hf_abstract_udf.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3843 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/abstract/pytorch_abstract_udf.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3914 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/abstract/tracker_abstract_udf.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3464 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/asl_action_recognition.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3219 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/chatgpt.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.447876 evadb-0.2.4/eva/udfs/decorators/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/decorators/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2188 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/decorators/decorators.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.447876 evadb-0.2.4/eva/udfs/decorators/io_descriptors/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/decorators/io_descriptors/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2755 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/decorators/io_descriptors/abstract_types.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3376 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/decorators/io_descriptors/data_types.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2067 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/decorators/utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5478 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/emotion_detector.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2539 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/face_detector.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5999 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/fastrcnn_object_detector.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1822 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/feature_extractor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1028 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/gpu_compatible.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2200 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/mvit_action_recognition.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.447876 evadb-0.2.4/eva/udfs/ndarray/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      638 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/ndarray/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2568 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/ndarray/array_count.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1647 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/ndarray/crop.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1179 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/ndarray/fuzzy_join.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1557 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/ndarray/open.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1782 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/ndarray/similarity.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2750 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/ocr_extractor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2899 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/sift_feature_extractor.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.447876 evadb-0.2.4/eva/udfs/trackers/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      636 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/trackers/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2367 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/trackers/nor_fair.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7609 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/udf_bootstrap_queries.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3859 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/udfs/yolo_object_detector.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.451876 evadb-0.2.4/eva/utils/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      611 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/utils/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      909 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/utils/errors.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7254 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/utils/generic_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1956 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/utils/kv_cache.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      985 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/utils/logging_manager.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1388 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/utils/math_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1562 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/utils/s3_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1692 2023-05-18 00:46:12.000000 evadb-0.2.4/eva/utils/stats.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      711 2023-05-18 03:01:42.000000 evadb-0.2.4/eva/version.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.451876 evadb-0.2.4/evadb.egg-info/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    16362 2023-05-18 03:49:40.000000 evadb-0.2.4/evadb.egg-info/PKG-INFO
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13679 2023-05-18 03:49:40.000000 evadb-0.2.4/evadb.egg-info/SOURCES.txt
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)        1 2023-05-18 03:49:40.000000 evadb-0.2.4/evadb.egg-info/dependency_links.txt
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       89 2023-05-18 03:49:40.000000 evadb-0.2.4/evadb.egg-info/entry_points.txt
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1240 2023-05-18 03:49:40.000000 evadb-0.2.4/evadb.egg-info/requires.txt
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       21 2023-05-18 03:49:40.000000 evadb-0.2.4/evadb.egg-info/top_level.txt
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       90 2023-05-18 00:46:12.000000 evadb-0.2.4/pyproject.toml
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)       38 2023-05-18 03:49:40.467877 evadb-0.2.4/setup.cfg
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4396 2023-05-18 00:46:12.000000 evadb-0.2.4/setup.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.451876 evadb-0.2.4/test/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.451876 evadb-0.2.4/test/benchmark_tests/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/benchmark_tests/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1176 2023-05-18 00:46:12.000000 evadb-0.2.4/test/benchmark_tests/conftest.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6639 2023-05-18 00:46:12.000000 evadb-0.2.4/test/benchmark_tests/test_benchmark_pytorch.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.451876 evadb-0.2.4/test/binder/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/binder/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2032 2023-05-18 00:46:12.000000 evadb-0.2.4/test/binder/test_binder_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13099 2023-05-18 00:46:12.000000 evadb-0.2.4/test/binder/test_statement_binder.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7962 2023-05-18 00:46:12.000000 evadb-0.2.4/test/binder/test_statement_binder_context.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.451876 evadb-0.2.4/test/catalog/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.451876 evadb-0.2.4/test/catalog/models/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/models/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7234 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/models/test_models.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.455876 evadb-0.2.4/test/catalog/services/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/services/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1918 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/services/test_column_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4794 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/services/test_index_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3639 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/services/test_table_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3639 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/services/test_udf_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3210 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/services/test_udf_cost_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3035 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/services/test_udf_io_catalog_service.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6808 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/test_catalog_manager.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1402 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/test_column_type.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1910 2023-05-18 00:46:12.000000 evadb-0.2.4/test/catalog/test_sqlalchemy.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.455876 evadb-0.2.4/test/configuration/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/configuration/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1490 2023-05-18 00:46:12.000000 evadb-0.2.4/test/configuration/test_bootstrap_environment.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1616 2023-05-18 00:46:12.000000 evadb-0.2.4/test/configuration/test_configuration_manager.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.455876 evadb-0.2.4/test/executor/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1106 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_abstract_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2441 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_create_mat_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3989 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_create_udf_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4227 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_execution_context.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1275 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_executor_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4650 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_limit_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3890 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_load_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2884 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_orderby_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10983 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_plan_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1397 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_pp_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1817 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_sample_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2752 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/test_seq_scan_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      847 2023-05-18 00:46:12.000000 evadb-0.2.4/test/executor/utils.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.455876 evadb-0.2.4/test/expression/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/expression/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3722 2023-05-18 00:46:12.000000 evadb-0.2.4/test/expression/test_abstract_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5149 2023-05-18 00:46:12.000000 evadb-0.2.4/test/expression/test_aggregation.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2975 2023-05-18 00:46:12.000000 evadb-0.2.4/test/expression/test_arithmetic.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5578 2023-05-18 00:46:12.000000 evadb-0.2.4/test/expression/test_comparison.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2867 2023-05-18 00:46:12.000000 evadb-0.2.4/test/expression/test_expression_tree.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7555 2023-05-18 00:46:12.000000 evadb-0.2.4/test/expression/test_expression_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2685 2023-05-18 00:46:12.000000 evadb-0.2.4/test/expression/test_function_expression.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10242 2023-05-18 00:46:12.000000 evadb-0.2.4/test/expression/test_logical.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.459876 evadb-0.2.4/test/integration_tests/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3585 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_array_count.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4522 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_chatgpt.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6167 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_create_index_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1091 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_create_table_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5158 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_delete_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4839 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_drop_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2358 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_error_handling_with_ray.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4086 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_explain_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3183 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_fuzzy_join.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13961 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_huggingface_udfs.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3806 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_insert_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2983 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_like.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    20622 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_load_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5377 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_mat_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2658 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_open.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10646 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_optimizer_rules.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    11709 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_pytorch.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2953 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_rename_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    10469 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_reuse.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5210 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_s3_load_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    30781 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_select_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3277 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_show_info_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    14709 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_similarity.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    12062 2023-05-18 00:46:12.000000 evadb-0.2.4/test/integration_tests/test_udf_executor.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1574 2023-05-18 00:46:12.000000 evadb-0.2.4/test/markers.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.459876 evadb-0.2.4/test/models/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/models/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.459876 evadb-0.2.4/test/models/catalog/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/models/catalog/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1010 2023-05-18 00:46:12.000000 evadb-0.2.4/test/models/catalog/test_frame_info.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.459876 evadb-0.2.4/test/models/storage/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/models/storage/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5919 2023-05-18 00:46:12.000000 evadb-0.2.4/test/models/storage/test_batch.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.459876 evadb-0.2.4/test/optimizer/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/optimizer/rules/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/rules/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    11993 2023-05-18 02:58:13.000000 evadb-0.2.4/test/optimizer/rules/test_rules.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4195 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/test_binder.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4377 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/test_cascade_optimizer.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4406 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/test_cost_model.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2689 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/test_group.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1996 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/test_memo.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1034 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/test_optimizer_context.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6122 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/test_optimizer_task.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2000 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/test_optimizer_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    13564 2023-05-18 00:46:12.000000 evadb-0.2.4/test/optimizer/test_statement_to_opr_converter.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/parser/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/parser/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    36070 2023-05-18 00:46:12.000000 evadb-0.2.4/test/parser/test_parser.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7783 2023-05-18 00:46:12.000000 evadb-0.2.4/test/parser/test_parser_statements.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/plan_nodes/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/plan_nodes/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     6292 2023-05-18 00:46:12.000000 evadb-0.2.4/test/plan_nodes/test_plan.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/readers/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/readers/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1688 2023-05-18 00:46:12.000000 evadb-0.2.4/test/readers/test_csv_reader.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     8104 2023-05-18 00:46:12.000000 evadb-0.2.4/test/readers/test_decord_reader.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/server/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/server/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1268 2023-05-18 00:46:12.000000 evadb-0.2.4/test/server/test_command_handler.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     5057 2023-05-18 00:46:12.000000 evadb-0.2.4/test/server/test_db_api.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2581 2023-05-18 00:46:12.000000 evadb-0.2.4/test/server/test_interpreter.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2066 2023-05-18 00:46:12.000000 evadb-0.2.4/test/server/test_server.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/storage/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/storage/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4113 2023-05-18 00:46:12.000000 evadb-0.2.4/test/storage/test_sqlite_storage_engine.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4023 2023-05-18 00:46:12.000000 evadb-0.2.4/test/storage/test_video_storage.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3309 2023-05-18 00:46:12.000000 evadb-0.2.4/test/test_eva_cmd_client.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1294 2023-05-18 00:46:12.000000 evadb-0.2.4/test/test_eva_imports.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     1825 2023-05-18 00:46:12.000000 evadb-0.2.4/test/test_eva_server.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/udfs/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      638 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/udfs/decorators/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/decorators/__init__.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/udfs/decorators/io_descriptors/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/decorators/io_descriptors/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     7429 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/decorators/io_descriptors/test_descriptors.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2137 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/decorators/test_decorators.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/udfs/ndarray/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      648 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/ndarray/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      849 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/ndarray/test_array_count.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2410 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/ndarray/test_crop.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2374 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/ndarray/test_open.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4412 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/test_abstract_udf.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2154 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/test_emotion_detector.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     3345 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/test_facenet_udf.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2548 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/test_fastrcnn_object_detector.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2768 2023-05-18 00:46:12.000000 evadb-0.2.4/test/udfs/test_yolo_object_detector.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)    17438 2023-05-18 00:46:12.000000 evadb-0.2.4/test/util.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.463877 evadb-0.2.4/test/utils/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)      587 2023-05-18 00:46:12.000000 evadb-0.2.4/test/utils/__init__.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     4196 2023-05-18 00:46:12.000000 evadb-0.2.4/test/utils/test_generic_utils.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2256 2023-05-18 00:46:12.000000 evadb-0.2.4/test/utils/test_timer.py
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)     2199 2023-05-18 00:46:12.000000 evadb-0.2.4/test/utils/test_xdist.py
-drwxr-xr-x   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-05-18 03:49:40.467877 evadb-0.2.4/third_party/
--rw-r--r--   0 gkakkar7 (1085173) gtperson  (2626)        0 2023-04-02 17:27:27.000000 evadb-0.2.4/third_party/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.189962 evadb-0.2.5/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11357 2022-08-11 16:20:33.000000 evadb-0.2.5/LICENSE.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14211 2023-06-03 02:07:23.185961 evadb-0.2.5/PKG-INFO
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13539 2023-06-02 21:04:24.000000 evadb-0.2.5/README.md
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.125959 evadb-0.2.5/eva/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      645 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.125959 evadb-0.2.5/eva/binder/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/binder/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7778 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/binder/binder_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    15552 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/binder/statement_binder.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7997 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/binder/statement_binder_context.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.125959 evadb-0.2.5/eva/catalog/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      616 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    18583 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/catalog_manager.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3320 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/catalog_type.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8604 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/catalog_utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.129959 evadb-0.2.5/eva/catalog/models/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      886 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1499 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/association_models.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4671 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/base_model.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5266 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/column_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3393 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/index_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2997 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/table_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3532 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/udf_cache_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4429 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/udf_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2262 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/udf_cost_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4722 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/udf_io_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2668 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/models/udf_metadata_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2127 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/schema_utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.129959 evadb-0.2.5/eva/catalog/services/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/services/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1167 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/services/base_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2873 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/services/column_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2899 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/services/index_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4571 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/services/table_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3669 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/services/udf_cache_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3078 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/services/udf_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2826 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/services/udf_cost_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2476 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/services/udf_io_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1936 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/services/udf_metadata_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2654 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/catalog/sql_config.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.129959 evadb-0.2.5/eva/configuration/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      620 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/configuration/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5490 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/configuration/bootstrap_environment.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4798 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/configuration/configuration_manager.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1005 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/configuration/constants.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      882 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/constants.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      852 2023-06-02 21:04:24.000000 evadb-0.2.5/eva/eva.yml
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1997 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/eva_cmd_client.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3246 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/eva_server.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.137960 evadb-0.2.5/eva/executor/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      615 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2140 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/abstract_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1910 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/apply_and_merge_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2005 2023-06-02 21:04:24.000000 evadb-0.2.5/eva/executor/create_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5191 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/create_index_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1924 2023-06-02 21:04:24.000000 evadb-0.2.5/eva/executor/create_mat_view_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7292 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/create_udf_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4738 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/delete_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2515 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/drop_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1968 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/drop_udf_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3537 2023-06-02 21:04:24.000000 evadb-0.2.5/eva/executor/exchange_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3017 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/execution_context.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4366 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/executor_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1522 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/explain_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1591 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/function_scan_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1759 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/groupby_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1800 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/hash_join_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2255 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/insert_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1616 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/join_build_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1661 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/lateral_join_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1583 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/limit_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3086 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/load_csv_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1648 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/load_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6038 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/load_multimedia_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1488 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/nested_loop_join_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4183 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/orderby_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8198 2023-06-02 21:04:24.000000 evadb-0.2.5/eva/executor/plan_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1644 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/pp_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1277 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/predicate_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1272 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/project_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2074 2023-06-02 21:04:24.000000 evadb-0.2.5/eva/executor/ray_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1186 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/rename_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1413 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/sample_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1812 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/seq_scan_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1870 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/show_info_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2533 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/storage_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1264 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/union_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3916 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/executor/vector_index_scan_executor.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.137960 evadb-0.2.5/eva/expression/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      617 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/expression/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5559 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/expression/abstract_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3973 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/expression/aggregation_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1618 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/expression/arithmetic_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4351 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/expression/comparison_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2542 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/expression/constant_value_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10433 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/expression/expression_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10358 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/expression/function_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3055 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/expression/logical_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4685 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/expression/tuple_value_expression.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.137960 evadb-0.2.5/eva/interfaces/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/interfaces/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.137960 evadb-0.2.5/eva/interfaces/relational/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/interfaces/relational/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10769 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/interfaces/relational/db.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7278 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/interfaces/relational/relation.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4472 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/interfaces/relational/utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.137960 evadb-0.2.5/eva/models/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      633 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/models/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.141960 evadb-0.2.5/eva/models/catalog/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/models/catalog/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1332 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/models/catalog/frame_info.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      857 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/models/catalog/properties.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.141960 evadb-0.2.5/eva/models/server/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/models/server/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1961 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/models/server/response.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.141960 evadb-0.2.5/eva/models/storage/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/models/storage/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14841 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/models/storage/batch.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.141960 evadb-0.2.5/eva/optimizer/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      620 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3259 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/binder.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2129 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/cost_model.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3450 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/group.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2669 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/group_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4335 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/memo.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    37333 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/operators.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3837 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/optimizer_context.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      982 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/optimizer_task_stack.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12582 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/optimizer_tasks.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10874 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/optimizer_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4102 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/plan_generator.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1169 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/property.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.141960 evadb-0.2.5/eva/optimizer/rules/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/rules/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1019 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/rules/pattern.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    49728 2023-06-02 21:04:24.000000 evadb-0.2.5/eva/optimizer/rules/rules.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7440 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/rules/rules_base.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7534 2023-06-02 21:04:24.000000 evadb-0.2.5/eva/optimizer/rules/rules_manager.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13726 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/optimizer/statement_to_opr_converter.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.145960 evadb-0.2.5/eva/parser/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1360 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/alias.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2740 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/create_index_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2872 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/create_mat_view_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5341 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/create_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4882 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/create_udf_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2048 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/delete_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1767 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/drop_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1793 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/drop_udf_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    19702 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/eva.lark
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1384 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/explain_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2922 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/insert_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1716 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_parser.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.149960 evadb-0.2.5/eva/parser/lark_visitor/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2655 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2161 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_common_clauses_ids.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10824 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_create_statements.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1404 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_delete_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1202 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_drop_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1006 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_explain_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4672 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_expressions.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6231 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_functions.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2465 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_insert_statements.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2241 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_load_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      932 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_rename_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2143 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_select_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1112 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_show_statements.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9469 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/lark_visitor/_table_sources.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3214 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/load_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1227 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/parser.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2007 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/rename_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6248 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/select_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1460 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/show_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1426 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8637 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/table_ref.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1787 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/types.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2654 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/parser/utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.153960 evadb-0.2.5/eva/plan_nodes/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      614 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1689 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/abstract_join_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3453 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/abstract_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1455 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/abstract_scan_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1930 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/apply_and_merge_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2469 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/create_index_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2076 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/create_mat_view_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2200 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/create_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3603 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/create_udf_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1951 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/delete_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1660 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/drop_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1532 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/drop_udf_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2057 2023-06-02 21:04:24.000000 evadb-0.2.5/eva/plan_nodes/exchange_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1033 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/explain_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1755 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/function_scan_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1499 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/groupby_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1712 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/hash_join_build_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2179 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/hash_join_probe_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2023 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/insert_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1408 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/lateral_join_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1468 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/limit_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2710 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/load_data_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1510 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/nested_loop_join_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1564 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/orderby_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1177 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/pp_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1245 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/predicate_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1249 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/project_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1616 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/rename_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1469 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/sample_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1760 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/seq_scan_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1201 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/show_info_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4419 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/storage_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1421 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/types.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1245 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/union_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2720 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/plan_nodes/vector_index_scan_plan.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.153960 evadb-0.2.5/eva/readers/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/readers/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2320 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/readers/abstract_reader.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2648 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/readers/csv_reader.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5987 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/readers/decord_reader.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.153960 evadb-0.2.5/eva/readers/document/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/readers/document/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1467 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/readers/document/document_reader.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1979 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/readers/document/registry.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.157960 evadb-0.2.5/eva/readers/image/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/readers/image/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1067 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/readers/image/opencv_image_reader.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2050 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/readers/pdf_reader.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.157960 evadb-0.2.5/eva/server/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      623 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/server/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3289 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/server/command_handler.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3263 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/server/interpreter.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2926 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/server/server.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.157960 evadb-0.2.5/eva/storage/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      616 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/storage/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6133 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/storage/abstract_media_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2383 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/storage/abstract_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1713 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/storage/document_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1717 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/storage/image_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1692 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/storage/pdf_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8972 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/storage/sqlite_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1941 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/storage/storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2496 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/storage/video_storage_engine.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.157960 evadb-0.2.5/eva/third_party/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      605 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/third_party/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.157960 evadb-0.2.5/eva/third_party/huggingface/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      612 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/third_party/huggingface/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1420 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/third_party/huggingface/binder.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6473 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/third_party/huggingface/create.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2615 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/third_party/huggingface/model.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.157960 evadb-0.2.5/eva/third_party/vector_stores/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      607 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/third_party/vector_stores/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3284 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/third_party/vector_stores/faiss.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2960 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/third_party/vector_stores/qdrant.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1376 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/third_party/vector_stores/types.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1594 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/third_party/vector_stores/utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.161960 evadb-0.2.5/eva/udfs/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      616 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.161960 evadb-0.2.5/eva/udfs/abstract/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      625 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/abstract/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2442 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/abstract/abstract_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4040 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/abstract/hf_abstract_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3843 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/abstract/pytorch_abstract_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3914 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/abstract/tracker_abstract_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3464 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/asl_action_recognition.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3413 2023-06-03 01:20:14.000000 evadb-0.2.5/eva/udfs/chatgpt.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.161960 evadb-0.2.5/eva/udfs/decorators/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/decorators/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2188 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/decorators/decorators.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.161960 evadb-0.2.5/eva/udfs/decorators/io_descriptors/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/decorators/io_descriptors/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2755 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/decorators/io_descriptors/abstract_types.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3376 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/decorators/io_descriptors/data_types.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2067 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/decorators/utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5478 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/emotion_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2539 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/face_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5999 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/fastrcnn_object_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1822 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/feature_extractor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1028 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/gpu_compatible.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3528 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/mnist_image_classifier.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2200 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/mvit_action_recognition.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.165961 evadb-0.2.5/eva/udfs/ndarray/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      638 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2472 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/annotate.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2568 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/array_count.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1647 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/crop.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1179 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/fuzzy_join.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2200 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/gaussian_blur.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2202 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/horizontal_flip.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1557 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/open.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1782 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/similarity.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2139 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/to_grayscale.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2188 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ndarray/vertical_flip.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2750 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/ocr_extractor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2899 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/sift_feature_extractor.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.165961 evadb-0.2.5/eva/udfs/trackers/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      636 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/trackers/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2367 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/trackers/nor_fair.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.165961 evadb-0.2.5/eva/udfs/tutorials/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      636 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/tutorials/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7934 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/udf_bootstrap_queries.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3859 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/udfs/yolo_object_detector.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.165961 evadb-0.2.5/eva/utils/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      611 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/utils/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      909 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/utils/errors.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6966 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/utils/generic_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1956 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/utils/kv_cache.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      985 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/utils/logging_manager.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1388 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/utils/math_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1562 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/utils/s3_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1692 2023-06-01 22:37:10.000000 evadb-0.2.5/eva/utils/stats.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      123 2023-06-03 02:07:22.000000 evadb-0.2.5/eva/version.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.165961 evadb-0.2.5/evadb.egg-info/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14211 2023-06-03 02:07:22.000000 evadb-0.2.5/evadb.egg-info/PKG-INFO
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14107 2023-06-03 02:07:23.000000 evadb-0.2.5/evadb.egg-info/SOURCES.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)        1 2023-06-03 02:07:22.000000 evadb-0.2.5/evadb.egg-info/dependency_links.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       88 2023-06-03 02:07:22.000000 evadb-0.2.5/evadb.egg-info/entry_points.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1329 2023-06-03 02:07:22.000000 evadb-0.2.5/evadb.egg-info/requires.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       21 2023-06-03 02:07:22.000000 evadb-0.2.5/evadb.egg-info/top_level.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       90 2022-06-26 17:11:46.000000 evadb-0.2.5/pyproject.toml
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       38 2023-06-03 02:07:23.189962 evadb-0.2.5/setup.cfg
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4575 2023-06-03 02:07:16.000000 evadb-0.2.5/setup.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.169961 evadb-0.2.5/test/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-09-30 14:20:49.000000 evadb-0.2.5/test/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.169961 evadb-0.2.5/test/benchmark_tests/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-01-02 23:54:53.000000 evadb-0.2.5/test/benchmark_tests/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1176 2023-05-09 19:58:04.000000 evadb-0.2.5/test/benchmark_tests/conftest.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6639 2023-05-12 03:48:38.000000 evadb-0.2.5/test/benchmark_tests/test_benchmark_pytorch.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.169961 evadb-0.2.5/test/binder/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/binder/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2032 2023-01-02 23:54:53.000000 evadb-0.2.5/test/binder/test_binder_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13819 2023-06-01 22:37:10.000000 evadb-0.2.5/test/binder/test_statement_binder.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7962 2023-05-16 03:45:18.000000 evadb-0.2.5/test/binder/test_statement_binder_context.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.169961 evadb-0.2.5/test/catalog/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/catalog/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.169961 evadb-0.2.5/test/catalog/models/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/catalog/models/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7234 2023-03-28 02:19:14.000000 evadb-0.2.5/test/catalog/models/test_models.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.169961 evadb-0.2.5/test/catalog/services/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/catalog/services/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1918 2023-01-07 03:29:08.000000 evadb-0.2.5/test/catalog/services/test_column_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4794 2023-05-17 22:20:34.000000 evadb-0.2.5/test/catalog/services/test_index_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3639 2023-03-28 02:19:14.000000 evadb-0.2.5/test/catalog/services/test_table_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3639 2023-04-01 16:09:26.000000 evadb-0.2.5/test/catalog/services/test_udf_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3210 2023-03-28 02:19:14.000000 evadb-0.2.5/test/catalog/services/test_udf_cost_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3035 2023-04-02 20:13:44.000000 evadb-0.2.5/test/catalog/services/test_udf_io_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6808 2023-05-09 19:58:04.000000 evadb-0.2.5/test/catalog/test_catalog_manager.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1402 2022-12-13 23:02:13.000000 evadb-0.2.5/test/catalog/test_column_type.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1910 2023-04-01 16:09:26.000000 evadb-0.2.5/test/catalog/test_sqlalchemy.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.169961 evadb-0.2.5/test/configuration/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/configuration/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1486 2023-05-25 14:58:01.000000 evadb-0.2.5/test/configuration/test_bootstrap_environment.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1620 2023-05-25 14:58:01.000000 evadb-0.2.5/test/configuration/test_configuration_manager.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.173961 evadb-0.2.5/test/executor/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/executor/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1106 2023-03-28 02:19:14.000000 evadb-0.2.5/test/executor/test_abstract_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3989 2023-05-16 03:45:18.000000 evadb-0.2.5/test/executor/test_create_udf_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4227 2023-04-09 04:33:37.000000 evadb-0.2.5/test/executor/test_execution_context.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1275 2022-12-13 23:02:13.000000 evadb-0.2.5/test/executor/test_executor_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4650 2023-01-02 23:54:50.000000 evadb-0.2.5/test/executor/test_limit_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3890 2023-04-09 22:04:17.000000 evadb-0.2.5/test/executor/test_load_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2884 2023-01-02 23:54:50.000000 evadb-0.2.5/test/executor/test_orderby_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10983 2023-05-16 03:45:18.000000 evadb-0.2.5/test/executor/test_plan_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1397 2022-08-08 22:30:00.000000 evadb-0.2.5/test/executor/test_pp_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1817 2023-01-02 23:54:50.000000 evadb-0.2.5/test/executor/test_sample_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2752 2023-04-09 04:33:37.000000 evadb-0.2.5/test/executor/test_seq_scan_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      847 2022-08-08 22:30:00.000000 evadb-0.2.5/test/executor/utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.173961 evadb-0.2.5/test/expression/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/expression/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3722 2023-03-28 02:19:14.000000 evadb-0.2.5/test/expression/test_abstract_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5149 2023-03-19 05:07:03.000000 evadb-0.2.5/test/expression/test_aggregation.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2975 2023-01-02 23:54:50.000000 evadb-0.2.5/test/expression/test_arithmetic.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5578 2023-01-02 23:54:53.000000 evadb-0.2.5/test/expression/test_comparison.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2867 2022-08-08 22:30:00.000000 evadb-0.2.5/test/expression/test_expression_tree.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7555 2023-04-01 16:09:26.000000 evadb-0.2.5/test/expression/test_expression_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2685 2022-11-12 17:07:12.000000 evadb-0.2.5/test/expression/test_function_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10242 2023-04-28 05:16:29.000000 evadb-0.2.5/test/expression/test_logical.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.177961 evadb-0.2.5/test/integration_tests/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/integration_tests/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3585 2023-05-09 19:58:04.000000 evadb-0.2.5/test/integration_tests/test_array_count.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4522 2023-05-09 19:58:04.000000 evadb-0.2.5/test/integration_tests/test_chatgpt.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6167 2023-05-17 22:20:34.000000 evadb-0.2.5/test/integration_tests/test_create_index_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3886 2023-06-01 22:37:10.000000 evadb-0.2.5/test/integration_tests/test_create_table_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5158 2023-05-14 18:56:25.000000 evadb-0.2.5/test/integration_tests/test_delete_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4839 2023-05-16 03:45:18.000000 evadb-0.2.5/test/integration_tests/test_drop_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2358 2023-05-14 15:06:41.000000 evadb-0.2.5/test/integration_tests/test_error_handling_with_ray.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3361 2023-05-25 14:58:01.000000 evadb-0.2.5/test/integration_tests/test_explain_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3183 2023-04-09 04:33:37.000000 evadb-0.2.5/test/integration_tests/test_fuzzy_join.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    16033 2023-06-01 22:37:10.000000 evadb-0.2.5/test/integration_tests/test_huggingface_udfs.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3806 2023-05-12 03:48:38.000000 evadb-0.2.5/test/integration_tests/test_insert_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2983 2023-05-14 15:06:41.000000 evadb-0.2.5/test/integration_tests/test_like.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    20932 2023-05-25 14:58:01.000000 evadb-0.2.5/test/integration_tests/test_load_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1961 2023-05-25 14:58:01.000000 evadb-0.2.5/test/integration_tests/test_load_pdf_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7168 2023-06-01 22:37:10.000000 evadb-0.2.5/test/integration_tests/test_mat_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2658 2023-05-09 19:58:04.000000 evadb-0.2.5/test/integration_tests/test_open.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10646 2023-05-16 03:45:18.000000 evadb-0.2.5/test/integration_tests/test_optimizer_rules.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14654 2023-06-02 21:04:24.000000 evadb-0.2.5/test/integration_tests/test_pytorch.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2953 2023-03-28 02:19:14.000000 evadb-0.2.5/test/integration_tests/test_rename_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10469 2023-05-25 14:58:01.000000 evadb-0.2.5/test/integration_tests/test_reuse.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5210 2023-04-09 04:33:37.000000 evadb-0.2.5/test/integration_tests/test_s3_load_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    30781 2023-05-09 19:58:04.000000 evadb-0.2.5/test/integration_tests/test_select_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3277 2023-05-07 22:24:29.000000 evadb-0.2.5/test/integration_tests/test_show_info_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14709 2023-05-17 22:20:34.000000 evadb-0.2.5/test/integration_tests/test_similarity.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12062 2023-04-09 04:33:37.000000 evadb-0.2.5/test/integration_tests/test_udf_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1574 2023-05-17 22:20:34.000000 evadb-0.2.5/test/markers.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.177961 evadb-0.2.5/test/models/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/models/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.177961 evadb-0.2.5/test/models/catalog/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/models/catalog/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1010 2022-10-16 04:44:32.000000 evadb-0.2.5/test/models/catalog/test_frame_info.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.177961 evadb-0.2.5/test/models/storage/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/models/storage/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5919 2023-04-09 04:33:37.000000 evadb-0.2.5/test/models/storage/test_batch.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.181961 evadb-0.2.5/test/optimizer/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/optimizer/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.181961 evadb-0.2.5/test/optimizer/rules/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-03-28 02:19:14.000000 evadb-0.2.5/test/optimizer/rules/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11653 2023-06-02 21:04:24.000000 evadb-0.2.5/test/optimizer/rules/test_rules.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4195 2023-03-16 05:59:55.000000 evadb-0.2.5/test/optimizer/test_binder.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2233 2023-05-25 14:58:01.000000 evadb-0.2.5/test/optimizer/test_cascade_optimizer.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4406 2022-08-08 22:30:00.000000 evadb-0.2.5/test/optimizer/test_cost_model.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2689 2022-08-08 22:30:00.000000 evadb-0.2.5/test/optimizer/test_group.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1996 2022-08-08 22:30:00.000000 evadb-0.2.5/test/optimizer/test_memo.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1034 2022-08-08 22:30:00.000000 evadb-0.2.5/test/optimizer/test_optimizer_context.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5522 2023-05-25 14:58:01.000000 evadb-0.2.5/test/optimizer/test_optimizer_task.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2000 2023-01-07 03:29:08.000000 evadb-0.2.5/test/optimizer/test_optimizer_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13564 2023-05-17 22:20:34.000000 evadb-0.2.5/test/optimizer/test_statement_to_opr_converter.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.181961 evadb-0.2.5/test/parser/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/parser/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    36070 2023-05-17 22:20:34.000000 evadb-0.2.5/test/parser/test_parser.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7783 2023-05-17 22:20:34.000000 evadb-0.2.5/test/parser/test_parser_statements.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.181961 evadb-0.2.5/test/plan_nodes/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-01-02 23:54:50.000000 evadb-0.2.5/test/plan_nodes/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6292 2023-03-28 02:19:14.000000 evadb-0.2.5/test/plan_nodes/test_plan.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.181961 evadb-0.2.5/test/readers/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/readers/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1688 2023-04-01 16:09:26.000000 evadb-0.2.5/test/readers/test_csv_reader.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8104 2023-05-07 22:24:29.000000 evadb-0.2.5/test/readers/test_decord_reader.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.181961 evadb-0.2.5/test/server/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-11-12 17:07:12.000000 evadb-0.2.5/test/server/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1268 2023-01-02 23:54:53.000000 evadb-0.2.5/test/server/test_command_handler.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5068 2023-06-01 22:37:10.000000 evadb-0.2.5/test/server/test_db_api.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2603 2023-06-01 22:37:10.000000 evadb-0.2.5/test/server/test_interpreter.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2066 2023-05-23 15:21:38.000000 evadb-0.2.5/test/server/test_server.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.185961 evadb-0.2.5/test/storage/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/storage/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4113 2023-05-07 22:24:29.000000 evadb-0.2.5/test/storage/test_sqlite_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4023 2023-03-28 02:19:14.000000 evadb-0.2.5/test/storage/test_video_storage.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3309 2023-05-16 03:45:18.000000 evadb-0.2.5/test/test_eva_cmd_client.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1294 2022-12-13 23:02:13.000000 evadb-0.2.5/test/test_eva_imports.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1841 2023-05-25 14:58:01.000000 evadb-0.2.5/test/test_eva_server.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.185961 evadb-0.2.5/test/udfs/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      638 2022-08-08 22:30:00.000000 evadb-0.2.5/test/udfs/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.185961 evadb-0.2.5/test/udfs/decorators/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-03-28 02:19:14.000000 evadb-0.2.5/test/udfs/decorators/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.185961 evadb-0.2.5/test/udfs/decorators/io_descriptors/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-03-28 02:19:14.000000 evadb-0.2.5/test/udfs/decorators/io_descriptors/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7429 2023-05-16 03:45:18.000000 evadb-0.2.5/test/udfs/decorators/io_descriptors/test_descriptors.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2137 2023-05-16 03:45:18.000000 evadb-0.2.5/test/udfs/decorators/test_decorators.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.185961 evadb-0.2.5/test/udfs/ndarray/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      648 2022-10-16 04:44:32.000000 evadb-0.2.5/test/udfs/ndarray/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1842 2023-06-01 22:37:10.000000 evadb-0.2.5/test/udfs/ndarray/test_annotate.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      849 2023-03-28 02:19:14.000000 evadb-0.2.5/test/udfs/ndarray/test_array_count.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2410 2022-10-16 04:44:32.000000 evadb-0.2.5/test/udfs/ndarray/test_crop.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2012 2023-05-25 14:58:01.000000 evadb-0.2.5/test/udfs/ndarray/test_flips.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1700 2023-05-25 14:58:01.000000 evadb-0.2.5/test/udfs/ndarray/test_gaussian_blur.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2374 2023-04-28 05:16:29.000000 evadb-0.2.5/test/udfs/ndarray/test_open.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1675 2023-05-25 14:58:01.000000 evadb-0.2.5/test/udfs/ndarray/test_to_grayscale.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4412 2023-05-10 04:58:49.000000 evadb-0.2.5/test/udfs/test_abstract_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2154 2022-09-30 14:24:37.000000 evadb-0.2.5/test/udfs/test_emotion_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3345 2023-03-28 02:19:14.000000 evadb-0.2.5/test/udfs/test_facenet_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2548 2022-10-30 19:28:39.000000 evadb-0.2.5/test/udfs/test_fastrcnn_object_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2768 2023-05-09 19:58:04.000000 evadb-0.2.5/test/udfs/test_yolo_object_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    17438 2023-05-16 03:45:18.000000 evadb-0.2.5/test/util.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.185961 evadb-0.2.5/test/utils/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.5/test/utils/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4196 2023-04-28 05:16:29.000000 evadb-0.2.5/test/utils/test_generic_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2256 2023-03-28 02:19:14.000000 evadb-0.2.5/test/utils/test_timer.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1296 2023-05-25 14:58:01.000000 evadb-0.2.5/test/utils/test_xdist.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-03 02:07:23.185961 evadb-0.2.5/third_party/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)        0 2022-06-26 17:11:46.000000 evadb-0.2.5/third_party/__init__.py
```

### Comparing `evadb-0.2.4/LICENSE.txt` & `evadb-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/PKG-INFO` & `evadb-0.2.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,251 +1,247 @@
 Metadata-Version: 2.1
 Name: evadb
-Version: 0.2.4
+Version: 0.2.5
 Summary: EVA AI-Relational Database System
 Home-page: https://github.com/georgia-tech-db/eva
+Download-URL: https://github.com/georgia-tech-db/eva
 Author: Georgia Tech Database Group
 Author-email: arulraj@gatech.edu
 License: Apache License 2.0
-Download-URL: https://github.com/georgia-tech-db/eva
-Description: <div >
-          <a href="https://evadb.readthedocs.io/">
-            <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-banner.png" alt="EVA" width="1000px" margin-left="-5px">
-          </a>
-        </div>
-        
-        # EVA AI-Relational Database System
-        
-        <div>
-                <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
-                    <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EVA on Colab"/>
-                </a>
-                <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
-                    <img alt="Slack" src="https://img.shields.io/badge/slack-eva-ff69b4.svg?logo=slack">
-                </a>          
-                <img alt="PyPI" src="https://img.shields.io/pypi/v/evadb.svg"/>
-                <img alt="License" src="https://img.shields.io/badge/license-Apache%202-brightgreen.svg?logo=apache"/>
-                <img alt="Coverage Status" src="https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master"/>     
-                <a href="https://github.com/orgs/georgia-tech-db/projects/3">
-                    <img src="https://img.shields.io/badge/eva-roadmap-ff3423" alt="Roadmap"/>
-                </a>
-                <a href="https://pepy.tech/project/evadb">
-                  <img alt="Downloads" src="https://static.pepy.tech/badge/evadb/month"/>
-                </a>
-                <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.8%20|%203.9%20|%203.10-brightgreen"/>       
-        </div>
-        
-        <p align="center"> <b><h3>EVA is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
-        
-        EVA is designed for supporting database applications that operate on both structured (tables, feature vectors) and unstructured data (videos, podcasts, PDFs, etc.) using deep learning models. It accelerates AI pipelines by 10-100x using a collection of optimizations inspired by time-tested relational database systems, including function caching, sampling, and cost-based predicate reordering. EVA supports an AI-oriented SQL-like query language tailored for analyzing unstructured data. It comes with a wide range of models for analyzing unstructured data, including models for object detection, question answering, OCR, text sentiment classification, face detection, etc. It is fully implemented in Python and licensed under the Apache license.
-        
-        ## Quick Links
-        
-        - [Features](#features)
-        - [Quick Start](#quick-start)
-        - [Documentation](#documentation)
-        - [Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
-        - [Architecture Diagram](#architecture-diagram)
-        - [Demo](#demo)
-        - [Illustrative Applications](#illustrative-applications)
-        - [Community and Support](#community-and-support)
-        - [Contributing](#contributing)
-        - [License](#license)
-        
-        ## Features
-        
-        - ð® Build simpler AI-powered applications using short SQL-like queries
-        - â¡ï¸ 10-100x faster AI pipelines using AI-centric query optimization  
-        - ð° Save money spent on GPU-driven inference
-        - ð First-class support for your custom deep learning models through user-defined functions
-        - ð¦ Built-in caching to eliminate redundant model invocations across queries
-        - â¨ï¸ First-class support for PyTorch and HuggingFace models
-        - ð Installable via pip and fully implemented in Python
-        
-        ## Demo
-        
-        Here are some illustrative EVA-backed applications (all of them are Jupyter notebooks that can be opened in Google Colab):
-        
-         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html">Using ChatGPT to ask questions based on videos</a>
-         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection</a>
-         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
-         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/11-similarity-search-for-motif-mining.html">Image Similarity Search on Reddit [FAISS + Qdrant]</a>
-         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
-         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/07-object-segmentation-huggingface.html">Image Segmentation using Hugging Face</a>
-         * ð® <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates </a>
-         * ð® <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
-        
-        ## Documentation
-        
-        * [Detailed Documentation](https://evadb.readthedocs.io/)
-          - If you are wondering why you might need an AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/aidb.html">Video Database Systems</a>.
-          - The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different AI pipelines, and how you can easily extend EVA by defining an user-defined function that wraps around your custom deep learning model.
-          - The <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/index.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab to run the code.
-        * [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
-        * [Join us on Slack!](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
-        * [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
-        * [Demo](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
-        
-        ## Quick Start
-        
-        - Install EVA using the pip package manager. EVA supports Python versions >= 3.7:
-        
-        ```shell
-        pip install evadb
-        ```
-        
-        - To launch and connect to an EVA server in a Jupyter notebook, check out this [illustrative emotion analysis notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb):
-        ```shell
-        cursor = connect_to_server()
-        ```
-        
-        - Load a video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration):
-        
-        ```mysql
-        LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO TrafficVideo;
-        ```
-        
-        - That's it! You can now run queries over the loaded video:
-        
-        ```mysql
-        SELECT id, data FROM TrafficVideo WHERE id < 5;
-        ```
-        
-        - Search for frames in the video that contain a car:
-        
-        ```mysql
-        SELECT id, data FROM TrafficVideo WHERE ['car'] <@ Yolo(data).labels;
-        ```
-        | Source Video  | Query Result |
-        |---------------|--------------|
-        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
-        
-        - Search for frames in the video that contain a pedestrian and a car:
-        
-        ```mysql
-        SELECT id, data FROM TrafficVideo WHERE ['pedestrian', 'car'] <@ Yolo(data).labels;
-        ```
-        
-        - Search for frames with more than three cars:
-        
-        ```mysql
-        SELECT id, data FROM TrafficVideo WHERE ArrayCount(Yolo(data).labels, 'car') > 3;
-        ```
-        
-        - **Use your custom deep learning model in queries** with a user-defined function (UDF):
-        
-        ```mysql
-        CREATE UDF IF NOT EXISTS Yolo
-        TYPE  ultralytics
-        'model' 'yolov8m.pt';
-        ```
-        
-        - **Compose multiple models in a single query** to set up useful AI pipelines.
-        
-        ```mysql
-           -- Analyse emotions of faces in a video
-           SELECT id, bbox, EmotionDetector(Crop(data, bbox)) 
-           FROM MovieVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)  
-           WHERE id < 15;
-        ```
-        
-        - **EVA runs queries faster using its AI-centric query optimizer**. Two key optimizations are:
-        
-           ð¾ **Caching**: EVA automatically caches and reuses previous query results (especially model inference results), eliminating redundant computation and reducing query processing time.
-        
-           ð¯ **Predicate Reordering**: EVA optimizes the order in which the query predicates are evaluated (e.g., runs the faster, more selective model first), leading to faster queries and lower inference costs.
-        
-        Consider these two exploratory queries on a dataset of ð images:
-        <img align="right" style="display:inline;" width="40%" src="https://github.com/georgia-tech-db/eva/blob/master/data/assets/eva_performance_comparison.png?raw=true"></a>
-        
-        ```mysql
-          -- Query 1: Find all images of black-colored dogs
-          SELECT id, bbox FROM dogs 
-          JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) 
-          WHERE Obj.label = 'dog' 
-            AND Color(Crop(data, bbox)) = 'black'; 
-        
-          -- Query 2: Find all Great Danes that are black-colored
-          SELECT id, bbox FROM dogs 
-          JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) 
-          WHERE Obj.label = 'dog' 
-            AND DogBreedClassifier(Crop(data, bbox)) = 'great dane' 
-            AND Color(Crop(data, bbox)) = 'black';
-        ```
-        
-        By reusing the results of the first query and reordering the predicates based on the available cached inference results, EVA runs the second query **10x faster**!
-        
-        ## Architecture Diagram
-        
-        The following architecture diagram presents the critical components of the EVA database system. EVA's AI-centric Query Optimizer takes a parsed query as input and generates a query plan that is then executed by the Query Engine. The Query Engine hits multiple storage engines to retrieve the data required for efficiently running the query:
-        1. Structured data (relational database system connected via `sqlalchemy`).
-        2. Unstructured media data (on cloud buckets or local filesystem).
-        3. Vector data (vector database system).
-        
-        <img width="700" alt="Architecture Diagram" src="https://github.com/georgia-tech-db/eva/assets/5521975/01452ec9-87d9-4d27-90b2-c0b1ab29b16c">
-        
-        ## Illustrative Applications 
-        
-        ### ð® [Traffic Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html) (Object Detection Model)
-        | Source Video  | Query Result |
-        |---------------|--------------|
-        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
-        
-        ### ð® [MNIST Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image Classification Model)
-        | Source Video  | Query Result |
-        |---------------|--------------|
-        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-input.webp" width="150"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-output.webp" width="150"> |
-        
-        ### ð® [Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classification Models)
-        
-        | Source Video  | Query Result |
-        |---------------|--------------|
-        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-input.webp" width="400"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-output.webp" width="400"> |
-        
-        ### ð® [License Plate Recognition](https://github.com/georgia-tech-db/eva-application-template) (Plate Detection + OCR Extraction Models)
-        
-        | Query Result |
-        |--------------|
-        <img alt="Query Result" src="https://github.com/georgia-tech-db/license-plate-recognition/blob/main/README_files/README_12_3.png" width="300"> |
-        
-        ### ð® [Meme Toxicity Classification](https://github.com/georgia-tech-db/toxicity-classification) (OCR Extraction + Toxicity Classification Models)
-        
-        | Query Result |
-        |--------------|
-        <img alt="Query Result" src="https://raw.githubusercontent.com/georgia-tech-db/toxicity-classification/main/README_files/README_16_2.png" width="200"> |
-        
-        ## Community and Support
-        
-        ð If you have general questions about EVA, want to say hello or just follow along, we'd like to invite you to join our [Slack Community](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg).
-        
-        <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">              
-            <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-slack.png" alt="EVA Slack Channel" width="500">
-        </a>
-        
-        If you run into any problems or issues, please create a Github issue and we'll try our best to help.
-        
-        Don't see a feature in the list? Search our issue tracker if someone has already requested it and add a comment to it explaining your use-case, or open a new issue if not. We prioritize our roadmap based on user feedback, so we'd love to hear from you.
-        
-        ## Contributing
-        
-        [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb)
-        [![CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva)
-        [![Documentation Status](https://readthedocs.org/projects/evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/index.html)
-        
-        EVA is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EVA are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
-        
-        For more information, see our
-        [contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
-        
-        ## License
-        Copyright (c) 2018-present [Georgia Tech Database Group](http://db.cc.gatech.edu/).
-        Licensed under [Apache License](LICENSE).
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE.txt
+
+# EVA AI-SQL Database System
+
+<div>
+        <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
+            <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EVA on Colab"/>
+        </a>
+        <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
+            <img alt="Slack" src="https://img.shields.io/badge/slack-eva-ff69b4.svg?logo=slack">
+        </a>          
+        <a href="https://twitter.com/evadb_ai">
+            <img alt="Twitter" src="https://img.shields.io/badge/twitter-eva-bde1ee.svg?logo=twitter">
+        </a>  
+        <a href="https://github.com/orgs/georgia-tech-db/projects/3">
+            <img src="https://img.shields.io/badge/eva-roadmap-a6c096" alt="Roadmap"/>
+        </a>
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/evadb.svg"/>
+        <img alt="License" src="https://img.shields.io/badge/license-Apache%202-brightgreen.svg?logo=apache"/>
+        <img alt="Coverage Status" src="https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master"/>     
+        <a href="https://pepy.tech/project/evadb">
+          <img alt="Downloads" src="https://static.pepy.tech/badge/evadb/month"/>
+        </a>
+        <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.8%20|%203.9%20|%203.10-brightgreen"/>       
+</div>
+
+<p align="center"> <b><h3>EVA DB is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
+
+EVA DB is an AI-SQL database system for developing applications powered by AI models. We aim to simplify the development and deployment of AI-powered applications that operate on structured (tables, feature stores) and unstructured data (videos, text, podcasts, PDFs, etc.).
+
+EVA DB accelerates AI pipelines by 10-100x using a collection of performance optimizations inspired by time-tested SQL database systems, including data-parallel query execution, function caching, sampling, and cost-based predicate reordering. EVA supports an AI-oriented SQL-like query language tailored for analyzing both structured and unstructured data. It has first-class support for PyTorch, Hugging Face, YOLO, and Open AI models.
+
+The high-level SQL API allows even beginners to use EVA in a few lines of code. Advanced users can define custom user-defined functions that wrap around any AI model or Python library. EVA DB is fully implemented in Python and licensed under the Apache license.
+
+## Quick Links
+
+- [Features](#features)
+- [Quick Start](#quick-start)
+- [Documentation](#documentation)
+- [Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
+- [Architecture Diagram](#architecture-diagram)
+- [Illustrative Applications](#illustrative-applications)
+- [Screenshots](#screenshots)
+- [Community and Support](#community-and-support)
+- [Twitter](https://twitter.com/evadb_ai)
+- [Contributing](#contributing)
+- [License](#license)
+
+## Features
+
+- 🔮 Build simpler AI-powered applications using short SQL-like queries
+- ⚡️ 10-100x faster AI pipelines using AI-centric query optimization  
+- 💰 Save money spent on GPUs
+- 🚀 First-class support for your custom deep learning models through user-defined functions
+- 📦 Built-in caching to eliminate redundant model invocations across queries
+- ⌨️ First-class support for PyTorch, Hugging Face, YOLO, and Open AI models
+- 🐍 Installable via pip and fully implemented in Python
+
+## Illustrative Applications
+
+Here are some illustrative EVA-powered applications (each Jupyter notebook can be opened on Google Colab):
+
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html">Using ChatGPT to ask questions based on videos</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/11-similarity-search-for-motif-mining.html">Image Similarity Search on Reddit [FAISS + Qdrant]</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/07-object-segmentation-huggingface.html">Image Segmentation using Hugging Face</a>
+ * 🔮 <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates </a>
+ * 🔮 <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
+
+## Documentation
+
+* [Detailed Documentation](https://evadb.readthedocs.io/)
+  - The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different AI tasks and how you can easily extend EVA to support your custom deep learning model through user-defined functions.
+  - The <a href="https://evadb.readthedocs.io/en/latest/source/tutorials/11-similarity-search-for-motif-mining.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab, where you can run the code yourself.
+* [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
+* [Join us on Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
+* [Follow us on Twitter](https://twitter.com/evadb_ai)
+* [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
+* [Demo](https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html)
+
+## Quick Start
+
+- Install EVA using the pip package manager. EVA supports Python versions >= 3.8:
+
+```shell
+pip install evadb
+```
+
+- To launch and connect to an EVA server in a Jupyter notebook, check out this [illustrative emotion analysis notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb):
+```shell
+cursor = connect_to_server()
+```
+
+- Load a video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration):
+
+```mysql
+LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO TrafficVideo;
+```
+
+- That's it! You can now run queries over the loaded video:
+
+```mysql
+SELECT id, data FROM TrafficVideo WHERE id < 5;
+```
+
+- Search for frames in the video that contain a car:
+
+```mysql
+SELECT id, data FROM TrafficVideo WHERE ['car'] <@ Yolo(data).labels;
+```
+| Source Video  | Query Result |
+|---------------|--------------|
+|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
+
+- Search for frames in the video that contain a pedestrian and a car:
+
+```mysql
+SELECT id, data FROM TrafficVideo WHERE ['pedestrian', 'car'] <@ Yolo(data).labels;
+```
+
+- Search for frames with more than three cars:
+
+```mysql
+SELECT id, data FROM TrafficVideo WHERE ArrayCount(Yolo(data).labels, 'car') > 3;
+```
+
+- **Use your custom deep learning model in queries** with a user-defined function (UDF):
+
+```mysql
+CREATE UDF IF NOT EXISTS Yolo
+TYPE  ultralytics
+'model' 'yolov8m.pt';
+```
+
+- **Chain multiple models in a single query** to set up useful AI pipelines.
+
+```mysql
+   -- Analyse emotions of faces in a video
+   SELECT id, bbox, EmotionDetector(Crop(data, bbox)) 
+   FROM MovieVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)  
+   WHERE id < 15;
+```
+
+- **EVA runs queries faster using its AI-centric query optimizer**. Two key optimizations are:
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
+  JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) 
+  WHERE Obj.label = 'dog' 
+    AND Color(Crop(data, bbox)) = 'black'; 
+
+  -- Query 2: Find all Great Danes that are black-colored
+  SELECT id, bbox FROM dogs 
+  JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) 
+  WHERE Obj.label = 'dog' 
+    AND DogBreedClassifier(Crop(data, bbox)) = 'great dane' 
+    AND Color(Crop(data, bbox)) = 'black';
+```
+
+By reusing the results of the first query and reordering the predicates based on the available cached inference results, EVA runs the second query **10x faster**!
+
+## Architecture Diagram
+
+This diagram presents the key components of EVA DB. EVA's AI-centric Query Optimizer takes a parsed query as input and generates a query plan that is then executed by the Query Engine. The Query Engine hits multiple storage engines to retrieve the data required for efficiently running the query:
+1. Structured data (SQL database system connected via `sqlalchemy`).
+2. Unstructured media data (on cloud buckets or local filesystem).
+3. Vector data (vector database system).
+
+<img width="700" alt="Architecture Diagram" src="https://github.com/georgia-tech-db/eva/assets/5521975/01452ec9-87d9-4d27-90b2-c0b1ab29b16c">
+
+## Screenshots
+
+### 🔮 [Traffic Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html) (Object Detection Model)
+| Source Video  | Query Result |
+|---------------|--------------|
+|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
+
+### 🔮 [MNIST Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image Classification Model)
+| Source Video  | Query Result |
+|---------------|--------------|
+|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-input.webp" width="150"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-output.webp" width="150"> |
+
+### 🔮 [Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classification Models)
+
+| Source Video  | Query Result |
+|---------------|--------------|
+|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-input.webp" width="400"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-output.webp" width="400"> |
+
+### 🔮 [License Plate Recognition](https://github.com/georgia-tech-db/eva-application-template) (Plate Detection + OCR Extraction Models)
+
+| Query Result |
+|--------------|
+<img alt="Query Result" src="https://github.com/georgia-tech-db/license-plate-recognition/blob/main/README_files/README_12_3.png" width="300"> |
+
+## Community and Support
+
+👋 If you have general questions about EVA, want to say hello or just follow along, we'd like to invite you to join our [Slack Community](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)and to [follow us on Twitter](https://twitter.com/evadb_ai).
+
+<a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">              
+    <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-slack.png" alt="EVA Slack Channel" width="500">
+</a>
+
+If you run into any problems or issues, please create a Github issue and we'll try our best to help.
+
+Don't see a feature in the list? Search our issue tracker if someone has already requested it and add a comment to it explaining your use-case, or open a new issue if not. We prioritize our [roadmap](https://github.com/orgs/georgia-tech-db/projects/3) based on user feedback, so we'd love to hear from you.
+
+## Contributing
+
+[![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb)
+[![CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva)
+[![Documentation Status](https://readthedocs.org/projects/evadb/badge/?version=latest)](https://evadb.readthedocs.io/en/latest/index.html)
+
+EVA is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EVA are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
+
+For more information, see our
+[contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
+
+## License
+Copyright (c) 2018-present [Georgia Tech Database Group](http://db.cc.gatech.edu/).
+Licensed under [Apache License](LICENSE).
```

#### html2text {}

```diff
@@ -1,140 +1,138 @@
-Metadata-Version: 2.1 Name: evadb Version: 0.2.4 Summary: EVA AI-Relational
-Database System Home-page: https://github.com/georgia-tech-db/eva Author:
-Georgia Tech Database Group Author-email: arulraj@gatech.edu License: Apache
-License 2.0 Download-URL: https://github.com/georgia-tech-db/eva Description:
-[EVA]
-# EVA AI-Relational Database System
-[Open_EVA_on_Colab] [Slack] [PyPI] [License] [Coverage Status] [Roadmap]
-[Downloads] [Python Versions]
-**** EVA is a database system for building simpler and faster AI-powered
+Metadata-Version: 2.1 Name: evadb Version: 0.2.5 Summary: EVA AI-Relational
+Database System Home-page: https://github.com/georgia-tech-db/eva Download-URL:
+https://github.com/georgia-tech-db/eva Author: Georgia Tech Database Group
+Author-email: arulraj@gatech.edu License: Apache License 2.0 Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
+text/markdown Provides-Extra: dev License-File: LICENSE.txt # EVA AI-SQL
+Database System
+[Open_EVA_on_Colab] [Slack] [Twitter] [Roadmap] [PyPI] [License] [Coverage
+Status] [Downloads] [Python Versions]
+**** EVA DB is a database system for building simpler and faster AI-powered
 applications. ****
-EVA is designed for supporting database applications that operate on both
-structured (tables, feature vectors) and unstructured data (videos, podcasts,
-PDFs, etc.) using deep learning models. It accelerates AI pipelines by 10-100x
-using a collection of optimizations inspired by time-tested relational database
-systems, including function caching, sampling, and cost-based predicate
-reordering. EVA supports an AI-oriented SQL-like query language tailored for
-analyzing unstructured data. It comes with a wide range of models for analyzing
-unstructured data, including models for object detection, question answering,
-OCR, text sentiment classification, face detection, etc. It is fully
+EVA DB is an AI-SQL database system for developing applications powered by AI
+models. We aim to simplify the development and deployment of AI-powered
+applications that operate on structured (tables, feature stores) and
+unstructured data (videos, text, podcasts, PDFs, etc.). EVA DB accelerates AI
+pipelines by 10-100x using a collection of performance optimizations inspired
+by time-tested SQL database systems, including data-parallel query execution,
+function caching, sampling, and cost-based predicate reordering. EVA supports
+an AI-oriented SQL-like query language tailored for analyzing both structured
+and unstructured data. It has first-class support for PyTorch, Hugging Face,
+YOLO, and Open AI models. The high-level SQL API allows even beginners to use
+EVA in a few lines of code. Advanced users can define custom user-defined
+functions that wrap around any AI model or Python library. EVA DB is fully
 implemented in Python and licensed under the Apache license. ## Quick Links -
 [Features](#features) - [Quick Start](#quick-start) - [Documentation]
 (#documentation) - [Roadmap](https://github.com/orgs/georgia-tech-db/projects/
-3) - [Architecture Diagram](#architecture-diagram) - [Demo](#demo) -
-[Illustrative Applications](#illustrative-applications) - [Community and
-Support](#community-and-support) - [Contributing](#contributing) - [License]
-(#license) ## Features - Ã°ÂÂÂ® Build simpler AI-powered applications using
-short SQL-like queries - Ã¢ÂÂ¡Ã¯Â¸Â 10-100x faster AI pipelines using AI-
-centric query optimization - Ã°ÂÂÂ° Save money spent on GPU-driven inference
-- Ã°ÂÂÂ First-class support for your custom deep learning models through
-user-defined functions - Ã°ÂÂÂ¦ Built-in caching to eliminate redundant model
-invocations across queries - Ã¢ÂÂ¨Ã¯Â¸Â First-class support for PyTorch and
-HuggingFace models - Ã°ÂÂÂ Installable via pip and fully implemented in
-Python ## Demo Here are some illustrative EVA-backed applications (all of them
-are Jupyter notebooks that can be opened in Google Colab): * Ã°ÂÂÂ® Using
-ChatGPT_to_ask_questions_based_on_videos * Ã°ÂÂÂ® Analysing_traffic_flow_at
-an_intersection * Ã°ÂÂÂ® Examining_the_emotion_palette_of_actors_in_a_movie *
-Ã°ÂÂÂ® Image_Similarity_Search_on_Reddit_[FAISS_+_Qdrant] * Ã°ÂÂÂ®
-Classifying_images_based_on_their_content * Ã°ÂÂÂ® Image_Segmentation_using
-Hugging_Face * Ã°ÂÂÂ® Recognizing_license_plates * Ã°ÂÂÂ® Analysing
-toxicity_of_social_media_memes ## Documentation * [Detailed Documentation]
-(https://evadb.readthedocs.io/) - If you are wondering why you might need an
-AI-relational database system, start with the page on Video_Database_Systems. -
-The Getting_Started page shows how you can use EVA for different AI pipelines,
-and how you can easily extend EVA by defining an user-defined function that
-wraps around your custom deep learning model. - The User_Guides section
-contains Jupyter Notebooks that demonstrate how to use various features of EVA.
-Each notebook includes a link to Google Colab to run the code. * [Tutorials]
-(https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-
-analysis.ipynb) * [Join us on Slack!](https://join.slack.com/t/eva-db/
-shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Medium-Term Roadmap]
-(https://github.com/orgs/georgia-tech-db/projects/3) * [Demo](https://
+3) - [Architecture Diagram](#architecture-diagram) - [Illustrative
+Applications](#illustrative-applications) - [Screenshots](#screenshots) -
+[Community and Support](#community-and-support) - [Twitter](https://
+twitter.com/evadb_ai) - [Contributing](#contributing) - [License](#license) ##
+Features - ð® Build simpler AI-powered applications using short SQL-like
+queries - â¡ï¸ 10-100x faster AI pipelines using AI-centric query
+optimization - ð° Save money spent on GPUs - ð First-class support for
+your custom deep learning models through user-defined functions - ð¦ Built-in
+caching to eliminate redundant model invocations across queries - â¨ï¸ First-
+class support for PyTorch, Hugging Face, YOLO, and Open AI models - ð
+Installable via pip and fully implemented in Python ## Illustrative
+Applications Here are some illustrative EVA-powered applications (each Jupyter
+notebook can be opened on Google Colab): * ð® Using_ChatGPT_to_ask_questions
+based_on_videos * ð® Analysing_traffic_flow_at_an_intersection * ð®
+Examining_the_emotion_palette_of_actors_in_a_movie * ð® Image_Similarity
+Search_on_Reddit_[FAISS_+_Qdrant] * ð® Classifying_images_based_on_their
+content * ð® Image_Segmentation_using_Hugging_Face * ð® Recognizing_license
+plates * ð® Analysing_toxicity_of_social_media_memes ## Documentation *
+[Detailed Documentation](https://evadb.readthedocs.io/) - The Getting_Started
+page shows how you can use EVA for different AI tasks and how you can easily
+extend EVA to support your custom deep learning model through user-defined
+functions. - The User_Guides section contains Jupyter Notebooks that
+demonstrate how to use various features of EVA. Each notebook includes a link
+to Google Colab, where you can run the code yourself. * [Tutorials](https://
 github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
-## Quick Start - Install EVA using the pip package manager. EVA supports Python
-versions >= 3.7: ```shell pip install evadb ``` - To launch and connect to an
-EVA server in a Jupyter notebook, check out this [illustrative emotion analysis
-notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-
-emotion-analysis.ipynb): ```shell cursor = connect_to_server() ``` - Load a
-video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4)
-for illustration): ```mysql LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO
-TrafficVideo; ``` - That's it! You can now run queries over the loaded video:
-```mysql SELECT id, data FROM TrafficVideo WHERE id < 5; ``` - Search for
-frames in the video that contain a car: ```mysql SELECT id, data FROM
-TrafficVideo WHERE ['car'] <@ Yolo(data).labels; ``` | Source Video | Query
-Result | |---------------|--------------| |[Source Video] |[Query Result] | -
-Search for frames in the video that contain a pedestrian and a car: ```mysql
-SELECT id, data FROM TrafficVideo WHERE ['pedestrian', 'car'] <@ Yolo
-(data).labels; ``` - Search for frames with more than three cars: ```mysql
-SELECT id, data FROM TrafficVideo WHERE ArrayCount(Yolo(data).labels, 'car') >
-3; ``` - **Use your custom deep learning model in queries** with a user-defined
-function (UDF): ```mysql CREATE UDF IF NOT EXISTS Yolo TYPE ultralytics 'model'
-'yolov8m.pt'; ``` - **Compose multiple models in a single query** to set up
-useful AI pipelines. ```mysql -- Analyse emotions of faces in a video SELECT
-id, bbox, EmotionDetector(Crop(data, bbox)) FROM MovieVideo JOIN LATERAL UNNEST
-(FaceDetector(data)) AS Face(bbox, conf) WHERE id < 15; ``` - **EVA runs
-queries faster using its AI-centric query optimizer**. Two key optimizations
-are: Ã°ÂÂÂ¾ **Caching**: EVA automatically caches and reuses previous query
-results (especially model inference results), eliminating redundant computation
-and reducing query processing time. Ã°ÂÂÂ¯ **Predicate Reordering**: EVA
-optimizes the order in which the query predicates are evaluated (e.g., runs the
-faster, more selective model first), leading to faster queries and lower
-inference costs. Consider these two exploratory queries on a dataset of
-Ã°ÂÂÂ images: [https://github.com/georgia-tech-db/eva/blob/master/data/
-assets/eva_performance_comparison.png?raw=true]
+* [Join us on Slack](https://join.slack.com/t/eva-db/shared_invite/zt-
+1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Follow us on Twitter](https://twitter.com/
+evadb_ai) * [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/
+projects/3) * [Demo](https://evadb.readthedocs.io/en/stable/source/tutorials/
+08-chatgpt.html) ## Quick Start - Install EVA using the pip package manager.
+EVA supports Python versions >= 3.8: ```shell pip install evadb ``` - To launch
+and connect to an EVA server in a Jupyter notebook, check out this
+[illustrative emotion analysis notebook](https://github.com/georgia-tech-db/
+eva/blob/master/tutorials/03-emotion-analysis.ipynb): ```shell cursor =
+connect_to_server() ``` - Load a video onto the EVA server (we use
+[ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration): ```mysql LOAD
+VIDEO "data/ua_detrac/ua_detrac.mp4" INTO TrafficVideo; ``` - That's it! You
+can now run queries over the loaded video: ```mysql SELECT id, data FROM
+TrafficVideo WHERE id < 5; ``` - Search for frames in the video that contain a
+car: ```mysql SELECT id, data FROM TrafficVideo WHERE ['car'] <@ Yolo
+(data).labels; ``` | Source Video | Query Result | |---------------|-----------
+---| |[Source Video] |[Query Result] | - Search for frames in the video that
+contain a pedestrian and a car: ```mysql SELECT id, data FROM TrafficVideo
+WHERE ['pedestrian', 'car'] <@ Yolo(data).labels; ``` - Search for frames with
+more than three cars: ```mysql SELECT id, data FROM TrafficVideo WHERE
+ArrayCount(Yolo(data).labels, 'car') > 3; ``` - **Use your custom deep learning
+model in queries** with a user-defined function (UDF): ```mysql CREATE UDF IF
+NOT EXISTS Yolo TYPE ultralytics 'model' 'yolov8m.pt'; ``` - **Chain multiple
+models in a single query** to set up useful AI pipelines. ```mysql -- Analyse
+emotions of faces in a video SELECT id, bbox, EmotionDetector(Crop(data, bbox))
+FROM MovieVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)
+WHERE id < 15; ``` - **EVA runs queries faster using its AI-centric query
+optimizer**. Two key optimizations are: ð¾ **Caching**: EVA automatically
+caches and reuses previous query results (especially model inference results),
+eliminating redundant computation and reducing query processing time. ð¯
+**Predicate Reordering**: EVA optimizes the order in which the query predicates
+are evaluated (e.g., runs the faster, more selective model first), leading to
+faster queries and lower inference costs. Consider these two exploratory
+queries on a dataset of dog images: [https://github.com/georgia-tech-db/eva/
+blob/master/data/assets/eva_performance_comparison.png?raw=true]
  ```mysql -- Query 1: Find all images of black-colored dogs SELECT id, bbox
 FROM dogs JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) WHERE
 Obj.label = 'dog' AND Color(Crop(data, bbox)) = 'black'; -- Query 2: Find all
 Great Danes that are black-colored SELECT id, bbox FROM dogs JOIN LATERAL
 UNNEST(Yolo(data)) AS Obj(label, bbox, score) WHERE Obj.label = 'dog' AND
 DogBreedClassifier(Crop(data, bbox)) = 'great dane' AND Color(Crop(data, bbox))
 = 'black'; ``` By reusing the results of the first query and reordering the
 predicates based on the available cached inference results, EVA runs the second
-query **10x faster**! ## Architecture Diagram The following architecture
-diagram presents the critical components of the EVA database system. EVA's AI-
-centric Query Optimizer takes a parsed query as input and generates a query
-plan that is then executed by the Query Engine. The Query Engine hits multiple
-storage engines to retrieve the data required for efficiently running the
-query: 1. Structured data (relational database system connected via
-`sqlalchemy`). 2. Unstructured media data (on cloud buckets or local
-filesystem). 3. Vector data (vector database system). [Architecture Diagram] ##
-Illustrative Applications ### Ã°ÂÂÂ® [Traffic Analysis](https://
+query **10x faster**! ## Architecture Diagram This diagram presents the key
+components of EVA DB. EVA's AI-centric Query Optimizer takes a parsed query as
+input and generates a query plan that is then executed by the Query Engine. The
+Query Engine hits multiple storage engines to retrieve the data required for
+efficiently running the query: 1. Structured data (SQL database system
+connected via `sqlalchemy`). 2. Unstructured media data (on cloud buckets or
+local filesystem). 3. Vector data (vector database system). [Architecture
+Diagram] ## Screenshots ### ð® [Traffic Analysis](https://
 evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html)
 (Object Detection Model) | Source Video | Query Result | |---------------|-----
----------| |[Source Video] |[Query Result] | ### Ã°ÂÂÂ® [MNIST Digit
-Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-
-mnist.html) (Image Classification Model) | Source Video | Query Result | |-----
-----------|--------------| |[Source Video] |[Query Result] | ### Ã°ÂÂÂ®
-[Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/
-tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classification
-Models) | Source Video | Query Result | |---------------|--------------| |
-[Source Video] |[Query Result] | ### Ã°ÂÂÂ® [License Plate Recognition]
-(https://github.com/georgia-tech-db/eva-application-template) (Plate Detection
-+ OCR Extraction Models) | Query Result | |--------------| [Query Result] | ###
-Ã°ÂÂÂ® [Meme Toxicity Classification](https://github.com/georgia-tech-db/
-toxicity-classification) (OCR Extraction + Toxicity Classification Models) |
-Query Result | |--------------| [Query Result] | ## Community and Support
-Ã°ÂÂÂ If you have general questions about EVA, want to say hello or just
-follow along, we'd like to invite you to join our [Slack Community](https://
-join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg).
-[EVA_Slack_Channel] If you run into any problems or issues, please create a
-Github issue and we'll try our best to help. Don't see a feature in the list?
-Search our issue tracker if someone has already requested it and add a comment
-to it explaining your use-case, or open a new issue if not. We prioritize our
-roadmap based on user feedback, so we'd love to hear from you. ## Contributing
-[![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/
-project/evadb) [![CI Status](https://circleci.com/gh/georgia-tech-db/
-eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva) [!
+---------| |[Source Video] |[Query Result] | ### ð® [MNIST Digit Recognition]
+(https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image
+Classification Model) | Source Video | Query Result | |---------------|--------
+------| |[Source Video] |[Query Result] | ### ð® [Movie Emotion Analysis]
+(https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-
+analysis.html) (Face Detection + Emotion Classification Models) | Source Video
+| Query Result | |---------------|--------------| |[Source Video] |[Query
+Result] | ### ð® [License Plate Recognition](https://github.com/georgia-tech-
+db/eva-application-template) (Plate Detection + OCR Extraction Models) | Query
+Result | |--------------| [Query Result] | ## Community and Support ð If you
+have general questions about EVA, want to say hello or just follow along, we'd
+like to invite you to join our [Slack Community](https://join.slack.com/t/eva-
+db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)and to [follow us on
+Twitter](https://twitter.com/evadb_ai). [EVA_Slack_Channel] If you run into any
+problems or issues, please create a Github issue and we'll try our best to
+help. Don't see a feature in the list? Search our issue tracker if someone has
+already requested it and add a comment to it explaining your use-case, or open
+a new issue if not. We prioritize our [roadmap](https://github.com/orgs/
+georgia-tech-db/projects/3) based on user feedback, so we'd love to hear from
+you. ## Contributing [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)]
+(https://pypi.org/project/evadb) [![CI Status](https://circleci.com/gh/georgia-
+tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva) [!
 [Documentation Status](https://readthedocs.org/projects/evadb/badge/
-?version=stable)](https://evadb.readthedocs.io/en/stable/index.html) EVA is the
+?version=latest)](https://evadb.readthedocs.io/en/latest/index.html) EVA is the
 beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/
 graphs/contributors). All kinds of contributions to EVA are appreciated. To
 file a bug or to request a feature, please use GitHub_issues. Pull_requests are
 welcome. For more information, see our [contribution guide](https://
 evadb.readthedocs.io/en/stable/source/contribute/index.html). ## License
 Copyright (c) 2018-present [Georgia Tech Database Group](http://
-db.cc.gatech.edu/). Licensed under [Apache License](LICENSE). Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
-OSI Approved :: Apache Software License Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: dev
+db.cc.gatech.edu/). Licensed under [Apache License](LICENSE).
```

### Comparing `evadb-0.2.4/README.md` & `evadb-0.2.5/evadb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,88 +1,109 @@
-<div >
-  <a href="https://evadb.readthedocs.io/">
-    <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-banner.png" alt="EVA" width="1000px" margin-left="-5px">
-  </a>
-</div>
+Metadata-Version: 2.1
+Name: evadb
+Version: 0.2.5
+Summary: EVA AI-Relational Database System
+Home-page: https://github.com/georgia-tech-db/eva
+Download-URL: https://github.com/georgia-tech-db/eva
+Author: Georgia Tech Database Group
+Author-email: arulraj@gatech.edu
+License: Apache License 2.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.txt
 
-# EVA AI-Relational Database System
+# EVA AI-SQL Database System
 
 <div>
         <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
             <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EVA on Colab"/>
         </a>
         <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
             <img alt="Slack" src="https://img.shields.io/badge/slack-eva-ff69b4.svg?logo=slack">
         </a>          
+        <a href="https://twitter.com/evadb_ai">
+            <img alt="Twitter" src="https://img.shields.io/badge/twitter-eva-bde1ee.svg?logo=twitter">
+        </a>  
+        <a href="https://github.com/orgs/georgia-tech-db/projects/3">
+            <img src="https://img.shields.io/badge/eva-roadmap-a6c096" alt="Roadmap"/>
+        </a>
         <img alt="PyPI" src="https://img.shields.io/pypi/v/evadb.svg"/>
         <img alt="License" src="https://img.shields.io/badge/license-Apache%202-brightgreen.svg?logo=apache"/>
         <img alt="Coverage Status" src="https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master"/>     
-        <a href="https://github.com/orgs/georgia-tech-db/projects/3">
-            <img src="https://img.shields.io/badge/eva-roadmap-ff3423" alt="Roadmap"/>
-        </a>
         <a href="https://pepy.tech/project/evadb">
           <img alt="Downloads" src="https://static.pepy.tech/badge/evadb/month"/>
         </a>
         <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.8%20|%203.9%20|%203.10-brightgreen"/>       
 </div>
 
-<p align="center"> <b><h3>EVA is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
+<p align="center"> <b><h3>EVA DB is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
+
+EVA DB is an AI-SQL database system for developing applications powered by AI models. We aim to simplify the development and deployment of AI-powered applications that operate on structured (tables, feature stores) and unstructured data (videos, text, podcasts, PDFs, etc.).
 
-EVA is designed for supporting database applications that operate on both structured (tables, feature vectors) and unstructured data (videos, podcasts, PDFs, etc.) using deep learning models. It accelerates AI pipelines by 10-100x using a collection of optimizations inspired by time-tested relational database systems, including function caching, sampling, and cost-based predicate reordering. EVA supports an AI-oriented SQL-like query language tailored for analyzing unstructured data. It comes with a wide range of models for analyzing unstructured data, including models for object detection, question answering, OCR, text sentiment classification, face detection, etc. It is fully implemented in Python and licensed under the Apache license.
+EVA DB accelerates AI pipelines by 10-100x using a collection of performance optimizations inspired by time-tested SQL database systems, including data-parallel query execution, function caching, sampling, and cost-based predicate reordering. EVA supports an AI-oriented SQL-like query language tailored for analyzing both structured and unstructured data. It has first-class support for PyTorch, Hugging Face, YOLO, and Open AI models.
+
+The high-level SQL API allows even beginners to use EVA in a few lines of code. Advanced users can define custom user-defined functions that wrap around any AI model or Python library. EVA DB is fully implemented in Python and licensed under the Apache license.
 
 ## Quick Links
 
 - [Features](#features)
 - [Quick Start](#quick-start)
 - [Documentation](#documentation)
 - [Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
 - [Architecture Diagram](#architecture-diagram)
-- [Demo](#demo)
 - [Illustrative Applications](#illustrative-applications)
+- [Screenshots](#screenshots)
 - [Community and Support](#community-and-support)
+- [Twitter](https://twitter.com/evadb_ai)
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Features
 
 - 🔮 Build simpler AI-powered applications using short SQL-like queries
 - ⚡️ 10-100x faster AI pipelines using AI-centric query optimization  
-- 💰 Save money spent on GPU-driven inference
+- 💰 Save money spent on GPUs
 - 🚀 First-class support for your custom deep learning models through user-defined functions
 - 📦 Built-in caching to eliminate redundant model invocations across queries
-- ⌨️ First-class support for PyTorch and HuggingFace models
+- ⌨️ First-class support for PyTorch, Hugging Face, YOLO, and Open AI models
 - 🐍 Installable via pip and fully implemented in Python
 
-## Demo
+## Illustrative Applications
 
-Here are some illustrative EVA-backed applications (all of them are Jupyter notebooks that can be opened in Google Colab):
+Here are some illustrative EVA-powered applications (each Jupyter notebook can be opened on Google Colab):
 
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html">Using ChatGPT to ask questions based on videos</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/11-similarity-search-for-motif-mining.html">Image Similarity Search on Reddit [FAISS + Qdrant]</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
  * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/07-object-segmentation-huggingface.html">Image Segmentation using Hugging Face</a>
  * 🔮 <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates </a>
  * 🔮 <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
 
 ## Documentation
 
 * [Detailed Documentation](https://evadb.readthedocs.io/)
-  - If you are wondering why you might need an AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/aidb.html">Video Database Systems</a>.
-  - The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different AI pipelines, and how you can easily extend EVA by defining an user-defined function that wraps around your custom deep learning model.
-  - The <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/index.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab to run the code.
+  - The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different AI tasks and how you can easily extend EVA to support your custom deep learning model through user-defined functions.
+  - The <a href="https://evadb.readthedocs.io/en/latest/source/tutorials/11-similarity-search-for-motif-mining.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab, where you can run the code yourself.
 * [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
-* [Join us on Slack!](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
+* [Join us on Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
+* [Follow us on Twitter](https://twitter.com/evadb_ai)
 * [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
-* [Demo](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
+* [Demo](https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html)
 
 ## Quick Start
 
-- Install EVA using the pip package manager. EVA supports Python versions >= 3.7:
+- Install EVA using the pip package manager. EVA supports Python versions >= 3.8:
 
 ```shell
 pip install evadb
 ```
 
 - To launch and connect to an EVA server in a Jupyter notebook, check out this [illustrative emotion analysis notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb):
 ```shell
@@ -126,30 +147,30 @@
 
 ```mysql
 CREATE UDF IF NOT EXISTS Yolo
 TYPE  ultralytics
 'model' 'yolov8m.pt';
 ```
 
-- **Compose multiple models in a single query** to set up useful AI pipelines.
+- **Chain multiple models in a single query** to set up useful AI pipelines.
 
 ```mysql
    -- Analyse emotions of faces in a video
    SELECT id, bbox, EmotionDetector(Crop(data, bbox)) 
    FROM MovieVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)  
    WHERE id < 15;
 ```
 
 - **EVA runs queries faster using its AI-centric query optimizer**. Two key optimizations are:
 
    💾 **Caching**: EVA automatically caches and reuses previous query results (especially model inference results), eliminating redundant computation and reducing query processing time.
 
    🎯 **Predicate Reordering**: EVA optimizes the order in which the query predicates are evaluated (e.g., runs the faster, more selective model first), leading to faster queries and lower inference costs.
 
-Consider these two exploratory queries on a dataset of 🐕 images:
+Consider these two exploratory queries on a dataset of dog images:
 <img align="right" style="display:inline;" width="40%" src="https://github.com/georgia-tech-db/eva/blob/master/data/assets/eva_performance_comparison.png?raw=true"></a>
 
 ```mysql
   -- Query 1: Find all images of black-colored dogs
   SELECT id, bbox FROM dogs 
   JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) 
   WHERE Obj.label = 'dog' 
@@ -163,22 +184,22 @@
     AND Color(Crop(data, bbox)) = 'black';
 ```
 
 By reusing the results of the first query and reordering the predicates based on the available cached inference results, EVA runs the second query **10x faster**!
 
 ## Architecture Diagram
 
-The following architecture diagram presents the critical components of the EVA database system. EVA's AI-centric Query Optimizer takes a parsed query as input and generates a query plan that is then executed by the Query Engine. The Query Engine hits multiple storage engines to retrieve the data required for efficiently running the query:
-1. Structured data (relational database system connected via `sqlalchemy`).
+This diagram presents the key components of EVA DB. EVA's AI-centric Query Optimizer takes a parsed query as input and generates a query plan that is then executed by the Query Engine. The Query Engine hits multiple storage engines to retrieve the data required for efficiently running the query:
+1. Structured data (SQL database system connected via `sqlalchemy`).
 2. Unstructured media data (on cloud buckets or local filesystem).
 3. Vector data (vector database system).
 
 <img width="700" alt="Architecture Diagram" src="https://github.com/georgia-tech-db/eva/assets/5521975/01452ec9-87d9-4d27-90b2-c0b1ab29b16c">
 
-## Illustrative Applications 
+## Screenshots
 
 ### 🔮 [Traffic Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html) (Object Detection Model)
 | Source Video  | Query Result |
 |---------------|--------------|
 |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
 
 ### 🔮 [MNIST Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image Classification Model)
@@ -194,37 +215,31 @@
 
 ### 🔮 [License Plate Recognition](https://github.com/georgia-tech-db/eva-application-template) (Plate Detection + OCR Extraction Models)
 
 | Query Result |
 |--------------|
 <img alt="Query Result" src="https://github.com/georgia-tech-db/license-plate-recognition/blob/main/README_files/README_12_3.png" width="300"> |
 
-### 🔮 [Meme Toxicity Classification](https://github.com/georgia-tech-db/toxicity-classification) (OCR Extraction + Toxicity Classification Models)
-
-| Query Result |
-|--------------|
-<img alt="Query Result" src="https://raw.githubusercontent.com/georgia-tech-db/toxicity-classification/main/README_files/README_16_2.png" width="200"> |
-
 ## Community and Support
 
-👋 If you have general questions about EVA, want to say hello or just follow along, we'd like to invite you to join our [Slack Community](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg).
+👋 If you have general questions about EVA, want to say hello or just follow along, we'd like to invite you to join our [Slack Community](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)and to [follow us on Twitter](https://twitter.com/evadb_ai).
 
 <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">              
     <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-slack.png" alt="EVA Slack Channel" width="500">
 </a>
 
 If you run into any problems or issues, please create a Github issue and we'll try our best to help.
 
-Don't see a feature in the list? Search our issue tracker if someone has already requested it and add a comment to it explaining your use-case, or open a new issue if not. We prioritize our roadmap based on user feedback, so we'd love to hear from you.
+Don't see a feature in the list? Search our issue tracker if someone has already requested it and add a comment to it explaining your use-case, or open a new issue if not. We prioritize our [roadmap](https://github.com/orgs/georgia-tech-db/projects/3) based on user feedback, so we'd love to hear from you.
 
 ## Contributing
 
 [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb)
 [![CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva)
-[![Documentation Status](https://readthedocs.org/projects/evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/index.html)
+[![Documentation Status](https://readthedocs.org/projects/evadb/badge/?version=latest)](https://evadb.readthedocs.io/en/latest/index.html)
 
 EVA is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EVA are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
 
 For more information, see our
 [contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
 
 ## License
```

#### html2text {}

```diff
@@ -1,130 +1,138 @@
-[EVA]
-# EVA AI-Relational Database System
-[Open_EVA_on_Colab] [Slack] [PyPI] [License] [Coverage Status] [Roadmap]
-[Downloads] [Python Versions]
-**** EVA is a database system for building simpler and faster AI-powered
+Metadata-Version: 2.1 Name: evadb Version: 0.2.5 Summary: EVA AI-Relational
+Database System Home-page: https://github.com/georgia-tech-db/eva Download-URL:
+https://github.com/georgia-tech-db/eva Author: Georgia Tech Database Group
+Author-email: arulraj@gatech.edu License: Apache License 2.0 Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
+text/markdown Provides-Extra: dev License-File: LICENSE.txt # EVA AI-SQL
+Database System
+[Open_EVA_on_Colab] [Slack] [Twitter] [Roadmap] [PyPI] [License] [Coverage
+Status] [Downloads] [Python Versions]
+**** EVA DB is a database system for building simpler and faster AI-powered
 applications. ****
-EVA is designed for supporting database applications that operate on both
-structured (tables, feature vectors) and unstructured data (videos, podcasts,
-PDFs, etc.) using deep learning models. It accelerates AI pipelines by 10-100x
-using a collection of optimizations inspired by time-tested relational database
-systems, including function caching, sampling, and cost-based predicate
-reordering. EVA supports an AI-oriented SQL-like query language tailored for
-analyzing unstructured data. It comes with a wide range of models for analyzing
-unstructured data, including models for object detection, question answering,
-OCR, text sentiment classification, face detection, etc. It is fully
+EVA DB is an AI-SQL database system for developing applications powered by AI
+models. We aim to simplify the development and deployment of AI-powered
+applications that operate on structured (tables, feature stores) and
+unstructured data (videos, text, podcasts, PDFs, etc.). EVA DB accelerates AI
+pipelines by 10-100x using a collection of performance optimizations inspired
+by time-tested SQL database systems, including data-parallel query execution,
+function caching, sampling, and cost-based predicate reordering. EVA supports
+an AI-oriented SQL-like query language tailored for analyzing both structured
+and unstructured data. It has first-class support for PyTorch, Hugging Face,
+YOLO, and Open AI models. The high-level SQL API allows even beginners to use
+EVA in a few lines of code. Advanced users can define custom user-defined
+functions that wrap around any AI model or Python library. EVA DB is fully
 implemented in Python and licensed under the Apache license. ## Quick Links -
 [Features](#features) - [Quick Start](#quick-start) - [Documentation]
 (#documentation) - [Roadmap](https://github.com/orgs/georgia-tech-db/projects/
-3) - [Architecture Diagram](#architecture-diagram) - [Demo](#demo) -
-[Illustrative Applications](#illustrative-applications) - [Community and
-Support](#community-and-support) - [Contributing](#contributing) - [License]
-(#license) ## Features - ð® Build simpler AI-powered applications using short
-SQL-like queries - â¡ï¸ 10-100x faster AI pipelines using AI-centric query
-optimization - ð° Save money spent on GPU-driven inference - ð First-class
-support for your custom deep learning models through user-defined functions -
-ð¦ Built-in caching to eliminate redundant model invocations across queries -
-â¨ï¸ First-class support for PyTorch and HuggingFace models - ð
-Installable via pip and fully implemented in Python ## Demo Here are some
-illustrative EVA-backed applications (all of them are Jupyter notebooks that
-can be opened in Google Colab): * ð® Using_ChatGPT_to_ask_questions_based_on
-videos * ð® Analysing_traffic_flow_at_an_intersection * ð® Examining_the
-emotion_palette_of_actors_in_a_movie * ð® Image_Similarity_Search_on_Reddit_
-[FAISS_+_Qdrant] * ð® Classifying_images_based_on_their_content * ð® Image
-Segmentation_using_Hugging_Face * ð® Recognizing_license_plates * ð®
-Analysing_toxicity_of_social_media_memes ## Documentation * [Detailed
-Documentation](https://evadb.readthedocs.io/) - If you are wondering why you
-might need an AI-relational database system, start with the page on Video
-Database_Systems. - The Getting_Started page shows how you can use EVA for
-different AI pipelines, and how you can easily extend EVA by defining an user-
-defined function that wraps around your custom deep learning model. - The User
-Guides section contains Jupyter Notebooks that demonstrate how to use various
-features of EVA. Each notebook includes a link to Google Colab to run the code.
-* [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-
-emotion-analysis.ipynb) * [Join us on Slack!](https://join.slack.com/t/eva-db/
-shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Medium-Term Roadmap]
-(https://github.com/orgs/georgia-tech-db/projects/3) * [Demo](https://
+3) - [Architecture Diagram](#architecture-diagram) - [Illustrative
+Applications](#illustrative-applications) - [Screenshots](#screenshots) -
+[Community and Support](#community-and-support) - [Twitter](https://
+twitter.com/evadb_ai) - [Contributing](#contributing) - [License](#license) ##
+Features - ð® Build simpler AI-powered applications using short SQL-like
+queries - â¡ï¸ 10-100x faster AI pipelines using AI-centric query
+optimization - ð° Save money spent on GPUs - ð First-class support for
+your custom deep learning models through user-defined functions - ð¦ Built-in
+caching to eliminate redundant model invocations across queries - â¨ï¸ First-
+class support for PyTorch, Hugging Face, YOLO, and Open AI models - ð
+Installable via pip and fully implemented in Python ## Illustrative
+Applications Here are some illustrative EVA-powered applications (each Jupyter
+notebook can be opened on Google Colab): * ð® Using_ChatGPT_to_ask_questions
+based_on_videos * ð® Analysing_traffic_flow_at_an_intersection * ð®
+Examining_the_emotion_palette_of_actors_in_a_movie * ð® Image_Similarity
+Search_on_Reddit_[FAISS_+_Qdrant] * ð® Classifying_images_based_on_their
+content * ð® Image_Segmentation_using_Hugging_Face * ð® Recognizing_license
+plates * ð® Analysing_toxicity_of_social_media_memes ## Documentation *
+[Detailed Documentation](https://evadb.readthedocs.io/) - The Getting_Started
+page shows how you can use EVA for different AI tasks and how you can easily
+extend EVA to support your custom deep learning model through user-defined
+functions. - The User_Guides section contains Jupyter Notebooks that
+demonstrate how to use various features of EVA. Each notebook includes a link
+to Google Colab, where you can run the code yourself. * [Tutorials](https://
 github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
-## Quick Start - Install EVA using the pip package manager. EVA supports Python
-versions >= 3.7: ```shell pip install evadb ``` - To launch and connect to an
-EVA server in a Jupyter notebook, check out this [illustrative emotion analysis
-notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-
-emotion-analysis.ipynb): ```shell cursor = connect_to_server() ``` - Load a
-video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4)
-for illustration): ```mysql LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO
-TrafficVideo; ``` - That's it! You can now run queries over the loaded video:
-```mysql SELECT id, data FROM TrafficVideo WHERE id < 5; ``` - Search for
-frames in the video that contain a car: ```mysql SELECT id, data FROM
-TrafficVideo WHERE ['car'] <@ Yolo(data).labels; ``` | Source Video | Query
-Result | |---------------|--------------| |[Source Video] |[Query Result] | -
-Search for frames in the video that contain a pedestrian and a car: ```mysql
-SELECT id, data FROM TrafficVideo WHERE ['pedestrian', 'car'] <@ Yolo
-(data).labels; ``` - Search for frames with more than three cars: ```mysql
-SELECT id, data FROM TrafficVideo WHERE ArrayCount(Yolo(data).labels, 'car') >
-3; ``` - **Use your custom deep learning model in queries** with a user-defined
-function (UDF): ```mysql CREATE UDF IF NOT EXISTS Yolo TYPE ultralytics 'model'
-'yolov8m.pt'; ``` - **Compose multiple models in a single query** to set up
-useful AI pipelines. ```mysql -- Analyse emotions of faces in a video SELECT
-id, bbox, EmotionDetector(Crop(data, bbox)) FROM MovieVideo JOIN LATERAL UNNEST
-(FaceDetector(data)) AS Face(bbox, conf) WHERE id < 15; ``` - **EVA runs
-queries faster using its AI-centric query optimizer**. Two key optimizations
-are: ð¾ **Caching**: EVA automatically caches and reuses previous query
-results (especially model inference results), eliminating redundant computation
-and reducing query processing time. ð¯ **Predicate Reordering**: EVA
-optimizes the order in which the query predicates are evaluated (e.g., runs the
-faster, more selective model first), leading to faster queries and lower
-inference costs. Consider these two exploratory queries on a dataset of ð
-images: [https://github.com/georgia-tech-db/eva/blob/master/data/assets/
-eva_performance_comparison.png?raw=true]
+* [Join us on Slack](https://join.slack.com/t/eva-db/shared_invite/zt-
+1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Follow us on Twitter](https://twitter.com/
+evadb_ai) * [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/
+projects/3) * [Demo](https://evadb.readthedocs.io/en/stable/source/tutorials/
+08-chatgpt.html) ## Quick Start - Install EVA using the pip package manager.
+EVA supports Python versions >= 3.8: ```shell pip install evadb ``` - To launch
+and connect to an EVA server in a Jupyter notebook, check out this
+[illustrative emotion analysis notebook](https://github.com/georgia-tech-db/
+eva/blob/master/tutorials/03-emotion-analysis.ipynb): ```shell cursor =
+connect_to_server() ``` - Load a video onto the EVA server (we use
+[ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration): ```mysql LOAD
+VIDEO "data/ua_detrac/ua_detrac.mp4" INTO TrafficVideo; ``` - That's it! You
+can now run queries over the loaded video: ```mysql SELECT id, data FROM
+TrafficVideo WHERE id < 5; ``` - Search for frames in the video that contain a
+car: ```mysql SELECT id, data FROM TrafficVideo WHERE ['car'] <@ Yolo
+(data).labels; ``` | Source Video | Query Result | |---------------|-----------
+---| |[Source Video] |[Query Result] | - Search for frames in the video that
+contain a pedestrian and a car: ```mysql SELECT id, data FROM TrafficVideo
+WHERE ['pedestrian', 'car'] <@ Yolo(data).labels; ``` - Search for frames with
+more than three cars: ```mysql SELECT id, data FROM TrafficVideo WHERE
+ArrayCount(Yolo(data).labels, 'car') > 3; ``` - **Use your custom deep learning
+model in queries** with a user-defined function (UDF): ```mysql CREATE UDF IF
+NOT EXISTS Yolo TYPE ultralytics 'model' 'yolov8m.pt'; ``` - **Chain multiple
+models in a single query** to set up useful AI pipelines. ```mysql -- Analyse
+emotions of faces in a video SELECT id, bbox, EmotionDetector(Crop(data, bbox))
+FROM MovieVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)
+WHERE id < 15; ``` - **EVA runs queries faster using its AI-centric query
+optimizer**. Two key optimizations are: ð¾ **Caching**: EVA automatically
+caches and reuses previous query results (especially model inference results),
+eliminating redundant computation and reducing query processing time. ð¯
+**Predicate Reordering**: EVA optimizes the order in which the query predicates
+are evaluated (e.g., runs the faster, more selective model first), leading to
+faster queries and lower inference costs. Consider these two exploratory
+queries on a dataset of dog images: [https://github.com/georgia-tech-db/eva/
+blob/master/data/assets/eva_performance_comparison.png?raw=true]
  ```mysql -- Query 1: Find all images of black-colored dogs SELECT id, bbox
 FROM dogs JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) WHERE
 Obj.label = 'dog' AND Color(Crop(data, bbox)) = 'black'; -- Query 2: Find all
 Great Danes that are black-colored SELECT id, bbox FROM dogs JOIN LATERAL
 UNNEST(Yolo(data)) AS Obj(label, bbox, score) WHERE Obj.label = 'dog' AND
 DogBreedClassifier(Crop(data, bbox)) = 'great dane' AND Color(Crop(data, bbox))
 = 'black'; ``` By reusing the results of the first query and reordering the
 predicates based on the available cached inference results, EVA runs the second
-query **10x faster**! ## Architecture Diagram The following architecture
-diagram presents the critical components of the EVA database system. EVA's AI-
-centric Query Optimizer takes a parsed query as input and generates a query
-plan that is then executed by the Query Engine. The Query Engine hits multiple
-storage engines to retrieve the data required for efficiently running the
-query: 1. Structured data (relational database system connected via
-`sqlalchemy`). 2. Unstructured media data (on cloud buckets or local
-filesystem). 3. Vector data (vector database system). [Architecture Diagram] ##
-Illustrative Applications ### ð® [Traffic Analysis](https://
+query **10x faster**! ## Architecture Diagram This diagram presents the key
+components of EVA DB. EVA's AI-centric Query Optimizer takes a parsed query as
+input and generates a query plan that is then executed by the Query Engine. The
+Query Engine hits multiple storage engines to retrieve the data required for
+efficiently running the query: 1. Structured data (SQL database system
+connected via `sqlalchemy`). 2. Unstructured media data (on cloud buckets or
+local filesystem). 3. Vector data (vector database system). [Architecture
+Diagram] ## Screenshots ### ð® [Traffic Analysis](https://
 evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html)
 (Object Detection Model) | Source Video | Query Result | |---------------|-----
 ---------| |[Source Video] |[Query Result] | ### ð® [MNIST Digit Recognition]
 (https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image
 Classification Model) | Source Video | Query Result | |---------------|--------
 ------| |[Source Video] |[Query Result] | ### ð® [Movie Emotion Analysis]
 (https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-
 analysis.html) (Face Detection + Emotion Classification Models) | Source Video
 | Query Result | |---------------|--------------| |[Source Video] |[Query
 Result] | ### ð® [License Plate Recognition](https://github.com/georgia-tech-
 db/eva-application-template) (Plate Detection + OCR Extraction Models) | Query
-Result | |--------------| [Query Result] | ### ð® [Meme Toxicity
-Classification](https://github.com/georgia-tech-db/toxicity-classification)
-(OCR Extraction + Toxicity Classification Models) | Query Result | |-----------
----| [Query Result] | ## Community and Support ð If you have general
-questions about EVA, want to say hello or just follow along, we'd like to
-invite you to join our [Slack Community](https://join.slack.com/t/eva-db/
-shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg). [EVA_Slack_Channel] If you
-run into any problems or issues, please create a Github issue and we'll try our
-best to help. Don't see a feature in the list? Search our issue tracker if
-someone has already requested it and add a comment to it explaining your use-
-case, or open a new issue if not. We prioritize our roadmap based on user
-feedback, so we'd love to hear from you. ## Contributing [![PyPI Version]
-(https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb) [!
-[CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https:/
-/circleci.com/gh/georgia-tech-db/eva) [![Documentation Status](https://
-readthedocs.org/projects/evadb/badge/?version=stable)](https://
-evadb.readthedocs.io/en/stable/index.html) EVA is the beneficiary of many
-[contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All
-kinds of contributions to EVA are appreciated. To file a bug or to request a
-feature, please use GitHub_issues. Pull_requests are welcome. For more
-information, see our [contribution guide](https://evadb.readthedocs.io/en/
-stable/source/contribute/index.html). ## License Copyright (c) 2018-present
-[Georgia Tech Database Group](http://db.cc.gatech.edu/). Licensed under [Apache
-License](LICENSE).
+Result | |--------------| [Query Result] | ## Community and Support ð If you
+have general questions about EVA, want to say hello or just follow along, we'd
+like to invite you to join our [Slack Community](https://join.slack.com/t/eva-
+db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)and to [follow us on
+Twitter](https://twitter.com/evadb_ai). [EVA_Slack_Channel] If you run into any
+problems or issues, please create a Github issue and we'll try our best to
+help. Don't see a feature in the list? Search our issue tracker if someone has
+already requested it and add a comment to it explaining your use-case, or open
+a new issue if not. We prioritize our [roadmap](https://github.com/orgs/
+georgia-tech-db/projects/3) based on user feedback, so we'd love to hear from
+you. ## Contributing [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)]
+(https://pypi.org/project/evadb) [![CI Status](https://circleci.com/gh/georgia-
+tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva) [!
+[Documentation Status](https://readthedocs.org/projects/evadb/badge/
+?version=latest)](https://evadb.readthedocs.io/en/latest/index.html) EVA is the
+beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/
+graphs/contributors). All kinds of contributions to EVA are appreciated. To
+file a bug or to request a feature, please use GitHub_issues. Pull_requests are
+welcome. For more information, see our [contribution guide](https://
+evadb.readthedocs.io/en/stable/source/contribute/index.html). ## License
+Copyright (c) 2018-present [Georgia Tech Database Group](http://
+db.cc.gatech.edu/). Licensed under [Apache License](LICENSE).
```

### Comparing `evadb-0.2.4/eva/__init__.py` & `evadb-0.2.5/eva/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/binder/__init__.py` & `evadb-0.2.5/test/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/eva/binder/binder_utils.py` & `evadb-0.2.5/eva/binder/binder_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/binder/statement_binder.py` & `evadb-0.2.5/eva/binder/statement_binder.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -25,20 +25,21 @@
     handle_bind_extract_object_function,
     resolve_alias_table_value_expression,
 )
 from eva.binder.statement_binder_context import StatementBinderContext
 from eva.catalog.catalog_manager import CatalogManager
 from eva.catalog.catalog_type import NdArrayType, TableType, VideoColumnName
 from eva.catalog.catalog_utils import get_metadata_properties
-from eva.configuration.constants import EVA_DEFAULT_DIR
+from eva.configuration.configuration_manager import ConfigurationManager
 from eva.expression.abstract_expression import AbstractExpression, ExpressionType
 from eva.expression.function_expression import FunctionExpression
 from eva.expression.tuple_value_expression import TupleValueExpression
 from eva.parser.create_index_statement import CreateIndexStatement
 from eva.parser.create_mat_view_statement import CreateMaterializedViewStatement
+from eva.parser.create_statement import ColumnDefinition, CreateTableStatement
 from eva.parser.delete_statement import DeleteTableStatement
 from eva.parser.explain_statement import ExplainStatement
 from eva.parser.rename_statement import RenameTableStatement
 from eva.parser.select_statement import SelectStatement
 from eva.parser.statement import AbstractStatement
 from eva.parser.table_ref import TableRef
 from eva.parser.types import UDFType
@@ -144,18 +145,84 @@
 
     @bind.register(DeleteTableStatement)
     def _bind_delete_statement(self, node: DeleteTableStatement):
         self.bind(node.table_ref)
         if node.where_clause:
             self.bind(node.where_clause)
 
+    @bind.register(CreateTableStatement)
+    def _bind_create_statement(self, node: CreateTableStatement):
+        if node.query is not None:
+            self.bind(node.query)
+            num_projected_columns = 0
+            for expr in node.query.target_list:
+                if expr.etype == ExpressionType.TUPLE_VALUE:
+                    num_projected_columns += 1
+                elif expr.etype == ExpressionType.FUNCTION_EXPRESSION:
+                    num_projected_columns += len(expr.output_objs)
+                else:
+                    raise BinderError("Unsupported expression type {}.".format(expr.etype))
+
+            binded_col_list = []
+            idx = 0
+            for expr in node.query.target_list:
+                output_objs = [(expr.col_name, expr.col_object)] \
+                    if expr.etype == ExpressionType.TUPLE_VALUE \
+                    else zip(expr.projection_columns, expr.output_objs)
+                for col_name, output_obj in output_objs:
+                    binded_col_list.append(
+                        ColumnDefinition(
+                            col_name,
+                            output_obj.type,
+                            output_obj.array_type,
+                            output_obj.array_dimensions,
+                        )
+                    )
+                    idx += 1
+            node.column_list = binded_col_list
+
     @bind.register(CreateMaterializedViewStatement)
     def _bind_create_mat_statement(self, node: CreateMaterializedViewStatement):
         self.bind(node.query)
-        # Todo Verify if the number projected columns matches table
+        num_projected_columns = 0
+        # TODO we should fix the binder. All binded object should have the same interface.
+        for expr in node.query.target_list:
+            if expr.etype == ExpressionType.TUPLE_VALUE:
+                num_projected_columns += 1
+            elif expr.etype == ExpressionType.FUNCTION_EXPRESSION:
+                num_projected_columns += len(expr.output_objs)
+            else:
+                raise BinderError("Unsupported expression type {}.".format(expr.etype))
+
+        assert (
+            len(node.col_list) == 0 or len(node.col_list) == num_projected_columns
+        ), "Projected columns mismatch, expected {} found {}.".format(
+            len(node.col_list), num_projected_columns
+        )
+        binded_col_list = []
+        idx = 0
+        for expr in node.query.target_list:
+            output_objs = (
+                [(expr.col_name, expr.col_object)]
+                if expr.etype == ExpressionType.TUPLE_VALUE
+                else zip(expr.projection_columns, expr.output_objs)
+            )
+            for col_name, output_obj in output_objs:
+                binded_col_list.append(
+                    ColumnDefinition(
+                        col_name
+                        if len(node.col_list) == 0
+                        else node.col_list[idx].name,
+                        output_obj.type,
+                        output_obj.array_type,
+                        output_obj.array_dimensions,
+                    )
+                )
+                idx += 1
+        node.col_list = binded_col_list
 
     @bind.register(RenameTableStatement)
     def _bind_rename_table_statement(self, node: RenameTableStatement):
         self.bind(node.old_table_ref)
         assert (
             node.old_table_ref.table.table_obj.table_type != TableType.STRUCTURED_DATA
         ), "Rename not yet supported on structured data"
@@ -236,18 +303,22 @@
         if udf_obj.type == "HuggingFace":
             node.function = assign_hf_udf(udf_obj)
 
         else:
             if udf_obj.type == "ultralytics":
                 # manually set the impl_path for yolo udfs we only handle object
                 # detection for now, hopefully this can be generalized
+                udf_dir = (
+                    Path(
+                        ConfigurationManager().get_value("core", "eva_installation_dir")
+                    )
+                    / "udfs"
+                )
                 udf_obj.impl_file_path = (
-                    Path(f"{EVA_DEFAULT_DIR}/udfs/yolo_object_detector.py")
-                    .absolute()
-                    .as_posix()
+                    Path(f"{udf_dir}/yolo_object_detector.py").absolute().as_posix()
                 )
 
             # Verify the consistency of the UDF. If the checksum of the UDF does not
             # match the one stored in the catalog, an error will be thrown and the user
             # will be asked to register the UDF again.
             assert (
                 get_file_checksum(udf_obj.impl_file_path) == udf_obj.checksum
```

### Comparing `evadb-0.2.4/eva/binder/statement_binder_context.py` & `evadb-0.2.5/eva/binder/statement_binder_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/__init__.py` & `evadb-0.2.5/eva/third_party/huggingface/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""
-catalog subdirectory
-"""
+"""hugging face utils"""
```

### Comparing `evadb-0.2.4/eva/catalog/catalog_manager.py` & `evadb-0.2.5/eva/catalog/catalog_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,15 +21,17 @@
     TableType,
     VectorStoreType,
     VideoColumnName,
 )
 from eva.catalog.catalog_utils import (
     cleanup_storage,
     construct_udf_cache_catalog_entry,
+    get_document_table_column_definitions,
     get_image_table_column_definitions,
+    get_pdf_table_column_definitions,
     get_video_table_column_definitions,
     xform_column_definitions_to_catalog_entries,
 )
 from eva.catalog.models.base_model import (
     drop_all_tables_except_catalog,
     init_db,
     truncate_catalog_tables,
@@ -420,22 +422,30 @@
 
         Returns:
             TableCatalogEntry: newly inserted table catalog entry
         """
         assert format_type in [
             FileFormatType.VIDEO,
             FileFormatType.IMAGE,
+            FileFormatType.DOCUMENT,
+            FileFormatType.PDF,
         ], f"Format Type {format_type} is not supported"
 
         if format_type is FileFormatType.VIDEO:
             columns = get_video_table_column_definitions()
             table_type = TableType.VIDEO_DATA
         elif format_type is FileFormatType.IMAGE:
             columns = get_image_table_column_definitions()
             table_type = TableType.IMAGE_DATA
+        elif format_type is FileFormatType.DOCUMENT:
+            columns = get_document_table_column_definitions()
+            table_type = TableType.DOCUMENT_DATA
+        elif format_type is FileFormatType.PDF:
+            columns = get_pdf_table_column_definitions()
+            table_type = TableType.PDF_DATA
 
         return self.create_and_insert_table_catalog_entry(
             TableInfo(name), columns, table_type=table_type
         )
 
     def get_multimedia_metadata_table_catalog_entry(
         self, input_table: TableCatalogEntry
```

### Comparing `evadb-0.2.4/eva/catalog/catalog_type.py` & `evadb-0.2.5/eva/catalog/catalog_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -20,14 +20,16 @@
     ANYDIM  # noqa: F821
 
 
 class TableType(EVAEnum):
     STRUCTURED_DATA  # noqa: F821
     VIDEO_DATA  # noqa: F821
     IMAGE_DATA  # noqa: F821
+    DOCUMENT_DATA  # noqa: F821
+    PDF_DATA  # noqa: F821
 
     # reserved for system generated tables
     # cannot be accessed/modified directly by user
     SYSTEM_STRUCTURED_DATA  # noqa: F821
 
 
 class ColumnType(EVAEnum):
@@ -113,7 +115,20 @@
 
         return False
 
 
 class ImageColumnName(EVAEnum):
     name  # noqa: F821
     data  # noqa: F821
+
+
+class DocumentColumnName(EVAEnum):
+    name  # noqa: F821
+    data  # noqa: F821
+    metadata  # noqa: F821
+
+
+class PDFColumnName(EVAEnum):
+    name  # noqa: F821
+    page  # noqa: F821
+    paragraph  # noqa: F821
+    data  # noqa: F821
```

### Comparing `evadb-0.2.4/eva/catalog/catalog_utils.py` & `evadb-0.2.5/eva/catalog/catalog_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,16 +14,18 @@
 # limitations under the License.
 import uuid
 from pathlib import Path
 from typing import Any, Dict, List
 
 from eva.catalog.catalog_type import (
     ColumnType,
+    DocumentColumnName,
     ImageColumnName,
     NdArrayType,
+    PDFColumnName,
     TableType,
     VideoColumnName,
 )
 from eva.catalog.models.column_catalog import ColumnCatalogEntry
 from eva.catalog.models.table_catalog import TableCatalogEntry
 from eva.catalog.models.udf_cache_catalog import UdfCacheCatalogEntry
 from eva.catalog.models.udf_catalog import UdfCatalogEntry
@@ -101,19 +103,67 @@
             NdArrayType.UINT8,
             (None, None, None),
         ),
     ]
     return columns
 
 
+def get_document_table_column_definitions() -> List[ColumnDefinition]:
+    """
+    name: file path
+    data: file extracted data
+    """
+    columns = [
+        ColumnDefinition(
+            DocumentColumnName.name.name,
+            ColumnType.TEXT,
+            None,
+            None,
+            ColConstraintInfo(unique=True),
+        ),
+        ColumnDefinition(
+            DocumentColumnName.data.name,
+            ColumnType.TEXT,
+            None,
+            None,
+        ),
+    ]
+    return columns
+
+
+def get_pdf_table_column_definitions() -> List[ColumnDefinition]:
+    """
+    name: pdf name
+    page: page no
+    paragraph: paragraph no
+    data: pdf paragraph data
+    """
+    columns = [
+        ColumnDefinition(PDFColumnName.name.name, ColumnType.TEXT, None, None),
+        ColumnDefinition(PDFColumnName.page.name, ColumnType.INTEGER, None, None),
+        ColumnDefinition(PDFColumnName.paragraph.name, ColumnType.INTEGER, None, None),
+        ColumnDefinition(
+            PDFColumnName.data.name,
+            ColumnType.TEXT,
+            None,
+            None,
+        ),
+    ]
+    return columns
+
+
 def get_table_primary_columns(table_catalog_obj: TableCatalogEntry):
     if table_catalog_obj.table_type == TableType.VIDEO_DATA:
         return get_video_table_column_definitions()[:2]
     elif table_catalog_obj.table_type == TableType.IMAGE_DATA:
         return get_image_table_column_definitions()[:1]
+    elif table_catalog_obj.table_type == TableType.DOCUMENT_DATA:
+        return get_document_table_column_definitions()[:1]
+    elif table_catalog_obj.table_type == TableType.PDF_DATA:
+        return get_pdf_table_column_definitions()[:3]
     else:
         raise Exception(f"Unexpected table type {table_catalog_obj.table_type}")
 
 
 def xform_column_definitions_to_catalog_entries(
     col_list: List[ColumnDefinition],
 ) -> List[ColumnCatalogEntry]:
```

### Comparing `evadb-0.2.4/eva/catalog/models/__init__.py` & `evadb-0.2.5/eva/catalog/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/models/association_models.py` & `evadb-0.2.5/eva/catalog/models/association_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/models/base_model.py` & `evadb-0.2.5/eva/catalog/models/base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/models/column_catalog.py` & `evadb-0.2.5/eva/catalog/models/column_catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/models/index_catalog.py` & `evadb-0.2.5/eva/catalog/models/index_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/models/table_catalog.py` & `evadb-0.2.5/eva/catalog/models/table_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/models/udf_cache_catalog.py` & `evadb-0.2.5/eva/catalog/models/udf_cache_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/models/udf_catalog.py` & `evadb-0.2.5/eva/catalog/models/udf_catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/models/udf_cost_catalog.py` & `evadb-0.2.5/eva/catalog/models/udf_cost_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/models/udf_io_catalog.py` & `evadb-0.2.5/eva/catalog/models/udf_io_catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/models/udf_metadata_catalog.py` & `evadb-0.2.5/eva/catalog/models/udf_metadata_catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/schema_utils.py` & `evadb-0.2.5/eva/catalog/schema_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/services/__init__.py` & `evadb-0.2.5/test/benchmark_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/eva/catalog/services/base_service.py` & `evadb-0.2.5/eva/catalog/services/base_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/services/column_catalog_service.py` & `evadb-0.2.5/eva/catalog/services/column_catalog_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/services/index_catalog_service.py` & `evadb-0.2.5/eva/catalog/services/index_catalog_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/services/table_catalog_service.py` & `evadb-0.2.5/eva/catalog/services/table_catalog_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/services/udf_cache_catalog_service.py` & `evadb-0.2.5/eva/catalog/services/udf_cache_catalog_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/services/udf_catalog_service.py` & `evadb-0.2.5/eva/catalog/services/udf_catalog_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/services/udf_cost_catalog_service.py` & `evadb-0.2.5/eva/catalog/services/udf_cost_catalog_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/services/udf_io_catalog_service.py` & `evadb-0.2.5/eva/catalog/services/udf_io_catalog_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/services/udf_metadata_catalog_service.py` & `evadb-0.2.5/eva/catalog/services/udf_metadata_catalog_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/catalog/sql_config.py` & `evadb-0.2.5/eva/catalog/sql_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import os
-
 from sqlalchemy import create_engine, event
 from sqlalchemy.orm import scoped_session, sessionmaker
 
 from eva.configuration.configuration_manager import ConfigurationManager
 
 IDENTIFIER_COLUMN = "_row_id"
 
@@ -58,26 +56,15 @@
     def __init__(self):
         """Initializes the engine and session for database operations
 
         Retrieves the database uri for connection from ConfigurationManager.
         """
         uri = ConfigurationManager().get_value("core", "catalog_database_uri")
 
-        # to parallelize tests using pytest-xdist
-        def prefix_worker_id_to_uri(uri: str):
-            try:
-                worker_id = os.environ["PYTEST_XDIST_WORKER"]
-                base = "eva_catalog.db"
-                # eva_catalog.db -> test_gw1_eva_catalog.db
-                uri = uri.replace(base, "test_" + str(worker_id) + "_" + base)
-            except KeyError:
-                pass
-            return uri
-
-        self.worker_uri = prefix_worker_id_to_uri(str(uri))
+        self.worker_uri = str(uri)
         # set echo=True to log SQL
         self.engine = create_engine(self.worker_uri, isolation_level="SERIALIZABLE")
 
         if self.engine.url.get_backend_name() == "sqlite":
             # enforce foreign key constraint and wal logging for sqlite
             # https://docs.sqlalchemy.org/en/20/dialects/sqlite.html#foreign-key-support
```

### Comparing `evadb-0.2.4/eva/configuration/__init__.py` & `evadb-0.2.5/eva/configuration/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/configuration/constants.py` & `evadb-0.2.5/eva/configuration/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,26 +11,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from pathlib import Path
 
 import eva
-from eva.version import VERSION
 
 EVA_INSTALLATION_DIR = Path(eva.__file__).parent
 EVA_ROOT_DIR = Path(eva.__file__).parent.parent
-# Using eva version to govern the EVA_DEFAULT_DIR
-# This means we won't support backward compatibility as each version will maintain its own copy of database.
-# Ideally, if the new release is not breaking backward compatibility, we can keep using the same copy.
-# We can revisit it later
-EVA_DEFAULT_DIR = Path.home() / ".eva" / str(VERSION)
+EVA_DATABASE_DIR = "eva_data"
 EVA_DATASET_DIR = "eva_datasets"
 EVA_CONFIG_FILE = "eva.yml"
 UDF_DIR = "udfs"
 CATALOG_DIR = "catalog"
 INDEX_DIR = "index"
 CACHE_DIR = "cache"
 DATASET_DATAFRAME_NAME = "dataset"
-DB_DEFAULT_URI = "sqlite:///{}/eva_catalog.db".format(EVA_DEFAULT_DIR.resolve())
+DB_DEFAULT_NAME = "eva.db"
 S3_DOWNLOAD_DIR = "s3_downloads"
 TMP_DIR = "tmp"
```

### Comparing `evadb-0.2.4/eva/constants.py` & `evadb-0.2.5/eva/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/eva.yml` & `evadb-0.2.5/eva/eva.yml`

 * *Files 16% similar despite different names*

```diff
@@ -35,16 +35,20 @@
 00000220: 2e73 746f 7261 6765 2e76 6964 656f 5f73  .storage.video_s
 00000230: 746f 7261 6765 5f65 6e67 696e 652e 4465  torage_engine.De
 00000240: 636f 7264 5374 6f72 6167 6545 6e67 696e  cordStorageEngin
 00000250: 6522 0a20 2069 6d61 6765 5f65 6e67 696e  e".  image_engin
 00000260: 653a 2022 6576 612e 7374 6f72 6167 652e  e: "eva.storage.
 00000270: 696d 6167 655f 7374 6f72 6167 655f 656e  image_storage_en
 00000280: 6769 6e65 2e49 6d61 6765 5374 6f72 6167  gine.ImageStorag
-00000290: 6545 6e67 696e 6522 0a73 6572 7665 723a  eEngine".server:
-000002a0: 0a20 2068 6f73 743a 2022 302e 302e 302e  .  host: "0.0.0.
-000002b0: 3022 0a20 2070 6f72 743a 2038 3830 330a  0".  port: 8803.
-000002c0: 2020 736f 636b 6574 5f74 696d 656f 7574    socket_timeout
-000002d0: 3a20 3630 0a0a 6578 7065 7269 6d65 6e74  : 60..experiment
-000002e0: 616c 3a0a 2020 7261 793a 2046 616c 7365  al:.  ray: False
-000002f0: 0a0a 7468 6972 645f 7061 7274 793a 0a20  ..third_party:. 
-00000300: 206f 7065 6e61 695f 6170 695f 6b65 793a   openai_api_key:
-00000310: 2022 22                                   ""
+00000290: 6545 6e67 696e 6522 0a20 2070 6466 5f65  eEngine".  pdf_e
+000002a0: 6e67 696e 653a 2022 6576 612e 7374 6f72  ngine: "eva.stor
+000002b0: 6167 652e 7064 665f 7374 6f72 6167 655f  age.pdf_storage_
+000002c0: 656e 6769 6e65 2e50 4446 5374 6f72 6167  engine.PDFStorag
+000002d0: 6545 6e67 696e 6522 0a0a 7365 7276 6572  eEngine"..server
+000002e0: 3a0a 2020 686f 7374 3a20 2230 2e30 2e30  :.  host: "0.0.0
+000002f0: 2e30 220a 2020 706f 7274 3a20 3838 3033  .0".  port: 8803
+00000300: 0a20 2073 6f63 6b65 745f 7469 6d65 6f75  .  socket_timeou
+00000310: 743a 2036 300a 0a65 7870 6572 696d 656e  t: 60..experimen
+00000320: 7461 6c3a 0a20 2072 6179 3a20 5472 7565  tal:.  ray: True
+00000330: 0a0a 7468 6972 645f 7061 7274 793a 0a20  ..third_party:. 
+00000340: 206f 7065 6e61 695f 6170 695f 6b65 793a   openai_api_key:
+00000350: 2022 220a                                 "".
```

### Comparing `evadb-0.2.4/eva/eva_cmd_client.py` & `evadb-0.2.5/eva/eva_cmd_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/eva_server.py` & `evadb-0.2.5/eva/eva_server.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -24,16 +24,17 @@
 To allow running eva_server from any location
 """
 THIS_DIR = dirname(__file__)
 EVA_CODE_DIR = abspath(join(THIS_DIR, ".."))
 sys.path.append(EVA_CODE_DIR)
 
 from eva.configuration.configuration_manager import ConfigurationManager  # noqa: E402
+from eva.configuration.constants import EVA_DATABASE_DIR  # noqa: E402
 from eva.server.server import EvaServer  # noqa: E402
-from eva.udfs.udf_bootstrap_queries import init_builtin_udfs  # noqa: E402
+from eva.utils.logging_manager import logger  # noqa: E402
 
 
 async def start_eva_server(host: str, port: int):
     """Start the eva server"""
     eva_server = EvaServer()
 
     await eva_server.start_eva_server(host, port)
@@ -60,14 +61,18 @@
 
     parser.add_argument(
         "--port",
         help="Specify the port number on which the server will start.",
     )
 
     parser.add_argument(
+        "--database", help="Specify the database folder which the server should access."
+    )
+
+    parser.add_argument(
         "--start",
         help="start server",
         action="store_true",
         default=True,
     )
 
     parser.add_argument(
@@ -80,25 +85,31 @@
     ## PARSE ARGS
     args, unknown = parser.parse_known_args()
 
     # Stop server
     if args.stop:
         return stop_server()
 
-    host = (
-        args.host if args.host else ConfigurationManager().get_value("server", "host")
-    )
+    eva_db_dir = args.database if args.database else EVA_DATABASE_DIR
 
-    port = (
-        args.port if args.port else ConfigurationManager().get_value("server", "port")
-    )
+    logger.debug(f"Database dir: {eva_db_dir}")
+
+    # Instantiate a Configuration Manager object with the appropriate database directory
+    # Subsequent calls will utilize the specified database directory
+    config_manager = ConfigurationManager(EVA_DATABASE_DIR=eva_db_dir)
+
+    host = args.host if args.host else config_manager.get_value("server", "host")
+
+    port = args.port if args.port else config_manager.get_value("server", "port")
 
     # Start server
     if args.start:
-        mode = ConfigurationManager().get_value("core", "mode")
+        mode = config_manager.get_value("core", "mode")
+        from eva.udfs.udf_bootstrap_queries import init_builtin_udfs  # noqa: E402
+
         init_builtin_udfs(mode=mode)
 
         asyncio.run(start_eva_server(host=host, port=int(port)))
 
 
 if __name__ == "__main__":
     # execute only if run as the entry point into the program
```

### Comparing `evadb-0.2.4/eva/executor/__init__.py` & `evadb-0.2.5/eva/executor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/abstract_executor.py` & `evadb-0.2.5/eva/executor/abstract_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/apply_and_merge_executor.py` & `evadb-0.2.5/eva/executor/apply_and_merge_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/create_executor.py` & `evadb-0.2.5/eva/executor/create_executor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -24,12 +24,26 @@
     def __init__(self, node: CreatePlan):
         super().__init__(node)
         self.catalog = CatalogManager()
 
     def exec(self, *args, **kwargs):
         if not handle_if_not_exists(self.node.table_info, self.node.if_not_exists):
             logger.debug(f"Creating table {self.node.table_info}")
+
             catalog_entry = self.catalog.create_and_insert_table_catalog_entry(
                 self.node.table_info, self.node.column_list
             )
             storage_engine = StorageEngine.factory(catalog_entry)
             storage_engine.create(table=catalog_entry)
+
+            if self.children != []:
+                assert (
+                    len(self.children) == 1
+                ), "Create materialized view expects 1 child, finds {}".format(
+                    len(self.children)
+                )
+                child = self.children[0]
+
+                # Populate the table
+                for batch in child.exec():
+                    batch.drop_column_alias()
+                    storage_engine.write(catalog_entry, batch)
```

### Comparing `evadb-0.2.4/eva/executor/create_index_executor.py` & `evadb-0.2.5/eva/executor/create_index_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/create_udf_executor.py` & `evadb-0.2.5/eva/executor/create_udf_executor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,80 +1,70 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import os
 from pathlib import Path
 from typing import Dict, List
 
 import pandas as pd
 
 from eva.catalog.catalog_manager import CatalogManager
 from eva.catalog.catalog_utils import get_metadata_properties
 from eva.catalog.models.udf_catalog import UdfCatalogEntry
 from eva.catalog.models.udf_io_catalog import UdfIOCatalogEntry
-from eva.configuration.constants import EVA_DEFAULT_DIR
+from eva.configuration.configuration_manager import ConfigurationManager
 from eva.executor.abstract_executor import AbstractExecutor
 from eva.models.storage.batch import Batch
 from eva.plan_nodes.create_udf_plan import CreateUDFPlan
 from eva.third_party.huggingface.create import gen_hf_io_catalog_entries
 from eva.udfs.decorators.utils import load_io_from_udf_decorators
 from eva.utils.errors import UDFIODefinitionError
 from eva.utils.generic_utils import load_udf_class_from_file
 from eva.utils.logging_manager import logger
 
 
 class CreateUDFExecutor(AbstractExecutor):
     def __init__(self, node: CreateUDFPlan):
         super().__init__(node)
+        self.udf_dir = (
+            Path(ConfigurationManager().get_value("core", "eva_installation_dir"))
+            / "udfs"
+        )
 
     def handle_huggingface_udf(self):
         """Handle HuggingFace UDFs
 
         HuggingFace UDFs are special UDFs that are not loaded from a file.
         So we do not need to call the setup method on them like we do for other UDFs.
         """
-        impl_path = f"{EVA_DEFAULT_DIR}/udfs/abstract/hf_abstract_udf.py"
+        impl_path = f"{self.udf_dir}/abstract/hf_abstract_udf.py"
         io_list = gen_hf_io_catalog_entries(self.node.name, self.node.metadata)
         return (
             self.node.name,
             impl_path,
             self.node.udf_type,
             io_list,
             self.node.metadata,
         )
 
-    def suffix_pytest_xdist_worker_id_to_dir(self, path: Path):
-        try:
-            worker_id = os.environ["PYTEST_XDIST_WORKER"]
-            path = path / str(worker_id)
-        except KeyError:
-            pass
-        return path
-
     def handle_ultralytics_udf(self):
         """Handle Ultralytics UDFs"""
-        initial_eva_config_dir = Path(EVA_DEFAULT_DIR)
-        updated_eva_config_dir = self.suffix_pytest_xdist_worker_id_to_dir(
-            initial_eva_config_dir
-        )
+
         impl_path = (
-            Path(f"{updated_eva_config_dir}/udfs/yolo_object_detector.py")
-            .absolute()
-            .as_posix()
+            Path(f"{self.udf_dir}/yolo_object_detector.py").absolute().as_posix()
         )
         udf = self._try_initializing_udf(
             impl_path, udf_args=get_metadata_properties(self.node)
         )
         io_list = self._resolve_udf_io(udf)
         return (
             self.node.name,
@@ -107,15 +97,14 @@
         Calls the catalog to insert a udf catalog entry.
         """
         catalog_manager = CatalogManager()
         # check catalog if it already has this udf entry
         if catalog_manager.get_udf_catalog_entry_by_name(self.node.name):
             if self.node.if_not_exists:
                 msg = f"UDF {self.node.name} already exists, nothing added."
-                logger.warn(msg)
                 yield Batch(pd.DataFrame([msg]))
                 return
             else:
                 msg = f"UDF {self.node.name} already exists."
                 logger.error(msg)
                 raise RuntimeError(msg)
```

### Comparing `evadb-0.2.4/eva/executor/delete_executor.py` & `evadb-0.2.5/eva/executor/delete_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/drop_executor.py` & `evadb-0.2.5/eva/executor/drop_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -42,15 +42,14 @@
             table_info.table_name, table_info.database_name
         ):
             err_msg = "Table: {} does not exist".format(table_info)
             if self.node.if_exists:
                 logger.warn(err_msg)
                 return Batch(pd.DataFrame([err_msg]))
             else:
-                logger.exception(err_msg)
                 raise ExecutorError(err_msg)
 
         table_obj = catalog_manager.get_table_catalog_entry(
             table_info.table_name, table_info.database_name
         )
         storage_engine = StorageEngine.factory(table_obj)
```

### Comparing `evadb-0.2.4/eva/executor/drop_udf_executor.py` & `evadb-0.2.5/eva/executor/drop_udf_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -35,15 +35,14 @@
         if not catalog_manager.get_udf_catalog_entry_by_name(self.node.name):
             err_msg = (
                 f"UDF {self.node.name} does not exist, therefore cannot be dropped."
             )
             if self.node.if_exists:
                 logger.warn(err_msg)
             else:
-                logger.exception(err_msg)
                 raise RuntimeError(err_msg)
         else:
             udf_entry = catalog_manager.get_udf_catalog_entry_by_name(self.node.name)
             for cache in udf_entry.dep_caches:
                 catalog_manager.drop_udf_cache_catalog_entry(cache)
             catalog_manager.delete_udf_catalog_entry_by_name(self.node.name)
             yield Batch(
```

### Comparing `evadb-0.2.4/eva/executor/execution_context.py` & `evadb-0.2.5/eva/executor/execution_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/executor_utils.py` & `evadb-0.2.5/eva/executor/executor_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,14 +21,15 @@
 
 from eva.catalog.catalog_manager import CatalogManager
 from eva.catalog.catalog_type import VectorStoreType
 from eva.expression.abstract_expression import AbstractExpression
 from eva.models.storage.batch import Batch
 from eva.parser.table_ref import TableInfo
 from eva.parser.types import FileFormatType
+from eva.readers.document.registry import SUPPORTED_TYPES
 from eva.utils.logging_manager import logger
 
 
 class ExecutorError(Exception):
     pass
 
 
@@ -87,19 +88,31 @@
         return True
     except Exception as e:
         logger.warning(
             f"Unexpected Exception {e} occurred while reading video file {video_path}"
         )
 
 
+def validate_document(doc_path: Path) -> bool:
+    return doc_path.suffix in SUPPORTED_TYPES
+
+
+def validate_pdf(doc_path: Path) -> bool:
+    return doc_path.suffix == ".pdf"
+
+
 def validate_media(file_path: Path, media_type: FileFormatType) -> bool:
     if media_type == FileFormatType.VIDEO:
         return validate_video(file_path)
     elif media_type == FileFormatType.IMAGE:
         return validate_image(file_path)
+    elif media_type == FileFormatType.DOCUMENT:
+        return validate_document(file_path)
+    elif media_type == FileFormatType.PDF:
+        return validate_pdf(file_path)
     else:
         raise ValueError(f"Unsupported Media type {str(media_type)}")
 
 
 def handle_vector_store_params(
     vector_store_type: VectorStoreType, index_path: str
 ) -> dict:
```

### Comparing `evadb-0.2.4/eva/executor/explain_executor.py` & `evadb-0.2.5/eva/executor/explain_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/function_scan_executor.py` & `evadb-0.2.5/eva/executor/function_scan_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/groupby_executor.py` & `evadb-0.2.5/eva/executor/groupby_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/hash_join_executor.py` & `evadb-0.2.5/eva/executor/hash_join_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/insert_executor.py` & `evadb-0.2.5/eva/executor/insert_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/join_build_executor.py` & `evadb-0.2.5/eva/executor/join_build_executor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/lateral_join_executor.py` & `evadb-0.2.5/eva/executor/lateral_join_executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/limit_executor.py` & `evadb-0.2.5/eva/executor/limit_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/load_csv_executor.py` & `evadb-0.2.5/eva/executor/load_csv_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/load_executor.py` & `evadb-0.2.5/eva/executor/load_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -28,14 +28,16 @@
         Use TYPE to determine the type of data to load.
         """
 
         # invoke the appropriate executor
         if self.node.file_options["file_format"] in [
             FileFormatType.VIDEO,
             FileFormatType.IMAGE,
+            FileFormatType.DOCUMENT,
+            FileFormatType.PDF,
         ]:
             executor = LoadMultimediaExecutor(self.node)
         elif self.node.file_options["file_format"] == FileFormatType.CSV:
             executor = LoadCSVExecutor(self.node)
 
         # for each batch, exec the executor
         for batch in executor.exec():
```

### Comparing `evadb-0.2.4/eva/executor/load_multimedia_executor.py` & `evadb-0.2.5/eva/executor/load_multimedia_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/nested_loop_join_executor.py` & `evadb-0.2.5/eva/executor/nested_loop_join_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/orderby_executor.py` & `evadb-0.2.5/eva/executor/orderby_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/plan_executor.py` & `evadb-0.2.5/eva/executor/plan_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -19,14 +19,15 @@
 from eva.executor.create_executor import CreateExecutor
 from eva.executor.create_index_executor import CreateIndexExecutor
 from eva.executor.create_mat_view_executor import CreateMaterializedViewExecutor
 from eva.executor.create_udf_executor import CreateUDFExecutor
 from eva.executor.delete_executor import DeleteExecutor
 from eva.executor.drop_executor import DropExecutor
 from eva.executor.drop_udf_executor import DropUDFExecutor
+from eva.executor.exchange_executor import ExchangeExecutor
 from eva.executor.executor_utils import ExecutorError
 from eva.executor.explain_executor import ExplainExecutor
 from eva.executor.function_scan_executor import FunctionScanExecutor
 from eva.executor.groupby_executor import GroupByExecutor
 from eva.executor.hash_join_executor import HashJoinExecutor
 from eva.executor.insert_executor import InsertExecutor
 from eva.executor.join_build_executor import BuildJoinExecutor
@@ -41,15 +42,14 @@
 from eva.executor.rename_executor import RenameExecutor
 from eva.executor.sample_executor import SampleExecutor
 from eva.executor.seq_scan_executor import SequentialScanExecutor
 from eva.executor.show_info_executor import ShowInfoExecutor
 from eva.executor.storage_executor import StorageExecutor
 from eva.executor.union_executor import UnionExecutor
 from eva.executor.vector_index_scan_executor import VectorIndexScanExecutor
-from eva.experimental.ray.executor.exchange_executor import ExchangeExecutor
 from eva.models.storage.batch import Batch
 from eva.plan_nodes.abstract_plan import AbstractPlan
 from eva.plan_nodes.types import PlanOprType
 from eva.utils.logging_manager import logger
 
 
 class PlanExecutor:
@@ -125,14 +125,16 @@
             executor_node = BuildJoinExecutor(node=plan)
         elif plan_opr_type == PlanOprType.FUNCTION_SCAN:
             executor_node = FunctionScanExecutor(node=plan)
         elif plan_opr_type == PlanOprType.CREATE_MATERIALIZED_VIEW:
             executor_node = CreateMaterializedViewExecutor(node=plan)
         elif plan_opr_type == PlanOprType.EXCHANGE:
             executor_node = ExchangeExecutor(node=plan)
+            inner_executor = self._build_execution_tree(plan.inner_plan)
+            executor_node.build_inner_executor(inner_executor)
         elif plan_opr_type == PlanOprType.PROJECT:
             executor_node = ProjectExecutor(node=plan)
         elif plan_opr_type == PlanOprType.PREDICATE_FILTER:
             executor_node = PredicateExecutor(node=plan)
         elif plan_opr_type == PlanOprType.SHOW_INFO:
             executor_node = ShowInfoExecutor(node=plan)
         elif plan_opr_type == PlanOprType.EXPLAIN:
@@ -168,9 +170,9 @@
         try:
             execution_tree = self._build_execution_tree(self._plan)
             output = execution_tree.exec()
             if output is not None:
                 yield from output
             self._clean_execution_tree(execution_tree)
         except Exception as e:
-            logger.error(str(e))
+            logger.exception(str(e))
             raise ExecutorError(e)
```

### Comparing `evadb-0.2.4/eva/executor/pp_executor.py` & `evadb-0.2.5/eva/executor/pp_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/predicate_executor.py` & `evadb-0.2.5/eva/executor/predicate_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/project_executor.py` & `evadb-0.2.5/eva/executor/project_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/rename_executor.py` & `evadb-0.2.5/eva/executor/rename_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/sample_executor.py` & `evadb-0.2.5/eva/executor/sample_executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/seq_scan_executor.py` & `evadb-0.2.5/eva/executor/seq_scan_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/show_info_executor.py` & `evadb-0.2.5/eva/executor/show_info_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/storage_executor.py` & `evadb-0.2.5/eva/executor/storage_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -39,16 +39,20 @@
                     sampling_rate=self.node.sampling_rate,
                     sampling_type=self.node.sampling_type,
                     read_audio=self.node.table_ref.get_audio,
                     read_video=self.node.table_ref.get_video,
                 )
             elif self.node.table.table_type == TableType.IMAGE_DATA:
                 return storage_engine.read(self.node.table)
+            elif self.node.table.table_type == TableType.DOCUMENT_DATA:
+                return storage_engine.read(self.node.table)
             elif self.node.table.table_type == TableType.STRUCTURED_DATA:
                 return storage_engine.read(self.node.table, self.node.batch_mem_size)
+            elif self.node.table.table_type == TableType.PDF_DATA:
+                return storage_engine.read(self.node.table)
             else:
                 raise ExecutorError(
                     f"Unsupported TableType  {self.node.table.table_type} encountered"
                 )
         except Exception as e:
             logger.error(e)
             raise ExecutorError(e)
```

### Comparing `evadb-0.2.4/eva/executor/union_executor.py` & `evadb-0.2.5/eva/executor/union_executor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/executor/vector_index_scan_executor.py` & `evadb-0.2.5/eva/executor/vector_index_scan_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/experimental/__init__.py` & `evadb-0.2.5/eva/catalog/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""experimental subdirectory"""
+"""
+catalog subdirectory
+"""
```

### Comparing `evadb-0.2.4/eva/experimental/ray/__init__.py` & `evadb-0.2.5/eva/expression/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""ray subdirectory"""
+"""expression subdirectory"""
```

### Comparing `evadb-0.2.4/eva/experimental/ray/executor/__init__.py` & `evadb-0.2.5/eva/plan_nodes/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""ray executor subdirectory"""
+"""planner subdirectory"""
```

### Comparing `evadb-0.2.4/eva/experimental/ray/executor/exchange_executor.py` & `evadb-0.2.5/eva/executor/exchange_executor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,92 +14,89 @@
 # limitations under the License.
 from typing import Iterator
 
 from ray.util.queue import Queue
 
 from eva.executor.abstract_executor import AbstractExecutor
 from eva.executor.executor_utils import ExecutorError
-from eva.experimental.ray.executor.ray_stage import (
+from eva.executor.ray_utils import (
     StageCompleteSignal,
-    ray_stage,
-    ray_stage_wait_and_alert,
+    ray_parallel,
+    ray_pull,
+    ray_wait_and_alert,
 )
-from eva.experimental.ray.planner.exchange_plan import ExchangePlan
 from eva.models.storage.batch import Batch
+from eva.plan_nodes.exchange_plan import ExchangePlan
 
 
 class QueueReaderExecutor(AbstractExecutor):
     def __init__(self):
         super().__init__(None)
 
     def exec(self, **kwargs) -> Iterator[Batch]:
-        assert (
-            "input_queues" in kwargs
-        ), "Invalid Ray execution stage. No input_queue found"
-        input_queues = kwargs["input_queues"]
-        assert len(input_queues) == 1, "Not support multiple input queues yet"
-        iq = input_queues[0]
+        assert "input_queue" in kwargs, "Invalid ray execution. No input_queue found"
+        input_queue = kwargs["input_queue"]
 
         while True:
-            next_item = iq.get(block=True)
+            next_item = input_queue.get(block=True)
             if next_item is StageCompleteSignal:
-                iq.put(StageCompleteSignal)
+                # Stop signal is put back to input queue again
+                # to ensure it is propagated to all ray parallel
+                # actors.
+                input_queue.put(StageCompleteSignal)
                 break
             elif isinstance(next_item, ExecutorError):
-                iq.put(next_item)
+                input_queue.put(next_item)
                 raise next_item
             else:
                 yield next_item
 
 
 class ExchangeExecutor(AbstractExecutor):
-    """
-    Applies predicates to filter the frames which satisfy the condition
-    Arguments:
-        node (AbstractPlan): The SequentialScanPlan
-
-    """
-
     def __init__(self, node: ExchangePlan):
+        self.inner_plan = node.inner_plan
         self.parallelism = node.parallelism
-        self.ray_conf = node.ray_conf
+        self.ray_pull_env_conf_dict = node.ray_pull_env_conf_dict
+        self.ray_parallel_env_conf_dict = node.ray_parallel_env_conf_dict
         super().__init__(node)
 
-    def exec(self, is_top=True) -> Iterator[Batch]:
-        assert (
-            len(self.children) == 1
-        ), "Exchange executor does not support children != 1"
-
-        # Find the exchange executor below the tree
-        curr_exec = self
-        input_queues = []
-        while len(curr_exec.children) > 0 and not isinstance(
-            curr_exec.children[0], ExchangeExecutor
-        ):
-            curr_exec = curr_exec.children[0]
-
-        if len(curr_exec.children) > 0:
-            iq = yield from curr_exec.children[0].exec(is_top=False)
-            input_queues.append(iq)
-            queue_exec = QueueReaderExecutor()
-            curr_exec.children = [queue_exec]
-            # curr_exec.append_child(queue_exec)
+    def build_inner_executor(self, inner_executor):
+        self.inner_executor = inner_executor
+        self.inner_executor.children = [QueueReaderExecutor()]
 
+    def exec(self) -> Iterator[Batch]:
+        input_queue = Queue(maxsize=100)
         output_queue = Queue(maxsize=100)
-        ray_task = []
-        for _ in range(self.parallelism):
-            ray_task.append(
-                ray_stage.options(**self.ray_conf).remote(
-                    self.children[0], input_queues, [output_queue]
+
+        # Pull data from child executor
+        assert (
+            len(self.children) == 1
+        ), "Exchange currently only supports parallelization of node with only one child"
+        ray_pull_task = ray_pull.remote(
+            self.ray_pull_env_conf_dict,
+            self.children[0],
+            input_queue,
+        )
+
+        # Parallel the inner executor.
+        ray_parallel_task_list = []
+        for i in range(self.parallelism):
+            ray_parallel_task_list.append(
+                ray_parallel.remote(
+                    self.ray_parallel_env_conf_dict[i],
+                    self.inner_executor,
+                    input_queue,
+                    output_queue,
                 )
             )
-        ray_stage_wait_and_alert.remote(ray_task, [output_queue])
-        while is_top:
+
+        ray_wait_and_alert.remote([ray_pull_task], input_queue)
+        ray_wait_and_alert.remote(ray_parallel_task_list, output_queue)
+
+        while True:
             res = output_queue.get(block=True)
             if res is StageCompleteSignal:
                 break
             elif isinstance(res, ExecutorError):
                 raise res
             else:
                 yield res
-        else:
-            return output_queue
```

### Comparing `evadb-0.2.4/eva/experimental/ray/optimizer/__init__.py` & `evadb-0.2.5/eva/third_party/vector_stores/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""ray optimizer subdirectory"""
+"""vector stores"""
```

### Comparing `evadb-0.2.4/eva/experimental/ray/optimizer/rules/__init__.py` & `evadb-0.2.5/eva/server/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""ray optimizer rules subdirectory"""
+"""sets up a local-hosted server"""
```

### Comparing `evadb-0.2.4/eva/experimental/ray/planner/__init__.py` & `evadb-0.2.5/eva/binder/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""ray planner subdirectory"""
```

### Comparing `evadb-0.2.4/eva/experimental/ray/planner/exchange_plan.py` & `evadb-0.2.5/eva/plan_nodes/union_plan.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from typing import Any, Dict
-
 from eva.plan_nodes.abstract_plan import AbstractPlan
 from eva.plan_nodes.types import PlanOprType
 
 
-class ExchangePlan(AbstractPlan):
+class UnionPlan(AbstractPlan):
     """
     This plan is used for storing information required for union operations.
 
     Arguments:
         all: Bool
             UNION (deduplication) vs UNION ALL (non-deduplication)
     """
 
-    def __init__(
-        self, parallelism: int = 1, ray_conf: Dict[str, Any] = {"num_cpus": 1}
-    ):
-        self.parallelism = parallelism
-        self.ray_conf = ray_conf
-        super().__init__(PlanOprType.EXCHANGE)
+    def __init__(self, all: bool):
+        self._all = all
+        super().__init__(PlanOprType.UNION)
+
+    @property
+    def all(self):
+        return self._all
 
-    def __str__(self) -> str:
-        return "ExchangePlan"
+    def __str__(self):
+        return "UnionAllPlan" if self._all else "UnionPlan"
 
     def __hash__(self) -> int:
-        return hash(
-            (super().__hash__(), self.parallelism, frozenset(self.ray_conf.items()))
-        )
+        return hash((super().__hash__(), self._all))
```

### Comparing `evadb-0.2.4/eva/expression/__init__.py` & `evadb-0.2.5/eva/catalog/services/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""expression subdirectory"""
```

### Comparing `evadb-0.2.4/eva/expression/abstract_expression.py` & `evadb-0.2.5/eva/expression/abstract_expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/expression/aggregation_expression.py` & `evadb-0.2.5/eva/expression/aggregation_expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -62,15 +62,14 @@
             updated_column_name = column_name.replace("AGGREGATION_", "")
             batch.modify_column_alias(updated_column_name)
 
         # TODO: Raise exception if data type doesn't match
         return batch
 
     def get_symbol(self) -> str:
-
         if self.etype == ExpressionType.AGGREGATION_FIRST:
             return "FIRST"
         if self.etype == ExpressionType.AGGREGATION_LAST:
             return "LAST"
         if self.etype == ExpressionType.AGGREGATION_SEGMENT:
             return "SEGMENT"
         if self.etype == ExpressionType.AGGREGATION_SUM:
```

### Comparing `evadb-0.2.4/eva/expression/arithmetic_expression.py` & `evadb-0.2.5/eva/expression/arithmetic_expression.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/expression/comparison_expression.py` & `evadb-0.2.5/eva/expression/comparison_expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/expression/constant_value_expression.py` & `evadb-0.2.5/eva/expression/constant_value_expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/expression/expression_utils.py` & `evadb-0.2.5/eva/expression/expression_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/expression/function_expression.py` & `evadb-0.2.5/eva/expression/function_expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -129,16 +129,19 @@
     def evaluate(self, batch: Batch, **kwargs) -> Batch:
         func = self._gpu_enabled_function()
         # record the time taken for the udf execution
         # note the udf might be using cache
         with self._stats.timer:
             # apply the function and project the required columns
             outcomes = self._apply_function_expression(func, batch, **kwargs)
-            outcomes = outcomes.project(self.projection_columns)
-            outcomes.modify_column_alias(self.alias)
+
+            # process outcomes only if output is not empty
+            if outcomes.frames.empty is False:
+                outcomes = outcomes.project(self.projection_columns)
+                outcomes.modify_column_alias(self.alias)
 
         # record the number of function calls
         self._stats.num_calls += len(batch)
 
         # try persisting the stats to catalog and do not crash if we fail in doing so
         try:
             self.persist_stats()
@@ -231,15 +234,16 @@
             # 4. merge the cache results
             results[cache_miss] = cache_miss_results.to_numpy()
 
         # 5. return the correct batch
         return Batch(pd.DataFrame(results, columns=output_cols))
 
     def __str__(self) -> str:
-        expr_str = f"{self.name}()"
+        args = [str(child) for child in self.children]
+        expr_str = f"{self.name}({','.join(args)})"
         return expr_str
 
     def __eq__(self, other):
         is_subtree_equal = super().__eq__(other)
         if not isinstance(other, FunctionExpression):
             return False
         return (
```

### Comparing `evadb-0.2.4/eva/expression/logical_expression.py` & `evadb-0.2.5/eva/expression/logical_expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/expression/tuple_value_expression.py` & `evadb-0.2.5/eva/expression/tuple_value_expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/models/__init__.py` & `evadb-0.2.5/eva/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/models/catalog/__init__.py` & `evadb-0.2.5/test/binder/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/eva/models/catalog/frame_info.py` & `evadb-0.2.5/eva/models/catalog/frame_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/models/catalog/properties.py` & `evadb-0.2.5/eva/models/catalog/properties.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/models/server/__init__.py` & `evadb-0.2.5/test/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/eva/models/server/response.py` & `evadb-0.2.5/eva/models/server/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/models/storage/__init__.py` & `evadb-0.2.5/test/catalog/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/eva/models/storage/batch.py` & `evadb-0.2.5/eva/models/storage/batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/optimizer/__init__.py` & `evadb-0.2.5/eva/optimizer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/optimizer/binder.py` & `evadb-0.2.5/eva/optimizer/binder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/optimizer/cost_model.py` & `evadb-0.2.5/eva/optimizer/cost_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/optimizer/group.py` & `evadb-0.2.5/eva/optimizer/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/optimizer/group_expression.py` & `evadb-0.2.5/eva/optimizer/group_expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/optimizer/memo.py` & `evadb-0.2.5/eva/optimizer/memo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/optimizer/operators.py` & `evadb-0.2.5/eva/optimizer/operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/optimizer/optimizer_context.py` & `evadb-0.2.5/eva/optimizer/optimizer_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/optimizer/optimizer_task_stack.py` & `evadb-0.2.5/eva/optimizer/optimizer_task_stack.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/optimizer/optimizer_tasks.py` & `evadb-0.2.5/eva/optimizer/optimizer_tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/optimizer/optimizer_utils.py` & `evadb-0.2.5/eva/optimizer/optimizer_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/optimizer/property.py` & `evadb-0.2.5/eva/optimizer/property.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/optimizer/rules/__init__.py` & `evadb-0.2.5/test/catalog/services/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/eva/optimizer/rules/pattern.py` & `evadb-0.2.5/eva/optimizer/rules/pattern.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/optimizer/rules/rules.py` & `evadb-0.2.5/eva/optimizer/rules/rules.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,14 +16,15 @@
 
 from typing import TYPE_CHECKING
 
 from eva.catalog.catalog_manager import CatalogManager
 from eva.catalog.catalog_type import TableType
 from eva.catalog.catalog_utils import is_video_table
 from eva.constants import CACHEABLE_UDFS
+from eva.executor.execution_context import Context
 from eva.expression.expression_utils import (
     conjunction_list_to_expression_tree,
     to_conjunction_list,
 )
 from eva.expression.function_expression import FunctionExpression
 from eva.expression.tuple_value_expression import TupleValueExpression
 from eva.optimizer.optimizer_utils import (
@@ -36,14 +37,15 @@
     get_expression_execution_cost,
 )
 from eva.optimizer.rules.pattern import Pattern
 from eva.optimizer.rules.rules_base import Promise, Rule, RuleType
 from eva.parser.types import JoinType, ParserOrderBySortType
 from eva.plan_nodes.apply_and_merge_plan import ApplyAndMergePlan
 from eva.plan_nodes.create_mat_view_plan import CreateMaterializedViewPlan
+from eva.plan_nodes.exchange_plan import ExchangePlan
 from eva.plan_nodes.explain_plan import ExplainPlan
 from eva.plan_nodes.hash_join_build_plan import HashJoinBuildPlan
 from eva.plan_nodes.nested_loop_join_plan import NestedLoopJoinPlan
 from eva.plan_nodes.predicate_plan import PredicatePlan
 from eva.plan_nodes.project_plan import ProjectPlan
 from eva.plan_nodes.show_info_plan import ShowInfoPlan
 
@@ -56,14 +58,15 @@
     LogicalCreate,
     LogicalCreateIndex,
     LogicalCreateMaterializedView,
     LogicalCreateUDF,
     LogicalDelete,
     LogicalDrop,
     LogicalDropUDF,
+    LogicalExchange,
     LogicalExplain,
     LogicalExtractObject,
     LogicalFilter,
     LogicalFunctionScan,
     LogicalGet,
     LogicalGroupBy,
     LogicalInsert,
@@ -700,14 +703,33 @@
         return True
 
     def apply(self, before: LogicalCreate, context: OptimizerContext):
         after = CreatePlan(before.video, before.column_list, before.if_not_exists)
         yield after
 
 
+class LogicalCreateFromSelectToPhysical(Rule):
+    def __init__(self):
+        pattern = Pattern(OperatorType.LOGICALCREATE)
+        pattern.append_child(Pattern(OperatorType.DUMMY))
+        super().__init__(RuleType.LOGICAL_CREATE_FROM_SELECT_TO_PHYSICAL, pattern)
+
+    def promise(self):
+        return Promise.LOGICAL_CREATE_FROM_SELECT_TO_PHYSICAL
+
+    def check(self, before: Operator, context: OptimizerContext):
+        return True
+
+    def apply(self, before: LogicalCreate, context: OptimizerContext):
+        after = CreatePlan(before.video, before.column_list, before.if_not_exists)
+        for child in before.children:
+            after.append_child(child)
+        yield after
+
+
 class LogicalRenameToPhysical(Rule):
     def __init__(self):
         pattern = Pattern(OperatorType.LOGICALRENAME)
         super().__init__(RuleType.LOGICAL_RENAME_TO_PHYSICAL, pattern)
 
     def promise(self):
         return Promise.LOGICAL_RENAME_TO_PHYSICAL
@@ -1236,9 +1258,98 @@
             before.search_query_expr,
         )
         for child in before.children:
             after.append_child(child)
         yield after
 
 
+class LogicalExchangeToPhysical(Rule):
+    def __init__(self):
+        pattern = Pattern(OperatorType.LOGICALEXCHANGE)
+        pattern.append_child(Pattern(OperatorType.DUMMY))
+        super().__init__(RuleType.LOGICAL_EXCHANGE_TO_PHYSICAL, pattern)
+
+    def promise(self):
+        return Promise.LOGICAL_EXCHANGE_TO_PHYSICAL
+
+    def check(self, grp_id: int, context: OptimizerContext):
+        return True
+
+    def apply(self, before: LogicalExchange, context: OptimizerContext):
+        after = ExchangePlan(before.view)
+        for child in before.children:
+            after.append_child(child)
+        yield after
+
+
+class LogicalApplyAndMergeToRayPhysical(Rule):
+    def __init__(self):
+        pattern = Pattern(OperatorType.LOGICAL_APPLY_AND_MERGE)
+        pattern.append_child(Pattern(OperatorType.DUMMY))
+        super().__init__(RuleType.LOGICAL_APPLY_AND_MERGE_TO_PHYSICAL, pattern)
+
+    def promise(self):
+        return Promise.LOGICAL_APPLY_AND_MERGE_TO_PHYSICAL
+
+    def check(self, grp_id: int, context: OptimizerContext):
+        return True
+
+    def apply(self, before: LogicalApplyAndMerge, context: OptimizerContext):
+        apply_plan = ApplyAndMergePlan(before.func_expr, before.alias, before.do_unnest)
+
+        parallelism = 2 if len(Context().gpus) > 1 else 1
+        ray_parallel_env_conf_dict = [
+            {"CUDA_VISIBLE_DEVICES": str(i)} for i in range(parallelism)
+        ]
+
+        exchange_plan = ExchangePlan(
+            inner_plan=apply_plan,
+            parallelism=parallelism,
+            ray_pull_env_conf_dict={"CUDA_VISIBLE_DEVICES": "0"},
+            ray_parallel_env_conf_dict=ray_parallel_env_conf_dict,
+        )
+        for child in before.children:
+            exchange_plan.append_child(child)
+
+        yield exchange_plan
+
+
+class LogicalProjectToRayPhysical(Rule):
+    def __init__(self):
+        pattern = Pattern(OperatorType.LOGICALPROJECT)
+        pattern.append_child(Pattern(OperatorType.DUMMY))
+        super().__init__(RuleType.LOGICAL_PROJECT_TO_PHYSICAL, pattern)
+
+    def promise(self):
+        return Promise.LOGICAL_PROJECT_TO_PHYSICAL
+
+    def check(self, before: LogicalProject, context: OptimizerContext):
+        return True
+
+    def apply(self, before: LogicalProject, context: OptimizerContext):
+        project_plan = ProjectPlan(before.target_list)
+        # Check whether the projection contains a UDF
+        if before.target_list is None or not any(
+            [isinstance(expr, FunctionExpression) for expr in before.target_list]
+        ):
+            for child in before.children:
+                project_plan.append_child(child)
+            yield project_plan
+        else:
+            parallelism = 2 if len(Context().gpus) > 1 else 1
+            ray_parallel_env_conf_dict = [
+                {"CUDA_VISIBLE_DEVICES": str(i)} for i in range(parallelism)
+            ]
+
+            exchange_plan = ExchangePlan(
+                inner_plan=project_plan,
+                parallelism=parallelism,
+                ray_pull_env_conf_dict={"CUDA_VISIBLE_DEVICES": "0"},
+                ray_parallel_env_conf_dict=ray_parallel_env_conf_dict,
+            )
+            for child in before.children:
+                exchange_plan.append_child(child)
+            yield exchange_plan
+
+
 # IMPLEMENTATION RULES END
 ##############################################
```

### Comparing `evadb-0.2.4/eva/optimizer/rules/rules_base.py` & `evadb-0.2.5/eva/optimizer/rules/rules_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -60,14 +60,15 @@
     LOGICAL_GROUPBY_TO_PHYSICAL = auto()
     LOGICAL_ORDERBY_TO_PHYSICAL = auto()
     LOGICAL_LIMIT_TO_PHYSICAL = auto()
     LOGICAL_INSERT_TO_PHYSICAL = auto()
     LOGICAL_DELETE_TO_PHYSICAL = auto()
     LOGICAL_LOAD_TO_PHYSICAL = auto()
     LOGICAL_CREATE_TO_PHYSICAL = auto()
+    LOGICAL_CREATE_FROM_SELECT_TO_PHYSICAL = auto()
     LOGICAL_RENAME_TO_PHYSICAL = auto()
     LOGICAL_DROP_TO_PHYSICAL = auto()
     LOGICAL_CREATE_UDF_TO_PHYSICAL = auto()
     LOGICAL_MATERIALIZED_VIEW_TO_PHYSICAL = auto()
     LOGICAL_GET_TO_SEQSCAN = auto()
     LOGICAL_SAMPLE_TO_UNIFORMSAMPLE = auto()
     LOGICAL_DERIVED_GET_TO_PHYSICAL = auto()
@@ -104,14 +105,15 @@
     LOGICAL_LIMIT_TO_PHYSICAL = auto()
     LOGICAL_INSERT_TO_PHYSICAL = auto()
     LOGICAL_DELETE_TO_PHYSICAL = auto()
     LOGICAL_RENAME_TO_PHYSICAL = auto()
     LOGICAL_DROP_TO_PHYSICAL = auto()
     LOGICAL_LOAD_TO_PHYSICAL = auto()
     LOGICAL_CREATE_TO_PHYSICAL = auto()
+    LOGICAL_CREATE_FROM_SELECT_TO_PHYSICAL = auto()
     LOGICAL_CREATE_UDF_TO_PHYSICAL = auto()
     LOGICAL_SAMPLE_TO_UNIFORMSAMPLE = auto()
     LOGICAL_GET_TO_SEQSCAN = auto()
     LOGICAL_DERIVED_GET_TO_PHYSICAL = auto()
     LOGICAL_LATERAL_JOIN_TO_PHYSICAL = auto()
 
     LOGICAL_JOIN_TO_PHYSICAL_HASH_JOIN = auto()
```

### Comparing `evadb-0.2.4/eva/optimizer/rules/rules_manager.py` & `evadb-0.2.5/eva/optimizer/rules/rules_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,59 +14,48 @@
 # limitations under the License.
 from __future__ import annotations
 
 from contextlib import contextmanager
 from typing import List
 
 from eva.configuration.configuration_manager import ConfigurationManager
-from eva.experimental.ray.optimizer.rules.rules import LogicalExchangeToPhysical
-from eva.experimental.ray.optimizer.rules.rules import (
-    LogicalGetToSeqScan as DistributedLogicalGetToSeqScan,
-)
-from eva.experimental.ray.optimizer.rules.rules import (
-    LogicalProjectToPhysical as DistributedLogicalProjectToPhysical,
-)
 from eva.optimizer.rules.rules import (
     CacheFunctionExpressionInApply,
     CacheFunctionExpressionInFilter,
     CacheFunctionExpressionInProject,
     CombineSimilarityOrderByAndLimitToVectorIndexScan,
     EmbedFilterIntoGet,
     EmbedSampleIntoGet,
     LogicalApplyAndMergeToPhysical,
+    LogicalApplyAndMergeToRayPhysical,
+    LogicalCreateFromSelectToPhysical,
     LogicalCreateIndexToVectorIndex,
     LogicalCreateMaterializedViewToPhysical,
     LogicalCreateToPhysical,
     LogicalCreateUDFToPhysical,
     LogicalDeleteToPhysical,
     LogicalDerivedGetToPhysical,
     LogicalDropToPhysical,
     LogicalDropUDFToPhysical,
+    LogicalExchangeToPhysical,
     LogicalExplainToPhysical,
     LogicalFilterToPhysical,
     LogicalFunctionScanToPhysical,
-)
-from eva.optimizer.rules.rules import (
-    LogicalGetToSeqScan as SequentialLogicalGetToSeqScan,
-)
-from eva.optimizer.rules.rules import (
+    LogicalGetToSeqScan,
     LogicalGroupByToPhysical,
     LogicalInnerJoinCommutativity,
     LogicalInsertToPhysical,
     LogicalJoinToPhysicalHashJoin,
     LogicalJoinToPhysicalNestedLoopJoin,
     LogicalLateralJoinToPhysical,
     LogicalLimitToPhysical,
     LogicalLoadToPhysical,
     LogicalOrderByToPhysical,
-)
-from eva.optimizer.rules.rules import (
-    LogicalProjectToPhysical as SequentialLogicalProjectToPhysical,
-)
-from eva.optimizer.rules.rules import (
+    LogicalProjectToPhysical,
+    LogicalProjectToRayPhysical,
     LogicalRenameToPhysical,
     LogicalShowToPhysical,
     LogicalUnionToPhysical,
     LogicalVectorIndexScanToPhysical,
     PushDownFilterThroughApplyAndMerge,
     PushDownFilterThroughJoin,
     ReorderPredicates,
@@ -96,51 +85,55 @@
             EmbedSampleIntoGet(),
             PushDownFilterThroughJoin(),
             PushDownFilterThroughApplyAndMerge(),
             CombineSimilarityOrderByAndLimitToVectorIndexScan(),
             ReorderPredicates(),
         ]
 
-        ray_enabled = ConfigurationManager().get_value("experimental", "ray")
-
         self._implementation_rules = [
             LogicalCreateToPhysical(),
+            LogicalCreateFromSelectToPhysical(),
             LogicalRenameToPhysical(),
             LogicalDropToPhysical(),
             LogicalCreateUDFToPhysical(),
             LogicalDropUDFToPhysical(),
             LogicalInsertToPhysical(),
             LogicalDeleteToPhysical(),
             LogicalLoadToPhysical(),
-            DistributedLogicalGetToSeqScan()
-            if ray_enabled
-            else SequentialLogicalGetToSeqScan(),
+            LogicalGetToSeqScan(),
             LogicalDerivedGetToPhysical(),
             LogicalUnionToPhysical(),
             LogicalGroupByToPhysical(),
             LogicalOrderByToPhysical(),
             LogicalLimitToPhysical(),
             LogicalJoinToPhysicalNestedLoopJoin(),
             LogicalLateralJoinToPhysical(),
             LogicalJoinToPhysicalHashJoin(),
             LogicalFunctionScanToPhysical(),
             LogicalCreateMaterializedViewToPhysical(),
             LogicalFilterToPhysical(),
-            DistributedLogicalProjectToPhysical()
-            if ray_enabled
-            else SequentialLogicalProjectToPhysical(),
             LogicalShowToPhysical(),
             LogicalExplainToPhysical(),
             LogicalCreateIndexToVectorIndex(),
-            LogicalApplyAndMergeToPhysical(),
             LogicalVectorIndexScanToPhysical(),
         ]
 
+        ray_enabled = ConfigurationManager().get_value("experimental", "ray")
         if ray_enabled:
-            self._implementation_rules.append(LogicalExchangeToPhysical())
+            self._implementation_rules.extend(
+                [
+                    LogicalExchangeToPhysical(),
+                    LogicalApplyAndMergeToRayPhysical(),
+                    LogicalProjectToRayPhysical(),
+                ]
+            )
+        else:
+            self._implementation_rules.extend(
+                [LogicalApplyAndMergeToPhysical(), LogicalProjectToPhysical()]
+            )
         self._all_rules = (
             self._stage_one_rewrite_rules
             + self._stage_two_rewrite_rules
             + self._logical_rules
             + self._implementation_rules
         )
```

### Comparing `evadb-0.2.4/eva/optimizer/statement_to_opr_converter.py` & `evadb-0.2.5/eva/optimizer/statement_to_opr_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -240,14 +240,18 @@
         table_info = statement.table_info
         if table_info is None:
             logger.error("Missing Table Name In Create Statement")
 
         create_opr = LogicalCreate(
             table_info, statement.column_list, statement.if_not_exists
         )
+
+        if statement.query is not None:
+            self.visit_select(statement.query)
+            create_opr.append_child(self._plan)
         self._plan = create_opr
 
     def visit_rename(self, statement: RenameTableStatement):
         """Converter for parsed rename statement
         Arguments:
             statement(RenameTableStatement): [Rename statement]
         """
```

### Comparing `evadb-0.2.4/eva/parser/__init__.py` & `evadb-0.2.5/test/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/eva/parser/alias.py` & `evadb-0.2.5/eva/parser/alias.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/create_index_statement.py` & `evadb-0.2.5/eva/parser/create_index_statement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/create_mat_view_statement.py` & `evadb-0.2.5/eva/parser/create_mat_view_statement.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -62,14 +62,18 @@
     def query(self):
         return self._query
 
     @property
     def col_list(self):
         return self._col_list
 
+    @col_list.setter
+    def col_list(self, value):
+        self._col_list = value
+
     def __eq__(self, other):
         if not isinstance(other, CreateMaterializedViewStatement):
             return False
         return (
             self.view_info == other.view_info
             and self.col_list == other.col_list
             and self.if_not_exists == other.if_not_exists
```

### Comparing `evadb-0.2.4/eva/parser/create_statement.py` & `evadb-0.2.5/eva/parser/create_statement.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List, Tuple
 
 from eva.catalog.catalog_type import ColumnType, NdArrayType
+from eva.parser.select_statement import SelectStatement
 from eva.parser.statement import AbstractStatement
 from eva.parser.table_ref import TableInfo
 from eva.parser.types import StatementType
 
 
 class ColConstraintInfo:
     def __init__(self, nullable=False, default_value=None, primary=False, unique=False):
@@ -117,25 +118,32 @@
     """
 
     def __init__(
         self,
         table_info: TableInfo,
         if_not_exists: bool,
         column_list: List[ColumnDefinition] = None,
+        query: SelectStatement = None,
     ):
         super().__init__(StatementType.CREATE)
         self._table_info = table_info
         self._if_not_exists = if_not_exists
         self._column_list = column_list
+        self._query = query
 
     def __str__(self) -> str:
         print_str = "CREATE TABLE {} ({}) \n".format(
             self._table_info, self._if_not_exists
         )
 
+        if self._query is not None:
+            print_str = "CREATE TABLE {} AS {}\n".format(
+                self._table_info, self._query
+            )
+
         for column in self.column_list:
             print_str += str(column) + "\n"
 
         return print_str
 
     @property
     def table_info(self):
@@ -145,25 +153,35 @@
     def if_not_exists(self):
         return self._if_not_exists
 
     @property
     def column_list(self):
         return self._column_list
 
+    @property
+    def query(self):
+        return self._query
+
+    @column_list.setter
+    def column_list(self, value):
+        self._column_list = value
+
     def __eq__(self, other):
         if not isinstance(other, CreateTableStatement):
             return False
         return (
             self.table_info == other.table_info
             and self.if_not_exists == other.if_not_exists
             and self.column_list == other.column_list
+            and self.query == other.query
         )
 
     def __hash__(self) -> int:
         return hash(
             (
                 super().__hash__(),
                 self.table_info,
                 self.if_not_exists,
                 tuple(self.column_list or []),
+                self.query
             )
         )
```

### Comparing `evadb-0.2.4/eva/parser/create_udf_statement.py` & `evadb-0.2.5/eva/parser/create_udf_statement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/delete_statement.py` & `evadb-0.2.5/eva/parser/delete_statement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/drop_statement.py` & `evadb-0.2.5/eva/parser/drop_statement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/drop_udf_statement.py` & `evadb-0.2.5/eva/parser/drop_udf_statement.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/eva.lark` & `evadb-0.2.5/eva/parser/eva.lark`

 * *Files 1% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 
 //    Create statements
 
 create_database: CREATE DATABASE if_not_exists? uid
 
 create_index: CREATE INDEX uid ON table_name index_elem vector_store_type?
 
-create_table: CREATE TABLE if_not_exists? table_name create_definitions 
+create_table: CREATE TABLE if_not_exists? table_name (create_definitions | (AS select_statement))
     
 // Rename statements
 
 rename_table: RENAME TABLE table_name TO table_name
     
 // Create UDFs
 create_udf: CREATE UDF if_not_exists? udf_name INPUT create_definitions OUTPUT create_definitions TYPE udf_type IMPL udf_impl udf_metadata* | CREATE UDF if_not_exists? udf_name IMPL udf_impl udf_metadata* | CREATE UDF if_not_exists? udf_name TYPE udf_type udf_metadata*
 
 // Create Materialized View
-create_materialized_view: CREATE MATERIALIZED VIEW if_not_exists? table_name ("(" uid_list ")") AS select_statement 
+create_materialized_view: CREATE MATERIALIZED VIEW if_not_exists? table_name ("(" uid_list ")")? AS select_statement
 
 // Details
 udf_name: uid
 
 udf_type: uid
 
 udf_impl: string_literal
@@ -83,15 +83,15 @@
 select_statement: query_specification                          ->simple_select
                | select_statement UNION ALL? select_statement  ->union_select
     
 update_statement: UPDATE table_name (AS? uid)? SET updated_element ("," updated_element)* (WHERE expression)? order_by_clause? limit_clause?
     
 load_statement: LOAD file_format file_name INTO table_name (("(" uid_list ")"))?
     
-file_format: CSV | VIDEO | IMAGE
+file_format: CSV | VIDEO | IMAGE | DOCUMENT | PDF
 
 file_options: FORMAT file_format
     
 file_name: string_literal
         
 // details
 
@@ -375,14 +375,16 @@
 
 // File Formats
 WITH:                 "WITH"i
 FORMAT:               "FORMAT"i
 CSV:                  "CSV"i
 VIDEO:                "VIDEO"i
 IMAGE:                "IMAGE"i
+DOCUMENT:             "DOCUMENT"i
+PDF:                  "PDF"i
 
 // Index types
 HNSW:                                "HNSW"i
 FAISS:                               "FAISS"i
 QDRANT:                              "QDRANT"i
 
 // Computer vision tasks
```

### Comparing `evadb-0.2.4/eva/parser/explain_statement.py` & `evadb-0.2.5/eva/parser/explain_statement.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/insert_statement.py` & `evadb-0.2.5/eva/parser/insert_statement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/lark_parser.py` & `evadb-0.2.5/eva/parser/lark_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -35,15 +35,14 @@
         dir_path = os.path.dirname(os.path.realpath(__file__))
         lark_path = os.path.join(dir_path, "eva.lark")
         with open(lark_path) as f:
             sql_grammar = f.read()
         self._parser = Lark(sql_grammar, parser="lalr")
 
     def parse(self, query_string: str) -> list:
-
         # remove trailing white space
         query_string = query_string.rstrip()
 
         # add semi-colon if needed
         if not query_string.endswith(";"):
             query_string += ";"
```

### Comparing `evadb-0.2.4/eva/parser/lark_visitor/__init__.py` & `evadb-0.2.5/eva/parser/lark_visitor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/lark_visitor/_common_clauses_ids.py` & `evadb-0.2.5/eva/parser/lark_visitor/_common_clauses_ids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/lark_visitor/_create_statements.py` & `evadb-0.2.5/eva/parser/lark_visitor/_create_statements.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -32,26 +32,29 @@
 # CREATE STATEMENTS
 ##################################################################
 class CreateTable:
     def create_table(self, tree):
         table_info = None
         if_not_exists = False
         create_definitions = []
+        query = None
 
         for child in tree.children:
             if isinstance(child, Tree):
                 if child.data == "if_not_exists":
                     if_not_exists = True
                 elif child.data == "table_name":
                     table_info = self.visit(child)
                 elif child.data == "create_definitions":
                     create_definitions = self.visit(child)
+                elif child.data == "simple_select":
+                    query = self.visit(child)
 
         create_stmt = CreateTableStatement(
-            table_info, if_not_exists, create_definitions
+            table_info, if_not_exists, create_definitions, query=query
         )
         return create_stmt
 
     def create_definitions(self, tree):
         column_definitions = []
         for child in tree.children:
             if isinstance(child, Tree):
@@ -230,28 +233,28 @@
         return dimensions
 
     # MATERIALIZED VIEW
     def create_materialized_view(self, tree):
         view_info = None
         if_not_exists = False
         query = None
+        uid_list = []
 
         for child in tree.children:
             if isinstance(child, Tree):
                 if child.data == "table_name":
                     view_info = self.visit(child)
                 elif child.data == "if_not_exists":
                     if_not_exists = True
                 elif child.data == "uid_list":
                     uid_list = self.visit(child)
                 elif child.data == "simple_select":
                     query = self.visit(child)
 
-        # setting all other column definition attributes as None,
-        # need to figure from query
+        # When uid_list is empty, the column information is inferred from the subquery in the binder.
         col_list = [
             ColumnDefinition(uid.col_name, None, None, None) for uid in uid_list
         ]
         return CreateMaterializedViewStatement(
             view_info, col_list, if_not_exists, query
         )
```

### Comparing `evadb-0.2.4/eva/parser/lark_visitor/_delete_statement.py` & `evadb-0.2.5/eva/parser/lark_visitor/_delete_statement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/lark_visitor/_drop_statement.py` & `evadb-0.2.5/eva/parser/lark_visitor/_drop_statement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/lark_visitor/_explain_statement.py` & `evadb-0.2.5/eva/parser/lark_visitor/_explain_statement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/lark_visitor/_expressions.py` & `evadb-0.2.5/eva/parser/lark_visitor/_expressions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/lark_visitor/_functions.py` & `evadb-0.2.5/eva/parser/lark_visitor/_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/lark_visitor/_insert_statements.py` & `evadb-0.2.5/eva/parser/lark_visitor/_insert_statements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/lark_visitor/_load_statement.py` & `evadb-0.2.5/eva/parser/lark_visitor/_load_statement.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -47,14 +47,18 @@
 
         if file_format_string == "VIDEO":
             file_format = FileFormatType.VIDEO
         elif file_format_string == "CSV":
             file_format = FileFormatType.CSV
         elif file_format_string == "IMAGE":
             file_format = FileFormatType.IMAGE
+        elif file_format_string == "DOCUMENT":
+            file_format = FileFormatType.DOCUMENT
+        elif file_format_string == "PDF":
+            file_format = FileFormatType.PDF
 
         return file_format
 
     def file_options(self, tree):
         file_options = {}
         file_format = self.visit(tree.children[1])
         file_options["file_format"] = file_format
```

### Comparing `evadb-0.2.4/eva/parser/lark_visitor/_rename_statement.py` & `evadb-0.2.5/eva/parser/lark_visitor/_rename_statement.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/lark_visitor/_select_statement.py` & `evadb-0.2.5/eva/parser/lark_visitor/_select_statement.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/lark_visitor/_show_statements.py` & `evadb-0.2.5/eva/parser/lark_visitor/_show_statements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/lark_visitor/_table_sources.py` & `evadb-0.2.5/eva/parser/lark_visitor/_table_sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -123,15 +123,15 @@
                 raise e
 
         select_stmt = SelectStatement(
             target_list,
             from_clause,
             where_clause,
             groupby_clause=groupby_clause,
-            orderby_clause_list=orderby_clause,
+            orderby_list=orderby_clause,
             limit_count=limit_count,
         )
 
         return select_stmt
 
     # TODO ACTION
     def from_clause(self, tree):
@@ -198,15 +198,15 @@
         func_expr = None
         has_unnest = False
 
         for child in tree.children:
             if isinstance(child, Tree):
                 if child.data.endswith("function_call"):
                     func_expr = self.visit(child)
-            elif child == "UNNEST":
+            elif child.lower() == "unnest":
                 has_unnest = True
 
         return TableValuedExpression(func_expr, do_unnest=has_unnest)
 
     def subquery_table_source_item(self, tree):
         subquery_table_source_item = None
         for child in tree.children:
```

### Comparing `evadb-0.2.4/eva/parser/load_statement.py` & `evadb-0.2.5/eva/parser/load_statement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/parser.py` & `evadb-0.2.5/eva/parser/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -31,10 +31,9 @@
     def __init__(self):
         if self._initialized:
             return
         self._lark_parser = LarkParser()
         self._initialized = True
 
     def parse(self, query_string: str) -> list:
-
         lark_output = self._lark_parser.parse(query_string)
         return lark_output
```

### Comparing `evadb-0.2.4/eva/parser/rename_statement.py` & `evadb-0.2.5/eva/parser/rename_statement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/select_statement.py` & `evadb-0.2.5/eva/parser/select_statement.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -52,15 +52,15 @@
         super().__init__(StatementType.SELECT)
         self._from_table = from_table
         self._where_clause = where_clause
         self._target_list = target_list
         self._union_link = None
         self._union_all = False
         self._groupby_clause = kwargs.get("groupby_clause", None)
-        self._orderby_list = kwargs.get("orderby_clause_list", None)
+        self._orderby_list = kwargs.get("orderby_list", None)
         self._limit_count = kwargs.get("limit_count", None)
 
     @property
     def union_link(self):
         return self._union_link
 
     @union_link.setter
@@ -99,22 +99,34 @@
     def from_table(self, table: TableRef):
         self._from_table = table
 
     @property
     def groupby_clause(self):
         return self._groupby_clause
 
+    @groupby_clause.setter
+    def groupby_clause(self, groupby_clause):
+        self._groupby_clause = groupby_clause
+
     @property
     def orderby_list(self):
         return self._orderby_list
 
+    @orderby_list.setter
+    def orderby_list(self, orderby_list):
+        self._orderby_list = orderby_list
+
     @property
     def limit_count(self):
         return self._limit_count
 
+    @limit_count.setter
+    def limit_count(self, limit_count):
+        self._limit_count = limit_count
+
     def __str__(self) -> str:
         target_list_str = ""
         if self._target_list is not None:
             for expr in self._target_list:
                 target_list_str += str(expr) + ", "
             target_list_str = target_list_str.rstrip(", ")
 
@@ -126,15 +138,14 @@
                     sort_str = "ASC"
                 elif expr[1] == ParserOrderBySortType.DESC:
                     sort_str = "DESC"
                 orderby_list_str += str(expr[0]) + " " + sort_str + ", "
             orderby_list_str = orderby_list_str.rstrip(", ")
 
         select_str = f"SELECT {target_list_str} FROM {str(self._from_table)}"
-
         if self._where_clause is not None:
             select_str += " WHERE " + str(self._where_clause)
 
         if self._union_link is not None:
             if not self._union_all:
                 select_str += " UNION " + str(self._union_link)
             else:
```

### Comparing `evadb-0.2.4/eva/parser/show_statement.py` & `evadb-0.2.5/eva/parser/show_statement.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/parser/statement.py` & `evadb-0.2.5/eva/parser/statement.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from copy import deepcopy
+
 from eva.parser.types import StatementType
 
 
 class AbstractStatement:
     """
     Base class for all Statements
 
@@ -30,7 +32,19 @@
 
     @property
     def stmt_type(self):
         return self._stmt_type
 
     def __hash__(self) -> int:
         return hash(self.stmt_type)
+
+    def __deepcopy__(self, memo):
+        cls = self.__class__
+        result = cls.__new__(cls)
+        memo[id(self)] = result
+        for k, v in self.__dict__.items():
+            setattr(result, k, deepcopy(v, memo))
+        return result
+
+    def copy(self):
+        """Returns a deepcopy of the statement."""
+        return deepcopy(self)
```

### Comparing `evadb-0.2.4/eva/parser/table_ref.py` & `evadb-0.2.5/eva/parser/table_ref.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -125,15 +125,17 @@
         return self._func_expr
 
     @property
     def do_unnest(self):
         return self._do_unnest
 
     def __str__(self) -> str:
-        return "{}".format(self._func_expr)
+        if self.do_unnest:
+            return f"unnest({self._func_expr})"
+        return f"{self._func_expr}"
 
     def __eq__(self, other):
         if not isinstance(other, TableValuedExpression):
             return False
         return self.func_expr == other.func_expr and self.do_unnest == other.do_unnest
 
     def __hash__(self) -> int:
@@ -254,23 +256,23 @@
         # create alias for the table
         # TableInfo -> table_name.lower()
         # SelectStatement -> select
         if isinstance(self._ref_handle, TableInfo):
             return Alias(self._ref_handle.table_name.lower())
 
     def __str__(self):
-        table_ref_str = f"{str(self._ref_handle)}"
+        if self.is_select():
+            table_ref_str = f"( {str(self._ref_handle)} ) AS {self.alias}"
+        else:
+            table_ref_str = f"{str(self._ref_handle)}"
+
         if self.sample_freq is not None:
             table_ref_str += f" {str(self.sample_freq)}"
         if self.sample_type is not None:
             table_ref_str += f" {str(self.sample_type)}"
-        if self._get_video is not None:
-            table_ref_str += f" {str(self._get_video)}"
-        if self._get_audio is not None:
-            table_ref_str += f" {str(self._get_audio)}"
         return table_ref_str
 
     def __eq__(self, other):
         if not isinstance(other, TableRef):
             return False
         return (
             self._ref_handle == other._ref_handle
```

### Comparing `evadb-0.2.4/eva/parser/types.py` & `evadb-0.2.5/eva/parser/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -58,14 +58,16 @@
     INNER_JOIN  # noqa: F821
 
 
 class FileFormatType(EVAEnum):
     VIDEO  # noqa: F821
     CSV  # noqa: F821
     IMAGE  # noqa: F821
+    DOCUMENT  # noqa: F821
+    PDF  # noqa: F821
 
 
 class ShowType(EVAEnum):
     UDFS  # noqa: F821
     TABLES  # noqa: F821
```

### Comparing `evadb-0.2.4/eva/plan_nodes/__init__.py` & `evadb-0.2.5/eva/interfaces/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""planner subdirectory"""
```

### Comparing `evadb-0.2.4/eva/plan_nodes/abstract_join_plan.py` & `evadb-0.2.5/eva/plan_nodes/abstract_join_plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/abstract_plan.py` & `evadb-0.2.5/eva/plan_nodes/abstract_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/abstract_scan_plan.py` & `evadb-0.2.5/eva/plan_nodes/abstract_scan_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/apply_and_merge_plan.py` & `evadb-0.2.5/eva/plan_nodes/apply_and_merge_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/create_index_plan.py` & `evadb-0.2.5/eva/plan_nodes/create_index_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/create_mat_view_plan.py` & `evadb-0.2.5/eva/plan_nodes/create_mat_view_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/create_plan.py` & `evadb-0.2.5/eva/plan_nodes/create_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import List
-
 from eva.catalog.models.column_catalog import ColumnCatalogEntry
+
 from eva.parser.table_ref import TableInfo
 from eva.plan_nodes.abstract_plan import AbstractPlan
 from eva.plan_nodes.types import PlanOprType
 
 
 class CreatePlan(AbstractPlan):
     """
```

### Comparing `evadb-0.2.4/eva/plan_nodes/create_udf_plan.py` & `evadb-0.2.5/eva/plan_nodes/create_udf_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/delete_plan.py` & `evadb-0.2.5/eva/plan_nodes/delete_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/drop_plan.py` & `evadb-0.2.5/eva/plan_nodes/drop_plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/drop_udf_plan.py` & `evadb-0.2.5/eva/plan_nodes/drop_udf_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/explain_plan.py` & `evadb-0.2.5/eva/plan_nodes/explain_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/function_scan_plan.py` & `evadb-0.2.5/eva/plan_nodes/function_scan_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/groupby_plan.py` & `evadb-0.2.5/eva/plan_nodes/groupby_plan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/hash_join_build_plan.py` & `evadb-0.2.5/eva/plan_nodes/hash_join_build_plan.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/hash_join_probe_plan.py` & `evadb-0.2.5/eva/plan_nodes/hash_join_probe_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/insert_plan.py` & `evadb-0.2.5/eva/plan_nodes/insert_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/lateral_join_plan.py` & `evadb-0.2.5/eva/plan_nodes/lateral_join_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/limit_plan.py` & `evadb-0.2.5/eva/plan_nodes/limit_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/load_data_plan.py` & `evadb-0.2.5/eva/plan_nodes/load_data_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/nested_loop_join_plan.py` & `evadb-0.2.5/eva/plan_nodes/nested_loop_join_plan.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/orderby_plan.py` & `evadb-0.2.5/eva/plan_nodes/orderby_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/pp_plan.py` & `evadb-0.2.5/eva/plan_nodes/pp_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/predicate_plan.py` & `evadb-0.2.5/eva/plan_nodes/predicate_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/project_plan.py` & `evadb-0.2.5/eva/plan_nodes/project_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/rename_plan.py` & `evadb-0.2.5/eva/plan_nodes/rename_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/sample_plan.py` & `evadb-0.2.5/eva/plan_nodes/sample_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/seq_scan_plan.py` & `evadb-0.2.5/eva/plan_nodes/seq_scan_plan.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/show_info_plan.py` & `evadb-0.2.5/eva/plan_nodes/show_info_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/storage_plan.py` & `evadb-0.2.5/eva/plan_nodes/storage_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/types.py` & `evadb-0.2.5/eva/plan_nodes/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/plan_nodes/union_plan.py` & `evadb-0.2.5/eva/utils/errors.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,28 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from eva.plan_nodes.abstract_plan import AbstractPlan
-from eva.plan_nodes.types import PlanOprType
+class CatalogError(Exception):
+    pass
 
 
-class UnionPlan(AbstractPlan):
-    """
-    This plan is used for storing information required for union operations.
+class UDFIODefinitionError(Exception):
+    pass
 
-    Arguments:
-        all: Bool
-            UNION (deduplication) vs UNION ALL (non-deduplication)
-    """
 
-    def __init__(self, all: bool):
-        self._all = all
-        super().__init__(PlanOprType.UNION)
-
-    @property
-    def all(self):
-        return self._all
-
-    def __str__(self):
-        return "UnionAllPlan" if self._all else "UnionPlan"
-
-    def __hash__(self) -> int:
-        return hash((super().__hash__(), self._all))
+class DatasetFileNotFoundError(Exception):
+    def __init__(
+        self,
+        message="The dataset file could not be found. Please verify that the file exists in the specified path.",
+    ):
+        super().__init__(message)
```

### Comparing `evadb-0.2.4/eva/plan_nodes/vector_index_scan_plan.py` & `evadb-0.2.5/eva/plan_nodes/vector_index_scan_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/readers/__init__.py` & `evadb-0.2.5/test/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/eva/readers/abstract_reader.py` & `evadb-0.2.5/eva/readers/abstract_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/readers/csv_reader.py` & `evadb-0.2.5/eva/readers/csv_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/readers/decord_reader.py` & `evadb-0.2.5/eva/readers/decord_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/readers/image/__init__.py` & `evadb-0.2.5/test/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/eva/readers/image/opencv_image_reader.py` & `evadb-0.2.5/eva/readers/image/opencv_image_reader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/server/__init__.py` & `evadb-0.2.5/test/udfs/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""sets up a local-hosted server"""
+"""user defined functions operating on ndarrays"""
```

### Comparing `evadb-0.2.4/eva/server/command_handler.py` & `evadb-0.2.5/eva/server/command_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -67,15 +67,15 @@
     error_msg = None
     query_runtime = Timer()
     with query_runtime:
         try:
             output_batch = execute_query_fetch_all(request_message)
         except Exception as e:
             error_msg = str(e)
-            logger.warn(error_msg)
+            logger.exception(error_msg)
             error = True
 
     if not error:
         response = Response(
             status=ResponseStatus.SUCCESS,
             batch=output_batch,
             query_time=query_runtime.total_elapsed_time,
```

### Comparing `evadb-0.2.4/eva/server/interpreter.py` & `evadb-0.2.5/eva/server/interpreter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,15 +15,15 @@
 import asyncio
 import os
 import sys
 from asyncio import StreamReader, StreamWriter
 from collections import deque
 from typing import Dict
 
-from eva.server.db_api import EVAConnection
+from eva.interfaces.relational.db import EVAConnection
 from eva.utils.logging_manager import logger
 
 # version.py defines the VERSION and VERSION_SHORT variables
 VERSION_DICT: Dict[str, str] = {}
 
 current_file_dir = os.path.dirname(__file__)
 current_file_parent_dir = os.path.join(current_file_dir, os.pardir)
```

### Comparing `evadb-0.2.4/eva/server/server.py` & `evadb-0.2.5/eva/server/server.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,15 +12,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import asyncio
 import string
 from asyncio import StreamReader, StreamWriter
 
-from eva.server.command_handler import handle_request
 from eva.utils.logging_manager import logger
 
 
 class EvaServer:
     """
     Receives messages and offloads them to another task for processing them.
     """
@@ -33,26 +32,25 @@
         """
         Start the server
         Server objects are asynchronous context managers.
 
         hostname: hostname of the server
         port: port of the server
         """
-        logger.info("Start Server")
-        print(f"EVA Server started at host {host} and port {port}", flush=True)
+        logger.warn(f"EVA server started at host {host} and port {port}")
 
         self._server = await asyncio.start_server(self.accept_client, host, port)
 
         async with self._server:
             await self._server.serve_forever()
 
-        logger.info("Successfully shutdown server")
+        logger.warn("EVA server stopped")
 
     async def stop_eva_server(self):
-        logger.info("Stop server")
+        logger.warn("EVA server stopped")
         if self._server is not None:
             await self._server.close()
 
     async def accept_client(
         self, client_reader: StreamReader, client_writer: StreamWriter
     ):
         task = asyncio.Task(self.handle_client(client_reader, client_writer))
@@ -79,11 +77,13 @@
                 logger.debug("Received --|%s|--", message)
 
                 if message.upper() in ["EXIT;", "QUIT;"]:
                     logger.info("Close client")
                     return
 
                 logger.debug("Handle request")
+                from eva.server.command_handler import handle_request
+
                 asyncio.create_task(handle_request(client_writer, message))
 
         except Exception as e:
             logger.critical("Error reading from client.", exc_info=e)
```

### Comparing `evadb-0.2.4/eva/storage/__init__.py` & `evadb-0.2.5/eva/interfaces/relational/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""
-storage subdirectory
-"""
```

### Comparing `evadb-0.2.4/eva/storage/abstract_media_storage_engine.py` & `evadb-0.2.5/eva/storage/abstract_media_storage_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/storage/abstract_storage_engine.py` & `evadb-0.2.5/eva/storage/abstract_storage_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/storage/image_storage_engine.py` & `evadb-0.2.5/eva/storage/image_storage_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/storage/sqlite_storage_engine.py` & `evadb-0.2.5/eva/storage/sqlite_storage_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/storage/storage_engine.py` & `evadb-0.2.5/eva/storage/storage_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,28 +12,33 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from eva.catalog.catalog_type import TableType
 from eva.catalog.models.table_catalog import TableCatalogEntry
 from eva.configuration.configuration_manager import ConfigurationManager
 from eva.storage.abstract_storage_engine import AbstractStorageEngine
+from eva.storage.document_storage_engine import DocumentStorageEngine
 from eva.utils.generic_utils import str_to_class
 
 
 class StorageEngine:
     storages = {
         TableType.STRUCTURED_DATA: str_to_class(
             ConfigurationManager().get_value("storage", "structured_data_engine")
         )(),
         TableType.VIDEO_DATA: str_to_class(
             ConfigurationManager().get_value("storage", "video_engine")
         )(),
         TableType.IMAGE_DATA: str_to_class(
             ConfigurationManager().get_value("storage", "image_engine")
         )(),
+        TableType.DOCUMENT_DATA: DocumentStorageEngine(),
+        TableType.PDF_DATA: str_to_class(
+            ConfigurationManager().get_value("storage", "pdf_engine")
+        )(),
     }
 
     @classmethod
     def factory(cls, table: TableCatalogEntry) -> AbstractStorageEngine:
         if table is None:
             raise ValueError("Expected TableCatalogEntry, got None")
         if table.table_type in cls.storages:
```

### Comparing `evadb-0.2.4/eva/storage/video_storage_engine.py` & `evadb-0.2.5/eva/storage/video_storage_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/third_party/__init__.py` & `evadb-0.2.5/eva/third_party/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/third_party/huggingface/__init__.py` & `evadb-0.2.5/test/udfs/ndarray/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""hugging face utils"""
+"""user defined test functions operating on ndarrays udfs"""
```

### Comparing `evadb-0.2.4/eva/third_party/huggingface/binder.py` & `evadb-0.2.5/eva/third_party/huggingface/binder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/third_party/huggingface/create.py` & `evadb-0.2.5/eva/third_party/huggingface/create.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -37,14 +37,15 @@
     "audio-classification": HFInputTypes.AUDIO,
     "automatic-speech-recognition": HFInputTypes.AUDIO,
     "text-classification": HFInputTypes.TEXT,
     "summarization": HFInputTypes.TEXT,
     "translation": HFInputTypes.TEXT,
     "text2text-generation": HFInputTypes.TEXT,
     "text-generation": HFInputTypes.TEXT,
+    "ner": HFInputTypes.TEXT,
     "image-classification": HFInputTypes.IMAGE,
     "image-segmentation": HFInputTypes.IMAGE,
     "image-to-text": HFInputTypes.IMAGE,
     "object-detection": HFInputTypes.IMAGE,
     "depth-estimation": HFInputTypes.IMAGE,
 }
 
@@ -52,24 +53,25 @@
     "audio-classification": AudioHFModel,
     "automatic-speech-recognition": ASRHFModel,
     "text-classification": TextHFModel,
     "summarization": TextHFModel,
     "translation": TextHFModel,
     "text2text-generation": TextHFModel,
     "text-generation": TextHFModel,
+    "ner": TextHFModel,
     "image-classification": ImageHFModel,
     "image-segmentation": ImageHFModel,
     "image-to-text": ImageHFModel,
     "object-detection": ImageHFModel,
     "depth-estimation": ImageHFModel,
 }
 
 
 def sample_text():
-    return "The cat is on the mat"
+    return "My name is Sarah and I live in London"
 
 
 def sample_image():
     width, height = 224, 224
     image = Image.new("RGB", (width, height), "white")
     draw = ImageDraw.Draw(image)
```

### Comparing `evadb-0.2.4/eva/third_party/huggingface/model.py` & `evadb-0.2.5/eva/third_party/huggingface/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/third_party/vector_stores/__init__.py` & `evadb-0.2.5/test/integration_tests/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""vector stores"""
```

### Comparing `evadb-0.2.4/eva/third_party/vector_stores/faiss.py` & `evadb-0.2.5/eva/third_party/vector_stores/faiss.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from pathlib import Path
 from typing import List
 
 import numpy as np
 
 from eva.third_party.vector_stores.types import (
     FeaturePayload,
     VectorIndexQuery,
@@ -81,9 +82,10 @@
         distances, ids = [], []
         for dis, idx in zip(dists[0], indices[0]):
             distances.append(dis)
             ids.append(idx)
         return VectorIndexQueryResult(distances, ids)
 
     def delete(self):
-        if self._index_path.exists():
-            self._index_path.unlink()
+        index_path = Path(self._index_path)
+        if index_path.exists():
+            index_path.unlink()
```

### Comparing `evadb-0.2.4/eva/third_party/vector_stores/qdrant.py` & `evadb-0.2.5/eva/third_party/vector_stores/qdrant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/third_party/vector_stores/types.py` & `evadb-0.2.5/eva/third_party/vector_stores/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/third_party/vector_stores/utils.py` & `evadb-0.2.5/eva/third_party/vector_stores/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/__init__.py` & `evadb-0.2.5/eva/udfs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/abstract/__init__.py` & `evadb-0.2.5/eva/udfs/abstract/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/abstract/abstract_udf.py` & `evadb-0.2.5/eva/udfs/abstract/abstract_udf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/abstract/hf_abstract_udf.py` & `evadb-0.2.5/eva/udfs/abstract/hf_abstract_udf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -76,19 +76,23 @@
             {'text' : 'transcript from video'}
             [[{'score': 0.25, 'label': 'bridge'}, {'score': 0.50, 'label': 'car'}]]
         """
         if isinstance(outputs, dict):
             return pd.DataFrame(outputs, index=[0])
         # PERF: Can improve performance by avoiding redundant list creation
         result_list = []
-        for row_output in outputs:
-            # account for the case where we have more than one prediction for an input
-            if isinstance(row_output, list):
-                row_output = {k: [dic[k] for dic in row_output] for k in row_output[0]}
-            result_list.append(row_output)
+        if outputs != [[]]:
+            for row_output in outputs:
+                # account for the case where we have more than one prediction for an input
+                if isinstance(row_output, list):
+                    row_output = {
+                        k: [dic[k] for dic in row_output] for k in row_output[0]
+                    }
+                result_list.append(row_output)
+
         result_df = pd.DataFrame(result_list)
         return result_df
 
     def forward(self, inputs, *args, **kwargs) -> pd.DataFrame:
         hf_input = self.input_formatter(inputs)
         hf_output = self.hf_udf_obj(hf_input, *args, **kwargs)
         eva_output = self.output_formatter(hf_output)
```

### Comparing `evadb-0.2.4/eva/udfs/abstract/pytorch_abstract_udf.py` & `evadb-0.2.5/eva/udfs/abstract/pytorch_abstract_udf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/abstract/tracker_abstract_udf.py` & `evadb-0.2.5/eva/udfs/abstract/tracker_abstract_udf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/asl_action_recognition.py` & `evadb-0.2.5/eva/udfs/asl_action_recognition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/chatgpt.py` & `evadb-0.2.5/eva/udfs/chatgpt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+import os
+
 import openai
 import pandas as pd
 
 from eva.catalog.catalog_type import NdArrayType
 from eva.configuration.configuration_manager import ConfigurationManager
 from eva.udfs.abstract.abstract_udf import AbstractUDF
 from eva.udfs.decorators.decorators import forward, setup
@@ -40,17 +42,21 @@
 
     @setup(cacheable=False, udf_type="chat-completion", batchable=True)
     def setup(
         self,
         model="gpt-3.5-turbo",
         temperature: float = 0,
     ) -> None:
+        # Try Configuration Manager
         openai.api_key = ConfigurationManager().get_value(
             "third_party", "openai_api_key"
         )
+        # If not found, try OS Environment Variable
+        if len(openai.api_key) == 0:
+            openai.api_key = os.environ["openai_api_key"]
         assert (
             len(openai.api_key) != 0
         ), "Please set your OpenAI API key in eva.yml file (third_party, open_api_key)"
 
         assert model in _VALID_CHAT_COMPLETION_MODEL, f"Unsupported ChatGPT {model}"
 
         self.model = model
```

### Comparing `evadb-0.2.4/eva/udfs/decorators/__init__.py` & `evadb-0.2.5/test/models/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/eva/udfs/decorators/decorators.py` & `evadb-0.2.5/eva/udfs/decorators/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/decorators/io_descriptors/__init__.py` & `evadb-0.2.5/test/models/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/eva/udfs/decorators/io_descriptors/abstract_types.py` & `evadb-0.2.5/eva/udfs/decorators/io_descriptors/abstract_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/decorators/io_descriptors/data_types.py` & `evadb-0.2.5/eva/udfs/decorators/io_descriptors/data_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/decorators/utils.py` & `evadb-0.2.5/eva/udfs/decorators/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/emotion_detector.py` & `evadb-0.2.5/eva/udfs/emotion_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/face_detector.py` & `evadb-0.2.5/eva/udfs/face_detector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/fastrcnn_object_detector.py` & `evadb-0.2.5/eva/udfs/fastrcnn_object_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/feature_extractor.py` & `evadb-0.2.5/eva/udfs/feature_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/gpu_compatible.py` & `evadb-0.2.5/eva/udfs/gpu_compatible.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/mvit_action_recognition.py` & `evadb-0.2.5/eva/udfs/mvit_action_recognition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/ndarray/__init__.py` & `evadb-0.2.5/test/models/storage/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""user defined functions operating on ndarrays"""
```

### Comparing `evadb-0.2.4/eva/udfs/ndarray/array_count.py` & `evadb-0.2.5/eva/udfs/ndarray/array_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/ndarray/crop.py` & `evadb-0.2.5/eva/udfs/ndarray/crop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/ndarray/fuzzy_join.py` & `evadb-0.2.5/eva/udfs/ndarray/fuzzy_join.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/ndarray/open.py` & `evadb-0.2.5/eva/udfs/ndarray/open.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/ndarray/similarity.py` & `evadb-0.2.5/eva/udfs/ndarray/similarity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/ocr_extractor.py` & `evadb-0.2.5/eva/udfs/ocr_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/sift_feature_extractor.py` & `evadb-0.2.5/eva/udfs/sift_feature_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/trackers/__init__.py` & `evadb-0.2.5/eva/utils/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""user defined functions for object tracking"""
+"""general eva utils"""
```

### Comparing `evadb-0.2.4/eva/udfs/trackers/nor_fair.py` & `evadb-0.2.5/eva/udfs/trackers/nor_fair.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/udfs/udf_bootstrap_queries.py` & `evadb-0.2.5/eva/udfs/udf_bootstrap_queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,14 +14,15 @@
 # limitations under the License.
 
 from eva.configuration.configuration_manager import ConfigurationManager
 from eva.server.command_handler import execute_query_fetch_all
 
 EVA_INSTALLATION_DIR = ConfigurationManager().get_value("core", "eva_installation_dir")
 NDARRAY_DIR = "ndarray"
+TUTORIALS_DIR = "tutorials"
 
 DummyObjectDetector_udf_query = """CREATE UDF IF NOT EXISTS DummyObjectDetector
                   INPUT  (Frame_Array NDARRAY INT8(3, ANYDIM, ANYDIM))
                   OUTPUT (label NDARRAY STR(1))
                   TYPE  Classification
                   IMPL  '{}/../test/util.py';
         """.format(
@@ -146,27 +147,35 @@
         OUTPUT (labels NDARRAY STR(ANYDIM))
         TYPE  Classification
         IMPL  '{}/udfs/asl_action_recognition.py';
         """.format(
     EVA_INSTALLATION_DIR
 )
 
-
 norfair_obj_tracker_query = """CREATE UDF IF NOT EXISTS NorFairTracker
                   IMPL  '{}/udfs/trackers/nor_fair.py';
         """.format(
     EVA_INSTALLATION_DIR
 )
 
 Sift_udf_query = """CREATE UDF IF NOT EXISTS SiftFeatureExtractor
         IMPL  '{}/udfs/sift_feature_extractor.py';
         """.format(
     EVA_INSTALLATION_DIR
 )
 
+mnistcnn_udf_query = """CREATE UDF IF NOT EXISTS MnistImageClassifier
+        INPUT  (data NDARRAY (3, 28, 28))
+        OUTPUT (label TEXT(2))
+        TYPE  Classification
+        IMPL  '{}/udfs/mnist_image_classifier.py';
+        """.format(
+    EVA_INSTALLATION_DIR
+)
+
 
 def init_builtin_udfs(mode: str = "debug") -> None:
     """Load the built-in UDFs into the system during system bootstrapping.
 
     The function loads a set of pre-defined UDF queries based on the `mode` argument.
     In 'debug' mode, the function loads debug UDFs along with release UDFs.
     In 'release' mode, only release UDFs are loaded. In addition, in 'debug' mode,
@@ -181,14 +190,15 @@
     queries = [
         Fastrcnn_udf_query,
         ArrayCount_udf_query,
         Crop_udf_query,
         Open_udf_query,
         Similarity_udf_query,
         norfair_obj_tracker_query,
+        mnistcnn_udf_query
         # Disabled because required packages (eg., easy_ocr might not be preinstalled)
         # face_detection_udf_query,
         # ocr_udf_query,
         # Mvit_udf_query, - Disabled as it requires specific pytorch package
         # Sift_udf_query, - requires package kornia
     ]
```

### Comparing `evadb-0.2.4/eva/udfs/yolo_object_detector.py` & `evadb-0.2.5/eva/udfs/yolo_object_detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/utils/__init__.py` & `evadb-0.2.5/eva/models/catalog/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""general eva utils"""
```

### Comparing `evadb-0.2.4/eva/utils/errors.py` & `evadb-0.2.5/test/udfs/ndarray/test_array_count.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,21 +8,18 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-class CatalogError(Exception):
-    pass
+import unittest
 
+from eva.udfs.ndarray.array_count import ArrayCount
 
-class UDFIODefinitionError(Exception):
-    pass
 
+class CropTests(unittest.TestCase):
+    def setUp(self):
+        self.array_count = ArrayCount()
 
-class DatasetFileNotFoundError(Exception):
-    def __init__(
-        self,
-        message="The dataset file could not be found. Please verify that the file exists in the specified path.",
-    ):
-        super().__init__(message)
+    def test_array_count_name_exists(self):
+        assert hasattr(self.array_count, "name")
```

### Comparing `evadb-0.2.4/eva/utils/generic_utils.py` & `evadb-0.2.5/eva/utils/generic_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -52,14 +52,15 @@
 
     Arguments:
         class_path (str): absolute path of import
 
     Returns:
         type: A Class for given path
     """
+    assert class_path is not None, "Class path is not found"
     module_path, class_name = class_path.rsplit(".", 1)
     module = importlib.import_module(module_path)
     return getattr(module, class_name)
 
 
 def load_udf_class_from_file(filepath, classname=None):
     """
@@ -111,25 +112,14 @@
         import torch
 
         return torch.cuda.is_available()
     except ImportError:
         return False
 
 
-def prefix_xdist_worker_id_to_path(path: str):
-    try:
-        worker_id = os.environ["PYTEST_XDIST_WORKER"]
-        base = "eva_datasets"
-        path = "build/" + str(worker_id) + "_" + base
-    except KeyError:
-        # Single threaded mode
-        pass
-    return path
-
-
 def get_gpu_count() -> int:
     """
     Check number of GPUs through Torch.
     """
     try:
         import torch
 
@@ -150,15 +140,14 @@
 
     """
     dataset_location = ConfigurationManager().get_value("core", "datasets_dir")
     if dataset_location is None:
         logger.error("Missing dataset location key in eva.yml")
         raise KeyError("Missing datasets_dir key in eva.yml")
 
-    dataset_location = prefix_xdist_worker_id_to_path(dataset_location)
     dataset_location = Path(dataset_location)
     dataset_location.mkdir(parents=True, exist_ok=True)
 
     salt = uuid.uuid4().hex
     file_name = hashlib.md5(salt.encode() + name.encode()).hexdigest()
     path = dataset_location / file_name
     return path.resolve()
```

### Comparing `evadb-0.2.4/eva/utils/kv_cache.py` & `evadb-0.2.5/eva/utils/kv_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/utils/logging_manager.py` & `evadb-0.2.5/eva/utils/logging_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/utils/math_utils.py` & `evadb-0.2.5/eva/utils/math_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/utils/s3_utils.py` & `evadb-0.2.5/eva/utils/s3_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/eva/utils/stats.py` & `evadb-0.2.5/eva/utils/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/evadb.egg-info/PKG-INFO` & `evadb-0.2.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,251 +1,228 @@
-Metadata-Version: 2.1
-Name: evadb
-Version: 0.2.4
-Summary: EVA AI-Relational Database System
-Home-page: https://github.com/georgia-tech-db/eva
-Author: Georgia Tech Database Group
-Author-email: arulraj@gatech.edu
-License: Apache License 2.0
-Download-URL: https://github.com/georgia-tech-db/eva
-Description: <div >
-          <a href="https://evadb.readthedocs.io/">
-            <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-banner.png" alt="EVA" width="1000px" margin-left="-5px">
-          </a>
-        </div>
-        
-        # EVA AI-Relational Database System
-        
-        <div>
-                <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
-                    <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EVA on Colab"/>
-                </a>
-                <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
-                    <img alt="Slack" src="https://img.shields.io/badge/slack-eva-ff69b4.svg?logo=slack">
-                </a>          
-                <img alt="PyPI" src="https://img.shields.io/pypi/v/evadb.svg"/>
-                <img alt="License" src="https://img.shields.io/badge/license-Apache%202-brightgreen.svg?logo=apache"/>
-                <img alt="Coverage Status" src="https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master"/>     
-                <a href="https://github.com/orgs/georgia-tech-db/projects/3">
-                    <img src="https://img.shields.io/badge/eva-roadmap-ff3423" alt="Roadmap"/>
-                </a>
-                <a href="https://pepy.tech/project/evadb">
-                  <img alt="Downloads" src="https://static.pepy.tech/badge/evadb/month"/>
-                </a>
-                <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.8%20|%203.9%20|%203.10-brightgreen"/>       
-        </div>
-        
-        <p align="center"> <b><h3>EVA is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
-        
-        EVA is designed for supporting database applications that operate on both structured (tables, feature vectors) and unstructured data (videos, podcasts, PDFs, etc.) using deep learning models. It accelerates AI pipelines by 10-100x using a collection of optimizations inspired by time-tested relational database systems, including function caching, sampling, and cost-based predicate reordering. EVA supports an AI-oriented SQL-like query language tailored for analyzing unstructured data. It comes with a wide range of models for analyzing unstructured data, including models for object detection, question answering, OCR, text sentiment classification, face detection, etc. It is fully implemented in Python and licensed under the Apache license.
-        
-        ## Quick Links
-        
-        - [Features](#features)
-        - [Quick Start](#quick-start)
-        - [Documentation](#documentation)
-        - [Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
-        - [Architecture Diagram](#architecture-diagram)
-        - [Demo](#demo)
-        - [Illustrative Applications](#illustrative-applications)
-        - [Community and Support](#community-and-support)
-        - [Contributing](#contributing)
-        - [License](#license)
-        
-        ## Features
-        
-        - ð® Build simpler AI-powered applications using short SQL-like queries
-        - â¡ï¸ 10-100x faster AI pipelines using AI-centric query optimization  
-        - ð° Save money spent on GPU-driven inference
-        - ð First-class support for your custom deep learning models through user-defined functions
-        - ð¦ Built-in caching to eliminate redundant model invocations across queries
-        - â¨ï¸ First-class support for PyTorch and HuggingFace models
-        - ð Installable via pip and fully implemented in Python
-        
-        ## Demo
-        
-        Here are some illustrative EVA-backed applications (all of them are Jupyter notebooks that can be opened in Google Colab):
-        
-         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html">Using ChatGPT to ask questions based on videos</a>
-         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection</a>
-         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
-         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/11-similarity-search-for-motif-mining.html">Image Similarity Search on Reddit [FAISS + Qdrant]</a>
-         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
-         * ð® <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/07-object-segmentation-huggingface.html">Image Segmentation using Hugging Face</a>
-         * ð® <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates </a>
-         * ð® <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
-        
-        ## Documentation
-        
-        * [Detailed Documentation](https://evadb.readthedocs.io/)
-          - If you are wondering why you might need an AI-relational database system, start with the page on <a href="https://evadb.readthedocs.io/en/stable/source/overview/aidb.html">Video Database Systems</a>.
-          - The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different AI pipelines, and how you can easily extend EVA by defining an user-defined function that wraps around your custom deep learning model.
-          - The <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/index.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab to run the code.
-        * [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
-        * [Join us on Slack!](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
-        * [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
-        * [Demo](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
-        
-        ## Quick Start
-        
-        - Install EVA using the pip package manager. EVA supports Python versions >= 3.7:
-        
-        ```shell
-        pip install evadb
-        ```
-        
-        - To launch and connect to an EVA server in a Jupyter notebook, check out this [illustrative emotion analysis notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb):
-        ```shell
-        cursor = connect_to_server()
-        ```
-        
-        - Load a video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration):
-        
-        ```mysql
-        LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO TrafficVideo;
-        ```
-        
-        - That's it! You can now run queries over the loaded video:
-        
-        ```mysql
-        SELECT id, data FROM TrafficVideo WHERE id < 5;
-        ```
-        
-        - Search for frames in the video that contain a car:
-        
-        ```mysql
-        SELECT id, data FROM TrafficVideo WHERE ['car'] <@ Yolo(data).labels;
-        ```
-        | Source Video  | Query Result |
-        |---------------|--------------|
-        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
-        
-        - Search for frames in the video that contain a pedestrian and a car:
-        
-        ```mysql
-        SELECT id, data FROM TrafficVideo WHERE ['pedestrian', 'car'] <@ Yolo(data).labels;
-        ```
-        
-        - Search for frames with more than three cars:
-        
-        ```mysql
-        SELECT id, data FROM TrafficVideo WHERE ArrayCount(Yolo(data).labels, 'car') > 3;
-        ```
-        
-        - **Use your custom deep learning model in queries** with a user-defined function (UDF):
-        
-        ```mysql
-        CREATE UDF IF NOT EXISTS Yolo
-        TYPE  ultralytics
-        'model' 'yolov8m.pt';
-        ```
-        
-        - **Compose multiple models in a single query** to set up useful AI pipelines.
-        
-        ```mysql
-           -- Analyse emotions of faces in a video
-           SELECT id, bbox, EmotionDetector(Crop(data, bbox)) 
-           FROM MovieVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)  
-           WHERE id < 15;
-        ```
-        
-        - **EVA runs queries faster using its AI-centric query optimizer**. Two key optimizations are:
-        
-           ð¾ **Caching**: EVA automatically caches and reuses previous query results (especially model inference results), eliminating redundant computation and reducing query processing time.
-        
-           ð¯ **Predicate Reordering**: EVA optimizes the order in which the query predicates are evaluated (e.g., runs the faster, more selective model first), leading to faster queries and lower inference costs.
-        
-        Consider these two exploratory queries on a dataset of ð images:
-        <img align="right" style="display:inline;" width="40%" src="https://github.com/georgia-tech-db/eva/blob/master/data/assets/eva_performance_comparison.png?raw=true"></a>
-        
-        ```mysql
-          -- Query 1: Find all images of black-colored dogs
-          SELECT id, bbox FROM dogs 
-          JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) 
-          WHERE Obj.label = 'dog' 
-            AND Color(Crop(data, bbox)) = 'black'; 
-        
-          -- Query 2: Find all Great Danes that are black-colored
-          SELECT id, bbox FROM dogs 
-          JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) 
-          WHERE Obj.label = 'dog' 
-            AND DogBreedClassifier(Crop(data, bbox)) = 'great dane' 
-            AND Color(Crop(data, bbox)) = 'black';
-        ```
-        
-        By reusing the results of the first query and reordering the predicates based on the available cached inference results, EVA runs the second query **10x faster**!
-        
-        ## Architecture Diagram
-        
-        The following architecture diagram presents the critical components of the EVA database system. EVA's AI-centric Query Optimizer takes a parsed query as input and generates a query plan that is then executed by the Query Engine. The Query Engine hits multiple storage engines to retrieve the data required for efficiently running the query:
-        1. Structured data (relational database system connected via `sqlalchemy`).
-        2. Unstructured media data (on cloud buckets or local filesystem).
-        3. Vector data (vector database system).
-        
-        <img width="700" alt="Architecture Diagram" src="https://github.com/georgia-tech-db/eva/assets/5521975/01452ec9-87d9-4d27-90b2-c0b1ab29b16c">
-        
-        ## Illustrative Applications 
-        
-        ### ð® [Traffic Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html) (Object Detection Model)
-        | Source Video  | Query Result |
-        |---------------|--------------|
-        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
-        
-        ### ð® [MNIST Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image Classification Model)
-        | Source Video  | Query Result |
-        |---------------|--------------|
-        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-input.webp" width="150"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-output.webp" width="150"> |
-        
-        ### ð® [Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classification Models)
-        
-        | Source Video  | Query Result |
-        |---------------|--------------|
-        |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-input.webp" width="400"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-output.webp" width="400"> |
-        
-        ### ð® [License Plate Recognition](https://github.com/georgia-tech-db/eva-application-template) (Plate Detection + OCR Extraction Models)
-        
-        | Query Result |
-        |--------------|
-        <img alt="Query Result" src="https://github.com/georgia-tech-db/license-plate-recognition/blob/main/README_files/README_12_3.png" width="300"> |
-        
-        ### ð® [Meme Toxicity Classification](https://github.com/georgia-tech-db/toxicity-classification) (OCR Extraction + Toxicity Classification Models)
-        
-        | Query Result |
-        |--------------|
-        <img alt="Query Result" src="https://raw.githubusercontent.com/georgia-tech-db/toxicity-classification/main/README_files/README_16_2.png" width="200"> |
-        
-        ## Community and Support
-        
-        ð If you have general questions about EVA, want to say hello or just follow along, we'd like to invite you to join our [Slack Community](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg).
-        
-        <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">              
-            <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-slack.png" alt="EVA Slack Channel" width="500">
+# EVA AI-SQL Database System
+
+<div>
+        <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
+            <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EVA on Colab"/>
         </a>
-        
-        If you run into any problems or issues, please create a Github issue and we'll try our best to help.
-        
-        Don't see a feature in the list? Search our issue tracker if someone has already requested it and add a comment to it explaining your use-case, or open a new issue if not. We prioritize our roadmap based on user feedback, so we'd love to hear from you.
-        
-        ## Contributing
-        
-        [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb)
-        [![CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva)
-        [![Documentation Status](https://readthedocs.org/projects/evadb/badge/?version=stable)](https://evadb.readthedocs.io/en/stable/index.html)
-        
-        EVA is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EVA are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
-        
-        For more information, see our
-        [contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
-        
-        ## License
-        Copyright (c) 2018-present [Georgia Tech Database Group](http://db.cc.gatech.edu/).
-        Licensed under [Apache License](LICENSE).
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
+        <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
+            <img alt="Slack" src="https://img.shields.io/badge/slack-eva-ff69b4.svg?logo=slack">
+        </a>          
+        <a href="https://twitter.com/evadb_ai">
+            <img alt="Twitter" src="https://img.shields.io/badge/twitter-eva-bde1ee.svg?logo=twitter">
+        </a>  
+        <a href="https://github.com/orgs/georgia-tech-db/projects/3">
+            <img src="https://img.shields.io/badge/eva-roadmap-a6c096" alt="Roadmap"/>
+        </a>
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/evadb.svg"/>
+        <img alt="License" src="https://img.shields.io/badge/license-Apache%202-brightgreen.svg?logo=apache"/>
+        <img alt="Coverage Status" src="https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master"/>     
+        <a href="https://pepy.tech/project/evadb">
+          <img alt="Downloads" src="https://static.pepy.tech/badge/evadb/month"/>
+        </a>
+        <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.8%20|%203.9%20|%203.10-brightgreen"/>       
+</div>
+
+<p align="center"> <b><h3>EVA DB is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
+
+EVA DB is an AI-SQL database system for developing applications powered by AI models. We aim to simplify the development and deployment of AI-powered applications that operate on structured (tables, feature stores) and unstructured data (videos, text, podcasts, PDFs, etc.).
+
+EVA DB accelerates AI pipelines by 10-100x using a collection of performance optimizations inspired by time-tested SQL database systems, including data-parallel query execution, function caching, sampling, and cost-based predicate reordering. EVA supports an AI-oriented SQL-like query language tailored for analyzing both structured and unstructured data. It has first-class support for PyTorch, Hugging Face, YOLO, and Open AI models.
+
+The high-level SQL API allows even beginners to use EVA in a few lines of code. Advanced users can define custom user-defined functions that wrap around any AI model or Python library. EVA DB is fully implemented in Python and licensed under the Apache license.
+
+## Quick Links
+
+- [Features](#features)
+- [Quick Start](#quick-start)
+- [Documentation](#documentation)
+- [Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
+- [Architecture Diagram](#architecture-diagram)
+- [Illustrative Applications](#illustrative-applications)
+- [Screenshots](#screenshots)
+- [Community and Support](#community-and-support)
+- [Twitter](https://twitter.com/evadb_ai)
+- [Contributing](#contributing)
+- [License](#license)
+
+## Features
+
+- 🔮 Build simpler AI-powered applications using short SQL-like queries
+- ⚡️ 10-100x faster AI pipelines using AI-centric query optimization  
+- 💰 Save money spent on GPUs
+- 🚀 First-class support for your custom deep learning models through user-defined functions
+- 📦 Built-in caching to eliminate redundant model invocations across queries
+- ⌨️ First-class support for PyTorch, Hugging Face, YOLO, and Open AI models
+- 🐍 Installable via pip and fully implemented in Python
+
+## Illustrative Applications
+
+Here are some illustrative EVA-powered applications (each Jupyter notebook can be opened on Google Colab):
+
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html">Using ChatGPT to ask questions based on videos</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/11-similarity-search-for-motif-mining.html">Image Similarity Search on Reddit [FAISS + Qdrant]</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/07-object-segmentation-huggingface.html">Image Segmentation using Hugging Face</a>
+ * 🔮 <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates </a>
+ * 🔮 <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
+
+## Documentation
+
+* [Detailed Documentation](https://evadb.readthedocs.io/)
+  - The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different AI tasks and how you can easily extend EVA to support your custom deep learning model through user-defined functions.
+  - The <a href="https://evadb.readthedocs.io/en/latest/source/tutorials/11-similarity-search-for-motif-mining.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab, where you can run the code yourself.
+* [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
+* [Join us on Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
+* [Follow us on Twitter](https://twitter.com/evadb_ai)
+* [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
+* [Demo](https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html)
+
+## Quick Start
+
+- Install EVA using the pip package manager. EVA supports Python versions >= 3.8:
+
+```shell
+pip install evadb
+```
+
+- To launch and connect to an EVA server in a Jupyter notebook, check out this [illustrative emotion analysis notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb):
+```shell
+cursor = connect_to_server()
+```
+
+- Load a video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration):
+
+```mysql
+LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO TrafficVideo;
+```
+
+- That's it! You can now run queries over the loaded video:
+
+```mysql
+SELECT id, data FROM TrafficVideo WHERE id < 5;
+```
+
+- Search for frames in the video that contain a car:
+
+```mysql
+SELECT id, data FROM TrafficVideo WHERE ['car'] <@ Yolo(data).labels;
+```
+| Source Video  | Query Result |
+|---------------|--------------|
+|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
+
+- Search for frames in the video that contain a pedestrian and a car:
+
+```mysql
+SELECT id, data FROM TrafficVideo WHERE ['pedestrian', 'car'] <@ Yolo(data).labels;
+```
+
+- Search for frames with more than three cars:
+
+```mysql
+SELECT id, data FROM TrafficVideo WHERE ArrayCount(Yolo(data).labels, 'car') > 3;
+```
+
+- **Use your custom deep learning model in queries** with a user-defined function (UDF):
+
+```mysql
+CREATE UDF IF NOT EXISTS Yolo
+TYPE  ultralytics
+'model' 'yolov8m.pt';
+```
+
+- **Chain multiple models in a single query** to set up useful AI pipelines.
+
+```mysql
+   -- Analyse emotions of faces in a video
+   SELECT id, bbox, EmotionDetector(Crop(data, bbox)) 
+   FROM MovieVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)  
+   WHERE id < 15;
+```
+
+- **EVA runs queries faster using its AI-centric query optimizer**. Two key optimizations are:
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
+  JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) 
+  WHERE Obj.label = 'dog' 
+    AND Color(Crop(data, bbox)) = 'black'; 
+
+  -- Query 2: Find all Great Danes that are black-colored
+  SELECT id, bbox FROM dogs 
+  JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) 
+  WHERE Obj.label = 'dog' 
+    AND DogBreedClassifier(Crop(data, bbox)) = 'great dane' 
+    AND Color(Crop(data, bbox)) = 'black';
+```
+
+By reusing the results of the first query and reordering the predicates based on the available cached inference results, EVA runs the second query **10x faster**!
+
+## Architecture Diagram
+
+This diagram presents the key components of EVA DB. EVA's AI-centric Query Optimizer takes a parsed query as input and generates a query plan that is then executed by the Query Engine. The Query Engine hits multiple storage engines to retrieve the data required for efficiently running the query:
+1. Structured data (SQL database system connected via `sqlalchemy`).
+2. Unstructured media data (on cloud buckets or local filesystem).
+3. Vector data (vector database system).
+
+<img width="700" alt="Architecture Diagram" src="https://github.com/georgia-tech-db/eva/assets/5521975/01452ec9-87d9-4d27-90b2-c0b1ab29b16c">
+
+## Screenshots
+
+### 🔮 [Traffic Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html) (Object Detection Model)
+| Source Video  | Query Result |
+|---------------|--------------|
+|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
+
+### 🔮 [MNIST Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image Classification Model)
+| Source Video  | Query Result |
+|---------------|--------------|
+|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-input.webp" width="150"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-output.webp" width="150"> |
+
+### 🔮 [Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classification Models)
+
+| Source Video  | Query Result |
+|---------------|--------------|
+|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-input.webp" width="400"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/gangubai-output.webp" width="400"> |
+
+### 🔮 [License Plate Recognition](https://github.com/georgia-tech-db/eva-application-template) (Plate Detection + OCR Extraction Models)
+
+| Query Result |
+|--------------|
+<img alt="Query Result" src="https://github.com/georgia-tech-db/license-plate-recognition/blob/main/README_files/README_12_3.png" width="300"> |
+
+## Community and Support
+
+👋 If you have general questions about EVA, want to say hello or just follow along, we'd like to invite you to join our [Slack Community](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)and to [follow us on Twitter](https://twitter.com/evadb_ai).
+
+<a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">              
+    <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-slack.png" alt="EVA Slack Channel" width="500">
+</a>
+
+If you run into any problems or issues, please create a Github issue and we'll try our best to help.
+
+Don't see a feature in the list? Search our issue tracker if someone has already requested it and add a comment to it explaining your use-case, or open a new issue if not. We prioritize our [roadmap](https://github.com/orgs/georgia-tech-db/projects/3) based on user feedback, so we'd love to hear from you.
+
+## Contributing
+
+[![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb)
+[![CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva)
+[![Documentation Status](https://readthedocs.org/projects/evadb/badge/?version=latest)](https://evadb.readthedocs.io/en/latest/index.html)
+
+EVA is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EVA are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
+
+For more information, see our
+[contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
+
+## License
+Copyright (c) 2018-present [Georgia Tech Database Group](http://db.cc.gatech.edu/).
+Licensed under [Apache License](LICENSE).
```

#### html2text {}

```diff
@@ -1,140 +1,129 @@
-Metadata-Version: 2.1 Name: evadb Version: 0.2.4 Summary: EVA AI-Relational
-Database System Home-page: https://github.com/georgia-tech-db/eva Author:
-Georgia Tech Database Group Author-email: arulraj@gatech.edu License: Apache
-License 2.0 Download-URL: https://github.com/georgia-tech-db/eva Description:
-[EVA]
-# EVA AI-Relational Database System
-[Open_EVA_on_Colab] [Slack] [PyPI] [License] [Coverage Status] [Roadmap]
-[Downloads] [Python Versions]
-**** EVA is a database system for building simpler and faster AI-powered
+# EVA AI-SQL Database System
+[Open_EVA_on_Colab] [Slack] [Twitter] [Roadmap] [PyPI] [License] [Coverage
+Status] [Downloads] [Python Versions]
+**** EVA DB is a database system for building simpler and faster AI-powered
 applications. ****
-EVA is designed for supporting database applications that operate on both
-structured (tables, feature vectors) and unstructured data (videos, podcasts,
-PDFs, etc.) using deep learning models. It accelerates AI pipelines by 10-100x
-using a collection of optimizations inspired by time-tested relational database
-systems, including function caching, sampling, and cost-based predicate
-reordering. EVA supports an AI-oriented SQL-like query language tailored for
-analyzing unstructured data. It comes with a wide range of models for analyzing
-unstructured data, including models for object detection, question answering,
-OCR, text sentiment classification, face detection, etc. It is fully
+EVA DB is an AI-SQL database system for developing applications powered by AI
+models. We aim to simplify the development and deployment of AI-powered
+applications that operate on structured (tables, feature stores) and
+unstructured data (videos, text, podcasts, PDFs, etc.). EVA DB accelerates AI
+pipelines by 10-100x using a collection of performance optimizations inspired
+by time-tested SQL database systems, including data-parallel query execution,
+function caching, sampling, and cost-based predicate reordering. EVA supports
+an AI-oriented SQL-like query language tailored for analyzing both structured
+and unstructured data. It has first-class support for PyTorch, Hugging Face,
+YOLO, and Open AI models. The high-level SQL API allows even beginners to use
+EVA in a few lines of code. Advanced users can define custom user-defined
+functions that wrap around any AI model or Python library. EVA DB is fully
 implemented in Python and licensed under the Apache license. ## Quick Links -
 [Features](#features) - [Quick Start](#quick-start) - [Documentation]
 (#documentation) - [Roadmap](https://github.com/orgs/georgia-tech-db/projects/
-3) - [Architecture Diagram](#architecture-diagram) - [Demo](#demo) -
-[Illustrative Applications](#illustrative-applications) - [Community and
-Support](#community-and-support) - [Contributing](#contributing) - [License]
-(#license) ## Features - Ã°ÂÂÂ® Build simpler AI-powered applications using
-short SQL-like queries - Ã¢ÂÂ¡Ã¯Â¸Â 10-100x faster AI pipelines using AI-
-centric query optimization - Ã°ÂÂÂ° Save money spent on GPU-driven inference
-- Ã°ÂÂÂ First-class support for your custom deep learning models through
-user-defined functions - Ã°ÂÂÂ¦ Built-in caching to eliminate redundant model
-invocations across queries - Ã¢ÂÂ¨Ã¯Â¸Â First-class support for PyTorch and
-HuggingFace models - Ã°ÂÂÂ Installable via pip and fully implemented in
-Python ## Demo Here are some illustrative EVA-backed applications (all of them
-are Jupyter notebooks that can be opened in Google Colab): * Ã°ÂÂÂ® Using
-ChatGPT_to_ask_questions_based_on_videos * Ã°ÂÂÂ® Analysing_traffic_flow_at
-an_intersection * Ã°ÂÂÂ® Examining_the_emotion_palette_of_actors_in_a_movie *
-Ã°ÂÂÂ® Image_Similarity_Search_on_Reddit_[FAISS_+_Qdrant] * Ã°ÂÂÂ®
-Classifying_images_based_on_their_content * Ã°ÂÂÂ® Image_Segmentation_using
-Hugging_Face * Ã°ÂÂÂ® Recognizing_license_plates * Ã°ÂÂÂ® Analysing
-toxicity_of_social_media_memes ## Documentation * [Detailed Documentation]
-(https://evadb.readthedocs.io/) - If you are wondering why you might need an
-AI-relational database system, start with the page on Video_Database_Systems. -
-The Getting_Started page shows how you can use EVA for different AI pipelines,
-and how you can easily extend EVA by defining an user-defined function that
-wraps around your custom deep learning model. - The User_Guides section
-contains Jupyter Notebooks that demonstrate how to use various features of EVA.
-Each notebook includes a link to Google Colab to run the code. * [Tutorials]
-(https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-
-analysis.ipynb) * [Join us on Slack!](https://join.slack.com/t/eva-db/
-shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Medium-Term Roadmap]
-(https://github.com/orgs/georgia-tech-db/projects/3) * [Demo](https://
+3) - [Architecture Diagram](#architecture-diagram) - [Illustrative
+Applications](#illustrative-applications) - [Screenshots](#screenshots) -
+[Community and Support](#community-and-support) - [Twitter](https://
+twitter.com/evadb_ai) - [Contributing](#contributing) - [License](#license) ##
+Features - ð® Build simpler AI-powered applications using short SQL-like
+queries - â¡ï¸ 10-100x faster AI pipelines using AI-centric query
+optimization - ð° Save money spent on GPUs - ð First-class support for
+your custom deep learning models through user-defined functions - ð¦ Built-in
+caching to eliminate redundant model invocations across queries - â¨ï¸ First-
+class support for PyTorch, Hugging Face, YOLO, and Open AI models - ð
+Installable via pip and fully implemented in Python ## Illustrative
+Applications Here are some illustrative EVA-powered applications (each Jupyter
+notebook can be opened on Google Colab): * ð® Using_ChatGPT_to_ask_questions
+based_on_videos * ð® Analysing_traffic_flow_at_an_intersection * ð®
+Examining_the_emotion_palette_of_actors_in_a_movie * ð® Image_Similarity
+Search_on_Reddit_[FAISS_+_Qdrant] * ð® Classifying_images_based_on_their
+content * ð® Image_Segmentation_using_Hugging_Face * ð® Recognizing_license
+plates * ð® Analysing_toxicity_of_social_media_memes ## Documentation *
+[Detailed Documentation](https://evadb.readthedocs.io/) - The Getting_Started
+page shows how you can use EVA for different AI tasks and how you can easily
+extend EVA to support your custom deep learning model through user-defined
+functions. - The User_Guides section contains Jupyter Notebooks that
+demonstrate how to use various features of EVA. Each notebook includes a link
+to Google Colab, where you can run the code yourself. * [Tutorials](https://
 github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
-## Quick Start - Install EVA using the pip package manager. EVA supports Python
-versions >= 3.7: ```shell pip install evadb ``` - To launch and connect to an
-EVA server in a Jupyter notebook, check out this [illustrative emotion analysis
-notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-
-emotion-analysis.ipynb): ```shell cursor = connect_to_server() ``` - Load a
-video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4)
-for illustration): ```mysql LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO
-TrafficVideo; ``` - That's it! You can now run queries over the loaded video:
-```mysql SELECT id, data FROM TrafficVideo WHERE id < 5; ``` - Search for
-frames in the video that contain a car: ```mysql SELECT id, data FROM
-TrafficVideo WHERE ['car'] <@ Yolo(data).labels; ``` | Source Video | Query
-Result | |---------------|--------------| |[Source Video] |[Query Result] | -
-Search for frames in the video that contain a pedestrian and a car: ```mysql
-SELECT id, data FROM TrafficVideo WHERE ['pedestrian', 'car'] <@ Yolo
-(data).labels; ``` - Search for frames with more than three cars: ```mysql
-SELECT id, data FROM TrafficVideo WHERE ArrayCount(Yolo(data).labels, 'car') >
-3; ``` - **Use your custom deep learning model in queries** with a user-defined
-function (UDF): ```mysql CREATE UDF IF NOT EXISTS Yolo TYPE ultralytics 'model'
-'yolov8m.pt'; ``` - **Compose multiple models in a single query** to set up
-useful AI pipelines. ```mysql -- Analyse emotions of faces in a video SELECT
-id, bbox, EmotionDetector(Crop(data, bbox)) FROM MovieVideo JOIN LATERAL UNNEST
-(FaceDetector(data)) AS Face(bbox, conf) WHERE id < 15; ``` - **EVA runs
-queries faster using its AI-centric query optimizer**. Two key optimizations
-are: Ã°ÂÂÂ¾ **Caching**: EVA automatically caches and reuses previous query
-results (especially model inference results), eliminating redundant computation
-and reducing query processing time. Ã°ÂÂÂ¯ **Predicate Reordering**: EVA
-optimizes the order in which the query predicates are evaluated (e.g., runs the
-faster, more selective model first), leading to faster queries and lower
-inference costs. Consider these two exploratory queries on a dataset of
-Ã°ÂÂÂ images: [https://github.com/georgia-tech-db/eva/blob/master/data/
-assets/eva_performance_comparison.png?raw=true]
+* [Join us on Slack](https://join.slack.com/t/eva-db/shared_invite/zt-
+1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Follow us on Twitter](https://twitter.com/
+evadb_ai) * [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/
+projects/3) * [Demo](https://evadb.readthedocs.io/en/stable/source/tutorials/
+08-chatgpt.html) ## Quick Start - Install EVA using the pip package manager.
+EVA supports Python versions >= 3.8: ```shell pip install evadb ``` - To launch
+and connect to an EVA server in a Jupyter notebook, check out this
+[illustrative emotion analysis notebook](https://github.com/georgia-tech-db/
+eva/blob/master/tutorials/03-emotion-analysis.ipynb): ```shell cursor =
+connect_to_server() ``` - Load a video onto the EVA server (we use
+[ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration): ```mysql LOAD
+VIDEO "data/ua_detrac/ua_detrac.mp4" INTO TrafficVideo; ``` - That's it! You
+can now run queries over the loaded video: ```mysql SELECT id, data FROM
+TrafficVideo WHERE id < 5; ``` - Search for frames in the video that contain a
+car: ```mysql SELECT id, data FROM TrafficVideo WHERE ['car'] <@ Yolo
+(data).labels; ``` | Source Video | Query Result | |---------------|-----------
+---| |[Source Video] |[Query Result] | - Search for frames in the video that
+contain a pedestrian and a car: ```mysql SELECT id, data FROM TrafficVideo
+WHERE ['pedestrian', 'car'] <@ Yolo(data).labels; ``` - Search for frames with
+more than three cars: ```mysql SELECT id, data FROM TrafficVideo WHERE
+ArrayCount(Yolo(data).labels, 'car') > 3; ``` - **Use your custom deep learning
+model in queries** with a user-defined function (UDF): ```mysql CREATE UDF IF
+NOT EXISTS Yolo TYPE ultralytics 'model' 'yolov8m.pt'; ``` - **Chain multiple
+models in a single query** to set up useful AI pipelines. ```mysql -- Analyse
+emotions of faces in a video SELECT id, bbox, EmotionDetector(Crop(data, bbox))
+FROM MovieVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)
+WHERE id < 15; ``` - **EVA runs queries faster using its AI-centric query
+optimizer**. Two key optimizations are: ð¾ **Caching**: EVA automatically
+caches and reuses previous query results (especially model inference results),
+eliminating redundant computation and reducing query processing time. ð¯
+**Predicate Reordering**: EVA optimizes the order in which the query predicates
+are evaluated (e.g., runs the faster, more selective model first), leading to
+faster queries and lower inference costs. Consider these two exploratory
+queries on a dataset of dog images: [https://github.com/georgia-tech-db/eva/
+blob/master/data/assets/eva_performance_comparison.png?raw=true]
  ```mysql -- Query 1: Find all images of black-colored dogs SELECT id, bbox
 FROM dogs JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) WHERE
 Obj.label = 'dog' AND Color(Crop(data, bbox)) = 'black'; -- Query 2: Find all
 Great Danes that are black-colored SELECT id, bbox FROM dogs JOIN LATERAL
 UNNEST(Yolo(data)) AS Obj(label, bbox, score) WHERE Obj.label = 'dog' AND
 DogBreedClassifier(Crop(data, bbox)) = 'great dane' AND Color(Crop(data, bbox))
 = 'black'; ``` By reusing the results of the first query and reordering the
 predicates based on the available cached inference results, EVA runs the second
-query **10x faster**! ## Architecture Diagram The following architecture
-diagram presents the critical components of the EVA database system. EVA's AI-
-centric Query Optimizer takes a parsed query as input and generates a query
-plan that is then executed by the Query Engine. The Query Engine hits multiple
-storage engines to retrieve the data required for efficiently running the
-query: 1. Structured data (relational database system connected via
-`sqlalchemy`). 2. Unstructured media data (on cloud buckets or local
-filesystem). 3. Vector data (vector database system). [Architecture Diagram] ##
-Illustrative Applications ### Ã°ÂÂÂ® [Traffic Analysis](https://
+query **10x faster**! ## Architecture Diagram This diagram presents the key
+components of EVA DB. EVA's AI-centric Query Optimizer takes a parsed query as
+input and generates a query plan that is then executed by the Query Engine. The
+Query Engine hits multiple storage engines to retrieve the data required for
+efficiently running the query: 1. Structured data (SQL database system
+connected via `sqlalchemy`). 2. Unstructured media data (on cloud buckets or
+local filesystem). 3. Vector data (vector database system). [Architecture
+Diagram] ## Screenshots ### ð® [Traffic Analysis](https://
 evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html)
 (Object Detection Model) | Source Video | Query Result | |---------------|-----
----------| |[Source Video] |[Query Result] | ### Ã°ÂÂÂ® [MNIST Digit
-Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-
-mnist.html) (Image Classification Model) | Source Video | Query Result | |-----
-----------|--------------| |[Source Video] |[Query Result] | ### Ã°ÂÂÂ®
-[Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/
-tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classification
-Models) | Source Video | Query Result | |---------------|--------------| |
-[Source Video] |[Query Result] | ### Ã°ÂÂÂ® [License Plate Recognition]
-(https://github.com/georgia-tech-db/eva-application-template) (Plate Detection
-+ OCR Extraction Models) | Query Result | |--------------| [Query Result] | ###
-Ã°ÂÂÂ® [Meme Toxicity Classification](https://github.com/georgia-tech-db/
-toxicity-classification) (OCR Extraction + Toxicity Classification Models) |
-Query Result | |--------------| [Query Result] | ## Community and Support
-Ã°ÂÂÂ If you have general questions about EVA, want to say hello or just
-follow along, we'd like to invite you to join our [Slack Community](https://
-join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg).
-[EVA_Slack_Channel] If you run into any problems or issues, please create a
-Github issue and we'll try our best to help. Don't see a feature in the list?
-Search our issue tracker if someone has already requested it and add a comment
-to it explaining your use-case, or open a new issue if not. We prioritize our
-roadmap based on user feedback, so we'd love to hear from you. ## Contributing
-[![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/
-project/evadb) [![CI Status](https://circleci.com/gh/georgia-tech-db/
-eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva) [!
+---------| |[Source Video] |[Query Result] | ### ð® [MNIST Digit Recognition]
+(https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image
+Classification Model) | Source Video | Query Result | |---------------|--------
+------| |[Source Video] |[Query Result] | ### ð® [Movie Emotion Analysis]
+(https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-
+analysis.html) (Face Detection + Emotion Classification Models) | Source Video
+| Query Result | |---------------|--------------| |[Source Video] |[Query
+Result] | ### ð® [License Plate Recognition](https://github.com/georgia-tech-
+db/eva-application-template) (Plate Detection + OCR Extraction Models) | Query
+Result | |--------------| [Query Result] | ## Community and Support ð If you
+have general questions about EVA, want to say hello or just follow along, we'd
+like to invite you to join our [Slack Community](https://join.slack.com/t/eva-
+db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)and to [follow us on
+Twitter](https://twitter.com/evadb_ai). [EVA_Slack_Channel] If you run into any
+problems or issues, please create a Github issue and we'll try our best to
+help. Don't see a feature in the list? Search our issue tracker if someone has
+already requested it and add a comment to it explaining your use-case, or open
+a new issue if not. We prioritize our [roadmap](https://github.com/orgs/
+georgia-tech-db/projects/3) based on user feedback, so we'd love to hear from
+you. ## Contributing [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)]
+(https://pypi.org/project/evadb) [![CI Status](https://circleci.com/gh/georgia-
+tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva) [!
 [Documentation Status](https://readthedocs.org/projects/evadb/badge/
-?version=stable)](https://evadb.readthedocs.io/en/stable/index.html) EVA is the
+?version=latest)](https://evadb.readthedocs.io/en/latest/index.html) EVA is the
 beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/
 graphs/contributors). All kinds of contributions to EVA are appreciated. To
 file a bug or to request a feature, please use GitHub_issues. Pull_requests are
 welcome. For more information, see our [contribution guide](https://
 evadb.readthedocs.io/en/stable/source/contribute/index.html). ## License
 Copyright (c) 2018-present [Georgia Tech Database Group](http://
-db.cc.gatech.edu/). Licensed under [Apache License](LICENSE). Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
-OSI Approved :: Apache Software License Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: dev
+db.cc.gatech.edu/). Licensed under [Apache License](LICENSE).
```

### Comparing `evadb-0.2.4/evadb.egg-info/SOURCES.txt` & `evadb-0.2.5/evadb.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 eva/executor/create_executor.py
 eva/executor/create_index_executor.py
 eva/executor/create_mat_view_executor.py
 eva/executor/create_udf_executor.py
 eva/executor/delete_executor.py
 eva/executor/drop_executor.py
 eva/executor/drop_udf_executor.py
+eva/executor/exchange_executor.py
 eva/executor/execution_context.py
 eva/executor/executor_utils.py
 eva/executor/explain_executor.py
 eva/executor/function_scan_executor.py
 eva/executor/groupby_executor.py
 eva/executor/hash_join_executor.py
 eva/executor/insert_executor.py
@@ -68,41 +69,37 @@
 eva/executor/load_multimedia_executor.py
 eva/executor/nested_loop_join_executor.py
 eva/executor/orderby_executor.py
 eva/executor/plan_executor.py
 eva/executor/pp_executor.py
 eva/executor/predicate_executor.py
 eva/executor/project_executor.py
+eva/executor/ray_utils.py
 eva/executor/rename_executor.py
 eva/executor/sample_executor.py
 eva/executor/seq_scan_executor.py
 eva/executor/show_info_executor.py
 eva/executor/storage_executor.py
 eva/executor/union_executor.py
 eva/executor/vector_index_scan_executor.py
-eva/experimental/__init__.py
-eva/experimental/ray/__init__.py
-eva/experimental/ray/executor/__init__.py
-eva/experimental/ray/executor/exchange_executor.py
-eva/experimental/ray/executor/ray_stage.py
-eva/experimental/ray/optimizer/__init__.py
-eva/experimental/ray/optimizer/rules/__init__.py
-eva/experimental/ray/optimizer/rules/rules.py
-eva/experimental/ray/planner/__init__.py
-eva/experimental/ray/planner/exchange_plan.py
 eva/expression/__init__.py
 eva/expression/abstract_expression.py
 eva/expression/aggregation_expression.py
 eva/expression/arithmetic_expression.py
 eva/expression/comparison_expression.py
 eva/expression/constant_value_expression.py
 eva/expression/expression_utils.py
 eva/expression/function_expression.py
 eva/expression/logical_expression.py
 eva/expression/tuple_value_expression.py
+eva/interfaces/__init__.py
+eva/interfaces/relational/__init__.py
+eva/interfaces/relational/db.py
+eva/interfaces/relational/relation.py
+eva/interfaces/relational/utils.py
 eva/models/__init__.py
 eva/models/catalog/__init__.py
 eva/models/catalog/frame_info.py
 eva/models/catalog/properties.py
 eva/models/server/__init__.py
 eva/models/server/response.py
 eva/models/storage/__init__.py
@@ -143,14 +140,15 @@
 eva/parser/parser.py
 eva/parser/rename_statement.py
 eva/parser/select_statement.py
 eva/parser/show_statement.py
 eva/parser/statement.py
 eva/parser/table_ref.py
 eva/parser/types.py
+eva/parser/utils.py
 eva/parser/lark_visitor/__init__.py
 eva/parser/lark_visitor/_common_clauses_ids.py
 eva/parser/lark_visitor/_create_statements.py
 eva/parser/lark_visitor/_delete_statement.py
 eva/parser/lark_visitor/_drop_statement.py
 eva/parser/lark_visitor/_explain_statement.py
 eva/parser/lark_visitor/_expressions.py
@@ -169,14 +167,15 @@
 eva/plan_nodes/create_index_plan.py
 eva/plan_nodes/create_mat_view_plan.py
 eva/plan_nodes/create_plan.py
 eva/plan_nodes/create_udf_plan.py
 eva/plan_nodes/delete_plan.py
 eva/plan_nodes/drop_plan.py
 eva/plan_nodes/drop_udf_plan.py
+eva/plan_nodes/exchange_plan.py
 eva/plan_nodes/explain_plan.py
 eva/plan_nodes/function_scan_plan.py
 eva/plan_nodes/groupby_plan.py
 eva/plan_nodes/hash_join_build_plan.py
 eva/plan_nodes/hash_join_probe_plan.py
 eva/plan_nodes/insert_plan.py
 eva/plan_nodes/lateral_join_plan.py
@@ -195,25 +194,30 @@
 eva/plan_nodes/types.py
 eva/plan_nodes/union_plan.py
 eva/plan_nodes/vector_index_scan_plan.py
 eva/readers/__init__.py
 eva/readers/abstract_reader.py
 eva/readers/csv_reader.py
 eva/readers/decord_reader.py
+eva/readers/pdf_reader.py
+eva/readers/document/__init__.py
+eva/readers/document/document_reader.py
+eva/readers/document/registry.py
 eva/readers/image/__init__.py
 eva/readers/image/opencv_image_reader.py
 eva/server/__init__.py
 eva/server/command_handler.py
-eva/server/db_api.py
 eva/server/interpreter.py
 eva/server/server.py
 eva/storage/__init__.py
 eva/storage/abstract_media_storage_engine.py
 eva/storage/abstract_storage_engine.py
+eva/storage/document_storage_engine.py
 eva/storage/image_storage_engine.py
+eva/storage/pdf_storage_engine.py
 eva/storage/sqlite_storage_engine.py
 eva/storage/storage_engine.py
 eva/storage/video_storage_engine.py
 eva/third_party/__init__.py
 eva/third_party/huggingface/__init__.py
 eva/third_party/huggingface/binder.py
 eva/third_party/huggingface/create.py
@@ -227,14 +231,15 @@
 eva/udfs/asl_action_recognition.py
 eva/udfs/chatgpt.py
 eva/udfs/emotion_detector.py
 eva/udfs/face_detector.py
 eva/udfs/fastrcnn_object_detector.py
 eva/udfs/feature_extractor.py
 eva/udfs/gpu_compatible.py
+eva/udfs/mnist_image_classifier.py
 eva/udfs/mvit_action_recognition.py
 eva/udfs/ocr_extractor.py
 eva/udfs/sift_feature_extractor.py
 eva/udfs/udf_bootstrap_queries.py
 eva/udfs/yolo_object_detector.py
 eva/udfs/abstract/__init__.py
 eva/udfs/abstract/abstract_udf.py
@@ -244,21 +249,27 @@
 eva/udfs/decorators/__init__.py
 eva/udfs/decorators/decorators.py
 eva/udfs/decorators/utils.py
 eva/udfs/decorators/io_descriptors/__init__.py
 eva/udfs/decorators/io_descriptors/abstract_types.py
 eva/udfs/decorators/io_descriptors/data_types.py
 eva/udfs/ndarray/__init__.py
+eva/udfs/ndarray/annotate.py
 eva/udfs/ndarray/array_count.py
 eva/udfs/ndarray/crop.py
 eva/udfs/ndarray/fuzzy_join.py
+eva/udfs/ndarray/gaussian_blur.py
+eva/udfs/ndarray/horizontal_flip.py
 eva/udfs/ndarray/open.py
 eva/udfs/ndarray/similarity.py
+eva/udfs/ndarray/to_grayscale.py
+eva/udfs/ndarray/vertical_flip.py
 eva/udfs/trackers/__init__.py
 eva/udfs/trackers/nor_fair.py
+eva/udfs/tutorials/__init__.py
 eva/utils/__init__.py
 eva/utils/errors.py
 eva/utils/generic_utils.py
 eva/utils/kv_cache.py
 eva/utils/logging_manager.py
 eva/utils/math_utils.py
 eva/utils/s3_utils.py
@@ -296,15 +307,14 @@
 test/catalog/services/test_udf_cost_catalog_service.py
 test/catalog/services/test_udf_io_catalog_service.py
 test/configuration/__init__.py
 test/configuration/test_bootstrap_environment.py
 test/configuration/test_configuration_manager.py
 test/executor/__init__.py
 test/executor/test_abstract_executor.py
-test/executor/test_create_mat_executor.py
 test/executor/test_create_udf_executor.py
 test/executor/test_execution_context.py
 test/executor/test_executor_utils.py
 test/executor/test_limit_executor.py
 test/executor/test_load_executor.py
 test/executor/test_orderby_executor.py
 test/executor/test_plan_executor.py
@@ -331,14 +341,15 @@
 test/integration_tests/test_error_handling_with_ray.py
 test/integration_tests/test_explain_executor.py
 test/integration_tests/test_fuzzy_join.py
 test/integration_tests/test_huggingface_udfs.py
 test/integration_tests/test_insert_executor.py
 test/integration_tests/test_like.py
 test/integration_tests/test_load_executor.py
+test/integration_tests/test_load_pdf_executor.py
 test/integration_tests/test_mat_executor.py
 test/integration_tests/test_open.py
 test/integration_tests/test_optimizer_rules.py
 test/integration_tests/test_pytorch.py
 test/integration_tests/test_rename_executor.py
 test/integration_tests/test_reuse.py
 test/integration_tests/test_s3_load_executor.py
@@ -386,15 +397,19 @@
 test/udfs/test_fastrcnn_object_detector.py
 test/udfs/test_yolo_object_detector.py
 test/udfs/decorators/__init__.py
 test/udfs/decorators/test_decorators.py
 test/udfs/decorators/io_descriptors/__init__.py
 test/udfs/decorators/io_descriptors/test_descriptors.py
 test/udfs/ndarray/__init__.py
+test/udfs/ndarray/test_annotate.py
 test/udfs/ndarray/test_array_count.py
 test/udfs/ndarray/test_crop.py
+test/udfs/ndarray/test_flips.py
+test/udfs/ndarray/test_gaussian_blur.py
 test/udfs/ndarray/test_open.py
+test/udfs/ndarray/test_to_grayscale.py
 test/utils/__init__.py
 test/utils/test_generic_utils.py
 test/utils/test_timer.py
 test/utils/test_xdist.py
 third_party/__init__.py
```

### Comparing `evadb-0.2.4/evadb.egg-info/requires.txt` & `evadb-0.2.5/evadb.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,86 @@
+numpy>=1.19.5
+pandas>=1.1.5
+opencv-contrib-python-headless>=4.6.0.66
 Pillow>=8.4.0
+sqlalchemy<2.0.0,>=1.4.0
+sqlalchemy-utils>=0.36.6
+lark>=1.0.0
+pyyaml>=5.1
+importlib-metadata<5.0
+ray>=1.13.0
 aenum>=2.2.0
-boto3
 diskcache>=5.4.0
 eva-decord>=0.6.1
-facenet-pytorch>=2.5.2
+boto3
+nest_asyncio
+langchain
+pymupdf
+pdfminer.six
+torch>=1.10.0
+torchvision>=0.11.1
 faiss-cpu
-importlib-metadata<5.0
+facenet-pytorch>=2.5.2
 ipython<8.13.0
-lark>=1.0.0
-nest_asyncio
+thefuzz
+ultralytics>=8.0.93
+transformers>=4.27.4
+openai>=0.27.4
+timm>=0.6.13
 norfair>=2.2.0
+
+[dev]
 numpy>=1.19.5
-openai>=0.27.4
-opencv-contrib-python-headless>=4.6.0.66
 pandas>=1.1.5
+opencv-contrib-python-headless>=4.6.0.66
+Pillow>=8.4.0
+sqlalchemy<2.0.0,>=1.4.0
+sqlalchemy-utils>=0.36.6
+lark>=1.0.0
 pyyaml>=5.1
+importlib-metadata<5.0
 ray>=1.13.0
-sqlalchemy-utils>=0.36.6
-sqlalchemy<2.0.0,>=1.4.0
-thefuzz
-timm>=0.6.13
+aenum>=2.2.0
+diskcache>=5.4.0
+eva-decord>=0.6.1
+boto3
+nest_asyncio
+langchain
+pymupdf
+pdfminer.six
 torch>=1.10.0
 torchvision>=0.11.1
-transformers>=4.27.4
+faiss-cpu
+facenet-pytorch>=2.5.2
+ipython<8.13.0
+thefuzz
 ultralytics>=8.0.93
-
-[dev]
-Pillow>=8.4.0
-aenum>=2.2.0
+transformers>=4.27.4
+openai>=0.27.4
+timm>=0.6.13
+norfair>=2.2.0
 black>=23.1.0
-boto3
-codespell
+isort>=5.10.1
+pytest>=6.1.2
+pytest-cov>=2.11.1
+pytest-random-order>=1.0.4
+pytest-virtualenv
+pytest-asyncio
+pytest-xdist
 coveralls>=3.0.1
-diskcache>=5.4.0
-eva-decord>=0.6.1
-facenet-pytorch>=2.5.2
-faiss-cpu
 flake8>=3.9.1
-importlib-metadata<5.0
-ipython<8.13.0
+moto[s3]>=4.1.1
 ipywidgets>=7.7.2
-isort>=5.10.1
-kornia
-lark>=1.0.0
 matplotlib>=3.3.4
-moto[s3]>=4.1.1
 nbmake>=1.2.1
 nest-asyncio>=1.5.6
-nest_asyncio
-norfair>=2.2.0
-numpy>=1.19.5
-openai>=0.27.4
-opencv-contrib-python-headless>=4.6.0.66
-pandas>=1.1.5
-pyenchant
+pytest-benchmark
+codespell
 pylint
 pymysql>=0.10.1
-pytest-asyncio
-pytest-benchmark
-pytest-cov>=2.11.1
-pytest-random-order>=1.0.4
-pytest-virtualenv
-pytest-xdist
-pytest>=6.1.2
-pyyaml>=5.1
-qdrant-client>=1.1.7
-ray>=1.13.0
-scriv>=0.16.0
-sqlalchemy-utils>=0.36.6
-sqlalchemy<2.0.0,>=1.4.0
-thefuzz
-timm>=0.6.13
-torch>=1.10.0
-torchvision>=0.11.1
-transformers>=4.27.4
-ultralytics>=8.0.93
 wheel>=0.37.1
+semantic_version
+PyGithub
+twine
+qdrant-client>=1.1.7
+kornia
+langchain>=0.0.177
```

### Comparing `evadb-0.2.4/setup.py` & `evadb-0.2.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,17 @@
     "importlib-metadata<5.0",
     "ray>=1.13.0",
     "aenum>=2.2.0",
     "diskcache>=5.4.0",
     "eva-decord>=0.6.1",
     "boto3",
     "nest_asyncio",
+    "langchain",
+    "pymupdf",
+    "pdfminer.six"
 ]
 
 formatter_libs = ["black>=23.1.0", "isort>=5.10.1"]
 
 test_libs = [
     "pytest>=6.1.2",
     "pytest-cov>=2.11.1",
@@ -84,17 +87,22 @@
     "faiss-cpu",  # faiss-gpu does not work on mac
 ]
 
 benchmark_libs = [
     "pytest-benchmark",
 ]
 
-doc_libs = ["pyenchant", "codespell", "pylint"]
+doc_libs = ["codespell", "pylint"]
 
-dist_libs = ["wheel>=0.37.1", "scriv>=0.16.0"]
+dist_libs = [
+    "wheel>=0.37.1", 
+    "semantic_version", 
+    "PyGithub", 
+    "twine"
+]
 
 ### NEEDED FOR AN ALTERNATE DATA SYSTEM OTHER THAN SQLITE
 database_libs = ["pymysql>=0.10.1"]
 
 ### NEEDED FOR A BATTERIES-LOADED EXPERIENCE
 udf_libs = [
     "facenet-pytorch>=2.5.2",  # FACE DETECTION
@@ -107,14 +115,16 @@
     "norfair>=2.2.0",  # OBJECT TRACKING
 ]
 
 ### NEEDED FOR EXPERIMENTAL FEATURES
 third_party_libs = [
     "qdrant-client>=1.1.7",  # Qdrant vector store client
     "kornia",  # SIFT features
+    "langchain>=0.0.177",  # langchain document loaders
+    "pdfminer.six",  # for reading pdfs
 ]
 
 ### NEEDED FOR EXPERIMENTAL FEATURES
 experimental_libs = []
 
 INSTALL_REQUIRES = minimal_requirement + integration_test_libs + udf_libs
 DEV_REQUIRES = (
```

### Comparing `evadb-0.2.4/test/__init__.py` & `evadb-0.2.5/test/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/benchmark_tests/__init__.py` & `evadb-0.2.5/test/optimizer/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/benchmark_tests/conftest.py` & `evadb-0.2.5/test/benchmark_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/benchmark_tests/test_benchmark_pytorch.py` & `evadb-0.2.5/test/benchmark_tests/test_benchmark_pytorch.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/binder/__init__.py` & `evadb-0.2.5/test/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/binder/test_binder_utils.py` & `evadb-0.2.5/test/binder/test_binder_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/binder/test_statement_binder.py` & `evadb-0.2.5/test/binder/test_statement_binder.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 from unittest.mock import MagicMock, patch
 
 from eva.binder.binder_utils import BinderError
 from eva.binder.statement_binder import StatementBinder
 from eva.binder.statement_binder_context import StatementBinderContext
 from eva.catalog.catalog_manager import CatalogManager
 from eva.catalog.catalog_type import NdArrayType
+from eva.expression.tuple_value_expression import TupleValueExpression
 from eva.parser.alias import Alias
+from eva.parser.create_statement import ColumnDefinition
 
 
 class StatementBinderTests(unittest.TestCase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def test_bind_tuple_value_expression(self):
@@ -112,14 +114,23 @@
     def test_bind_create_mat_statement(self):
         with patch.object(StatementBinder, "bind") as mock_binder:
             binder = StatementBinder(StatementBinderContext())
             mat_statement = MagicMock()
             binder._bind_create_mat_statement(mat_statement)
             mock_binder.assert_called_with(mat_statement.query)
 
+    def test_raises_mismatch_columns_create_mat_statement(self):
+        with patch.object(StatementBinder, "bind"):
+            binder = StatementBinder(StatementBinderContext())
+            mat_statement = MagicMock()
+            mat_statement.col_list = [ColumnDefinition('id', None, None, None)]
+            mat_statement.query.target_list = [TupleValueExpression(col_name='id'), TupleValueExpression(col_name='label')]
+            with self.assertRaises(Exception, msg='Projected columns mismatch, expected 1 found 2.'):
+                binder._bind_create_mat_statement(mat_statement)
+
     def test_bind_explain_statement(self):
         with patch.object(StatementBinder, "bind") as mock_binder:
             binder = StatementBinder(StatementBinderContext())
             stmt = MagicMock()
             binder._bind_explain_statement(stmt)
             mock_binder.assert_called_with(stmt.explainable_stmt)
```

### Comparing `evadb-0.2.4/test/binder/test_statement_binder_context.py` & `evadb-0.2.5/test/binder/test_statement_binder_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/catalog/__init__.py` & `evadb-0.2.5/test/plan_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/catalog/models/__init__.py` & `evadb-0.2.5/test/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/catalog/models/test_models.py` & `evadb-0.2.5/test/catalog/models/test_models.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/catalog/services/__init__.py` & `evadb-0.2.5/test/server/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/catalog/services/test_column_catalog_service.py` & `evadb-0.2.5/test/catalog/services/test_column_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/catalog/services/test_index_catalog_service.py` & `evadb-0.2.5/test/catalog/services/test_index_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/catalog/services/test_table_catalog_service.py` & `evadb-0.2.5/test/catalog/services/test_table_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/catalog/services/test_udf_catalog_service.py` & `evadb-0.2.5/test/catalog/services/test_udf_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/catalog/services/test_udf_cost_catalog_service.py` & `evadb-0.2.5/test/catalog/services/test_udf_cost_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/catalog/services/test_udf_io_catalog_service.py` & `evadb-0.2.5/test/catalog/services/test_udf_io_catalog_service.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/catalog/test_catalog_manager.py` & `evadb-0.2.5/test/catalog/test_catalog_manager.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/catalog/test_column_type.py` & `evadb-0.2.5/test/catalog/test_column_type.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/catalog/test_sqlalchemy.py` & `evadb-0.2.5/test/catalog/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/configuration/__init__.py` & `evadb-0.2.5/test/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/configuration/test_bootstrap_environment.py` & `evadb-0.2.5/test/configuration/test_bootstrap_environment.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import tempfile
 import unittest
 from pathlib import Path
 
-import pytest
-
 from eva.configuration.bootstrap_environment import bootstrap_environment
 from eva.configuration.constants import EVA_CONFIG_FILE, EVA_INSTALLATION_DIR, UDF_DIR
 
 
 class BootstrapEnvironmentTests(unittest.TestCase):
     def test_bootstrap_environment(self):
         with tempfile.TemporaryDirectory() as temp_dir:
@@ -31,10 +29,10 @@
             config_path = temp_dir_path / EVA_CONFIG_FILE
             assert config_path.exists()
 
             udfs_dir = temp_dir_path / UDF_DIR
             assert udfs_dir.exists()
 
     def test_invalid_eva_path_setup(self):
-        with pytest.raises(OSError):
-            with tempfile.TemporaryDirectory() as temp_dir:
+        with tempfile.TemporaryDirectory() as temp_dir:
+            with self.assertRaises(AssertionError):
                 bootstrap_environment(Path(temp_dir), Path("invalid", "dir"))
```

### Comparing `evadb-0.2.4/test/configuration/test_configuration_manager.py` & `evadb-0.2.5/test/configuration/test_configuration_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         return super().setUp()
 
     def test_configuration_manager_read_valid_key(self):
         value = self.config.get_value("core", "datasets_dir")
         self.assertIsNotNone(value)
 
     def test_configuration_manager_read_invalid_category(self):
-        self.assertIsNone(self.config.get_value("invalid", ""))
+        self.assertEquals(self.config.get_value("invalid", ""), {})
 
     def test_configuration_manager_read_invalid_key(self):
         self.assertIsNone(self.config.get_value("core", "invalid"))
 
     def test_configuration_manager_update_valid_key(self):
         value = self.config.get_value("core", "mode")
```

### Comparing `evadb-0.2.4/test/executor/__init__.py` & `evadb-0.2.5/test/udfs/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/executor/test_abstract_executor.py` & `evadb-0.2.5/test/executor/test_abstract_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/executor/test_create_udf_executor.py` & `evadb-0.2.5/test/executor/test_create_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/executor/test_execution_context.py` & `evadb-0.2.5/test/executor/test_execution_context.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/executor/test_executor_utils.py` & `evadb-0.2.5/test/executor/test_executor_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/executor/test_limit_executor.py` & `evadb-0.2.5/test/executor/test_limit_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/executor/test_load_executor.py` & `evadb-0.2.5/test/executor/test_load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/executor/test_orderby_executor.py` & `evadb-0.2.5/test/executor/test_orderby_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/executor/test_plan_executor.py` & `evadb-0.2.5/test/executor/test_plan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/executor/test_pp_executor.py` & `evadb-0.2.5/test/executor/test_pp_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/executor/test_sample_executor.py` & `evadb-0.2.5/test/executor/test_sample_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/executor/test_seq_scan_executor.py` & `evadb-0.2.5/test/executor/test_seq_scan_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/executor/utils.py` & `evadb-0.2.5/test/executor/utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/expression/__init__.py` & `evadb-0.2.5/test/udfs/decorators/io_descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/expression/test_abstract_expression.py` & `evadb-0.2.5/test/expression/test_abstract_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/expression/test_aggregation.py` & `evadb-0.2.5/test/expression/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/expression/test_arithmetic.py` & `evadb-0.2.5/test/expression/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/expression/test_comparison.py` & `evadb-0.2.5/test/expression/test_comparison.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/expression/test_expression_tree.py` & `evadb-0.2.5/test/expression/test_expression_tree.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/expression/test_expression_utils.py` & `evadb-0.2.5/test/expression/test_expression_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/expression/test_function_expression.py` & `evadb-0.2.5/test/expression/test_function_expression.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/expression/test_logical.py` & `evadb-0.2.5/test/expression/test_logical.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/integration_tests/__init__.py` & `evadb-0.2.5/test/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/integration_tests/test_array_count.py` & `evadb-0.2.5/test/integration_tests/test_array_count.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/integration_tests/test_chatgpt.py` & `evadb-0.2.5/test/integration_tests/test_chatgpt.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/integration_tests/test_create_index_executor.py` & `evadb-0.2.5/test/integration_tests/test_create_index_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/integration_tests/test_create_table_executor.py` & `evadb-0.2.5/test/optimizer/test_optimizer_context.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,25 +10,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
 
-from eva.executor.executor_utils import ExecutorError
-from eva.server.command_handler import execute_query_fetch_all
+from mock import MagicMock
 
+from eva.optimizer.cost_model import CostModel
+from eva.optimizer.optimizer_context import OptimizerContext
 
-class CreateTableTest(unittest.TestCase):
-    @classmethod
-    def setUpClass(cls):
-        pass
 
-    @classmethod
-    def tearDownClass(cls):
-        pass
+class TestOptimizerContext(unittest.TestCase):
+    def test_add_root(self):
+        fake_opr = MagicMock()
+        fake_opr.children = []
 
-    def test_currently_cannot_create_boolean_table(self):
-        query = """ CREATE TABLE BooleanTable( A BOOLEAN);"""
-
-        with self.assertRaises(ExecutorError):
-            execute_query_fetch_all(query)
+        opt_ctxt = OptimizerContext(CostModel())
+        opt_ctxt.add_opr_to_group(fake_opr)
+        self.assertEqual(len(opt_ctxt.memo.group_exprs), 1)
```

### Comparing `evadb-0.2.4/test/integration_tests/test_delete_executor.py` & `evadb-0.2.5/test/integration_tests/test_delete_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/integration_tests/test_drop_executor.py` & `evadb-0.2.5/test/integration_tests/test_drop_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/integration_tests/test_error_handling_with_ray.py` & `evadb-0.2.5/test/integration_tests/test_error_handling_with_ray.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/integration_tests/test_explain_executor.py` & `evadb-0.2.5/test/integration_tests/test_explain_executor.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # limitations under the License.
 import unittest
 from test.util import create_sample_video, file_remove, load_udfs_for_testing
 
 import pytest
 
 from eva.catalog.catalog_manager import CatalogManager
-from eva.configuration.configuration_manager import ConfigurationManager
 from eva.optimizer.plan_generator import PlanGenerator
 from eva.optimizer.rules.rules import (
     EmbedFilterIntoGet,
     LogicalInnerJoinCommutativity,
     XformLateralJoinToLinearFlow,
 )
 from eva.optimizer.rules.rules_manager import disable_rules
@@ -43,35 +42,28 @@
 
     @classmethod
     def tearDownClass(cls):
         file_remove("dummy.avi")
         execute_query_fetch_all("DROP TABLE IF EXISTS MyVideo;")
 
     def test_explain_simple_select(self):
-        ray_enabled = ConfigurationManager().get_value("experimental", "ray")
         select_query = "EXPLAIN SELECT id, data FROM MyVideo"
         batch = execute_query_fetch_all(select_query)
         expected_output = (
-            """|__ ExchangePlan\n    |__ ProjectPlan\n        |__ SeqScanPlan\n            |__ ExchangePlan\n                |__ StoragePlan\n"""
-            if ray_enabled
-            else """|__ ProjectPlan\n    |__ SeqScanPlan\n        |__ StoragePlan\n"""
+            """|__ ProjectPlan\n    |__ SeqScanPlan\n        |__ StoragePlan\n"""
         )
         self.assertEqual(batch.frames[0][0], expected_output)
 
         with disable_rules([XformLateralJoinToLinearFlow()]) as rules_manager:
             custom_plan_generator = PlanGenerator(rules_manager)
             select_query = "EXPLAIN SELECT id, data FROM MyVideo JOIN LATERAL DummyObjectDetector(data) AS T ;"
             batch = execute_query_fetch_all(
                 select_query, plan_generator=custom_plan_generator
             )
-            expected_output = (
-                """|__ ProjectPlan\n    |__ LateralJoinPlan\n        |__ SeqScanPlan\n            |__ StoragePlan\n        |__ FunctionScanPlan\n"""
-                if ray_enabled
-                else """|__ ProjectPlan\n    |__ LateralJoinPlan\n        |__ SeqScanPlan\n            |__ StoragePlan\n        |__ FunctionScanPlan\n"""
-            )
+            expected_output = """|__ ProjectPlan\n    |__ LateralJoinPlan\n        |__ SeqScanPlan\n            |__ StoragePlan\n        |__ FunctionScanPlan\n"""
             self.assertEqual(batch.frames[0][0], expected_output)
 
         # Disable more rules
         with disable_rules(
             [
                 XformLateralJoinToLinearFlow(),
                 EmbedFilterIntoGet(),
@@ -79,13 +71,10 @@
             ]
         ) as rules_manager:
             custom_plan_generator = PlanGenerator(rules_manager)
             select_query = "EXPLAIN SELECT id, data FROM MyVideo JOIN LATERAL DummyObjectDetector(data) AS T ;"
             batch = execute_query_fetch_all(
                 select_query, plan_generator=custom_plan_generator
             )
-            expected_output = (
-                """|__ ProjectPlan\n    |__ LateralJoinPlan\n        |__ SeqScanPlan\n            |__ StoragePlan\n        |__ FunctionScanPlan\n"""
-                if ray_enabled
-                else """|__ ProjectPlan\n    |__ LateralJoinPlan\n        |__ SeqScanPlan\n            |__ StoragePlan\n        |__ FunctionScanPlan\n"""
-            )
+            expected_output = """|__ ProjectPlan\n    |__ LateralJoinPlan\n        |__ SeqScanPlan\n            |__ StoragePlan\n        |__ FunctionScanPlan\n"""
+            print(batch.frames[0][0])
             self.assertEqual(batch.frames[0][0], expected_output)
```

### Comparing `evadb-0.2.4/test/integration_tests/test_fuzzy_join.py` & `evadb-0.2.5/test/integration_tests/test_fuzzy_join.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/integration_tests/test_huggingface_udfs.py` & `evadb-0.2.5/test/integration_tests/test_huggingface_udfs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -36,21 +36,24 @@
         # Use DETRAC for HF Tests to test variety of models
         query = """LOAD VIDEO 'data/ua_detrac/ua_detrac.mp4' INTO DETRAC;"""
         execute_query_fetch_all(query)
 
         query = """LOAD VIDEO 'data/sample_videos/touchdown.mp4' INTO VIDEOS"""
         execute_query_fetch_all(query)
 
+        query = """LOAD PDF 'data/documents/pdf_sample1.pdf' INTO MyPDFs;"""
+        execute_query_fetch_all(query)
         # Text CSV for testing HF Text Based Models
         self.csv_file_path = create_text_csv()
 
     def tearDown(self) -> None:
         execute_query_fetch_all("DROP TABLE IF EXISTS DETRAC;")
         execute_query_fetch_all("DROP TABLE IF EXISTS VIDEOS;")
         execute_query_fetch_all("DROP TABLE IF EXISTS MyCSV;")
+        execute_query_fetch_all("DROP TABLE IF EXISTS MyPDFs;")
         file_remove(self.csv_file_path)
 
     def test_io_catalog_entries_populated(self):
         udf_name, task = "HFObjectDetector", "image-classification"
         create_udf_query = f"""CREATE UDF {udf_name}
             TYPE HuggingFace
             'task' '{task}'
@@ -354,7 +357,57 @@
             all(
                 isinstance(x, float) for x in output.frames[udf_name.lower() + ".score"]
             )
         )
 
         drop_udf_query = f"DROP UDF {udf_name};"
         execute_query_fetch_all(drop_udf_query)
+
+    @pytest.mark.benchmark
+    def test_named_entity_recognition_model_all_pdf_data(self):
+        udf_name = "HFNERModel"
+        create_udf_query = f"""CREATE UDF {udf_name}
+            TYPE HuggingFace
+            'task' 'ner'
+        """
+        execute_query_fetch_all(create_udf_query)
+
+        # running test case on all the pdf data
+        select_query = f"SELECT data, {udf_name}(data) FROM MyPDFs;"
+        output = execute_query_fetch_all(select_query)
+
+        # Test that output has 7 columns
+        self.assertEqual(len(output.frames.columns), 7)
+
+        # Test that there exists a column with udf_name.entity
+        self.assertTrue(udf_name.lower() + ".entity" in output.frames.columns)
+
+        # Test that there exists a column with udf_name.score
+        self.assertTrue(udf_name.lower() + ".score" in output.frames.columns)
+
+        drop_udf_query = f"DROP UDF {udf_name};"
+        execute_query_fetch_all(drop_udf_query)
+
+    @pytest.mark.benchmark
+    def test_named_entity_recognition_model_no_ner_data_exists(self):
+        udf_name = "HFNERModel"
+        create_udf_query = f"""CREATE UDF {udf_name}
+            TYPE HuggingFace
+            'task' 'ner'
+        """
+        execute_query_fetch_all(create_udf_query)
+
+        # running test case where ner gives no data
+        select_query = f"""SELECT data, {udf_name}(data)
+                  FROM MyPDFs
+                  WHERE page = 3
+                  AND paragraph >= 1 AND paragraph <= 3;"""
+        output = execute_query_fetch_all(select_query)
+
+        # Test that output only has 1 column (data)
+        self.assertEqual(len(output.frames.columns), 1)
+
+        # Test that there does not exist a column with udf_name.entity
+        self.assertFalse(udf_name.lower() + ".entity" in output.frames.columns)
+
+        drop_udf_query = f"DROP UDF {udf_name};"
+        execute_query_fetch_all(drop_udf_query)
```

### Comparing `evadb-0.2.4/test/integration_tests/test_insert_executor.py` & `evadb-0.2.5/test/integration_tests/test_insert_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/integration_tests/test_like.py` & `evadb-0.2.5/test/integration_tests/test_like.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/integration_tests/test_load_executor.py` & `evadb-0.2.5/test/integration_tests/test_load_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -492,10 +492,18 @@
 
         drop_query = "DROP TABLE IF EXISTS MyLargeScaleImages;"
         execute_query_fetch_all(drop_query)
 
         # Clean up large scale image directory.
         shutil.rmtree(large_scale_image_files_path)
 
+    def test_load_pdfs(self):
+        execute_query_fetch_all(
+            f"""LOAD DOCUMENT '{EVA_ROOT_DIR}/data/documents/*.pdf' INTO pdfs;"""
+        )
+        result = execute_query_fetch_all("SELECT * from pdfs;")
+        self.assertEqual(len(result.columns), 3)
+        self.assertEqual(len(result), 3)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `evadb-0.2.4/test/integration_tests/test_mat_executor.py` & `evadb-0.2.5/test/integration_tests/test_mat_executor.py`

 * *Files 17% similar despite different names*

```diff
@@ -49,14 +49,22 @@
     def tearDownClass(cls):
         shutdown_ray()
         file_remove("dummy.avi")
         file_remove("ua_detrac.mp4")
         execute_query_fetch_all("DROP TABLE IF EXISTS MyVideo;")
         execute_query_fetch_all("DROP TABLE UATRAC;")
 
+    def setUp(self):
+        execute_query_fetch_all("DROP TABLE IF EXISTS dummy_view;")
+        execute_query_fetch_all("DROP TABLE IF EXISTS uadtrac_fastRCNN;")
+
+    def tearDown(self):
+        execute_query_fetch_all("DROP TABLE IF EXISTS dummy_view;")
+        execute_query_fetch_all("DROP TABLE IF EXISTS uadtrac_fastRCNN;")
+
     def test_should_mat_view_with_dummy(self):
         materialized_query = """CREATE MATERIALIZED VIEW dummy_view (id, label)
             AS SELECT id, DummyObjectDetector(data).label FROM MyVideo;
         """
         execute_query_fetch_all(materialized_query)
 
         select_query = "SELECT id, label FROM dummy_view;"
@@ -69,39 +77,58 @@
             for i in range(NUM_FRAMES)
         ]
         expected_batch = Batch(frames=pd.DataFrame(expected))
         self.assertEqual(actual_batch, expected_batch)
 
     def test_should_mat_view_to_the_same_table(self):
         materialized_query = """CREATE MATERIALIZED VIEW IF NOT EXISTS
-            dummy_view2 (id, label)
+            dummy_view (id, label)
             AS SELECT id, DummyObjectDetector(data).label FROM MyVideo
             WHERE id < 5;
         """
         execute_query_fetch_all(materialized_query)
 
         materialized_query = """CREATE MATERIALIZED VIEW IF NOT EXISTS
-            dummy_view2 (id, label)
+            dummy_view (id, label)
             AS SELECT id, DummyObjectDetector(data).label FROM MyVideo
             WHERE id >= 5;
         """
         execute_query_fetch_all(materialized_query)
 
-        select_query = "SELECT id, label FROM dummy_view2;"
+        select_query = "SELECT id, label FROM dummy_view;"
         actual_batch = execute_query_fetch_all(select_query)
         actual_batch.sort()
 
         labels = DummyObjectDetector().labels
         expected = [
-            {"dummy_view2.id": i, "dummy_view2.label": [labels[1 + i % 2]]}
+            {"dummy_view.id": i, "dummy_view.label": [labels[1 + i % 2]]}
             for i in range(5)
         ]
         expected_batch = Batch(frames=pd.DataFrame(expected))
         self.assertEqual(actual_batch, expected_batch)
 
+    def test_should_infer_mat_view_column_names_with_dummy(self):
+        execute_query_fetch_all("DROP TABLE IF EXISTS dummy_view;")
+        materialized_query = """CREATE MATERIALIZED VIEW dummy_view
+            AS SELECT id, DummyObjectDetector(data).label FROM MyVideo;
+        """
+        execute_query_fetch_all(materialized_query)
+
+        select_query = "SELECT id, label FROM dummy_view;"
+        actual_batch = execute_query_fetch_all(select_query)
+        actual_batch.sort()
+
+        labels = DummyObjectDetector().labels
+        expected = [
+            {"dummy_view.id": i, "dummy_view.label": [labels[1 + i % 2]]}
+            for i in range(NUM_FRAMES)
+        ]
+        expected_batch = Batch(frames=pd.DataFrame(expected))
+        self.assertEqual(actual_batch, expected_batch)
+
     @pytest.mark.torchtest
     def test_should_mat_view_with_yolo(self):
         select_query = (
             "SELECT id, Yolo(data).labels, "
             "Yolo(data).bboxes "
             "FROM UATRAC WHERE id < 5;"
         )
@@ -117,32 +144,50 @@
 
         self.assertEqual(len(actual_batch), 5)
         # non-trivial test case
         res = actual_batch.frames
         for idx in res.index:
             self.assertTrue("car" in res["uadtrac_fastrcnn.labels"][idx])
 
-        execute_query_fetch_all("DROP TABLE IF EXISTS uadtrac_fastRCNN;")
-
     @pytest.mark.torchtest
     def test_should_mat_view_with_fastrcnn_lateral_join(self):
         select_query = (
             "SELECT id, label, bbox FROM UATRAC JOIN LATERAL "
             "Yolo(data) AS T(label, bbox, score) WHERE id < 5;"
         )
         query = (
             "CREATE MATERIALIZED VIEW IF NOT EXISTS "
-            f"uadtrac_fastRCNN_new (id, label, bbox) AS {select_query};"
+            f"uadtrac_fastRCNN (id, label, bbox) AS {select_query};"
         )
         execute_query_fetch_all(query)
 
-        select_view_query = "SELECT id, label, bbox FROM uadtrac_fastRCNN_new"
+        select_view_query = "SELECT id, label, bbox FROM uadtrac_fastRCNN"
         actual_batch = execute_query_fetch_all(select_view_query)
         actual_batch.sort()
 
         self.assertEqual(len(actual_batch), 5)
         # non-trivial test case
         res = actual_batch.frames
         for idx in res.index:
-            self.assertTrue("car" in res["uadtrac_fastrcnn_new.label"][idx])
+            self.assertTrue("car" in res["uadtrac_fastrcnn.label"][idx])
 
-        execute_query_fetch_all("DROP TABLE IF EXISTS uadtrac_fastRCNN;")
+    @pytest.mark.torchtest
+    def test_should_infer_mat_view_column_names_with_fastrcnn_lateral_join(self):
+        select_query = (
+            "SELECT id, label, bbox FROM UATRAC JOIN LATERAL "
+            "Yolo(data) AS T(label, bbox, score) WHERE id < 5;"
+        )
+        query = (
+            "CREATE MATERIALIZED VIEW IF NOT EXISTS "
+            f"uadtrac_fastRCNN AS {select_query};"
+        )
+        execute_query_fetch_all(query)
+
+        select_view_query = "SELECT id, label, bbox FROM uadtrac_fastRCNN"
+        actual_batch = execute_query_fetch_all(select_view_query)
+        actual_batch.sort()
+
+        self.assertEqual(len(actual_batch), 5)
+        # non-trivial test case
+        res = actual_batch.frames
+        for idx in res.index:
+            self.assertTrue("car" in res["uadtrac_fastrcnn.label"][idx])
```

### Comparing `evadb-0.2.4/test/integration_tests/test_open.py` & `evadb-0.2.5/test/integration_tests/test_open.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/integration_tests/test_optimizer_rules.py` & `evadb-0.2.5/test/integration_tests/test_optimizer_rules.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/integration_tests/test_pytorch.py` & `evadb-0.2.5/test/integration_tests/test_pytorch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,23 +11,31 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import unittest
 from test.markers import ocr_skip_marker, windows_skip_marker
-from test.util import file_remove, load_udfs_for_testing, shutdown_ray
+from test.util import (
+    create_sample_video,
+    file_remove,
+    load_udfs_for_testing,
+    shutdown_ray,
+)
 
 import cv2
 import numpy as np
+import pandas.testing as pd_testing
 import pytest
 
 from eva.catalog.catalog_manager import CatalogManager
 from eva.configuration.configuration_manager import ConfigurationManager
 from eva.configuration.constants import EVA_ROOT_DIR
+from eva.executor.executor_utils import ExecutorError
+from eva.models.storage.batch import Batch
 from eva.server.command_handler import execute_query_fetch_all
 from eva.udfs.udf_bootstrap_queries import Asl_udf_query, Mvit_udf_query
 
 
 @pytest.mark.notparallel
 class PytorchTest(unittest.TestCase):
     @classmethod
@@ -59,14 +67,97 @@
 
         execute_query_fetch_all("DROP TABLE IF EXISTS Actions;")
         execute_query_fetch_all("DROP TABLE IF EXISTS MNIST;")
         execute_query_fetch_all("DROP TABLE IF EXISTS MyVideo;")
         execute_query_fetch_all("DROP TABLE IF EXISTS Asl_actions;")
         execute_query_fetch_all("DROP TABLE IF EXISTS MemeImages;")
 
+    def assertBatchEqual(self, a: Batch, b: Batch, msg: str):
+        try:
+            pd_testing.assert_frame_equal(a.frames, b.frames)
+        except AssertionError as e:
+            raise self.failureException(msg) from e
+
+    def setUp(self):
+        self.addTypeEqualityFunc(Batch, self.assertBatchEqual)
+
+    @pytest.mark.skipif(
+        not ConfigurationManager().get_value("experimental", "ray"),
+        reason="Only test for parallel execution",
+    )
+    def test_should_apply_parallel_match_sequential(self):
+        # Parallel execution
+        select_query = """SELECT id, obj.labels
+                          FROM MyVideo JOIN LATERAL
+                          FastRCNNObjectDetector(data)
+                          AS obj(labels, bboxes, scores)
+                         WHERE id < 20;"""
+        par_batch = execute_query_fetch_all(select_query)
+
+        # Sequential execution.
+        ConfigurationManager().update_value("experimental", "ray", False)
+        select_query = """SELECT id, obj.labels
+                          FROM MyVideo JOIN LATERAL
+                          FastRCNNObjectDetector(data)
+                          AS obj(labels, bboxes, scores)
+                         WHERE id < 20;"""
+        seq_batch = execute_query_fetch_all(select_query)
+        # Recover configuration back.
+        ConfigurationManager().update_value("experimental", "ray", True)
+
+        self.assertEqual(len(par_batch), len(seq_batch))
+        self.assertEqual(par_batch, seq_batch)
+
+    @pytest.mark.skipif(
+        not ConfigurationManager().get_value("experimental", "ray"),
+        reason="Only test for Ray",
+    )
+    def test_should_project_parallel_match_sequential(self):
+        create_udf_query = """CREATE UDF FaceDetector
+                  INPUT  (frame NDARRAY UINT8(3, ANYDIM, ANYDIM))
+                  OUTPUT (bboxes NDARRAY FLOAT32(ANYDIM, 4),
+                          scores NDARRAY FLOAT32(ANYDIM))
+                  TYPE  FaceDetection
+                  IMPL  'eva/udfs/face_detector.py';
+        """
+        execute_query_fetch_all(create_udf_query)
+
+        select_query = """SELECT FaceDetector(data) FROM MyVideo
+                        WHERE id < 5;"""
+        # Parallel execution
+        par_batch = execute_query_fetch_all(select_query)
+
+        # Sequential execution.
+        ConfigurationManager().update_value("experimental", "ray", False)
+        seq_batch = execute_query_fetch_all(select_query)
+        # Recover configuration back.
+        ConfigurationManager().update_value("experimental", "ray", True)
+
+        self.assertEqual(len(par_batch), len(seq_batch))
+        self.assertEqual(par_batch, seq_batch)
+
+    @pytest.mark.skipif(
+        not ConfigurationManager().get_value("experimental", "ray"),
+        reason="Only test for Ray",
+    )
+    def test_should_raise_exception_with_parallel(self):
+        # Deliberately cause error.
+        video_path = create_sample_video(100)
+        load_query = f"LOAD VIDEO '{video_path}' INTO parallelErrorVideo;"
+        execute_query_fetch_all(load_query)
+        file_remove("dummy.avi")
+
+        select_query = """SELECT id, obj.labels
+                          FROM parallelErrorVideo JOIN LATERAL
+                          FastRCNNObjectDetector(data)
+                          AS obj(labels, bboxes, scores)
+                         WHERE id < 2;"""
+        with self.assertRaises(ExecutorError):
+            execute_query_fetch_all(select_query)
+
     @pytest.mark.torchtest
     def test_should_run_pytorch_and_fastrcnn_with_lateral_join(self):
         select_query = """SELECT id, obj.labels
                           FROM MyVideo JOIN LATERAL
                           FastRCNNObjectDetector(data)
                           AS obj(labels, bboxes, scores)
                          WHERE id < 2;"""
@@ -105,30 +196,14 @@
         res = actual_batch.frames
 
         self.assertEqual(len(res), 1)
         for idx in res.index:
             self.assertTrue("computer" in res["aslactionrecognition.labels"][idx])
 
     @pytest.mark.torchtest
-    def test_should_run_pytorch_and_facenet(self):
-        create_udf_query = """CREATE UDF FaceDetector
-                  INPUT  (frame NDARRAY UINT8(3, ANYDIM, ANYDIM))
-                  OUTPUT (bboxes NDARRAY FLOAT32(ANYDIM, 4),
-                          scores NDARRAY FLOAT32(ANYDIM))
-                  TYPE  FaceDetection
-                  IMPL  'eva/udfs/face_detector.py';
-        """
-        execute_query_fetch_all(create_udf_query)
-
-        select_query = """SELECT FaceDetector(data) FROM MyVideo
-                        WHERE id < 5;"""
-        actual_batch = execute_query_fetch_all(select_query)
-        self.assertEqual(len(actual_batch), 5)
-
-    @pytest.mark.torchtest
     @windows_skip_marker
     @ocr_skip_marker
     def test_should_run_pytorch_and_ocr(self):
         create_udf_query = """CREATE UDF IF NOT EXISTS OCRExtractor
                   INPUT  (frame NDARRAY UINT8(3, ANYDIM, ANYDIM))
                   OUTPUT (labels NDARRAY STR(10),
                           bboxes NDARRAY FLOAT32(ANYDIM, 4),
```

### Comparing `evadb-0.2.4/test/integration_tests/test_rename_executor.py` & `evadb-0.2.5/test/integration_tests/test_rename_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/integration_tests/test_reuse.py` & `evadb-0.2.5/test/integration_tests/test_reuse.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         select_query = (
             """SELECT id, HFObjectDetector(data).label FROM DETRAC WHERE id < 15;"""
         )
         reuse_batch = execute_query_fetch_all(select_query)
         self._verify_reuse_correctness(select_query, reuse_batch)
 
         # different query format
-        select_query = """SELECT id, HFObjectDetector(data).score FROM DETRAC WHERE ['car'] <@ HFObjectDetector(data).label AND id < 20"""
+        select_query = """SELECT id, HFObjectDetector(data).label FROM DETRAC WHERE ['car'] <@ HFObjectDetector(data).label AND id < 20"""
         reuse_batch = execute_query_fetch_all(select_query)
         self._verify_reuse_correctness(select_query, reuse_batch)
 
     def test_reuse_logical_project_with_duplicate_query(self):
         project_query = (
             """SELECT id, HFObjectDetector(data).label FROM DETRAC WHERE id < 10;"""
         )
```

### Comparing `evadb-0.2.4/test/integration_tests/test_s3_load_executor.py` & `evadb-0.2.5/test/integration_tests/test_s3_load_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/integration_tests/test_select_executor.py` & `evadb-0.2.5/test/integration_tests/test_select_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/integration_tests/test_show_info_executor.py` & `evadb-0.2.5/test/integration_tests/test_show_info_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/integration_tests/test_similarity.py` & `evadb-0.2.5/test/integration_tests/test_similarity.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/integration_tests/test_udf_executor.py` & `evadb-0.2.5/test/integration_tests/test_udf_executor.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/markers.py` & `evadb-0.2.5/test/markers.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/models/__init__.py` & `evadb-0.2.5/eva/storage/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""
+storage subdirectory
+"""
```

### Comparing `evadb-0.2.4/test/models/catalog/__init__.py` & `evadb-0.2.5/eva/models/server/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/test/models/catalog/test_frame_info.py` & `evadb-0.2.5/test/models/catalog/test_frame_info.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/models/storage/__init__.py` & `evadb-0.2.5/eva/models/storage/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/test/models/storage/test_batch.py` & `evadb-0.2.5/test/models/storage/test_batch.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/optimizer/__init__.py` & `evadb-0.2.5/eva/optimizer/rules/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/test/optimizer/rules/__init__.py` & `evadb-0.2.5/eva/parser/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/test/optimizer/rules/test_rules.py` & `evadb-0.2.5/test/optimizer/rules/test_rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -18,65 +18,54 @@
 import pytest
 from mock import MagicMock, patch
 
 from eva.catalog.catalog_manager import CatalogManager
 from eva.catalog.catalog_type import TableType
 from eva.catalog.models.table_catalog import TableCatalogEntry
 from eva.configuration.configuration_manager import ConfigurationManager
-from eva.experimental.ray.optimizer.rules.rules import LogicalExchangeToPhysical
-from eva.experimental.ray.optimizer.rules.rules import (
-    LogicalGetToSeqScan as DistributedLogicalGetToSeqScan,
-)
-from eva.experimental.ray.optimizer.rules.rules import (
-    LogicalProjectToPhysical as DistributedLogicalProjectToPhysical,
-)
 from eva.optimizer.operators import (
     LogicalFilter,
     LogicalGet,
     LogicalJoin,
     LogicalSample,
 )
 from eva.optimizer.rules.rules import (
     CacheFunctionExpressionInApply,
     CacheFunctionExpressionInFilter,
     CacheFunctionExpressionInProject,
     CombineSimilarityOrderByAndLimitToVectorIndexScan,
     EmbedFilterIntoGet,
     EmbedSampleIntoGet,
     LogicalApplyAndMergeToPhysical,
+    LogicalApplyAndMergeToRayPhysical,
+    LogicalCreateFromSelectToPhysical,
     LogicalCreateIndexToVectorIndex,
     LogicalCreateMaterializedViewToPhysical,
     LogicalCreateToPhysical,
     LogicalCreateUDFToPhysical,
     LogicalDeleteToPhysical,
     LogicalDerivedGetToPhysical,
     LogicalDropToPhysical,
     LogicalDropUDFToPhysical,
+    LogicalExchangeToPhysical,
     LogicalExplainToPhysical,
     LogicalFilterToPhysical,
     LogicalFunctionScanToPhysical,
-)
-from eva.optimizer.rules.rules import (
-    LogicalGetToSeqScan as SequentialLogicalGetToSeqScan,
-)
-from eva.optimizer.rules.rules import (
+    LogicalGetToSeqScan,
     LogicalGroupByToPhysical,
     LogicalInnerJoinCommutativity,
     LogicalInsertToPhysical,
     LogicalJoinToPhysicalHashJoin,
     LogicalJoinToPhysicalNestedLoopJoin,
     LogicalLateralJoinToPhysical,
     LogicalLimitToPhysical,
     LogicalLoadToPhysical,
     LogicalOrderByToPhysical,
-)
-from eva.optimizer.rules.rules import (
-    LogicalProjectToPhysical as SequentialLogicalProjectToPhysical,
-)
-from eva.optimizer.rules.rules import (
+    LogicalProjectToPhysical,
+    LogicalProjectToRayPhysical,
     LogicalRenameToPhysical,
     LogicalShowToPhysical,
     LogicalUnionToPhysical,
     LogicalVectorIndexScanToPhysical,
     Promise,
     PushDownFilterThroughApplyAndMerge,
     PushDownFilterThroughJoin,
@@ -132,14 +121,15 @@
             Promise.LOGICAL_LIMIT_TO_PHYSICAL,
             Promise.LOGICAL_INSERT_TO_PHYSICAL,
             Promise.LOGICAL_DELETE_TO_PHYSICAL,
             Promise.LOGICAL_RENAME_TO_PHYSICAL,
             Promise.LOGICAL_DROP_TO_PHYSICAL,
             Promise.LOGICAL_LOAD_TO_PHYSICAL,
             Promise.LOGICAL_CREATE_TO_PHYSICAL,
+            Promise.LOGICAL_CREATE_FROM_SELECT_TO_PHYSICAL,
             Promise.LOGICAL_CREATE_UDF_TO_PHYSICAL,
             Promise.LOGICAL_SAMPLE_TO_UNIFORMSAMPLE,
             Promise.LOGICAL_GET_TO_SEQSCAN,
             Promise.LOGICAL_DERIVED_GET_TO_PHYSICAL,
             Promise.LOGICAL_LATERAL_JOIN_TO_PHYSICAL,
             Promise.LOGICAL_JOIN_TO_PHYSICAL_HASH_JOIN,
             Promise.LOGICAL_JOIN_TO_PHYSICAL_NESTED_LOOP_JOIN,
@@ -209,42 +199,43 @@
         # For the current version, we choose either the distributed or the
         # sequential rule, because we do not have a logic to choose one over
         # the other in the current optimizer. Sequential rewrite is currently
         # embedded inside distributed rule if ray is enabled. The rule itself
         # has some simple heuristics to choose one over the other.
         supported_implementation_rules = [
             LogicalCreateToPhysical(),
+            LogicalCreateFromSelectToPhysical(),
             LogicalRenameToPhysical(),
             LogicalDropToPhysical(),
             LogicalCreateUDFToPhysical(),
             LogicalDropUDFToPhysical(),
             LogicalInsertToPhysical(),
             LogicalDeleteToPhysical(),
             LogicalLoadToPhysical(),
-            DistributedLogicalGetToSeqScan()
+            LogicalGetToSeqScan(),
+            LogicalProjectToRayPhysical()
             if ray_enabled
-            else SequentialLogicalGetToSeqScan(),
+            else LogicalProjectToPhysical(),
             LogicalDerivedGetToPhysical(),
             LogicalUnionToPhysical(),
             LogicalGroupByToPhysical(),
             LogicalOrderByToPhysical(),
             LogicalLimitToPhysical(),
             LogicalJoinToPhysicalNestedLoopJoin(),
             LogicalLateralJoinToPhysical(),
             LogicalFunctionScanToPhysical(),
             LogicalJoinToPhysicalHashJoin(),
             LogicalCreateMaterializedViewToPhysical(),
             LogicalFilterToPhysical(),
-            DistributedLogicalProjectToPhysical()
+            LogicalApplyAndMergeToRayPhysical()
             if ray_enabled
-            else SequentialLogicalProjectToPhysical(),
+            else LogicalApplyAndMergeToPhysical(),
             LogicalShowToPhysical(),
             LogicalExplainToPhysical(),
             LogicalCreateIndexToVectorIndex(),
-            LogicalApplyAndMergeToPhysical(),
             LogicalVectorIndexScanToPhysical(),
         ]
 
         if ray_enabled:
             supported_implementation_rules.append(LogicalExchangeToPhysical())
         self.assertEqual(
             len(supported_implementation_rules),
```

### Comparing `evadb-0.2.4/test/optimizer/test_binder.py` & `evadb-0.2.5/test/optimizer/test_binder.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/optimizer/test_cost_model.py` & `evadb-0.2.5/test/optimizer/test_cost_model.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/optimizer/test_group.py` & `evadb-0.2.5/test/optimizer/test_group.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/optimizer/test_memo.py` & `evadb-0.2.5/test/optimizer/test_memo.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/optimizer/test_optimizer_task.py` & `evadb-0.2.5/test/optimizer/test_optimizer_task.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
 from unittest.mock import patch
 
 from mock import MagicMock
 
-from eva.configuration.configuration_manager import ConfigurationManager
-from eva.experimental.ray.planner.exchange_plan import ExchangePlan
 from eva.optimizer.cost_model import CostModel
 from eva.optimizer.operators import (
     LogicalFilter,
     LogicalGet,
     LogicalProject,
     LogicalQueryDerivedGet,
 )
@@ -118,32 +116,21 @@
                     [MagicMock()], children=[root_filter_opr]
                 )
 
                 opt_cxt, root_grp_id = self.top_down_rewrite(root_project_opr)
                 opt_cxt, root_grp_id = self.bottom_up_rewrite(root_grp_id, opt_cxt)
                 opt_cxt, root_grp_id = self.implement_group(root_grp_id, opt_cxt)
 
-                if not ConfigurationManager().get_value("experimental", "ray"):
-                    expected_expr_order = [
-                        ProjectPlan,
-                        PredicatePlan,
-                        SeqScanPlan,
-                        ProjectPlan,
-                        SeqScanPlan,
-                    ]
-                else:
-                    expected_expr_order = [
-                        ExchangePlan,
-                        ProjectPlan,
-                        PredicatePlan,
-                        SeqScanPlan,
-                        ExchangePlan,
-                        ProjectPlan,
-                        SeqScanPlan,
-                    ]
+                expected_expr_order = [
+                    ProjectPlan,
+                    PredicatePlan,
+                    SeqScanPlan,
+                    ProjectPlan,
+                    SeqScanPlan,
+                ]
                 curr_grp_id = root_grp_id
                 idx = 0
                 while True:
                     root_grp = opt_cxt.memo.groups[curr_grp_id]
                     best_root_grp_expr = root_grp.get_best_expr(PropertyType.DEFAULT)
                     self.assertEqual(
                         type(best_root_grp_expr.opr), expected_expr_order[idx]
```

### Comparing `evadb-0.2.4/test/optimizer/test_optimizer_utils.py` & `evadb-0.2.5/test/optimizer/test_optimizer_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/optimizer/test_statement_to_opr_converter.py` & `evadb-0.2.5/test/optimizer/test_statement_to_opr_converter.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/parser/__init__.py` & `evadb-0.2.5/eva/readers/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/test/parser/test_parser.py` & `evadb-0.2.5/test/parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/parser/test_parser_statements.py` & `evadb-0.2.5/test/parser/test_parser_statements.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/plan_nodes/__init__.py` & `evadb-0.2.5/eva/readers/document/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/test/plan_nodes/test_plan.py` & `evadb-0.2.5/test/plan_nodes/test_plan.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/readers/__init__.py` & `evadb-0.2.5/eva/readers/image/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/test/readers/test_csv_reader.py` & `evadb-0.2.5/test/readers/test_csv_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/readers/test_decord_reader.py` & `evadb-0.2.5/test/readers/test_decord_reader.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/server/__init__.py` & `evadb-0.2.5/eva/udfs/decorators/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/test/server/test_command_handler.py` & `evadb-0.2.5/test/server/test_command_handler.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/server/test_db_api.py` & `evadb-0.2.5/test/server/test_db_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import sys
 import unittest
 from test.util import prefix_worker_id
 
 from mock import MagicMock, patch
 
 from eva.models.server.response import Response
-from eva.server.db_api import EVACursor, connect
+from eva.interfaces.relational.db import EVACursor, connect
 
 # Check for Python 3.8+ for IsolatedAsyncioTestCase support
 if sys.version_info >= (3, 8):
     from unittest.mock import AsyncMock
 
     class DBAPITests(unittest.IsolatedAsyncioTestCase):
         def __init__(self, *args, **kwargs):
```

### Comparing `evadb-0.2.4/test/server/test_interpreter.py` & `evadb-0.2.5/test/server/test_interpreter.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
     class InterpreterTests(unittest.IsolatedAsyncioTestCase):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
 
         @patch("asyncio.open_connection")
         @patch("eva.server.interpreter.create_stdin_reader")
-        @patch("eva.server.db_api.EVACursor.execute_async")
-        @patch("eva.server.db_api.EVACursor.fetch_all_async")
+        @patch("eva.interfaces.relational.db.EVACursor.execute_async")
+        @patch("eva.interfaces.relational.db.EVACursor.fetch_all_async")
         async def test_start_cmd_client(
             self, mock_fetch, mock_execute, mock_stdin_reader, mock_open
         ):
             host = "localhost"
             port = find_free_port()
 
             server_reader = asyncio.StreamReader()
```

### Comparing `evadb-0.2.4/test/server/test_server.py` & `evadb-0.2.5/test/server/test_server.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/storage/__init__.py` & `evadb-0.2.5/eva/udfs/decorators/io_descriptors/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/test/storage/test_sqlite_storage_engine.py` & `evadb-0.2.5/test/storage/test_sqlite_storage_engine.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/storage/test_video_storage.py` & `evadb-0.2.5/test/storage/test_video_storage.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/test_eva_cmd_client.py` & `evadb-0.2.5/test/test_eva_cmd_client.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/test_eva_imports.py` & `evadb-0.2.5/test/test_eva_imports.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/test_eva_server.py` & `evadb-0.2.5/test/test_eva_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # Check for Python 3.8+ for IsolatedAsyncioTestCase support
 if sys.version_info >= (3, 8):
 
     class EVAServerTest(unittest.IsolatedAsyncioTestCase):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
 
-        @patch("eva.eva_server.init_builtin_udfs")
+        @patch("eva.udfs.udf_bootstrap_queries.init_builtin_udfs")
         @patch("eva.eva_server.start_eva_server")
         @patch("eva.eva_server.ConfigurationManager")
         @patch("asyncio.run")
         def test_main(self, mock_run, mock_config, mock_start_eva_server, mock_udfs):
             mock_obj_1 = MagicMock()
             mock_config.return_value.get_value = mock_obj_1
             main()
```

### Comparing `evadb-0.2.4/test/udfs/__init__.py` & `evadb-0.2.5/eva/udfs/ndarray/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.4/test/udfs/decorators/io_descriptors/test_descriptors.py` & `evadb-0.2.5/test/udfs/decorators/io_descriptors/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/udfs/decorators/test_decorators.py` & `evadb-0.2.5/test/udfs/decorators/test_decorators.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/udfs/ndarray/test_array_count.py` & `evadb-0.2.5/eva/udfs/trackers/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,15 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EVA
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import unittest
-
-from eva.udfs.ndarray.array_count import ArrayCount
-
-
-class CropTests(unittest.TestCase):
-    def setUp(self):
-        self.array_count = ArrayCount()
-
-    def test_array_count_name_exists(self):
-        assert hasattr(self.array_count, "name")
+"""user defined functions for object tracking"""
```

### Comparing `evadb-0.2.4/test/udfs/ndarray/test_crop.py` & `evadb-0.2.5/test/udfs/ndarray/test_crop.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/udfs/ndarray/test_open.py` & `evadb-0.2.5/test/udfs/ndarray/test_open.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/udfs/test_abstract_udf.py` & `evadb-0.2.5/test/udfs/test_abstract_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/udfs/test_emotion_detector.py` & `evadb-0.2.5/test/udfs/test_emotion_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/udfs/test_facenet_udf.py` & `evadb-0.2.5/test/udfs/test_facenet_udf.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/udfs/test_fastrcnn_object_detector.py` & `evadb-0.2.5/test/udfs/test_fastrcnn_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/udfs/test_yolo_object_detector.py` & `evadb-0.2.5/test/udfs/test_yolo_object_detector.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/util.py` & `evadb-0.2.5/test/util.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/utils/test_generic_utils.py` & `evadb-0.2.5/test/utils/test_generic_utils.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/utils/test_timer.py` & `evadb-0.2.5/test/utils/test_timer.py`

 * *Files identical despite different names*

### Comparing `evadb-0.2.4/test/utils/test_xdist.py` & `evadb-0.2.5/test/utils/test_xdist.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,48 +11,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import unittest
-from pathlib import Path
 
-from eva.catalog.sql_config import SQLConfig
 from eva.configuration.configuration_manager import ConfigurationManager
-from eva.utils.generic_utils import prefix_xdist_worker_id_to_path
 
 
 class XdistTests(unittest.TestCase):
-    def test_prefix_worker_id_to_uri_in_sql_config(self):
-        os.environ["PYTEST_XDIST_WORKER"] = "gw1"
-        sql_config = SQLConfig()
-        self.assertTrue("gw1" in sql_config.worker_uri)
-
-        os.environ["PYTEST_XDIST_WORKER"] = ""
-        sql_config = SQLConfig()
-        self.assertFalse("gw1" in sql_config.worker_uri)
 
     def test_suffix_pytest_xdist_worker_id_to_dir(self):
         os.environ["PYTEST_XDIST_WORKER"] = "gw1"
-        foo_path = Path("foo")
+        foo_path = "foo"
         configuration_manager = ConfigurationManager()
         updated_path = configuration_manager.suffix_pytest_xdist_worker_id_to_dir(
             foo_path
         )
         self.assertTrue("gw1" in str(updated_path))
 
         os.environ["PYTEST_XDIST_WORKER"] = ""
         updated_path = configuration_manager.suffix_pytest_xdist_worker_id_to_dir(
             foo_path
         )
         self.assertFalse("gw1" in str(updated_path))
-
-    def test_prefix_worker_id_to_path_in_generic_utils(self):
-        os.environ["PYTEST_XDIST_WORKER"] = "gw1"
-        foo_path = Path("foo")
-        updated_path = prefix_xdist_worker_id_to_path(foo_path)
-        self.assertTrue("gw1" in str(updated_path))
-
-        os.environ["PYTEST_XDIST_WORKER"] = ""
-        updated_path = prefix_xdist_worker_id_to_path(foo_path)
-        self.assertFalse("gw1" in str(updated_path))
```

