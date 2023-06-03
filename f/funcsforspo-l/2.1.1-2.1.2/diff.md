# Comparing `tmp/funcsforspo_l-2.1.1.tar.gz` & `tmp/funcsforspo_l-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcsforspo_l-2.1.1.tar", last modified: Mon Apr 24 15:27:36 2023, max compression
+gzip compressed data, was "funcsforspo_l-2.1.2.tar", last modified: Sat Jun  3 13:19:29 2023, max compression
```

## Comparing `funcsforspo_l-2.1.1.tar` & `funcsforspo_l-2.1.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.343428 funcsforspo_l-2.1.1/
--rw-rw-rw-   0        0        0     1076 2023-02-03 19:05:17.000000 funcsforspo_l-2.1.1/LICENSE
--rw-rw-rw-   0        0        0     1374 2023-04-24 15:27:36.338461 funcsforspo_l-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      935 2023-02-03 19:05:17.000000 funcsforspo_l-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.128252 funcsforspo_l-2.1.1/funcsforspo_l/
-drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.188733 funcsforspo_l-2.1.1/funcsforspo_l/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 funcsforspo_l-2.1.1/funcsforspo_l/femails/__init__.py
--rw-rw-rw-   0        0        0     7604 2023-01-19 14:03:01.000000 funcsforspo_l-2.1.1/funcsforspo_l/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.200789 funcsforspo_l-2.1.1/funcsforspo_l/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.1/funcsforspo_l/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      638 2023-01-19 14:04:05.000000 funcsforspo_l-2.1.1/funcsforspo_l/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.208796 funcsforspo_l-2.1.1/funcsforspo_l/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.1/funcsforspo_l/fftp/__init__.py
--rw-rw-rw-   0        0        0     6241 2023-01-19 14:03:52.000000 funcsforspo_l-2.1.1/funcsforspo_l/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.218305 funcsforspo_l-2.1.1/funcsforspo_l/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.1/funcsforspo_l/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11086 2023-02-03 19:05:17.000000 funcsforspo_l-2.1.1/funcsforspo_l/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.121889 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/
-drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.224008 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/base/
--rw-rw-rw-   0        0        0    10163 2023-04-14 13:50:03.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/base/base.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.241009 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fcompress/
--rw-rw-rw-   0        0        0     7782 2023-01-19 14:04:21.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1637 2023-02-03 19:05:17.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.257167 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     3198 2023-03-25 20:17:19.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1607 2023-02-03 21:27:39.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.264387 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    11127 2023-01-19 14:04:42.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.280904 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     3546 2023-03-25 20:46:53.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     2715 2023-03-25 20:26:53.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.285386 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/pdftoxlsx/
--rw-rw-rw-   0        0        0     4212 2023-04-13 21:48:05.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpdf/pdftoxlsx/pdftoxlsx.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.295128 funcsforspo_l-2.1.1/funcsforspo_l/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4620 2023-01-19 14:04:54.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.304118 funcsforspo_l-2.1.1/funcsforspo_l/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpython/__init__.py
--rw-rw-rw-   0        0        0    67709 2023-03-25 20:45:09.000000 funcsforspo_l-2.1.1/funcsforspo_l/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.314461 funcsforspo_l-2.1.1/funcsforspo_l/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.1/funcsforspo_l/fregex/__init__.py
--rw-rw-rw-   0        0        0    10116 2023-02-03 19:05:17.000000 funcsforspo_l-2.1.1/funcsforspo_l/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.322914 funcsforspo_l-2.1.1/funcsforspo_l/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.1/funcsforspo_l/fselenium/__init__.py
--rw-rw-rw-   0        0        0    37863 2023-04-24 15:26:45.000000 funcsforspo_l-2.1.1/funcsforspo_l/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.334971 funcsforspo_l-2.1.1/funcsforspo_l/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.1/funcsforspo_l/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1645 2023-02-03 19:02:23.000000 funcsforspo_l-2.1.1/funcsforspo_l/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-04-24 15:27:36.178473 funcsforspo_l-2.1.1/funcsforspo_l.egg-info/
--rw-rw-rw-   0        0        0     1374 2023-04-24 15:27:35.000000 funcsforspo_l-2.1.1/funcsforspo_l.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1375 2023-04-24 15:27:36.000000 funcsforspo_l-2.1.1/funcsforspo_l.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 15:27:35.000000 funcsforspo_l-2.1.1/funcsforspo_l.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      139 2023-04-24 15:27:35.000000 funcsforspo_l-2.1.1/funcsforspo_l.egg-info/requires.txt
--rw-rw-rw-   0        0        0      391 2023-04-24 15:27:35.000000 funcsforspo_l-2.1.1/funcsforspo_l.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 15:27:36.343934 funcsforspo_l-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2153 2023-04-24 15:26:59.000000 funcsforspo_l-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:19:29.825299 funcsforspo_l-2.1.2/
+-rw-rw-rw-   0        0        0     1076 2023-02-03 19:05:17.000000 funcsforspo_l-2.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1374 2023-06-03 13:19:29.821889 funcsforspo_l-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      935 2023-02-03 19:05:17.000000 funcsforspo_l-2.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 13:19:29.563938 funcsforspo_l-2.1.2/funcsforspo_l/
+drwxrwxrwx   0        0        0        0 2023-06-03 13:19:29.633643 funcsforspo_l-2.1.2/funcsforspo_l/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 funcsforspo_l-2.1.2/funcsforspo_l/femails/__init__.py
+-rw-rw-rw-   0        0        0     7604 2023-01-19 14:03:01.000000 funcsforspo_l-2.1.2/funcsforspo_l/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:19:29.644481 funcsforspo_l-2.1.2/funcsforspo_l/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.2/funcsforspo_l/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      638 2023-01-19 14:04:05.000000 funcsforspo_l-2.1.2/funcsforspo_l/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:19:29.655465 funcsforspo_l-2.1.2/funcsforspo_l/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.2/funcsforspo_l/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6241 2023-01-19 14:03:52.000000 funcsforspo_l-2.1.2/funcsforspo_l/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:19:29.666133 funcsforspo_l-2.1.2/funcsforspo_l/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.2/funcsforspo_l/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11086 2023-02-03 19:05:17.000000 funcsforspo_l-2.1.2/funcsforspo_l/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:19:29.558919 funcsforspo_l-2.1.2/funcsforspo_l/fpdf/
+drwxrwxrwx   0        0        0        0 2023-06-03 13:19:29.673758 funcsforspo_l-2.1.2/funcsforspo_l/fpdf/base/
+-rw-rw-rw-   0        0        0    10163 2023-04-14 13:50:03.000000 funcsforspo_l-2.1.2/funcsforspo_l/fpdf/base/base.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:19:29.692299 funcsforspo_l-2.1.2/funcsforspo_l/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     7782 2023-01-19 14:04:21.000000 funcsforspo_l-2.1.2/funcsforspo_l/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 funcsforspo_l-2.1.2/funcsforspo_l/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1637 2023-02-03 19:05:17.000000 funcsforspo_l-2.1.2/funcsforspo_l/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:19:29.709673 funcsforspo_l-2.1.2/funcsforspo_l/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     3198 2023-03-25 20:17:19.000000 funcsforspo_l-2.1.2/funcsforspo_l/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 funcsforspo_l-2.1.2/funcsforspo_l/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1607 2023-02-03 21:27:39.000000 funcsforspo_l-2.1.2/funcsforspo_l/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:19:29.714682 funcsforspo_l-2.1.2/funcsforspo_l/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    11127 2023-01-19 14:04:42.000000 funcsforspo_l-2.1.2/funcsforspo_l/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:19:29.732897 funcsforspo_l-2.1.2/funcsforspo_l/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 funcsforspo_l-2.1.2/funcsforspo_l/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     3546 2023-03-25 20:46:53.000000 funcsforspo_l-2.1.2/funcsforspo_l/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     2719 2023-04-24 15:27:51.000000 funcsforspo_l-2.1.2/funcsforspo_l/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:19:29.738079 funcsforspo_l-2.1.2/funcsforspo_l/fpdf/pdftoxlsx/
+-rw-rw-rw-   0        0        0     4212 2023-04-13 21:48:05.000000 funcsforspo_l-2.1.2/funcsforspo_l/fpdf/pdftoxlsx/pdftoxlsx.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:19:29.747977 funcsforspo_l-2.1.2/funcsforspo_l/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.2/funcsforspo_l/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4620 2023-01-19 14:04:54.000000 funcsforspo_l-2.1.2/funcsforspo_l/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:19:29.758212 funcsforspo_l-2.1.2/funcsforspo_l/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.2/funcsforspo_l/fpython/__init__.py
+-rw-rw-rw-   0        0        0    65246 2023-06-03 13:16:05.000000 funcsforspo_l-2.1.2/funcsforspo_l/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:19:29.769796 funcsforspo_l-2.1.2/funcsforspo_l/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.2/funcsforspo_l/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10116 2023-02-03 19:05:17.000000 funcsforspo_l-2.1.2/funcsforspo_l/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:19:29.779841 funcsforspo_l-2.1.2/funcsforspo_l/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.2/funcsforspo_l/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    37863 2023-04-24 15:26:45.000000 funcsforspo_l-2.1.2/funcsforspo_l/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:19:29.790713 funcsforspo_l-2.1.2/funcsforspo_l/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 funcsforspo_l-2.1.2/funcsforspo_l/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1645 2023-02-03 19:02:23.000000 funcsforspo_l-2.1.2/funcsforspo_l/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:19:29.622143 funcsforspo_l-2.1.2/funcsforspo_l.egg-info/
+-rw-rw-rw-   0        0        0     1374 2023-06-03 13:19:29.000000 funcsforspo_l-2.1.2/funcsforspo_l.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1375 2023-06-03 13:19:29.000000 funcsforspo_l-2.1.2/funcsforspo_l.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 13:19:29.000000 funcsforspo_l-2.1.2/funcsforspo_l.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      139 2023-06-03 13:19:29.000000 funcsforspo_l-2.1.2/funcsforspo_l.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      391 2023-06-03 13:19:29.000000 funcsforspo_l-2.1.2/funcsforspo_l.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 13:19:29.826299 funcsforspo_l-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2153 2023-06-03 13:19:16.000000 funcsforspo_l-2.1.2/setup.py
```

### Comparing `funcsforspo_l-2.1.1/LICENSE` & `funcsforspo_l-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.1.1/PKG-INFO` & `funcsforspo_l-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcsforspo_l
-Version: 2.1.1
+Version: 2.1.2
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium - Linux
 Home-page: https://github.com/githubpaycon/funcsforspo_l
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium - Linux
 Description-Content-Type: text/markdown
```

### Comparing `funcsforspo_l-2.1.1/README.md` & `funcsforspo_l-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.1.1/funcsforspo_l/femails/femails.py` & `funcsforspo_l-2.1.2/funcsforspo_l/femails/femails.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.1.1/funcsforspo_l/fexceptions/exceptions.py` & `funcsforspo_l-2.1.2/funcsforspo_l/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.1.1/funcsforspo_l/fftp/fftp.py` & `funcsforspo_l-2.1.2/funcsforspo_l/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.1.1/funcsforspo_l/fopenpyxl/openpyxl_funcs.py` & `funcsforspo_l-2.1.2/funcsforspo_l/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.1.1/funcsforspo_l/fpdf/base/base.py` & `funcsforspo_l-2.1.2/funcsforspo_l/fpdf/base/base.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fcompress/__compress_online.py` & `funcsforspo_l-2.1.2/funcsforspo_l/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fcompress/compress.py` & `funcsforspo_l-2.1.2/funcsforspo_l/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `funcsforspo_l-2.1.2/funcsforspo_l/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fhtml_to_pdf/html_to_pdf.py` & `funcsforspo_l-2.1.2/funcsforspo_l/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.1.1/funcsforspo_l/fpdf/fimgpdf/img_to_pdf.py` & `funcsforspo_l-2.1.2/funcsforspo_l/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.1.1/funcsforspo_l/fpdf/focr/__ocr_online.py` & `funcsforspo_l-2.1.2/funcsforspo_l/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.1.1/funcsforspo_l/fpdf/focr/orc.py` & `funcsforspo_l-2.1.2/funcsforspo_l/fpdf/focr/orc.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,7 +73,9 @@
     else:
         text = transforma_lista_em_string(text)
         
         if export_from_file_txt:
             with open('extraction_pdf.txt', 'w', encoding='utf-8') as f:
                 f.write(text)
         return text
+
+
```

### Comparing `funcsforspo_l-2.1.1/funcsforspo_l/fpdf/pdftoxlsx/pdftoxlsx.py` & `funcsforspo_l-2.1.2/funcsforspo_l/fpdf/pdftoxlsx/pdftoxlsx.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.1.1/funcsforspo_l/fpysimplegui/functions_for_sg.py` & `funcsforspo_l-2.1.2/funcsforspo_l/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.1.1/funcsforspo_l/fpython/functions_for_py.py` & `funcsforspo_l-2.1.2/funcsforspo_l/fpython/functions_for_py.py`

 * *Files 10% similar despite different names*

```diff
@@ -1368,29 +1368,28 @@
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.chrome.options import Options as ChromeOptions
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.wait import WebDriverWait
 from selenium.common.exceptions import *
 from webdriver_manager.chrome import ChromeDriverManager
-from funcsforspo_l.fpython.functions_for_py import *
-from funcsforspo_l.fselenium.functions_selenium import *
-from funcsforspo_l.fwinotify.fwinotify import *
-from funcsforspo_l.fregex.functions_re import *
-from src.exceptions.exceptions import *
+from FuncsForSPO.fpython.functions_for_py import *
+from FuncsForSPO.fselenium.functions_selenium import *
+from FuncsForSPO.fwinotify.fwinotify import *
+from FuncsForSPO.fregex.functions_re import *
 import pandas as pd
 import json
 import os
 
 # -- GLOBAL -- #
 URL_SUPORTE = f'https://api.whatsapp.com/send?phone=5511985640273'
 CONFIG_PATH = arquivo_com_caminho_absoluto('bin', 'config.json')
 BASE = os.path.abspath('base')
-__DOWNLOAD_DIR =  cria_dir_no_dir_de_trabalho_atual(dir='downloads', print_value=False, criar_diretorio=True)
-limpa_diretorio(__DOWNLOAD_DIR)
+DOWNLOAD_DIR =  cria_dir_no_dir_de_trabalho_atual(dir='downloads', print_value=False, criar_diretorio=True)
+limpa_diretorio(DOWNLOAD_DIR)
 # -- GLOBAL -- #
 
 class Bot:    
     def __init__(self, headless, download_files) -> None:
         # --- CHROME OPTIONS --- #
         self._options = ChromeOptions()
         
@@ -1406,16 +1405,16 @@
                         ],
                         "selectedDestinationId": "Save as PDF",
                         "version": 2,
                     }
 
 
             self._PROFILE = {'printing.print_preview_sticky_settings.appState': json.dumps(self._SETTINGS_SAVE_AS_PDF),
-                    "savefile.default_directory":  f"{__DOWNLOAD_DIR}",
-                    "download.default_directory":  f"{__DOWNLOAD_DIR}",
+                    "savefile.default_directory":  f"{DOWNLOAD_DIR}",
+                    "download.default_directory":  f"{DOWNLOAD_DIR}",
                     "download.prompt_for_download": False,
                     "download.directory_upgrade": True,
                     "profile.managed_default_content_settings.images": 2,
                     "safebrowsing.enabled": True}
                 
             self._options.add_experimental_option('prefs', self._PROFILE)
         
@@ -1441,14 +1440,16 @@
         self._options.add_argument("--proxy-server='direct://'")
         self._options.add_argument('--proxy-bypass-list=*')
         self._options.add_argument('--disable-dev-shm-usage')
         self._options.add_argument('--block-new-web-contents')
         self._options.add_argument('--incognito')
         self._options.add_argument('–disable-notifications')
         self._options.add_argument("--window-size=1920,1080")
+        self._options.add_argument('--kiosk-printing')
+
         
         self.__service = Service(ChromeDriverManager().install())
         
         # create DRIVER
         self.DRIVER = Chrome(service=self.__service, options=self._options)
         
         def enable_download_in_headless_chrome(driver, download_dir):
@@ -1461,15 +1462,15 @@
 
             Em resumo, o código adiciona suporte para o download automático de arquivos em um diretório especificado no Chrome sem interface gráfica usando o Selenium WebDriver.
             '''
             driver.command_executor._commands["send_command"] = ("POST", '/session/$sessionId/chromium/send_command')
 
             params = {'cmd': 'Page.setDownloadBehavior', 'params': {'behavior': 'allow', 'downloadPath': download_dir}}
             command_result = driver.execute("send_command", params)
-        enable_download_in_headless_chrome(self.DRIVER, self.DOWNLOAD_DIR)
+        enable_download_in_headless_chrome(self.DRIVER, DOWNLOAD_DIR)
         
         
         self.WDW3 = WebDriverWait(self.DRIVER, timeout=3)
         self.WDW5 = WebDriverWait(self.DRIVER, timeout=5)
         self.WDW7 = WebDriverWait(self.DRIVER, timeout=7)
         self.WDW10 = WebDriverWait(self.DRIVER, timeout=10)
         self.WDW30 = WebDriverWait(self.DRIVER, timeout=30)
@@ -1477,104 +1478,82 @@
 
         self.DRIVER.maximize_window()
         return self.DRIVER
 """)
     
     # CRIA ARQUIVO PYTHON EM database
     with open(DATABASE_PATH, 'w', encoding='utf-8') as f:
-        f.write("""from funcsforspo_l.fpython.functions_for_py import *
-from funcsforspo_l.fselenium.functions_selenium import *
-from funcsforspo_l.fsqlite.sqlite_functions import *
-from funcsforspo_l.fpysimplegui.functions_for_sg import *
-import pandas as pd
+        f.write("""from FuncsForSPO.fpython.functions_for_py import *
+from sqlalchemy import create_engine
+from sqlalchemy.orm import sessionmaker
+from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy import Column, String, Integer
 
-# GLOBAL
-DATABASE_PATH = arquivo_com_caminho_absoluto('bin', 'database.db')
-RESULTADO = cria_dir_no_dir_de_trabalho_atual('Resultados')
-# GLOBAL
-
-# BACKUP
-def faz_backup_do_banco_de_dados():
-    json_config = read_json(arquivo_com_caminho_absoluto('bin', 'config.json'))
-
-    # cria os dirs
-    cria_dir_no_dir_de_trabalho_atual(arquivo_com_caminho_absoluto('bin', 'backup'))
-    
-    path_database_copy = arquivo_com_caminho_absoluto(['bin', 'backup'], f'database_{datetime.now().strftime("%d-%m-%Y_%H-%M-%S")}.db')
-    shutil.copy2(DATABASE_PATH, path_database_copy)
-    return path_database_copy
-# BACKUP
-
-
-# EXPORT
-def exportar_database():
-    cur, con =  connect_db(DATABASE_PATH)
-    arquivos = pd.read_sql('SELECT * FROM arquivos', con)
-    arquivos_com_ocr = pd.read_sql('SELECT * FROM arquivos_com_ocr', con)
-    # TRATAMENTOS
-    arquivos_com_ocr['data_adicao'] = arquivos_com_ocr['data_adicao'].apply(lambda x: datetime.strptime(x, '%Y-%m-%d %H:%M:%S.%f'))
-    
-    arquivos_com_ocr.rename(columns={'caminho_arquivo': 'Caminho do Arquivo'}, inplace=True)
-    arquivos_com_ocr.rename(columns={'nome_do_arquivo': 'Nome do Arquivo'}, inplace=True)
-    arquivos_com_ocr.rename(columns={'ocr': 'OCR do Arquivo'}, inplace=True)
-    arquivos_com_ocr.rename(columns={'data_adicao': 'Data de Envio no Database'}, inplace=True)
-
-
-    arquivos.rename(columns={'caminho_arquivo': 'Caminho do Arquivo'}, inplace=True)
-    arquivos.rename(columns={'nome_do_arquivo': 'Nome do Arquivo'}, inplace=True)
-    # TRATAMENTOS
-    
-    try:
-        with pd.ExcelWriter(os.path.join(RESULTADO, 'DATABASE.xlsx')) as writer:
-            arquivos_com_ocr.to_excel(writer, sheet_name="Arquivos Com OCR", index=False)
-            arquivos.to_excel(writer, sheet_name="PDFs Recuperados da Máquina", index=False)
-    except PermissionError:
-        sleep(10)
-        try:
-            with pd.ExcelWriter(os.path.join(RESULTADO, 'DATABASE.xlsx')) as writer:
-                arquivos_com_ocr.to_excel(writer, sheet_name="Arquivos Com OCR", index=False)
-                arquivos.to_excel(writer, sheet_name="PDFs Recuperados da Máquina", index=False)
-        except PermissionError:
-            faz_log('O Arquivo está aberto, não foi possível exportar...')
-    except OSError:
-        popup_erro('Sem espaço em disco para fazer o arquivo...', 'Sem espaço...')
-        pass
-# EXPORT
-
-# DELETE
-def delete(table):
-    # Apaga todos os dados da tabela enviada
-    cur, con =  connect_db(DATABASE_PATH)
-    query = f'DELETE FROM {table};'
-    cur.execute(query)
-    con.commit()
-# DELETE
-
-# SELECT
-def select(table:str, col: str='*', data_from_line: bool=False):
-    cur, con =  connect_db(DATABASE_PATH)
-    cur.execute(f'SELECT {col} FROM {table}')
-    faz_log(f'SELECT {col} FROM {table}', 'i*')
-    data = []
-    if data_from_line:
-        for line in cur.fetchall():
-            for i in line:
-                data.append(i)
-        return tuple(data)
-    else:
-        for line in cur.fetchall():
-            data.append(line)
-        return tuple(data)
-# SELECT
+engine = create_engine('sqlite:///database.db', pool_size=15, max_overflow=20)
+Base = declarative_base()
+Session = sessionmaker(bind=engine)
+
+
+class TABLE(Base):
+    __tablename__ = 'table'
+
+    id = Column(Integer, primary_key=True, autoincrement=True)
+    status = Column(String)
+    nome = Column(String)
+    
+Base.metadata.create_all(engine)  # cria a tabela no banco de dados
+
+    
+class DBManager:
+    def __init__(self):
+        # Inicializa uma nova sessão com o banco de dados.
+        
+        self.session = Session()
+
+    def create_item(self, status, name):
+        # Cria um novo registro na tabela.
+
+        new_item = TABLE(status=status, name=name)
+        self.session.add(new_item)
+        self.session.commit()
+
+    def get_item(self, id):
+        # Retorna o registro com o ID fornecido
+        return self.session.query(TABLE).filter_by(id=id).first()
+    
+
+    def delete_item(self, id):
+        # Exclui o registro com o ID fornecido da tabela
+
+        delete_item_from_db = self.get_item(id)
+        self.session.delete(delete_item_from_db)
+        self.session.commit()
+        
+    def delete_all(self):
+        # Exclui todos os registros da tabela.
+
+        self.session.query(TABLE).delete()
+        self.session.commit()
+
+    def get_item(self, id):
+        # Retorna o registro com o ID fornecido da tabela. Se nenhum registro for encontrado, retorna None.
+        return self.session.query(TABLE).filter_by(id=id).first()
+    
+
+    def get_column_status(self):
+        # Retorna o registro de status com o ID fornecido da tabela. Se nenhum registro for encontrado, retorna None.
+        return self.session.query(TABLE.status).all()
+    
+    
 
 """)
     
     # CRIA ARQUIVO PYTHON EM exceptions
     with open(EXCEPTIONS_PATH, 'w', encoding='utf-8') as f:
-        f.write("""from funcsforspo_l.fexceptions.exceptions import *
+        f.write("""from FuncsForSPO.fexceptions.exceptions import *
 """)
     
     # cria arquivo json
     with open(CONFIG_PATH, 'w', encoding='utf-8') as fjson:
         fjson.write("""{
     "CONFIG": {
         "STRING": "STRING",
@@ -1585,21 +1564,26 @@
         
     # cria arquivo utils
     with open(UTILS_PATH, 'w', encoding='utf-8') as fjson:
         fjson.write("""""")
 
     # cria arquivo de tests
     with open(TESTS_PATH, 'w', encoding='utf-8') as fjson:
-        fjson.write("""from funcsforspo_l.fpdf.focr.orc import *
-from funcsforspo_l.fpdf.fcompress.compress import *
-from funcsforspo_l.fpdf.fimgpdf.img_to_pdf import *
-from funcsforspo_l.fpysimplegui.functions_for_sg import *
-from funcsforspo_l.fpython.functions_for_py import *
-from funcsforspo_l.fregex.functions_re import *
-from funcsforspo_l.fselenium.functions_selenium import *
+        fjson.write("""from FuncsForSPO.fpdf.focr.orc import *
+from FuncsForSPO.fpdf.fcompress.compress import *
+from FuncsForSPO.fpdf.fimgpdf.img_to_pdf import *
+from FuncsForSPO.fpysimplegui.functions_for_sg import *
+from FuncsForSPO.fpython.functions_for_py import *
+from FuncsForSPO.fregex.functions_re import *
+from FuncsForSPO.fselenium.functions_selenium import *
+import sys
+import os
+
+root_dir = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+sys.path.append(root_dir)
 
 # SEMPRE COLOQUE O QUE A FUNÇÃO TEM QUE FAZER EXPLICITAMENTE
 """)
 
     # cria diretório base
     if create_base_dir:
         cria_dir_no_dir_de_trabalho_atual('base')
@@ -1686,78 +1670,24 @@
         if (format_exit == '') or (format_exit is None) or (isinstance(format_exit, bool)):
             return data
         data_ = data.strftime(format_exit)
         return data_
 
 
 def remove_pontos_e_barras(string):
-    """Função remove esses elementos da string
-    
-    '.'
-    
-    '/'
-    
-    ','
-    
-    '-'
-    
-    '_'
-    
-    '='
-    
-    '|'
-    
-    '#'
-    
-    '`'
-    
-    '~'
-    
-    "'"
-    
-    '"'
-    
-    'string'.strip()
-    #### Função já converte o argumento para str()
+    """Remove caracteres especiais da string.
 
     Args:
-        string (str): str com os caracteres
+        string (str): String com os caracteres especiais.
 
     Returns:
-        str: Retorna string sem nenhum desses caracteres
+        str: String sem os caracteres especiais.
     """
-    string = str(string)
-    string = string.replace('.','')
-    string = string.replace('/', '')
-    string = string.replace(',', '')
-    string = string.replace('-', '')
-    string = string.replace('_', '')
-    string = string.replace('=', '')
-    string = string.replace('|', '')
-    string = string.replace('`', '')
-    string = string.replace('~', '')
-    string = string.replace("'", '')
-    string = string.replace('"', '')
-    string = string.replace('#', '')
-    string = string.replace(';', '')
-    string = string.replace(':', '')
-    string = string.replace('@', '')
-    string = string.replace('!', '')
-    string = string.replace('(', '')
-    string = string.replace(')', '')
-    string = string.replace('$', '')
-    string = string.replace('%', '')
-    string = string.replace('+', '')
-    string = string.replace('&', '')
-    string = string.replace('^', '')
-    string = string.replace('*', '')
-    string = string.replace('{', '')
-    string = string.replace('}', '')
-    string = string.replace('[', '')
-    string = string.replace(']', '')
+    special_chars = r'[./,_=\|`~\'"#;:@!()\$%+&^\*\{\}\[\]\\]'
+    string = re.sub(special_chars, '', str(string))
     string = string.strip()
     return string
 
 
 def remove_duplicados_na_lista(iteravel:list|tuple, convert_str:bool=False):
     """Remove duplicados de uma lista
```

### Comparing `funcsforspo_l-2.1.1/funcsforspo_l/fregex/functions_re.py` & `funcsforspo_l-2.1.2/funcsforspo_l/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.1.1/funcsforspo_l/fselenium/functions_selenium.py` & `funcsforspo_l-2.1.2/funcsforspo_l/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.1.1/funcsforspo_l/fsqlite/sqlite_functions.py` & `funcsforspo_l-2.1.2/funcsforspo_l/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.1.1/funcsforspo_l.egg-info/PKG-INFO` & `funcsforspo_l-2.1.2/funcsforspo_l.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcsforspo-l
-Version: 2.1.1
+Version: 2.1.2
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium - Linux
 Home-page: https://github.com/githubpaycon/funcsforspo_l
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium - Linux
 Description-Content-Type: text/markdown
```

### Comparing `funcsforspo_l-2.1.1/funcsforspo_l.egg-info/SOURCES.txt` & `funcsforspo_l-2.1.2/funcsforspo_l.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funcsforspo_l-2.1.1/setup.py` & `funcsforspo_l-2.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 import os
 from setuptools import setup
 
-version = '2.1.1'
+version = '2.1.2'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='funcsforspo_l',
         version=version,
         url='https://github.com/githubpaycon/funcsforspo_l',
```

