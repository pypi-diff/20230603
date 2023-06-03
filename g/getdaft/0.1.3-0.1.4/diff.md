# Comparing `tmp/getdaft-0.1.3.tar.gz` & `tmp/getdaft-0.1.4.tar.gz`

## Comparing `getdaft-0.1.3.tar` & `getdaft-0.1.4.tar`

### file list

```diff
@@ -1,445 +1,462 @@
--rw-r--r--   0        0        0     1306 1970-01-01 00:00:00.000000 getdaft-0.1.3/Cargo.toml
--rw-r--r--   0      501       20      834 2023-05-24 05:44:49.000000 getdaft-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0      501       20      595 2023-05-24 05:44:49.000000 getdaft-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0      501       20      428 2023-05-24 05:44:49.000000 getdaft-0.1.3/.github/dependabot.yml
--rw-r--r--   0      501       20     1333 2023-05-24 05:44:49.000000 getdaft-0.1.3/.github/workflows/broken-link-checker.yml
--rw-r--r--   0      501       20     3378 2023-05-24 05:44:49.000000 getdaft-0.1.3/.github/workflows/daft-profiling.yml
--rw-r--r--   0      501       20     1627 2023-05-24 05:44:49.000000 getdaft-0.1.3/.github/workflows/notebook-checker.yml
--rw-r--r--   0      501       20     2194 2023-05-24 05:44:49.000000 getdaft-0.1.3/.github/workflows/property-based-tests.yml
--rw-r--r--   0      501       20    12886 2023-05-24 05:44:49.000000 getdaft-0.1.3/.github/workflows/python-package.yml
--rw-r--r--   0      501       20     6182 2023-05-24 05:44:49.000000 getdaft-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0      501       20     2638 2023-05-24 05:44:49.000000 getdaft-0.1.3/.github/workflows/ray-compatibility.yml
--rw-r--r--   0      501       20      300 2023-05-24 05:44:49.000000 getdaft-0.1.3/.gitignore
--rw-r--r--   0      501       20     2126 2023-05-24 05:44:49.000000 getdaft-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0      501       20      205 2023-05-24 05:44:49.000000 getdaft-0.1.3/.readthedocs.yaml
--rw-r--r--   0      501       20     1550 2023-05-24 05:44:49.000000 getdaft-0.1.3/CONTRIBUTING.md
--rw-r--r--   0      501       20    11357 2023-05-24 05:44:49.000000 getdaft-0.1.3/LICENSE
--rw-r--r--   0      501       20     1295 2023-05-24 05:44:49.000000 getdaft-0.1.3/Makefile
--rw-r--r--   0      501       20     6126 2023-05-24 05:44:49.000000 getdaft-0.1.3/README.rst
--rw-r--r--   0      501       20        0 2023-05-24 05:44:49.000000 getdaft-0.1.3/benchmarking/__init__.py
--rw-r--r--   0      501       20        0 2023-05-24 05:44:49.000000 getdaft-0.1.3/benchmarking/tpch/__init__.py
--rw-r--r--   0      501       20     9495 2023-05-24 05:44:49.000000 getdaft-0.1.3/benchmarking/tpch/__main__.py
--rw-r--r--   0      501       20    12428 2023-05-24 05:44:49.000000 getdaft-0.1.3/benchmarking/tpch/answers.py
--rw-r--r--   0      501       20    12140 2023-05-24 05:44:49.000000 getdaft-0.1.3/benchmarking/tpch/data_generation.py
--rw-r--r--   0      501       20     4573 2023-05-24 05:44:49.000000 getdaft-0.1.3/benchmarking/tpch/pipelined_data_generation.py
--rw-r--r--   0      501       20     1436 2023-05-24 05:44:49.000000 getdaft-0.1.3/ci/upload_wheels.sh
--rw-r--r--   0      501       20      440 2023-05-24 05:44:49.000000 getdaft-0.1.3/codecov.yml
--rw-r--r--   0      501       20     2092 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/__init__.py
--rw-r--r--   0      501       20     6724 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/analytics.py
--rw-r--r--   0      501       20     3935 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/api_annotations.py
--rw-r--r--   0      501       20    10591 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/arrow_utils.py
--rw-r--r--   0      501       20     5395 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/context.py
--rw-r--r--   0      501       20     3403 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/convert.py
--rw-r--r--   0      501       20       94 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/dataframe/__init__.py
--rw-r--r--   0      501       20    49646 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/dataframe/dataframe.py
--rw-r--r--   0      501       20      306 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/dataframe/preview.py
--rw-r--r--   0      501       20      850 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/datasources.py
--rw-r--r--   0      501       20    10207 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/datatype.py
--rw-r--r--   0      501       20       84 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/errors.py
--rw-r--r--   0      501       20        0 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/execution/__init__.py
--rw-r--r--   0      501       20    24879 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/execution/execution_step.py
--rw-r--r--   0      501       20     4231 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/execution/logical_op_runners.py
--rw-r--r--   0      501       20    27790 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/execution/physical_plan.py
--rw-r--r--   0      501       20     6110 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/execution/physical_plan_factory.py
--rw-r--r--   0      501       20      170 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/expressions/__init__.py
--rw-r--r--   0      501       20    24529 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/expressions/expressions.py
--rw-r--r--   0      501       20      572 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/expressions/testing.py
--rw-r--r--   0      501       20    12728 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/filesystem.py
--rw-r--r--   0      501       20        0 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/internal/__init__.py
--rw-r--r--   0      501       20      509 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/internal/gpu.py
--rw-r--r--   0      501       20     1804 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/internal/rule.py
--rw-r--r--   0      501       20     1965 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/internal/rule_runner.py
--rw-r--r--   0      501       20     3490 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/internal/treenode.py
--rw-r--r--   0      501       20      263 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/io/__init__.py
--rw-r--r--   0      501       20     1682 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/io/_csv.py
--rw-r--r--   0      501       20     1223 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/io/_json.py
--rw-r--r--   0      501       20     2032 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/io/common.py
--rw-r--r--   0      501       20     2034 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/io/file_path.py
--rw-r--r--   0      501       20     1243 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/io/parquet.py
--rw-r--r--   0      501       20      264 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/logging.py
--rw-r--r--   0      501       20        0 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/logical/__init__.py
--rw-r--r--   0      501       20     8601 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/logical/aggregation_plan_builder.py
--rw-r--r--   0      501       20    37496 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/logical/logical_plan.py
--rw-r--r--   0      501       20     1492 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/logical/map_partition_ops.py
--rw-r--r--   0      501       20    19183 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/logical/optimizer.py
--rw-r--r--   0      501       20     3625 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/logical/schema.py
--rw-r--r--   0      501       20       99 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/pickle/__init__.py
--rw-r--r--   0      501       20    34760 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/pickle/cloudpickle.py
--rw-r--r--   0      501       20    34262 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/pickle/cloudpickle_fast.py
--rw-r--r--   0      501       20      639 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/pickle/compat.py
--rw-r--r--   0      501       20      312 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/pickle/pickle.py
--rw-r--r--   0      501       20     2036 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/resource_request.py
--rw-r--r--   0      501       20        0 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/runners/__init__.py
--rw-r--r--   0      501       20     5708 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/runners/partitioning.py
--rw-r--r--   0      501       20     1488 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/runners/profiler.py
--rw-r--r--   0      501       20    13059 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/runners/pyrunner.py
--rw-r--r--   0      501       20    25296 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/runners/ray_runner.py
--rw-r--r--   0      501       20      918 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/runners/runner.py
--rw-r--r--   0      501       20     4324 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/runners/runner_io.py
--rw-r--r--   0      501       20    18981 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/series.py
--rw-r--r--   0      501       20       82 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/table/__init__.py
--rw-r--r--   0      501       20    13420 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/table/table.py
--rw-r--r--   0      501       20     9457 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/table/table_io.py
--rw-r--r--   0      501       20     7263 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/udf.py
--rw-r--r--   0      501       20        0 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/udf_library/__init__.py
--rw-r--r--   0      501       20     3486 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/udf_library/url_udfs.py
--rw-r--r--   0      501       20     2697 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/utils.py
--rw-r--r--   0      501       20      183 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/viz/__init__.py
--rw-r--r--   0      501       20     1699 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/viz/dataframe_display.py
--rw-r--r--   0      501       20     1517 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/viz/html_viz_hooks.py
--rw-r--r--   0      501       20     5738 2023-05-24 05:44:49.000000 getdaft-0.1.3/daft/viz/repr.py
--rw-r--r--   0      501       20      148 2023-05-24 05:44:49.000000 getdaft-0.1.3/docs/CONTRIBUTING.md
--rw-r--r--   0      501       20      638 2023-05-24 05:44:49.000000 getdaft-0.1.3/docs/Makefile
--rw-r--r--   0      501       20    71692 2023-05-24 05:44:49.000000 getdaft-0.1.3/docs/source/10-min.ipynb
--rw-r--r--   0      501       20      389 2023-05-24 05:44:49.000000 getdaft-0.1.3/docs/source/_static/custom-function-signatures.css
--rw-r--r--   0      501       20      565 2023-05-24 05:44:49.000000 getdaft-0.1.3/docs/source/_static/daft-favicon.png
--rw-r--r--   0      501       20     7804 2023-05-24 05:44:49.000000 getdaft-0.1.3/docs/source/_static/daft-logo.png
--rw-r--r--   0      501       20    42148 2023-05-24 05:44:49.000000 getdaft-0.1.3/docs/source/_static/daft_illustration.png
--rw-r--r--   0      501       20    25200 2023-05-24 05:44:49.000000 getdaft-0.1.3/docs/source/_static/execution_model.png
--rw-r--r--   0      501       20     1901 2023-05-24 05:44:49.000000 getdaft-0.1.3/docs/source/_static/header.css
--rw-r--r--   0      501       20    32864 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/_static/high_level_architecture.png
--rw-r--r--   0      501       20      343 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/_static/icon-menu-close.svg
--rw-r--r--   0      501       20      333 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/_static/icon-menu-dots.svg
--rw-r--r--   0      501       20    18177 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/_static/in_memory_data_representation.png
--rw-r--r--   0      501       20      786 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/_static/mobile-menu.js
--rw-r--r--   0      501       20      856 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/_templates/layout.html
--rw-r--r--   0      501       20      994 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/_templates/sections/header.html
--rw-r--r--   0      501       20      957 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/_templates/sections/mobile-menu.html
--rw-r--r--   0      501       20      325 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/api_docs/context.rst
--rw-r--r--   0      501       20     2564 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/api_docs/dataframe.rst
--rw-r--r--   0      501       20     3444 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/api_docs/expressions.rst
--rw-r--r--   0      501       20      784 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/api_docs/groupby.rst
--rw-r--r--   0      501       20      124 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/api_docs/index.rst
--rw-r--r--   0      501       20     1457 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/api_docs/input_output.rst
--rw-r--r--   0      501       20       88 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/api_docs/udf.rst
--rw-r--r--   0      501       20     3547 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/conf.py
--rw-r--r--   0      501       20     4964 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/dataframe_comparison.rst
--rw-r--r--   0      501       20     1645 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/index.rst
--rw-r--r--   0      501       20     1089 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/install.rst
--rw-r--r--   0      501       20      743 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/index.rst
--rw-r--r--   0      501       20     7586 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/key_concepts.rst
--rw-r--r--   0      501       20     1398 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/tutorials.rst
--rw-r--r--   0      501       20     1388 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/user_guides/aggregations.rst
--rw-r--r--   0      501       20     6686 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/user_guides/dataframe-operations.rst
--rw-r--r--   0      501       20     9024 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/user_guides/expressions.rst
--rw-r--r--   0      501       20     7829 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/user_guides/intro-dataframes.rst
--rw-r--r--   0      501       20      206 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/user_guides/partitioning.rst
--rw-r--r--   0      501       20     3190 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/user_guides/read-write.rst
--rw-r--r--   0      501       20     1257 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/user_guides/scaling-up.rst
--rw-r--r--   0      501       20     8691 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/user_guides/udf.rst
--rw-r--r--   0      501       20     1551 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/learn/user_guides.rst
--rw-r--r--   0      501       20     3575 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.13.rst
--rw-r--r--   0      501       20     2241 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.14.rst
--rw-r--r--   0      501       20     1913 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.16.rst
--rw-r--r--   0      501       20     1750 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.17.rst
--rw-r--r--   0      501       20     2100 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.18.rst
--rw-r--r--   0      501       20     3647 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.19.rst
--rw-r--r--   0      501       20     4240 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.20.rst
--rw-r--r--   0      501       20     4633 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.21.rst
--rw-r--r--   0      501       20     8016 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.22.rst
--rw-r--r--   0      501       20     5385 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.23.rst
--rw-r--r--   0      501       20    11759 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.0.24.rst
--rw-r--r--   0      501       20     4750 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.1.0.rst
--rw-r--r--   0      501       20     2411 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.1.1.rst
--rw-r--r--   0      501       20     2555 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.1.2.rst
--rw-r--r--   0      501       20      839 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/0.1.3.rst
--rw-r--r--   0      501       20      935 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/_template.rst
--rw-r--r--   0      501       20      350 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/release_notes/index.rst
--rw-r--r--   0      501       20     6574 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/technical_architecture.rst
--rw-r--r--   0      501       20     1316 2023-05-24 05:44:50.000000 getdaft-0.1.3/docs/source/telemetry.rst
--rw-r--r--   0      501       20     1873 2023-05-24 05:44:50.000000 getdaft-0.1.3/pyproject.toml
--rw-r--r--   0      501       20      680 2023-05-24 05:44:50.000000 getdaft-0.1.3/requirements-dev.txt
--rw-r--r--   0      501       20       98 2023-05-24 05:44:50.000000 getdaft-0.1.3/rust-toolchain.toml
--rw-r--r--   0      501       20     4466 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/from.rs
--rw-r--r--   0      501       20      734 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/iterator.rs
--rw-r--r--   0      501       20     2945 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/mod.rs
--rw-r--r--   0      501       20      257 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/abs.rs
--rw-r--r--   0      501       20      726 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/apply.rs
--rw-r--r--   0      501       20      841 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/arange.rs
--rw-r--r--   0      501       20     6964 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/arithmetic.rs
--rw-r--r--   0      501       20     3048 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/arrow2/comparison.rs
--rw-r--r--   0      501       20       34 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/arrow2/mod.rs
--rw-r--r--   0      501       20       19 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/arrow2/sort/mod.rs
--rw-r--r--   0      501       20     3482 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/arrow2/sort/primitive/common.rs
--rw-r--r--   0      501       20      723 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/arrow2/sort/primitive/indices.rs
--rw-r--r--   0      501       20       47 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/arrow2/sort/primitive/mod.rs
--rw-r--r--   0      501       20     8075 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/arrow2/sort/primitive/sort.rs
--rw-r--r--   0      501       20     2861 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/as_arrow.rs
--rw-r--r--   0      501       20    11304 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/broadcast.rs
--rw-r--r--   0      501       20    19737 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/cast.rs
--rw-r--r--   0      501       20    11017 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/compare_agg.rs
--rw-r--r--   0      501       20    47218 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/comparison.rs
--rw-r--r--   0      501       20     1634 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/concat.rs
--rw-r--r--   0      501       20     5982 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/concat_agg.rs
--rw-r--r--   0      501       20     1433 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/count.rs
--rw-r--r--   0      501       20     1550 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/date.rs
--rw-r--r--   0      501       20     2889 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/filter.rs
--rw-r--r--   0      501       20     1264 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/float.rs
--rw-r--r--   0      501       20     1936 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/full.rs
--rw-r--r--   0      501       20     4112 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/groups.rs
--rw-r--r--   0      501       20     1515 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/hash.rs
--rw-r--r--   0      501       20    12019 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/if_else.rs
--rw-r--r--   0      501       20     1058 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/len.rs
--rw-r--r--   0      501       20     3446 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/list.rs
--rw-r--r--   0      501       20     3360 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/list_agg.rs
--rw-r--r--   0      501       20     1622 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/mean.rs
--rw-r--r--   0      501       20     2595 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/mod.rs
--rw-r--r--   0      501       20     1156 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/null.rs
--rw-r--r--   0      501       20     3819 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/pairwise.rs
--rw-r--r--   0      501       20      484 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/search_sorted.rs
--rw-r--r--   0      501       20    19071 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/sort.rs
--rw-r--r--   0      501       20     2383 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/sum.rs
--rw-r--r--   0      501       20    15006 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/take.rs
--rw-r--r--   0      501       20     5279 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/ops/utf8.rs
--rw-r--r--   0      501       20      995 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/pseudo_arrow/compute.rs
--rw-r--r--   0      501       20    13611 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/pseudo_arrow/mod.rs
--rw-r--r--   0      501       20     2502 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/array/pseudo_arrow/python.rs
--rw-r--r--   0      501       20    13119 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/datatypes/dtype.rs
--rw-r--r--   0      501       20     2012 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/datatypes/field.rs
--rw-r--r--   0      501       20     2744 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/datatypes/logical.rs
--rw-r--r--   0      501       20     8970 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/datatypes/matching.rs
--rw-r--r--   0      501       20     6650 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/datatypes/mod.rs
--rw-r--r--   0      501       20     1083 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/datatypes/time_unit.rs
--rw-r--r--   0      501       20      273 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/README.md
--rw-r--r--   0      501       20     1474 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/arithmetic.rs
--rw-r--r--   0      501       20    21828 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/expr.rs
--rw-r--r--   0      501       20     1421 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/float/is_nan.rs
--rw-r--r--   0      501       20      587 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/float/mod.rs
--rw-r--r--   0      501       20     1112 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/list/explode.rs
--rw-r--r--   0      501       20      597 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/list/mod.rs
--rw-r--r--   0      501       20     1774 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/mod.rs
--rw-r--r--   0      501       20     1178 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/numeric/abs.rs
--rw-r--r--   0      501       20      580 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/numeric/mod.rs
--rw-r--r--   0      501       20      676 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/python/mod.rs
--rw-r--r--   0      501       20     2050 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/python/partial_udf.rs
--rw-r--r--   0      501       20     2769 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/python/udf.rs
--rw-r--r--   0      501       20     1310 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/temporal/day.rs
--rw-r--r--   0      501       20     1338 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/temporal/day_of_week.rs
--rw-r--r--   0      501       20     1425 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/temporal/mod.rs
--rw-r--r--   0      501       20     1320 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/temporal/month.rs
--rw-r--r--   0      501       20     1314 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/temporal/year.rs
--rw-r--r--   0      501       20     1617 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/utf8/contains.rs
--rw-r--r--   0      501       20     1617 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/utf8/endswith.rs
--rw-r--r--   0      501       20     1336 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/utf8/length.rs
--rw-r--r--   0      501       20     1524 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/utf8/mod.rs
--rw-r--r--   0      501       20     1627 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/functions/utf8/startswith.rs
--rw-r--r--   0      501       20     4961 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/lit.rs
--rw-r--r--   0      501       20      233 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/mod.rs
--rw-r--r--   0      501       20     5298 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/optimization.rs
--rw-r--r--   0      501       20     1982 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/dsl/pyobject.rs
--rw-r--r--   0      501       20     1681 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/error.rs
--rw-r--r--   0      501       20     7867 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/ffi.rs
--rw-r--r--   0      501       20     6022 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/kernels/hashing.rs
--rw-r--r--   0      501       20       54 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/kernels/mod.rs
--rw-r--r--   0      501       20    12159 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/kernels/search_sorted.rs
--rw-r--r--   0      501       20     3917 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/kernels/utf8.rs
--rw-r--r--   0      501       20     1117 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/lib.rs
--rw-r--r--   0      501       20     5763 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/python/datatype.rs
--rw-r--r--   0      501       20      307 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/python/error.rs
--rw-r--r--   0      501       20    10188 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/python/expr.rs
--rw-r--r--   0      501       20     1644 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/python/field.rs
--rw-r--r--   0      501       20      731 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/python/mod.rs
--rw-r--r--   0      501       20     2425 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/python/schema.rs
--rw-r--r--   0      501       20     9248 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/python/series.rs
--rw-r--r--   0      501       20    10114 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/python/table.rs
--rw-r--r--   0      501       20     3016 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/schema.rs
--rw-r--r--   0      501       20    10158 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/array_impl/data_array.rs
--rw-r--r--   0      501       20     5346 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/array_impl/logical_array.rs
--rw-r--r--   0      501       20      161 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/array_impl/mod.rs
--rw-r--r--   0      501       20     2099 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/from.rs
--rw-r--r--   0      501       20     2190 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/mod.rs
--rw-r--r--   0      501       20      902 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/abs.rs
--rw-r--r--   0      501       20     5207 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/agg.rs
--rw-r--r--   0      501       20     6298 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/arithmetic.rs
--rw-r--r--   0      501       20     1925 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/broadcast.rs
--rw-r--r--   0      501       20      194 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/cast.rs
--rw-r--r--   0      501       20     2609 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/comparison.rs
--rw-r--r--   0      501       20     1558 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/concat.rs
--rw-r--r--   0      501       20     1822 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/date.rs
--rw-r--r--   0      501       20     3612 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/downcast.rs
--rw-r--r--   0      501       20      697 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/filter.rs
--rw-r--r--   0      501       20      399 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/float.rs
--rw-r--r--   0      501       20      432 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/groups.rs
--rw-r--r--   0      501       20      412 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/hash.rs
--rw-r--r--   0      501       20      314 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/if_else.rs
--rw-r--r--   0      501       20      229 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/len.rs
--rw-r--r--   0      501       20      934 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/list.rs
--rw-r--r--   0      501       20     2352 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/mod.rs
--rw-r--r--   0      501       20      475 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/not.rs
--rw-r--r--   0      501       20      150 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/null.rs
--rw-r--r--   0      501       20      638 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/search_sorted.rs
--rw-r--r--   0      501       20     1492 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/sort.rs
--rw-r--r--   0      501       20      557 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/take.rs
--rw-r--r--   0      501       20     1528 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/ops/utf8.rs
--rw-r--r--   0      501       20     1351 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/series/series_like.rs
--rw-r--r--   0      501       20    16667 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/mod.rs
--rw-r--r--   0      501       20     2165 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/ops/agg.rs
--rw-r--r--   0      501       20     3729 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/ops/explode.rs
--rw-r--r--   0      501       20     4403 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/ops/groups.rs
--rw-r--r--   0      501       20     2886 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/ops/hash.rs
--rw-r--r--   0      501       20     2483 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/ops/joins/hash_join.rs
--rw-r--r--   0      501       20     3712 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/ops/joins/mod.rs
--rw-r--r--   0      501       20       99 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/ops/mod.rs
--rw-r--r--   0      501       20     3468 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/ops/partition.rs
--rw-r--r--   0      501       20     1804 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/ops/search_sorted.rs
--rw-r--r--   0      501       20      999 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/table/ops/sort.rs
--rw-r--r--   0      501       20     5371 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/utils/arrow.rs
--rw-r--r--   0      501       20       34 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/utils/mod.rs
--rw-r--r--   0      501       20    10065 2023-05-24 05:44:50.000000 getdaft-0.1.3/src/utils/supertype.rs
--rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/__init__.py
--rw-r--r--   0      501       20      299 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/__init__.py
--rw-r--r--   0      501       20      544 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/1.sql
--rw-r--r--   0      501       20      542 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/10.sql
--rw-r--r--   0      501       20      703 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/2.sql
--rw-r--r--   0      501       20      444 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/3.sql
--rw-r--r--   0      501       20      371 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/4.sql
--rw-r--r--   0      501       20      504 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/5.sql
--rw-r--r--   0      501       20      259 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/6.sql
--rw-r--r--   0      501       20      834 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/7.sql
--rw-r--r--   0      501       20      815 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/8.sql
--rw-r--r--   0      501       20      627 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/9.sql
--rw-r--r--   0      501       20       48 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/assets/tpch-sqlite-queries/README.md
--rw-r--r--   0      501       20      604 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/benchmarks/conftest.py
--rw-r--r--   0      501       20     1227 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/benchmarks/test_df_arithmetic.py
--rw-r--r--   0      501       20     2706 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/benchmarks/test_file_read.py
--rw-r--r--   0      501       20     5604 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/benchmarks/test_groups_and_aggs.py
--rw-r--r--   0      501       20     7292 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/benchmarks/test_join.py
--rw-r--r--   0      501       20     2603 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/benchmarks/test_repartition.py
--rw-r--r--   0      501       20     4005 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/benchmarks/test_sort.py
--rw-r--r--   0      501       20     2911 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/conftest.py
--rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/__init__.py
--rw-r--r--   0      501       20    13229 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/assets/311-service-requests.24.csv
--rw-r--r--   0      501       20      255 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/assets/__init__.py
--rw-r--r--   0      501       20      882 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/conftest.py
--rw-r--r--   0      501       20     9268 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_aggregations.py
--rw-r--r--   0      501       20     2979 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_computations.py
--rw-r--r--   0      501       20     1798 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_count_rows.py
--rw-r--r--   0      501       20     7099 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_dataloading.py
--rw-r--r--   0      501       20      800 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_distinct.py
--rw-r--r--   0      501       20     6049 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_filter.py
--rw-r--r--   0      501       20     3810 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_joins.py
--rw-r--r--   0      501       20     2878 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_literals.py
--rw-r--r--   0      501       20    10311 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_pandas_cookbook.py
--rw-r--r--   0      501       20     4148 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_sorting.py
--rw-r--r--   0      501       20     1497 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/cookbook/test_write.py
--rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/__init__.py
--rw-r--r--   0      501       20      751 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/conftest.py
--rw-r--r--   0      501       20      805 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_accessors.py
--rw-r--r--   0      501       20    10308 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_aggregations.py
--rw-r--r--   0      501       20    21893 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_creation.py
--rw-r--r--   0      501       20     1824 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_distinct.py
--rw-r--r--   0      501       20     1428 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_explode.py
--rw-r--r--   0      501       20     1097 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_filter.py
--rw-r--r--   0      501       20     2435 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_getitem.py
--rw-r--r--   0      501       20     4091 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_joins.py
--rw-r--r--   0      501       20      744 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_logical_type.py
--rw-r--r--   0      501       20     4500 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_repr.py
--rw-r--r--   0      501       20      815 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_select.py
--rw-r--r--   0      501       20      656 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_show.py
--rw-r--r--   0      501       20     6364 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_sort.py
--rw-r--r--   0      501       20     3596 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_temporals.py
--rw-r--r--   0      501       20     2385 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_to_integrations.py
--rw-r--r--   0      501       20      850 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/dataframe/test_with_column.py
--rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/__init__.py
--rw-r--r--   0      501       20     1417 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/test_apply.py
--rw-r--r--   0      501       20     3533 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/test_expressions.py
--rw-r--r--   0      501       20     4259 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/test_expressions_projection.py
--rw-r--r--   0      501       20     5019 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/test_udf.py
--rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/__init__.py
--rw-r--r--   0      501       20     6290 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/conftest.py
--rw-r--r--   0      501       20     1363 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/test_aggs.py
--rw-r--r--   0      501       20     2335 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/test_arithmetic.py
--rw-r--r--   0      501       20      853 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/test_compare.py
--rw-r--r--   0      501       20      792 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/test_dt.py
--rw-r--r--   0      501       20      531 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/test_float.py
--rw-r--r--   0      501       20      684 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/test_if_else.py
--rw-r--r--   0      501       20      422 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/test_is_null.py
--rw-r--r--   0      501       20     1176 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/test_logical.py
--rw-r--r--   0      501       20     1544 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/expressions/typing/test_str.py
--rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/integration/__init__.py
--rw-r--r--   0      501       20     4193 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/integration/test_tpch.py
--rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/optimizer/__init__.py
--rw-r--r--   0      501       20     1116 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/optimizer/conftest.py
--rw-r--r--   0      501       20     1666 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/optimizer/test_drop_projections.py
--rw-r--r--   0      501       20     1847 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/optimizer/test_drop_repartition.py
--rw-r--r--   0      501       20     2463 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/optimizer/test_fold_projections.py
--rw-r--r--   0      501       20     7624 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/optimizer/test_prune_columns.py
--rw-r--r--   0      501       20     3597 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/optimizer/test_pushdown_clauses_into_scan.py
--rw-r--r--   0      501       20     1170 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/optimizer/test_pushdown_limit.py
--rw-r--r--   0      501       20     8453 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/optimizer/test_pushdown_predicates.py
--rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/property_based_testing/__init__.py
--rw-r--r--   0      501       20     4575 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/property_based_testing/strategies.py
--rw-r--r--   0      501       20     8895 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/property_based_testing/test_sort.py
--rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/ray/__init__.py
--rw-r--r--   0      501       20     5375 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/ray/test_dask.py
--rw-r--r--   0      501       20     8461 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/ray/test_datasets.py
--rw-r--r--   0      501       20      278 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/__init__.py
--rw-r--r--   0      501       20     9299 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_arithmetic.py
--rw-r--r--   0      501       20     5635 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_cast.py
--rw-r--r--   0      501       20    17207 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_comparisons.py
--rw-r--r--   0      501       20     7188 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_concat.py
--rw-r--r--   0      501       20      864 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_embedding.py
--rw-r--r--   0      501       20     6151 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_filter.py
--rw-r--r--   0      501       20      874 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_float.py
--rw-r--r--   0      501       20     3344 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_hash.py
--rw-r--r--   0      501       20    21522 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_if_else.py
--rw-r--r--   0      501       20      889 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_numeric_ops.py
--rw-r--r--   0      501       20     3418 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_series.py
--rw-r--r--   0      501       20     9173 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_size_bytes.py
--rw-r--r--   0      501       20     2188 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_slice.py
--rw-r--r--   0      501       20     5495 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_sort.py
--rw-r--r--   0      501       20     6111 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_take.py
--rw-r--r--   0      501       20     1934 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_temporal_ops.py
--rw-r--r--   0      501       20     4413 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/series/test_utf8_ops.py
--rw-r--r--   0      501       20      694 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/__init__.py
--rw-r--r--   0      501       20     1070 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_blackbox_kernels.py
--rw-r--r--   0      501       20      426 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_broadcasts.py
--rw-r--r--   0      501       20     2123 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_concat.py
--rw-r--r--   0      501       20     4900 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_eval.py
--rw-r--r--   0      501       20     3930 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_explodes.py
--rw-r--r--   0      501       20     7413 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_filter.py
--rw-r--r--   0      501       20    23407 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_from_py.py
--rw-r--r--   0      501       20      842 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_head.py
--rw-r--r--   0      501       20    10974 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_joins.py
--rw-r--r--   0      501       20     7811 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_partitioning.py
--rw-r--r--   0      501       20      654 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_size_bytes.py
--rw-r--r--   0      501       20    10955 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_sorting.py
--rw-r--r--   0      501       20    20923 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_table_aggs.py
--rw-r--r--   0      501       20    10064 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_table_io.py
--rw-r--r--   0      501       20     5061 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/test_take.py
--rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/utf8/__init__.py
--rw-r--r--   0      501       20     1165 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/utf8/test_compares.py
--rw-r--r--   0      501       20      321 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/table/utf8/test_length.py
--rw-r--r--   0      501       20     3533 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/test_analytics.py
--rw-r--r--   0      501       20      703 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/test_datatypes.py
--rw-r--r--   0      501       20     3542 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/test_schema.py
--rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/udf_library/__init__.py
--rw-r--r--   0      501       20     3989 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/udf_library/test_url_udfs.py
--rw-r--r--   0      501       20      338 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests/utils.py
--rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests_legacy/__init__.py
--rw-r--r--   0      501       20     6988 2023-05-24 05:44:50.000000 getdaft-0.1.3/tests_legacy/test_resource_requests.py
--rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/__init__.py
--rw-r--r--   0      501       20     1633 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/patch_package_version.py
--rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/__init__.py
--rw-r--r--   0      501       20        0 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/_vendor/__init__.py
--rw-r--r--   0      501       20     1125 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/_vendor/wheel/LICENSE.txt
--rw-r--r--   0      501       20       59 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/_vendor/wheel/__init__.py
--rw-r--r--   0      501       20     2499 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/_vendor/wheel/cli/__init__.py
--rw-r--r--   0      501       20     9514 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/_vendor/wheel/cli/convert.py
--rw-r--r--   0      501       20     3113 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/_vendor/wheel/cli/pack.py
--rw-r--r--   0      501       20      662 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/_vendor/wheel/cli/unpack.py
--rw-r--r--   0      501       20     1246 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/_vendor/wheel/pkginfo.py
--rw-r--r--   0      501       20      974 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/_vendor/wheel/util.py
--rw-r--r--   0      501       20     7125 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/_vendor/wheel/wheelfile.py
--rw-r--r--   0      501       20      878 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/fix-and-copy-wheel.py
--rw-r--r--   0      501       20     2981 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/tmpdirs.py
--rw-r--r--   0      501       20     4469 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/tools.py
--rw-r--r--   0      501       20     9484 2023-05-24 05:44:50.000000 getdaft-0.1.3/tools/wheels/wheeltools.py
--rw-r--r--   0      501       20       19 2023-05-24 05:44:50.000000 getdaft-0.1.3/tutorials/.gitignore
--rw-r--r--   0      501       20    19576 2023-05-24 05:44:50.000000 getdaft-0.1.3/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb
--rw-r--r--   0      501       20    12068 2023-05-24 05:44:50.000000 getdaft-0.1.3/tutorials/image_querying/top_n_red_color.ipynb
--rw-r--r--   0      501       20    98730 2023-05-24 05:44:50.000000 getdaft-0.1.3/tutorials/mnist.ipynb
--rw-r--r--   0      501       20    11847 2023-05-24 05:44:50.000000 getdaft-0.1.3/tutorials/text_to_image/text_to_image_generation.ipynb
--rw-r--r--   0      501       20     9134 2023-05-24 05:44:50.000000 getdaft-0.1.3/tutorials/text_to_image/using_cloud_with_ray.ipynb
--rw-r--r--   0      501       20    32068 2023-05-24 05:44:49.000000 getdaft-0.1.3/Cargo.lock
--rw-r--r--   0        0        0     7325 1970-01-01 00:00:00.000000 getdaft-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 getdaft-0.1.4/Cargo.toml
+-rw-r--r--   0      501       20      834 2023-06-03 10:38:04.000000 getdaft-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0      501       20      595 2023-06-03 10:38:04.000000 getdaft-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0      501       20      428 2023-06-03 10:38:04.000000 getdaft-0.1.4/.github/dependabot.yml
+-rw-r--r--   0      501       20     1333 2023-06-03 10:38:04.000000 getdaft-0.1.4/.github/workflows/broken-link-checker.yml
+-rw-r--r--   0      501       20     3378 2023-06-03 10:38:04.000000 getdaft-0.1.4/.github/workflows/daft-profiling.yml
+-rw-r--r--   0      501       20     1627 2023-06-03 10:38:04.000000 getdaft-0.1.4/.github/workflows/notebook-checker.yml
+-rw-r--r--   0      501       20     2194 2023-06-03 10:38:04.000000 getdaft-0.1.4/.github/workflows/property-based-tests.yml
+-rw-r--r--   0      501       20    12886 2023-06-03 10:38:04.000000 getdaft-0.1.4/.github/workflows/python-package.yml
+-rw-r--r--   0      501       20     6182 2023-06-03 10:38:04.000000 getdaft-0.1.4/.github/workflows/python-publish.yml
+-rw-r--r--   0      501       20     2638 2023-06-03 10:38:04.000000 getdaft-0.1.4/.github/workflows/ray-compatibility.yml
+-rw-r--r--   0      501       20      300 2023-06-03 10:38:04.000000 getdaft-0.1.4/.gitignore
+-rw-r--r--   0      501       20     2126 2023-06-03 10:38:04.000000 getdaft-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0      501       20      205 2023-06-03 10:38:04.000000 getdaft-0.1.4/.readthedocs.yaml
+-rw-r--r--   0      501       20     1550 2023-06-03 10:38:04.000000 getdaft-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0      501       20    11357 2023-06-03 10:38:04.000000 getdaft-0.1.4/LICENSE
+-rw-r--r--   0      501       20     1295 2023-06-03 10:38:04.000000 getdaft-0.1.4/Makefile
+-rw-r--r--   0      501       20     6126 2023-06-03 10:38:04.000000 getdaft-0.1.4/README.rst
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/benchmarking/__init__.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/benchmarking/tpch/__init__.py
+-rw-r--r--   0      501       20     9495 2023-06-03 10:38:04.000000 getdaft-0.1.4/benchmarking/tpch/__main__.py
+-rw-r--r--   0      501       20    12428 2023-06-03 10:38:04.000000 getdaft-0.1.4/benchmarking/tpch/answers.py
+-rw-r--r--   0      501       20    12140 2023-06-03 10:38:04.000000 getdaft-0.1.4/benchmarking/tpch/data_generation.py
+-rw-r--r--   0      501       20     4573 2023-06-03 10:38:04.000000 getdaft-0.1.4/benchmarking/tpch/pipelined_data_generation.py
+-rw-r--r--   0      501       20     1436 2023-06-03 10:38:04.000000 getdaft-0.1.4/ci/upload_wheels.sh
+-rw-r--r--   0      501       20      440 2023-06-03 10:38:04.000000 getdaft-0.1.4/codecov.yml
+-rw-r--r--   0      501       20     2092 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/__init__.py
+-rw-r--r--   0      501       20     6724 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/analytics.py
+-rw-r--r--   0      501       20     3935 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/api_annotations.py
+-rw-r--r--   0      501       20    10591 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/arrow_utils.py
+-rw-r--r--   0      501       20     5395 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/context.py
+-rw-r--r--   0      501       20     3403 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/convert.py
+-rw-r--r--   0      501       20      724 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/daft.pyi
+-rw-r--r--   0      501       20       94 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/dataframe/__init__.py
+-rw-r--r--   0      501       20    49646 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/dataframe/dataframe.py
+-rw-r--r--   0      501       20      306 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/dataframe/preview.py
+-rw-r--r--   0      501       20      850 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/datasources.py
+-rw-r--r--   0      501       20    13221 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/datatype.py
+-rw-r--r--   0      501       20       84 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/errors.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/execution/__init__.py
+-rw-r--r--   0      501       20    24774 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/execution/execution_step.py
+-rw-r--r--   0      501       20     4231 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/execution/logical_op_runners.py
+-rw-r--r--   0      501       20    28173 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/execution/physical_plan.py
+-rw-r--r--   0      501       20     6110 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/execution/physical_plan_factory.py
+-rw-r--r--   0      501       20      170 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/expressions/__init__.py
+-rw-r--r--   0      501       20    25203 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/expressions/expressions.py
+-rw-r--r--   0      501       20      572 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/expressions/testing.py
+-rw-r--r--   0      501       20    12728 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/filesystem.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/internal/__init__.py
+-rw-r--r--   0      501       20      509 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/internal/gpu.py
+-rw-r--r--   0      501       20     1804 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/internal/rule.py
+-rw-r--r--   0      501       20     2030 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/internal/rule_runner.py
+-rw-r--r--   0      501       20     3490 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/internal/treenode.py
+-rw-r--r--   0      501       20      263 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/io/__init__.py
+-rw-r--r--   0      501       20     1682 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/io/_csv.py
+-rw-r--r--   0      501       20     1223 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/io/_json.py
+-rw-r--r--   0      501       20     2032 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/io/common.py
+-rw-r--r--   0      501       20     2034 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/io/file_path.py
+-rw-r--r--   0      501       20     1243 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/io/parquet.py
+-rw-r--r--   0      501       20      264 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/logging.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/logical/__init__.py
+-rw-r--r--   0      501       20     8601 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/logical/aggregation_plan_builder.py
+-rw-r--r--   0      501       20    37496 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/logical/logical_plan.py
+-rw-r--r--   0      501       20     1492 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/logical/map_partition_ops.py
+-rw-r--r--   0      501       20    19183 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/logical/optimizer.py
+-rw-r--r--   0      501       20     3625 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/logical/schema.py
+-rw-r--r--   0      501       20       99 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/pickle/__init__.py
+-rw-r--r--   0      501       20    34760 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/pickle/cloudpickle.py
+-rw-r--r--   0      501       20    34262 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/pickle/cloudpickle_fast.py
+-rw-r--r--   0      501       20      639 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/pickle/compat.py
+-rw-r--r--   0      501       20      312 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/pickle/pickle.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/py.typed
+-rw-r--r--   0      501       20     2036 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/resource_request.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/runners/__init__.py
+-rw-r--r--   0      501       20     5708 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/runners/partitioning.py
+-rw-r--r--   0      501       20     1488 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/runners/profiler.py
+-rw-r--r--   0      501       20    13059 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/runners/pyrunner.py
+-rw-r--r--   0      501       20    25296 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/runners/ray_runner.py
+-rw-r--r--   0      501       20      918 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/runners/runner.py
+-rw-r--r--   0      501       20     4324 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/runners/runner_io.py
+-rw-r--r--   0      501       20    19568 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/series.py
+-rw-r--r--   0      501       20       82 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/table/__init__.py
+-rw-r--r--   0      501       20    13765 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/table/table.py
+-rw-r--r--   0      501       20     9457 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/table/table_io.py
+-rw-r--r--   0      501       20     7263 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/udf.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/udf_library/__init__.py
+-rw-r--r--   0      501       20     3486 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/udf_library/url_udfs.py
+-rw-r--r--   0      501       20     2796 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/utils.py
+-rw-r--r--   0      501       20      183 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/viz/__init__.py
+-rw-r--r--   0      501       20     1699 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/viz/dataframe_display.py
+-rw-r--r--   0      501       20     1517 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/viz/html_viz_hooks.py
+-rw-r--r--   0      501       20     6592 2023-06-03 10:38:04.000000 getdaft-0.1.4/daft/viz/repr.py
+-rw-r--r--   0      501       20      148 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/CONTRIBUTING.md
+-rw-r--r--   0      501       20      638 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/Makefile
+-rw-r--r--   0      501       20    71692 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/10-min.ipynb
+-rw-r--r--   0      501       20      389 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/custom-function-signatures.css
+-rw-r--r--   0      501       20      565 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/daft-favicon.png
+-rw-r--r--   0      501       20     7804 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/daft-logo.png
+-rw-r--r--   0      501       20    42148 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/daft_illustration.png
+-rw-r--r--   0      501       20    25200 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/execution_model.png
+-rw-r--r--   0      501       20     1901 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/header.css
+-rw-r--r--   0      501       20    32864 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/high_level_architecture.png
+-rw-r--r--   0      501       20      343 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/icon-menu-close.svg
+-rw-r--r--   0      501       20      333 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/icon-menu-dots.svg
+-rw-r--r--   0      501       20    18177 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/in_memory_data_representation.png
+-rw-r--r--   0      501       20      786 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/mobile-menu.js
+-rw-r--r--   0      501       20     9142 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/tpch-1000sf.html
+-rw-r--r--   0      501       20     9647 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/tpch-100sf.html
+-rw-r--r--   0      501       20     8757 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_static/tpch-nodes-count-daft-1000-sf.html
+-rw-r--r--   0      501       20      856 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_templates/layout.html
+-rw-r--r--   0      501       20      994 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_templates/sections/header.html
+-rw-r--r--   0      501       20      957 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/_templates/sections/mobile-menu.html
+-rw-r--r--   0      501       20      325 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/api_docs/context.rst
+-rw-r--r--   0      501       20     2564 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/api_docs/dataframe.rst
+-rw-r--r--   0      501       20     1881 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/api_docs/datatype.rst
+-rw-r--r--   0      501       20     3474 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/api_docs/expressions.rst
+-rw-r--r--   0      501       20      784 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/api_docs/groupby.rst
+-rw-r--r--   0      501       20      136 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/api_docs/index.rst
+-rw-r--r--   0      501       20     1457 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/api_docs/input_output.rst
+-rw-r--r--   0      501       20       88 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/api_docs/udf.rst
+-rw-r--r--   0      501       20    14528 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/benchmarks/index.rst
+-rw-r--r--   0      501       20     3547 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/conf.py
+-rw-r--r--   0      501       20     4964 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/dataframe_comparison.rst
+-rw-r--r--   0      501       20     1666 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/index.rst
+-rw-r--r--   0      501       20     1089 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/install.rst
+-rw-r--r--   0      501       20      743 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/index.rst
+-rw-r--r--   0      501       20     7586 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/key_concepts.rst
+-rw-r--r--   0      501       20     1398 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/tutorials.rst
+-rw-r--r--   0      501       20     1388 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/user_guides/aggregations.rst
+-rw-r--r--   0      501       20     6686 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/user_guides/dataframe-operations.rst
+-rw-r--r--   0      501       20     4695 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/user_guides/datatypes.rst
+-rw-r--r--   0      501       20     9131 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/user_guides/expressions.rst
+-rw-r--r--   0      501       20     7829 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/user_guides/intro-dataframes.rst
+-rw-r--r--   0      501       20      206 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/user_guides/partitioning.rst
+-rw-r--r--   0      501       20     3190 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/user_guides/read-write.rst
+-rw-r--r--   0      501       20     1257 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/user_guides/scaling-up.rst
+-rw-r--r--   0      501       20     8691 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/user_guides/udf.rst
+-rw-r--r--   0      501       20     1577 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/learn/user_guides.rst
+-rw-r--r--   0      501       20     3575 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.13.rst
+-rw-r--r--   0      501       20     2241 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.14.rst
+-rw-r--r--   0      501       20     1913 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.16.rst
+-rw-r--r--   0      501       20     1750 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.17.rst
+-rw-r--r--   0      501       20     2100 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.18.rst
+-rw-r--r--   0      501       20     3647 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.19.rst
+-rw-r--r--   0      501       20     4240 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.20.rst
+-rw-r--r--   0      501       20     4633 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.21.rst
+-rw-r--r--   0      501       20     8016 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.22.rst
+-rw-r--r--   0      501       20     5385 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.23.rst
+-rw-r--r--   0      501       20    11759 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.0.24.rst
+-rw-r--r--   0      501       20     4750 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.1.0.rst
+-rw-r--r--   0      501       20     2411 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.1.1.rst
+-rw-r--r--   0      501       20     2557 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.1.2.rst
+-rw-r--r--   0      501       20      839 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.1.3.rst
+-rw-r--r--   0      501       20     3065 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/0.1.4.rst
+-rw-r--r--   0      501       20      935 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/_template.rst
+-rw-r--r--   0      501       20      350 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/release_notes/index.rst
+-rw-r--r--   0      501       20     6574 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/technical_architecture.rst
+-rw-r--r--   0      501       20     1316 2023-06-03 10:38:04.000000 getdaft-0.1.4/docs/source/telemetry.rst
+-rw-r--r--   0      501       20     1873 2023-06-03 10:38:04.000000 getdaft-0.1.4/pyproject.toml
+-rw-r--r--   0      501       20      843 2023-06-03 10:38:04.000000 getdaft-0.1.4/requirements-dev.txt
+-rw-r--r--   0      501       20       98 2023-06-03 10:38:04.000000 getdaft-0.1.4/rust-toolchain.toml
+-rw-r--r--   0      501       20     4732 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/from.rs
+-rw-r--r--   0      501       20      734 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/iterator.rs
+-rw-r--r--   0      501       20     2945 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/mod.rs
+-rw-r--r--   0      501       20      257 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/abs.rs
+-rw-r--r--   0      501       20      726 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/apply.rs
+-rw-r--r--   0      501       20      841 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/arange.rs
+-rw-r--r--   0      501       20     6964 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/arithmetic.rs
+-rw-r--r--   0      501       20     3048 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/arrow2/comparison.rs
+-rw-r--r--   0      501       20       34 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/arrow2/mod.rs
+-rw-r--r--   0      501       20       19 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/arrow2/sort/mod.rs
+-rw-r--r--   0      501       20     3482 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/arrow2/sort/primitive/common.rs
+-rw-r--r--   0      501       20      723 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/arrow2/sort/primitive/indices.rs
+-rw-r--r--   0      501       20       47 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/arrow2/sort/primitive/mod.rs
+-rw-r--r--   0      501       20     8075 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/arrow2/sort/primitive/sort.rs
+-rw-r--r--   0      501       20     3407 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/as_arrow.rs
+-rw-r--r--   0      501       20    11304 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/broadcast.rs
+-rw-r--r--   0      501       20    26977 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/cast.rs
+-rw-r--r--   0      501       20    11017 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/compare_agg.rs
+-rw-r--r--   0      501       20    47218 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/comparison.rs
+-rw-r--r--   0      501       20     1634 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/concat.rs
+-rw-r--r--   0      501       20     5982 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/concat_agg.rs
+-rw-r--r--   0      501       20     1433 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/count.rs
+-rw-r--r--   0      501       20     1550 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/date.rs
+-rw-r--r--   0      501       20     3335 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/filter.rs
+-rw-r--r--   0      501       20     1264 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/float.rs
+-rw-r--r--   0      501       20     1936 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/full.rs
+-rw-r--r--   0      501       20     4112 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/groups.rs
+-rw-r--r--   0      501       20     1515 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/hash.rs
+-rw-r--r--   0      501       20    12551 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/if_else.rs
+-rw-r--r--   0      501       20    16405 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/image.rs
+-rw-r--r--   0      501       20     1058 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/len.rs
+-rw-r--r--   0      501       20     3446 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/list.rs
+-rw-r--r--   0      501       20     3360 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/list_agg.rs
+-rw-r--r--   0      501       20     1622 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/mean.rs
+-rw-r--r--   0      501       20     2617 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/mod.rs
+-rw-r--r--   0      501       20     1314 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/null.rs
+-rw-r--r--   0      501       20     3819 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/pairwise.rs
+-rw-r--r--   0      501       20      484 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/search_sorted.rs
+-rw-r--r--   0      501       20    19387 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/sort.rs
+-rw-r--r--   0      501       20     2383 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/sum.rs
+-rw-r--r--   0      501       20    17241 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/take.rs
+-rw-r--r--   0      501       20     5279 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/ops/utf8.rs
+-rw-r--r--   0      501       20      995 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/pseudo_arrow/compute.rs
+-rw-r--r--   0      501       20    13611 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/pseudo_arrow/mod.rs
+-rw-r--r--   0      501       20     2502 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/array/pseudo_arrow/python.rs
+-rw-r--r--   0      501       20    14860 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/datatypes/dtype.rs
+-rw-r--r--   0      501       20     2012 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/datatypes/field.rs
+-rw-r--r--   0      501       20     4549 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/datatypes/image_mode.rs
+-rw-r--r--   0      501       20     2889 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/datatypes/logical.rs
+-rw-r--r--   0      501       20     9088 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/datatypes/matching.rs
+-rw-r--r--   0      501       20     6836 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/datatypes/mod.rs
+-rw-r--r--   0      501       20     1083 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/datatypes/time_unit.rs
+-rw-r--r--   0      501       20      273 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/README.md
+-rw-r--r--   0      501       20     1474 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/arithmetic.rs
+-rw-r--r--   0      501       20    21828 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/expr.rs
+-rw-r--r--   0      501       20     1431 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/float/is_nan.rs
+-rw-r--r--   0      501       20      587 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/float/mod.rs
+-rw-r--r--   0      501       20      496 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/image/decode.rs
+-rw-r--r--   0      501       20      914 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/image/mod.rs
+-rw-r--r--   0      501       20     1071 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/image/resize.rs
+-rw-r--r--   0      501       20     1122 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/list/explode.rs
+-rw-r--r--   0      501       20      597 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/list/mod.rs
+-rw-r--r--   0      501       20     1944 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/mod.rs
+-rw-r--r--   0      501       20     1188 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/numeric/abs.rs
+-rw-r--r--   0      501       20      580 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/numeric/mod.rs
+-rw-r--r--   0      501       20      676 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/python/mod.rs
+-rw-r--r--   0      501       20     2050 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/python/partial_udf.rs
+-rw-r--r--   0      501       20     2779 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/python/udf.rs
+-rw-r--r--   0      501       20     1320 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/temporal/day.rs
+-rw-r--r--   0      501       20     1348 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/temporal/day_of_week.rs
+-rw-r--r--   0      501       20     1425 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/temporal/mod.rs
+-rw-r--r--   0      501       20     1330 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/temporal/month.rs
+-rw-r--r--   0      501       20     1324 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/temporal/year.rs
+-rw-r--r--   0      501       20     1627 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/utf8/contains.rs
+-rw-r--r--   0      501       20     1627 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/utf8/endswith.rs
+-rw-r--r--   0      501       20     1346 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/utf8/length.rs
+-rw-r--r--   0      501       20     1524 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/utf8/mod.rs
+-rw-r--r--   0      501       20     1637 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/functions/utf8/startswith.rs
+-rw-r--r--   0      501       20     4961 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/lit.rs
+-rw-r--r--   0      501       20      233 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/mod.rs
+-rw-r--r--   0      501       20     5298 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/optimization.rs
+-rw-r--r--   0      501       20     1982 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/dsl/pyobject.rs
+-rw-r--r--   0      501       20     1681 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/error.rs
+-rw-r--r--   0      501       20     7867 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/ffi.rs
+-rw-r--r--   0      501       20     6022 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/kernels/hashing.rs
+-rw-r--r--   0      501       20       54 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/kernels/mod.rs
+-rw-r--r--   0      501       20    12159 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/kernels/search_sorted.rs
+-rw-r--r--   0      501       20     3917 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/kernels/utf8.rs
+-rw-r--r--   0      501       20     1117 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/lib.rs
+-rw-r--r--   0      501       20     6900 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/python/datatype.rs
+-rw-r--r--   0      501       20      307 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/python/error.rs
+-rw-r--r--   0      501       20    10801 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/python/expr.rs
+-rw-r--r--   0      501       20     1644 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/python/field.rs
+-rw-r--r--   0      501       20      802 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/python/mod.rs
+-rw-r--r--   0      501       20     2425 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/python/schema.rs
+-rw-r--r--   0      501       20     9789 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/python/series.rs
+-rw-r--r--   0      501       20    10760 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/python/table.rs
+-rw-r--r--   0      501       20     3016 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/schema.rs
+-rw-r--r--   0      501       20    10158 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/array_impl/data_array.rs
+-rw-r--r--   0      501       20     5459 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/array_impl/logical_array.rs
+-rw-r--r--   0      501       20      161 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/array_impl/mod.rs
+-rw-r--r--   0      501       20     2099 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/from.rs
+-rw-r--r--   0      501       20     2190 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/mod.rs
+-rw-r--r--   0      501       20      902 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/abs.rs
+-rw-r--r--   0      501       20     5207 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/agg.rs
+-rw-r--r--   0      501       20     6298 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/arithmetic.rs
+-rw-r--r--   0      501       20     1925 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/broadcast.rs
+-rw-r--r--   0      501       20      194 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/cast.rs
+-rw-r--r--   0      501       20     2609 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/comparison.rs
+-rw-r--r--   0      501       20     1558 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/concat.rs
+-rw-r--r--   0      501       20     1822 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/date.rs
+-rw-r--r--   0      501       20     3612 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/downcast.rs
+-rw-r--r--   0      501       20      697 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/filter.rs
+-rw-r--r--   0      501       20      399 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/float.rs
+-rw-r--r--   0      501       20      432 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/groups.rs
+-rw-r--r--   0      501       20      412 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/hash.rs
+-rw-r--r--   0      501       20      314 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/if_else.rs
+-rw-r--r--   0      501       20     1024 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/image.rs
+-rw-r--r--   0      501       20      229 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/len.rs
+-rw-r--r--   0      501       20     1925 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/list.rs
+-rw-r--r--   0      501       20     2367 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/mod.rs
+-rw-r--r--   0      501       20      475 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/not.rs
+-rw-r--r--   0      501       20      150 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/null.rs
+-rw-r--r--   0      501       20      638 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/search_sorted.rs
+-rw-r--r--   0      501       20     1492 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/sort.rs
+-rw-r--r--   0      501       20      557 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/take.rs
+-rw-r--r--   0      501       20     1528 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/ops/utf8.rs
+-rw-r--r--   0      501       20     1351 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/series/series_like.rs
+-rw-r--r--   0      501       20    16798 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/mod.rs
+-rw-r--r--   0      501       20     2165 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/ops/agg.rs
+-rw-r--r--   0      501       20     3729 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/ops/explode.rs
+-rw-r--r--   0      501       20     4403 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/ops/groups.rs
+-rw-r--r--   0      501       20     2886 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/ops/hash.rs
+-rw-r--r--   0      501       20     2483 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/ops/joins/hash_join.rs
+-rw-r--r--   0      501       20     3712 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/ops/joins/mod.rs
+-rw-r--r--   0      501       20       99 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/ops/mod.rs
+-rw-r--r--   0      501       20     3468 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/ops/partition.rs
+-rw-r--r--   0      501       20     1804 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/ops/search_sorted.rs
+-rw-r--r--   0      501       20      999 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/table/ops/sort.rs
+-rw-r--r--   0      501       20     5371 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/utils/arrow.rs
+-rw-r--r--   0      501       20       34 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/utils/mod.rs
+-rw-r--r--   0      501       20    10065 2023-06-03 10:38:04.000000 getdaft-0.1.4/src/utils/supertype.rs
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/__init__.py
+-rw-r--r--   0      501       20      299 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/__init__.py
+-rw-r--r--   0      501       20      544 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/1.sql
+-rw-r--r--   0      501       20      542 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/10.sql
+-rw-r--r--   0      501       20      703 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/2.sql
+-rw-r--r--   0      501       20      444 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/3.sql
+-rw-r--r--   0      501       20      371 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/4.sql
+-rw-r--r--   0      501       20      504 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/5.sql
+-rw-r--r--   0      501       20      259 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/6.sql
+-rw-r--r--   0      501       20      834 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/7.sql
+-rw-r--r--   0      501       20      815 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/8.sql
+-rw-r--r--   0      501       20      627 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/9.sql
+-rw-r--r--   0      501       20       48 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/assets/tpch-sqlite-queries/README.md
+-rw-r--r--   0      501       20      604 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/benchmarks/conftest.py
+-rw-r--r--   0      501       20     1227 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/benchmarks/test_df_arithmetic.py
+-rw-r--r--   0      501       20     2706 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/benchmarks/test_file_read.py
+-rw-r--r--   0      501       20     5604 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/benchmarks/test_groups_and_aggs.py
+-rw-r--r--   0      501       20     7292 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/benchmarks/test_join.py
+-rw-r--r--   0      501       20     2603 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/benchmarks/test_repartition.py
+-rw-r--r--   0      501       20     4005 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/benchmarks/test_sort.py
+-rw-r--r--   0      501       20     2911 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/conftest.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/__init__.py
+-rw-r--r--   0      501       20    13229 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/assets/311-service-requests.24.csv
+-rw-r--r--   0      501       20      255 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/assets/__init__.py
+-rw-r--r--   0      501       20      882 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/conftest.py
+-rw-r--r--   0      501       20     9268 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_aggregations.py
+-rw-r--r--   0      501       20     2979 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_computations.py
+-rw-r--r--   0      501       20     1798 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_count_rows.py
+-rw-r--r--   0      501       20     7099 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_dataloading.py
+-rw-r--r--   0      501       20      800 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_distinct.py
+-rw-r--r--   0      501       20     6049 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_filter.py
+-rw-r--r--   0      501       20     3810 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_joins.py
+-rw-r--r--   0      501       20     2878 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_literals.py
+-rw-r--r--   0      501       20    10311 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_pandas_cookbook.py
+-rw-r--r--   0      501       20     4148 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_sorting.py
+-rw-r--r--   0      501       20     1497 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/cookbook/test_write.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/__init__.py
+-rw-r--r--   0      501       20      751 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/conftest.py
+-rw-r--r--   0      501       20      805 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_accessors.py
+-rw-r--r--   0      501       20    10308 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_aggregations.py
+-rw-r--r--   0      501       20    21893 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_creation.py
+-rw-r--r--   0      501       20     1824 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_distinct.py
+-rw-r--r--   0      501       20     1428 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_explode.py
+-rw-r--r--   0      501       20     1097 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_filter.py
+-rw-r--r--   0      501       20     2435 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_getitem.py
+-rw-r--r--   0      501       20     4091 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_joins.py
+-rw-r--r--   0      501       20     1940 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_logical_type.py
+-rw-r--r--   0      501       20      223 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_repartition.py
+-rw-r--r--   0      501       20     4858 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_repr.py
+-rw-r--r--   0      501       20      815 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_select.py
+-rw-r--r--   0      501       20      656 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_show.py
+-rw-r--r--   0      501       20     6364 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_sort.py
+-rw-r--r--   0      501       20     3596 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_temporals.py
+-rw-r--r--   0      501       20     2385 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_to_integrations.py
+-rw-r--r--   0      501       20      850 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/dataframe/test_with_column.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/__init__.py
+-rw-r--r--   0      501       20     1417 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/test_apply.py
+-rw-r--r--   0      501       20     3533 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/test_expressions.py
+-rw-r--r--   0      501       20     4259 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/test_expressions_projection.py
+-rw-r--r--   0      501       20     5019 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/test_udf.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/__init__.py
+-rw-r--r--   0      501       20     6290 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/conftest.py
+-rw-r--r--   0      501       20     1363 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/test_aggs.py
+-rw-r--r--   0      501       20     2335 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/test_arithmetic.py
+-rw-r--r--   0      501       20      853 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/test_compare.py
+-rw-r--r--   0      501       20      792 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/test_dt.py
+-rw-r--r--   0      501       20      531 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/test_float.py
+-rw-r--r--   0      501       20      684 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/test_if_else.py
+-rw-r--r--   0      501       20      422 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/test_is_null.py
+-rw-r--r--   0      501       20     1176 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/test_logical.py
+-rw-r--r--   0      501       20     1544 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/expressions/typing/test_str.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/integration/__init__.py
+-rw-r--r--   0      501       20     4193 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/integration/test_tpch.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/optimizer/__init__.py
+-rw-r--r--   0      501       20     1116 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/optimizer/conftest.py
+-rw-r--r--   0      501       20     1666 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/optimizer/test_drop_projections.py
+-rw-r--r--   0      501       20     1847 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/optimizer/test_drop_repartition.py
+-rw-r--r--   0      501       20     2463 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/optimizer/test_fold_projections.py
+-rw-r--r--   0      501       20     7624 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/optimizer/test_prune_columns.py
+-rw-r--r--   0      501       20     3597 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/optimizer/test_pushdown_clauses_into_scan.py
+-rw-r--r--   0      501       20     1170 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/optimizer/test_pushdown_limit.py
+-rw-r--r--   0      501       20     8453 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/optimizer/test_pushdown_predicates.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/property_based_testing/__init__.py
+-rw-r--r--   0      501       20     4575 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/property_based_testing/strategies.py
+-rw-r--r--   0      501       20     8895 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/property_based_testing/test_sort.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/ray/__init__.py
+-rw-r--r--   0      501       20     5375 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/ray/test_dask.py
+-rw-r--r--   0      501       20     8461 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/ray/test_datasets.py
+-rw-r--r--   0      501       20      278 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/__init__.py
+-rw-r--r--   0      501       20     9299 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_arithmetic.py
+-rw-r--r--   0      501       20     8932 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_cast.py
+-rw-r--r--   0      501       20    17207 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_comparisons.py
+-rw-r--r--   0      501       20     7188 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_concat.py
+-rw-r--r--   0      501       20      864 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_embedding.py
+-rw-r--r--   0      501       20     6151 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_filter.py
+-rw-r--r--   0      501       20      874 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_float.py
+-rw-r--r--   0      501       20     3344 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_hash.py
+-rw-r--r--   0      501       20    21522 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_if_else.py
+-rw-r--r--   0      501       20     9303 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_image.py
+-rw-r--r--   0      501       20      889 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_numeric_ops.py
+-rw-r--r--   0      501       20     3418 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_series.py
+-rw-r--r--   0      501       20     9173 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_size_bytes.py
+-rw-r--r--   0      501       20     2188 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_slice.py
+-rw-r--r--   0      501       20     5495 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_sort.py
+-rw-r--r--   0      501       20     6111 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_take.py
+-rw-r--r--   0      501       20     1934 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_temporal_ops.py
+-rw-r--r--   0      501       20     4413 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/series/test_utf8_ops.py
+-rw-r--r--   0      501       20      694 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/__init__.py
+-rw-r--r--   0      501       20     1070 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_blackbox_kernels.py
+-rw-r--r--   0      501       20      426 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_broadcasts.py
+-rw-r--r--   0      501       20     2123 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_concat.py
+-rw-r--r--   0      501       20     4900 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_eval.py
+-rw-r--r--   0      501       20     3930 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_explodes.py
+-rw-r--r--   0      501       20     7413 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_filter.py
+-rw-r--r--   0      501       20    23374 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_from_py.py
+-rw-r--r--   0      501       20      842 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_head.py
+-rw-r--r--   0      501       20    10974 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_joins.py
+-rw-r--r--   0      501       20     7811 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_partitioning.py
+-rw-r--r--   0      501       20      654 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_size_bytes.py
+-rw-r--r--   0      501       20    10955 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_sorting.py
+-rw-r--r--   0      501       20    20923 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_table_aggs.py
+-rw-r--r--   0      501       20    10064 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_table_io.py
+-rw-r--r--   0      501       20     5061 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/test_take.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/utf8/__init__.py
+-rw-r--r--   0      501       20     1165 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/utf8/test_compares.py
+-rw-r--r--   0      501       20      321 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/table/utf8/test_length.py
+-rw-r--r--   0      501       20     3533 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/test_analytics.py
+-rw-r--r--   0      501       20      703 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/test_datatypes.py
+-rw-r--r--   0      501       20     3542 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/test_schema.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/udf_library/__init__.py
+-rw-r--r--   0      501       20     3777 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/udf_library/test_url_udfs.py
+-rw-r--r--   0      501       20      338 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests/utils.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests_legacy/__init__.py
+-rw-r--r--   0      501       20     6988 2023-06-03 10:38:04.000000 getdaft-0.1.4/tests_legacy/test_resource_requests.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/__init__.py
+-rw-r--r--   0      501       20     1633 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/patch_package_version.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/__init__.py
+-rw-r--r--   0      501       20        0 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/_vendor/__init__.py
+-rw-r--r--   0      501       20     1125 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/_vendor/wheel/LICENSE.txt
+-rw-r--r--   0      501       20       59 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/_vendor/wheel/__init__.py
+-rw-r--r--   0      501       20     2499 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/_vendor/wheel/cli/__init__.py
+-rw-r--r--   0      501       20     9514 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/_vendor/wheel/cli/convert.py
+-rw-r--r--   0      501       20     3113 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/_vendor/wheel/cli/pack.py
+-rw-r--r--   0      501       20      662 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/_vendor/wheel/cli/unpack.py
+-rw-r--r--   0      501       20     1246 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/_vendor/wheel/pkginfo.py
+-rw-r--r--   0      501       20      974 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/_vendor/wheel/util.py
+-rw-r--r--   0      501       20     7125 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/_vendor/wheel/wheelfile.py
+-rw-r--r--   0      501       20      878 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/fix-and-copy-wheel.py
+-rw-r--r--   0      501       20     2981 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/tmpdirs.py
+-rw-r--r--   0      501       20     4469 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/tools.py
+-rw-r--r--   0      501       20     9484 2023-06-03 10:38:04.000000 getdaft-0.1.4/tools/wheels/wheeltools.py
+-rw-r--r--   0      501       20       19 2023-06-03 10:38:04.000000 getdaft-0.1.4/tutorials/.gitignore
+-rw-r--r--   0      501       20    19576 2023-06-03 10:38:04.000000 getdaft-0.1.4/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb
+-rw-r--r--   0      501       20    12068 2023-06-03 10:38:04.000000 getdaft-0.1.4/tutorials/image_querying/top_n_red_color.ipynb
+-rw-r--r--   0      501       20    98730 2023-06-03 10:38:04.000000 getdaft-0.1.4/tutorials/mnist.ipynb
+-rw-r--r--   0      501       20    11847 2023-06-03 10:38:04.000000 getdaft-0.1.4/tutorials/text_to_image/text_to_image_generation.ipynb
+-rw-r--r--   0      501       20     9134 2023-06-03 10:38:04.000000 getdaft-0.1.4/tutorials/text_to_image/using_cloud_with_ray.ipynb
+-rw-r--r--   0      501       20    34807 2023-06-03 10:38:04.000000 getdaft-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0     7325 1970-01-01 00:00:00.000000 getdaft-0.1.4/PKG-INFO
```

### Comparing `getdaft-0.1.3/Cargo.toml` & `getdaft-0.1.4/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 [dependencies]
 dyn-clone = "1.0.11"
 fnv = "1.0.7"
+ndarray = "0.15.6"
+num-derive = "0.3.3"
 prettytable-rs = "^0.10"
 pyo3-log = "0.8.1"
 rand = "^0.8"
 serde_json = "1.0.96"
 
 [features]
 default = [ "python",]
@@ -16,36 +18,41 @@
 
 [net]
 git-fetch-with-cli = true
 
 [package]
 edition = "2021"
 name = "daft"
-version = "0.1.3"
+version = "0.1.4"
 
 [dependencies.arrow2]
 branch = "clark/expand-casting-support"
-features = [ "compute", "io_ipc",]
+features = [ "compute_take", "compute_cast", "compute_aggregate", "compute_if_then_else", "compute_sort", "compute_filter", "compute_temporal", "compute_comparison", "compute_arithmetics", "compute_concatenate", "io_ipc",]
 git = "https://github.com/Eventual-Inc/arrow2"
 package = "arrow2"
 version = "0.17.1"
 
 [dependencies.bincode]
 version = "1.3.3"
 
+[dependencies.image]
+default-features = false
+features = [ "gif", "jpeg", "ico", "png", "tiff", "webp", "bmp", "hdr",]
+version = "0.24.6"
+
 [dependencies.indexmap]
 features = [ "serde",]
 version = "1.9.2"
 
 [dependencies.lazy_static]
 version = "1.4.0"
 
 [dependencies.log]
 features = [ "std",]
-version = "0.4.17"
+version = "0.4.18"
 
 [dependencies.num-traits]
 version = "0.2"
 
 [dependencies.numpy]
 optional = true
 version = "0.18"
```

### Comparing `getdaft-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md` & `getdaft-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md` & `getdaft-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/.github/workflows/broken-link-checker.yml` & `getdaft-0.1.4/.github/workflows/broken-link-checker.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/.github/workflows/daft-profiling.yml` & `getdaft-0.1.4/.github/workflows/daft-profiling.yml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     branches: [main]
   workflow_dispatch:
 
 env:
   DAFT_ANALYTICS_ENABLED: '0'
   TPCH_SCALE_FACTOR: '4'
   TPCH_NUM_PARTS: '32'
-  PYTHON_VERSION: '3.8'
+  PYTHON_VERSION: '3.9'
 
 
 jobs:
   profile-daft:
     runs-on: ubuntu-latest
     timeout-minutes: 20
     strategy:
```

### Comparing `getdaft-0.1.3/.github/workflows/notebook-checker.yml` & `getdaft-0.1.4/.github/workflows/notebook-checker.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/.github/workflows/property-based-tests.yml` & `getdaft-0.1.4/.github/workflows/property-based-tests.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/.github/workflows/python-package.yml` & `getdaft-0.1.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/.github/workflows/python-publish.yml` & `getdaft-0.1.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/.github/workflows/ray-compatibility.yml` & `getdaft-0.1.4/.github/workflows/ray-compatibility.yml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 jobs:
   build:
     runs-on: ubuntu-latest
     timeout-minutes: 15
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.8']
+        python-version: ['3.9']
         ray-version: [2.3.0, 2.2.0, 2.1.0, 2.0.0]
 
     steps:
     - uses: actions/checkout@v3
     - uses: moonrepo/setup-rust@v0
     - uses: actions/cache@v3
       env:
```

### Comparing `getdaft-0.1.3/.pre-commit-config.yaml` & `getdaft-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/CONTRIBUTING.md` & `getdaft-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/LICENSE` & `getdaft-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/Makefile` & `getdaft-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/README.rst` & `getdaft-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/benchmarking/tpch/__main__.py` & `getdaft-0.1.4/benchmarking/tpch/__main__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/benchmarking/tpch/answers.py` & `getdaft-0.1.4/benchmarking/tpch/answers.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/benchmarking/tpch/data_generation.py` & `getdaft-0.1.4/benchmarking/tpch/data_generation.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/benchmarking/tpch/pipelined_data_generation.py` & `getdaft-0.1.4/benchmarking/tpch/pipelined_data_generation.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/ci/upload_wheels.sh` & `getdaft-0.1.4/ci/upload_wheels.sh`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/__init__.py` & `getdaft-0.1.4/daft/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/analytics.py` & `getdaft-0.1.4/daft/analytics.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/api_annotations.py` & `getdaft-0.1.4/daft/api_annotations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/arrow_utils.py` & `getdaft-0.1.4/daft/arrow_utils.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/context.py` & `getdaft-0.1.4/daft/context.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/convert.py` & `getdaft-0.1.4/daft/convert.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/dataframe/dataframe.py` & `getdaft-0.1.4/daft/dataframe/dataframe.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/datasources.py` & `getdaft-0.1.4/daft/datasources.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/execution/execution_step.py` & `getdaft-0.1.4/daft/execution/execution_step.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 import daft
 from daft.expressions import Expression, ExpressionsProjection, col
 from daft.logical import logical_plan
 from daft.logical.map_partition_ops import MapPartitionOp
 from daft.resource_request import ResourceRequest
 from daft.runners.partitioning import PartialPartitionMetadata, PartitionMetadata
-from daft.series import Series
 from daft.table import Table
 
 PartitionT = TypeVar("PartitionT")
 ID_GEN = itertools.count()
 
 
 @dataclass
@@ -689,16 +688,15 @@
         [input] = inputs
         results = []
 
         for start, end in self.slices:
             assert start >= 0, f"start must be positive, but got {start}"
             end = min(end, len(input))
 
-            indices_block = Series.from_pylist(list(range(start, end)))
-            results.append(input.take(indices_block))
+            results.append(input.slice(start, end))
 
         return results
 
     def run_partial_metadata(self, input_metadatas: list[PartialPartitionMetadata]) -> list[PartialPartitionMetadata]:
         [input_meta] = input_metadatas
 
         results = []
```

### Comparing `getdaft-0.1.3/daft/execution/logical_op_runners.py` & `getdaft-0.1.4/daft/execution/logical_op_runners.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/execution/physical_plan.py` & `getdaft-0.1.4/daft/execution/physical_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,16 @@
     """Pairwise join the partitions from `left_child_plan` and `right_child_plan` together."""
 
     # Materialize the steps from the left and right sources to get partitions.
     # As the materializations complete, emit new steps to join each left and right partition.
     left_requests: deque[SingleOutputPartitionTask[PartitionT]] = deque()
     right_requests: deque[SingleOutputPartitionTask[PartitionT]] = deque()
 
+    yield_left = True
+
     while True:
         # Emit new join steps if we have left and right partitions ready.
         while (
             len(left_requests) > 0 and len(right_requests) > 0 and left_requests[0].done() and right_requests[0].done()
         ):
             next_left = left_requests.popleft()
             next_right = right_requests.popleft()
@@ -173,19 +175,23 @@
                 resource_request=ResourceRequest(
                     memory_bytes=next_left.partition_metadata().size_bytes + next_right.partition_metadata().size_bytes
                 ),
             ).add_instruction(instruction=execution_step.Join(join))
             yield join_step
 
         # Exhausted all ready inputs; execute a single child step to get more join inputs.
-        # Choose whether to execute from left child or right child (whichever one is more behind),
-        if len(left_requests) <= len(right_requests):
+        # Choose whether to execute from left child or right child (whichever one is more behind)
+        if len(left_requests) < len(right_requests):
             next_plan, next_requests = left_plan, left_requests
-        else:
+        elif len(left_requests) > len(right_requests):
             next_plan, next_requests = right_plan, right_requests
+        elif len(left_requests) == len(right_requests):
+            # Both plans have progressed equally; alternate between the two plans to avoid starving either one
+            next_plan, next_requests = (left_plan, left_requests) if yield_left else (right_plan, right_requests)
+            yield_left = not yield_left
 
         try:
             step = next(next_plan)
             if isinstance(step, PartitionTaskBuilder):
                 step = step.finalize_partition_task_single_output()
                 next_requests.append(step)
             yield step
```

### Comparing `getdaft-0.1.3/daft/execution/physical_plan_factory.py` & `getdaft-0.1.4/daft/execution/physical_plan_factory.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/expressions/expressions.py` & `getdaft-0.1.4/daft/expressions/expressions.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,19 @@
         return ExpressionFloatNamespace.from_expression(self)
 
     @property
     def url(self) -> ExpressionUrlNamespace:
         """Access methods that work on columns of URLs"""
         return ExpressionUrlNamespace.from_expression(self)
 
+    @property
+    def image(self) -> ExpressionImageNamespace:
+        """Access methods that work on columns of images"""
+        return ExpressionImageNamespace.from_expression(self)
+
     @staticmethod
     def _from_pyexpr(pyexpr: _PyExpr) -> Expression:
         expr = Expression.__new__(Expression)
         expr._expr = pyexpr
         return expr
 
     @staticmethod
@@ -656,7 +661,19 @@
         if name not in self._output_name_to_exprs:
             raise ValueError(f"{name} not found in ExpressionsProjection")
         return self._output_name_to_exprs[name]
 
     def resolve_schema(self, schema: Schema) -> Schema:
         fields = [e._to_field(schema) for e in self]
         return Schema._from_field_name_and_types([(f.name, f.dtype) for f in fields])
+
+
+class ExpressionImageNamespace(ExpressionNamespace):
+    def decode(self) -> Expression:
+        return Expression._from_pyexpr(self._expr.image_decode())
+
+    def resize(self, w: int, h: int) -> Expression:
+        if not isinstance(w, int):
+            raise TypeError(f"expected int for w but got {type(w)}")
+        if not isinstance(h, int):
+            raise TypeError(f"expected int for h but got {type(h)}")
+        return Expression._from_pyexpr(self._expr.image_resize(w, h))
```

### Comparing `getdaft-0.1.3/daft/expressions/testing.py` & `getdaft-0.1.4/daft/expressions/testing.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/filesystem.py` & `getdaft-0.1.4/daft/filesystem.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/internal/rule.py` & `getdaft-0.1.4/daft/internal/rule.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/internal/rule_runner.py` & `getdaft-0.1.4/daft/internal/rule_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 
 
 class RuleRunner(Generic[TreeNodeType]):
     def __init__(self, batches: list[RuleBatch[TreeNodeType]]) -> None:
         self._batches = batches
 
     def optimize(self, root: TreeNodeType) -> TreeNodeType:
+        from copy import deepcopy
+
+        root = deepcopy(root)
         for batch in self._batches:
             root = self._run_single_batch(root, batch)
         return root
 
     def __call__(self, root: TreeNodeType) -> TreeNodeType:
         return self.optimize(root)
```

### Comparing `getdaft-0.1.3/daft/internal/treenode.py` & `getdaft-0.1.4/daft/internal/treenode.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/io/_csv.py` & `getdaft-0.1.4/daft/io/_csv.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/io/_json.py` & `getdaft-0.1.4/daft/io/_json.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/io/common.py` & `getdaft-0.1.4/daft/io/common.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/io/file_path.py` & `getdaft-0.1.4/daft/io/file_path.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/io/parquet.py` & `getdaft-0.1.4/daft/io/parquet.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/logical/aggregation_plan_builder.py` & `getdaft-0.1.4/daft/logical/aggregation_plan_builder.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/logical/logical_plan.py` & `getdaft-0.1.4/daft/logical/logical_plan.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/logical/map_partition_ops.py` & `getdaft-0.1.4/daft/logical/map_partition_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/logical/optimizer.py` & `getdaft-0.1.4/daft/logical/optimizer.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/logical/schema.py` & `getdaft-0.1.4/daft/logical/schema.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/pickle/cloudpickle.py` & `getdaft-0.1.4/daft/pickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/pickle/cloudpickle_fast.py` & `getdaft-0.1.4/daft/pickle/cloudpickle_fast.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/pickle/compat.py` & `getdaft-0.1.4/daft/pickle/compat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/resource_request.py` & `getdaft-0.1.4/daft/resource_request.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/runners/partitioning.py` & `getdaft-0.1.4/daft/runners/partitioning.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/runners/profiler.py` & `getdaft-0.1.4/daft/runners/profiler.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/runners/pyrunner.py` & `getdaft-0.1.4/daft/runners/pyrunner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/runners/ray_runner.py` & `getdaft-0.1.4/daft/runners/ray_runner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/runners/runner.py` & `getdaft-0.1.4/daft/runners/runner.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/runners/runner_io.py` & `getdaft-0.1.4/daft/runners/runner_io.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/series.py` & `getdaft-0.1.4/daft/series.py`

 * *Files 2% similar despite different names*

```diff
@@ -379,14 +379,18 @@
     def dt(self) -> SeriesDateNamespace:
         return SeriesDateNamespace.from_series(self)
 
     @property
     def arr(self) -> SeriesArrayNamespace:
         return SeriesArrayNamespace.from_series(self)
 
+    @property
+    def image(self) -> SeriesImageNamespace:
+        return SeriesImageNamespace.from_series(self)
+
     def __reduce__(self) -> tuple:
         if self.datatype()._is_python_type():
             return (Series.from_pylist, (self.to_pylist(), self.name(), "force"))
         else:
             return (Series.from_arrow, (self.to_arrow(), self.name()))
 
 
@@ -454,7 +458,20 @@
     def day_of_week(self) -> Series:
         return Series._from_pyseries(self._series.dt_day_of_week())
 
 
 class SeriesArrayNamespace(SeriesNamespace):
     def lengths(self) -> Series:
         return Series._from_pyseries(self._series.arr_lengths())
+
+
+class SeriesImageNamespace(SeriesNamespace):
+    def decode(self) -> Series:
+        return Series._from_pyseries(self._series.image_decode())
+
+    def resize(self, w: int, h: int) -> Series:
+        if not isinstance(w, int):
+            raise TypeError(f"expected int for w but got {type(w)}")
+        if not isinstance(h, int):
+            raise TypeError(f"expected int for h but got {type(h)}")
+
+        return Series._from_pyseries(self._series.image_resize(w, h))
```

### Comparing `getdaft-0.1.3/daft/table/table.py` & `getdaft-0.1.4/daft/table/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,21 @@
         tables = []
         for t in to_merge:
             if not isinstance(t, Table):
                 raise TypeError(f"Expected a Table for concat, got {type(t)}")
             tables.append(t._table)
         return Table._from_pytable(_PyTable.concat(tables))
 
+    def slice(self, start: int, end: int) -> Table:
+        if not isinstance(start, int):
+            raise TypeError(f"expected int for start but got {type(start)}")
+        if not isinstance(end, int):
+            raise TypeError(f"expected int for end but got {type(end)}")
+        return Table._from_pytable(self._table.slice(start, end))
+
     ###
     # Exporting methods
     ###
 
     def to_arrow(self) -> pa.Table:
         python_fields = {field.name for field in self.schema() if field.dtype == DataType.python()}
         if python_fields:
```

### Comparing `getdaft-0.1.3/daft/table/table_io.py` & `getdaft-0.1.4/daft/table/table_io.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/udf.py` & `getdaft-0.1.4/daft/udf.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/udf_library/url_udfs.py` & `getdaft-0.1.4/daft/udf_library/url_udfs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/utils.py` & `getdaft-0.1.4/daft/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,16 +60,19 @@
 
     # Sampling complete.
     # If we ended up measuring the entire list, just return the exact value.
     if len(sampled_sizes) == len(pylist):
         return sum(sampled_sizes)
 
     # Otherwise, reduce to a one-item estimate and extrapolate.
-    mean, stdev = statistics.mean(sampled_sizes), statistics.stdev(sampled_sizes)
-    one_item_size_estimate = int(mean + stdev)
+    if len(sampled_sizes) == 1:
+        [one_item_size_estimate] = sampled_sizes
+    else:
+        mean, stdev = statistics.mean(sampled_sizes), statistics.stdev(sampled_sizes)
+        one_item_size_estimate = int(mean + stdev)
 
     return one_item_size_estimate * len(pylist)
 
 
 def map_operator_arrow_semantics_bool(
     operator: Callable[[Any, Any], Any],
     left_pylist: list,
```

### Comparing `getdaft-0.1.3/daft/viz/dataframe_display.py` & `getdaft-0.1.4/daft/viz/dataframe_display.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/viz/html_viz_hooks.py` & `getdaft-0.1.4/daft/viz/html_viz_hooks.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/daft/viz/repr.py` & `getdaft-0.1.4/daft/viz/repr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import html
-from typing import Any, Callable, Iterable
+from typing import Any, Iterable
 
 from tabulate import tabulate
 
 from daft.datatype import DataType
 from daft.logical.schema import Schema
 from daft.table import Table
 from daft.viz.html_viz_hooks import get_viz_hook
@@ -18,55 +18,74 @@
     """Truncates a string and adds an ellipsis if it exceeds (max_col_width * max_lines) number of characters"""
     max_len = max_col_width * max_lines
     if len(s) > max_len:
         s = s[: (max_col_width * max_lines) - 3] + "..."
     return s
 
 
-def _stringify_object_default(val: Any, max_col_width: int, max_lines: int):
-    """Stringifies Python objects for the REPL"""
-    return _truncate(str(val), max_col_width, max_lines)
-
-
 def _stringify_object_html(val: Any, max_col_width: int, max_lines: int):
     """Stringifies Python objects, with custom handling for specific objects that Daft recognizes as media types"""
     viz_hook = get_viz_hook(val)
     if viz_hook is not None:
         return viz_hook(val)
     return html.escape(_truncate(str(val), max_col_width, max_lines))
 
 
 def _stringify_vpartition(
     data: dict[str, list[Any]],
     daft_schema: Schema,
-    custom_stringify_object: Callable = _stringify_object_default,
     max_col_width: int = DEFAULT_MAX_COL_WIDTH,
     max_lines: int = DEFAULT_MAX_LINES,
 ) -> dict[str, Iterable[str]]:
     """Converts a vPartition into a dictionary of display-friendly stringified values"""
     assert all(
         colname in data for colname in daft_schema.column_names()
     ), f"Data does not contain columns: {set(daft_schema.column_names()) - set(data.keys())}"
 
     data_stringified: dict[str, Iterable[str]] = {}
     for colname in daft_schema.column_names():
         field = daft_schema[colname]
         if field.dtype._is_python_type():
-            data_stringified[colname] = [
-                custom_stringify_object(val, max_col_width, max_lines) for val in data[colname]
-            ]
+            data_stringified[colname] = [_truncate(str(val), max_col_width, max_lines) for val in data[colname]]
         elif field.dtype == DataType.bool():
             # BUG: tabulate library does not handle string literal values "True" and "False" correctly, so we lowercase them.
             data_stringified[colname] = [_truncate(str(val).lower(), max_col_width, max_lines) for val in data[colname]]
         else:
             data_stringified[colname] = [_truncate(str(val), max_col_width, max_lines) for val in data[colname]]
 
     return data_stringified
 
 
+def _stringify_vpartition_html(
+    data: dict[str, list[Any]],
+    daft_schema: Schema,
+    max_col_width: int = DEFAULT_MAX_COL_WIDTH,
+    max_lines: int = DEFAULT_MAX_LINES,
+) -> dict[str, Iterable[str]]:
+    """Converts a vPartition into a dictionary of display-friendly stringified values"""
+    assert all(
+        colname in data for colname in daft_schema.column_names()
+    ), f"Data does not contain columns: {set(daft_schema.column_names()) - set(data.keys())}"
+
+    data_stringified: dict[str, Iterable[str]] = {}
+    for colname in daft_schema.column_names():
+        field = daft_schema[colname]
+        if field.dtype._is_python_type():
+            data_stringified[colname] = [_stringify_object_html(val, max_col_width, max_lines) for val in data[colname]]
+        elif field.dtype == DataType.bool():
+            # BUG: tabulate library does not handle string literal values "True" and "False" correctly, so we lowercase them.
+            data_stringified[colname] = [_truncate(str(val).lower(), max_col_width, max_lines) for val in data[colname]]
+        else:
+            data_stringified[colname] = [
+                html.escape(_truncate(str(val), max_col_width, max_lines)) for val in data[colname]
+            ]
+
+    return data_stringified
+
+
 def vpartition_repr_html(
     vpartition: Table | None,
     daft_schema: Schema,
     num_rows: int,
     user_message: str,
     max_col_width: int = DEFAULT_MAX_COL_WIDTH,
     max_lines: int = DEFAULT_MAX_LINES,
@@ -75,18 +94,17 @@
     if len(daft_schema) == 0:
         return "<small>(No data to display: Dataframe has no columns)</small>"
     data = (
         {k: v[:num_rows] for k, v in vpartition.to_pydict().items()}
         if vpartition is not None
         else {colname: [] for colname in daft_schema.column_names()}
     )
-    data_stringified = _stringify_vpartition(
+    data_stringified = _stringify_vpartition_html(
         data,
         daft_schema,
-        custom_stringify_object=_stringify_object_html,
         max_col_width=max_col_width,
         max_lines=max_lines,
     )
 
     headers = [f"{name}<br>{daft_schema[name].dtype}" for name in daft_schema.column_names()]
 
     # Workaround for https://github.com/astanin/python-tabulate/issues/224
@@ -137,15 +155,14 @@
         {k: v[:num_rows] for k, v in vpartition.to_pydict().items()}
         if vpartition is not None
         else {colname: [] for colname in daft_schema.column_names()}
     )
     data_stringified = _stringify_vpartition(
         data,
         daft_schema,
-        custom_stringify_object=_stringify_object_default,
         max_col_width=max_col_width,
         max_lines=max_lines,
     )
 
     return (
         tabulate(
             data_stringified,
```

### Comparing `getdaft-0.1.3/docs/Makefile` & `getdaft-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/10-min.ipynb` & `getdaft-0.1.4/docs/source/10-min.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/_static/daft-favicon.png` & `getdaft-0.1.4/docs/source/_static/daft-favicon.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/_static/daft-logo.png` & `getdaft-0.1.4/docs/source/_static/daft-logo.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/_static/daft_illustration.png` & `getdaft-0.1.4/docs/source/_static/daft_illustration.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/_static/execution_model.png` & `getdaft-0.1.4/docs/source/_static/execution_model.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/_static/header.css` & `getdaft-0.1.4/docs/source/_static/header.css`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/_static/high_level_architecture.png` & `getdaft-0.1.4/docs/source/_static/high_level_architecture.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/_static/in_memory_data_representation.png` & `getdaft-0.1.4/docs/source/_static/in_memory_data_representation.png`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/_static/mobile-menu.js` & `getdaft-0.1.4/docs/source/_static/mobile-menu.js`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/_templates/layout.html` & `getdaft-0.1.4/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/_templates/sections/header.html` & `getdaft-0.1.4/docs/source/_templates/sections/header.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/_templates/sections/mobile-menu.html` & `getdaft-0.1.4/docs/source/_templates/sections/mobile-menu.html`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/api_docs/dataframe.rst` & `getdaft-0.1.4/docs/source/api_docs/dataframe.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/api_docs/expressions.rst` & `getdaft-0.1.4/docs/source/api_docs/expressions.rst`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 
     daft.expressions.expressions.ExpressionStringNamespace.concat
     daft.expressions.expressions.ExpressionStringNamespace.contains
     daft.expressions.expressions.ExpressionStringNamespace.endswith
     daft.expressions.expressions.ExpressionStringNamespace.startswith
     daft.expressions.expressions.ExpressionStringNamespace.length
 
+.. _api-expressions-temporal:
 
 Dates
 *****
 
 Operations on datetimes, accessible through the ``Expression.dt`` method accessor:
 
 Example: ``e.dt.day()``
```

### Comparing `getdaft-0.1.3/docs/source/api_docs/groupby.rst` & `getdaft-0.1.4/docs/source/api_docs/groupby.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/api_docs/input_output.rst` & `getdaft-0.1.4/docs/source/api_docs/input_output.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/conf.py` & `getdaft-0.1.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/dataframe_comparison.rst` & `getdaft-0.1.4/docs/source/dataframe_comparison.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/index.rst` & `getdaft-0.1.4/docs/source/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -50,14 +50,16 @@
    10-min
    learn/index
    api_docs/index
    release_notes/index
    Telemetry <telemetry>
    dataframe_comparison
    technical_architecture
+   benchmarks/index
+
 
 .. Indices and tables
 .. ==================
 
 .. * :ref:`genindex`
 .. * :ref:`modindex`
 .. * :ref:`search`
```

### Comparing `getdaft-0.1.3/docs/source/install.rst` & `getdaft-0.1.4/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/learn/index.rst` & `getdaft-0.1.4/docs/source/learn/index.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/learn/key_concepts.rst` & `getdaft-0.1.4/docs/source/learn/key_concepts.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/learn/tutorials.rst` & `getdaft-0.1.4/docs/source/learn/tutorials.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/learn/user_guides/aggregations.rst` & `getdaft-0.1.4/docs/source/learn/user_guides/aggregations.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/learn/user_guides/dataframe-operations.rst` & `getdaft-0.1.4/docs/source/learn/user_guides/dataframe-operations.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/learn/user_guides/expressions.rst` & `getdaft-0.1.4/docs/source/learn/user_guides/expressions.rst`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     from daft import lit
 
     # Refers to an expression which always evaluates to 42
     lit(42)
 
 This special ``lit`` expression we just created evaluates always to the value ``42``.
 
+.. _userguide-numeric-expressions:
+
 Numeric Expressions
 -------------------
 
 Since column "A" is an integer, we can run numeric computation such as addition, division and checking its value. Here are some examples where we create new columns using the results of such computations:
 
 .. code:: python
 
@@ -88,14 +90,16 @@
     +---------+-------------+----------------+-----------+
     (Showing first 3 of 3 rows)
 
 Notice that the returned types of these operations are also well-typed according to their input types. For example, calling ``df["A"] > 1`` returns a column of type ``Boolean``.
 
 Both The Float and Int types are numeric types, and inherit many of the same arithmetic Expression operations. You may find the full list of numeric operations in the :ref:`Expressions API reference <api-numeric-expression-operations>`.
 
+.. _userguide-string-expressions:
+
 String Expressions
 ------------------
 
 Daft also lets you have columns of strings in a DataFrame. Let's take a look!
 
 .. code:: python
 
@@ -196,15 +200,17 @@
     | images/validation-   | 01\x01\x00H\x00H\... |
     | images/0001e...      |                      |
     +----------------------+----------------------+
     (Showing first 2 of 2 rows)
 
 This works well for URLs which are HTTP paths to non-HTML files (e.g. jpeg), local filepaths or even paths to a file in an object store such as AWS S3 as well!
 
-Boolean Expressions
+.. _userguide-logical-expressions:
+
+Logical Expressions
 -------------------
 
 Logical Expressions are an expression that refers to a column of type ``Boolean``, and can only take on the values True or False.
 
 .. code:: python
 
     df = daft.from_pydict({"C": [True, False, True]})
```

### Comparing `getdaft-0.1.3/docs/source/learn/user_guides/intro-dataframes.rst` & `getdaft-0.1.4/docs/source/learn/user_guides/intro-dataframes.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/learn/user_guides/read-write.rst` & `getdaft-0.1.4/docs/source/learn/user_guides/read-write.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/learn/user_guides/scaling-up.rst` & `getdaft-0.1.4/docs/source/learn/user_guides/scaling-up.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/learn/user_guides/udf.rst` & `getdaft-0.1.4/docs/source/learn/user_guides/udf.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/learn/user_guides.rst` & `getdaft-0.1.4/docs/source/learn/user_guides.rst`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 * **It is intelligent** - Daft performs query optimizations to speed up your work.
 
 .. toctree::
     :maxdepth: 1
 
     user_guides/intro-dataframes
+    user_guides/datatypes
     user_guides/expressions
     user_guides/read-write
     user_guides/dataframe-operations
     user_guides/aggregations
     user_guides/udf
     user_guides/scaling-up
     user_guides/partitioning
```

### Comparing `getdaft-0.1.3/docs/source/release_notes/0.0.13.rst` & `getdaft-0.1.4/docs/source/release_notes/0.0.13.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/release_notes/0.0.14.rst` & `getdaft-0.1.4/docs/source/release_notes/0.0.14.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/release_notes/0.0.16.rst` & `getdaft-0.1.4/docs/source/release_notes/0.0.16.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/release_notes/0.0.17.rst` & `getdaft-0.1.4/docs/source/release_notes/0.0.17.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/release_notes/0.0.18.rst` & `getdaft-0.1.4/docs/source/release_notes/0.0.18.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/release_notes/0.0.19.rst` & `getdaft-0.1.4/docs/source/release_notes/0.0.19.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/release_notes/0.0.20.rst` & `getdaft-0.1.4/docs/source/release_notes/0.0.20.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/release_notes/0.0.21.rst` & `getdaft-0.1.4/docs/source/release_notes/0.0.21.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/release_notes/0.0.22.rst` & `getdaft-0.1.4/docs/source/release_notes/0.0.22.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/release_notes/0.0.23.rst` & `getdaft-0.1.4/docs/source/release_notes/0.0.23.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/release_notes/0.0.24.rst` & `getdaft-0.1.4/docs/source/release_notes/0.0.24.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/release_notes/0.1.0.rst` & `getdaft-0.1.4/docs/source/release_notes/0.1.0.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/release_notes/0.1.1.rst` & `getdaft-0.1.4/docs/source/release_notes/0.1.1.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/release_notes/0.1.2.rst` & `getdaft-0.1.4/docs/source/release_notes/0.1.2.rst`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 Build Changes
 -------------
 
 * \[ci\] enable pyrunner for 310 `#946 <https://github.com/Eventual-Inc/Daft/pull/946>`_
 * Add Pyarrow 6.0 in matrix for CI testing `#945 <https://github.com/Eventual-Inc/Daft/pull/945>`_
 * Update requirement of tabulate to \>=0.9.0 `#940 <https://github.com/Eventual-Inc/Daft/pull/940>`_
 * unpin numpy for 3.7 to get dependabot to stop complaining `#938 <https://github.com/Eventual-Inc/Daft/pull/938>`_
-* Bump slackapi/slack-github-action from 1.23.0 to 1.24.0 `#936 <https:github.com/Eventual-Inc/Daft/pull/936>`_
+* Bump slackapi/slack-github-action from 1.23.0 to 1.24.0 `#936 <https://github.com/Eventual-Inc/Daft/pull/936>`_
 * Bump hypothesis from 6.75.2 to 6.75.3 `#928 <https://github.com/Eventual-Inc/Daft/pull/928>`_
 * Bump dask from 2023.4.1 to 2023.5.0 `#927 <https://github.com/Eventual-Inc/Daft/pull/927>`_
 * Bump serde from 1.0.162 to 1.0.163 `#921 <https://github.com/Eventual-Inc/Daft/pull/921>`_
 
 
 Documentation
 -------------
```

### Comparing `getdaft-0.1.3/docs/source/release_notes/0.1.3.rst` & `getdaft-0.1.4/docs/source/release_notes/0.1.3.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/release_notes/_template.rst` & `getdaft-0.1.4/docs/source/release_notes/_template.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/technical_architecture.rst` & `getdaft-0.1.4/docs/source/technical_architecture.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/docs/source/telemetry.rst` & `getdaft-0.1.4/docs/source/telemetry.rst`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/pyproject.toml` & `getdaft-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/requirements-dev.txt` & `getdaft-0.1.4/requirements-dev.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 # Development/Build utilities (allow to be unpinned)
 ipdb
 maturin
 pre-commit
 
 # Tracing
-orjson==3.8.12  # orjson recommended for viztracer
+orjson==3.9.0  # orjson recommended for viztracer
 py-spy==0.3.14
 viztracer==0.15.6
 
 # Testing frameworks
-hypothesis==6.75.3
+hypothesis==6.75.9
 pytest==7.3.1
 pytest-benchmark==4.0.0
-pytest-cov==4.0.0
+pytest-cov==4.1.0
 
 # Testing dependencies
 lxml==4.9.2
 dask==2022.2.0; python_version < '3.8'
-dask==2023.5.0; python_version >= '3.8'
+dask==2023.5.0; python_version == '3.8'
+dask==2023.5.1; python_version >= '3.9'
 numpy; python_version < '3.8'
 numpy==1.24.3; python_version >= '3.8'
 pandas==1.3.5; python_version < '3.8'
-pandas==2.0.1; python_version >= '3.8'
+pandas==2.0.2; python_version >= '3.8'
 xxhash>=3.0.0
+Pillow==9.5.0
+opencv-python==4.7.0.72
 
 # Ray
 ray[data, default]==2.4.0
 
+# AWS
+s3fs==2023.1.0; python_version < '3.8'
+s3fs==2023.5.0; python_version >= '3.8'
+
 # Documentation
 myst-nb>=0.16.0
 Sphinx <= 5
 sphinx-book-theme>=0.3.3,<1.0.0
 sphinx-reredirects>=0.1.1
```

### Comparing `getdaft-0.1.3/src/array/from.rs` & `getdaft-0.1.4/src/array/from.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 use std::sync::Arc;
 
 use crate::datatypes::{
-    BinaryArray, BooleanArray, DaftNumericType, DaftPhysicalType, DataType, Field, Utf8Array,
-    Utf8Type,
+    BinaryArray, BooleanArray, DaftNumericType, DaftPhysicalType, DataType, Field, NullArray,
+    Utf8Array, Utf8Type,
 };
 
 use crate::array::DataArray;
 use crate::error::{DaftError, DaftResult};
 
 impl<T: DaftNumericType> From<(&str, Box<arrow2::array::PrimitiveArray<T::Native>>)>
     for DataArray<T>
 {
     fn from(item: (&str, Box<arrow2::array::PrimitiveArray<T::Native>>)) -> Self {
         let (name, array) = item;
         DataArray::new(Field::new(name, T::get_dtype()).into(), array).unwrap()
     }
 }
 
+impl From<(&str, Box<arrow2::array::NullArray>)> for NullArray {
+    fn from(item: (&str, Box<arrow2::array::NullArray>)) -> Self {
+        let (name, array) = item;
+        DataArray::new(Field::new(name, DataType::Null).into(), array).unwrap()
+    }
+}
+
 impl From<(&str, Box<arrow2::array::Utf8Array<i64>>)> for Utf8Array {
     fn from(item: (&str, Box<arrow2::array::Utf8Array<i64>>)) -> Self {
         let (name, array) = item;
         DataArray::new(Field::new(name, DataType::Utf8).into(), array).unwrap()
     }
 }
```

### Comparing `getdaft-0.1.3/src/array/iterator.rs` & `getdaft-0.1.4/src/array/iterator.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/mod.rs` & `getdaft-0.1.4/src/array/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/apply.rs` & `getdaft-0.1.4/src/array/ops/apply.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/arange.rs` & `getdaft-0.1.4/src/array/ops/arange.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/arithmetic.rs` & `getdaft-0.1.4/src/array/ops/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/arrow2/comparison.rs` & `getdaft-0.1.4/src/array/ops/arrow2/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/arrow2/sort/primitive/common.rs` & `getdaft-0.1.4/src/array/ops/arrow2/sort/primitive/common.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/arrow2/sort/primitive/indices.rs` & `getdaft-0.1.4/src/array/ops/arrow2/sort/primitive/indices.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/arrow2/sort/primitive/sort.rs` & `getdaft-0.1.4/src/array/ops/arrow2/sort/primitive/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/as_arrow.rs` & `getdaft-0.1.4/src/array/ops/as_arrow.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use arrow2;
 use arrow2::array;
 
 use crate::{
     array::DataArray,
     datatypes::{
-        logical::{DateArray, EmbeddingArray},
+        logical::{DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray},
         BinaryArray, BooleanArray, DaftNumericType, FixedSizeListArray, ListArray, StructArray,
         Utf8Array,
     },
 };
 
 pub trait AsArrow {
     type Output;
@@ -100,12 +100,30 @@
         self.data().as_any().downcast_ref().unwrap()
     }
 }
 
 impl AsArrow for EmbeddingArray {
     type Output = array::FixedSizeListArray;
 
-    // downcasts a DataArray<T> to an Arrow FixedSizeListArray.
+    // downcasts an EmbeddingArray to an Arrow FixedSizeListArray.
+    fn as_arrow(&self) -> &Self::Output {
+        self.physical.data().as_any().downcast_ref().unwrap()
+    }
+}
+
+impl AsArrow for ImageArray {
+    type Output = array::StructArray;
+
+    // downcasts an ImageArray to an Arrow StructArray.
+    fn as_arrow(&self) -> &Self::Output {
+        self.physical.data().as_any().downcast_ref().unwrap()
+    }
+}
+
+impl AsArrow for FixedShapeImageArray {
+    type Output = array::FixedSizeListArray;
+
+    // downcasts a FixedShapeImageArray to an Arrow FixedSizeListArray.
     fn as_arrow(&self) -> &Self::Output {
         self.physical.data().as_any().downcast_ref().unwrap()
     }
 }
```

### Comparing `getdaft-0.1.3/src/array/ops/broadcast.rs` & `getdaft-0.1.4/src/array/ops/broadcast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/cast.rs` & `getdaft-0.1.4/src/array/ops/cast.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 use arrow2::compute::{
     self,
     cast::{can_cast_types, cast, CastOptions},
 };
 
-use crate::datatypes::FixedSizeListArray;
-use crate::datatypes::ListArray;
 use crate::series::IntoSeries;
 use crate::{
-    array::DataArray,
-    datatypes::{logical::DateArray, Field},
-    datatypes::{DaftArrowBackedType, DataType, Utf8Array},
+    array::{ops::image::ImageArrayVecs, DataArray},
+    datatypes::logical::{
+        DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray, LogicalArray,
+    },
+    datatypes::{DaftArrowBackedType, DataType, Field, Utf8Array},
     error::{DaftError, DaftResult},
     series::Series,
-    with_match_arrow_daft_types, with_match_daft_logical_types,
-};
-use crate::{
-    datatypes::logical::{EmbeddingArray, LogicalArray},
-    with_match_numeric_daft_types,
+    with_match_arrow_daft_types, with_match_daft_logical_types, with_match_numeric_daft_types,
 };
 use arrow2::array::Array;
-use num_traits::{NumCast, ToPrimitive};
-use std::iter;
+use num_traits::NumCast;
 
+#[cfg(feature = "python")]
+use crate::datatypes::{FixedSizeListArray, ListArray};
+#[cfg(feature = "python")]
+use crate::datatypes::{ImageMode, PythonArray};
+#[cfg(feature = "python")]
 use log;
-
 #[cfg(feature = "python")]
-use crate::datatypes::PythonArray;
+use num_traits::ToPrimitive;
 #[cfg(feature = "python")]
 use numpy::PyReadonlyArrayDyn;
 #[cfg(feature = "python")]
 use pyo3::prelude::*;
+#[cfg(feature = "python")]
+use std::iter;
 
 use super::as_arrow::AsArrow;
 use std::sync::Arc;
 fn arrow_cast<T>(to_cast: &DataArray<T>, dtype: &DataType) -> DaftResult<Series>
 where
     T: DaftArrowBackedType,
 {
-    let _arrow_type = dtype.to_arrow();
-
     if !dtype.is_arrow() || !to_cast.data_type().is_arrow() {
         return Err(DaftError::TypeError(format!(
             "Can not cast {:?} to type: {:?}: not convertible to Arrow",
             to_cast.data_type(),
             dtype
         )));
     }
@@ -188,112 +187,163 @@
 #[cfg(feature = "python")]
 fn append_values_from_numpy<
     Tgt: numpy::Element + NumCast + ToPrimitive + arrow2::types::NativeType,
 >(
     pyarray: &PyAny,
     index: usize,
     from_numpy_dtype_fn: &PyAny,
+    enforce_dtype: Option<&DataType>,
     values_vec: &mut Vec<Tgt>,
+    shapes_vec: &mut Vec<Vec<u64>>,
 ) -> DaftResult<usize> {
     use crate::python::PyDataType;
-    use numpy::PyArray1;
     use std::num::Wrapping;
 
     let np_dtype = pyarray.getattr(pyo3::intern!(pyarray.py(), "dtype"))?;
 
     let datatype = from_numpy_dtype_fn
         .call1((np_dtype,))?
         .getattr(pyo3::intern!(pyarray.py(), "_dtype"))?
         .extract::<PyDataType>()?;
     let datatype = datatype.dtype;
-
+    if let Some(enforce_dtype) = enforce_dtype {
+        if enforce_dtype != &datatype {
+            return Err(DaftError::ValueError(format!(
+                "Expected Numpy array to be of type: {enforce_dtype} but is {datatype} at index: {index}",
+            )));
+        }
+    }
     if !datatype.is_numeric() {
         return Err(DaftError::ValueError(format!(
             "Numpy array has unsupported type {} at index: {index}",
             datatype
         )));
     }
     with_match_numeric_daft_types!(datatype, |$N| {
         type Src = <$N as DaftNumericType>::Native;
         let pyarray: PyReadonlyArrayDyn<'_, Src> = pyarray.extract()?;
-        if pyarray.ndim() != 1 {
+        // All of the conditions given in the ndarray::ArrayView::from_shape_ptr() docstring must be met in order to do
+        // the pyarray.as_array conversion: https://docs.rs/ndarray/0.15.6/ndarray/type.ArrayView.html#method.from_shape_ptr
+        // Relevant:
+        //  1. Must have non-negative strides.
+
+        // TODO(Clark): Double-check that we're covering all bases here for this unsafe handoff.
+        if pyarray.strides().iter().any(|s| *s < 0) {
             return Err(DaftError::ValueError(format!(
-                "we only support 1 dim numpy arrays, got {} at index: {}",
-                pyarray.ndim(), index
+                "we only support numpy arrays with non-negative strides, but got {:?} at index: {}",
+                pyarray.strides(), index
             )));
         }
 
-        let pyarray = pyarray.downcast::<PyArray1<Src>>().expect("downcasted to numpy array");
-        let sl: &[Src] = unsafe { pyarray.as_slice()}.expect("convert numpy array to slice");
+        let pyarray = pyarray.as_array();
+        let owned_arr;
+        // Create 1D slice from potentially non-contiguous and non-C-order arrays.
+        // This will only create a copy if the ndarray is non-contiguous.
+        let sl: &[Src] = match pyarray.as_slice_memory_order() {
+            Some(sl) => sl,
+            None => {
+                owned_arr = pyarray.to_owned();
+                owned_arr.as_slice_memory_order().unwrap()
+            }
+        };
         values_vec.extend(sl.iter().map(|v| <Wrapping<Tgt> as NumCast>::from(*v).unwrap().0));
-        Ok(sl.len())
+        shapes_vec.push(pyarray.shape().iter().map(|v| *v as u64).collect::<Vec<u64>>());
+        Ok((sl.len()))
     })
 }
 
+type ArrayPayload<Tgt> = (Vec<Tgt>, Option<Vec<i64>>, Option<Vec<Vec<u64>>>);
+
 #[cfg(feature = "python")]
 fn extract_python_to_vec<
     Tgt: numpy::Element + NumCast + ToPrimitive + arrow2::types::NativeType,
 >(
     py: Python<'_>,
     python_objects: &PythonArray,
     child_dtype: &DataType,
+    enforce_dtype: Option<&DataType>,
     list_size: Option<usize>,
-) -> DaftResult<(Vec<Tgt>, Option<Vec<i64>>)> {
+    shape_size: Option<usize>,
+) -> DaftResult<ArrayPayload<Tgt>> {
     use std::num::Wrapping;
 
     let mut values_vec: Vec<Tgt> =
         Vec::with_capacity(list_size.unwrap_or(0) * python_objects.len());
 
     let mut offsets_vec: Vec<i64> = vec![];
+    let mut shapes_vec: Vec<Vec<u64>> = vec![];
 
     if list_size.is_none() {
         offsets_vec.reserve(python_objects.len() + 1);
         offsets_vec.push(0);
+        shapes_vec.reserve(python_objects.len() + 1);
     }
 
     let from_numpy_dtype = {
         PyModule::import(py, pyo3::intern!(py, "daft.datatype"))?
             .getattr(pyo3::intern!(py, "DataType"))?
             .getattr(pyo3::intern!(py, "from_numpy_dtype"))?
     };
 
     let pytype = match child_dtype {
         dtype if dtype.is_integer() => Ok("int"),
         dtype if dtype.is_floating() => Ok("float"),
         dtype => Err(DaftError::ValueError(format!(
-            "We only support numeric types when converting to FixedSizeList, got {dtype}"
+            "We only support numeric types when converting to List or FixedSizeList, got {dtype}"
         ))),
     }?;
 
     let py_type_fn = { PyModule::import(py, pyo3::intern!(py, "builtins"))?.getattr(pytype)? };
+    let py_memory_view = py
+        .import("builtins")?
+        .getattr(pyo3::intern!(py, "memoryview"))?;
+
+    // TODO: use this to extract our the image mode
+    // let py_pil_image_type = py
+    //     .import("PIL.Image")
+    //     .and_then(|m| m.getattr(pyo3::intern!(py, "Image")));
 
     for (i, object) in python_objects.as_arrow().iter().enumerate() {
         if let Some(object) = object {
             let object = object.into_py(py);
             let object = object.as_ref(py);
 
-            let pyarray = object.call_method0(pyo3::intern!(py, "__array__"));
-
-            if let Ok(pyarray) = pyarray {
-                // Path if object is array-like
-                let num_values =
-                    append_values_from_numpy(pyarray, i, from_numpy_dtype, &mut values_vec)?;
+            let supports_buffer_protocol = py_memory_view.call1((object,)).is_ok();
+            let supports_array_interface_protocol =
+                object.hasattr(pyo3::intern!(py, "__array_interface__"))?;
+            let supports_array_protocol = object.hasattr(pyo3::intern!(py, "__array__"))?;
+
+            if supports_buffer_protocol
+                || supports_array_interface_protocol
+                || supports_array_protocol
+            {
+                // Path if object is supports buffer/array protocols.
+                let np_as_array_fn = py.import("numpy")?.getattr(pyo3::intern!(py, "asarray"))?;
+                let pyarray = np_as_array_fn.call1((object,))?;
+                let num_values = append_values_from_numpy(
+                    pyarray,
+                    i,
+                    from_numpy_dtype,
+                    enforce_dtype,
+                    &mut values_vec,
+                    &mut shapes_vec,
+                )?;
                 if let Some(list_size) = list_size {
                     if num_values != list_size {
                         return Err(DaftError::ValueError(format!(
                                 "Expected Array-like Object to have {list_size} elements but got {} at index {}",
                                 num_values, i
                             )));
                     }
                 } else {
                     offsets_vec.push(offsets_vec.last().unwrap() + num_values as i64);
                 }
             } else {
-                // Path if object is not array-like
-                // try to see if we can iterate over the object
+                // Path if object does not support buffer/array protocols.
+                // Try a best-effort conversion of the elements.
                 let pyiter = object.iter();
                 if let Ok(pyiter) = pyiter {
                     // has an iter
                     let casted_iter = pyiter.map(|v| v.and_then(|f| py_type_fn.call1((f,))));
                     let collected = if child_dtype.is_integer() {
                         let int_iter = casted_iter
                             .map(|v| v.and_then(|v| v.extract::<i64>()))
@@ -322,62 +372,76 @@
                                         .into(),
                                     )
                                 })
                             })
                             .map(|v| v.map(|v| v.0));
                         float_iter.collect::<PyResult<Vec<_>>>()
                     } else {
-                        return Err(DaftError::ValueError(format!(
-                            "Python Object is neither array-like or an iterable at index {}. Can not convert to a list. object type: {}",
-                            i, object.getattr(pyo3::intern!(py, "__class__"))?)));
+                        unreachable!(
+                            "dtype should either be int or float at this point; this is a bug"
+                        );
                     };
 
                     if collected.is_err() {
-                        log::warn!("Could not convert python object to fixed size list at index: {i} for input series: {}", python_objects.name())
+                        log::warn!("Could not convert python object to list at index: {i} for input series: {}", python_objects.name())
                     }
                     let collected: Vec<Tgt> = collected?;
                     if let Some(list_size) = list_size {
                         if collected.len() != list_size {
                             return Err(DaftError::ValueError(format!(
-                            "Expected Array-like Object to have {list_size} elements but got {} at index {}",
-                            collected.len(), i
-                        )));
+                                "Expected Array-like Object to have {list_size} elements but got {} at index {}",
+                                collected.len(), i
+                            )));
                         }
                     } else {
                         let offset = offsets_vec.last().unwrap() + collected.len() as i64;
                         offsets_vec.push(offset);
+                        shapes_vec.push(vec![1]);
                     }
                     values_vec.extend_from_slice(collected.as_slice());
+                } else {
+                    return Err(DaftError::ValueError(format!(
+                        "Python Object is neither array-like or an iterable at index {}. Can not convert to a list. object type: {}",
+                        i, object.getattr(pyo3::intern!(py, "__class__"))?)));
                 }
             }
         } else if let Some(list_size) = list_size {
             values_vec.extend(iter::repeat(Tgt::default()).take(list_size));
         } else {
             let offset = offsets_vec.last().unwrap();
             offsets_vec.push(*offset);
+            if let Some(shape_size) = shape_size {
+                shapes_vec.push(iter::repeat(1).take(shape_size).collect());
+            }
         }
     }
     if list_size.is_some() {
-        Ok((values_vec, None))
+        Ok((values_vec, None, None))
     } else {
-        Ok((values_vec, Some(offsets_vec)))
+        Ok((values_vec, Some(offsets_vec), Some(shapes_vec)))
     }
 }
 
 #[cfg(feature = "python")]
 fn extract_python_like_to_fixed_size_list<
     Tgt: numpy::Element + NumCast + ToPrimitive + arrow2::types::NativeType,
 >(
     py: Python<'_>,
     python_objects: &PythonArray,
     child_field: &Field,
     list_size: usize,
 ) -> DaftResult<FixedSizeListArray> {
-    let (values_vec, _) =
-        extract_python_to_vec::<Tgt>(py, python_objects, &child_field.dtype, Some(list_size))?;
+    let (values_vec, _, _) = extract_python_to_vec::<Tgt>(
+        py,
+        python_objects,
+        &child_field.dtype,
+        None,
+        Some(list_size),
+        None,
+    )?;
 
     let values_array: Box<dyn arrow2::array::Array> =
         Box::new(arrow2::array::PrimitiveArray::from_vec(values_vec));
 
     let inner_field = child_field.to_arrow()?;
 
     let list_dtype = arrow2::datatypes::DataType::FixedSizeList(Box::new(inner_field), list_size);
@@ -400,16 +464,16 @@
 fn extract_python_like_to_list<
     Tgt: numpy::Element + NumCast + ToPrimitive + arrow2::types::NativeType,
 >(
     py: Python<'_>,
     python_objects: &PythonArray,
     child_field: &Field,
 ) -> DaftResult<ListArray> {
-    let (values_vec, offsets) =
-        extract_python_to_vec::<Tgt>(py, python_objects, &child_field.dtype, None)?;
+    let (values_vec, offsets, _) =
+        extract_python_to_vec::<Tgt>(py, python_objects, &child_field.dtype, None, None, None)?;
 
     let offsets = offsets.expect("Offsets should but non-None for dynamic list");
 
     let values_array: Box<dyn arrow2::array::Array> =
         Box::new(arrow2::array::PrimitiveArray::from_vec(values_vec));
 
     let inner_field = child_field.to_arrow()?;
@@ -428,14 +492,110 @@
     ListArray::new(
         Field::new(python_objects.name(), daft_type).into(),
         Box::new(list_array),
     )
 }
 
 #[cfg(feature = "python")]
+fn extract_python_like_to_image_array<
+    Tgt: numpy::Element + NumCast + ToPrimitive + arrow2::types::NativeType,
+>(
+    py: Python<'_>,
+    python_objects: &PythonArray,
+    dtype: &DataType,
+    child_dtype: &DataType,
+    mode_from_dtype: Option<ImageMode>,
+) -> DaftResult<ImageArray> {
+    // 3 dimensions - height x width x channel.
+
+    let shape_size = 3;
+    let (values_vec, offsets, shapes) = extract_python_to_vec::<Tgt>(
+        py,
+        python_objects,
+        child_dtype,
+        Some(child_dtype),
+        None,
+        Some(shape_size),
+    )?;
+
+    let offsets = offsets.expect("Offsets should but non-None for image struct array");
+    let shapes = shapes.expect("Shapes should be non-None for image struct array");
+
+    let validity = python_objects.as_arrow().validity();
+
+    let num_rows = shapes.len();
+
+    let mut channels = Vec::<u16>::with_capacity(num_rows);
+    let mut heights = Vec::<u32>::with_capacity(num_rows);
+    let mut widths = Vec::<u32>::with_capacity(num_rows);
+    let mut modes = Vec::<u8>::with_capacity(num_rows);
+    for (mut shape, is_valid) in iter::zip(
+        shapes.into_iter(),
+        validity
+            .unwrap_or(&arrow2::bitmap::Bitmap::from_iter(
+                iter::repeat(true).take(num_rows),
+            ))
+            .iter(),
+    ) {
+        if !is_valid {
+            // Handle invalid row by populating dummy data.
+            channels.push(1);
+            heights.push(1);
+            widths.push(1);
+            modes.push(mode_from_dtype.unwrap_or(ImageMode::L) as u8);
+            continue;
+        }
+        if shape.len() == shape_size - 1 {
+            shape.push(1);
+        } else if shape.len() != shape_size {
+            return Err(DaftError::ValueError(format!(
+                "Image expected to have {} dimensions, but has {}. Image shape = {:?}",
+                shape_size,
+                shape.len(),
+                shape,
+            )));
+        }
+        assert!(shape.len() == shape_size);
+        heights.push(
+            shape[0]
+                .try_into()
+                .expect("Image height should fit into a uint16"),
+        );
+        widths.push(
+            shape[1]
+                .try_into()
+                .expect("Image width should fit into a uint16"),
+        );
+        channels.push(
+            shape[2]
+                .try_into()
+                .expect("Number of channels should fit into a uint8"),
+        );
+
+        modes.push(mode_from_dtype.unwrap_or(ImageMode::try_from_num_channels(
+            shape[2].try_into().unwrap(),
+            child_dtype,
+        )?) as u8);
+    }
+    ImageArray::from_vecs(
+        python_objects.name(),
+        dtype.clone(),
+        ImageArrayVecs {
+            data: values_vec,
+            channels,
+            heights,
+            widths,
+            modes,
+            offsets,
+            validity: validity.cloned(),
+        },
+    )
+}
+
+#[cfg(feature = "python")]
 impl PythonArray {
     pub fn cast(&self, dtype: &DataType) -> DaftResult<Series> {
         use crate::python::PySeries;
         use pyo3::prelude::*;
         match dtype {
             DataType::Python => Ok(self.clone().into_series()),
 
@@ -490,28 +650,63 @@
                     type Tgt = <$T as DaftNumericType>::Native;
                     pyo3::Python::with_gil(|py| {
                         let result = extract_python_like_to_fixed_size_list::<Tgt>(py, self, field, *size)?;
                         Ok(result.into_series())
                     })
                 })
             }
+            DataType::Struct(_) => unimplemented!(),
             DataType::Embedding(..) => {
                 let result = self.cast(&dtype.to_physical())?;
                 let embedding_array = EmbeddingArray::new(
                     Field::new(self.name(), dtype.clone()),
                     result.fixed_size_list()?.clone(),
                 );
                 Ok(embedding_array.into_series())
             }
-            DataType::Struct(_) => unimplemented!(),
+            DataType::Image(inner_dtype, mode) => {
+                if !inner_dtype.is_numeric() {
+                    panic!(
+                        "Image logical type should only have numeric physical dtype, but got {}",
+                        inner_dtype
+                    );
+                }
+                with_match_numeric_daft_types!(**inner_dtype, |$T| {
+                    type Tgt = <$T as DaftNumericType>::Native;
+                    pyo3::Python::with_gil(|py| {
+                        let result = extract_python_like_to_image_array::<Tgt>(py, self, dtype, inner_dtype, *mode)?;
+                        Ok(result.into_series())
+                    })
+                })
+            }
+            DataType::FixedShapeImage(..) => {
+                let result = self.cast(&dtype.to_physical())?;
+                let image_array = FixedShapeImageArray::new(
+                    Field::new(self.name(), dtype.clone()),
+                    result.fixed_size_list()?.clone(),
+                );
+                Ok(image_array.into_series())
+            }
             // TODO: Add implementations for these types
             // DataType::Timestamp(_, _) => $self.timestamp().unwrap().$method($($args),*),
             dt => unimplemented!("dtype {:?} not supported", dt),
         }
     }
 }
 
 impl EmbeddingArray {
     pub fn cast(&self, dtype: &DataType) -> DaftResult<Series> {
         self.physical.cast(dtype)
     }
 }
+
+impl ImageArray {
+    pub fn cast(&self, dtype: &DataType) -> DaftResult<Series> {
+        self.physical.cast(dtype)
+    }
+}
+
+impl FixedShapeImageArray {
+    pub fn cast(&self, dtype: &DataType) -> DaftResult<Series> {
+        self.physical.cast(dtype)
+    }
+}
```

### Comparing `getdaft-0.1.3/src/array/ops/compare_agg.rs` & `getdaft-0.1.4/src/array/ops/compare_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/comparison.rs` & `getdaft-0.1.4/src/array/ops/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/concat.rs` & `getdaft-0.1.4/src/array/ops/concat.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/concat_agg.rs` & `getdaft-0.1.4/src/array/ops/concat_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/count.rs` & `getdaft-0.1.4/src/array/ops/count.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/date.rs` & `getdaft-0.1.4/src/array/ops/date.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/filter.rs` & `getdaft-0.1.4/src/array/ops/filter.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use crate::{
     array::DataArray,
     datatypes::{
-        logical::{DateArray, EmbeddingArray},
+        logical::{DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray},
         BooleanArray, DaftArrowBackedType,
     },
     error::DaftResult,
 };
 
 use super::as_arrow::AsArrow;
 
@@ -82,7 +82,21 @@
 
 impl EmbeddingArray {
     pub fn filter(&self, mask: &BooleanArray) -> DaftResult<Self> {
         let new_array = self.physical.filter(mask)?;
         Ok(Self::new(self.field.clone(), new_array))
     }
 }
+
+impl ImageArray {
+    pub fn filter(&self, mask: &BooleanArray) -> DaftResult<Self> {
+        let new_array = self.physical.filter(mask)?;
+        Ok(Self::new(self.field.clone(), new_array))
+    }
+}
+
+impl FixedShapeImageArray {
+    pub fn filter(&self, mask: &BooleanArray) -> DaftResult<Self> {
+        let new_array = self.physical.filter(mask)?;
+        Ok(Self::new(self.field.clone(), new_array))
+    }
+}
```

### Comparing `getdaft-0.1.3/src/array/ops/float.rs` & `getdaft-0.1.4/src/array/ops/float.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/full.rs` & `getdaft-0.1.4/src/array/ops/full.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/groups.rs` & `getdaft-0.1.4/src/array/ops/groups.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/hash.rs` & `getdaft-0.1.4/src/array/ops/hash.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/if_else.rs` & `getdaft-0.1.4/src/array/ops/if_else.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use crate::array::DataArray;
-use crate::datatypes::logical::{DateArray, EmbeddingArray};
+use crate::datatypes::logical::{DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray};
 use crate::datatypes::{
     BinaryArray, BooleanArray, DaftArrowBackedType, DaftNumericType, ExtensionArray, Field,
     FixedSizeListArray, ListArray, NullArray, StructArray, Utf8Array,
 };
 use crate::error::{DaftError, DaftResult};
 use crate::utils::arrow::arrow_bitmap_and_helper;
 use std::convert::identity;
@@ -330,7 +330,21 @@
 
 impl EmbeddingArray {
     pub fn if_else(&self, other: &Self, predicate: &BooleanArray) -> DaftResult<Self> {
         let new_array = self.physical.if_else(&other.physical, predicate)?;
         Ok(Self::new(self.field.clone(), new_array))
     }
 }
+
+impl ImageArray {
+    pub fn if_else(&self, other: &Self, predicate: &BooleanArray) -> DaftResult<Self> {
+        let new_array = self.physical.if_else(&other.physical, predicate)?;
+        Ok(Self::new(self.field.clone(), new_array))
+    }
+}
+
+impl FixedShapeImageArray {
+    pub fn if_else(&self, other: &Self, predicate: &BooleanArray) -> DaftResult<Self> {
+        let new_array = self.physical.if_else(&other.physical, predicate)?;
+        Ok(Self::new(self.field.clone(), new_array))
+    }
+}
```

### Comparing `getdaft-0.1.3/src/array/ops/len.rs` & `getdaft-0.1.4/src/array/ops/len.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/list.rs` & `getdaft-0.1.4/src/array/ops/list.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/list_agg.rs` & `getdaft-0.1.4/src/array/ops/list_agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/mean.rs` & `getdaft-0.1.4/src/array/ops/mean.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/mod.rs` & `getdaft-0.1.4/src/array/ops/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 mod date;
 mod filter;
 mod float;
 mod full;
 pub(crate) mod groups;
 mod hash;
 mod if_else;
+pub(crate) mod image;
 mod len;
 mod list;
 mod list_agg;
 mod mean;
 mod null;
 mod pairwise;
 mod search_sorted;
```

### Comparing `getdaft-0.1.3/src/array/ops/null.rs` & `getdaft-0.1.4/src/array/ops/null.rs`

 * *Files 8% similar despite different names*

```diff
@@ -29,7 +29,17 @@
         });
         DataArray::<BooleanType>::new(
             Arc::new(Field::new(self.field.name.clone(), DataType::Boolean)),
             result_arrow_array,
         )
     }
 }
+
+impl<T> DataArray<T>
+where
+    T: DaftPhysicalType,
+{
+    #[inline]
+    pub fn is_valid(&self, idx: usize) -> bool {
+        self.data.is_valid(idx)
+    }
+}
```

### Comparing `getdaft-0.1.3/src/array/ops/pairwise.rs` & `getdaft-0.1.4/src/array/ops/pairwise.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/sort.rs` & `getdaft-0.1.4/src/array/ops/sort.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use crate::{
     array::DataArray,
     datatypes::{
-        logical::{DateArray, EmbeddingArray},
+        logical::{DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray},
         BinaryArray, BooleanArray, DaftIntegerType, DaftNumericType, ExtensionArray,
         FixedSizeListArray, Float32Array, Float64Array, ListArray, NullArray, StructArray,
         Utf8Array,
     },
     error::DaftResult,
     kernels::search_sorted::{build_compare_with_nulls, cmp_float},
     series::Series,
@@ -587,19 +587,31 @@
 #[cfg(feature = "python")]
 impl PythonArray {
     pub fn sort(&self, _descending: bool) -> DaftResult<Self> {
         todo!("impl sort for python array")
     }
 }
 
+impl DateArray {
+    pub fn sort(&self, descending: bool) -> DaftResult<Self> {
+        let new_array = self.physical.sort(descending)?;
+        Ok(Self::new(self.field.clone(), new_array))
+    }
+}
+
 impl EmbeddingArray {
     pub fn sort(&self, _descending: bool) -> DaftResult<Self> {
-        todo!("impl sort for FixedSizeListArray")
+        todo!("impl sort for EmbeddingArray")
     }
 }
 
-impl DateArray {
-    pub fn sort(&self, descending: bool) -> DaftResult<Self> {
-        let new_array = self.physical.sort(descending)?;
-        Ok(Self::new(self.field.clone(), new_array))
+impl ImageArray {
+    pub fn sort(&self, _descending: bool) -> DaftResult<Self> {
+        todo!("impl sort for ImageArray")
+    }
+}
+
+impl FixedShapeImageArray {
+    pub fn sort(&self, _descending: bool) -> DaftResult<Self> {
+        todo!("impl sort for FixedShapeImageArray")
     }
 }
```

### Comparing `getdaft-0.1.3/src/array/ops/sum.rs` & `getdaft-0.1.4/src/array/ops/sum.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/ops/take.rs` & `getdaft-0.1.4/src/array/ops/take.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use crate::{
     array::DataArray,
     datatypes::{
-        logical::{DateArray, EmbeddingArray},
+        logical::{DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray},
         BinaryArray, BooleanArray, DaftIntegerType, DaftNumericType, ExtensionArray,
         FixedSizeListArray, ListArray, NullArray, StructArray, Utf8Array,
     },
     error::DaftResult,
 };
 
 use super::as_arrow::AsArrow;
@@ -464,14 +464,87 @@
     #[inline]
     pub fn get(&self, idx: usize) -> Option<Box<dyn arrow2::array::Array>> {
         if idx >= self.len() {
             panic!("Out of bounds: {} vs len: {}", idx, self.len())
         }
         let arrow_array = self.as_arrow();
         let is_valid = arrow_array
+            .validity()
+            .map_or(true, |validity| validity.get_bit(idx));
+        if is_valid {
+            Some(unsafe { arrow_array.value_unchecked(idx) })
+        } else {
+            None
+        }
+    }
+
+    pub fn take<I>(&self, idx: &DataArray<I>) -> DaftResult<Self>
+    where
+        I: DaftIntegerType,
+        <I as DaftNumericType>::Native: arrow2::types::Index,
+    {
+        let new_array = self.physical.take(idx)?;
+        Ok(Self::new(self.field.clone(), new_array))
+    }
+
+    pub fn str_value(&self, idx: usize) -> DaftResult<String> {
+        let val = self.get(idx);
+        match val {
+            None => Ok("None".to_string()),
+            Some(v) => Ok(format!("{v:?}")),
+        }
+    }
+}
+
+impl ImageArray {
+    #[inline]
+    pub fn get(&self, idx: usize) -> Option<Box<dyn arrow2::array::Array>> {
+        if idx >= self.len() {
+            panic!("Out of bounds: {} vs len: {}", idx, self.len())
+        }
+        let arrow_array = self.as_arrow();
+        let is_valid = arrow_array
+            .validity()
+            .map_or(true, |validity| validity.get_bit(idx));
+        if is_valid {
+            let data_array = arrow_array.values()[0]
+                .as_any()
+                .downcast_ref::<arrow2::array::ListArray<i64>>()?;
+            Some(unsafe { data_array.value_unchecked(idx) })
+        } else {
+            None
+        }
+    }
+
+    pub fn take<I>(&self, idx: &DataArray<I>) -> DaftResult<Self>
+    where
+        I: DaftIntegerType,
+        <I as DaftNumericType>::Native: arrow2::types::Index,
+    {
+        let new_array = self.physical.take(idx)?;
+        Ok(Self::new(self.field.clone(), new_array))
+    }
+
+    pub fn str_value(&self, idx: usize) -> DaftResult<String> {
+        let val = self.get(idx);
+        match val {
+            None => Ok("None".to_string()),
+            Some(v) => Ok(format!("{v:?}")),
+        }
+    }
+}
+
+impl FixedShapeImageArray {
+    #[inline]
+    pub fn get(&self, idx: usize) -> Option<Box<dyn arrow2::array::Array>> {
+        if idx >= self.len() {
+            panic!("Out of bounds: {} vs len: {}", idx, self.len())
+        }
+        let arrow_array = self.as_arrow();
+        let is_valid = arrow_array
             .validity()
             .map_or(true, |validity| validity.get_bit(idx));
         if is_valid {
             Some(unsafe { arrow_array.value_unchecked(idx) })
         } else {
             None
         }
```

### Comparing `getdaft-0.1.3/src/array/ops/utf8.rs` & `getdaft-0.1.4/src/array/ops/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/pseudo_arrow/compute.rs` & `getdaft-0.1.4/src/array/pseudo_arrow/compute.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/pseudo_arrow/mod.rs` & `getdaft-0.1.4/src/array/pseudo_arrow/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/array/pseudo_arrow/python.rs` & `getdaft-0.1.4/src/array/pseudo_arrow/python.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/datatypes/dtype.rs` & `getdaft-0.1.4/src/datatypes/dtype.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use std::fmt::{Display, Formatter, Result};
 
 use arrow2::datatypes::DataType as ArrowType;
 
 use crate::{
-    datatypes::{field::Field, time_unit::TimeUnit},
+    datatypes::{field::Field, image_mode::ImageMode, time_unit::TimeUnit},
     error::{DaftError, DaftResult},
 };
 
 use serde::{Deserialize, Serialize};
 
 // pub type TimeZone = String;
 
@@ -71,16 +71,20 @@
     /// A list of some logical data type whose offsets are represented as [`i64`].
     List(Box<Field>),
     /// A nested [`DataType`] with a given number of [`Field`]s.
     Struct(Vec<Field>),
     /// Extension type.
     Extension(String, Box<DataType>, Option<String>),
     // Stop ArrowTypes
-    /// A Embedding Logical Type
+    /// A logical type for embeddings.
     Embedding(Box<Field>, usize),
+    /// A logical type for images with variable shapes.
+    Image(Box<DataType>, Option<ImageMode>),
+    /// A logical type for images with the same size (height x width).
+    FixedShapeImage(Box<DataType>, ImageMode, u32, u32),
     Python,
     Unknown,
 }
 
 #[derive(Serialize, Deserialize)]
 struct DataTypePayload {
     datatype: DataType,
@@ -139,15 +143,15 @@
                 ArrowType::Struct(fields)
             }),
             DataType::Extension(name, dtype, metadata) => Ok(ArrowType::Extension(
                 name.clone(),
                 Box::new(dtype.to_arrow()?),
                 metadata.clone(),
             )),
-            DataType::Embedding(..) => {
+            DataType::Embedding(..) | DataType::Image(..) | DataType::FixedShapeImage(..) => {
                 let physical = Box::new(self.to_physical());
                 let embedding_extension = DataType::Extension(
                     DAFT_SUPER_EXTENSION_NAME.into(),
                     physical,
                     Some(self.to_json()?),
                 );
                 embedding_extension.to_arrow()
@@ -174,14 +178,28 @@
                 ),
                 *size,
             ),
             Embedding(field, size) => FixedSizeList(
                 Box::new(Field::new(field.name.clone(), field.dtype.to_physical())),
                 *size,
             ),
+            Image(dtype, _) => Struct(vec![
+                Field::new(
+                    "data",
+                    List(Box::new(Field::new("data", dtype.to_physical()))),
+                ),
+                Field::new("channel", UInt16),
+                Field::new("height", UInt32),
+                Field::new("width", UInt32),
+                Field::new("mode", UInt8),
+            ]),
+            FixedShapeImage(dtype, mode, height, width) => FixedSizeList(
+                Box::new(Field::new("data", dtype.to_physical())),
+                usize::try_from(mode.num_channels() as u32 * height * width).unwrap(),
+            ),
             _ => self.clone(),
         }
     }
 
     #[inline]
     pub fn is_arrow(&self) -> bool {
         self.to_arrow().is_ok()
@@ -259,15 +277,21 @@
             DataType::Extension(_, inner, _) => inner.is_python(),
             _ => false,
         }
     }
 
     #[inline]
     pub fn is_logical(&self) -> bool {
-        matches!(self, DataType::Date | DataType::Embedding(..))
+        matches!(
+            self,
+            DataType::Date
+                | DataType::Embedding(..)
+                | DataType::Image(..)
+                | DataType::FixedShapeImage(..)
+        )
     }
 
     #[inline]
     pub fn is_physical(&self) -> bool {
         !self.is_logical()
     }
 
@@ -356,30 +380,52 @@
             }
 
             _ => panic!("DataType :{item:?} is not supported"),
         }
     }
 }
 
+impl From<&ImageMode> for DataType {
+    fn from(mode: &ImageMode) -> Self {
+        use ImageMode::*;
+
+        match mode {
+            L16 | LA16 | RGB16 | RGBA16 => DataType::UInt16,
+            RGB32F | RGBA32F => DataType::Float32,
+            _ => DataType::UInt8,
+        }
+    }
+}
+
 impl Display for DataType {
     // `f` is a buffer, and this method must write the formatted string into it
     fn fmt(&self, f: &mut Formatter) -> Result {
         match self {
             DataType::List(nested) => write!(f, "List[{}:{}]", nested.name, nested.dtype),
             DataType::FixedSizeList(inner, size) => {
                 write!(f, "FixedSizeList[{}; {}]", inner.dtype, size)
             }
-            DataType::Embedding(inner, size) => {
-                write!(f, "Embedding[{}; {}]", inner.dtype, size)
-            }
             DataType::Struct(fields) => {
                 let fields: String = fields
                     .iter()
                     .map(|f| format!("{}: {}", f.name, f.dtype))
                     .collect::<Vec<String>>()
                     .join(", ");
                 write!(f, "Struct[{fields}]")
             }
+            DataType::Embedding(inner, size) => {
+                write!(f, "Embedding[{}; {}]", inner.dtype, size)
+            }
+            DataType::Image(dtype, mode) => {
+                write!(f, "Image[{}; {:?}]", dtype, mode)
+            }
+            DataType::FixedShapeImage(dtype, mode, height, width) => {
+                write!(
+                    f,
+                    "Image[{}; {:?}; {:?} x {:?}]",
+                    dtype, mode, height, width
+                )
+            }
             _ => write!(f, "{self:?}"),
         }
     }
 }
```

### Comparing `getdaft-0.1.3/src/datatypes/field.rs` & `getdaft-0.1.4/src/datatypes/field.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/datatypes/logical.rs` & `getdaft-0.1.4/src/datatypes/logical.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 use std::{marker::PhantomData, sync::Arc};
 
 use crate::{
     datatypes::{DaftLogicalType, DateType, Field},
     error::DaftResult,
 };
 
-use super::{DataArray, DataType, EmbeddingType};
-
+use super::{DataArray, DataType, EmbeddingType, FixedShapeImageType, ImageType};
 pub struct LogicalArray<L: DaftLogicalType> {
     pub field: Arc<Field>,
     pub physical: DataArray<L::PhysicalType>,
     marker_: PhantomData<L>,
 }
 
 impl<L: DaftLogicalType + 'static> LogicalArray<L> {
@@ -90,7 +89,9 @@
         let concatd = DataArray::<L::PhysicalType>::concat(physicals.as_slice())?;
         Ok(Self::new(arrays.first().unwrap().field.clone(), concatd))
     }
 }
 
 pub type DateArray = LogicalArray<DateType>;
 pub type EmbeddingArray = LogicalArray<EmbeddingType>;
+pub type ImageArray = LogicalArray<ImageType>;
+pub type FixedShapeImageArray = LogicalArray<FixedShapeImageType>;
```

### Comparing `getdaft-0.1.3/src/datatypes/matching.rs` & `getdaft-0.1.4/src/datatypes/matching.rs`

 * *Files 1% similar despite different names*

```diff
@@ -228,10 +228,12 @@
     use $crate::datatypes::DataType::*;
     #[allow(unused_imports)]
     use $crate::datatypes::*;
 
     match $key_type {
         Date => __with_ty__! { DateType },
         Embedding(..) => __with_ty__! { EmbeddingType },
+        Image(..) => __with_ty__! { ImageType },
+        FixedShapeImage(..) => __with_ty__! { FixedShapeImageType },
         _ => panic!("{:?} not implemented for with_match_daft_logical_types", $key_type)
     }
 })}
```

### Comparing `getdaft-0.1.3/src/datatypes/mod.rs` & `getdaft-0.1.4/src/datatypes/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 mod dtype;
 mod field;
+mod image_mode;
 mod matching;
 mod time_unit;
 
 use std::ops::{Add, Div, Mul, Rem, Sub};
 
 pub use crate::array::DataArray;
 use arrow2::{
     compute::{arithmetics::basic::NativeArithmetics, comparison::Simd8},
     types::{simd::Simd, NativeType},
 };
 pub use dtype::DataType;
 pub use field::Field;
+pub use image_mode::ImageMode;
 use num_traits::{Bounded, Float, FromPrimitive, Num, NumCast, ToPrimitive, Zero};
 pub use time_unit::TimeUnit;
 pub mod logical;
 
 /// Trait to wrap DataType Enum
 pub trait DaftDataType: Sync + Send {
     // returns Daft DataType Enum
@@ -103,14 +105,16 @@
 impl_daft_non_arrow_datatype!(PythonType, Python);
 
 impl_daft_logical_datatype!(TimestampType, Unknown, Int64Type);
 impl_daft_logical_datatype!(DateType, Date, Int32Type);
 impl_daft_logical_datatype!(TimeType, Unknown, Int64Type);
 impl_daft_logical_datatype!(DurationType, Unknown, Int64Type);
 impl_daft_logical_datatype!(EmbeddingType, Unknown, FixedSizeListType);
+impl_daft_logical_datatype!(ImageType, Unknown, StructType);
+impl_daft_logical_datatype!(FixedShapeImageType, Unknown, FixedSizeListType);
 
 pub trait NumericNative:
     PartialOrd
     + NativeType
     + Num
     + NumCast
     + Zero
```

### Comparing `getdaft-0.1.3/src/datatypes/time_unit.rs` & `getdaft-0.1.4/src/datatypes/time_unit.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/dsl/arithmetic.rs` & `getdaft-0.1.4/src/dsl/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/dsl/expr.rs` & `getdaft-0.1.4/src/dsl/expr.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/dsl/functions/float/is_nan.rs` & `getdaft-0.1.4/src/dsl/functions/float/is_nan.rs`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             _ => Err(DaftError::SchemaMismatch(format!(
                 "Expected 1 input args, got {}",
                 inputs.len()
             ))),
         }
     }
 
-    fn evaluate(&self, inputs: &[Series]) -> DaftResult<Series> {
+    fn evaluate(&self, inputs: &[Series], _: &Expr) -> DaftResult<Series> {
         match inputs {
             [data] => data.is_nan(),
             _ => Err(DaftError::ValueError(format!(
                 "Expected 1 input args, got {}",
                 inputs.len()
             ))),
         }
```

### Comparing `getdaft-0.1.3/src/dsl/functions/float/mod.rs` & `getdaft-0.1.4/src/dsl/functions/float/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/dsl/functions/list/explode.rs` & `getdaft-0.1.4/src/dsl/functions/list/explode.rs`

 * *Files 11% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             _ => Err(DaftError::SchemaMismatch(format!(
                 "Expected 1 input arg, got {}",
                 inputs.len()
             ))),
         }
     }
 
-    fn evaluate(&self, inputs: &[Series]) -> DaftResult<Series> {
+    fn evaluate(&self, inputs: &[Series], _: &Expr) -> DaftResult<Series> {
         match inputs {
             [input] => input.explode(),
             _ => Err(DaftError::ValueError(format!(
                 "Expected 1 input arg, got {}",
                 inputs.len()
             ))),
         }
```

### Comparing `getdaft-0.1.3/src/dsl/functions/list/mod.rs` & `getdaft-0.1.4/src/dsl/functions/list/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/dsl/functions/mod.rs` & `getdaft-0.1.4/src/dsl/functions/mod.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 pub mod float;
+pub mod image;
 pub mod list;
 pub mod numeric;
 pub mod temporal;
 pub mod utf8;
 
+use self::float::FloatExpr;
+use self::image::ImageExpr;
+use self::list::ListExpr;
+use self::numeric::NumericExpr;
 use self::temporal::TemporalExpr;
+use self::utf8::Utf8Expr;
 use crate::{datatypes::Field, error::DaftResult, schema::Schema, series::Series};
-use float::FloatExpr;
-use list::ListExpr;
-use numeric::NumericExpr;
 use serde::{Deserialize, Serialize};
-use utf8::Utf8Expr;
 
 #[cfg(feature = "python")]
 pub mod python;
 #[cfg(feature = "python")]
 use python::PythonUDF;
 
 use super::Expr;
@@ -22,34 +24,36 @@
 #[derive(Debug, Clone, Serialize, Deserialize, PartialEq)]
 pub enum FunctionExpr {
     Numeric(NumericExpr),
     Float(FloatExpr),
     Utf8(Utf8Expr),
     Temporal(TemporalExpr),
     List(ListExpr),
+    Image(ImageExpr),
     #[cfg(feature = "python")]
     Python(PythonUDF),
 }
 
 pub trait FunctionEvaluator {
     fn fn_name(&self) -> &'static str;
     fn to_field(&self, inputs: &[Expr], schema: &Schema) -> DaftResult<Field>;
-    fn evaluate(&self, inputs: &[Series]) -> DaftResult<Series>;
+    fn evaluate(&self, inputs: &[Series], expr: &Expr) -> DaftResult<Series>;
 }
 
 impl FunctionExpr {
     #[inline]
     fn get_evaluator(&self) -> &dyn FunctionEvaluator {
         use FunctionExpr::*;
         match self {
             Numeric(expr) => expr.get_evaluator(),
             Float(expr) => expr.get_evaluator(),
             Utf8(expr) => expr.get_evaluator(),
             Temporal(expr) => expr.get_evaluator(),
             List(expr) => expr.get_evaluator(),
+            Image(expr) => expr.get_evaluator(),
             #[cfg(feature = "python")]
             Python(expr) => expr,
         }
     }
 }
 
 impl FunctionEvaluator for FunctionExpr {
@@ -57,11 +61,11 @@
         self.get_evaluator().fn_name()
     }
 
     fn to_field(&self, inputs: &[Expr], schema: &Schema) -> DaftResult<Field> {
         self.get_evaluator().to_field(inputs, schema)
     }
 
-    fn evaluate(&self, inputs: &[Series]) -> DaftResult<Series> {
-        self.get_evaluator().evaluate(inputs)
+    fn evaluate(&self, inputs: &[Series], expr: &Expr) -> DaftResult<Series> {
+        self.get_evaluator().evaluate(inputs, expr)
     }
 }
```

### Comparing `getdaft-0.1.3/src/dsl/functions/numeric/abs.rs` & `getdaft-0.1.4/src/dsl/functions/numeric/abs.rs`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                 "Expected input to abs to be numeric, got {}",
                 field.dtype
             )));
         }
         Ok(field)
     }
 
-    fn evaluate(&self, inputs: &[Series]) -> DaftResult<Series> {
+    fn evaluate(&self, inputs: &[Series], _: &Expr) -> DaftResult<Series> {
         if inputs.len() != 1 {
             return Err(DaftError::ValueError(format!(
                 "Expected 1 input arg, got {}",
                 inputs.len()
             )));
         }
         inputs.first().unwrap().abs()
```

### Comparing `getdaft-0.1.3/src/dsl/functions/numeric/mod.rs` & `getdaft-0.1.4/src/dsl/functions/numeric/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/dsl/functions/python/mod.rs` & `getdaft-0.1.4/src/dsl/functions/python/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/dsl/functions/python/partial_udf.rs` & `getdaft-0.1.4/src/dsl/functions/python/partial_udf.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/dsl/functions/python/udf.rs` & `getdaft-0.1.4/src/dsl/functions/python/udf.rs`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             [] => Err(DaftError::ValueError(
                 "Cannot run UDF with 0 expression arguments".into(),
             )),
             [first, ..] => Ok(Field::new(first.name()?, self.return_dtype.clone())),
         }
     }
 
-    fn evaluate(&self, inputs: &[Series]) -> DaftResult<Series> {
+    fn evaluate(&self, inputs: &[Series], _: &Expr) -> DaftResult<Series> {
         use pyo3::Python;
 
         if inputs.len() != self.num_expressions {
             return Err(DaftError::SchemaMismatch(format!(
                 "Number of inputs required by UDF {} does not match number of inputs provided: {}",
                 self.num_expressions,
                 inputs.len()
```

### Comparing `getdaft-0.1.3/src/dsl/functions/temporal/day.rs` & `getdaft-0.1.4/src/dsl/functions/temporal/day.rs`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             _ => Err(DaftError::SchemaMismatch(format!(
                 "Expected 1 input arg, got {}",
                 inputs.len()
             ))),
         }
     }
 
-    fn evaluate(&self, inputs: &[Series]) -> DaftResult<Series> {
+    fn evaluate(&self, inputs: &[Series], _: &Expr) -> DaftResult<Series> {
         match inputs {
             [input] => input.dt_day(),
             _ => Err(DaftError::ValueError(format!(
                 "Expected 1 input arg, got {}",
                 inputs.len()
             ))),
         }
```

### Comparing `getdaft-0.1.3/src/dsl/functions/temporal/day_of_week.rs` & `getdaft-0.1.4/src/dsl/functions/utf8/length.rs`

 * *Files 10% similar despite different names*

```diff
@@ -4,43 +4,42 @@
     error::{DaftError, DaftResult},
     schema::Schema,
     series::Series,
 };
 
 use super::super::FunctionEvaluator;
 
-pub(super) struct DayOfWeekEvaluator {}
+pub(super) struct LengthEvaluator {}
 
-impl FunctionEvaluator for DayOfWeekEvaluator {
+impl FunctionEvaluator for LengthEvaluator {
     fn fn_name(&self) -> &'static str {
-        "day_of_week"
+        "length"
     }
 
     fn to_field(&self, inputs: &[Expr], schema: &Schema) -> DaftResult<Field> {
         match inputs {
-            [input] => match input.to_field(schema) {
-                Ok(field) if field.dtype.is_temporal() => {
-                    Ok(Field::new(field.name, DataType::UInt32))
-                }
-                Ok(field) => Err(DaftError::TypeError(format!(
-                    "Expected input to day to be temporal, got {}",
-                    field.dtype
-                ))),
+            [data] => match data.to_field(schema) {
+                Ok(data_field) => match &data_field.dtype {
+                    DataType::Utf8 => Ok(Field::new(data_field.name, DataType::UInt64)),
+                    _ => Err(DaftError::TypeError(format!(
+                        "Expects input to length to be utf8, but received {data_field}",
+                    ))),
+                },
                 Err(e) => Err(e),
             },
             _ => Err(DaftError::SchemaMismatch(format!(
-                "Expected 1 input arg, got {}",
+                "Expected 1 input args, got {}",
                 inputs.len()
             ))),
         }
     }
 
-    fn evaluate(&self, inputs: &[Series]) -> DaftResult<Series> {
+    fn evaluate(&self, inputs: &[Series], _: &Expr) -> DaftResult<Series> {
         match inputs {
-            [input] => input.dt_day_of_week(),
+            [data] => data.utf8_length(),
             _ => Err(DaftError::ValueError(format!(
-                "Expected 1 input arg, got {}",
+                "Expected 1 input args, got {}",
                 inputs.len()
             ))),
         }
     }
 }
```

### Comparing `getdaft-0.1.3/src/dsl/functions/temporal/mod.rs` & `getdaft-0.1.4/src/dsl/functions/temporal/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/dsl/functions/temporal/month.rs` & `getdaft-0.1.4/src/dsl/functions/temporal/month.rs`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             _ => Err(DaftError::SchemaMismatch(format!(
                 "Expected 1 input arg, got {}",
                 inputs.len()
             ))),
         }
     }
 
-    fn evaluate(&self, inputs: &[Series]) -> DaftResult<Series> {
+    fn evaluate(&self, inputs: &[Series], _: &Expr) -> DaftResult<Series> {
         match inputs {
             [input] => input.dt_month(),
             _ => Err(DaftError::ValueError(format!(
                 "Expected 1 input arg, got {}",
                 inputs.len()
             ))),
         }
```

### Comparing `getdaft-0.1.3/src/dsl/functions/temporal/year.rs` & `getdaft-0.1.4/src/dsl/functions/temporal/year.rs`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             _ => Err(DaftError::SchemaMismatch(format!(
                 "Expected 1 input arg, got {}",
                 inputs.len()
             ))),
         }
     }
 
-    fn evaluate(&self, inputs: &[Series]) -> DaftResult<Series> {
+    fn evaluate(&self, inputs: &[Series], _: &Expr) -> DaftResult<Series> {
         match inputs {
             [input] => input.dt_year(),
             _ => Err(DaftError::ValueError(format!(
                 "Expected 1 input arg, got {}",
                 inputs.len()
             ))),
         }
```

### Comparing `getdaft-0.1.3/src/dsl/functions/utf8/contains.rs` & `getdaft-0.1.4/src/dsl/functions/utf8/contains.rs`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             _ => Err(DaftError::SchemaMismatch(format!(
                 "Expected 2 input args, got {}",
                 inputs.len()
             ))),
         }
     }
 
-    fn evaluate(&self, inputs: &[Series]) -> DaftResult<Series> {
+    fn evaluate(&self, inputs: &[Series], _: &Expr) -> DaftResult<Series> {
         match inputs {
             [data, pattern] => data.utf8_contains(pattern),
             _ => Err(DaftError::ValueError(format!(
                 "Expected 2 input args, got {}",
                 inputs.len()
             ))),
         }
```

### Comparing `getdaft-0.1.3/src/dsl/functions/utf8/endswith.rs` & `getdaft-0.1.4/src/dsl/functions/utf8/endswith.rs`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             _ => Err(DaftError::SchemaMismatch(format!(
                 "Expected 2 input args, got {}",
                 inputs.len()
             ))),
         }
     }
 
-    fn evaluate(&self, inputs: &[Series]) -> DaftResult<Series> {
+    fn evaluate(&self, inputs: &[Series], _: &Expr) -> DaftResult<Series> {
         match inputs {
             [data, pattern] => data.utf8_endswith(pattern),
             _ => Err(DaftError::ValueError(format!(
                 "Expected 2 input args, got {}",
                 inputs.len()
             ))),
         }
```

### Comparing `getdaft-0.1.3/src/dsl/functions/utf8/length.rs` & `getdaft-0.1.4/src/dsl/functions/temporal/day_of_week.rs`

 * *Files 24% similar despite different names*

```diff
@@ -4,42 +4,43 @@
     error::{DaftError, DaftResult},
     schema::Schema,
     series::Series,
 };
 
 use super::super::FunctionEvaluator;
 
-pub(super) struct LengthEvaluator {}
+pub(super) struct DayOfWeekEvaluator {}
 
-impl FunctionEvaluator for LengthEvaluator {
+impl FunctionEvaluator for DayOfWeekEvaluator {
     fn fn_name(&self) -> &'static str {
-        "length"
+        "day_of_week"
     }
 
     fn to_field(&self, inputs: &[Expr], schema: &Schema) -> DaftResult<Field> {
         match inputs {
-            [data] => match data.to_field(schema) {
-                Ok(data_field) => match &data_field.dtype {
-                    DataType::Utf8 => Ok(Field::new(data_field.name, DataType::UInt64)),
-                    _ => Err(DaftError::TypeError(format!(
-                        "Expects input to length to be utf8, but received {data_field}",
-                    ))),
-                },
+            [input] => match input.to_field(schema) {
+                Ok(field) if field.dtype.is_temporal() => {
+                    Ok(Field::new(field.name, DataType::UInt32))
+                }
+                Ok(field) => Err(DaftError::TypeError(format!(
+                    "Expected input to day to be temporal, got {}",
+                    field.dtype
+                ))),
                 Err(e) => Err(e),
             },
             _ => Err(DaftError::SchemaMismatch(format!(
-                "Expected 1 input args, got {}",
+                "Expected 1 input arg, got {}",
                 inputs.len()
             ))),
         }
     }
 
-    fn evaluate(&self, inputs: &[Series]) -> DaftResult<Series> {
+    fn evaluate(&self, inputs: &[Series], _: &Expr) -> DaftResult<Series> {
         match inputs {
-            [data] => data.utf8_length(),
+            [input] => input.dt_day_of_week(),
             _ => Err(DaftError::ValueError(format!(
-                "Expected 1 input args, got {}",
+                "Expected 1 input arg, got {}",
                 inputs.len()
             ))),
         }
     }
 }
```

### Comparing `getdaft-0.1.3/src/dsl/functions/utf8/mod.rs` & `getdaft-0.1.4/src/dsl/functions/utf8/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/dsl/functions/utf8/startswith.rs` & `getdaft-0.1.4/src/dsl/functions/utf8/startswith.rs`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             _ => Err(DaftError::SchemaMismatch(format!(
                 "Expected 2 input args, got {}",
                 inputs.len()
             ))),
         }
     }
 
-    fn evaluate(&self, inputs: &[Series]) -> DaftResult<Series> {
+    fn evaluate(&self, inputs: &[Series], _: &Expr) -> DaftResult<Series> {
         match inputs {
             [data, pattern] => data.utf8_startswith(pattern),
             _ => Err(DaftError::ValueError(format!(
                 "Expected 2 input args, got {}",
                 inputs.len()
             ))),
         }
```

### Comparing `getdaft-0.1.3/src/dsl/lit.rs` & `getdaft-0.1.4/src/dsl/lit.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/dsl/optimization.rs` & `getdaft-0.1.4/src/dsl/optimization.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/dsl/pyobject.rs` & `getdaft-0.1.4/src/dsl/pyobject.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/error.rs` & `getdaft-0.1.4/src/error.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/ffi.rs` & `getdaft-0.1.4/src/ffi.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/kernels/hashing.rs` & `getdaft-0.1.4/src/kernels/hashing.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/kernels/search_sorted.rs` & `getdaft-0.1.4/src/kernels/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/kernels/utf8.rs` & `getdaft-0.1.4/src/kernels/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/lib.rs` & `getdaft-0.1.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/python/datatype.rs` & `getdaft-0.1.4/src/python/datatype.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::datatypes::{DataType, Field};
+use crate::datatypes::{DataType, Field, ImageMode};
 use pyo3::{
     exceptions::PyValueError,
     prelude::*,
     types::{PyBytes, PyDict, PyString, PyTuple},
 };
 
 #[pyclass]
@@ -121,36 +121,14 @@
             Box::new(Field::new(name, data_type.dtype)),
             usize::try_from(size)?,
         )
         .into())
     }
 
     #[staticmethod]
-    pub fn embedding(name: &str, data_type: Self, size: i64) -> PyResult<Self> {
-        if size <= 0 {
-            return Err(PyValueError::new_err(format!(
-                "The size for embedding types must be a positive integer, but got: {}",
-                size
-            )));
-        }
-        if !data_type.dtype.is_numeric() {
-            return Err(PyValueError::new_err(format!(
-                "The data type for an embedding must be numeric, but got: {}",
-                data_type.dtype
-            )));
-        }
-
-        Ok(DataType::Embedding(
-            Box::new(Field::new(name, data_type.dtype)),
-            usize::try_from(size)?,
-        )
-        .into())
-    }
-
-    #[staticmethod]
     pub fn r#struct(fields: &PyDict) -> PyResult<Self> {
         Ok(DataType::Struct(
             fields
                 .iter()
                 .map(|(name, dtype)| {
                     Ok(Field::new(
                         name.downcast::<PyString>()?.to_str()?,
@@ -173,14 +151,62 @@
             Box::new(storage_data_type.dtype),
             metadata.map(|s| s.to_string()),
         )
         .into())
     }
 
     #[staticmethod]
+    pub fn embedding(name: &str, data_type: Self, size: i64) -> PyResult<Self> {
+        if size <= 0 {
+            return Err(PyValueError::new_err(format!(
+                "The size for embedding types must be a positive integer, but got: {}",
+                size
+            )));
+        }
+        if !data_type.dtype.is_numeric() {
+            return Err(PyValueError::new_err(format!(
+                "The data type for an embedding must be numeric, but got: {}",
+                data_type.dtype
+            )));
+        }
+
+        Ok(DataType::Embedding(
+            Box::new(Field::new(name, data_type.dtype)),
+            usize::try_from(size)?,
+        )
+        .into())
+    }
+
+    #[staticmethod]
+    pub fn image(
+        mode: Option<ImageMode>,
+        height: Option<u32>,
+        width: Option<u32>,
+    ) -> PyResult<Self> {
+        // TODO(Clark): Make dtype optional instead of falling back to UInt8 here.
+        let dtype = mode.map_or(Box::new(DataType::UInt8), |m| Box::new(DataType::from(&m)));
+        if !dtype.is_numeric() {
+            panic!(
+                "The data type for an image must be numeric, but got: {}",
+                dtype
+            );
+        }
+        match (height, width) {
+            (Some(height), Some(width)) => {
+                let image_mode = mode.ok_or(PyValueError::new_err(
+                    "Image mode must be provided if specifying an image size.",
+                ))?;
+                Ok(DataType::FixedShapeImage(dtype, image_mode, height, width).into())
+            }
+            (None, None) => Ok(DataType::Image(dtype, mode).into()),
+            (_, _) => Err(PyValueError::new_err(format!("Height and width for image type must both be specified or both not specified, but got: height={:?}, width={:?}", height, width))),
+        }
+    }
+
+    #[staticmethod]
     pub fn python() -> PyResult<Self> {
         Ok(DataType::Python.into())
     }
 
     pub fn is_equal(&self, other: &PyAny) -> PyResult<bool> {
         if other.is_instance_of::<PyDataType>()? {
             let other = other.extract::<PyDataType>()?;
```

### Comparing `getdaft-0.1.3/src/python/expr.rs` & `getdaft-0.1.4/src/python/expr.rs`

 * *Files 1% similar despite different names*

```diff
@@ -304,14 +304,34 @@
         Ok(contains(&self.expr, &pattern.expr).into())
     }
 
     pub fn utf8_length(&self) -> PyResult<Self> {
         use dsl::functions::utf8::length;
         Ok(length(&self.expr).into())
     }
+
+    pub fn image_decode(&self) -> PyResult<Self> {
+        use dsl::functions::image::decode;
+        Ok(decode(&self.expr).into())
+    }
+
+    pub fn image_resize(&self, w: i64, h: i64) -> PyResult<Self> {
+        if w < 0 {
+            return Err(PyValueError::new_err(format!(
+                "width can not be negative: {w}"
+            )));
+        }
+        if h < 0 {
+            return Err(PyValueError::new_err(format!(
+                "height can not be negative: {h}"
+            )));
+        }
+        use dsl::functions::image::resize;
+        Ok(resize(&self.expr, w as u32, h as u32).into())
+    }
 }
 
 impl From<dsl::Expr> for PyExpr {
     fn from(value: dsl::Expr) -> Self {
         PyExpr { expr: value }
     }
 }
```

### Comparing `getdaft-0.1.3/src/python/field.rs` & `getdaft-0.1.4/src/python/field.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/python/mod.rs` & `getdaft-0.1.4/src/python/mod.rs`

 * *Files 19% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 mod error;
 mod expr;
 mod field;
 mod schema;
 mod series;
 mod table;
 
+use crate::datatypes::ImageMode;
 pub use datatype::PyDataType;
 pub use series::PySeries;
 
 pub fn register_modules(_py: Python, parent: &PyModule) -> PyResult<()> {
     parent.add_class::<expr::PyExpr>()?;
     parent.add_class::<table::PyTable>()?;
     parent.add_class::<series::PySeries>()?;
     parent.add_class::<datatype::PyDataType>()?;
     parent.add_class::<schema::PySchema>()?;
     parent.add_class::<field::PyField>()?;
+    parent.add_class::<ImageMode>()?;
 
     parent.add_wrapped(wrap_pyfunction!(expr::col))?;
     parent.add_wrapped(wrap_pyfunction!(expr::lit))?;
     parent.add_wrapped(wrap_pyfunction!(expr::udf))?;
     parent.add_wrapped(wrap_pyfunction!(expr::eq))?;
 
     Ok(())
```

### Comparing `getdaft-0.1.3/src/python/schema.rs` & `getdaft-0.1.4/src/python/schema.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/python/series.rs` & `getdaft-0.1.4/src/python/series.rs`

 * *Files 3% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         if start < 0 {
             return Err(PyValueError::new_err(format!(
                 "slice start can not be negative: {start}"
             )));
         }
         if end < 0 {
             return Err(PyValueError::new_err(format!(
-                "slice end can not be negative: {start}"
+                "slice end can not be negative: {end}"
             )));
         }
         if start > end {
             return Err(PyValueError::new_err(format!(
                 "slice length can not be negative: start: {start} end: {end}"
             )));
         }
@@ -262,14 +262,32 @@
         Ok(self.series.dt_day_of_week()?.into())
     }
 
     pub fn arr_lengths(&self) -> PyResult<Self> {
         Ok(self.series.arr_lengths()?.into_series().into())
     }
 
+    pub fn image_decode(&self) -> PyResult<Self> {
+        Ok(self.series.image_decode()?.into())
+    }
+    pub fn image_resize(&self, w: i64, h: i64) -> PyResult<Self> {
+        if w < 0 {
+            return Err(PyValueError::new_err(format!(
+                "width can not be negative: {w}"
+            )));
+        }
+        if h < 0 {
+            return Err(PyValueError::new_err(format!(
+                "height can not be negative: {h}"
+            )));
+        }
+
+        Ok(self.series.image_resize(w as u32, h as u32)?.into())
+    }
+
     pub fn if_else(&self, other: &Self, predicate: &Self) -> PyResult<Self> {
         Ok(self
             .series
             .if_else(&other.series, &predicate.series)?
             .into())
     }
```

### Comparing `getdaft-0.1.3/src/python/table.rs` & `getdaft-0.1.4/src/python/table.rs`

 * *Files 6% similar despite different names*

```diff
@@ -249,14 +249,33 @@
 
     #[staticmethod]
     pub fn concat(py: Python, tables: Vec<Self>) -> PyResult<Self> {
         let tables: Vec<_> = tables.iter().map(|t| &t.table).collect();
         py.allow_threads(|| Ok(Table::concat(tables.as_slice())?.into()))
     }
 
+    pub fn slice(&self, start: i64, end: i64) -> PyResult<Self> {
+        if start < 0 {
+            return Err(PyValueError::new_err(format!(
+                "slice start can not be negative: {start}"
+            )));
+        }
+        if end < 0 {
+            return Err(PyValueError::new_err(format!(
+                "slice end can not be negative: {start}"
+            )));
+        }
+        if start > end {
+            return Err(PyValueError::new_err(format!(
+                "slice length can not be negative: start: {start} end: {end}"
+            )));
+        }
+        Ok(self.table.slice(start as usize, end as usize)?.into())
+    }
+
     #[staticmethod]
     pub fn from_arrow_record_batches(
         py: Python,
         record_batches: Vec<&PyAny>,
         schema: &PySchema,
     ) -> PyResult<Self> {
         let table =
```

### Comparing `getdaft-0.1.3/src/schema.rs` & `getdaft-0.1.4/src/schema.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/series/array_impl/data_array.rs` & `getdaft-0.1.4/src/series/array_impl/data_array.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/series/array_impl/logical_array.rs` & `getdaft-0.1.4/src/series/array_impl/logical_array.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-use crate::datatypes::logical::DateArray;
-use crate::datatypes::logical::EmbeddingArray;
+use crate::datatypes::logical::{DateArray, EmbeddingArray, FixedShapeImageArray, ImageArray};
 
 use super::{ArrayWrapper, IntoSeries, Series};
 use crate::array::ops::GroupIndices;
 use crate::series::DaftResult;
 use crate::series::SeriesLike;
 use crate::with_match_integer_daft_types;
 use std::sync::Arc;
@@ -138,7 +137,9 @@
             }
         }
     };
 }
 
 impl_series_like_for_logical_array!(DateArray);
 impl_series_like_for_logical_array!(EmbeddingArray);
+impl_series_like_for_logical_array!(ImageArray);
+impl_series_like_for_logical_array!(FixedShapeImageArray);
```

### Comparing `getdaft-0.1.3/src/series/from.rs` & `getdaft-0.1.4/src/series/from.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/series/mod.rs` & `getdaft-0.1.4/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/series/ops/abs.rs` & `getdaft-0.1.4/src/series/ops/abs.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/series/ops/agg.rs` & `getdaft-0.1.4/src/series/ops/agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/series/ops/arithmetic.rs` & `getdaft-0.1.4/src/series/ops/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/series/ops/broadcast.rs` & `getdaft-0.1.4/src/series/ops/broadcast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/series/ops/comparison.rs` & `getdaft-0.1.4/src/series/ops/comparison.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/series/ops/concat.rs` & `getdaft-0.1.4/src/series/ops/concat.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/series/ops/date.rs` & `getdaft-0.1.4/src/series/ops/date.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/series/ops/downcast.rs` & `getdaft-0.1.4/src/series/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/series/ops/filter.rs` & `getdaft-0.1.4/src/series/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/series/ops/list.rs` & `getdaft-0.1.4/src/series/ops/list.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use crate::array::ops::as_arrow::AsArrow;
 use crate::datatypes::{DataType, UInt64Array};
 use crate::error::DaftError;
 use crate::{error::DaftResult, series::Series};
 
 impl Series {
     pub fn explode(&self) -> DaftResult<Series> {
         use DataType::*;
@@ -14,18 +15,38 @@
             ))),
         }
     }
 
     pub fn arr_lengths(&self) -> DaftResult<UInt64Array> {
         use DataType::*;
 
-        let p = self.as_physical()?;
-        match p.data_type() {
-            List(_) => p.list()?.lengths(),
-            FixedSizeList(..) => p.fixed_size_list()?.lengths(),
+        match self.data_type() {
+            List(_) => self.list()?.lengths(),
+            FixedSizeList(..) => self.fixed_size_list()?.lengths(),
+            Embedding(..) | FixedShapeImage(..) => self.as_physical()?.arr_lengths(),
+            Image(..) => {
+                let struct_array = self.as_physical()?;
+                let data_array = struct_array.struct_()?.as_arrow().values()[0]
+                    .as_any()
+                    .downcast_ref::<arrow2::array::ListArray<i64>>()
+                    .unwrap();
+                let offsets = data_array.offsets();
+
+                let mut lens = Vec::with_capacity(self.len());
+                for i in 0..self.len() {
+                    lens.push(
+                        (unsafe { offsets.get_unchecked(i + 1) - offsets.get_unchecked(i) }) as u64,
+                    )
+                }
+                let array = Box::new(
+                    arrow2::array::PrimitiveArray::from_vec(lens)
+                        .with_validity(data_array.validity().cloned()),
+                );
+                Ok(UInt64Array::from((self.name(), array)))
+            }
             dt => Err(DaftError::TypeError(format!(
                 "lengths not implemented for {}",
                 dt
             ))),
         }
     }
 }
```

### Comparing `getdaft-0.1.3/src/series/ops/mod.rs` & `getdaft-0.1.4/src/series/ops/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 pub mod date;
 pub mod downcast;
 pub mod filter;
 pub mod float;
 pub mod groups;
 pub mod hash;
 pub mod if_else;
+pub mod image;
 pub mod len;
 pub mod list;
 pub mod not;
 pub mod null;
 pub mod search_sorted;
 pub mod sort;
 pub mod take;
```

### Comparing `getdaft-0.1.3/src/series/ops/search_sorted.rs` & `getdaft-0.1.4/src/series/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/series/ops/sort.rs` & `getdaft-0.1.4/src/series/ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/series/ops/take.rs` & `getdaft-0.1.4/src/series/ops/take.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/series/ops/utf8.rs` & `getdaft-0.1.4/src/series/ops/utf8.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/series/series_like.rs` & `getdaft-0.1.4/src/series/series_like.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/table/mod.rs` & `getdaft-0.1.4/src/table/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -96,27 +96,31 @@
         if self.num_columns() == 0 {
             0
         } else {
             self.get_column_by_index(0).unwrap().len()
         }
     }
 
+    pub fn slice(&self, start: usize, end: usize) -> DaftResult<Self> {
+        let new_series: DaftResult<Vec<_>> =
+            self.columns.iter().map(|s| s.slice(start, end)).collect();
+        Ok(Table {
+            schema: self.schema.clone(),
+            columns: new_series?,
+        })
+    }
+
     pub fn head(&self, num: usize) -> DaftResult<Self> {
         if num >= self.len() {
             return Ok(Table {
                 schema: self.schema.clone(),
                 columns: self.columns.clone(),
             });
         }
-
-        let new_series: DaftResult<Vec<_>> = self.columns.iter().map(|s| s.head(num)).collect();
-        Ok(Table {
-            schema: self.schema.clone(),
-            columns: new_series?,
-        })
+        self.slice(0, num)
     }
 
     pub fn sample(&self, num: usize) -> DaftResult<Self> {
         if num >= self.len() {
             Ok(self.clone())
         } else {
             use rand::{distributions::Uniform, Rng};
@@ -300,15 +304,15 @@
                 }
             }
             Function { func, inputs } => {
                 let evaluated_inputs = inputs
                     .iter()
                     .map(|e| self.eval_expression(e))
                     .collect::<DaftResult<Vec<_>>>()?;
-                func.evaluate(evaluated_inputs.as_slice())
+                func.evaluate(evaluated_inputs.as_slice(), expr)
             }
             Literal(lit_value) => Ok(lit_value.to_series()),
             IfElse {
                 if_true,
                 if_false,
                 predicate,
             } => {
```

### Comparing `getdaft-0.1.3/src/table/ops/agg.rs` & `getdaft-0.1.4/src/table/ops/agg.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/table/ops/explode.rs` & `getdaft-0.1.4/src/table/ops/explode.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/table/ops/groups.rs` & `getdaft-0.1.4/src/table/ops/groups.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/table/ops/hash.rs` & `getdaft-0.1.4/src/table/ops/hash.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/table/ops/joins/hash_join.rs` & `getdaft-0.1.4/src/table/ops/joins/hash_join.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/table/ops/joins/mod.rs` & `getdaft-0.1.4/src/table/ops/joins/mod.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/table/ops/partition.rs` & `getdaft-0.1.4/src/table/ops/partition.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/table/ops/search_sorted.rs` & `getdaft-0.1.4/src/table/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/table/ops/sort.rs` & `getdaft-0.1.4/src/table/ops/sort.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/utils/arrow.rs` & `getdaft-0.1.4/src/utils/arrow.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/src/utils/supertype.rs` & `getdaft-0.1.4/src/utils/supertype.rs`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/assets/tpch-sqlite-queries/1.sql` & `getdaft-0.1.4/tests/assets/tpch-sqlite-queries/1.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/assets/tpch-sqlite-queries/10.sql` & `getdaft-0.1.4/tests/assets/tpch-sqlite-queries/10.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/assets/tpch-sqlite-queries/2.sql` & `getdaft-0.1.4/tests/assets/tpch-sqlite-queries/2.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/assets/tpch-sqlite-queries/7.sql` & `getdaft-0.1.4/tests/assets/tpch-sqlite-queries/7.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/assets/tpch-sqlite-queries/8.sql` & `getdaft-0.1.4/tests/assets/tpch-sqlite-queries/8.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/assets/tpch-sqlite-queries/9.sql` & `getdaft-0.1.4/tests/assets/tpch-sqlite-queries/9.sql`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/benchmarks/conftest.py` & `getdaft-0.1.4/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/benchmarks/test_df_arithmetic.py` & `getdaft-0.1.4/tests/benchmarks/test_df_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/benchmarks/test_file_read.py` & `getdaft-0.1.4/tests/benchmarks/test_file_read.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/benchmarks/test_groups_and_aggs.py` & `getdaft-0.1.4/tests/benchmarks/test_groups_and_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/benchmarks/test_join.py` & `getdaft-0.1.4/tests/benchmarks/test_join.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/benchmarks/test_repartition.py` & `getdaft-0.1.4/tests/benchmarks/test_repartition.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/benchmarks/test_sort.py` & `getdaft-0.1.4/tests/benchmarks/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/conftest.py` & `getdaft-0.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/cookbook/assets/311-service-requests.24.csv` & `getdaft-0.1.4/tests/cookbook/assets/311-service-requests.24.csv`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/cookbook/conftest.py` & `getdaft-0.1.4/tests/cookbook/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/cookbook/test_aggregations.py` & `getdaft-0.1.4/tests/cookbook/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/cookbook/test_computations.py` & `getdaft-0.1.4/tests/cookbook/test_computations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/cookbook/test_count_rows.py` & `getdaft-0.1.4/tests/cookbook/test_count_rows.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/cookbook/test_dataloading.py` & `getdaft-0.1.4/tests/cookbook/test_dataloading.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/cookbook/test_distinct.py` & `getdaft-0.1.4/tests/cookbook/test_distinct.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/cookbook/test_filter.py` & `getdaft-0.1.4/tests/cookbook/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/cookbook/test_joins.py` & `getdaft-0.1.4/tests/cookbook/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/cookbook/test_literals.py` & `getdaft-0.1.4/tests/cookbook/test_literals.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/cookbook/test_pandas_cookbook.py` & `getdaft-0.1.4/tests/cookbook/test_pandas_cookbook.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/cookbook/test_sorting.py` & `getdaft-0.1.4/tests/cookbook/test_sorting.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/cookbook/test_write.py` & `getdaft-0.1.4/tests/cookbook/test_write.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/dataframe/conftest.py` & `getdaft-0.1.4/tests/dataframe/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/dataframe/test_accessors.py` & `getdaft-0.1.4/tests/dataframe/test_accessors.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/dataframe/test_aggregations.py` & `getdaft-0.1.4/tests/dataframe/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/dataframe/test_creation.py` & `getdaft-0.1.4/tests/dataframe/test_creation.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/dataframe/test_distinct.py` & `getdaft-0.1.4/tests/dataframe/test_distinct.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/dataframe/test_explode.py` & `getdaft-0.1.4/tests/dataframe/test_explode.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/dataframe/test_filter.py` & `getdaft-0.1.4/tests/dataframe/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/dataframe/test_getitem.py` & `getdaft-0.1.4/tests/dataframe/test_getitem.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/dataframe/test_joins.py` & `getdaft-0.1.4/tests/dataframe/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/dataframe/test_repr.py` & `getdaft-0.1.4/tests/dataframe/test_repr.py`

 * *Files 12% similar despite different names*

```diff
@@ -121,7 +121,18 @@
         ),
     }
     expected_data_html = {
         **expected_data,
     }
     assert parse_str_table(df.__repr__()) == expected_data
     assert parse_html_table(df._repr_html_()) == expected_data_html
+
+
+def test_repr_with_html_string():
+    df = daft.from_pydict({"A": [f"<div>body{i}</div>" for i in range(3)]})
+    df.collect()
+
+    non_html_table = df.__repr__()
+    html_table = df._repr_html_()
+    for i in range(3):
+        assert f"<div>body{i}</div>" in non_html_table
+        assert f"<tr><td>&lt;div&gt;body{i}&lt;/div&gt;</td></tr>" in html_table
```

### Comparing `getdaft-0.1.3/tests/dataframe/test_select.py` & `getdaft-0.1.4/tests/dataframe/test_select.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/dataframe/test_show.py` & `getdaft-0.1.4/tests/dataframe/test_show.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/dataframe/test_sort.py` & `getdaft-0.1.4/tests/dataframe/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/dataframe/test_temporals.py` & `getdaft-0.1.4/tests/dataframe/test_temporals.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/dataframe/test_to_integrations.py` & `getdaft-0.1.4/tests/dataframe/test_to_integrations.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/dataframe/test_with_column.py` & `getdaft-0.1.4/tests/dataframe/test_with_column.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/expressions/test_apply.py` & `getdaft-0.1.4/tests/expressions/test_apply.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/expressions/test_expressions.py` & `getdaft-0.1.4/tests/expressions/test_expressions.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/expressions/test_expressions_projection.py` & `getdaft-0.1.4/tests/expressions/test_expressions_projection.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/expressions/test_udf.py` & `getdaft-0.1.4/tests/expressions/test_udf.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/expressions/typing/conftest.py` & `getdaft-0.1.4/tests/expressions/typing/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/expressions/typing/test_aggs.py` & `getdaft-0.1.4/tests/expressions/typing/test_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/expressions/typing/test_arithmetic.py` & `getdaft-0.1.4/tests/expressions/typing/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/expressions/typing/test_compare.py` & `getdaft-0.1.4/tests/expressions/typing/test_compare.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/expressions/typing/test_dt.py` & `getdaft-0.1.4/tests/expressions/typing/test_dt.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/expressions/typing/test_float.py` & `getdaft-0.1.4/tests/expressions/typing/test_float.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/expressions/typing/test_if_else.py` & `getdaft-0.1.4/tests/expressions/typing/test_if_else.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/expressions/typing/test_logical.py` & `getdaft-0.1.4/tests/expressions/typing/test_logical.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/expressions/typing/test_str.py` & `getdaft-0.1.4/tests/expressions/typing/test_str.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/integration/test_tpch.py` & `getdaft-0.1.4/tests/integration/test_tpch.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/optimizer/conftest.py` & `getdaft-0.1.4/tests/optimizer/conftest.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/optimizer/test_drop_projections.py` & `getdaft-0.1.4/tests/optimizer/test_drop_projections.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/optimizer/test_drop_repartition.py` & `getdaft-0.1.4/tests/optimizer/test_drop_repartition.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/optimizer/test_fold_projections.py` & `getdaft-0.1.4/tests/optimizer/test_fold_projections.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/optimizer/test_prune_columns.py` & `getdaft-0.1.4/tests/optimizer/test_prune_columns.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/optimizer/test_pushdown_clauses_into_scan.py` & `getdaft-0.1.4/tests/optimizer/test_pushdown_clauses_into_scan.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/optimizer/test_pushdown_limit.py` & `getdaft-0.1.4/tests/optimizer/test_pushdown_limit.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/optimizer/test_pushdown_predicates.py` & `getdaft-0.1.4/tests/optimizer/test_pushdown_predicates.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/property_based_testing/strategies.py` & `getdaft-0.1.4/tests/property_based_testing/strategies.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/property_based_testing/test_sort.py` & `getdaft-0.1.4/tests/property_based_testing/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/ray/test_dask.py` & `getdaft-0.1.4/tests/ray/test_dask.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/ray/test_datasets.py` & `getdaft-0.1.4/tests/ray/test_datasets.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/series/test_arithmetic.py` & `getdaft-0.1.4/tests/series/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/series/test_comparisons.py` & `getdaft-0.1.4/tests/series/test_comparisons.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/series/test_concat.py` & `getdaft-0.1.4/tests/series/test_concat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/series/test_embedding.py` & `getdaft-0.1.4/tests/series/test_embedding.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/series/test_filter.py` & `getdaft-0.1.4/tests/series/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/series/test_float.py` & `getdaft-0.1.4/tests/series/test_float.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/series/test_hash.py` & `getdaft-0.1.4/tests/series/test_hash.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/series/test_if_else.py` & `getdaft-0.1.4/tests/series/test_if_else.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/series/test_numeric_ops.py` & `getdaft-0.1.4/tests/series/test_numeric_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/series/test_series.py` & `getdaft-0.1.4/tests/series/test_series.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/series/test_size_bytes.py` & `getdaft-0.1.4/tests/series/test_size_bytes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/series/test_slice.py` & `getdaft-0.1.4/tests/series/test_slice.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/series/test_sort.py` & `getdaft-0.1.4/tests/series/test_sort.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/series/test_take.py` & `getdaft-0.1.4/tests/series/test_take.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/series/test_temporal_ops.py` & `getdaft-0.1.4/tests/series/test_temporal_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/series/test_utf8_ops.py` & `getdaft-0.1.4/tests/series/test_utf8_ops.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/table/__init__.py` & `getdaft-0.1.4/tests/table/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/table/test_blackbox_kernels.py` & `getdaft-0.1.4/tests/table/test_blackbox_kernels.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/table/test_concat.py` & `getdaft-0.1.4/tests/table/test_concat.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/table/test_eval.py` & `getdaft-0.1.4/tests/table/test_eval.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/table/test_explodes.py` & `getdaft-0.1.4/tests/table/test_explodes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/table/test_filter.py` & `getdaft-0.1.4/tests/table/test_filter.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/table/test_from_py.py` & `getdaft-0.1.4/tests/table/test_from_py.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,14 @@
             arrs[col_name] = pa.array(col, type=schema.field(col_name).type)
     expected_table = pa.table(arrs, schema=schema)
     assert table.to_arrow() == expected_table
 
 
 def test_from_pydict_arrow_roundtrip(uuid_ext_type) -> None:
     arrow_roundtrip_types, arrow_type_arrays = _with_uuid_ext_type(uuid_ext_type)
-    print(arrow_roundtrip_types)
     table = Table.from_pydict(arrow_type_arrays)
     assert len(table) == 2
     assert set(table.column_names()) == set(arrow_type_arrays.keys())
     for field in table.schema():
         assert field.dtype == DataType.from_arrow_type(arrow_type_arrays[field.name].type)
     expected_table = pa.table(arrow_type_arrays).cast(pa.schema(arrow_roundtrip_types))
     assert table.to_arrow() == expected_table
```

### Comparing `getdaft-0.1.3/tests/table/test_head.py` & `getdaft-0.1.4/tests/table/test_head.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/table/test_joins.py` & `getdaft-0.1.4/tests/table/test_joins.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/table/test_partitioning.py` & `getdaft-0.1.4/tests/table/test_partitioning.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/table/test_size_bytes.py` & `getdaft-0.1.4/tests/table/test_size_bytes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/table/test_sorting.py` & `getdaft-0.1.4/tests/table/test_sorting.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/table/test_table_aggs.py` & `getdaft-0.1.4/tests/table/test_table_aggs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/table/test_table_io.py` & `getdaft-0.1.4/tests/table/test_table_io.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/table/test_take.py` & `getdaft-0.1.4/tests/table/test_take.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/table/utf8/test_compares.py` & `getdaft-0.1.4/tests/table/utf8/test_compares.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/test_analytics.py` & `getdaft-0.1.4/tests/test_analytics.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/test_datatypes.py` & `getdaft-0.1.4/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/test_schema.py` & `getdaft-0.1.4/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tests/udf_library/test_url_udfs.py` & `getdaft-0.1.4/tests/udf_library/test_url_udfs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import pathlib
 import uuid
-from unittest.mock import patch
 
 import pandas as pd
 import pytest
 from fsspec.implementations.local import LocalFileSystem
 
 import daft
 from daft.context import get_context
@@ -44,20 +43,16 @@
     # Mark that this filesystem instance shouldn't be automatically reused by fsspec; without this,
     # fsspec would cache this instance and reuse it for Daft's default construction of filesystems,
     # which would make this test pass without the passed filesystem being used.
     fs = LocalFileSystem(skip_instance_cache=True)
 
     df = daft.from_pydict({"filenames": [str(f) for f in files]})
 
-    with patch.object(fs, "cat_file", wraps=fs.cat_file) as mock_cat:
-        df = df.with_column("bytes", col("filenames").url.download(fs=fs))
-        out_df = df.to_pandas()
-
-        # Check that cat_file() is called on the passed filesystem.
-        mock_cat.assert_called()
+    df = df.with_column("bytes", col("filenames").url.download(fs=fs))
+    out_df = df.to_pandas()
 
     pd_df = pd.DataFrame.from_dict({"filenames": [str(f) for f in files]})
     pd_df["bytes"] = pd.Series([pathlib.Path(fn).read_bytes() for fn in files])
     assert_df_equals(out_df, pd_df, sort_key="filenames")
 
 
 def test_download_with_none(files):
```

### Comparing `getdaft-0.1.3/tests_legacy/test_resource_requests.py` & `getdaft-0.1.4/tests_legacy/test_resource_requests.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tools/patch_package_version.py` & `getdaft-0.1.4/tools/patch_package_version.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tools/wheels/_vendor/wheel/LICENSE.txt` & `getdaft-0.1.4/tools/wheels/_vendor/wheel/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tools/wheels/_vendor/wheel/cli/__init__.py` & `getdaft-0.1.4/tools/wheels/_vendor/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tools/wheels/_vendor/wheel/cli/convert.py` & `getdaft-0.1.4/tools/wheels/_vendor/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tools/wheels/_vendor/wheel/cli/pack.py` & `getdaft-0.1.4/tools/wheels/_vendor/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tools/wheels/_vendor/wheel/cli/unpack.py` & `getdaft-0.1.4/tools/wheels/_vendor/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tools/wheels/_vendor/wheel/pkginfo.py` & `getdaft-0.1.4/tools/wheels/_vendor/wheel/pkginfo.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tools/wheels/_vendor/wheel/util.py` & `getdaft-0.1.4/tools/wheels/_vendor/wheel/util.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tools/wheels/_vendor/wheel/wheelfile.py` & `getdaft-0.1.4/tools/wheels/_vendor/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tools/wheels/fix-and-copy-wheel.py` & `getdaft-0.1.4/tools/wheels/fix-and-copy-wheel.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tools/wheels/tmpdirs.py` & `getdaft-0.1.4/tools/wheels/tmpdirs.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tools/wheels/tools.py` & `getdaft-0.1.4/tools/wheels/tools.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tools/wheels/wheeltools.py` & `getdaft-0.1.4/tools/wheels/wheeltools.py`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb` & `getdaft-0.1.4/tutorials/embeddings/daft_tutorial_embeddings_stackexchange.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tutorials/image_querying/top_n_red_color.ipynb` & `getdaft-0.1.4/tutorials/image_querying/top_n_red_color.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tutorials/mnist.ipynb` & `getdaft-0.1.4/tutorials/mnist.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tutorials/text_to_image/text_to_image_generation.ipynb` & `getdaft-0.1.4/tutorials/text_to_image/text_to_image_generation.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/tutorials/text_to_image/using_cloud_with_ray.ipynb` & `getdaft-0.1.4/tutorials/text_to_image/using_cloud_with_ray.ipynb`

 * *Files identical despite different names*

### Comparing `getdaft-0.1.3/Cargo.lock` & `getdaft-0.1.4/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "adler"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
+
+[[package]]
 name = "ahash"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
 dependencies = [
  "cfg-if",
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
-name = "aho-corasick"
-version = "1.0.1"
+name = "android-tzdata"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
-dependencies = [
- "memchr",
-]
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
 
 [[package]]
 name = "arc-swap"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
 
@@ -57,20 +60,17 @@
  "dyn-clone",
  "either",
  "ethnum",
  "foreign_vec",
  "getrandom",
  "hash_hasher",
  "hashbrown 0.13.2",
- "itertools",
  "lexical-core",
  "multiversion",
  "num-traits",
- "regex",
- "regex-syntax 0.6.29",
  "rustc_version",
  "simdutf8",
  "strength_reduce",
 ]
 
 [[package]]
 name = "autocfg"
@@ -91,17 +91,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bumpalo"
-version = "3.12.2"
+version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c6ed94e98ecff0c12dd1b04c15ec0d7d9458ca8fe806cea6f12954efe74c63b"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "bytemuck"
 version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
 dependencies = [
@@ -112,40 +112,61 @@
 name = "bytemuck_derive"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fdde5c9cd29ebd706ce1b35600920a33550e402fc998a2e53ad3b42c3c47a192"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.18",
 ]
 
 [[package]]
+name = "byteorder"
+version = "1.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
+
+[[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.24"
+version = "0.4.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
+checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
 dependencies = [
- "num-integer",
+ "android-tzdata",
  "num-traits",
 ]
 
 [[package]]
+name = "color_quant"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3d7b894f5411737b7867f4827955924d7c254fc9f4d91a6aad6b097804b1018b"
+
+[[package]]
+name = "crc32fast"
+version = "1.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
+dependencies = [
+ "cfg-if",
+]
+
+[[package]]
 name = "csv"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b015497079b9a9d69c02ad25de6c0a6edef051ea6360a327d0bd05802ef64ad"
 dependencies = [
  "csv-core",
  "itoa",
@@ -160,23 +181,26 @@
 checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "daft"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "arrow2",
  "bincode",
  "dyn-clone",
  "fnv",
+ "image",
  "indexmap",
  "lazy_static",
  "log",
+ "ndarray",
+ "num-derive",
  "num-traits",
  "numpy",
  "prettytable-rs",
  "pyo3",
  "pyo3-log",
  "rand",
  "serde",
@@ -247,14 +271,33 @@
 [[package]]
 name = "ethnum"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0198b9d0078e0f30dedc7acbb21c974e838fc8fae3ee170128658a98cb2c1c04"
 
 [[package]]
+name = "fdeflate"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d329bdeac514ee06249dabc27877490f17f5d371ec693360768b838e19f3ae10"
+dependencies = [
+ "simd-adler32",
+]
+
+[[package]]
+name = "flate2"
+version = "1.0.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
+dependencies = [
+ "crc32fast",
+ "miniz_oxide",
+]
+
+[[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "foreign_vec"
@@ -272,14 +315,24 @@
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "gif"
+version = "0.12.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "80792593675e051cf94a4b111980da2ba60d4a83e43e0048c5693baab3977045"
+dependencies = [
+ "color_quant",
+ "weezl",
+]
+
+[[package]]
 name = "hash_hasher"
 version = "2.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "74721d007512d0cb3338cd20f0654ac913920061a4c4d0d8708edb3f2a698c0c"
 
 [[package]]
 name = "hashbrown"
@@ -296,14 +349,31 @@
 [[package]]
 name = "hermit-abi"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
+name = "image"
+version = "0.24.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "527909aa81e20ac3a44803521443a765550f09b5130c2c2fa1ea59c2f8f50a3a"
+dependencies = [
+ "bytemuck",
+ "byteorder",
+ "color_quant",
+ "gif",
+ "jpeg-decoder",
+ "num-rational",
+ "num-traits",
+ "png",
+ "tiff",
+]
+
+[[package]]
 name = "indexmap"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
@@ -314,17 +384,17 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "io-lifetimes"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
+checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
  "hermit-abi",
  "libc",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
@@ -336,29 +406,26 @@
  "hermit-abi",
  "io-lifetimes",
  "rustix",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
-name = "itertools"
-version = "0.10.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
-dependencies = [
- "either",
-]
-
-[[package]]
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
+name = "jpeg-decoder"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bc0000e42512c92e31c2252315bda326620a4e034105e900c98ec492fa077b3e"
+
+[[package]]
 name = "js-sys"
 version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
 dependencies = [
  "wasm-bindgen",
 ]
@@ -437,36 +504,33 @@
 name = "libc"
 version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.3.7"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ece97ea872ece730aed82664c424eb4c8291e1ff2480247ccf7409044bc6479f"
+checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
 
 [[package]]
 name = "matrixmultiply"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
 dependencies = [
@@ -486,14 +550,24 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "miniz_oxide"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+dependencies = [
+ "adler",
+ "simd-adler32",
+]
+
+[[package]]
 name = "multiversion"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8cda45dade5144c2c929bf2ed6c24bebbba784e9198df049ec87d722b9462bd1"
 dependencies = [
  "multiversion-macros",
  "target-features",
@@ -530,24 +604,46 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
+name = "num-derive"
+version = "0.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "876a53fff98e03a936a674b29568b0e605f06b29372c2489ff4de23f1949743d"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "num-integer"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
 dependencies = [
  "autocfg",
  "num-traits",
 ]
 
 [[package]]
+name = "num-rational"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
+dependencies = [
+ "autocfg",
+ "num-integer",
+ "num-traits",
+]
+
+[[package]]
 name = "num-traits"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
@@ -565,17 +661,17 @@
  "num-traits",
  "pyo3",
  "rustc-hash",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
@@ -602,14 +698,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
 dependencies = [
  "array-init-cursor",
 ]
 
 [[package]]
+name = "png"
+version = "0.17.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aaeebc51f9e7d2c150d3f3bfeb667f2aa985db5ef1e3d212847bdedb488beeaa"
+dependencies = [
+ "bitflags",
+ "crc32fast",
+ "fdeflate",
+ "flate2",
+ "miniz_oxide",
+]
+
+[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "prettytable-rs"
@@ -623,17 +732,17 @@
  "lazy_static",
  "term",
  "unicode-width",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa1fb82fc0c281dd9671101b66b771ebbe1eaf967b96ac8740dcba4b70005ca8"
+checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.3"
@@ -703,17 +812,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.27"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -767,37 +876,14 @@
 dependencies = [
  "getrandom",
  "redox_syscall",
  "thiserror",
 ]
 
 [[package]]
-name = "regex"
-version = "1.8.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
-dependencies = [
- "aho-corasick",
- "memchr",
- "regex-syntax 0.7.1",
-]
-
-[[package]]
-name = "regex-syntax"
-version = "0.6.29"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
-
-[[package]]
-name = "regex-syntax"
-version = "0.7.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
-
-[[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustc_version"
@@ -859,29 +945,35 @@
 name = "serde_derive"
 version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "simd-adler32"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "238abfbb77c1915110ad968465608b68e869e0772622c9656714e73e5a1a522f"
+
+[[package]]
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
 
 [[package]]
 name = "smallvec"
@@ -910,17 +1002,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.16"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6f671d4b5ffdb8eadec19c0ae67fe2639df8684bd7bc4b83d986b8db549cf01"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -959,22 +1051,33 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.18",
+]
+
+[[package]]
+name = "tiff"
+version = "0.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7449334f9ff2baf290d55d73983a7d6fa15e01198faef72af07e2a8db851e471"
+dependencies = [
+ "flate2",
+ "jpeg-decoder",
+ "weezl",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unicode-width"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
 
@@ -1013,15 +1116,15 @@
 checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1035,26 +1138,32 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.16",
+ "syn 2.0.18",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
 
 [[package]]
+name = "weezl"
+version = "0.1.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9193164d4de03a926d909d3bc7c30543cecb35400c02114792c2cae20d5e2dbb"
+
+[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
```

### Comparing `getdaft-0.1.3/PKG-INFO` & `getdaft-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: getdaft
-Version: 0.1.3
+Version: 0.1.4
 Requires-Dist: pyarrow >= 6.0.1
 Requires-Dist: fsspec[http]
 Requires-Dist: loguru
 Requires-Dist: tabulate >= 0.9.0
 Requires-Dist: psutil
 Requires-Dist: typing-extensions >= 4.0.0; python_version < '3.8'
 Requires-Dist: pickle5 >= 0.0.12; python_version < '3.8'
-Requires-Dist: ray[data, default]>=2.0.0; extra == 'ray'
-Requires-Dist: packaging; extra == 'ray'
-Requires-Dist: getdaft[aws, ray, pandas, numpy, viz]; extra == 'all'
 Requires-Dist: pydot; extra == 'viz'
+Requires-Dist: s3fs; extra == 'aws'
+Requires-Dist: getdaft[aws, ray, pandas, numpy, viz]; extra == 'all'
 Requires-Dist: numpy; extra == 'numpy'
 Requires-Dist: pandas; extra == 'pandas'
-Requires-Dist: s3fs; extra == 'aws'
-Provides-Extra: ray
-Provides-Extra: all
+Requires-Dist: ray[data, default]>=2.0.0; extra == 'ray'
+Requires-Dist: packaging; extra == 'ray'
 Provides-Extra: viz
+Provides-Extra: aws
+Provides-Extra: all
 Provides-Extra: numpy
 Provides-Extra: pandas
-Provides-Extra: aws
+Provides-Extra: ray
 License-File: LICENSE
 Summary: A Distributed DataFrame library for large scale complex data processing.
 Author-email: Eventual Inc <daft@eventualcomputing.com>
 Maintainer-email: Sammy Sidhu <sammy@eventualcomputing.com>, Jay Chia <jay@eventualcomputing.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
-Project-URL: homepage, https://www.getdaft.io
 Project-URL: repository, https://github.com/Eventual-Inc/Daft
+Project-URL: homepage, https://www.getdaft.io
 
 |Banner|
 
 |CI| |PyPI| |Latest Tag| |Coverage| |Slack|
 
 `Website <https://www.getdaft.io>`_ • `Docs <https://www.getdaft.io/projects/docs/>`_ • `Installation`_ • `10-minute tour of Daft <https://www.getdaft.io/projects/docs/en/latest/learn/10-min.html>`_ • `Community and Support <https://github.com/Eventual-Inc/Daft/discussions>`_
```

