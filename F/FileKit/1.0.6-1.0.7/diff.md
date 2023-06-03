# Comparing `tmp/FileKit-1.0.6.tar.gz` & `tmp/FileKit-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FileKit-1.0.6.tar", last modified: Sat Jun  3 09:30:18 2023, max compression
+gzip compressed data, was "FileKit-1.0.7.tar", last modified: Sat Jun  3 09:35:42 2023, max compression
```

## Comparing `FileKit-1.0.6.tar` & `FileKit-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 09:30:18.812263 FileKit-1.0.6/
-drwxrwxrwx   0        0        0        0 2023-06-03 09:30:18.807276 FileKit-1.0.6/FileKit/
--rw-rw-rw-   0        0        0     1462 2023-06-03 09:29:32.000000 FileKit-1.0.6/FileKit/File.py
--rw-rw-rw-   0        0        0       21 2023-06-02 08:25:07.000000 FileKit-1.0.6/FileKit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 09:30:18.811266 FileKit-1.0.6/FileKit.egg-info/
--rw-rw-rw-   0        0        0      669 2023-06-03 09:30:18.000000 FileKit-1.0.6/FileKit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-03 09:30:18.000000 FileKit-1.0.6/FileKit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 09:30:18.000000 FileKit-1.0.6/FileKit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-03 09:30:18.000000 FileKit-1.0.6/FileKit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      669 2023-06-03 09:30:18.812263 FileKit-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      556 2023-06-01 14:32:32.000000 FileKit-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-03 09:30:18.813263 FileKit-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      415 2023-06-03 09:29:49.000000 FileKit-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 09:35:42.110823 FileKit-1.0.7/
+drwxrwxrwx   0        0        0        0 2023-06-03 09:35:42.105247 FileKit-1.0.7/FileKit/
+-rw-rw-rw-   0        0        0     1462 2023-06-03 09:35:23.000000 FileKit-1.0.7/FileKit/File.py
+-rw-rw-rw-   0        0        0       21 2023-06-02 08:25:07.000000 FileKit-1.0.7/FileKit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 09:35:42.109824 FileKit-1.0.7/FileKit.egg-info/
+-rw-rw-rw-   0        0        0      669 2023-06-03 09:35:42.000000 FileKit-1.0.7/FileKit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-03 09:35:42.000000 FileKit-1.0.7/FileKit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 09:35:42.000000 FileKit-1.0.7/FileKit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-03 09:35:42.000000 FileKit-1.0.7/FileKit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      669 2023-06-03 09:35:42.110823 FileKit-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2023-06-01 14:32:32.000000 FileKit-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-03 09:35:42.111821 FileKit-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      415 2023-06-03 09:35:40.000000 FileKit-1.0.7/setup.py
```

### Comparing `FileKit-1.0.6/FileKit/File.py` & `FileKit-1.0.7/FileKit/File.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     file.close()
     return text
 
 
 def write(file_name, text, encoding='utf-8', mode='w'):
     """  覆盖模式写入文本文件内容， 如果文件不存在会新建 """
     if mode == 'wb':
-        file = open(file_name, mode=mode, encoding=encoding)
-    else:
         file = open(file_name, mode=mode)
+    else:
+        file = open(file_name, mode=mode, encoding=encoding)
     file.write(text)
     file.close()
 
 
 def read_lines(file_name, encoding='utf-8'):
     """  读取文件为数组 """
     file = open(file_name, mode='r', encoding=encoding)
```

### Comparing `FileKit-1.0.6/FileKit.egg-info/PKG-INFO` & `FileKit-1.0.7/FileKit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FileKit
-Version: 1.0.6
+Version: 1.0.7
 Author: 孙亮
 Description-Content-Type: text/markdown
 
 # Filekit
 
 简易使用 Python 的文件读写内置模块，针对单词读写操作。省去 open 和 close。
```

### Comparing `FileKit-1.0.6/PKG-INFO` & `FileKit-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FileKit
-Version: 1.0.6
+Version: 1.0.7
 Author: 孙亮
 Description-Content-Type: text/markdown
 
 # Filekit
 
 简易使用 Python 的文件读写内置模块，针对单词读写操作。省去 open 和 close。
```

### Comparing `FileKit-1.0.6/README.md` & `FileKit-1.0.7/README.md`

 * *Files identical despite different names*

