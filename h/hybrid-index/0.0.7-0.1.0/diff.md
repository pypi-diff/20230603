# Comparing `tmp/hybrid_index-0.0.7.tar.gz` & `tmp/hybrid_index-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hybrid_index-0.0.7.tar", last modified: Sat Jun  3 19:57:00 2023, max compression
+gzip compressed data, was "hybrid_index-0.1.0.tar", last modified: Fri Jun  2 09:44:51 2023, max compression
```

## Comparing `hybrid_index-0.0.7.tar` & `hybrid_index-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 gigagiova  (1000) gigagiova  (1000)        0 2023-06-03 19:57:00.002677 hybrid_index-0.0.7/
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)     3618 2023-06-03 19:57:00.002677 hybrid_index-0.0.7/PKG-INFO
-drwxrwxr-x   0 gigagiova  (1000) gigagiova  (1000)        0 2023-06-03 19:56:59.998677 hybrid_index-0.0.7/hybrid/
-drwxrwxr-x   0 gigagiova  (1000) gigagiova  (1000)        0 2023-06-03 19:56:59.998677 hybrid_index-0.0.7/hybrid/hybrid_index/
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)       76 2023-06-02 10:22:00.000000 hybrid_index-0.0.7/hybrid/hybrid_index/__init__.py
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)     8394 2023-06-03 19:56:38.000000 hybrid_index-0.0.7/hybrid/hybrid_index/index.py
-drwxrwxr-x   0 gigagiova  (1000) gigagiova  (1000)        0 2023-06-03 19:57:00.002677 hybrid_index-0.0.7/hybrid/hybrid_index.egg-info/
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)     3618 2023-06-03 19:56:59.000000 hybrid_index-0.0.7/hybrid/hybrid_index.egg-info/PKG-INFO
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      283 2023-06-03 19:56:59.000000 hybrid_index-0.0.7/hybrid/hybrid_index.egg-info/SOURCES.txt
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)        1 2023-06-03 19:56:59.000000 hybrid_index-0.0.7/hybrid/hybrid_index.egg-info/dependency_links.txt
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)      175 2023-06-03 19:56:59.000000 hybrid_index-0.0.7/hybrid/hybrid_index.egg-info/requires.txt
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)       13 2023-06-03 19:56:59.000000 hybrid_index-0.0.7/hybrid/hybrid_index.egg-info/top_level.txt
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)       38 2023-06-03 19:57:00.002677 hybrid_index-0.0.7/setup.cfg
--rw-rw-r--   0 gigagiova  (1000) gigagiova  (1000)     1162 2023-06-03 19:56:58.000000 hybrid_index-0.0.7/setup.py
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

### Comparing `hybrid_index-0.0.7/hybrid/hybrid_index/index.py` & `hybrid_index-0.1.0/hybrid/hybrid_index/index.py`

 * *Files 12% similar despite different names*

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
@@ -134,131 +120,99 @@
             score += (self.idf.get(q) or 0) * (self.delta + (q_freq * (self.k1 + 1)) /
                                                (self.k1 * (1 - self.b + self.b * doc_len / self.avgdl) + q_freq))
 
         # Returns the normalized scores, 0 is the infimum of BM25
         return normalize_array(score, 0)
 
 
-class Index:
-    id_map: List
-
-    def __init__(self):
-        # Mapping from ids to unique string ids
-        self.id_map = []
-
-    def serialize(self):
-
-        # Create a dictionary representation of your object
-        data = self.__dict__
-
-        if 'semantic_index' in data:
-            # Serialize the index to a byte array
-            data['semantic_index'] = faiss.serialize_index(self.semantic_index)
-
-        # Pickle the dictionary
-        return pickle.dumps(data)
-
-    @classmethod
-    def deserialize(cls, pickled_data: dict, openai_key: str = None):
-
-        # Sets the openai key
-        if openai_key:
-            openai.api_key = openai_key
-
-        # Unpickle the data
-        data = pickle.loads(pickled_data)
-
-        if 'semantic_index' in data:
-            # Deserializes the faiss index
-            data['semantic_index'] = faiss.deserialize_index(data['semantic_index'])
-
-        instance = cls.__new__(cls)
-        instance.__dict__.update(data)
-        return instance
-
-
-class SemanticIndex(Index):
+class HybridIndex:
+    a: float
+    index_id: str
     openai_key: str
+    id_map: List
     semantic_index: IndexFlatIP
+    lexical_index: BM25OPlus
 
-    def __init__(self, openai_key: str = None):
+    def __init__(self, index_id: str, openai_key: str = None, a: float = 0.7):
+        self.index_id = index_id
+        self.a = a
 
-        super().__init__()
         if openai_key:
             openai.api_key = openai_key
 
-        # Sets up the faiss index with OpenAI embedding dimensions
-        self.semantic_index = IndexFlatIP(1536)
-
-    async def add(self, corpus: List[Tuple[str, str]]):
-        ids, documents = zip(*corpus)
-
-        # Get embeddings for new documents and adds them into the index
-        embeddings = await openai_emb(documents)
-        self.semantic_index.add(embeddings)
-
-        self.id_map.extend(ids)
-
-    async def query(self, query: str, top_n: int):
-
-        # Get semantic results
-        query_vector = await openai_aemb([query])
-        faiss_scores, faiss_indices = self.semantic_index.search(query_vector, top_n)
-        faiss_scores, faiss_indices = normalize_array(faiss_scores[0], -1), faiss_indices[0]
-        faiss_result = {self.id_map[r]: faiss_scores[idx] for idx, r in enumerate(faiss_indices)}
-
-        # Return the ranked top n indices
-        return faiss_result
-
-
-class HybridIndex(SemanticIndex):
-    a: float
-    openai_key: str
-    lexical_index: BM25OPlus
-
-    def __init__(self, openai_key: str = None, a: float = 0.7):
-
-        self.a = a
-
-        # Initializes the semantic index
-        super().__init__(openai_key)
+        # Mapping from ids to unique string ids
+        self.id_map = []
 
         # Sets up the tokenizer and the lexical index
         nltk.download('punkt')
 
         self.lexical_index = BM25OPlus(RegexpTokenizer(r'\w+').tokenize)
 
+        # Sets up the faiss index with OpenAI embedding dimensions
+        self.semantic_index = IndexFlatIP(1536)
+
     async def add(self, corpus: List[Tuple[str, str]]):
         ids, documents = zip(*corpus)
 
         # Update BM25 Index
         self.lexical_index.add(documents)
 
         # Get embeddings for new documents and adds them into the index
         embeddings = await openai_emb(documents)
         self.semantic_index.add(embeddings)
 
         self.id_map.extend(ids)
 
     async def query(self, query: str, top_n: int):
 
-        # Get 10 times more results from each index to compare them
-        query_length = min(top_n * 10, len(self.id_map))
-
         # Get semantic results
-        faiss_result = await super().query(query, query_length)
+        query_vector = await openai_emb([query])
+        faiss_scores, faiss_indices = self.semantic_index.search(query_vector, top_n * 10)
+        faiss_scores, faiss_indices = normalize_array(faiss_scores[0], -1), faiss_indices[0]
+        faiss_result = {self.id_map[r]: faiss_scores[idx] for idx, r in enumerate(faiss_indices)}
 
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
 
             combined_scores[id] = self.a * faiss_score + (1 - self.a) * bm25_score
 
         # Return the ranked top n indices
         return sorted(combined_scores, key=combined_scores.get, reverse=True)[:top_n]
+
+    def serialize(self):
+
+        # Create a dictionary representation of your object
+        data = self.__dict__
+
+        # Serialize the index to a byte array
+        data['semantic_index'] = faiss.serialize_index(self.semantic_index)
+
+        # Pickle the dictionary
+        return pickle.dumps(data)
+
+    @classmethod
+    def deserialize(cls, pickled_data: dict, openai_key: str = None):
+
+        # Sets the openai key
+        if openai_key:
+            openai.api_key = openai_key
+
+        # Unpickle the data
+        data = pickle.loads(pickled_data)
+
+        # Deserializes the faiss index
+        data['semantic_index'] = faiss.deserialize_index(data['semantic_index'])
+
+        # Sets the api key
+        openai.api_key = data['openai_key']
+
+        instance = cls.__new__(cls)
+        instance.__dict__.update(data)
+        return instance
```

### Comparing `hybrid_index-0.0.7/setup.py` & `hybrid_index-0.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("hybrid/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="hybrid_index",
-    version="0.0.7",
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
-      "attrs",
-      "charset-normalizer",
+      "aiohttp >=3.8.4",
+      "aiosignal >=1.3.1",
+      "async-timeout >=4.0.2",
+      "attrs >=23.1.0",
+      "certifi >=2023.5.7",
+      "charset-normalizer >=3.1.0",
       "click",
-      "distlib",
-      "faiss-gpu",
-      "filelock",
-      "frozenlist",
-      "idna",
-      "multidict",
+      "distlib >=0.3.6",
+      "faiss-gpu >=1.7.2",
+      "filelock >=3.10.7",
+      "frozenlist >=1.3.3",
+      "idna >=3.4",
+      "mkl-fft >=1.3.6",
+      "mkl-service >=2.4.0",
+      "multidict >=6.0.4",
       "nltk",
       "numpy",
-      "openai",
-      "platformdirs",
+      "openai >=0.27.7",
+      "platformdirs >=3.2.0",
       "regex",
-      "requests",
-      "urllib3",
-      "yarl",
+      "requests >=2.31.0",
+      "urllib3 >=2.0.2",
+      "virtualenv >=20.21.0",
+      "yarl >=1.9.2",
     ],
     extras_require={
         "dev": ["pytest>=7.0", "twine>=4.0.2"],
     },
     python_requires=">=3.10",
 )
```

