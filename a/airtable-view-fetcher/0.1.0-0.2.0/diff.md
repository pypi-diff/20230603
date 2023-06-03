# Comparing `tmp/airtable_view_fetcher-0.1.0.tar.gz` & `tmp/airtable_view_fetcher-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtable_view_fetcher-0.1.0.tar", last modified: Fri Jun  2 11:54:42 2023, max compression
+gzip compressed data, was "airtable_view_fetcher-0.2.0.tar", last modified: Sat Jun  3 13:42:21 2023, max compression
```

## Comparing `airtable_view_fetcher-0.1.0.tar` & `airtable_view_fetcher-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-02 11:54:42.247986 airtable_view_fetcher-0.1.0/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1070 2023-06-02 08:31:49.000000 airtable_view_fetcher-0.1.0/LICENSE
--rw-rw-r--   0 dev       (1000) dev       (1000)      370 2023-06-02 11:54:42.247986 airtable_view_fetcher-0.1.0/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)     1021 2023-06-02 11:51:22.000000 airtable_view_fetcher-0.1.0/README.md
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-02 11:54:42.247986 airtable_view_fetcher-0.1.0/airtable_view_fetcher/
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2023-06-02 08:40:25.000000 airtable_view_fetcher-0.1.0/airtable_view_fetcher/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1807 2023-06-02 08:41:11.000000 airtable_view_fetcher-0.1.0/airtable_view_fetcher/fetch_airtable_data.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-02 11:54:42.247986 airtable_view_fetcher-0.1.0/airtable_view_fetcher.egg-info/
--rw-rw-r--   0 dev       (1000) dev       (1000)      370 2023-06-02 11:54:42.000000 airtable_view_fetcher-0.1.0/airtable_view_fetcher.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)      377 2023-06-02 11:54:42.000000 airtable_view_fetcher-0.1.0/airtable_view_fetcher.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-06-02 11:54:42.000000 airtable_view_fetcher-0.1.0/airtable_view_fetcher.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       89 2023-06-02 11:54:42.000000 airtable_view_fetcher-0.1.0/airtable_view_fetcher.egg-info/entry_points.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       14 2023-06-02 11:54:42.000000 airtable_view_fetcher-0.1.0/airtable_view_fetcher.egg-info/requires.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       22 2023-06-02 11:54:42.000000 airtable_view_fetcher-0.1.0/airtable_view_fetcher.egg-info/top_level.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       38 2023-06-02 11:54:42.247986 airtable_view_fetcher-0.1.0/setup.cfg
--rw-rw-r--   0 dev       (1000) dev       (1000)      685 2023-06-02 11:54:37.000000 airtable_view_fetcher-0.1.0/setup.py
+drwxrwxr-x   0 vartur    (1000) vartur    (1000)        0 2023-06-03 13:42:21.126885 airtable_view_fetcher-0.2.0/
+-rw-rw-r--   0 vartur    (1000) vartur    (1000)     1070 2023-06-03 13:14:31.000000 airtable_view_fetcher-0.2.0/LICENSE
+-rw-rw-r--   0 vartur    (1000) vartur    (1000)      370 2023-06-03 13:42:21.126885 airtable_view_fetcher-0.2.0/PKG-INFO
+-rw-rw-r--   0 vartur    (1000) vartur    (1000)     1236 2023-06-03 13:37:01.000000 airtable_view_fetcher-0.2.0/README.md
+drwxrwxr-x   0 vartur    (1000) vartur    (1000)        0 2023-06-03 13:42:21.126885 airtable_view_fetcher-0.2.0/airtable_view_fetcher/
+-rw-rw-r--   0 vartur    (1000) vartur    (1000)        0 2023-06-03 13:14:31.000000 airtable_view_fetcher-0.2.0/airtable_view_fetcher/__init__.py
+-rw-rw-r--   0 vartur    (1000) vartur    (1000)     2538 2023-06-03 13:30:03.000000 airtable_view_fetcher-0.2.0/airtable_view_fetcher/fetch_airtable_data.py
+drwxrwxr-x   0 vartur    (1000) vartur    (1000)        0 2023-06-03 13:42:21.126885 airtable_view_fetcher-0.2.0/airtable_view_fetcher.egg-info/
+-rw-rw-r--   0 vartur    (1000) vartur    (1000)      370 2023-06-03 13:42:21.000000 airtable_view_fetcher-0.2.0/airtable_view_fetcher.egg-info/PKG-INFO
+-rw-rw-r--   0 vartur    (1000) vartur    (1000)      377 2023-06-03 13:42:21.000000 airtable_view_fetcher-0.2.0/airtable_view_fetcher.egg-info/SOURCES.txt
+-rw-rw-r--   0 vartur    (1000) vartur    (1000)        1 2023-06-03 13:42:21.000000 airtable_view_fetcher-0.2.0/airtable_view_fetcher.egg-info/dependency_links.txt
+-rw-rw-r--   0 vartur    (1000) vartur    (1000)       89 2023-06-03 13:42:21.000000 airtable_view_fetcher-0.2.0/airtable_view_fetcher.egg-info/entry_points.txt
+-rw-rw-r--   0 vartur    (1000) vartur    (1000)       14 2023-06-03 13:42:21.000000 airtable_view_fetcher-0.2.0/airtable_view_fetcher.egg-info/requires.txt
+-rw-rw-r--   0 vartur    (1000) vartur    (1000)       22 2023-06-03 13:42:21.000000 airtable_view_fetcher-0.2.0/airtable_view_fetcher.egg-info/top_level.txt
+-rw-rw-r--   0 vartur    (1000) vartur    (1000)       38 2023-06-03 13:42:21.126885 airtable_view_fetcher-0.2.0/setup.cfg
+-rw-rw-r--   0 vartur    (1000) vartur    (1000)      685 2023-06-03 13:34:39.000000 airtable_view_fetcher-0.2.0/setup.py
```

### Comparing `airtable_view_fetcher-0.1.0/LICENSE` & `airtable_view_fetcher-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airtable_view_fetcher-0.1.0/README.md` & `airtable_view_fetcher-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,49 @@
 # Airtable View Fetcher
 
-Airtable View Fetcher is a Python package that allows you to fetch data from Airtable shared views without the need of an API token.
+Airtable View Fetcher is a Python package that allows you to fetch data from Airtable shared views without the need of
+an API token.
 
 ## Installation
 
 You can install the package using pip:
+
 ```bash
-pip install airtable_view_fetcher
+pip install airtable-view-fetcher
 ```
 
 ## Usage
 
 To use Airtable View Fetcher, you can execute it as a command-line tool with the shared view URL as the argument:
+
 ```bash
-airtable_view_fetcher <shared_view_url>
+airtable-view-fetcher <shared_view_url>
 ```
 
-
 Replace `<shared_view_url>` with the URL of the Airtable shared view you want to fetch data from.
 
+To write the output to a JSON file, you can use the following option:
+
+```bash
+airtable-view-fetcher <shared_view_url> -o <output_file_name>
+```
+
+Replace `<output_file_name>` with the name of the output JSON file
+
 ## Requirements
 
 Airtable View Fetcher requires the following dependencies:
 
 - Python 3.8+
 - requests
 - pytz
 
 ## Contributing
 
-Contributions to Airtable View Fetcher are welcome! If you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request on the [GitHub repository](https://github.com/vartur/airtable_view_fetcher).
+Contributions to Airtable View Fetcher are welcome! If you encounter any issues or have suggestions for improvements,
+please feel free to open an issue or submit a pull request on
+the [GitHub repository](https://github.com/vartur/airtable_view_fetcher).
 
 ## License
 
 This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `airtable_view_fetcher-0.1.0/setup.py` & `airtable_view_fetcher-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='airtable_view_fetcher',
-    version='0.1.0',
+    version='0.2.0',
     description='Tool to scrape data from an Airtable shared view',
     url='https://github.com/vartur/airtable_view_fetcher',
     author='Vincent Artur',
     author_email='6145191+vartur@users.noreply.github.com',
     packages=['airtable_view_fetcher'],
     install_requires=[
         'requests',
```

