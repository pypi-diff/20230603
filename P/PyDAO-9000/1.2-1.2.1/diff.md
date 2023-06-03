# Comparing `tmp/PyDAO_9000-1.2.tar.gz` & `tmp/PyDAO_9000-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDAO_9000-1.2.tar", last modified: Sat May 27 15:57:40 2023, max compression
+gzip compressed data, was "PyDAO_9000-1.2.1.tar", last modified: Sat Jun  3 13:24:50 2023, max compression
```

## Comparing `PyDAO_9000-1.2.tar` & `PyDAO_9000-1.2.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 15:57:40.155782 PyDAO_9000-1.2/
--rw-rw-rw-   0        0        0     1090 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/LICENSE
--rw-rw-rw-   0        0        0     4209 2023-05-27 15:57:40.155782 PyDAO_9000-1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-27 15:57:40.030781 PyDAO_9000-1.2/PyDAO_9000.egg-info/
--rw-rw-rw-   0        0        0     4209 2023-05-27 15:57:39.000000 PyDAO_9000-1.2/PyDAO_9000.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1040 2023-05-27 15:57:39.000000 PyDAO_9000-1.2/PyDAO_9000.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 15:57:39.000000 PyDAO_9000-1.2/PyDAO_9000.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-27 15:57:39.000000 PyDAO_9000-1.2/PyDAO_9000.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3695 2023-05-27 15:38:38.000000 PyDAO_9000-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 15:57:40.062030 PyDAO_9000-1.2/SqltDAO/
-drwxrwxrwx   0        0        0        0 2023-05-27 15:57:40.093280 PyDAO_9000-1.2/SqltDAO/CodeGen01/
--rw-rw-rw-   0        0        0     3108 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/CodeGen01/CodeGen.py
--rw-rw-rw-   0        0        0      865 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/CodeGen01/CodeLevel.py
--rw-rw-rw-   0        0        0      264 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/CodeGen01/DaoExceptions.py
--rw-rw-rw-   0        0        0      475 2023-05-27 15:22:37.000000 PyDAO_9000-1.2/SqltDAO/CodeGen01/Meta.py
--rw-rw-rw-   0        0        0     1816 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/CodeGen01/Normalizers.py
--rw-rw-rw-   0        0        0     4309 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/CodeGen01/OrderClass.py
--rw-rw-rw-   0        0        0    12389 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/CodeGen01/SqlSyntax.py
--rw-rw-rw-   0        0        0     7315 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/CodeGen01/TextDataDetector.py
--rw-rw-rw-   0        0        0    13912 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/CrudMeister.py
-drwxrwxrwx   0        0        0        0 2023-05-27 15:57:40.108907 PyDAO_9000-1.2/SqltDAO/DaoTest01/
--rw-rw-rw-   0        0        0      678 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/DaoTest01/GenNasdaq.py
--rw-rw-rw-   0        0        0      507 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/DaoTest01/GenNasdaqTest.py
--rw-rw-rw-   0        0        0     3252 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/DaoTest01/Income.py
--rw-rw-rw-   0        0        0     3054 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/DaoTest01/NasdaqDAO.py
--rw-rw-rw-   0        0        0     3488 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/DaoTest01/foo.py
--rw-rw-rw-   0        0        0      847 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/DaoTest01/tc001_driver.py
--rw-rw-rw-   0        0        0      691 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/DaoTest01/tc001_gen.py
--rw-rw-rw-   0        0        0     2923 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/Demo123.py
-drwxrwxrwx   0        0        0        0 2023-05-27 15:57:40.140152 PyDAO_9000-1.2/SqltDAO/Gui/
--rw-rw-rw-   0        0        0     6185 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/Gui/Data2Code.py
--rw-rw-rw-   0        0        0     6553 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/Gui/DataAI.py
--rw-rw-rw-   0        0        0     4628 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/Gui/DataFrameOne.py
--rw-rw-rw-   0        0        0     4892 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/Gui/DataPreferences.py
--rw-rw-rw-   0        0        0     4771 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/Gui/StandardEntry.py
--rw-rw-rw-   0        0        0     6403 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/Gui/TableDef.py
--rw-rw-rw-   0        0        0     3504 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/Ledger.py
-drwxrwxrwx   0        0        0        0 2023-05-27 15:57:40.140152 PyDAO_9000-1.2/SqltDAO/SchemaDef/
--rw-rw-rw-   0        0        0     8393 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/SchemaDef/DataDetective.py
--rw-rw-rw-   0        0        0     9378 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/SchemaDef/Factory.py
--rw-rw-rw-   0        0        0     8987 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/SchemaDef/OrderDef.py
--rw-rw-rw-   0        0        0     3179 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/SchemaDef/Table.py
--rw-rw-rw-   0        0        0     3602 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/UpdateTestCase.py
--rw-rw-rw-   0        0        0      103 2023-05-27 11:01:18.000000 PyDAO_9000-1.2/SqltDAO/__init__.py
--rw-rw-rw-   0        0        0     7747 2023-05-27 15:38:24.000000 PyDAO_9000-1.2/SqltDAO/main.py
--rw-rw-rw-   0        0        0      503 2023-05-27 15:52:15.000000 PyDAO_9000-1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 15:57:40.155782 PyDAO_9000-1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-03 13:24:50.494898 PyDAO_9000-1.2.1/
+-rw-rw-rw-   0        0        0     1090 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4213 2023-06-03 13:24:50.494898 PyDAO_9000-1.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-03 13:24:50.073030 PyDAO_9000-1.2.1/PyDAO_9000.egg-info/
+-rw-rw-rw-   0        0        0     4213 2023-06-03 13:24:49.000000 PyDAO_9000-1.2.1/PyDAO_9000.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1040 2023-06-03 13:24:50.000000 PyDAO_9000-1.2.1/PyDAO_9000.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 13:24:49.000000 PyDAO_9000-1.2.1/PyDAO_9000.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-03 13:24:49.000000 PyDAO_9000-1.2.1/PyDAO_9000.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3695 2023-06-03 13:10:19.000000 PyDAO_9000-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 13:24:50.151156 PyDAO_9000-1.2.1/SqltDAO/
+drwxrwxrwx   0        0        0        0 2023-06-03 13:24:50.244926 PyDAO_9000-1.2.1/SqltDAO/CodeGen01/
+-rw-rw-rw-   0        0        0     3108 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/CodeGen01/CodeGen.py
+-rw-rw-rw-   0        0        0      865 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/CodeGen01/CodeLevel.py
+-rw-rw-rw-   0        0        0      264 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/CodeGen01/DaoExceptions.py
+-rw-rw-rw-   0        0        0      478 2023-06-03 13:21:24.000000 PyDAO_9000-1.2.1/SqltDAO/CodeGen01/Meta.py
+-rw-rw-rw-   0        0        0     1816 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/CodeGen01/Normalizers.py
+-rw-rw-rw-   0        0        0     4309 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/CodeGen01/OrderClass.py
+-rw-rw-rw-   0        0        0    12415 2023-06-03 13:14:31.000000 PyDAO_9000-1.2.1/SqltDAO/CodeGen01/SqlSyntax.py
+-rw-rw-rw-   0        0        0     7315 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/CodeGen01/TextDataDetector.py
+-rw-rw-rw-   0        0        0    13912 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/CrudMeister.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:24:50.338655 PyDAO_9000-1.2.1/SqltDAO/DaoTest01/
+-rw-rw-rw-   0        0        0      678 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/DaoTest01/GenNasdaq.py
+-rw-rw-rw-   0        0        0      507 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/DaoTest01/GenNasdaqTest.py
+-rw-rw-rw-   0        0        0     3252 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/DaoTest01/Income.py
+-rw-rw-rw-   0        0        0     3054 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/DaoTest01/NasdaqDAO.py
+-rw-rw-rw-   0        0        0     3488 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/DaoTest01/foo.py
+-rw-rw-rw-   0        0        0      847 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/DaoTest01/tc001_driver.py
+-rw-rw-rw-   0        0        0      691 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/DaoTest01/tc001_gen.py
+-rw-rw-rw-   0        0        0     2923 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/Demo123.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:24:50.432398 PyDAO_9000-1.2.1/SqltDAO/Gui/
+-rw-rw-rw-   0        0        0     6185 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/Gui/Data2Code.py
+-rw-rw-rw-   0        0        0     6553 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/Gui/DataAI.py
+-rw-rw-rw-   0        0        0     4628 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/Gui/DataFrameOne.py
+-rw-rw-rw-   0        0        0     4892 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/Gui/DataPreferences.py
+-rw-rw-rw-   0        0        0     4771 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/Gui/StandardEntry.py
+-rw-rw-rw-   0        0        0     6403 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/Gui/TableDef.py
+-rw-rw-rw-   0        0        0     3504 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/Ledger.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:24:50.479272 PyDAO_9000-1.2.1/SqltDAO/SchemaDef/
+-rw-rw-rw-   0        0        0     8393 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/SchemaDef/DataDetective.py
+-rw-rw-rw-   0        0        0     9378 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/SchemaDef/Factory.py
+-rw-rw-rw-   0        0        0     8987 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/SchemaDef/OrderDef.py
+-rw-rw-rw-   0        0        0     3179 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/SchemaDef/Table.py
+-rw-rw-rw-   0        0        0     3602 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/UpdateTestCase.py
+-rw-rw-rw-   0        0        0      103 2023-05-27 11:01:18.000000 PyDAO_9000-1.2.1/SqltDAO/__init__.py
+-rw-rw-rw-   0        0        0     7751 2023-06-03 13:21:45.000000 PyDAO_9000-1.2.1/SqltDAO/main.py
+-rw-rw-rw-   0        0        0      506 2023-06-03 13:23:45.000000 PyDAO_9000-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 13:24:50.494898 PyDAO_9000-1.2.1/setup.cfg
```

### Comparing `PyDAO_9000-1.2/LICENSE` & `PyDAO_9000-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/PKG-INFO` & `PyDAO_9000-1.2.1/PyDAO_9000.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: PyDAO_9000
-Version: 1.2
-Summary: All-In-One File SQL Code Generator
+Name: PyDAO-9000
+Version: 1.2.1
+Summary: 'All-In-One File' SQL Code Generator
 Author-email: Randall Nagy <r.a.nagy@gmail.com>
 Project-URL: Homepage, https://github.com/soft9000/PyDAO
 Project-URL: Bug Tracker, https://github.com/soft9000/PyDAO/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -36,15 +36,15 @@
 All four (4) workflows are supported - feel free to give each a try!
 
 
 The GUI
 -------
 ![PyDAO GUI](PyDAO_GUI.png)
 
-Years latter the project is working well enough to declare what we have as an [Official PyPy Package](https://pypi.org/project/PyDAO-9000/).
+Years latter the project is working well enough to declare what we have as an [Official PyPi Package](https://pypi.org/project/PyDAO-9000/).
 
 Once installed most will probably want to use the GUI:
 
 ```
 >>> from SqltDAO import main as PyDAO
 >>> PyDAO.Main.mainloop()
 ```
```

### Comparing `PyDAO_9000-1.2/PyDAO_9000.egg-info/PKG-INFO` & `PyDAO_9000-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: PyDAO-9000
-Version: 1.2
-Summary: All-In-One File SQL Code Generator
+Name: PyDAO_9000
+Version: 1.2.1
+Summary: 'All-In-One File' SQL Code Generator
 Author-email: Randall Nagy <r.a.nagy@gmail.com>
 Project-URL: Homepage, https://github.com/soft9000/PyDAO
 Project-URL: Bug Tracker, https://github.com/soft9000/PyDAO/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -36,15 +36,15 @@
 All four (4) workflows are supported - feel free to give each a try!
 
 
 The GUI
 -------
 ![PyDAO GUI](PyDAO_GUI.png)
 
-Years latter the project is working well enough to declare what we have as an [Official PyPy Package](https://pypi.org/project/PyDAO-9000/).
+Years latter the project is working well enough to declare what we have as an [Official PyPi Package](https://pypi.org/project/PyDAO-9000/).
 
 Once installed most will probably want to use the GUI:
 
 ```
 >>> from SqltDAO import main as PyDAO
 >>> PyDAO.Main.mainloop()
 ```
```

### Comparing `PyDAO_9000-1.2/PyDAO_9000.egg-info/SOURCES.txt` & `PyDAO_9000-1.2.1/PyDAO_9000.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/README.md` & `PyDAO_9000-1.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 All four (4) workflows are supported - feel free to give each a try!
 
 
 The GUI
 -------
 ![PyDAO GUI](PyDAO_GUI.png)
 
-Years latter the project is working well enough to declare what we have as an [Official PyPy Package](https://pypi.org/project/PyDAO-9000/).
+Years latter the project is working well enough to declare what we have as an [Official PyPi Package](https://pypi.org/project/PyDAO-9000/).
 
 Once installed most will probably want to use the GUI:
 
 ```
 >>> from SqltDAO import main as PyDAO
 >>> PyDAO.Main.mainloop()
 ```
```

### Comparing `PyDAO_9000-1.2/SqltDAO/CodeGen01/CodeGen.py` & `PyDAO_9000-1.2.1/SqltDAO/CodeGen01/CodeGen.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/CodeGen01/CodeLevel.py` & `PyDAO_9000-1.2.1/SqltDAO/CodeGen01/CodeLevel.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/CodeGen01/Normalizers.py` & `PyDAO_9000-1.2.1/SqltDAO/CodeGen01/Normalizers.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/CodeGen01/OrderClass.py` & `PyDAO_9000-1.2.1/SqltDAO/CodeGen01/OrderClass.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/CodeGen01/SqlSyntax.py` & `PyDAO_9000-1.2.1/SqltDAO/CodeGen01/SqlSyntax.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,14 +177,15 @@
         self.level.inc();
         result += self.level.print("pass")
         self.level.dec()
         self.level.dec()
         result += self.level.print("return None")
         result += self.level.print("")
         self.level.dec()
+        self.level.dec()
 
         self.level.push()
         result += self.level.print("@staticmethod")
         if self.order.encoding:
             encoding = "'" + self.order.encoding + "'"
         else:
             encoding = str(self.order.encoding)
```

### Comparing `PyDAO_9000-1.2/SqltDAO/CodeGen01/TextDataDetector.py` & `PyDAO_9000-1.2.1/SqltDAO/CodeGen01/TextDataDetector.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/CrudMeister.py` & `PyDAO_9000-1.2.1/SqltDAO/CrudMeister.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/DaoTest01/GenNasdaq.py` & `PyDAO_9000-1.2.1/SqltDAO/DaoTest01/GenNasdaq.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/DaoTest01/Income.py` & `PyDAO_9000-1.2.1/SqltDAO/DaoTest01/Income.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/DaoTest01/NasdaqDAO.py` & `PyDAO_9000-1.2.1/SqltDAO/DaoTest01/NasdaqDAO.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/DaoTest01/foo.py` & `PyDAO_9000-1.2.1/SqltDAO/DaoTest01/foo.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/DaoTest01/tc001_driver.py` & `PyDAO_9000-1.2.1/SqltDAO/DaoTest01/tc001_driver.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/DaoTest01/tc001_gen.py` & `PyDAO_9000-1.2.1/SqltDAO/DaoTest01/tc001_gen.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/Demo123.py` & `PyDAO_9000-1.2.1/SqltDAO/Demo123.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/Gui/Data2Code.py` & `PyDAO_9000-1.2.1/SqltDAO/Gui/Data2Code.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/Gui/DataAI.py` & `PyDAO_9000-1.2.1/SqltDAO/Gui/DataAI.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/Gui/DataFrameOne.py` & `PyDAO_9000-1.2.1/SqltDAO/Gui/DataFrameOne.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/Gui/DataPreferences.py` & `PyDAO_9000-1.2.1/SqltDAO/Gui/DataPreferences.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/Gui/StandardEntry.py` & `PyDAO_9000-1.2.1/SqltDAO/Gui/StandardEntry.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/Gui/TableDef.py` & `PyDAO_9000-1.2.1/SqltDAO/Gui/TableDef.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/Ledger.py` & `PyDAO_9000-1.2.1/SqltDAO/Ledger.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/SchemaDef/DataDetective.py` & `PyDAO_9000-1.2.1/SqltDAO/SchemaDef/DataDetective.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/SchemaDef/Factory.py` & `PyDAO_9000-1.2.1/SqltDAO/SchemaDef/Factory.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/SchemaDef/OrderDef.py` & `PyDAO_9000-1.2.1/SqltDAO/SchemaDef/OrderDef.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/SchemaDef/Table.py` & `PyDAO_9000-1.2.1/SqltDAO/SchemaDef/Table.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/UpdateTestCase.py` & `PyDAO_9000-1.2.1/SqltDAO/UpdateTestCase.py`

 * *Files identical despite different names*

### Comparing `PyDAO_9000-1.2/SqltDAO/main.py` & `PyDAO_9000-1.2.1/SqltDAO/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 #
 # Author: Soft9000.com
-# 2018/11/24: Project Begun
+# 2018/11/24: GUI Project Begun
 
 # Mission: Create a graphical user interface to PyDAO.
-# Status: WORK IN PROGRESS
+# Status: Released to PyPi
 
 import os
 import sys
 sys.path.insert(1, os.path.join(sys.path[0], '..'))
 
 from tkinter import *
 from tkinter import messagebox
```

