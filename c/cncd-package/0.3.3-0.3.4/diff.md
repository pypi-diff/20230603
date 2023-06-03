# Comparing `tmp/cncd_package-0.3.3.tar.gz` & `tmp/cncd_package-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cncd_package-0.3.3.tar", last modified: Sat Jun  3 07:59:14 2023, max compression
+gzip compressed data, was "cncd_package-0.3.4.tar", last modified: Sat Jun  3 09:06:01 2023, max compression
```

## Comparing `cncd_package-0.3.3.tar` & `cncd_package-0.3.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 07:59:14.572418 cncd_package-0.3.3/
--rw-rw-rw-   0        0        0    10336 2023-06-03 07:59:14.572418 cncd_package-0.3.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 07:59:14.556794 cncd_package-0.3.3/cncd_package/
--rw-rw-rw-   0        0        0    29722 2023-06-03 07:15:35.000000 cncd_package-0.3.3/cncd_package/QC.py
--rw-rw-rw-   0        0        0        0 2023-05-31 11:15:28.000000 cncd_package-0.3.3/cncd_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 07:59:14.572418 cncd_package-0.3.3/cncd_package.egg-info/
--rw-rw-rw-   0        0        0    10336 2023-06-03 07:59:14.000000 cncd_package-0.3.3/cncd_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-06-03 07:59:14.000000 cncd_package-0.3.3/cncd_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 07:59:14.000000 cncd_package-0.3.3/cncd_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-03 07:59:14.000000 cncd_package-0.3.3/cncd_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-03 07:59:14.000000 cncd_package-0.3.3/cncd_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 07:59:14.572418 cncd_package-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1388 2023-06-03 07:58:09.000000 cncd_package-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 09:06:01.532954 cncd_package-0.3.4/
+-rw-rw-rw-   0        0        0     9376 2023-06-03 09:06:01.532954 cncd_package-0.3.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 09:06:01.517329 cncd_package-0.3.4/cncd_package/
+-rw-rw-rw-   0        0        0    29722 2023-06-03 07:15:35.000000 cncd_package-0.3.4/cncd_package/QC.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 11:15:28.000000 cncd_package-0.3.4/cncd_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 09:06:01.532954 cncd_package-0.3.4/cncd_package.egg-info/
+-rw-rw-rw-   0        0        0     9376 2023-06-03 09:06:01.000000 cncd_package-0.3.4/cncd_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-06-03 09:06:01.000000 cncd_package-0.3.4/cncd_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 09:06:01.000000 cncd_package-0.3.4/cncd_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-03 09:06:01.000000 cncd_package-0.3.4/cncd_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-03 09:06:01.000000 cncd_package-0.3.4/cncd_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 09:06:01.532954 cncd_package-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1388 2023-06-03 09:05:27.000000 cncd_package-0.3.4/setup.py
```

### Comparing `cncd_package-0.3.3/PKG-INFO` & `cncd_package-0.3.4/cncd_package.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cncd_package
-Version: 0.3.3
+Name: cncd-package
+Version: 0.3.4
 Summary: A Python package for CNCD
 Home-page: https://github.com/shahzaib-raza/cncd
 Author: Shahzaib Raza
 Author-email: shahzaib.raza@cncd.org
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -68,27 +68,15 @@
 qc.age_check().head()
 ```
 
 
 
 
 <div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-</style>
+
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>study_id</th>
       <th>name</th>
       <th>age</th>
@@ -138,27 +126,15 @@
 qc.gender_check(gender='male')
 ```
 
 
 
 
 <div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-</style>
+
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>study_id</th>
       <th>name</th>
       <th>gender</th>
@@ -255,27 +231,15 @@
 qc.gender_check(gender='female')
 ```
 
 
 
 
 <div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-</style>
+
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>study_id</th>
       <th>name</th>
       <th>gender</th>
@@ -374,27 +338,15 @@
 qc.check_qc_status()
 ```
 
 
 
 
 <div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-</style>
+
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>study_id</th>
       <th>status</th>
       <th>mi</th>
```

### Comparing `cncd_package-0.3.3/cncd_package/QC.py` & `cncd_package-0.3.4/cncd_package/QC.py`

 * *Files identical despite different names*

### Comparing `cncd_package-0.3.3/cncd_package.egg-info/PKG-INFO` & `cncd_package-0.3.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cncd-package
-Version: 0.3.3
+Name: cncd_package
+Version: 0.3.4
 Summary: A Python package for CNCD
 Home-page: https://github.com/shahzaib-raza/cncd
 Author: Shahzaib Raza
 Author-email: shahzaib.raza@cncd.org
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -68,27 +68,15 @@
 qc.age_check().head()
 ```
 
 
 
 
 <div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-</style>
+
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>study_id</th>
       <th>name</th>
       <th>age</th>
@@ -138,27 +126,15 @@
 qc.gender_check(gender='male')
 ```
 
 
 
 
 <div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-</style>
+
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>study_id</th>
       <th>name</th>
       <th>gender</th>
@@ -255,27 +231,15 @@
 qc.gender_check(gender='female')
 ```
 
 
 
 
 <div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-</style>
+
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>study_id</th>
       <th>name</th>
       <th>gender</th>
@@ -374,27 +338,15 @@
 qc.check_qc_status()
 ```
 
 
 
 
 <div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-</style>
+
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>study_id</th>
       <th>status</th>
       <th>mi</th>
```

### Comparing `cncd_package-0.3.3/setup.py` & `cncd_package-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path("README.md").parent
 long_desc = (this_directory / "README.md").read_text()
 
 setup(
     name='cncd_package',
-    version='0.3.3',    
+    version='0.3.4',    
     description='A Python package for CNCD',
     long_description=long_desc,
     long_description_content_type='text/markdown',
     url='https://github.com/shahzaib-raza/cncd',
     author='Shahzaib Raza',
     author_email='shahzaib.raza@cncd.org',
     license='BSD 2-clause',
```

