# Comparing `tmp/phone_gen-2.3.0.tar.gz` & `tmp/phone_gen-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phone_gen-2.3.0.tar", last modified: Tue May 23 15:16:38 2023, max compression
+gzip compressed data, was "phone_gen-2.3.1.tar", last modified: Sat Jun  3 11:58:29 2023, max compression
```

## Comparing `phone_gen-2.3.0.tar` & `phone_gen-2.3.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:16:38.700802 phone_gen-2.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:16:38.684802 phone_gen-2.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:16:38.692802 phone_gen-2.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-23 15:16:22.000000 phone_gen-2.3.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-23 15:16:22.000000 phone_gen-2.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-23 15:16:22.000000 phone_gen-2.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-23 15:16:22.000000 phone_gen-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-23 15:16:38.700802 phone_gen-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-23 15:16:22.000000 phone_gen-2.3.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-23 15:16:22.000000 phone_gen-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:16:38.692802 phone_gen-2.3.0/dev_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-05-23 15:16:22.000000 phone_gen-2.3.0/dev_tools/patterns_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-23 15:16:22.000000 phone_gen-2.3.0/dev_tools/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:16:38.696802 phone_gen-2.3.0/phone_gen/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-23 15:16:22.000000 phone_gen-2.3.0/phone_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 15:16:38.000000 phone_gen-2.3.0/phone_gen/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-05-23 15:16:22.000000 phone_gen-2.3.0/phone_gen/_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-23 15:16:22.000000 phone_gen-2.3.0/phone_gen/alt_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-23 15:16:22.000000 phone_gen-2.3.0/phone_gen/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-05-23 15:16:22.000000 phone_gen-2.3.0/phone_gen/country_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-05-23 15:16:22.000000 phone_gen-2.3.0/phone_gen/iso3.py
--rw-r--r--   0 runner    (1001) docker     (123)    87966 2023-05-23 15:16:22.000000 phone_gen-2.3.0/phone_gen/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:16:38.696802 phone_gen-2.3.0/phone_gen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-23 15:16:38.000000 phone_gen-2.3.0/phone_gen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-23 15:16:38.000000 phone_gen-2.3.0/phone_gen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:16:38.000000 phone_gen-2.3.0/phone_gen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-23 15:16:38.000000 phone_gen-2.3.0/phone_gen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 15:16:38.000000 phone_gen-2.3.0/phone_gen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-23 15:16:38.700802 phone_gen-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-23 15:16:22.000000 phone_gen-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:16:38.700802 phone_gen-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-23 15:16:22.000000 phone_gen-2.3.0/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-23 15:16:22.000000 phone_gen-2.3.0/tests/test_alt_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-23 15:16:22.000000 phone_gen-2.3.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-23 15:16:22.000000 phone_gen-2.3.0/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-23 15:16:22.000000 phone_gen-2.3.0/tests/test_load_alt_patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-23 15:16:22.000000 phone_gen-2.3.0/tests/test_phone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:58:29.720630 phone_gen-2.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:58:29.716630 phone_gen-2.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:58:29.720630 phone_gen-2.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-03 11:58:13.000000 phone_gen-2.3.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-03 11:58:13.000000 phone_gen-2.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-03 11:58:13.000000 phone_gen-2.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-03 11:58:13.000000 phone_gen-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-03 11:58:29.720630 phone_gen-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-03 11:58:13.000000 phone_gen-2.3.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-03 11:58:13.000000 phone_gen-2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:58:29.720630 phone_gen-2.3.1/dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-03 11:58:13.000000 phone_gen-2.3.1/dev_tools/patterns_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-03 11:58:13.000000 phone_gen-2.3.1/dev_tools/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:58:29.720630 phone_gen-2.3.1/phone_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-03 11:58:13.000000 phone_gen-2.3.1/phone_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-03 11:58:29.000000 phone_gen-2.3.1/phone_gen/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-06-03 11:58:13.000000 phone_gen-2.3.1/phone_gen/_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-03 11:58:13.000000 phone_gen-2.3.1/phone_gen/alt_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-03 11:58:13.000000 phone_gen-2.3.1/phone_gen/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16602 2023-06-03 11:58:13.000000 phone_gen-2.3.1/phone_gen/country_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-03 11:58:13.000000 phone_gen-2.3.1/phone_gen/iso3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87915 2023-06-03 11:58:13.000000 phone_gen-2.3.1/phone_gen/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:58:29.720630 phone_gen-2.3.1/phone_gen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-03 11:58:29.000000 phone_gen-2.3.1/phone_gen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-03 11:58:29.000000 phone_gen-2.3.1/phone_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 11:58:29.000000 phone_gen-2.3.1/phone_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-03 11:58:29.000000 phone_gen-2.3.1/phone_gen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-03 11:58:29.000000 phone_gen-2.3.1/phone_gen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-03 11:58:29.724630 phone_gen-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-03 11:58:13.000000 phone_gen-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 11:58:29.720630 phone_gen-2.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-03 11:58:13.000000 phone_gen-2.3.1/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-03 11:58:13.000000 phone_gen-2.3.1/tests/test_alt_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-03 11:58:13.000000 phone_gen-2.3.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-03 11:58:13.000000 phone_gen-2.3.1/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-03 11:58:13.000000 phone_gen-2.3.1/tests/test_load_alt_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-03 11:58:13.000000 phone_gen-2.3.1/tests/test_phone.py
```

### Comparing `phone_gen-2.3.0/.github/workflows/python-package.yml` & `phone_gen-2.3.1/.github/workflows/python-package.yml`

 * *Files 13% similar despite different names*

```diff
@@ -21,18 +21,18 @@
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install flake8 pep8-naming pytest black pytest-cov phonenumbers==8.13.11
+          python -m pip install flake8 pep8-naming pytest black pytest-cov phonenumbers==8.13.13
           python -m pip install -e .
       - name: Flake8
         run: |
           flake8 phone_gen
       - name: Black
         run: |
           black --check phone_gen
       - name: Test with pytest
         run: |
-          pytest -m "not phonenumbers" tests
+          pytest tests
```

### Comparing `phone_gen-2.3.0/.github/workflows/python-publish.yml` & `phone_gen-2.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.0/.gitignore` & `phone_gen-2.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.0/LICENSE` & `phone_gen-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.0/PKG-INFO` & `phone_gen-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phone_gen
-Version: 2.3.0
+Version: 2.3.1
 Summary: International phone number generation
 Home-page: https://github.com/tolstislon/phone-gen
 Author: tolstislon
 Author-email: tolstislon@gmail.com
 License: MIT License
 Keywords: testing,test-data,phone-number,phone,test-data-generator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `phone_gen-2.3.0/README.md` & `phone_gen-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.0/dev_tools/patterns_generator.py` & `phone_gen-2.3.1/dev_tools/patterns_generator.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.0/dev_tools/update.py` & `phone_gen-2.3.1/dev_tools/update.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.0/phone_gen/__init__.py` & `phone_gen-2.3.1/phone_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.0/phone_gen/_generator.py` & `phone_gen-2.3.1/phone_gen/_generator.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.0/phone_gen/alt_patterns.py` & `phone_gen-2.3.1/phone_gen/alt_patterns.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.0/phone_gen/cli.py` & `phone_gen-2.3.1/phone_gen/cli.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.0/phone_gen/country_name.py` & `phone_gen-2.3.1/phone_gen/country_name.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.0/phone_gen/iso3.py` & `phone_gen-2.3.1/phone_gen/iso3.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.0/phone_gen/patterns.py` & `phone_gen-2.3.1/phone_gen/patterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 """
-Auto-generated file 2023-05-23 15:07:18 UTC
-Resource: https://github.com/google/libphonenumber v8.13.12
+Auto-generated file 2023-06-03 11:49:59 UTC
+Resource: https://github.com/google/libphonenumber v8.13.13
 """
 
 
 PATTERNS = {
-    "info": "libphonenumber v8.13.12",
+    "info": "libphonenumber v8.13.13",
     "data": {
         "AC": {
             "code": "247",
             "pattern": "((6[2-467][\\d]{3}))",
             "mobile": "((4[\\d]{4}))",
         },
         "AD": {
@@ -67,15 +67,15 @@
             "code": "43",
             "pattern": "((1(11[\\d])|([2-9][\\d]{3:11}))|((316)|(463)|((51)|(66)|(73)2)[\\d]{3:10})|((2(1[467])|(2[13-8])|(5[2357])|(6[1-46-8])|(7[1-8])|(8[124-7])|(9[1458]))|(3(1[1-578])|(3[23568])|(4[5-7])|(5[1378])|(6[1-38])|(8[3-68]))|(4(2[1-8])|(35)|(7[1368])|(8[2457]))|(5(2[1-8])|(3[357])|(4[147])|(5[12578])|(6[37]))|(6(13)|(2[1-47])|(4[135-8])|(5[468]))|(7(2[1-8])|(35)|(4[13478])|(5[68])|(6[16-8])|(7[1-6])|(9[45]))[\\d]{4:10}))",
             "mobile": "((6(5[0-3579])|(6[013-9])|([7-9][\\d])[\\d]{4:10}))",
         },
         "AU": {
             "code": "61",
             "pattern": "((((2([0-26-9][\\d])|(3[0-8])|(4[02-9])|(5[0135-9]))|(3([0-3589][\\d])|(4[0-578])|(6[1-9])|(7[0-35-9]))|(7([013-57-9][\\d])|(2[0-8]))[\\d]{3})|(8(51(0(0[03-9])|([12479][\\d])|(3[2-9])|(5[0-8])|(6[1-9])|(8[0-7]))|(1([0235689][\\d])|(1[0-69])|(4[0-589])|(7[0-47-9]))|(2(0[0-79])|([18][13579])|(2[14-9])|(3[0-46-9])|([4-6][\\d])|(7[89])|(9[0-4])))|((6[0-8])|([78][\\d])[\\d]{3})|(9([02-9][\\d]{3})|(1(([0-58][\\d])|(6[0135-9])[\\d])|(7(0[0-24-9])|([1-9][\\d]))|(9([0-46-9][\\d])|(5[0-79])))))[\\d]{3}))",
-            "mobile": "((4(79[01])|(83[0-389])|(93[0-6])[\\d]{5})|(4([0-3][\\d])|(4[047-9])|(5[0-25-9])|(6[016-9])|(7[02-8])|(8[0-24-9])|(9[0-27-9])[\\d]{6}))",
+            "mobile": "((4((79)|(94)[01])|(83[0-389])[\\d]{5})|(4([0-3][\\d])|(4[047-9])|(5[0-25-9])|(6[016-9])|(7[02-8])|(8[0-24-9])|(9[0-37-9])[\\d]{6}))",
         },
         "AW": {
             "code": "297",
             "pattern": "((5(2[\\d])|(8[1-9])[\\d]{4}))",
             "mobile": "(((290)|(5[69][\\d])|(6([03]0)|(22)|(4[0-2])|([69][\\d]))|(7([34][\\d])|(7[07]))|(9(6[45])|(9[4-8]))[\\d]{4}))",
         },
         "AX": {
@@ -127,15 +127,15 @@
             "code": "257",
             "pattern": "(((22)|(31)[\\d]{6}))",
             "mobile": "(((29)|([67][125-9])[\\d]{6}))",
         },
         "BJ": {
             "code": "229",
             "pattern": "((2(02)|(1[037])|(2[45])|(3[68])|(4[\\d])[\\d]{5}))",
-            "mobile": "(((4[0-256])|([56][\\d])|(9[013-9])[\\d]{6}))",
+            "mobile": "(((4[0-356])|([56][\\d])|(9[013-9])[\\d]{6}))",
         },
         "BL": {
             "code": "590",
             "pattern": "((590(2[7-9])|(5[12])|(87)[\\d]{4}))",
             "mobile": "((69(0[\\d][\\d])|(1(2[2-9])|(3[0-5]))[\\d]{4}))",
         },
         "BM": {
@@ -192,15 +192,15 @@
             "code": "1",
             "pattern": "(((2(04)|([23]6)|([48]9)|(50)|(63))|(3(06)|(43)|(54)|(6[578])|(82))|(4(03)|(1[68])|([26]8)|(3[178])|(50)|(74))|(5(06)|(1[49])|(48)|(79)|(8[147]))|(6(04)|([18]3)|(39)|(47)|(72))|(7(0[59])|(42)|(53)|(78)|(8[02]))|(8([06]7)|(19)|(25)|(73))|(90[25])[2-9][\\d]{6}))",
             "mobile": "(((2(04)|([23]6)|([48]9)|(50)|(63))|(3(06)|(43)|(54)|(6[578])|(82))|(4(03)|(1[68])|([26]8)|(3[178])|(50)|(74))|(5(06)|(1[49])|(48)|(79)|(8[147]))|(6(04)|([18]3)|(39)|(47)|(72))|(7(0[59])|(42)|(53)|(78)|(8[02]))|(8([06]7)|(19)|(25)|(73))|(90[25])[2-9][\\d]{6}))",
         },
         "CC": {
             "code": "61",
             "pattern": "((8(51(0(02)|(31)|(60)|(89))|(1(18)|(76))|(223))|(91(0(1[0-2])|(29))|(1([28]2)|(50)|(79))|(2(10)|(64))|(3([06]8)|(22))|(4[29]8)|(62[\\d])|(70[23])|(959))[\\d]{3}))",
-            "mobile": "((4(79[01])|(83[0-389])|(93[0-6])[\\d]{5})|(4([0-3][\\d])|(4[047-9])|(5[0-25-9])|(6[016-9])|(7[02-8])|(8[0-24-9])|(9[0-27-9])[\\d]{6}))",
+            "mobile": "((4((79)|(94)[01])|(83[0-389])[\\d]{5})|(4([0-3][\\d])|(4[047-9])|(5[0-25-9])|(6[016-9])|(7[02-8])|(8[0-24-9])|(9[0-37-9])[\\d]{6}))",
         },
         "CD": {
             "code": "243",
             "pattern": "((12[\\d]{7})|([1-6][\\d]{6}))",
             "mobile": "((88[\\d]{5})|((8[0-59])|(9[017-9])[\\d]{7}))",
         },
         "CF": {
@@ -267,15 +267,15 @@
             "code": "599",
             "pattern": "((9(4(3[0-5])|(4[14])|(6[\\d]))|(50[\\d])|(7(2[014])|(3[02-9])|(4[4-9])|(6[357])|(77)|(8[7-9]))|(8(3[39])|([46][\\d])|(7[01])|(8[57-9]))[\\d]{4}))",
             "mobile": "((953[01][\\d]{4})|(9(5[12467])|(6[5-9])[\\d]{5}))",
         },
         "CX": {
             "code": "61",
             "pattern": "((8(51(0(01)|(30)|(59)|(88))|(1(17)|(46)|(75))|(2(22)|(35)))|(91(00[6-9])|(1([28]1)|(49)|(78))|(2(09)|(63))|(3(12)|(26)|(75))|(4(56)|(97))|(64[\\d])|(7(0[01])|(1[0-2]))|(958))[\\d]{3}))",
-            "mobile": "((4(79[01])|(83[0-389])|(93[0-6])[\\d]{5})|(4([0-3][\\d])|(4[047-9])|(5[0-25-9])|(6[016-9])|(7[02-8])|(8[0-24-9])|(9[0-27-9])[\\d]{6}))",
+            "mobile": "((4((79)|(94)[01])|(83[0-389])[\\d]{5})|(4([0-3][\\d])|(4[047-9])|(5[0-25-9])|(6[016-9])|(7[02-8])|(8[0-24-9])|(9[0-37-9])[\\d]{6}))",
         },
         "CY": {
             "code": "357",
             "pattern": "((2[2-6][\\d]{6}))",
             "mobile": "((9(10)|([4-79][\\d])[\\d]{5}))",
         },
         "CZ": {
@@ -381,15 +381,15 @@
         "GA": {
             "code": "241",
             "pattern": "(([01]1[\\d]{6}))",
             "mobile": "((((0[2-7])|(7[467])[\\d])|(6(0[0-4])|(10)|([256][\\d]))[\\d]{5})|([2-7][\\d]{6}))",
         },
         "GB": {
             "code": "44",
-            "pattern": "(((1(1(3([0-58][\\d][\\d])|(73[0235]))|(4([0-5][\\d][\\d])|(69[7-9])|(70[0-579]))|(((5[0-26-9])|([78][0-49])[\\d])|(6([0-4][\\d])|(50))[\\d]))|(2((0[024-9])|(2[3-9])|(3[3-79])|(4[1-689])|([58][02-9])|(6[0-47-9])|(7[013-9])|(9[\\d])[\\d][\\d])|(1([0-7][\\d][\\d])|(8([02][\\d])|(1[0-46-9]))))|((3(0[\\d])|(1[0-8])|([25][02-9])|(3[02-579])|([468][0-46-9])|(7[1-35-79])|(9[2-578]))|(4(0[03-9])|([137][\\d])|([28][02-57-9])|(4[02-69])|(5[0-8])|([69][0-79]))|(5(0[1-35-9])|([16][\\d])|(2[024-9])|(3[015689])|(4[02-9])|(5[03-9])|(7[0-35-9])|(8[0-468])|(9[0-57-9]))|(6(0[034689])|(1[\\d])|(2[0-35689])|([38][013-9])|(4[1-467])|(5[0-69])|(6[13-9])|(7[0-8])|(9[0-24578]))|(7(0[0246-9])|(2[\\d])|(3[0236-8])|(4[03-9])|(5[0-46-9])|(6[013-9])|(7[0-35-9])|(8[024-9])|(9[02-9]))|(8(0[35-9])|(2[1-57-9])|(3[02-578])|(4[0-578])|(5[124-9])|(6[2-69])|(7[\\d])|(8[02-9])|(9[02569]))|(9(0[02-589])|([18][\\d])|(2[02-689])|(3[1-57-9])|(4[2-9])|(5[0-579])|(6[2-47-9])|(7[0-24578])|(9[2-57]))[\\d][\\d]))|(2(0[013478])|(3[0189])|(4[017])|(8[0-46-9])|(9[0-2])[\\d]{3})[\\d]{4})|(1(2(0(46[1-4])|(87[2-9]))|(545[1-79])|(76(2[\\d])|(3[1-8])|(6[1-6]))|(9(7(2[0-4])|(3[2-5]))|(8(2[2-8])|(7[0-47-9])|(8[3-5]))))|(3(6(38[2-5])|(47[23]))|(8(47[04-9])|(64[0157-9])))|(4(044[1-7])|(20(2[23])|(8[\\d]))|(6(0(30)|(5[2-57])|(6[1-8])|(7[2-8]))|(140))|(8(052)|(87[1-3])))|(5(2(4(3[2-79])|(6[\\d]))|(76[\\d]))|(6(26[06-9])|(686)))|(6(06(4[\\d])|(7[4-79]))|(295[5-7])|(35[34][\\d])|(47(24)|(61))|(59(5[08])|(6[67])|(74))|(9(55[0-4])|(77[23])))|(7(26(6[13-9])|(7[0-7]))|((442)|(688)[\\d])|(50(2[0-3])|([3-68]2)|(76)))|(8(27[56][\\d])|(37(5[2-5])|(8[239]))|(843[2-58]))|(9(0(0(6[1-8])|(85))|(52[\\d]))|(3583)|(4(66[1-8])|(9(2[01])|(81)))|(63(23)|(3[1-4]))|(9561))[\\d]{3}))",
+            "pattern": "(((1(1(3([0-58][\\d][\\d])|(73[0235]))|(4([0-5][\\d][\\d])|(69[7-9])|(70[0-579]))|(((5[0-26-9])|([78][0-49])[\\d])|(6([0-4][\\d])|(50))[\\d]))|((2((0[024-9])|(2[3-9])|(3[3-79])|(4[1-689])|([58][02-9])|(6[0-47-9])|(7[013-9])|(9[\\d])[\\d])|(1([0-7][\\d])|(8[0-2])))|((3(0[\\d])|(1[0-8])|([25][02-9])|(3[02-579])|([468][0-46-9])|(7[1-35-79])|(9[2-578]))|(4(0[03-9])|([137][\\d])|([28][02-57-9])|(4[02-69])|(5[0-8])|([69][0-79]))|(5(0[1-35-9])|([16][\\d])|(2[024-9])|(3[015689])|(4[02-9])|(5[03-9])|(7[0-35-9])|(8[0-468])|(9[0-57-9]))|(6(0[034689])|(1[\\d])|(2[0-35689])|([38][013-9])|(4[1-467])|(5[0-69])|(6[13-9])|(7[0-8])|(9[0-24578]))|(7(0[0246-9])|(2[\\d])|(3[0236-8])|(4[03-9])|(5[0-46-9])|(6[013-9])|(7[0-35-9])|(8[024-9])|(9[02-9]))|(8(0[35-9])|(2[1-57-9])|(3[02-578])|(4[0-578])|(5[124-9])|(6[2-69])|(7[\\d])|(8[02-9])|(9[02569]))|(9(0[02-589])|([18][\\d])|(2[02-689])|(3[1-57-9])|(4[2-9])|(5[0-579])|(6[2-47-9])|(7[0-24578])|(9[2-57]))[\\d])[\\d]))|(2(0[013478])|(3[0189])|(4[017])|(8[0-46-9])|(9[0-2])[\\d]{3})[\\d]{4})|(1(2(0(46[1-4])|(87[2-9]))|(545[1-79])|(76(2[\\d])|(3[1-8])|(6[1-6]))|(9(7(2[0-4])|(3[2-5]))|(8(2[2-8])|(7[0-47-9])|(8[3-5]))))|(3(6(38[2-5])|(47[23]))|(8(47[04-9])|(64[0157-9])))|(4(044[1-7])|(20(2[23])|(8[\\d]))|(6(0(30)|(5[2-57])|(6[1-8])|(7[2-8]))|(140))|(8(052)|(87[1-3])))|(5(2(4(3[2-79])|(6[\\d]))|(76[\\d]))|(6(26[06-9])|(686)))|(6(06(4[\\d])|(7[4-79]))|(295[5-7])|(35[34][\\d])|(47(24)|(61))|(59(5[08])|(6[67])|(74))|(9(55[0-4])|(77[23])))|(7(26(6[13-9])|(7[0-7]))|((442)|(688)[\\d])|(50(2[0-3])|([3-68]2)|(76)))|(8(27[56][\\d])|(37(5[2-5])|(8[239]))|(843[2-58]))|(9(0(0(6[1-8])|(85))|(52[\\d]))|(3583)|(4(66[1-8])|(9(2[01])|(81)))|(63(23)|(3[1-4]))|(9561))[\\d]{3}))",
             "mobile": "((7(457[0-57-9])|(700[01])|(911[028])[\\d]{5})|(7([1-3][\\d][\\d])|(4([0-46-9][\\d])|(5[0-689]))|(5(0[0-8])|([13-9][\\d])|(2[0-35-9]))|(7(0[1-9])|([1-7][\\d])|(8[02-9])|(9[0-689]))|(8([014-9][\\d])|([23][0-8]))|(9([024-9][\\d])|(1[02-9])|(3[0-689]))[\\d]{6}))",
         },
         "GD": {
             "code": "1",
             "pattern": "((473(2(3[0-2])|(69))|(3(2[89])|(86))|(4([06]8)|(3[5-9])|(4[0-49])|(5[5-79])|(73)|(90))|(63[68])|(7(58)|(84))|(800)|(938)[\\d]{4}))",
             "mobile": "((473(4(0[2-79])|(1[04-9])|(2[0-5])|(58))|(5(2[01])|(3[3-8]))|(901)[\\d]{4}))",
         },
@@ -637,15 +637,15 @@
         "LK": {
             "code": "94",
             "pattern": "(((12[2-9])|(602)|(8[12][\\d])|(9(1[\\d])|(22)|(9[245]))[\\d]{6})|((11)|(2[13-7])|(3[1-8])|(4[157])|(5[12457])|(6[35-7])[2-57][\\d]{6}))",
             "mobile": "((7([0-25-8][\\d])|(4[0-4])[\\d]{6}))",
         },
         "LR": {
             "code": "231",
-            "pattern": "(((2[\\d]{3})|(33333)[\\d]{4}))",
+            "pattern": "((2[\\d]{7}))",
             "mobile": "(((((22)|(33)0)|(555)|((77)|(88)[\\d])[\\d])|(4[67])[\\d]{5})|([56][\\d]{6}))",
         },
         "LS": {"code": "266", "pattern": "((2[\\d]{7}))", "mobile": "(([56][\\d]{7}))"},
         "LT": {
             "code": "370",
             "pattern": "(((3[1478])|(4[124-6])|(52)[\\d]{6}))",
             "mobile": "((6[\\d]{7}))",
@@ -749,15 +749,15 @@
             "code": "356",
             "pattern": "((20(3[1-4])|(6[059])[\\d]{4})|(2(0[19])|([1-357][\\d])|(60)[\\d]{5}))",
             "mobile": "(((7(210)|([79][\\d][\\d]))|(9([29][\\d][\\d])|(69[67])|(8(1[1-3])|(89)|(97)))[\\d]{4}))",
         },
         "MU": {
             "code": "230",
             "pattern": "(((2([0346-8][\\d])|(1[0-7]))|(4([013568][\\d])|(2[4-7]))|(54([3-5][\\d])|(71))|(6[\\d][\\d])|(8(14)|(3[129]))[\\d]{4}))",
-            "mobile": "((5(4(2[1-389])|(7[1-9]))|(87[15-8])[\\d]{4})|((5(2[5-9])|(4[3-689])|([57][\\d])|(8[0-689])|(9[0-8]))|(7(0[01])|(3[03]))[\\d]{5}))",
+            "mobile": "((5(4(2[1-389])|(7[1-9]))|(87[15-8])[\\d]{4})|((5(2[5-9])|(4[3-689])|([57][\\d])|(8[0-689])|(9[0-8]))|(7(0[0-2])|(3[013]))[\\d]{5}))",
         },
         "MV": {
             "code": "960",
             "pattern": "(((3(0[0-3])|(3[0-59]))|(6([58][024689])|(6[024-68])|(7[02468]))[\\d]{4}))",
             "mobile": "(((46[46])|([79][\\d][\\d])[\\d]{4}))",
         },
         "MW": {
```

### Comparing `phone_gen-2.3.0/phone_gen.egg-info/PKG-INFO` & `phone_gen-2.3.1/phone_gen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phone-gen
-Version: 2.3.0
+Version: 2.3.1
 Summary: International phone number generation
 Home-page: https://github.com/tolstislon/phone-gen
 Author: tolstislon
 Author-email: tolstislon@gmail.com
 License: MIT License
 Keywords: testing,test-data,phone-number,phone,test-data-generator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `phone_gen-2.3.0/phone_gen.egg-info/SOURCES.txt` & `phone_gen-2.3.1/phone_gen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.0/setup.py` & `phone_gen-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.0/tests/test_alt_pattern.py` & `phone_gen-2.3.1/tests/test_alt_pattern.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.0/tests/test_cli.py` & `phone_gen-2.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.0/tests/test_generator.py` & `phone_gen-2.3.1/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.0/tests/test_load_alt_patterns.py` & `phone_gen-2.3.1/tests/test_load_alt_patterns.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.3.0/tests/test_phone.py` & `phone_gen-2.3.1/tests/test_phone.py`

 * *Files identical despite different names*

