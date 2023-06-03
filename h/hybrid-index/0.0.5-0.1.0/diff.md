# Comparing `tmp/hybrid_index-0.0.5.tar.gz` & `tmp/hybrid_index-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hybrid_index-0.0.5.tar", last modified: Fri Jun  2 10:35:12 2023, max compression
+gzip compressed data, was "hybrid_index-0.1.0.tar", last modified: Fri Jun  2 09:44:51 2023, max compression
```

## Comparing `hybrid_index-0.0.5.tar` & `hybrid_index-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 gigagiova  (1000) gigagiova  (1000)        0 2023-06-02 10:35:12.370878 hybrid_index-0.0.5/
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      480 2023-06-02 10:35:12.370878 hybrid_index-0.0.5/PKG-INFO
-drwxrwxr-x   0 gigagiova  (1000) gigagiova  (1000)        0 2023-06-02 10:35:12.366878 hybrid_index-0.0.5/hybrid/
-drwxrwxr-x   0 gigagiova  (1000) gigagiova  (1000)        0 2023-06-02 10:35:12.366878 hybrid_index-0.0.5/hybrid/hybrid_index/
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)       76 2023-06-02 10:22:00.000000 hybrid_index-0.0.5/hybrid/hybrid_index/__init__.py
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)     7669 2023-06-02 10:35:03.000000 hybrid_index-0.0.5/hybrid/hybrid_index/index.py
-drwxrwxr-x   0 gigagiova  (1000) gigagiova  (1000)        0 2023-06-02 10:35:12.370878 hybrid_index-0.0.5/hybrid/hybrid_index.egg-info/
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      480 2023-06-02 10:35:12.000000 hybrid_index-0.0.5/hybrid/hybrid_index.egg-info/PKG-INFO
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      283 2023-06-02 10:35:12.000000 hybrid_index-0.0.5/hybrid/hybrid_index.egg-info/SOURCES.txt
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)        1 2023-06-02 10:35:12.000000 hybrid_index-0.0.5/hybrid/hybrid_index.egg-info/dependency_links.txt
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      268 2023-06-02 10:35:12.000000 hybrid_index-0.0.5/hybrid/hybrid_index.egg-info/requires.txt
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)       13 2023-06-02 10:35:12.000000 hybrid_index-0.0.5/hybrid/hybrid_index.egg-info/top_level.txt
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)       38 2023-06-02 10:35:12.370878 hybrid_index-0.0.5/setup.cfg
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)     1268 2023-06-02 10:35:03.000000 hybrid_index-0.0.5/setup.py
+drwxrwxr-x   0 gigagiova  (1000) gigagiova  (1000)        0 2023-06-02 09:44:51.848622 hybrid_index-0.1.0/
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      549 2023-06-02 09:44:51.848622 hybrid_index-0.1.0/PKG-INFO
+drwxrwxr-x   0 gigagiova  (1000) gigagiova  (1000)        0 2023-06-02 09:44:51.844622 hybrid_index-0.1.0/hybrid/
+drwxrwxr-x   0 gigagiova  (1000) gigagiova  (1000)        0 2023-06-02 09:44:51.848622 hybrid_index-0.1.0/hybrid/hybrid_index/
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)       83 2023-06-02 09:42:53.000000 hybrid_index-0.1.0/hybrid/hybrid_index/__init__.py
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)     7078 2023-06-02 08:36:03.000000 hybrid_index-0.1.0/hybrid/hybrid_index/index.py
+drwxrwxr-x   0 gigagiova  (1000) gigagiova  (1000)        0 2023-06-02 09:44:51.848622 hybrid_index-0.1.0/hybrid/hybrid_index.egg-info/
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      549 2023-06-02 09:44:51.000000 hybrid_index-0.1.0/hybrid/hybrid_index.egg-info/PKG-INFO
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      308 2023-06-02 09:44:51.000000 hybrid_index-0.1.0/hybrid/hybrid_index.egg-info/SOURCES.txt
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)        1 2023-06-02 09:44:51.000000 hybrid_index-0.1.0/hybrid/hybrid_index.egg-info/dependency_links.txt
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      393 2023-06-02 09:44:51.000000 hybrid_index-0.1.0/hybrid/hybrid_index.egg-info/requires.txt
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)       13 2023-06-02 09:44:51.000000 hybrid_index-0.1.0/hybrid/hybrid_index.egg-info/top_level.txt
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      968 2023-06-02 09:14:47.000000 hybrid_index-0.1.0/pyproject.toml
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      555 2023-06-02 09:44:51.848622 hybrid_index-0.1.0/setup.cfg
+-rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)     1464 2023-06-02 09:43:20.000000 hybrid_index-0.1.0/setup.py
```

### Comparing `hybrid_index-0.0.5/hybrid/hybrid_index/index.py` & `hybrid_index-0.1.0/hybrid/hybrid_index/index.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,30 +6,15 @@
 import faiss
 import nltk
 from faiss import IndexIDMap, IndexFlatIP
 from nltk import RegexpTokenizer
 import numpy as np
 
 
-def openai_emb(passages: List[str]):
-
-    chunk_size = 100
-    arr = np.empty((0, 1536)).astype('float32')
-
-    for i in range(0, len(passages), chunk_size):
-        chunk = passages[i:min(i + chunk_size, len(passages))]
-        res = openai.Embedding.create(
-            input=chunk,
-            engine='text-embedding-ada-002'
-        )
-        arr = np.concatenate((arr, np.array([r['embedding'] for r in res['data']]).astype('float32')), axis=0)
-
-    return arr
-
-async def openai_aemb(passages: List[str]):
+async def openai_emb(passages: List[str]):
 
     chunk_size = 100
     arr = np.empty((0, 1536)).astype('float32')
 
     for i in range(0, len(passages), chunk_size):
         chunk = passages[i:min(i + chunk_size, len(passages))]
         res = await openai.Embedding.acreate(
@@ -37,14 +22,15 @@
             engine='text-embedding-ada-002'
         )
         arr = np.concatenate((arr, np.array([r['embedding'] for r in res['data']]).astype('float32')), axis=0)
 
     return arr
 
 
+
 def normalize_array(array: np.ndarray, infimum: int = None):
     """
     This technique was taken from
     :param array:
     :param infimum:
     :return:
     """
@@ -174,26 +160,23 @@
         embeddings = await openai_emb(documents)
         self.semantic_index.add(embeddings)
 
         self.id_map.extend(ids)
 
     async def query(self, query: str, top_n: int):
 
-        # Get 10 times more results from each index to compare them
-        query_length = min(top_n * 10, len(self.id_map))
-
         # Get semantic results
-        query_vector = openai_emb([query])
-        faiss_scores, faiss_indices = self.semantic_index.search(query_vector, query_length)
+        query_vector = await openai_emb([query])
+        faiss_scores, faiss_indices = self.semantic_index.search(query_vector, top_n * 10)
         faiss_scores, faiss_indices = normalize_array(faiss_scores[0], -1), faiss_indices[0]
         faiss_result = {self.id_map[r]: faiss_scores[idx] for idx, r in enumerate(faiss_indices)}
 
         # Returns the top n results in order from the bm25 index
         bm25_scores = self.lexical_index.get_scores(query)
-        bm25_results = sorted(range(len(bm25_scores)), key=lambda i: bm25_scores[i], reverse=True)[:query_length]
+        bm25_results = sorted(range(len(bm25_scores)), key=lambda i: bm25_scores[i], reverse=True)[:top_n * 10]
         bm25_result = {self.id_map[r]: bm25_scores[r] for r in bm25_results}
 
         # Combine results
         combined_scores = {}
         for id in set(list(faiss_result.keys()) + list(bm25_result.keys())):
             faiss_score = faiss_result.get(id, 0)
             bm25_score = bm25_result.get(id, 0)
```

### Comparing `hybrid_index-0.0.5/setup.py` & `hybrid_index-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("hybrid/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="hybrid_index",
-    version="0.0.5",
+    version="0.0.10",
     description="Easy to use hybrid index for semantic + keyword search",
     package_dir={"": "hybrid"},
     packages=find_packages(where="hybrid"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gigagiova/hybrid-index",
     author="Giovanni del Gallo",
@@ -17,30 +17,37 @@
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ],
     install_requires=[
+      "aiohttp >=3.8.4",
+      "aiosignal >=1.3.1",
+      "async-timeout >=4.0.2",
       "attrs >=23.1.0",
+      "certifi >=2023.5.7",
       "charset-normalizer >=3.1.0",
       "click",
       "distlib >=0.3.6",
       "faiss-gpu >=1.7.2",
       "filelock >=3.10.7",
       "frozenlist >=1.3.3",
       "idna >=3.4",
+      "mkl-fft >=1.3.6",
+      "mkl-service >=2.4.0",
       "multidict >=6.0.4",
       "nltk",
       "numpy",
       "openai >=0.27.7",
       "platformdirs >=3.2.0",
       "regex",
       "requests >=2.31.0",
       "urllib3 >=2.0.2",
+      "virtualenv >=20.21.0",
       "yarl >=1.9.2",
     ],
     extras_require={
         "dev": ["pytest>=7.0", "twine>=4.0.2"],
     },
     python_requires=">=3.10",
 )
```

