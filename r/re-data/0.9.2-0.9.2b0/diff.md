# Comparing `tmp/re_data-0.9.2.tar.gz` & `tmp/re_data-0.9.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "re_data-0.9.2.tar", last modified: Fri Jun 17 12:21:37 2022, max compression
+gzip compressed data, was "re_data-0.9.2b0.tar", last modified: Fri Jun 17 11:47:16 2022, max compression
```

## Comparing `re_data-0.9.2.tar` & `re_data-0.9.2b0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:37.476852 re_data-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-06-17 12:21:24.000000 re_data-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-06-17 12:21:24.000000 re_data-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2086 2022-06-17 12:21:37.476852 re_data-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-06-17 12:21:24.000000 re_data-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:37.468852 re_data-0.9.2/re_data/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20136 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/command_line.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:37.468852 re_data-0.9.2/re_data/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1806 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/config/system.py
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/config/validate.py
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/config/yaml_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:37.472852 re_data-0.9.2/re_data/dbt_template/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/dbt_template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/dbt_template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:37.472852 re_data-0.9.2/re_data/dbt_template/analysis/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/dbt_template/analysis/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:37.472852 re_data-0.9.2/re_data/dbt_template/macros/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/dbt_template/macros/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/dbt_template/macros/schema_changes.sql
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:37.472852 re_data-0.9.2/re_data/dbt_template/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/dbt_template/models/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/dbt_template/models/pending_orders_per_customer.sql
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/dbt_template/packages.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:37.472852 re_data-0.9.2/re_data/dbt_template/seeds/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/dbt_template/seeds/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/dbt_template/seeds/customers.csv
--rw-r--r--   0 runner    (1001) docker     (121)     9558 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/dbt_template/seeds/orders.csv
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/dbt_template/seeds/schema.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:37.472852 re_data-0.9.2/re_data/dbt_template/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/dbt_template/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:37.472852 re_data-0.9.2/re_data/include/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/include/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)  2514719 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/include/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:37.476852 re_data-0.9.2/re_data/notifications/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/notifications/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:37.476852 re_data-0.9.2/re_data/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/templates/dbt_project.yml
--rw-r--r--   0 runner    (1001) docker     (121)     7309 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/templates/email_alert.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:37.476852 re_data-0.9.2/re_data/templating/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/templating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/templating/render.py
--rw-r--r--   0 runner    (1001) docker     (121)     3111 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/tracking.py
--rw-r--r--   0 runner    (1001) docker     (121)    10271 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-06-17 12:21:24.000000 re_data-0.9.2/re_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 12:21:37.468852 re_data-0.9.2/re_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2086 2022-06-17 12:21:36.000000 re_data-0.9.2/re_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-06-17 12:21:37.000000 re_data-0.9.2/re_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-17 12:21:36.000000 re_data-0.9.2/re_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-06-17 12:21:37.000000 re_data-0.9.2/re_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-06-17 12:21:37.000000 re_data-0.9.2/re_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-17 12:21:37.000000 re_data-0.9.2/re_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-17 12:21:37.476852 re_data-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2022-06-17 12:21:24.000000 re_data-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:16.939895 re_data-0.9.2b0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-06-17 11:47:02.000000 re_data-0.9.2b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2022-06-17 11:47:02.000000 re_data-0.9.2b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2088 2022-06-17 11:47:16.939895 re_data-0.9.2b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-06-17 11:47:02.000000 re_data-0.9.2b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:16.931895 re_data-0.9.2b0/re_data/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20136 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/command_line.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:16.931895 re_data-0.9.2b0/re_data/config/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1806 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/config/system.py
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      984 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/config/validate.py
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/config/yaml_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:16.931895 re_data-0.9.2b0/re_data/dbt_template/
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/dbt_template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1185 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/dbt_template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:16.931895 re_data-0.9.2b0/re_data/dbt_template/analysis/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/dbt_template/analysis/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:16.931895 re_data-0.9.2b0/re_data/dbt_template/macros/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/dbt_template/macros/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)      413 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/dbt_template/macros/schema_changes.sql
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:16.931895 re_data-0.9.2b0/re_data/dbt_template/models/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/dbt_template/models/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)      374 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/dbt_template/models/pending_orders_per_customer.sql
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/dbt_template/packages.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:16.935895 re_data-0.9.2b0/re_data/dbt_template/seeds/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/dbt_template/seeds/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/dbt_template/seeds/customers.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     9558 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/dbt_template/seeds/orders.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      733 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/dbt_template/seeds/schema.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:16.935895 re_data-0.9.2b0/re_data/dbt_template/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/dbt_template/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:16.935895 re_data-0.9.2b0/re_data/include/
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/include/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)  2514719 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/include/index.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:16.935895 re_data-0.9.2b0/re_data/notifications/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      515 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/notifications/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:16.935895 re_data-0.9.2b0/re_data/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/templates/dbt_project.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     7309 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/templates/email_alert.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:16.935895 re_data-0.9.2b0/re_data/templating/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/templating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/templating/render.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3111 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10271 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-06-17 11:47:02.000000 re_data-0.9.2b0/re_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 11:47:16.931895 re_data-0.9.2b0/re_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2088 2022-06-17 11:47:16.000000 re_data-0.9.2b0/re_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-06-17 11:47:16.000000 re_data-0.9.2b0/re_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-17 11:47:16.000000 re_data-0.9.2b0/re_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-06-17 11:47:16.000000 re_data-0.9.2b0/re_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2022-06-17 11:47:16.000000 re_data-0.9.2b0/re_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-17 11:47:16.000000 re_data-0.9.2b0/re_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-17 11:47:16.939895 re_data-0.9.2b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1359 2022-06-17 11:47:02.000000 re_data-0.9.2b0/setup.py
```

### Comparing `re_data-0.9.2/LICENSE` & `re_data-0.9.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `re_data-0.9.2/MANIFEST.in` & `re_data-0.9.2b0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `re_data-0.9.2/PKG-INFO` & `re_data-0.9.2b0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re_data
-Version: 0.9.2
+Version: 0.9.2b0
 Summary: re_data - data quality framework
 Home-page: https://github.com/re-data/re-data
 Author: redata-team
 Author-email: mateusz@getre.io
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: re_data Version: 0.9.2 Summary: re_data - data
+Metadata-Version: 2.1 Name: re_data Version: 0.9.2b0 Summary: re_data - data
 quality framework Home-page: https://github.com/re-data/re-data Author: redata-
 team Author-email: mateusz@getre.io License: MIT Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown Provides-Extra: dev License-File: LICENSE
                                     [Logo]
                              [Slack] [Last commit]
```

### Comparing `re_data-0.9.2/README.md` & `re_data-0.9.2b0/README.md`

 * *Files identical despite different names*

### Comparing `re_data-0.9.2/re_data/command_line.py` & `re_data-0.9.2b0/re_data/command_line.py`

 * *Files identical despite different names*

### Comparing `re_data-0.9.2/re_data/config/system.py` & `re_data-0.9.2b0/re_data/config/system.py`

 * *Files identical despite different names*

### Comparing `re_data-0.9.2/re_data/config/utils.py` & `re_data-0.9.2b0/re_data/config/utils.py`

 * *Files identical despite different names*

### Comparing `re_data-0.9.2/re_data/config/validate.py` & `re_data-0.9.2b0/re_data/config/validate.py`

 * *Files identical despite different names*

### Comparing `re_data-0.9.2/re_data/dbt_template/README.md` & `re_data-0.9.2b0/re_data/dbt_template/README.md`

 * *Files identical despite different names*

### Comparing `re_data-0.9.2/re_data/dbt_template/seeds/orders.csv` & `re_data-0.9.2b0/re_data/dbt_template/seeds/orders.csv`

 * *Files identical despite different names*

### Comparing `re_data-0.9.2/re_data/dbt_template/seeds/schema.yml` & `re_data-0.9.2b0/re_data/dbt_template/seeds/schema.yml`

 * *Files identical despite different names*

### Comparing `re_data-0.9.2/re_data/include/index.html` & `re_data-0.9.2b0/re_data/include/index.html`

 * *Files identical despite different names*

### Comparing `re_data-0.9.2/re_data/notifications/slack.py` & `re_data-0.9.2b0/re_data/notifications/slack.py`

 * *Files identical despite different names*

### Comparing `re_data-0.9.2/re_data/templates/dbt_project.yml` & `re_data-0.9.2b0/re_data/templates/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `re_data-0.9.2/re_data/templates/email_alert.html` & `re_data-0.9.2b0/re_data/templates/email_alert.html`

 * *Files identical despite different names*

### Comparing `re_data-0.9.2/re_data/tracking.py` & `re_data-0.9.2b0/re_data/tracking.py`

 * *Files identical despite different names*

### Comparing `re_data-0.9.2/re_data/utils.py` & `re_data-0.9.2b0/re_data/utils.py`

 * *Files identical despite different names*

### Comparing `re_data-0.9.2/re_data/version.py` & `re_data-0.9.2b0/re_data/version.py`

 * *Files identical despite different names*

### Comparing `re_data-0.9.2/re_data.egg-info/PKG-INFO` & `re_data-0.9.2b0/re_data.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: re-data
-Version: 0.9.2
+Version: 0.9.2b0
 Summary: re_data - data quality framework
 Home-page: https://github.com/re-data/re-data
 Author: redata-team
 Author-email: mateusz@getre.io
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: re-data Version: 0.9.2 Summary: re_data - data
+Metadata-Version: 2.1 Name: re-data Version: 0.9.2b0 Summary: re_data - data
 quality framework Home-page: https://github.com/re-data/re-data Author: redata-
 team Author-email: mateusz@getre.io License: MIT Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown Provides-Extra: dev License-File: LICENSE
                                     [Logo]
                              [Slack] [Last commit]
```

### Comparing `re_data-0.9.2/re_data.egg-info/SOURCES.txt` & `re_data-0.9.2b0/re_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `re_data-0.9.2/setup.py` & `re_data-0.9.2b0/setup.py`

 * *Files identical despite different names*

