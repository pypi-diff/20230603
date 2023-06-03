# Comparing `tmp/customtkinterx-0.2.0.tar.gz` & `tmp/customtkinterx-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customtkinterx-0.2.0.tar", max compression
+gzip compressed data, was "customtkinterx-0.2.1.tar", max compression
```

## Comparing `customtkinterx-0.2.0.tar` & `customtkinterx-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0      242 2023-06-02 14:05:53.035149 customtkinterx-0.2.0/customtkinterx/__base64.py
--rw-r--r--   0        0        0     1012 2023-06-03 04:42:25.299802 customtkinterx-0.2.0/customtkinterx/__init__.py
--rw-r--r--   0        0        0      804 2023-06-03 04:32:03.691398 customtkinterx-0.2.0/customtkinterx/__main__.py
--rw-r--r--   0        0        0     6241 2023-06-03 04:57:04.722519 customtkinterx-0.2.0/customtkinterx/CTkCustom.py
--rw-r--r--   0        0        0     6220 2023-06-03 03:49:13.477694 customtkinterx-0.2.0/customtkinterx/CTkFluentTheme.py
--rw-r--r--   0        0        0     6286 2023-06-03 04:57:04.717519 customtkinterx-0.2.0/customtkinterx/CTkInfoBar.py
--rw-r--r--   0        0        0     1244 2023-06-02 11:00:54.754723 customtkinterx-0.2.0/customtkinterx/CTkListBox.py
--rw-r--r--   0        0        0     3180 2023-06-03 04:57:04.655526 customtkinterx-0.2.0/customtkinterx/CTkMegaMenuBar.py
--rw-r--r--   0        0        0      269 2023-05-29 10:31:31.000000 customtkinterx-0.2.0/customtkinterx/CTkMenuBar/__init__.py
--rw-r--r--   0        0        0      522 2023-06-03 04:06:01.937274 customtkinterx-0.2.0/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    16174 2023-06-03 04:13:46.399109 customtkinterx-0.2.0/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc
--rw-r--r--   0        0        0     5239 2023-06-03 04:13:46.393587 customtkinterx-0.2.0/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc
--rw-r--r--   0        0        0     9724 2023-06-03 04:13:46.396108 customtkinterx-0.2.0/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc
--rw-r--r--   0        0        0     9636 2023-06-03 04:10:48.431998 customtkinterx-0.2.0/customtkinterx/CTkMenuBar/dropdown_menu.py
--rw-r--r--   0        0        0     3300 2023-06-03 04:10:48.421486 customtkinterx-0.2.0/customtkinterx/CTkMenuBar/menu_bar.py
--rw-r--r--   0        0        0     5858 2023-06-03 04:10:48.439015 customtkinterx-0.2.0/customtkinterx/CTkMenuBar/title_menu_win.py
--rw-r--r--   0        0        0     6190 2023-06-03 04:57:53.921397 customtkinterx-0.2.0/customtkinterx/CTkMinimalTheme.py
--rw-r--r--   0        0        0      241 2023-05-31 01:43:30.000000 customtkinterx-0.2.0/customtkinterx/CTkPDFViewer/__init__.py
--rw-r--r--   0        0        0      445 2023-06-03 04:13:46.400109 customtkinterx-0.2.0/customtkinterx/CTkPDFViewer/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6311 2023-06-03 04:14:21.525818 customtkinterx-0.2.0/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc
--rw-r--r--   0        0        0     3539 2023-06-03 04:14:21.178450 customtkinterx-0.2.0/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py
--rw-r--r--   0        0        0      227 2023-05-31 01:40:22.000000 customtkinterx-0.2.0/customtkinterx/CTkTable/__init__.py
--rw-r--r--   0        0        0      427 2023-06-03 04:41:34.919572 customtkinterx-0.2.0/customtkinterx/CTkTable/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    11621 2023-06-03 04:41:34.922572 customtkinterx-0.2.0/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc
--rw-r--r--   0        0        0     8158 2023-06-03 04:41:34.520984 customtkinterx-0.2.0/customtkinterx/CTkTable/ctktable.py
--rw-r--r--   0        0        0      225 2023-05-08 22:30:16.000000 customtkinterx-0.2.0/customtkinterx/CTkToolTip/__init__.py
--rw-r--r--   0        0        0      426 2023-06-03 04:22:17.427710 customtkinterx-0.2.0/customtkinterx/CTkToolTip/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    10684 2023-06-03 04:26:02.400121 customtkinterx-0.2.0/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc
--rw-r--r--   0        0        0     6942 2023-06-03 04:22:52.495987 customtkinterx-0.2.0/customtkinterx/CTkToolTip/ctk_tooltip.py
--rw-r--r--   0        0        0     5598 2023-06-02 14:38:51.493749 customtkinterx-0.2.0/customtkinterx/Fluent.json
--rw-r--r--   0        0        0     2418 2023-06-02 22:37:52.229296 customtkinterx-0.2.0/customtkinterx/LaunchMusix.py
--rw-r--r--   0        0        0     5561 2023-06-03 04:47:54.791777 customtkinterx-0.2.0/customtkinterx/Minimal.json
--rw-r--r--   0        0        0      343 2023-06-03 04:58:23.990003 customtkinterx-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3405 2023-06-03 04:59:32.072137 customtkinterx-0.2.0/README.md
--rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 customtkinterx-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      242 2023-06-02 14:05:53.035149 customtkinterx-0.2.1/customtkinterx/__base64.py
+-rw-r--r--   0        0        0     1012 2023-06-03 04:42:25.299802 customtkinterx-0.2.1/customtkinterx/__init__.py
+-rw-r--r--   0        0        0      804 2023-06-03 04:32:03.691398 customtkinterx-0.2.1/customtkinterx/__main__.py
+-rw-r--r--   0        0        0     6241 2023-06-03 04:57:04.722519 customtkinterx-0.2.1/customtkinterx/CTkCustom.py
+-rw-r--r--   0        0        0     6220 2023-06-03 03:49:13.477694 customtkinterx-0.2.1/customtkinterx/CTkFluentTheme.py
+-rw-r--r--   0        0        0     6286 2023-06-03 04:57:04.717519 customtkinterx-0.2.1/customtkinterx/CTkInfoBar.py
+-rw-r--r--   0        0        0     1244 2023-06-02 11:00:54.754723 customtkinterx-0.2.1/customtkinterx/CTkListBox.py
+-rw-r--r--   0        0        0     3180 2023-06-03 04:57:04.655526 customtkinterx-0.2.1/customtkinterx/CTkMegaMenuBar.py
+-rw-r--r--   0        0        0      269 2023-05-29 10:31:31.000000 customtkinterx-0.2.1/customtkinterx/CTkMenuBar/__init__.py
+-rw-r--r--   0        0        0      522 2023-06-03 04:06:01.937274 customtkinterx-0.2.1/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    16174 2023-06-03 04:13:46.399109 customtkinterx-0.2.1/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc
+-rw-r--r--   0        0        0     5239 2023-06-03 04:13:46.393587 customtkinterx-0.2.1/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc
+-rw-r--r--   0        0        0     9724 2023-06-03 04:13:46.396108 customtkinterx-0.2.1/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc
+-rw-r--r--   0        0        0     9636 2023-06-03 04:10:48.431998 customtkinterx-0.2.1/customtkinterx/CTkMenuBar/dropdown_menu.py
+-rw-r--r--   0        0        0     3300 2023-06-03 04:10:48.421486 customtkinterx-0.2.1/customtkinterx/CTkMenuBar/menu_bar.py
+-rw-r--r--   0        0        0     5858 2023-06-03 04:10:48.439015 customtkinterx-0.2.1/customtkinterx/CTkMenuBar/title_menu_win.py
+-rw-r--r--   0        0        0     6190 2023-06-03 04:57:53.921397 customtkinterx-0.2.1/customtkinterx/CTkMinimalTheme.py
+-rw-r--r--   0        0        0      241 2023-05-31 01:43:30.000000 customtkinterx-0.2.1/customtkinterx/CTkPDFViewer/__init__.py
+-rw-r--r--   0        0        0      445 2023-06-03 04:13:46.400109 customtkinterx-0.2.1/customtkinterx/CTkPDFViewer/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6311 2023-06-03 04:14:21.525818 customtkinterx-0.2.1/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc
+-rw-r--r--   0        0        0     3543 2023-06-03 05:14:11.938896 customtkinterx-0.2.1/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py
+-rw-r--r--   0        0        0      227 2023-05-31 01:40:22.000000 customtkinterx-0.2.1/customtkinterx/CTkTable/__init__.py
+-rw-r--r--   0        0        0      427 2023-06-03 04:41:34.919572 customtkinterx-0.2.1/customtkinterx/CTkTable/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    11621 2023-06-03 04:41:34.922572 customtkinterx-0.2.1/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc
+-rw-r--r--   0        0        0     8158 2023-06-03 04:41:34.520984 customtkinterx-0.2.1/customtkinterx/CTkTable/ctktable.py
+-rw-r--r--   0        0        0      225 2023-05-08 22:30:16.000000 customtkinterx-0.2.1/customtkinterx/CTkToolTip/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-03 04:22:17.427710 customtkinterx-0.2.1/customtkinterx/CTkToolTip/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    10684 2023-06-03 04:26:02.400121 customtkinterx-0.2.1/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc
+-rw-r--r--   0        0        0     6942 2023-06-03 04:22:52.495987 customtkinterx-0.2.1/customtkinterx/CTkToolTip/ctk_tooltip.py
+-rw-r--r--   0        0        0     5598 2023-06-02 14:38:51.493749 customtkinterx-0.2.1/customtkinterx/Fluent.json
+-rw-r--r--   0        0        0  1445444 2023-06-03 05:09:33.609641 customtkinterx-0.2.1/customtkinterx/input.png
+-rw-r--r--   0        0        0     2418 2023-06-02 22:37:52.229296 customtkinterx-0.2.1/customtkinterx/LaunchMusix.py
+-rw-r--r--   0        0        0     5561 2023-06-03 04:47:54.791777 customtkinterx-0.2.1/customtkinterx/Minimal.json
+-rw-r--r--   0        0        0      343 2023-06-03 05:14:23.598522 customtkinterx-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3405 2023-06-03 04:59:32.072137 customtkinterx-0.2.1/README.md
+-rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 customtkinterx-0.2.1/PKG-INFO
```

### Comparing `customtkinterx-0.2.0/customtkinterx/__init__.py` & `customtkinterx-0.2.1/customtkinterx/__init__.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/__main__.py` & `customtkinterx-0.2.1/customtkinterx/__main__.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/CTkCustom.py` & `customtkinterx-0.2.1/customtkinterx/CTkCustom.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/CTkFluentTheme.py` & `customtkinterx-0.2.1/customtkinterx/CTkFluentTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/CTkInfoBar.py` & `customtkinterx-0.2.1/customtkinterx/CTkInfoBar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/CTkListBox.py` & `customtkinterx-0.2.1/customtkinterx/CTkListBox.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/CTkMegaMenuBar.py` & `customtkinterx-0.2.1/customtkinterx/CTkMegaMenuBar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc` & `customtkinterx-0.2.1/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc` & `customtkinterx-0.2.1/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc` & `customtkinterx-0.2.1/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc` & `customtkinterx-0.2.1/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/CTkMenuBar/dropdown_menu.py` & `customtkinterx-0.2.1/customtkinterx/CTkMenuBar/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/CTkMenuBar/menu_bar.py` & `customtkinterx-0.2.1/customtkinterx/CTkMenuBar/menu_bar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/CTkMenuBar/title_menu_win.py` & `customtkinterx-0.2.1/customtkinterx/CTkMenuBar/title_menu_win.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/CTkMinimalTheme.py` & `customtkinterx-0.2.1/customtkinterx/CTkMinimalTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc` & `customtkinterx-0.2.1/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py` & `customtkinterx-0.2.1/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 CTkPDFViewer is a pdf viewer widget for customtkinter.
 Author: Akash Bora
 License: MIT
 """
 
 import customtkinter
-from PIL import Image
 
 try:
     import fitz
+    from PIL import Image
 except ModuleNotFoundError:
     pass
 from threading import Thread
 import math
 import io
 import os
```

### Comparing `customtkinterx-0.2.0/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc` & `customtkinterx-0.2.1/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/CTkTable/ctktable.py` & `customtkinterx-0.2.1/customtkinterx/CTkTable/ctktable.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc` & `customtkinterx-0.2.1/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/CTkToolTip/ctk_tooltip.py` & `customtkinterx-0.2.1/customtkinterx/CTkToolTip/ctk_tooltip.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/Fluent.json` & `customtkinterx-0.2.1/customtkinterx/Fluent.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/LaunchMusix.py` & `customtkinterx-0.2.1/customtkinterx/LaunchMusix.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/customtkinterx/Minimal.json` & `customtkinterx-0.2.1/customtkinterx/Minimal.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/README.md` & `customtkinterx-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.2.0/PKG-INFO` & `customtkinterx-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customtkinterx
-Version: 0.2.0
+Version: 0.2.1
 Summary: extra widgets for customtkinter
 Author: XiangQinxi
 Author-email: XiangQinxi@outlook.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

