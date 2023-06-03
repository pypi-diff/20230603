# Comparing `tmp/cicc_excel-0.2.0.tar.gz` & `tmp/cicc_excel-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cicc_excel-0.2.0.tar", last modified: Mon May 22 08:08:50 2023, max compression
+gzip compressed data, was "cicc_excel-0.3.0.tar", last modified: Sat Jun  3 01:26:21 2023, max compression
```

## Comparing `cicc_excel-0.2.0.tar` & `cicc_excel-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 08:08:50.280000 cicc_excel-0.2.0/
--rw-rw-rw-   0        0        0     1093 2023-05-14 05:35:00.000000 cicc_excel-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1777 2023-05-22 08:08:52.000000 cicc_excel-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1214 2023-05-22 08:03:36.000000 cicc_excel-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 08:08:50.310000 cicc_excel-0.2.0/cicc_excel/
--rw-rw-rw-   0        0        0        0 2023-05-14 05:35:00.000000 cicc_excel-0.2.0/cicc_excel/__init__.py
--rw-rw-rw-   0        0        0    13899 2023-05-22 08:02:56.000000 cicc_excel-0.2.0/cicc_excel/excelwriter.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:08:50.340000 cicc_excel-0.2.0/cicc_excel.egg-info/
--rw-rw-rw-   0        0        0     1777 2023-05-22 08:08:50.000000 cicc_excel-0.2.0/cicc_excel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-22 08:08:52.000000 cicc_excel-0.2.0/cicc_excel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 08:08:50.000000 cicc_excel-0.2.0/cicc_excel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-22 08:08:50.000000 cicc_excel-0.2.0/cicc_excel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-22 08:08:50.000000 cicc_excel-0.2.0/cicc_excel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 08:08:52.000000 cicc_excel-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      867 2023-05-22 08:08:38.000000 cicc_excel-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 01:26:21.170000 cicc_excel-0.3.0/
+-rw-rw-rw-   0        0        0     1093 2023-05-14 05:35:00.000000 cicc_excel-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     1837 2023-06-03 01:26:22.000000 cicc_excel-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1274 2023-06-02 15:16:00.000000 cicc_excel-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 01:26:21.220000 cicc_excel-0.3.0/cicc_excel/
+-rw-rw-rw-   0        0        0        0 2023-05-14 05:35:00.000000 cicc_excel-0.3.0/cicc_excel/__init__.py
+-rw-rw-rw-   0        0        0    14346 2023-06-02 15:13:08.000000 cicc_excel-0.3.0/cicc_excel/excelwriter.py
+drwxrwxrwx   0        0        0        0 2023-06-03 01:26:21.250000 cicc_excel-0.3.0/cicc_excel.egg-info/
+-rw-rw-rw-   0        0        0     1837 2023-06-03 01:26:22.000000 cicc_excel-0.3.0/cicc_excel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-03 01:26:22.000000 cicc_excel-0.3.0/cicc_excel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 01:26:22.000000 cicc_excel-0.3.0/cicc_excel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-03 01:26:22.000000 cicc_excel-0.3.0/cicc_excel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-03 01:26:22.000000 cicc_excel-0.3.0/cicc_excel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 01:26:22.000000 cicc_excel-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      867 2023-06-02 15:16:16.000000 cicc_excel-0.3.0/setup.py
```

### Comparing `cicc_excel-0.2.0/LICENSE` & `cicc_excel-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cicc_excel-0.2.0/PKG-INFO` & `cicc_excel-0.3.0/cicc_excel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cicc_excel
-Version: 0.2.0
+Name: cicc-excel
+Version: 0.3.0
 Summary: Library of export pandas into excel for CICCers
 Home-page: https://github.com/nyuspc/cicc_excel
 Author: Pengcheng Song
 Author-email: smth_spc@hotmail.com
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -21,15 +21,16 @@
 
 ```python
 from cicc_excel.excelwriter import ExcelWriter
 
 # create new writer
 # default font is 宋体, Arial, Times New Roman
 # to setup a percentage column, put a % in column name
-wb = ExcelWriter('export_file_name.xlsx', ch_font="中文字体", num_font="Number Font", en_font="English Font", first_row_color='#EEECE1', first_row_height=20)
+# default col width will adjust by font_size
+wb = ExcelWriter('export_file_name.xlsx', ch_font="中文字体", num_font="Number Font", en_font="English Font", first_row_color='#EEECE1', first_row_height=20, font_size=10)
 
 #load data into writer in pandas dataframe
 wb.load_data(df)
 
 #set highlight columns by name
 #color in #FFFFFF format
 wb.set_hl_col_by_names('col_name', 'sheet_name', 'background_color', 'color')
```

### Comparing `cicc_excel-0.2.0/README.md` & `cicc_excel-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 ```python
 from cicc_excel.excelwriter import ExcelWriter
 
 # create new writer
 # default font is 宋体, Arial, Times New Roman
 # to setup a percentage column, put a % in column name
-wb = ExcelWriter('export_file_name.xlsx', ch_font="中文字体", num_font="Number Font", en_font="English Font", first_row_color='#EEECE1', first_row_height=20)
+# default col width will adjust by font_size
+wb = ExcelWriter('export_file_name.xlsx', ch_font="中文字体", num_font="Number Font", en_font="English Font", first_row_color='#EEECE1', first_row_height=20, font_size=10)
 
 #load data into writer in pandas dataframe
 wb.load_data(df)
 
 #set highlight columns by name
 #color in #FFFFFF format
 wb.set_hl_col_by_names('col_name', 'sheet_name', 'background_color', 'color')
```

### Comparing `cicc_excel-0.2.0/cicc_excel/excelwriter.py` & `cicc_excel-0.3.0/cicc_excel/excelwriter.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,109 +9,111 @@
 import re
 import xlsxwriter
 
 class ExcelWriter(object):
     """
     Class for writing data to an xlsx file.
     """
-    def __init__(self, filename, en_font='Arial', ch_font='宋体', num_font='Arial', first_row_color=None, first_row_height=None):
+    def __init__(self, filename, en_font='Arial', ch_font='宋体', num_font='Arial', first_row_color=None, first_row_height=None, font_size=10):
         """
         Initialize an open workbook and add a worksheets.
         """
         self.filename = filename
         self.workbook = xlsxwriter.Workbook(filename, {'nan_inf_to_errors':True})
         self.styles = {
             'normal':{}
         }
         self.en_font = en_font
         self.ch_font = ch_font
         self.num_font = num_font
+        self.font_size = font_size
         self.hl_cols = {}
         #Setting Styles
         self.first_row_height = first_row_height
         if first_row_color is None:
             self.styles['normal']['header'] = self.workbook.add_format({
                 'border':None,
                 'bold': True,
-                'font_size': 10,
+                'font_size': font_size,
                 'font_name': ch_font,
                 'align': 'center',
                 'valign': 'vcenter'
             })
         else:
             self.styles['normal']['header'] = self.workbook.add_format({
                 'border':None,
                 'bold': True,
-                'font_size': 10,
+                'font_size': font_size,
                 'font_name': ch_font,
                 'bg_color': first_row_color,
                 'align': 'center',
                 'valign': 'vcenter'
             })
         self.styles['normal']['number_format'] = self.workbook.add_format({
-            'font_size': 10,
+            'font_size': font_size,
             'align': 'right',
             'valign': 'vcenter',
             'font_name': num_font,
             'num_format': '#,##0'
         })
         self.styles['normal']['worktime_format'] = self.workbook.add_format({
-            'font_size': 10,
+            'font_size': font_size,
             'align': 'right',
             'valign': 'vcenter',
             'font_name': num_font,
             'num_format': '#,##0.00'
         })
         self.styles['normal']['percent_format'] = self.workbook.add_format({
-            'font_size': 10,
+            'font_size': font_size,
             'align': 'right',
             'valign': 'vcenter',
             'font_name': num_font,
             'num_format': '0.00%'
         })
         self.styles['normal']['chinese_format'] = self.workbook.add_format({
             'font_name': ch_font,
-            'font_size': 10,
+            'font_size': font_size,
             'align': 'left',
             'valign': 'vcenter'
         })
         self.styles['normal']['english_format'] = self.workbook.add_format({
             'font_name': en_font,
-            'font_size': 10,
+            'font_size': font_size,
             'align': 'left',
             'valign': 'vcenter'
         })
         self.styles['normal']['sn_format'] = self.workbook.add_format({
             'font_name': num_font,
-            'font_size': 10,
+            'font_size': font_size,
             'align': 'left',
             'valign': 'vcenter',
             'bold': True
         })
         self.styles['normal']['date_format'] = self.workbook.add_format({
-            'font_size': 10,
+            'font_size': font_size,
             'align': 'right',
             'valign': 'vcenter',
             'font_name': num_font,
             'num_format':'yyyy/mm/dd'
         })
         self.styles['normal']['default_format'] = self.workbook.add_format({
-            'font_size':10,
+            'font_size': font_size,
             'align': 'left',
             'valign': 'vcenter'
         })
         #set default width
+        width_ratio = font_size/10
         self.column_width = {
-            'number': 15,
-            'worktime': 10,
-            'date': 10,
-            'percent': 8,
-            'text': 15,
-            'sn': 8,
-            'default': 10
+            'number': 12 * width_ratio,
+            'worktime': 5 * width_ratio,
+            'date': 8 * width_ratio,
+            'percent': 7 * width_ratio,
+            'text': 10 * width_ratio,
+            'sn': 8 * width_ratio,
+            'default': 8 * width_ratio
         }
     
     def load_data(self, data):
         """
         load data into workbook
         """
         self.set_global_format()
@@ -251,26 +253,28 @@
 
     def hide_col(self, start_col=0, end_col=0, sheet_name='Sheet1'):
         """
         Hide columns.
         """
         ws = self.workbook.get_worksheet_by_name(sheet_name)
         if ws is not None:
-            ws.set_column(start_col-1, end_col-1, None, None, {'hidden': True})
+            for col in range(start_col, end_col):
+                ws.set_column(col-1, col, None, None, {'hidden': True})
         else:
             print("Error: worksheets", sheet_name, "not found")
     
     def collapse_col(self, start_col=0, end_col=0, sheet_name='Sheet1'):
         """
         collapse columns.
         """
         ws = self.workbook.get_worksheet_by_name(sheet_name)
         if ws is not None:
         #collapsed note does not work, use hidden + level instead.
-            ws.set_column(start_col-1, end_col-1, None, None, {'hidden': True, 'level': 1})
+            for col in range(start_col, end_col):
+                ws.set_column(col-1, col, None, None, {'hidden': True, 'level': 1})
         else:
             print("Error: worksheets", sheet_name, "not found")
     
     def set_hl_col_by_names(self, col_name, sheet_name, hl_bg_color='#EEECE1', hl_color='#000000'):
         """
         Set col by col name
         """
@@ -283,82 +287,82 @@
             self.styles[sheet_name] = {}
         if self.styles[sheet_name].get(col_name) is None:
             self.styles[sheet_name][col_name] = {}
          # Set Highlight Styles
         self.styles[sheet_name][col_name]['header'] = self.workbook.add_format({
             'border':None,
             'bold': True,
-            'font_size': 10,
+            'font_size': self.font_size,
             'font_name': self.ch_font,
             'bg_color': hl_bg_color,
             'font_color': hl_color,
             'align': 'center',
             'valign': 'vcenter'
         })
         self.styles[sheet_name][col_name]['number_format'] = self.workbook.add_format({
-            'font_size': 10,
+            'font_size': self.font_size,
             'bg_color': hl_bg_color,
             'font_color': hl_color,
             'align': 'right',
             'valign': 'vcenter',
             'font_name': self.num_font,
             'num_format': '#,##0'
         })
         self.styles[sheet_name][col_name]['worktime_format'] = self.workbook.add_format({
-            'font_size': 10,
+            'font_size': self.font_size,
             'bg_color': hl_bg_color,
             'font_color': 'hl_color',
             'align': 'right',
             'valign': 'vcenter',
             'font_name': self.num_font,
             'num_format': '#,##0.00'
         })
         self.styles[sheet_name][col_name]['percent_format'] = self.workbook.add_format({
-            'font_size': 10,
+            'font_size': self.font_size,
             'bg_color': hl_bg_color,
             'font_color': hl_color,
             'align': 'right',
             'valign': 'vcenter',
             'font_name': self.num_font,
             'num_format': '0.00%'
         })
         self.styles[sheet_name][col_name]['chinese_format'] = self.workbook.add_format({
             'font_name': self.ch_font,
             'bg_color': hl_bg_color,
             'font_color': hl_color,
-            'font_size': 10,
+            'font_size': self.font_size,
             'align': 'left',
             'valign': 'vcenter'
         })
         self.styles[sheet_name][col_name]['english_format'] = self.workbook.add_format({
             'font_name': self.en_font,
             'bg_color': hl_bg_color,
             'font_color': hl_color,
-            'font_size': 10,
+            'font_size': self.font_size,
             'valign': 'vcenter',
             'align': 'left'
         })
         self.styles[sheet_name][col_name]['sn_format'] = self.workbook.add_format({
             'font_name': self.num_font,
             'bg_color': hl_bg_color,
             'font_color': hl_color,
-            'font_size': 10,
+            'font_size': self.font_size,
             'align': 'left',
             'valign': 'vcenter',
             'bold': True
         })
         self.styles[sheet_name][col_name]['date_format'] = self.workbook.add_format({
-            'font_size': 10,
+            'font_size': self.font_size,
             'bg_color': hl_bg_color,
             'font_color': hl_color,
             'align': 'right',
             'valign': 'vcenter',
             'font_name': self.num_font,
             'num_format':'yyyy/mm/dd'
         })
         self.styles[sheet_name][col_name]['default_format'] = self.workbook.add_format({
-            'font_size':10,
+            'font_size': self.font_size,
             'bg_color': hl_bg_color,
             'font_color': hl_color,
             'align': 'left',
             'valign': 'vcenter'
         })
```

### Comparing `cicc_excel-0.2.0/cicc_excel.egg-info/PKG-INFO` & `cicc_excel-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cicc-excel
-Version: 0.2.0
+Name: cicc_excel
+Version: 0.3.0
 Summary: Library of export pandas into excel for CICCers
 Home-page: https://github.com/nyuspc/cicc_excel
 Author: Pengcheng Song
 Author-email: smth_spc@hotmail.com
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -21,15 +21,16 @@
 
 ```python
 from cicc_excel.excelwriter import ExcelWriter
 
 # create new writer
 # default font is 宋体, Arial, Times New Roman
 # to setup a percentage column, put a % in column name
-wb = ExcelWriter('export_file_name.xlsx', ch_font="中文字体", num_font="Number Font", en_font="English Font", first_row_color='#EEECE1', first_row_height=20)
+# default col width will adjust by font_size
+wb = ExcelWriter('export_file_name.xlsx', ch_font="中文字体", num_font="Number Font", en_font="English Font", first_row_color='#EEECE1', first_row_height=20, font_size=10)
 
 #load data into writer in pandas dataframe
 wb.load_data(df)
 
 #set highlight columns by name
 #color in #FFFFFF format
 wb.set_hl_col_by_names('col_name', 'sheet_name', 'background_color', 'color')
```

### Comparing `cicc_excel-0.2.0/setup.py` & `cicc_excel-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cicc_excel",
-    version="0.2.0",
+    version="0.3.0",
     author="Pengcheng Song",
     author_email="smth_spc@hotmail.com",
     description="Library of export pandas into excel for CICCers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nyuspc/cicc_excel",
     install_requires=[
```

