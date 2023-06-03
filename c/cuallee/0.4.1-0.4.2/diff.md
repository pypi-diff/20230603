# Comparing `tmp/cuallee-0.4.1.tar.gz` & `tmp/cuallee-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuallee-0.4.1.tar", last modified: Sun May 14 15:16:26 2023, max compression
+gzip compressed data, was "cuallee-0.4.2.tar", last modified: Sat Jun  3 16:07:44 2023, max compression
```

## Comparing `cuallee-0.4.1.tar` & `cuallee-0.4.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-05-14 15:16:26.166523 cuallee-0.4.1/
--rw-r--r--   0 herminio  (1000) herminio  (1000)    11357 2022-10-08 07:12:42.000000 cuallee-0.4.1/LICENSE
--rw-r--r--   0 herminio  (1000) herminio  (1000)    13591 2023-05-14 15:16:26.166523 cuallee-0.4.1/PKG-INFO
--rw-r--r--   0 herminio  (1000) herminio  (1000)    12798 2023-05-14 15:09:02.000000 cuallee-0.4.1/README.md
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-05-14 15:16:26.166523 cuallee-0.4.1/cuallee/
--rw-r--r--   0 herminio  (1000) herminio  (1000)    20284 2023-05-14 14:49:13.000000 cuallee-0.4.1/cuallee/__init__.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)     9876 2023-05-14 14:49:09.000000 cuallee-0.4.1/cuallee/duckdb_validation.py
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-05-14 15:16:26.166523 cuallee-0.4.1/cuallee/iso/
--rw-r--r--   0 herminio  (1000) herminio  (1000)        0 2023-05-14 14:49:13.000000 cuallee-0.4.1/cuallee/iso/__init__.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)     2244 2023-05-14 14:49:13.000000 cuallee-0.4.1/cuallee/iso/checks.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    12990 2023-05-14 14:49:13.000000 cuallee-0.4.1/cuallee/pandas_validation.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)        0 2023-05-14 09:02:43.000000 cuallee-0.4.1/cuallee/polars.validation.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    31138 2023-05-14 14:49:09.000000 cuallee-0.4.1/cuallee/pyspark_validation.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)    28442 2023-05-14 09:02:43.000000 cuallee-0.4.1/cuallee/snowpark_validation.py
--rw-r--r--   0 herminio  (1000) herminio  (1000)     2043 2023-05-14 09:02:43.000000 cuallee-0.4.1/cuallee/utils.py
-drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-05-14 15:16:26.166523 cuallee-0.4.1/cuallee.egg-info/
--rw-r--r--   0 herminio  (1000) herminio  (1000)    13591 2023-05-14 15:16:26.000000 cuallee-0.4.1/cuallee.egg-info/PKG-INFO
--rw-r--r--   0 herminio  (1000) herminio  (1000)      427 2023-05-14 15:16:26.000000 cuallee-0.4.1/cuallee.egg-info/SOURCES.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)        1 2023-05-14 15:16:26.000000 cuallee-0.4.1/cuallee.egg-info/dependency_links.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)      281 2023-05-14 15:16:26.000000 cuallee-0.4.1/cuallee.egg-info/requires.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)        8 2023-05-14 15:16:26.000000 cuallee-0.4.1/cuallee.egg-info/top_level.txt
--rw-r--r--   0 herminio  (1000) herminio  (1000)     1164 2023-05-14 15:16:13.000000 cuallee-0.4.1/pyproject.toml
--rw-r--r--   0 herminio  (1000) herminio  (1000)      109 2023-05-14 15:16:26.166523 cuallee-0.4.1/setup.cfg
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-03 16:07:44.616026 cuallee-0.4.2/
+-rw-rw-r--   0 herminio  (1000) herminio  (1000)    11357 2022-09-20 23:24:07.000000 cuallee-0.4.2/LICENSE
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    15051 2023-06-03 16:07:44.616026 cuallee-0.4.2/PKG-INFO
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    14258 2023-06-03 15:46:05.000000 cuallee-0.4.2/README.md
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-03 16:07:44.616026 cuallee-0.4.2/cuallee/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    20284 2023-06-03 15:46:05.000000 cuallee-0.4.2/cuallee/__init__.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     9876 2023-06-03 15:46:05.000000 cuallee-0.4.2/cuallee/duckdb_validation.py
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-03 16:07:44.616026 cuallee-0.4.2/cuallee/iso/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)        0 2023-06-03 15:46:05.000000 cuallee-0.4.2/cuallee/iso/__init__.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     2244 2023-06-03 15:46:05.000000 cuallee-0.4.2/cuallee/iso/checks.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    12990 2023-06-03 15:46:05.000000 cuallee-0.4.2/cuallee/pandas_validation.py
+-rw-rw-r--   0 herminio  (1000) herminio  (1000)        0 2022-11-26 21:58:56.000000 cuallee-0.4.2/cuallee/polars.validation.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    31138 2023-06-03 15:46:05.000000 cuallee-0.4.2/cuallee/pyspark_validation.py
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    28442 2022-12-04 15:12:29.000000 cuallee-0.4.2/cuallee/snowpark_validation.py
+-rw-rw-r--   0 herminio  (1000) herminio  (1000)     2043 2022-10-23 12:45:17.000000 cuallee-0.4.2/cuallee/utils.py
+drwxr-xr-x   0 herminio  (1000) herminio  (1000)        0 2023-06-03 16:07:44.616026 cuallee-0.4.2/cuallee.egg-info/
+-rw-r--r--   0 herminio  (1000) herminio  (1000)    15051 2023-06-03 16:07:44.000000 cuallee-0.4.2/cuallee.egg-info/PKG-INFO
+-rw-r--r--   0 herminio  (1000) herminio  (1000)      427 2023-06-03 16:07:44.000000 cuallee-0.4.2/cuallee.egg-info/SOURCES.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)        1 2023-06-03 16:07:44.000000 cuallee-0.4.2/cuallee.egg-info/dependency_links.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)      298 2023-06-03 16:07:44.000000 cuallee-0.4.2/cuallee.egg-info/requires.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)        8 2023-06-03 16:07:44.000000 cuallee-0.4.2/cuallee.egg-info/top_level.txt
+-rw-r--r--   0 herminio  (1000) herminio  (1000)     1190 2023-06-03 16:07:12.000000 cuallee-0.4.2/pyproject.toml
+-rw-r--r--   0 herminio  (1000) herminio  (1000)      109 2023-06-03 16:07:44.616026 cuallee-0.4.2/setup.cfg
```

### Comparing `cuallee-0.4.1/LICENSE` & `cuallee-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.1/PKG-INFO` & `cuallee-0.4.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: cuallee
-Version: 0.4.1
-Summary: Python library for data validation on DataFrame APIs including Snowflake/Snowpark, Apache/PySpark and Pandas/DataFrame.
-Author-email: Virginie Grosboillot <vestalisvirginis@gmail.com>, Herminio Vazquez <canimus@gmail.com>
-Project-URL: Homepage, https://github.com/canimus/cuallee
-Project-URL: Bug Tracker, https://github.com/canimus/cuallee
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: pyspark
-Provides-Extra: snowpark
-Provides-Extra: pandas
-Provides-Extra: duckdb
-Provides-Extra: polars
-Provides-Extra: iso
-Provides-Extra: test
-License-File: LICENSE
-
 # cuallee
 Meaning `good` in Aztec (Nahuatl), _pronounced: QUAL-E_
 
 This library provides an intuitive `API` to describe `checks` initially just for `PySpark` dataframes `v3.3.0`. And extended to `pandas`, `snowpark`, `duckdb`, and more.
 It is a replacement written in pure `python` of the `pydeequ` framework.
 
 I gave up in _deequ_ as after extensive use, the API is not user-friendly, the Python Callback servers produce additional costs in our compute clusters, and the lack of support to the newest version of PySpark.
@@ -37,14 +16,15 @@
 
 `cuallee` is the data quality framework truly dataframe agnostic.
 
 Provider | API | Versions
  ------- | ----------- | ------
 ![snowflake](logos/snowflake.svg?raw=true "Snowpark DataFrame API")| `snowpark` | `1.4.0`
 ![databricks](logos/databricks.svg?raw=true "PySpark DataFrame API")| `pyspark` | `3.4.0`, `3.3.x`, `3.2.x`
+![bigquery](logos/bigquery.png?raw=true "BigQuery Client API")| `bigquery` | `3.4.1`
 ![pandas](logos/pandas.svg?raw=true "Pandas DataFrame API")| `pandas`| `2.0.1`, `1.5.x`, `1.4.x`
 ![duckdb](logos/duckdb.png?raw=true "DuckDB API")|`duckdb` | `0.7.1`
 ![polars](logos/polars.svg?raw=true "Polars API")|`polars`|`0.15.x (wip)` 
  
  <sub>Logos are trademarks of their own brands.</sub>
 
 ## Stats
@@ -227,14 +207,33 @@
 `is_on_sunday` | For date fields confirms day is `Sun` | _date_
 `is_on_schedule` | For date fields confirms time windows i.e. `9:00 - 17:00` | _timestamp_
 `is_daily` | Can verify daily continuity on date fields by default. `[2,3,4,5,6]` which represents `Mon-Fri` in PySpark. However new schedules can be used for custom date continuity | _date_
 `has_workflow` | Adjacency matrix validation on `3-column` graph, based on `group`, `event`, `order` columns.  | _agnostic_
 `satisfies` | An open `SQL expression` builder to construct custom checks | _agnostic_
 `validate` | The ultimate transformation of a check with a `dataframe` input for validation | _agnostic_
 
+## ISO Standard
+A new module has been incorporated in `cuallee==0.4.0` which allows the verification of International Standard Organization columns in data frames. Simply access the `check.iso` interface to add the set of checks as shown below.
+
+Check | Description | DataType
+ ------- | ----------- | ----
+`iso_4217` | currency compliant `ccy` | _string_
+`iso_3166` | country compliant `country` | _string_
+
+```python
+df = spark.createDataFrame([[1, "USD"], [2, "MXN"], [3, "CAD"], [4, "EUR"], [5, "CHF"]], ["id", "ccy"])
+check = Check(CheckLevel.WARNING, "ISO Compliant")
+check.iso.iso_4217("ccy")
+check.validate(df).show()
++---+-------------------+-------------+-------+------+---------------+--------------------+----+----------+---------+--------------+------+
+| id|          timestamp|        check|  level|column|           rule|               value|rows|violations|pass_rate|pass_threshold|status|
++---+-------------------+-------------+-------+------+---------------+--------------------+----+----------+---------+--------------+------+
+|  1|2023-05-14 18:28:02|ISO Compliant|WARNING|   ccy|is_contained_in|{'BHD', 'CRC', 'M...|   5|       0.0|      1.0|           1.0|  PASS|
++---+-------------------+-------------+-------+------+---------------+--------------------+----+----------+---------+--------------+------+
+```
 
 
 ## Snowflake Connection
 In order to establish a connection to your SnowFlake account `cuallee` relies in the following environment variables to be avaialble in your environment:
 - `SF_ACCOUNT`
 - `SF_USER`
 - `SF_PASSWORD`
@@ -268,17 +267,17 @@
 `100%` data frame agnostic implementation of data quality checks.
 Define once, `run everywhere`
 - [x] PySpark 3.3.0
 - [x] PySpark 3.2.x 
 - [x] Snowpark DataFrame
 - [x] Pandas DataFrame
 - [x] DuckDB Tables
+- [x] BigQuery Client
 - Polars DataFrame
-- SQLite Tables
-- MS-SQL Tables
+
 
 Whilst expanding the functionality feels a bit as an overkill because you most likely can connect `spark` via its drivers to whatever `DBMS` of your choice.
 In the desire to make it even more `user-friendly` we are aiming to make `cuallee` portable to all the providers above.
 
 ## Authors
 - [canimus](https://github.com/canimus) / Herminio Vazquez / 🇲🇽 
 - [vestalisvirginis](https://github.com/vestalisvirginis) / Virginie Grosboillot / 🇫🇷 
@@ -287,8 +286,9 @@
 
 ## License
 Apache License 2.0
 Free for commercial use, modification, distribution, patent use, private use.
 Just preserve the copyright and license.
 
 
-> Made with ❤️ in Utrecht 🇳🇱
+> Made with ❤️ in Utrecht 🇳🇱<br/>
+> Maintained over ⌛ from Ljubljana in 🇸🇮
```

### Comparing `cuallee-0.4.1/README.md` & `cuallee-0.4.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: cuallee
+Version: 0.4.2
+Summary: Python library for data validation on DataFrame APIs including Snowflake/Snowpark, Apache/PySpark and Pandas/DataFrame.
+Author-email: Virginie Grosboillot <vestalisvirginis@gmail.com>, Herminio Vazquez <canimus@gmail.com>
+Project-URL: Homepage, https://github.com/canimus/cuallee
+Project-URL: Bug Tracker, https://github.com/canimus/cuallee
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: pyspark
+Provides-Extra: snowpark
+Provides-Extra: pandas
+Provides-Extra: duckdb
+Provides-Extra: polars
+Provides-Extra: iso
+Provides-Extra: test
+License-File: LICENSE
+
 # cuallee
 Meaning `good` in Aztec (Nahuatl), _pronounced: QUAL-E_
 
 This library provides an intuitive `API` to describe `checks` initially just for `PySpark` dataframes `v3.3.0`. And extended to `pandas`, `snowpark`, `duckdb`, and more.
 It is a replacement written in pure `python` of the `pydeequ` framework.
 
 I gave up in _deequ_ as after extensive use, the API is not user-friendly, the Python Callback servers produce additional costs in our compute clusters, and the lack of support to the newest version of PySpark.
@@ -16,14 +37,15 @@
 
 `cuallee` is the data quality framework truly dataframe agnostic.
 
 Provider | API | Versions
  ------- | ----------- | ------
 ![snowflake](logos/snowflake.svg?raw=true "Snowpark DataFrame API")| `snowpark` | `1.4.0`
 ![databricks](logos/databricks.svg?raw=true "PySpark DataFrame API")| `pyspark` | `3.4.0`, `3.3.x`, `3.2.x`
+![bigquery](logos/bigquery.png?raw=true "BigQuery Client API")| `bigquery` | `3.4.1`
 ![pandas](logos/pandas.svg?raw=true "Pandas DataFrame API")| `pandas`| `2.0.1`, `1.5.x`, `1.4.x`
 ![duckdb](logos/duckdb.png?raw=true "DuckDB API")|`duckdb` | `0.7.1`
 ![polars](logos/polars.svg?raw=true "Polars API")|`polars`|`0.15.x (wip)` 
  
  <sub>Logos are trademarks of their own brands.</sub>
 
 ## Stats
@@ -206,14 +228,33 @@
 `is_on_sunday` | For date fields confirms day is `Sun` | _date_
 `is_on_schedule` | For date fields confirms time windows i.e. `9:00 - 17:00` | _timestamp_
 `is_daily` | Can verify daily continuity on date fields by default. `[2,3,4,5,6]` which represents `Mon-Fri` in PySpark. However new schedules can be used for custom date continuity | _date_
 `has_workflow` | Adjacency matrix validation on `3-column` graph, based on `group`, `event`, `order` columns.  | _agnostic_
 `satisfies` | An open `SQL expression` builder to construct custom checks | _agnostic_
 `validate` | The ultimate transformation of a check with a `dataframe` input for validation | _agnostic_
 
+## ISO Standard
+A new module has been incorporated in `cuallee==0.4.0` which allows the verification of International Standard Organization columns in data frames. Simply access the `check.iso` interface to add the set of checks as shown below.
+
+Check | Description | DataType
+ ------- | ----------- | ----
+`iso_4217` | currency compliant `ccy` | _string_
+`iso_3166` | country compliant `country` | _string_
+
+```python
+df = spark.createDataFrame([[1, "USD"], [2, "MXN"], [3, "CAD"], [4, "EUR"], [5, "CHF"]], ["id", "ccy"])
+check = Check(CheckLevel.WARNING, "ISO Compliant")
+check.iso.iso_4217("ccy")
+check.validate(df).show()
++---+-------------------+-------------+-------+------+---------------+--------------------+----+----------+---------+--------------+------+
+| id|          timestamp|        check|  level|column|           rule|               value|rows|violations|pass_rate|pass_threshold|status|
++---+-------------------+-------------+-------+------+---------------+--------------------+----+----------+---------+--------------+------+
+|  1|2023-05-14 18:28:02|ISO Compliant|WARNING|   ccy|is_contained_in|{'BHD', 'CRC', 'M...|   5|       0.0|      1.0|           1.0|  PASS|
++---+-------------------+-------------+-------+------+---------------+--------------------+----+----------+---------+--------------+------+
+```
 
 
 ## Snowflake Connection
 In order to establish a connection to your SnowFlake account `cuallee` relies in the following environment variables to be avaialble in your environment:
 - `SF_ACCOUNT`
 - `SF_USER`
 - `SF_PASSWORD`
@@ -247,17 +288,17 @@
 `100%` data frame agnostic implementation of data quality checks.
 Define once, `run everywhere`
 - [x] PySpark 3.3.0
 - [x] PySpark 3.2.x 
 - [x] Snowpark DataFrame
 - [x] Pandas DataFrame
 - [x] DuckDB Tables
+- [x] BigQuery Client
 - Polars DataFrame
-- SQLite Tables
-- MS-SQL Tables
+
 
 Whilst expanding the functionality feels a bit as an overkill because you most likely can connect `spark` via its drivers to whatever `DBMS` of your choice.
 In the desire to make it even more `user-friendly` we are aiming to make `cuallee` portable to all the providers above.
 
 ## Authors
 - [canimus](https://github.com/canimus) / Herminio Vazquez / 🇲🇽 
 - [vestalisvirginis](https://github.com/vestalisvirginis) / Virginie Grosboillot / 🇫🇷 
@@ -266,8 +307,9 @@
 
 ## License
 Apache License 2.0
 Free for commercial use, modification, distribution, patent use, private use.
 Just preserve the copyright and license.
 
 
-> Made with ❤️ in Utrecht 🇳🇱
+> Made with ❤️ in Utrecht 🇳🇱<br/>
+> Maintained over ⌛ from Ljubljana in 🇸🇮
```

### Comparing `cuallee-0.4.1/cuallee/__init__.py` & `cuallee-0.4.2/cuallee/__init__.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.1/cuallee/duckdb_validation.py` & `cuallee-0.4.2/cuallee/duckdb_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.1/cuallee/iso/checks.py` & `cuallee-0.4.2/cuallee/iso/checks.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.1/cuallee/pandas_validation.py` & `cuallee-0.4.2/cuallee/pandas_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.1/cuallee/pyspark_validation.py` & `cuallee-0.4.2/cuallee/pyspark_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.1/cuallee/snowpark_validation.py` & `cuallee-0.4.2/cuallee/snowpark_validation.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.1/cuallee/utils.py` & `cuallee-0.4.2/cuallee/utils.py`

 * *Files identical despite different names*

### Comparing `cuallee-0.4.1/cuallee.egg-info/PKG-INFO` & `cuallee-0.4.2/cuallee.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuallee
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python library for data validation on DataFrame APIs including Snowflake/Snowpark, Apache/PySpark and Pandas/DataFrame.
 Author-email: Virginie Grosboillot <vestalisvirginis@gmail.com>, Herminio Vazquez <canimus@gmail.com>
 Project-URL: Homepage, https://github.com/canimus/cuallee
 Project-URL: Bug Tracker, https://github.com/canimus/cuallee
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -37,14 +37,15 @@
 
 `cuallee` is the data quality framework truly dataframe agnostic.
 
 Provider | API | Versions
  ------- | ----------- | ------
 ![snowflake](logos/snowflake.svg?raw=true "Snowpark DataFrame API")| `snowpark` | `1.4.0`
 ![databricks](logos/databricks.svg?raw=true "PySpark DataFrame API")| `pyspark` | `3.4.0`, `3.3.x`, `3.2.x`
+![bigquery](logos/bigquery.png?raw=true "BigQuery Client API")| `bigquery` | `3.4.1`
 ![pandas](logos/pandas.svg?raw=true "Pandas DataFrame API")| `pandas`| `2.0.1`, `1.5.x`, `1.4.x`
 ![duckdb](logos/duckdb.png?raw=true "DuckDB API")|`duckdb` | `0.7.1`
 ![polars](logos/polars.svg?raw=true "Polars API")|`polars`|`0.15.x (wip)` 
  
  <sub>Logos are trademarks of their own brands.</sub>
 
 ## Stats
@@ -227,14 +228,33 @@
 `is_on_sunday` | For date fields confirms day is `Sun` | _date_
 `is_on_schedule` | For date fields confirms time windows i.e. `9:00 - 17:00` | _timestamp_
 `is_daily` | Can verify daily continuity on date fields by default. `[2,3,4,5,6]` which represents `Mon-Fri` in PySpark. However new schedules can be used for custom date continuity | _date_
 `has_workflow` | Adjacency matrix validation on `3-column` graph, based on `group`, `event`, `order` columns.  | _agnostic_
 `satisfies` | An open `SQL expression` builder to construct custom checks | _agnostic_
 `validate` | The ultimate transformation of a check with a `dataframe` input for validation | _agnostic_
 
+## ISO Standard
+A new module has been incorporated in `cuallee==0.4.0` which allows the verification of International Standard Organization columns in data frames. Simply access the `check.iso` interface to add the set of checks as shown below.
+
+Check | Description | DataType
+ ------- | ----------- | ----
+`iso_4217` | currency compliant `ccy` | _string_
+`iso_3166` | country compliant `country` | _string_
+
+```python
+df = spark.createDataFrame([[1, "USD"], [2, "MXN"], [3, "CAD"], [4, "EUR"], [5, "CHF"]], ["id", "ccy"])
+check = Check(CheckLevel.WARNING, "ISO Compliant")
+check.iso.iso_4217("ccy")
+check.validate(df).show()
++---+-------------------+-------------+-------+------+---------------+--------------------+----+----------+---------+--------------+------+
+| id|          timestamp|        check|  level|column|           rule|               value|rows|violations|pass_rate|pass_threshold|status|
++---+-------------------+-------------+-------+------+---------------+--------------------+----+----------+---------+--------------+------+
+|  1|2023-05-14 18:28:02|ISO Compliant|WARNING|   ccy|is_contained_in|{'BHD', 'CRC', 'M...|   5|       0.0|      1.0|           1.0|  PASS|
++---+-------------------+-------------+-------+------+---------------+--------------------+----+----------+---------+--------------+------+
+```
 
 
 ## Snowflake Connection
 In order to establish a connection to your SnowFlake account `cuallee` relies in the following environment variables to be avaialble in your environment:
 - `SF_ACCOUNT`
 - `SF_USER`
 - `SF_PASSWORD`
@@ -268,17 +288,17 @@
 `100%` data frame agnostic implementation of data quality checks.
 Define once, `run everywhere`
 - [x] PySpark 3.3.0
 - [x] PySpark 3.2.x 
 - [x] Snowpark DataFrame
 - [x] Pandas DataFrame
 - [x] DuckDB Tables
+- [x] BigQuery Client
 - Polars DataFrame
-- SQLite Tables
-- MS-SQL Tables
+
 
 Whilst expanding the functionality feels a bit as an overkill because you most likely can connect `spark` via its drivers to whatever `DBMS` of your choice.
 In the desire to make it even more `user-friendly` we are aiming to make `cuallee` portable to all the providers above.
 
 ## Authors
 - [canimus](https://github.com/canimus) / Herminio Vazquez / 🇲🇽 
 - [vestalisvirginis](https://github.com/vestalisvirginis) / Virginie Grosboillot / 🇫🇷 
@@ -287,8 +307,9 @@
 
 ## License
 Apache License 2.0
 Free for commercial use, modification, distribution, patent use, private use.
 Just preserve the copyright and license.
 
 
-> Made with ❤️ in Utrecht 🇳🇱
+> Made with ❤️ in Utrecht 🇳🇱<br/>
+> Maintained over ⌛ from Ljubljana in 🇸🇮
```

### Comparing `cuallee-0.4.1/pyproject.toml` & `cuallee-0.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cuallee"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="Virginie Grosboillot", email="vestalisvirginis@gmail.com" },
   { name="Herminio Vazquez", email="canimus@gmail.com"}
 ]
 description = "Python library for data validation on DataFrame APIs including Snowflake/Snowpark, Apache/PySpark and Pandas/DataFrame."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -17,15 +17,16 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "colorama >= 0.4.6",
     "toolz >= 0.12.0",
     "pygments >= 2.15.1",
-    "lxml >= 4.9.2"
+    "lxml >= 4.9.2",
+    "requests >= 2.28.2"
 ]
 
 [project.optional-dependencies]
 pyspark = [
   "pyspark>=3.4.0"
 ]
 snowpark = [
```

