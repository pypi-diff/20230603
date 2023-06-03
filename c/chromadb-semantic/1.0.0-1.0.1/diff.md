# Comparing `tmp/chromadb-semantic-1.0.0.tar.gz` & `tmp/chromadb-semantic-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromadb-semantic-1.0.0.tar", last modified: Sat Jun  3 16:41:41 2023, max compression
+gzip compressed data, was "chromadb-semantic-1.0.1.tar", last modified: Sat Jun  3 16:45:13 2023, max compression
```

## Comparing `chromadb-semantic-1.0.0.tar` & `chromadb-semantic-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-03 16:41:41.869964 chromadb-semantic-1.0.0/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2814 2023-06-03 16:41:41.869824 chromadb-semantic-1.0.0/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     2711 2023-06-03 16:41:41.000000 chromadb-semantic-1.0.0/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-03 16:41:41.869589 chromadb-semantic-1.0.0/chromadb_semantic.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2814 2023-06-03 16:41:41.000000 chromadb-semantic-1.0.0/chromadb_semantic.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      287 2023-06-03 16:41:41.000000 chromadb-semantic-1.0.0/chromadb_semantic.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-06-03 16:41:41.000000 chromadb-semantic-1.0.0/chromadb_semantic.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       61 2023-06-03 16:41:41.000000 chromadb-semantic-1.0.0/chromadb_semantic.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       37 2023-06-03 16:41:41.000000 chromadb-semantic-1.0.0/chromadb_semantic.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       18 2023-06-03 16:41:41.000000 chromadb-semantic-1.0.0/chromadb_semantic.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     1957 2023-06-03 16:41:41.000000 chromadb-semantic-1.0.0/chromadb_semantic.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-06-03 16:41:41.870009 chromadb-semantic-1.0.0/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      532 2023-06-03 16:41:41.000000 chromadb-semantic-1.0.0/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-03 16:45:13.986749 chromadb-semantic-1.0.1/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3018 2023-06-03 16:45:13.986627 chromadb-semantic-1.0.1/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2915 2023-06-03 16:45:13.000000 chromadb-semantic-1.0.1/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-03 16:45:13.986459 chromadb-semantic-1.0.1/chromadb_semantic.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3018 2023-06-03 16:45:13.000000 chromadb-semantic-1.0.1/chromadb_semantic.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      287 2023-06-03 16:45:13.000000 chromadb-semantic-1.0.1/chromadb_semantic.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-06-03 16:45:13.000000 chromadb-semantic-1.0.1/chromadb_semantic.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       61 2023-06-03 16:45:13.000000 chromadb-semantic-1.0.1/chromadb_semantic.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       37 2023-06-03 16:45:13.000000 chromadb-semantic-1.0.1/chromadb_semantic.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       18 2023-06-03 16:45:13.000000 chromadb-semantic-1.0.1/chromadb_semantic.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     1957 2023-06-03 16:45:13.000000 chromadb-semantic-1.0.1/chromadb_semantic.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-06-03 16:45:13.986786 chromadb-semantic-1.0.1/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      532 2023-06-03 16:45:13.000000 chromadb-semantic-1.0.1/setup.py
```

### Comparing `chromadb-semantic-1.0.0/PKG-INFO` & `chromadb-semantic-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Metadata-Version: 2.1
 Name: chromadb-semantic
-Version: 1.0.0
+Version: 1.0.1
 Description-Content-Type: text/markdown
 
 # ChromaDB Semantic Search
+```
+🐔動機: 要升級, 讓「語境探索」散亂 .pt 檔案變成 duckdb+parquet 資料庫形式，並加入高速索引功能
+💣地雷: python 3.11無法編譯通過, python 3.10測試成功
 本專案使用 [ChromaDB](https://github.com/chroma-core/chroma) 以及 [Sentence Transformers](https://github.com/UKPLab/sentence-transformers) 來實現中文與英文的語意搜尋。請按照以下的步驟進行安裝和使用。
+```
 
 ## 安裝
 1. 先確保您已安裝 Python 3.8 或更高版本。
 2. 運行以下指令安裝必要的套件：
 
 ```bash
 python -m pip install chromadb-semantic
```

### Comparing `chromadb-semantic-1.0.0/README.md` & `chromadb-semantic-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # ChromaDB Semantic Search
+```
+🐔動機: 要升級, 讓「語境探索」散亂 .pt 檔案變成 duckdb+parquet 資料庫形式，並加入高速索引功能
+💣地雷: python 3.11無法編譯通過, python 3.10測試成功
 本專案使用 [ChromaDB](https://github.com/chroma-core/chroma) 以及 [Sentence Transformers](https://github.com/UKPLab/sentence-transformers) 來實現中文與英文的語意搜尋。請按照以下的步驟進行安裝和使用。
+```
 
 ## 安裝
 1. 先確保您已安裝 Python 3.8 或更高版本。
 2. 運行以下指令安裝必要的套件：
 
 ```bash
 python -m pip install chromadb-semantic
```

### Comparing `chromadb-semantic-1.0.0/chromadb_semantic.egg-info/PKG-INFO` & `chromadb-semantic-1.0.1/chromadb_semantic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Metadata-Version: 2.1
 Name: chromadb-semantic
-Version: 1.0.0
+Version: 1.0.1
 Description-Content-Type: text/markdown
 
 # ChromaDB Semantic Search
+```
+🐔動機: 要升級, 讓「語境探索」散亂 .pt 檔案變成 duckdb+parquet 資料庫形式，並加入高速索引功能
+💣地雷: python 3.11無法編譯通過, python 3.10測試成功
 本專案使用 [ChromaDB](https://github.com/chroma-core/chroma) 以及 [Sentence Transformers](https://github.com/UKPLab/sentence-transformers) 來實現中文與英文的語意搜尋。請按照以下的步驟進行安裝和使用。
+```
 
 ## 安裝
 1. 先確保您已安裝 Python 3.8 或更高版本。
 2. 運行以下指令安裝必要的套件：
 
 ```bash
 python -m pip install chromadb-semantic
```

### Comparing `chromadb-semantic-1.0.0/chromadb_semantic.py` & `chromadb-semantic-1.0.1/chromadb_semantic.py`

 * *Files identical despite different names*

### Comparing `chromadb-semantic-1.0.0/setup.py` & `chromadb-semantic-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="chromadb-semantic",
-    version="1.0.0",
+    version="1.0.1",
     packages=find_packages(),
     py_modules=['chromadb_semantic'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'chromadb_semantic = chromadb_semantic:main',
         ],
```

