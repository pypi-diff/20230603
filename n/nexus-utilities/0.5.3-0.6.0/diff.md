# Comparing `tmp/nexus-utilities-0.5.3.tar.gz` & `tmp/nexus-utilities-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus-utilities-0.5.3.tar", last modified: Tue May 23 13:14:59 2023, max compression
+gzip compressed data, was "nexus-utilities-0.6.0.tar", last modified: Sat Jun  3 15:57:03 2023, max compression
```

## Comparing `nexus-utilities-0.5.3.tar` & `nexus-utilities-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:14:59.103170 nexus-utilities-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-23 13:14:59.103170 nexus-utilities-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:14:59.103170 nexus-utilities-0.5.3/nexus_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-23 13:14:58.000000 nexus-utilities-0.5.3/nexus_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-23 13:14:59.000000 nexus-utilities-0.5.3/nexus_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:14:58.000000 nexus-utilities-0.5.3/nexus_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-23 13:14:58.000000 nexus-utilities-0.5.3/nexus_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 13:14:58.000000 nexus-utilities-0.5.3/nexus_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:14:59.103170 nexus-utilities-0.5.3/nexus_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/nexus_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/nexus_utils/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/nexus_utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/nexus_utils/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/nexus_utils/flatfile_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/nexus_utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/nexus_utils/password_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/nexus_utils/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:14:59.103170 nexus-utilities-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-23 13:14:48.000000 nexus-utilities-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:57:03.239004 nexus-utilities-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-03 15:57:03.239004 nexus-utilities-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:57:03.235004 nexus-utilities-0.6.0/nexus_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-03 15:57:02.000000 nexus-utilities-0.6.0/nexus_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-03 15:57:03.000000 nexus-utilities-0.6.0/nexus_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 15:57:02.000000 nexus-utilities-0.6.0/nexus_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-03 15:57:02.000000 nexus-utilities-0.6.0/nexus_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 15:57:02.000000 nexus-utilities-0.6.0/nexus_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:57:03.239004 nexus-utilities-0.6.0/nexus_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/nexus_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/nexus_utils/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/nexus_utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/nexus_utils/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/nexus_utils/flatfile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/nexus_utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/nexus_utils/password_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/nexus_utils/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 15:57:03.239004 nexus-utilities-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/setup.py
```

### Comparing `nexus-utilities-0.5.3/LICENSE.txt` & `nexus-utilities-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.5.3/PKG-INFO` & `nexus-utilities-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.5.3
+Version: 0.6.0
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.5.3/README.md` & `nexus-utilities-0.6.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,28 +4,32 @@
 ## Table of Contents <!-- omit in toc -->
 
 - [Installation](#installation)
 - [config\_utils.py](#config_utilspy)
   - [**read\_config\_file(config\_filepath)**](#read_config_fileconfig_filepath)
 - [database\_utils.py](#database_utilspy)
   - [**build\_engine(connect\_type, server\_address, server\_port, server\_name, user\_name, password, schema=None)**](#build_engineconnect_type-server_address-server_port-server_name-user_name-password-schemanone)
+  - [**check\_engine\_read(engine, schema=None, table\_name=None)**](#check_engine_readengine-schemanone-table_namenone)
+  - [**check\_engine\_write\_delete(engine, schema=None)**](#check_engine_write_deleteengine-schemanone)
   - [**clean\_sql\_statement(sql\_statement)**](#clean_sql_statementsql_statement)
 - [datetime\_utils.py](#datetime_utilspy)
   - [**get\_current\_timestamp()**](#get_current_timestamp)
   - [**get\_duration(then, now=datetime.datetime.now())**](#get_durationthen-nowdatetimedatetimenow)
   - [**determine\_date\_format(date\_list)**](#determine_date_formatdate_list)
 - [flatfile\_utils.py](#flatfile_utilspy)
   - [**detect\_encoding(file\_path)**](#detect_encodingfile_path)
   - [**analyze\_dataframe(df)**](#analyze_dataframedf)
 - [package\_utils.py](#package_utilspy)
   - [**add\_package\_to\_path()**](#add_package_to_path)
   - [**import\_relative(package\_root\_name, module\_path, import\_name, alias=None)**](#import_relativepackage_root_name-module_path-import_name-aliasnone)
+  - [**extract\_from\_error(full\_error\_message, error\_keyword)**](#extract_from_errorfull_error_message-error_keyword)
 - [password\_utils.py](#password_utilspy)
   - [**get\_password(password\_method, password\_key, account\_name=None, access\_key=None, secret\_key=None, endpoint\_url=None, region\_name=None, password\_path=None, encoding='utf-8')**](#get_passwordpassword_method-password_key-account_namenone-access_keynone-secret_keynone-endpoint_urlnone-region_namenone-password_pathnone-encodingutf-8)
 - [string\_utils.py](#string_utilspy)
+  - [**string\_to\_bool(bool\_string)**](#string_to_boolbool_string)
   - [**cleanse\_string(string, remove\_symbols=True, title\_to\_snake\_case=False, hyphen\_to\_underscore=True, period\_to\_underscore=True, to\_upper=False, to\_lower=True)**](#cleanse_stringstring-remove_symbolstrue-title_to_snake_casefalse-hyphen_to_underscoretrue-period_to_underscoretrue-to_upperfalse-to_lowertrue)
 - [About the Author](#about-the-author)
 
 ---
 
 ## Installation
 
@@ -69,14 +73,38 @@
  * ***schema (str):*** Default database schema (optional)
 
 Returns:
  * ***engine (sqlalchemy.engine.Engine Class):*** SQLAlchemy Engine Class for interacting with the database
 
 Creates a SQLAlchemy Engine Class object for interacting with your database.
 
+### **check_engine_read(engine, schema=None, table_name=None)**
+
+Arguments:
+ * ***engine (sqlalchemy.engine.Engine Class):*** Engine object to attempt connection
+ * ***schema (str):*** Optional argument to specify the schema to test
+ * ***table_name (str):*** Optional argument to specify a table to test  
+*Note:*  Both schema and table_name must be provided to utilize that functionality
+
+Returns:
+ * ***result (str):*** "Success" or the text content of any error encountered
+
+Checks that an established SQLAlchemy Engine Class object has select access to the default schema.  If a schema and table_name is provided, ity will use a "SELECT COUNT(*) FROM {schema}.{table_name}" to confirm, otherwise it utilizes a simple "SELECT 1" from the default schema.
+
+### **check_engine_write_delete(engine, schema=None)**
+
+Arguments:
+ * ***engine (sqlalchemy.engine.Engine Class):*** Engine object to attempt connection
+ * ***schema (str):*** Optional argument to specify the schema to test
+
+Returns:
+ * ***result (str):*** "Success" or the text content of any error encountered
+
+Checks that an established SQLAlchemy Engine Class object has create, write, delete and drop permissions on the specified schema.  It does this by creating a "nexus_access_test" table, inserting into it, updating it, deleting from it, then dropping it.  Helpful for checking the functionality of a connection object designed for ETL activities.
+
 ### **clean_sql_statement(sql_statement)**
 
 Arguments:
  * ***sql_statement (str):*** SQL script to be cleansed
 
 Returns:
  * ***sql_statements_output (list):*** List of cleansed SQL statements in the order they appeared in the provided script
@@ -213,14 +241,25 @@
  * ***import_name (str):*** Name of the object to be imported.  Can be a ".py" file name, or a function within a ".py" file (in the latter case, make sure the ".py" file name is part of the "module_path" above)
 * ***alias (str):*** Optional alias for the imported library or function
 
 Allows for importing package-relative libraries or functions given a programmatically-determined package root folder.  Useful for programs with multiple entry points and utilities called from multiple libraries.
 
 ***Important note: Pylance will show an error since the imports are done at runtime.  These can be avoided by attaching "# type: ignore" to any line using one of these relative imports.***
 
+### **extract_from_error(full_error_message, error_keyword)**
+
+Arguments:
+ * ***full_error_message (str):*** Full error text 
+ * ***error_keyword (str):*** Dot-separated path from the package root to the library to be imported
+
+Returns:
+ * ***error_message (str):***  Single line error message
+
+Accepts a full error message, identifies the first line containing a provided keyword, and returns only that line.  Can be helpful if you want to capture the most important portion of an error without printing the entire stack trace.
+
 ---
 
 ## password_utils.py
 
 This module contains functions for working with passwords and other sensitive information.
 
 ### **get_password(password_method, password_key, account_name=None, access_key=None, secret_key=None, endpoint_url=None, region_name=None, password_path=None, encoding='utf-8')**
@@ -264,14 +303,26 @@
 
 ---
 
 ## string_utils.py
 
 This module contains functions for working with strings.
 
+### **string_to_bool(bool_string)**
+
+Arguments:
+ * ***bool_string (str):*** String to attempt to convert to a boolean
+
+Returns:
+ * ***string (bool or str):*** Will return booleans True or False if conversion is successful, or a string explaining why the conversion failed, either due to an invalid input type provided, or an unrecognized value
+
+Takes a string input and attempts to interpret it as a boolean value based on the below recognized values (after converting to lowercase):
+* **True:**  ['true', 't', 'yes', 'y', 'yep', 'yeah', 'affirmative', 'x', '1', '1.0', 'on', 'enabled']
+* **False:**  ['false', 'f', 'no', 'n', 'nope', 'nah', '', '0', '0.0', 'off', 'disabled']
+
 ### **cleanse_string(string, remove_symbols=True, title_to_snake_case=False, hyphen_to_underscore=True, period_to_underscore=True, to_upper=False, to_lower=True)**
 
 Arguments:
  * ***string (str):*** String to be cleansed
  * ***remove_symbols (bool):*** Remove some symbols, and replace others with "_"
  * ***title_to_snake_case (bool):*** Convert TitleCase to Snake_Case
  * ***hyphen_to_underscore (bool):*** Change hypehens to underscores
```

### Comparing `nexus-utilities-0.5.3/nexus_utilities.egg-info/PKG-INFO` & `nexus-utilities-0.6.0/nexus_utilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.5.3
+Version: 0.6.0
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.5.3/nexus_utils/config_utils.py` & `nexus-utilities-0.6.0/nexus_utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.5.3/nexus_utils/datetime_utils.py` & `nexus-utilities-0.6.0/nexus_utils/datetime_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -274,68 +274,66 @@
     except ValueError:
       date_format = None
   
   return date_format, format_string
 
 #%%
 # Left in for testing purposes
-# if __name__ == "__main__":
-"""
-import pandas as pd
+if __name__ == "__main__":
+  import pandas as pd
 
-file_path = r''
+  file_path = r''
 
-if file_path:
-  # Read the .txt file into a DataFrame
-  df = pd.read_csv(file_path, delimiter='\t', encoding='utf-16')
+  if file_path:
+    # Read the .txt file into a DataFrame
+    df = pd.read_csv(file_path, delimiter='\t', encoding='utf-16')
 
-  date_list = df['DownloadDatePST'].tolist()
-#%%
-determine_date_format(date_list)
+    date_list = df['DownloadDatePST'].tolist()
+  #%%
+  determine_date_format(date_list)
 
-#%%
+  #%%
 
-date_list = ['13/5/2023', '5/5/2023', '17/10/2023']
-determine_date_format(date_list)
+  date_list = ['13/5/2023', '5/5/2023', '17/10/2023']
+  determine_date_format(date_list)
 
-#%%
+  #%%
 
-date_list = ['5/5/2023', '6/5/2023', '7/5/2023']
-determine_date_format(date_list)
+  date_list = ['5/5/2023', '6/5/2023', '7/5/2023']
+  determine_date_format(date_list)
 
-#%%
+  #%%
 
-date_list = ['5/5/2023', '5/6/2023', '5/7/2023']
-determine_date_format(date_list)
+  date_list = ['5/5/2023', '5/6/2023', '5/7/2023']
+  determine_date_format(date_list)
 
-#%%
+  #%%
 
-date_list = ['2023-5-5', '2023-5-6', '2023-5-17']
-determine_date_format(date_list)
+  date_list = ['2023-5-5', '2023-5-6', '2023-5-17']
+  determine_date_format(date_list)
 
-#%%
+  #%%
 
-date_list = ['2023-5-15', '2023-5-16', '2023-5-17']
-determine_date_format(date_list)
+  date_list = ['2023-5-15', '2023-5-16', '2023-5-17']
+  determine_date_format(date_list)
 
-#%%
+  #%%
 
-date_list = ['20230515', '20230516', '20230517']
-determine_date_format(date_list)
+  date_list = ['20230515', '20230516', '20230517']
+  determine_date_format(date_list)
 
-#%%
+  #%%
 
-date_list = ['05152023', '05162023', '05172023']
-determine_date_format(date_list)
+  date_list = ['05152023', '05162023', '05172023']
+  determine_date_format(date_list)
 
-#%%
+  #%%
 
-date_list = ['051523', '051623', '051723']
-print(determine_date_format(date_list))
+  date_list = ['051523', '051623', '051723']
+  print(determine_date_format(date_list))
 
-#%%
+  #%%
 
-date_list = ['05052023', '05052023', '05052023']
-print(determine_date_format(date_list))
+  date_list = ['05052023', '05052023', '05052023']
+  print(determine_date_format(date_list))
 
-#%%
-"""
+  #%%
```

### Comparing `nexus-utilities-0.5.3/nexus_utils/flatfile_utils.py` & `nexus-utilities-0.6.0/nexus_utils/flatfile_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.5.3/nexus_utils/package_utils.py` & `nexus-utilities-0.6.0/nexus_utils/package_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -72,7 +72,15 @@
     if alias:
         caller_globals[alias] = obj
     else:
         caller_globals[import_name] = obj
 
     # Return the imported object
     # return obj
+
+def extract_from_error(full_error_message, error_keyword):
+    """Extract a single line from error message based on keyword"""
+    
+    error_lines = full_error_message.splitlines()
+    error_message = next((line for line in error_lines if error_keyword in line), None)
+    
+    return error_message
```

### Comparing `nexus-utilities-0.5.3/nexus_utils/password_utils.py` & `nexus-utilities-0.6.0/nexus_utils/password_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.5.3/nexus_utils/string_utils.py` & `nexus-utilities-0.6.0/nexus_utils/string_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,31 @@
 #%%
 import re
 
 # def title_to_snake_case(string):
 #     converted_string = re.sub(r'(?<=[a-z0-9])([A-Z])|(?<=[^_])([A-Z](?=[a-z]))', r'_\1\2', string)
 #     return converted_string.lower()
 
+def string_to_bool(bool_string):
+    """Attempts to change a string into its representative boolean.  If it cannot, it will return a string with the boolean_string provided"""
+    if isinstance(bool_string, bool):
+        return bool_string
+    else:
+        try:
+            bool_string = str(bool_string)
+        except ValueError:
+            return f'Value not a string.  Type: {type(bool_string)}'
+
+        if str(bool_string).lower() in ['true', 't', 'yes', 'y', 'yep', 'yeah', 'affirmative', 'x', '1', '1.0', 'on', 'enabled']:
+            return True
+        elif str(bool_string).lower() in ['false', 'f', 'no', 'n', 'nope', 'nah', '', '0', '0.0', 'off', 'disabled']:
+            return False
+        else:
+            return f"Unknown boolean: '{str(bool_string)}'"
+
 def cleanse_string(
     string, 
     remove_symbols=True, 
     title_to_snake_case=False, 
     hyphen_to_underscore=True, 
     period_to_underscore=True, 
     to_upper=False, 
@@ -50,19 +67,33 @@
         if to_lower:
             string = string.lower()
 
         return string
     
     return None
 #%%
+if __name__ == '__main__':
 
-"""
-print(cleanse_string(
-    'Field__(Name)', 
-    remove_symbols=True, 
-    title_to_snake_case=True, 
-    hyphen_to_underscore=True, 
-    period_to_underscore=True, 
-    to_upper=False, 
-    to_lower=True
-))
-"""
+    class NoStringRepresentation:
+        def __str__(self):
+            raise ValueError("")
+
+    obj = NoStringRepresentation()
+
+    print(string_to_bool(0))
+    print(string_to_bool(0.0))
+    print(string_to_bool(1.0))
+    print(string_to_bool('hello'))
+    print(string_to_bool(obj))
+
+    """
+    print(cleanse_string(
+        'Field__(Name)', 
+        remove_symbols=True, 
+        title_to_snake_case=True, 
+        hyphen_to_underscore=True, 
+        period_to_underscore=True, 
+        to_upper=False, 
+        to_lower=True
+    ))
+    """
+    # %%
```

### Comparing `nexus-utilities-0.5.3/setup.py` & `nexus-utilities-0.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nexus-utilities',
-    version='0.5.3',
+    version='0.6.0',
     author='James Larsen',
     author_email='james.larsen42@gmail.com',
     description='Common python utilities',
     long_description='This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.',
     long_description_content_type='text/markdown',
     url='https://github.com/james-larsen/nexus-utilities',
     packages=['nexus_utils'],
```

