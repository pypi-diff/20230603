# Comparing `tmp/kkexcel-0.1.6.tar.gz` & `tmp/kkexcel-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kkexcel-0.1.6.tar", last modified: Sun Jul 17 16:54:02 2022, max compression
+gzip compressed data, was "dist/kkexcel-0.1.7.tar", last modified: Sat Jun  3 12:20:15 2023, max compression
```

## Comparing `kkexcel-0.1.6.tar` & `kkexcel-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vekair     (502) staff       (20)        0 2022-07-17 16:54:02.000000 kkexcel-0.1.6/
--rw-r--r--   0 vekair     (502) staff       (20)      230 2022-07-17 16:54:02.000000 kkexcel-0.1.6/PKG-INFO
--rw-r--r--   0 vekair     (502) staff       (20)      501 2021-10-27 08:52:59.000000 kkexcel-0.1.6/README.md
-drwxr-xr-x   0 vekair     (502) staff       (20)        0 2022-07-17 16:54:02.000000 kkexcel-0.1.6/kkexcel/
--rw-r--r--   0 vekair     (502) staff       (20)      113 2022-07-17 16:04:31.000000 kkexcel-0.1.6/kkexcel/__init__.py
--rw-r--r--   0 vekair     (502) staff       (20)     1279 2022-07-17 15:54:23.000000 kkexcel-0.1.6/kkexcel/generate_excel.py
-drwxr-xr-x   0 vekair     (502) staff       (20)        0 2022-07-17 16:54:02.000000 kkexcel-0.1.6/kkexcel.egg-info/
--rw-r--r--   0 vekair     (502) staff       (20)      230 2022-07-17 16:54:01.000000 kkexcel-0.1.6/kkexcel.egg-info/PKG-INFO
--rw-r--r--   0 vekair     (502) staff       (20)      218 2022-07-17 16:54:02.000000 kkexcel-0.1.6/kkexcel.egg-info/SOURCES.txt
--rw-r--r--   0 vekair     (502) staff       (20)        1 2022-07-17 16:54:02.000000 kkexcel-0.1.6/kkexcel.egg-info/dependency_links.txt
--rw-r--r--   0 vekair     (502) staff       (20)       11 2022-07-17 16:54:02.000000 kkexcel-0.1.6/kkexcel.egg-info/requires.txt
--rw-r--r--   0 vekair     (502) staff       (20)        8 2022-07-17 16:54:02.000000 kkexcel-0.1.6/kkexcel.egg-info/top_level.txt
--rw-r--r--   0 vekair     (502) staff       (20)       38 2022-07-17 16:54:02.000000 kkexcel-0.1.6/setup.cfg
--rw-r--r--   0 vekair     (502) staff       (20)      454 2022-07-17 16:53:29.000000 kkexcel-0.1.6/setup.py
+drwxr-xr-x   0 vekair     (502) staff       (20)        0 2023-06-03 12:20:15.670774 kkexcel-0.1.7/
+-rw-r--r--   0 vekair     (502) staff       (20)      212 2023-06-03 12:20:15.670477 kkexcel-0.1.7/PKG-INFO
+-rw-r--r--   0 vekair     (502) staff       (20)       80 2023-06-03 12:05:48.000000 kkexcel-0.1.7/README.md
+drwxr-xr-x   0 vekair     (502) staff       (20)        0 2023-06-03 12:20:15.667869 kkexcel-0.1.7/kkexcel/
+-rw-r--r--   0 vekair     (502) staff       (20)      113 2023-06-03 12:05:48.000000 kkexcel-0.1.7/kkexcel/__init__.py
+-rw-r--r--   0 vekair     (502) staff       (20)     1325 2023-06-03 12:07:07.000000 kkexcel-0.1.7/kkexcel/generate_excel.py
+drwxr-xr-x   0 vekair     (502) staff       (20)        0 2023-06-03 12:20:15.669986 kkexcel-0.1.7/kkexcel.egg-info/
+-rw-r--r--   0 vekair     (502) staff       (20)      212 2023-06-03 12:20:15.000000 kkexcel-0.1.7/kkexcel.egg-info/PKG-INFO
+-rw-r--r--   0 vekair     (502) staff       (20)      218 2023-06-03 12:20:15.000000 kkexcel-0.1.7/kkexcel.egg-info/SOURCES.txt
+-rw-r--r--   0 vekair     (502) staff       (20)        1 2023-06-03 12:20:15.000000 kkexcel-0.1.7/kkexcel.egg-info/dependency_links.txt
+-rw-r--r--   0 vekair     (502) staff       (20)       11 2023-06-03 12:20:15.000000 kkexcel-0.1.7/kkexcel.egg-info/requires.txt
+-rw-r--r--   0 vekair     (502) staff       (20)        8 2023-06-03 12:20:15.000000 kkexcel-0.1.7/kkexcel.egg-info/top_level.txt
+-rw-r--r--   0 vekair     (502) staff       (20)       38 2023-06-03 12:20:15.670916 kkexcel-0.1.7/setup.cfg
+-rw-r--r--   0 vekair     (502) staff       (20)      648 2023-06-03 12:07:56.000000 kkexcel-0.1.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `kkexcel-0.1.6/kkexcel/generate_excel.py` & `kkexcel-0.1.7/kkexcel/generate_excel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+# /usr/bin/python
 # -*- coding: utf-8 -*-
+# @Time    : 2020/12/18 01:01
 # @Author: vekair
 
 import xlsxwriter
 
 
 def generate_excel(expenses, NAME):
     """
     自动顺序生成excel文件
     :param expenses: 列表、数组，里面是字典形式key,value 例如：[{"name":'XXX'}]
     :param NAME: new file name
     :return: XXX.xlsx
     """
-    workbook = xlsxwriter.Workbook('./{}.xlsx'.format(NAME))
+    workbook = xlsxwriter.Workbook('{}.xlsx'.format(NAME))
     worksheet = workbook.add_worksheet()
     keysList = [k for k in expenses[0].keys()]
     # 设定格式，等号左边格式名称自定义，字典中格式为指定选项
     # bold：加粗，num_format:数字格式
     bold_format = workbook.add_format({'bold': True})
     columnList = [chr(i) for i in range(ord("A"), ord("Z") + 1)]
     # 将二行二列设置宽度为15(从0开始)
```

