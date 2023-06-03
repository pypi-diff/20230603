# Comparing `tmp/chromadb-semantic-1.0.2.tar.gz` & `tmp/chromadb-semantic-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromadb-semantic-1.0.2.tar", last modified: Sat Jun  3 16:46:57 2023, max compression
+gzip compressed data, was "chromadb-semantic-1.0.3.tar", last modified: Sat Jun  3 16:51:14 2023, max compression
```

## Comparing `chromadb-semantic-1.0.2.tar` & `chromadb-semantic-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-03 16:46:57.016883 chromadb-semantic-1.0.2/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2989 2023-06-03 16:46:57.016754 chromadb-semantic-1.0.2/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)     2886 2023-06-03 16:46:56.000000 chromadb-semantic-1.0.2/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-03 16:46:57.016381 chromadb-semantic-1.0.2/chromadb_semantic.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     2989 2023-06-03 16:46:56.000000 chromadb-semantic-1.0.2/chromadb_semantic.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      287 2023-06-03 16:46:57.000000 chromadb-semantic-1.0.2/chromadb_semantic.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-06-03 16:46:56.000000 chromadb-semantic-1.0.2/chromadb_semantic.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       61 2023-06-03 16:46:56.000000 chromadb-semantic-1.0.2/chromadb_semantic.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       37 2023-06-03 16:46:56.000000 chromadb-semantic-1.0.2/chromadb_semantic.egg-info/requires.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       18 2023-06-03 16:46:56.000000 chromadb-semantic-1.0.2/chromadb_semantic.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)     1957 2023-06-03 16:46:56.000000 chromadb-semantic-1.0.2/chromadb_semantic.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-06-03 16:46:57.016931 chromadb-semantic-1.0.2/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      532 2023-06-03 16:46:56.000000 chromadb-semantic-1.0.2/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-03 16:51:14.077301 chromadb-semantic-1.0.3/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3073 2023-06-03 16:51:14.077184 chromadb-semantic-1.0.3/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)     2970 2023-06-03 16:51:13.000000 chromadb-semantic-1.0.3/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-06-03 16:51:14.077017 chromadb-semantic-1.0.3/chromadb_semantic.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     3073 2023-06-03 16:51:14.000000 chromadb-semantic-1.0.3/chromadb_semantic.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      287 2023-06-03 16:51:14.000000 chromadb-semantic-1.0.3/chromadb_semantic.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-06-03 16:51:14.000000 chromadb-semantic-1.0.3/chromadb_semantic.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       61 2023-06-03 16:51:14.000000 chromadb-semantic-1.0.3/chromadb_semantic.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       37 2023-06-03 16:51:14.000000 chromadb-semantic-1.0.3/chromadb_semantic.egg-info/requires.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       18 2023-06-03 16:51:14.000000 chromadb-semantic-1.0.3/chromadb_semantic.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)     1957 2023-06-03 16:51:13.000000 chromadb-semantic-1.0.3/chromadb_semantic.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-06-03 16:51:14.077344 chromadb-semantic-1.0.3/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      532 2023-06-03 16:51:13.000000 chromadb-semantic-1.0.3/setup.py
```

### Comparing `chromadb-semantic-1.0.2/PKG-INFO` & `chromadb-semantic-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 Metadata-Version: 2.1
 Name: chromadb-semantic
-Version: 1.0.2
+Version: 1.0.3
 Description-Content-Type: text/markdown
 
 # ChromaDB Semantic Search
 ```
-🐔動機: 「語境探索」散亂的 .pt 檔案升級為 duckdb+parquet 向量資料庫，並加入高速索引
-💣地雷: python 3.11無法編譯通過, python 3.10測試成功
+🐔動機: 
+. 高速語境探索資料庫，自然語言搜尋
+. 將「語境探索」原本散亂的文字向量 .pt 檔案群升級為 duckdb+parquet 向量資料庫，並加入高速索引
+
+💣地雷: 
+. python 3.11無法編譯通過
+. python 3.10測試成功
+
 本專案使用 [ChromaDB](https://github.com/chroma-core/chroma) 以及 [Sentence Transformers](https://github.com/UKPLab/sentence-transformers) 來實現中文與英文的語意搜尋。請按照以下的步驟進行安裝和使用。
 ```
 
 ## 安裝
 1. 先確保您已安裝 Python 3.10。
 2. 運行以下指令安裝必要的套件：
```

### Comparing `chromadb-semantic-1.0.2/README.md` & `chromadb-semantic-1.0.3/chromadb_semantic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,22 @@
+Metadata-Version: 2.1
+Name: chromadb-semantic
+Version: 1.0.3
+Description-Content-Type: text/markdown
+
 # ChromaDB Semantic Search
 ```
-🐔動機: 「語境探索」散亂的 .pt 檔案升級為 duckdb+parquet 向量資料庫，並加入高速索引
-💣地雷: python 3.11無法編譯通過, python 3.10測試成功
+🐔動機: 
+. 高速語境探索資料庫，自然語言搜尋
+. 將「語境探索」原本散亂的文字向量 .pt 檔案群升級為 duckdb+parquet 向量資料庫，並加入高速索引
+
+💣地雷: 
+. python 3.11無法編譯通過
+. python 3.10測試成功
+
 本專案使用 [ChromaDB](https://github.com/chroma-core/chroma) 以及 [Sentence Transformers](https://github.com/UKPLab/sentence-transformers) 來實現中文與英文的語意搜尋。請按照以下的步驟進行安裝和使用。
 ```
 
 ## 安裝
 1. 先確保您已安裝 Python 3.10。
 2. 運行以下指令安裝必要的套件：
 
@@ -64,8 +75,8 @@
 
 輸出示例：
 ```
 Results for query: 哪一個鄉鎮的月亮比較圓
 {'ids': [['doc2', 'doc1']], 'embeddings': None, 'documents': [['玉里鎮的月亮比較大顆', 'This is a sample docummetadatas': [[{'type': 'example'}, {'type': 'sample'}]], 'distances': [[5.628111839294434, 43.863502502441406]]}
 ```
 
-注意：第一次創建集合和添加文檔時，嵌入運算可能需要一些時間。之後的查詢將會更快。
+注意：第一次創建集合和添加文檔時，嵌入運算可能需要一些時間。之後的查詢將會更快。
```

### Comparing `chromadb-semantic-1.0.2/chromadb_semantic.egg-info/PKG-INFO` & `chromadb-semantic-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1
-Name: chromadb-semantic
-Version: 1.0.2
-Description-Content-Type: text/markdown
-
 # ChromaDB Semantic Search
 ```
-🐔動機: 「語境探索」散亂的 .pt 檔案升級為 duckdb+parquet 向量資料庫，並加入高速索引
-💣地雷: python 3.11無法編譯通過, python 3.10測試成功
+🐔動機: 
+. 高速語境探索資料庫，自然語言搜尋
+. 將「語境探索」原本散亂的文字向量 .pt 檔案群升級為 duckdb+parquet 向量資料庫，並加入高速索引
+
+💣地雷: 
+. python 3.11無法編譯通過
+. python 3.10測試成功
+
 本專案使用 [ChromaDB](https://github.com/chroma-core/chroma) 以及 [Sentence Transformers](https://github.com/UKPLab/sentence-transformers) 來實現中文與英文的語意搜尋。請按照以下的步驟進行安裝和使用。
 ```
 
 ## 安裝
 1. 先確保您已安裝 Python 3.10。
 2. 運行以下指令安裝必要的套件：
 
@@ -69,8 +70,8 @@
 
 輸出示例：
 ```
 Results for query: 哪一個鄉鎮的月亮比較圓
 {'ids': [['doc2', 'doc1']], 'embeddings': None, 'documents': [['玉里鎮的月亮比較大顆', 'This is a sample docummetadatas': [[{'type': 'example'}, {'type': 'sample'}]], 'distances': [[5.628111839294434, 43.863502502441406]]}
 ```
 
-注意：第一次創建集合和添加文檔時，嵌入運算可能需要一些時間。之後的查詢將會更快。
+注意：第一次創建集合和添加文檔時，嵌入運算可能需要一些時間。之後的查詢將會更快。
```

### Comparing `chromadb-semantic-1.0.2/chromadb_semantic.py` & `chromadb-semantic-1.0.3/chromadb_semantic.py`

 * *Files identical despite different names*

### Comparing `chromadb-semantic-1.0.2/setup.py` & `chromadb-semantic-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="chromadb-semantic",
-    version="1.0.2",
+    version="1.0.3",
     packages=find_packages(),
     py_modules=['chromadb_semantic'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'chromadb_semantic = chromadb_semantic:main',
         ],
```

