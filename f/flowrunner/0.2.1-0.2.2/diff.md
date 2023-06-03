# Comparing `tmp/flowrunner-0.2.1.tar.gz` & `tmp/flowrunner-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowrunner-0.2.1.tar", last modified: Sun Apr  2 08:16:58 2023, max compression
+gzip compressed data, was "flowrunner-0.2.2.tar", last modified: Sat Jun  3 12:58:38 2023, max compression
```

## Comparing `flowrunner-0.2.1.tar` & `flowrunner-0.2.2.tar`

### file list

```diff
@@ -1,97 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:58.765656 flowrunner-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:58.749656 flowrunner-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:58.749656 flowrunner-0.2.1/.github/issue_template/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-02 08:16:41.000000 flowrunner-0.2.1/.github/issue_template/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-02 08:16:41.000000 flowrunner-0.2.1/.github/issue_template/documentation_improvement.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-02 08:16:41.000000 flowrunner-0.2.1/.github/issue_template/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-02 08:16:41.000000 flowrunner-0.2.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:58.749656 flowrunner-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-02 08:16:41.000000 flowrunner-0.2.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-02 08:16:41.000000 flowrunner-0.2.1/.github/workflows/code_scan.yml
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-02 08:16:41.000000 flowrunner-0.2.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-02 08:16:41.000000 flowrunner-0.2.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-02 08:16:41.000000 flowrunner-0.2.1/.github/workflows/release_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-02 08:16:41.000000 flowrunner-0.2.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-04-02 08:16:41.000000 flowrunner-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-02 08:16:41.000000 flowrunner-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-02 08:16:41.000000 flowrunner-0.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-02 08:16:41.000000 flowrunner-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-02 08:16:41.000000 flowrunner-0.2.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-04-02 08:16:58.765656 flowrunner-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-02 08:16:41.000000 flowrunner-0.2.1/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:58.749656 flowrunner-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:58.753656 flowrunner-0.2.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:58.757656 flowrunner-0.2.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   955116 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/source/_static/flowrunner_databricks_example.html
--rw-r--r--   0 runner    (1001) docker     (123)   601383 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/source/_static/flowrunner_pandas_notebook_example.html
--rw-r--r--   0 runner    (1001) docker     (123)   607135 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/source/_static/flowrunner_pyspark_example.html
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/source/api_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/source/contributing_guide_code.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/source/contributing_guide_docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/source/creating_your_development_environment.rst
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/source/docutils.conf
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/source/flowrunner.core.rst
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/source/flowrunner.core.templates.rst
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/source/flowrunner.rst
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/source/flowrunner.runner.rst
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/source/flowrunner.system.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/source/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/source/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/source/notebook_examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/source/pandas_example.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-04-02 08:16:41.000000 flowrunner-0.2.1/docs/source/pyspark_example.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:58.757656 flowrunner-0.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-02 08:16:41.000000 flowrunner-0.2.1/examples/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-02 08:16:41.000000 flowrunner-0.2.1/examples/pandas_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-02 08:16:41.000000 flowrunner-0.2.1/examples/pyspark_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:58.757656 flowrunner-0.2.1/flowrunner/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-02 08:16:41.000000 flowrunner-0.2.1/flowrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-02 08:16:41.000000 flowrunner-0.2.1/flowrunner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-04-02 08:16:41.000000 flowrunner-0.2.1/flowrunner/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:58.761656 flowrunner-0.2.1/flowrunner/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:41.000000 flowrunner-0.2.1/flowrunner/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-04-02 08:16:41.000000 flowrunner-0.2.1/flowrunner/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-02 08:16:41.000000 flowrunner-0.2.1/flowrunner/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14889 2023-04-02 08:16:41.000000 flowrunner-0.2.1/flowrunner/core/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:58.761656 flowrunner-0.2.1/flowrunner/core/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:41.000000 flowrunner-0.2.1/flowrunner/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-02 08:16:41.000000 flowrunner-0.2.1/flowrunner/core/templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:58.761656 flowrunner-0.2.1/flowrunner/runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:41.000000 flowrunner-0.2.1/flowrunner/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-04-02 08:16:41.000000 flowrunner-0.2.1/flowrunner/runner/flow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:58.761656 flowrunner-0.2.1/flowrunner/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:41.000000 flowrunner-0.2.1/flowrunner/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-02 08:16:41.000000 flowrunner-0.2.1/flowrunner/system/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-02 08:16:41.000000 flowrunner-0.2.1/flowrunner/system/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:58.761656 flowrunner-0.2.1/flowrunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-04-02 08:16:58.000000 flowrunner-0.2.1/flowrunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-02 08:16:58.000000 flowrunner-0.2.1/flowrunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 08:16:58.000000 flowrunner-0.2.1/flowrunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-02 08:16:58.000000 flowrunner-0.2.1/flowrunner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-02 08:16:58.000000 flowrunner-0.2.1/flowrunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-02 08:16:58.000000 flowrunner-0.2.1/flowrunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-04-02 08:16:41.000000 flowrunner-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-04-02 08:16:41.000000 flowrunner-0.2.1/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 08:16:58.765656 flowrunner-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-02 08:16:41.000000 flowrunner-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:58.761656 flowrunner-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:41.000000 flowrunner-0.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:58.761656 flowrunner-0.2.1/tests/test_flowrunner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:41.000000 flowrunner-0.2.1/tests/test_flowrunner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:58.765656 flowrunner-0.2.1/tests/test_flowrunner/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:41.000000 flowrunner-0.2.1/tests/test_flowrunner/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-02 08:16:41.000000 flowrunner-0.2.1/tests/test_flowrunner/core/examplepandas.html
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-04-02 08:16:41.000000 flowrunner-0.2.1/tests/test_flowrunner/core/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-02 08:16:41.000000 flowrunner-0.2.1/tests/test_flowrunner/core/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-04-02 08:16:41.000000 flowrunner-0.2.1/tests/test_flowrunner/core/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:58.765656 flowrunner-0.2.1/tests/test_flowrunner/runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:41.000000 flowrunner-0.2.1/tests/test_flowrunner/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-02 08:16:41.000000 flowrunner-0.2.1/tests/test_flowrunner/runner/test_flow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:58.765656 flowrunner-0.2.1/tests/test_flowrunner/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 08:16:41.000000 flowrunner-0.2.1/tests/test_flowrunner/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-02 08:16:41.000000 flowrunner-0.2.1/tests/test_flowrunner/system/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-02 08:16:41.000000 flowrunner-0.2.1/tests/test_flowrunner/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.387430 flowrunner-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.375429 flowrunner-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.375429 flowrunner-0.2.2/.github/issue_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.github/issue_template/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.github/issue_template/documentation_improvement.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.github/issue_template/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.375429 flowrunner-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.github/workflows/code_scan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.github/workflows/release_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-03 12:58:27.000000 flowrunner-0.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-03 12:58:27.000000 flowrunner-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-03 12:58:27.000000 flowrunner-0.2.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-06-03 12:58:38.387430 flowrunner-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-03 12:58:27.000000 flowrunner-0.2.2/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.375429 flowrunner-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.379429 flowrunner-0.2.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.379429 flowrunner-0.2.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   955116 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/_static/flowrunner_databricks_example.html
+-rw-r--r--   0 runner    (1001) docker     (123)   601383 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/_static/flowrunner_pandas_notebook_example.html
+-rw-r--r--   0 runner    (1001) docker     (123)   607135 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/_static/flowrunner_pyspark_example.html
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/contributing_guide_code.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/contributing_guide_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/creating_flowrunner_projects.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/creating_your_development_environment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/docutils.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/flowrunner.core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/flowrunner.core.templates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/flowrunner.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/flowrunner.runner.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/flowrunner.system.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/notebook_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/pandas_example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-03 12:58:27.000000 flowrunner-0.2.2/docs/source/pyspark_example.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.379429 flowrunner-0.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-03 12:58:27.000000 flowrunner-0.2.2/examples/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-03 12:58:27.000000 flowrunner-0.2.2/examples/pandas_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-03 12:58:27.000000 flowrunner-0.2.2/examples/pyspark_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/flowrunner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/flowrunner/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14889 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/core/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/flowrunner/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/core/templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/flowrunner/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9622 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/runner/flow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/flowrunner/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/system/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-03 12:58:27.000000 flowrunner-0.2.2/flowrunner/system/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/flowrunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-06-03 12:58:38.000000 flowrunner-0.2.2/flowrunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-03 12:58:38.000000 flowrunner-0.2.2/flowrunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 12:58:38.000000 flowrunner-0.2.2/flowrunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-03 12:58:38.000000 flowrunner-0.2.2/flowrunner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-03 12:58:38.000000 flowrunner-0.2.2/flowrunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-03 12:58:38.000000 flowrunner-0.2.2/flowrunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-03 12:58:27.000000 flowrunner-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-06-03 12:58:27.000000 flowrunner-0.2.2/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 12:58:38.387430 flowrunner-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-03 12:58:27.000000 flowrunner-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-03 12:58:27.000000 flowrunner-0.2.2/templates/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/
+-rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-06-03 12:58:27.000000 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-03 12:58:27.000000 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-03 12:58:27.000000 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-03 12:58:27.000000 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-03 12:58:27.000000 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.371429 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/html_dags/
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-03 12:58:27.000000 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/html_dags/dagsexamplepandas.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/my_flows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:27.000000 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/my_flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-03 12:58:27.000000 flowrunner-0.2.2/templates/{{ cookiecutter.project_name }}/{{ cookiecutter.project_slug }}/my_flows/pandas_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.383430 flowrunner-0.2.2/tests/test_flowrunner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.387430 flowrunner-0.2.2/tests/test_flowrunner/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/core/examplepandas.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/core/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/core/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/core/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.387430 flowrunner-0.2.2/tests/test_flowrunner/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/runner/test_flow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.387430 flowrunner-0.2.2/tests/test_flowrunner/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/system/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_flowrunner/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 12:58:38.387430 flowrunner-0.2.2/tests/test_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-03 12:58:27.000000 flowrunner-0.2.2/tests/test_templates/test_cookiecutter.py
```

### Comparing `flowrunner-0.2.1/.github/issue_template/bug_report.md` & `flowrunner-0.2.2/.github/issue_template/bug_report.md`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/.github/issue_template/feature_request.md` & `flowrunner-0.2.2/.github/issue_template/feature_request.md`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/.github/workflows/build.yml` & `flowrunner-0.2.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/.github/workflows/code_scan.yml` & `flowrunner-0.2.2/.github/workflows/code_scan.yml`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/.github/workflows/docs.yml` & `flowrunner-0.2.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/.github/workflows/release.yml` & `flowrunner-0.2.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/.github/workflows/release_test.yml` & `flowrunner-0.2.2/.github/workflows/release_test.yml`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/.github/workflows/tests.yml` & `flowrunner-0.2.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/.gitignore` & `flowrunner-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/.pre-commit-config.yaml` & `flowrunner-0.2.2/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
-exclude: '^docs/source/_static/' # the databricks notebook is larger but required, compression did not work
-
+exclude:
+    '[^docs/source/_static/]' # the databricks notebook is larger but required, compression did not work, and templates because that makes an issue for cookic
 
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v3.2.0
     hooks:
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
```

### Comparing `flowrunner-0.2.1/.readthedocs.yaml` & `flowrunner-0.2.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/LICENSE` & `flowrunner-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/Makefile` & `flowrunner-0.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/PKG-INFO` & `flowrunner-0.2.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowrunner
-Version: 0.2.1
+Version: 0.2.2
 Summary: Flowrunner is a lightweight package to organize and represent Data Engineering/Science workflows
 Author-email: Prithvijit Guha <prithvijit_guha2@hotmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Prithvijit
         All rights reserved.
         
@@ -85,15 +85,14 @@
 ```
 
 Or install from source
 ```sh
 pip install git+https://github.com/prithvijitguha/flowrunner@main
 ```
 
-
 ## Usage
 
 Here is a quick example to run as is
 
 ```python
 # example.py
 from flowrunner import BaseFlow, step, start, end
@@ -266,14 +265,103 @@
 
 Now when you run `ExamplePandas().display()` you get the following output
 
 
 ![image](https://user-images.githubusercontent.com/71138854/227732600-7bae5e21-3c9a-4ad9-85da-f926cded2636.png)
 
 
+## PySpark Example
+
+```python
+
+# -*- coding: utf-8 -*-
+from pyspark.sql import SparkSession
+from pyspark.sql.functions import lit
+
+from flowrunner import BaseFlow, end, start, step
+
+spark = SparkSession.builder.getOrCreate()
+
+
+class ExamplePySpark(BaseFlow):
+    @start
+    @step(next=["transformation_function_1", "transformation_function_2"])
+    def create_data(self):
+        """
+        This is an example where we use the Spark engine instead of Pandas
+
+        This method we create the dataset we are going use. In real use cases,
+        you'll have to read from a source (csv, parquet, etc)
+
+        For this example we create two dataframes for students ranked by marked scored
+        for when they attempted the example on 1st January 2023 and 12th March 2023
+
+        After creating the dataset we pass it to the next methods
+
+        - transformation_function_1
+        - transformation_function_2
+        """
+
+        data1 = [
+            ("Hermione",100),
+            ("Harry", 85),
+            ("Ron", 75),
+        ]
+
+        data2 =  [
+            ("Hermione",100),
+            ("Harry", 90),
+            ("Ron", 80),
+        ]
+
+        columns = ["Name", "marks"]
+
+        rdd1 = spark.sparkContext.parallelize(data1)
+        rdd2 = spark.sparkContext.parallelize(data2)
+        self.df1 = spark.createDataFrame(rdd1).toDF(*columns)
+        self.df2 = spark.createDataFrame(rdd2).toDF(*columns)
+
+    @step(next=["append_data"])
+    def transformation_function_1(self):
+        """
+        Here we add a snapshot_date to the input dataframe of 2023-03-12
+        """
+
+        self.transformed_df_1 = self.df1.withColumn("snapshot_date", lit("2023-03-12"))
+
+    @step(next=["append_data"])
+    def transformation_function_2(self):
+        """
+        Here we add a snapshot_date to the input dataframe of 2023-01-01
+        """
+        self.transformed_df_2 = self.df2.withColumn("snapshot_date", lit("2023-01-01"))
+
+    @step(next=["show_data"])
+    def append_data(self):
+        """
+        Here we append the two dataframe together
+        """
+        self.final_df = self.transformed_df_1.union(self.transformed_df_2)
+
+    @end
+    @step
+    def show_data(self):
+        """
+        Here we show the new final dataframe of aggregated data. However in real use cases. It would
+        be more likely to write the data to some final layer/format
+        """
+        self.final_df.show()
+        return self.final_df
+
+```
+
+Now when you run `ExamplePySpark().display()` you get the following output
+
+![image](https://user-images.githubusercontent.com/71138854/230785408-38e476b2-f58b-4150-b315-ea958fd73359.png)
+
 ## Documentation
 Check out the latest documentation here: [FlowRunner documentation](https://flowrunner.readthedocs.io/en/latest/)
 
 ## Contributing
 All contributions are welcome :smiley:
 
 If you are interested in contributing, please check out this page: [FlowRunner Contribution Page](https://flowrunner.readthedocs.io/en/latest/contributing_guide_code.html)
```

### Comparing `flowrunner-0.2.1/changelog.md` & `flowrunner-0.2.2/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,7 +34,17 @@
 - Support for PySpark `pip install flowrunner[pyspark]`
 - Improved validation for stranded middle origin nodes
 
 ### Documentation:
 - Changed theme to sphinx_the_docs
 - Added API reference documentation
 - Improved documentation examples with Databricks and PySpark
+
+
+## 0.2.2 (2023-06-03)
+
+### Features:
+- Add cookie cutter template
+- Improved logging
+
+### Documentation:
+- Fixed broken notebook example links
```

### Comparing `flowrunner-0.2.1/docs/Makefile` & `flowrunner-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/docs/make.bat` & `flowrunner-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/docs/source/_static/flowrunner_databricks_example.html` & `flowrunner-0.2.2/docs/source/_static/flowrunner_databricks_example.html`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/docs/source/_static/flowrunner_pandas_notebook_example.html` & `flowrunner-0.2.2/docs/source/_static/flowrunner_pandas_notebook_example.html`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/docs/source/_static/flowrunner_pyspark_example.html` & `flowrunner-0.2.2/docs/source/_static/flowrunner_pyspark_example.html`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/docs/source/conf.py` & `flowrunner-0.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/docs/source/contributing_guide_code.rst` & `flowrunner-0.2.2/docs/source/contributing_guide_code.rst`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/docs/source/contributing_guide_docs.rst` & `flowrunner-0.2.2/docs/source/contributing_guide_docs.rst`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/docs/source/creating_your_development_environment.rst` & `flowrunner-0.2.2/docs/source/creating_your_development_environment.rst`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/docs/source/flowrunner.core.rst` & `flowrunner-0.2.2/docs/source/flowrunner.core.rst`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/docs/source/flowrunner.system.rst` & `flowrunner-0.2.2/docs/source/flowrunner.system.rst`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/docs/source/getting_started.rst` & `flowrunner-0.2.2/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/docs/source/introduction.rst` & `flowrunner-0.2.2/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/docs/source/notebook_examples.rst` & `flowrunner-0.2.2/docs/source/notebook_examples.rst`

 * *Files 13% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 ===================
 
 Flowrunner works in notebooks as well!
 
 Jupyter Notebook Example
 ------------------------
 
-`Jupyter notebook <../html/_static/flowrunner_pandas_notebook_example.html>`_
+`Jupyter notebook <_static/flowrunner_pandas_notebook_example.html>`_
 
 
 PySpark Example:
 ----------------------
 Flowrunner can be used with PySpark
 
-`PySpark notebook <../html/_static/flowrunner_pyspark_example.html>`_
+`PySpark notebook <_static/flowrunner_pyspark_example.html>`_
 
 
 
 Databricks Notebook
 ----------------------
 Flowrunner can be used inside Databricks on DBR 10.4 and above, below is the link to the example notebook.
 
-`Databricks notebook <../html/_static/flowrunner_databricks_example.html>`_
+`Databricks notebook <_static/flowrunner_databricks_example.html>`_
```

### Comparing `flowrunner-0.2.1/docs/source/pandas_example.rst` & `flowrunner-0.2.2/docs/source/pandas_example.rst`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/docs/source/pyspark_example.rst` & `flowrunner-0.2.2/docs/source/pyspark_example.rst`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/examples/example.py` & `flowrunner-0.2.2/examples/example.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/examples/pandas_example.py` & `flowrunner-0.2.2/examples/pandas_example.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/examples/pyspark_example.py` & `flowrunner-0.2.2/examples/pyspark_example.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/flowrunner/__init__.py` & `flowrunner-0.2.2/flowrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/flowrunner/cli.py` & `flowrunner-0.2.2/flowrunner/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 Options:
   --help  Show this message and exit.
 
 Commands:
   run       Command to run a Flow
   show      Command to show the order of iteration of a Flow
   validate  Command to validate a Flow
-
-
+  directory Command to visualize a directory
 """
 import inspect
+import os
 from pydoc import importfile
 
 import click
 
 from flowrunner import BaseFlow
 from flowrunner.system.logger import logger
 
@@ -146,17 +146,54 @@
         python -m flowrunner display /my_path/to/flow_file.py
 
     Args:
         path: A string value of path to save flow in. Defaults to current directory
         description: Optional argument for descriptive or non descriptive dag, default is descriptive
 
     Returns:
-        Runs the Flow
+        Displays the flows
     """
+    # if we pass only a single filepath as input then we visualize that filepath
     flow_list = _read_python_file(filepath)
     for flow_class in flow_list:
         logger.info("Creating Flow DAG for flow %s", flow_class.__name__)
         flow_class().dag(save_file=True, path=path, description=description) # we keep save file as True, assumption being if we are running through cli then we are going to save
 
 
+
+
+@cli.command()
+@click.option("--path")
+@click.option("--description", default=True)
+@click.argument("directory")
+def display_dir(directory: str, path: str = None, description:bool = True):
+    """Command to visualize a directory of Flows as Directed Acyclical Graph
+
+    Examples:
+        python -m flowrunner display_dir /my_path/to/flow_file.py
+
+    Args:
+        path: A string value of path to save flow in. Defaults to current directory
+        description: Optional argument for descriptive or non descriptive dag, default is descriptive
+        directory: A string value of directory to check for flows
+
+    Returns:
+        Displays the flows
+    """
+    flow_list = [] # list of flows to store all files
+    # then we susbtitute that value as filepath
+    for filepath in os.listdir(directory):
+        # check if the file is python file otherwise ignore otherwise
+        # sometimes other files can get in the way and cause errors
+        if filepath.endswith(".py"):
+            flow_list = _read_python_file(os.path.join(directory, filepath))
+            for flow_class in flow_list:
+                logger.info("Creating Flow DAG for flow %s", flow_class.__name__)
+                flow_class().dag(save_file=True, path=path, description=description) # we keep save file as True, assumption being if we are running through cli then we are going to save
+
+
+
+
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `flowrunner-0.2.1/flowrunner/core/base.py` & `flowrunner-0.2.2/flowrunner/core/base.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/flowrunner/core/decorators.py` & `flowrunner-0.2.2/flowrunner/core/decorators.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/flowrunner/core/helpers.py` & `flowrunner-0.2.2/flowrunner/core/helpers.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/flowrunner/core/templates/base.html` & `flowrunner-0.2.2/flowrunner/core/templates/base.html`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/flowrunner/runner/flow.py` & `flowrunner-0.2.2/flowrunner/runner/flow.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/flowrunner.egg-info/PKG-INFO` & `flowrunner-0.2.2/flowrunner.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowrunner
-Version: 0.2.1
+Version: 0.2.2
 Summary: Flowrunner is a lightweight package to organize and represent Data Engineering/Science workflows
 Author-email: Prithvijit Guha <prithvijit_guha2@hotmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Prithvijit
         All rights reserved.
         
@@ -85,15 +85,14 @@
 ```
 
 Or install from source
 ```sh
 pip install git+https://github.com/prithvijitguha/flowrunner@main
 ```
 
-
 ## Usage
 
 Here is a quick example to run as is
 
 ```python
 # example.py
 from flowrunner import BaseFlow, step, start, end
@@ -266,14 +265,103 @@
 
 Now when you run `ExamplePandas().display()` you get the following output
 
 
 ![image](https://user-images.githubusercontent.com/71138854/227732600-7bae5e21-3c9a-4ad9-85da-f926cded2636.png)
 
 
+## PySpark Example
+
+```python
+
+# -*- coding: utf-8 -*-
+from pyspark.sql import SparkSession
+from pyspark.sql.functions import lit
+
+from flowrunner import BaseFlow, end, start, step
+
+spark = SparkSession.builder.getOrCreate()
+
+
+class ExamplePySpark(BaseFlow):
+    @start
+    @step(next=["transformation_function_1", "transformation_function_2"])
+    def create_data(self):
+        """
+        This is an example where we use the Spark engine instead of Pandas
+
+        This method we create the dataset we are going use. In real use cases,
+        you'll have to read from a source (csv, parquet, etc)
+
+        For this example we create two dataframes for students ranked by marked scored
+        for when they attempted the example on 1st January 2023 and 12th March 2023
+
+        After creating the dataset we pass it to the next methods
+
+        - transformation_function_1
+        - transformation_function_2
+        """
+
+        data1 = [
+            ("Hermione",100),
+            ("Harry", 85),
+            ("Ron", 75),
+        ]
+
+        data2 =  [
+            ("Hermione",100),
+            ("Harry", 90),
+            ("Ron", 80),
+        ]
+
+        columns = ["Name", "marks"]
+
+        rdd1 = spark.sparkContext.parallelize(data1)
+        rdd2 = spark.sparkContext.parallelize(data2)
+        self.df1 = spark.createDataFrame(rdd1).toDF(*columns)
+        self.df2 = spark.createDataFrame(rdd2).toDF(*columns)
+
+    @step(next=["append_data"])
+    def transformation_function_1(self):
+        """
+        Here we add a snapshot_date to the input dataframe of 2023-03-12
+        """
+
+        self.transformed_df_1 = self.df1.withColumn("snapshot_date", lit("2023-03-12"))
+
+    @step(next=["append_data"])
+    def transformation_function_2(self):
+        """
+        Here we add a snapshot_date to the input dataframe of 2023-01-01
+        """
+        self.transformed_df_2 = self.df2.withColumn("snapshot_date", lit("2023-01-01"))
+
+    @step(next=["show_data"])
+    def append_data(self):
+        """
+        Here we append the two dataframe together
+        """
+        self.final_df = self.transformed_df_1.union(self.transformed_df_2)
+
+    @end
+    @step
+    def show_data(self):
+        """
+        Here we show the new final dataframe of aggregated data. However in real use cases. It would
+        be more likely to write the data to some final layer/format
+        """
+        self.final_df.show()
+        return self.final_df
+
+```
+
+Now when you run `ExamplePySpark().display()` you get the following output
+
+![image](https://user-images.githubusercontent.com/71138854/230785408-38e476b2-f58b-4150-b315-ea958fd73359.png)
+
 ## Documentation
 Check out the latest documentation here: [FlowRunner documentation](https://flowrunner.readthedocs.io/en/latest/)
 
 ## Contributing
 All contributions are welcome :smiley:
 
 If you are interested in contributing, please check out this page: [FlowRunner Contribution Page](https://flowrunner.readthedocs.io/en/latest/contributing_guide_code.html)
```

### Comparing `flowrunner-0.2.1/flowrunner.egg-info/requires.txt` & `flowrunner-0.2.2/flowrunner.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 requests
 click>=8.1.3
 Jinja2>=3.1.2
 coloredlogs>=15.0.1
 ipython>=8.11.0
 matplotlib>=3.7.1
+cookiecutter>=2.1.1
 
 [:python_version <= "3.8"]
 importlib-metadata
 
 [dev]
 click>=8.1.3
 Jinja2>=3.1.2
 pylint>=2.16.4
 black>=23.1.0
 coverage<=7.2.1
 pytest>=7.2.1
+pytest-cookies>=0.7.0
 isort>=5.12.0
 pre-commit>=3.1.1
 pandas>=1.5.3
 ipython>=8.11.0
 matplotlib>=3.7.1
 pylint>=2.17.0
-coloredlogs>=15.0.1
 pyspark>=3.3.2
+cookiecutter>=2.1.1
+colorama<=0.4.6
 
 [doc]
 click>=8.1.3
 Jinja2>=3.1.2
 Sphinx>=6.1.3
 sphinxcontrib-mermaid>=0.8.1
 sphinx-autoapi>=2.0.1
@@ -35,29 +38,31 @@
 sphinx-rtd-theme>=1.2.0
 isort>=5.12.0
 black>=23.1.0
 pre-commit>=3.1.1
 coverage<=7.2.1
 pytest>=7.2.1
 pylint>=2.17.0
-coloredlogs>=15.0.1
+colorama<=0.4.6
 
 [pandas]
 pandas>=1.5.3
 
 [pyspark]
 pyspark>=3.3.2
 
 [test]
 click>=8.1.3
 Jinja2>=3.1.2
 pytest>=7.2.1
+pytest-cookies>=0.7.0
 black>=23.1.0
 coverage<=7.2.1
 isort>=5.12.0
 pre-commit>=3.1.1
 pandas>=1.5.3
 ipython>=8.11.0
 matplotlib>=3.7.1
 pylint>=2.17.0
-coloredlogs>=15.0.1
 pyspark>=3.3.2
+cookiecutter>=2.1.1
+colorama<=0.4.6
```

### Comparing `flowrunner-0.2.1/pyproject.toml` & `flowrunner-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [project]
 name = "flowrunner"
 authors = [
     {name = "Prithvijit Guha", email = "prithvijit_guha2@hotmail.com"},
 ]
 
-version = "0.2.1"
+version = "0.2.2"
 
 
 description = "Flowrunner is a lightweight package to organize and represent Data Engineering/Science workflows"
 readme = "readme.md"
 requires-python = ">=3.8"
 keywords = ["Data Engineering", "Data Science"]
 license = {file = "LICENSE"}
@@ -26,15 +26,16 @@
 dependencies = [
     'requests',
     'importlib-metadata; python_version<="3.8"',
     'click>=8.1.3',
     'Jinja2>=3.1.2',
     'coloredlogs>=15.0.1',
     'ipython>=8.11.0',
-    'matplotlib>=3.7.1'
+    'matplotlib>=3.7.1',
+    'cookiecutter>=2.1.1'
 ]
 
 
 
 
 [project.urls]
 Homepage = "https://github.com/prithvijitguha/flowrunner"
@@ -56,47 +57,51 @@
     "sphinx-rtd-theme>=1.2.0",
     "isort>=5.12.0",
     "black>=23.1.0",
     "pre-commit>=3.1.1",
     "coverage<=7.2.1",
     "pytest>=7.2.1",
     "pylint>=2.17.0",
-    "coloredlogs>=15.0.1"
+    "colorama<=0.4.6"
 ]
 
 dev = [
     "click>=8.1.3",
     "Jinja2>=3.1.2",
     "pylint>=2.16.4",
     "black>=23.1.0",
     "coverage<=7.2.1",
     "pytest>=7.2.1",
+    "pytest-cookies>=0.7.0",
     "isort>=5.12.0",
     "pre-commit>=3.1.1",
     "pandas>=1.5.3",
     "ipython>=8.11.0",
     "matplotlib>=3.7.1",
     "pylint>=2.17.0",
-    "coloredlogs>=15.0.1",
-    "pyspark>=3.3.2"
+    "pyspark>=3.3.2",
+    "cookiecutter>=2.1.1",
+    "colorama<=0.4.6"
 ]
 test = [
     "click>=8.1.3",
     "Jinja2>=3.1.2",
     "pytest>=7.2.1",
+    "pytest-cookies>=0.7.0",
     "black>=23.1.0",
     "coverage<=7.2.1",
     "isort>=5.12.0",
     "pre-commit>=3.1.1",
     "pandas>=1.5.3",
     "ipython>=8.11.0",
     "matplotlib>=3.7.1",
     "pylint>=2.17.0",
-    "coloredlogs>=15.0.1",
-    "pyspark>=3.3.2"
+    "pyspark>=3.3.2",
+    "cookiecutter>=2.1.1",
+    "colorama<=0.4.6"
 ]
 pandas = [
     "pandas>=1.5.3"
 ]
 
 pyspark = [
     "pyspark>=3.3.2"
@@ -114,17 +119,21 @@
     "flowrunner"
 ]
 
 
 [project.scripts]
 cli = "flowrunner.cli:cli"
 
+[tool.setuptools]
+py-modules = ["flowrunner"]
+
 [tool.pytest.ini_options]
 pythonpath = [
     "flowrunner",
+    "templates",
     "tests"
     ]
 testpaths = [
     "tests"
 ]
 addopts = [
     "--cache-clear",
@@ -152,15 +161,16 @@
 ignore-paths = [
     # we skip lintingcheck for docs and examples
     "^examples/.*$",
     "^docs/source/.*$",
 ]
 ignored-modules=[
     "pandas",
-    "pytest"
+    "pytest",
+    "flowrunner"
 ]
 
 
 [tool.pylint.format]
 max-line-length=145
```

### Comparing `flowrunner-0.2.1/readme.md` & `flowrunner-0.2.2/readme.md`

 * *Files 15% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 ```
 
 Or install from source
 ```sh
 pip install git+https://github.com/prithvijitguha/flowrunner@main
 ```
 
-
 ## Usage
 
 Here is a quick example to run as is
 
 ```python
 # example.py
 from flowrunner import BaseFlow, step, start, end
@@ -214,14 +213,103 @@
 
 Now when you run `ExamplePandas().display()` you get the following output
 
 
 ![image](https://user-images.githubusercontent.com/71138854/227732600-7bae5e21-3c9a-4ad9-85da-f926cded2636.png)
 
 
+## PySpark Example
+
+```python
+
+# -*- coding: utf-8 -*-
+from pyspark.sql import SparkSession
+from pyspark.sql.functions import lit
+
+from flowrunner import BaseFlow, end, start, step
+
+spark = SparkSession.builder.getOrCreate()
+
+
+class ExamplePySpark(BaseFlow):
+    @start
+    @step(next=["transformation_function_1", "transformation_function_2"])
+    def create_data(self):
+        """
+        This is an example where we use the Spark engine instead of Pandas
+
+        This method we create the dataset we are going use. In real use cases,
+        you'll have to read from a source (csv, parquet, etc)
+
+        For this example we create two dataframes for students ranked by marked scored
+        for when they attempted the example on 1st January 2023 and 12th March 2023
+
+        After creating the dataset we pass it to the next methods
+
+        - transformation_function_1
+        - transformation_function_2
+        """
+
+        data1 = [
+            ("Hermione",100),
+            ("Harry", 85),
+            ("Ron", 75),
+        ]
+
+        data2 =  [
+            ("Hermione",100),
+            ("Harry", 90),
+            ("Ron", 80),
+        ]
+
+        columns = ["Name", "marks"]
+
+        rdd1 = spark.sparkContext.parallelize(data1)
+        rdd2 = spark.sparkContext.parallelize(data2)
+        self.df1 = spark.createDataFrame(rdd1).toDF(*columns)
+        self.df2 = spark.createDataFrame(rdd2).toDF(*columns)
+
+    @step(next=["append_data"])
+    def transformation_function_1(self):
+        """
+        Here we add a snapshot_date to the input dataframe of 2023-03-12
+        """
+
+        self.transformed_df_1 = self.df1.withColumn("snapshot_date", lit("2023-03-12"))
+
+    @step(next=["append_data"])
+    def transformation_function_2(self):
+        """
+        Here we add a snapshot_date to the input dataframe of 2023-01-01
+        """
+        self.transformed_df_2 = self.df2.withColumn("snapshot_date", lit("2023-01-01"))
+
+    @step(next=["show_data"])
+    def append_data(self):
+        """
+        Here we append the two dataframe together
+        """
+        self.final_df = self.transformed_df_1.union(self.transformed_df_2)
+
+    @end
+    @step
+    def show_data(self):
+        """
+        Here we show the new final dataframe of aggregated data. However in real use cases. It would
+        be more likely to write the data to some final layer/format
+        """
+        self.final_df.show()
+        return self.final_df
+
+```
+
+Now when you run `ExamplePySpark().display()` you get the following output
+
+![image](https://user-images.githubusercontent.com/71138854/230785408-38e476b2-f58b-4150-b315-ea958fd73359.png)
+
 ## Documentation
 Check out the latest documentation here: [FlowRunner documentation](https://flowrunner.readthedocs.io/en/latest/)
 
 ## Contributing
 All contributions are welcome :smiley:
 
 If you are interested in contributing, please check out this page: [FlowRunner Contribution Page](https://flowrunner.readthedocs.io/en/latest/contributing_guide_code.html)
```

### Comparing `flowrunner-0.2.1/tests/test_flowrunner/core/examplepandas.html` & `flowrunner-0.2.2/tests/test_flowrunner/core/examplepandas.html`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/tests/test_flowrunner/core/test_base.py` & `flowrunner-0.2.2/tests/test_flowrunner/core/test_base.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/tests/test_flowrunner/core/test_decorators.py` & `flowrunner-0.2.2/tests/test_flowrunner/core/test_decorators.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/tests/test_flowrunner/core/test_helpers.py` & `flowrunner-0.2.2/tests/test_flowrunner/core/test_helpers.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/tests/test_flowrunner/runner/test_flow.py` & `flowrunner-0.2.2/tests/test_flowrunner/runner/test_flow.py`

 * *Files identical despite different names*

### Comparing `flowrunner-0.2.1/tests/test_flowrunner/system/test_logger.py` & `flowrunner-0.2.2/tests/test_flowrunner/system/test_logger.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 def test_logger_output(fixture_logger, caplog):
     fixture_logger.info("hello world info")
     fixture_logger.warning("hello world warn")
     fixture_logger.debug("hello world debug")
     fixture_logger.error("hello world error")
     pytest.approx(
         caplog.records[0].msg,
-        "INFO     hello world info  flowrunner.system.logger:test_logger.py:13",
+        "INFO | hello world info | flowrunner.system.logger:test_logger.py:13",
     )
     pytest.approx(
         caplog.records[1].msg,
-        "WARNING  hello world warn  flowrunner.system.logger:test_logger.py:14",
+        "WARNING | hello world warn | flowrunner.system.logger:test_logger.py:14",
     )
     pytest.approx(
         caplog.records[2].msg,
-        "DEBUG    hello world debug  flowrunner.system.logger:test_logger.py:15",
+        "DEBUG | hello world debug | flowrunner.system.logger:test_logger.py:15",
     )
     pytest.approx(
         caplog.records[3].msg,
-        "ERROR    hello world error  flowrunner.system.logger:test_logger.py:16",
+        "ERROR | hello world error | flowrunner.system.logger:test_logger.py:16",
     )
```

### Comparing `flowrunner-0.2.1/tests/test_flowrunner/test_cli.py` & `flowrunner-0.2.2/tests/test_flowrunner/test_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """Commands to check the cli"""
 
 import pytest
 from click.testing import CliRunner
 
-from flowrunner.cli import cli, display, run, show, validate
+from flowrunner.cli import cli, display, display_dir, run, show, validate
 
 
 @pytest.fixture(scope="session")
 def temp_directory_fixture(tmp_path_factory):
     folder = tmp_path_factory.mktemp("example_flowchart")
     return folder
 
@@ -29,30 +29,40 @@
     """Test to check cli::run function"""
     runner = CliRunner()
     result = runner.invoke(run, ["examples/example.py"])
     assert result.exit_code == 0
 
 
 def test_display(temp_directory_fixture):
-    """Test to check cli::flowchart function, we use a temporary directory
+    """Test to check cli::display function, we use a temporary directory
     fixture for saving"""
     runner = CliRunner()
     result = runner.invoke(
         display, ["examples/example.py", f"--path={temp_directory_fixture}"]
     )
     assert result.exit_code == 0
 
 def test_display_description(temp_directory_fixture):
-    """Test to check cli::flowchart function, we use a temporary directory
+    """Test to check cli::display function, we use a temporary directory
     fixture for saving. We use the description flag"""
     runner = CliRunner()
     result = runner.invoke(
         display, ["examples/example.py", f"--path={temp_directory_fixture}", f"--description={True}"]
     )
     assert result.exit_code == 0
 
 
+def test_display_directory(temp_directory_fixture):
+    """Test to check cli::display_dir function, we use a temporary directory
+    fixture for saving. We use the description flag"""
+    runner = CliRunner()
+    result = runner.invoke(
+        display_dir, ["examples", f"--path={temp_directory_fixture}", f"--description={True}"]
+    )
+    assert result.exit_code == 0
+
+
 def test_cli():
     """Test to check cli::cli function"""
     runner = CliRunner()
     result = runner.invoke(cli)
     assert result.exit_code == 0
```

