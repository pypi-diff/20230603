# Comparing `tmp/dnadb-0.6.3.tar.gz` & `tmp/dnadb-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnadb-0.6.3.tar", last modified: Tue May 23 07:19:48 2023, max compression
+gzip compressed data, was "dnadb-0.6.4.tar", last modified: Sat Jun  3 17:04:12 2023, max compression
```

## Comparing `dnadb-0.6.3.tar` & `dnadb-0.6.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 07:19:48.883777 dnadb-0.6.3/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.6.3/LICENSE
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-23 07:19:48.883777 dnadb-0.6.3/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.6.3/README.md
--rw-r--r--   0 dwl2x     (1000) users      (100)      742 2023-05-23 07:17:21.000000 dnadb-0.6.3/pyproject.toml
--rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-05-23 07:19:48.883777 dnadb-0.6.3/setup.cfg
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 07:19:48.879777 dnadb-0.6.3/src/
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 07:19:48.879777 dnadb-0.6.3/src/dnadb/
--rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-05-23 07:17:33.000000 dnadb-0.6.3/src/dnadb/__init__.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 07:19:48.883777 dnadb-0.6.3/src/dnadb/datasets/
--rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.6.3/src/dnadb/datasets/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-05-14 15:51:22.000000 dnadb-0.6.3/src/dnadb/datasets/dataset.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.6.3/src/dnadb/datasets/greengenes.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 07:19:48.883777 dnadb-0.6.3/src/dnadb/datasets/silva/
--rw-r--r--   0 dwl2x     (1000) users      (100)     5538 2023-05-14 21:04:53.000000 dnadb-0.6.3/src/dnadb/datasets/silva/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-05-15 03:13:49.000000 dnadb-0.6.3/src/dnadb/datasets/silva/taxonomy_map.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     2252 2023-05-21 14:19:04.000000 dnadb-0.6.3/src/dnadb/db.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     4958 2023-05-23 07:14:31.000000 dnadb-0.6.3/src/dnadb/dna.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     8047 2023-05-23 07:16:22.000000 dnadb-0.6.3/src/dnadb/fasta.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6278 2023-05-23 07:17:08.000000 dnadb-0.6.3/src/dnadb/fastq.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 07:19:48.883777 dnadb-0.6.3/src/dnadb/integration/
--rw-r--r--   0 dwl2x     (1000) users      (100)        0 2023-05-23 06:13:30.000000 dnadb-0.6.3/src/dnadb/integration/__init__.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 07:19:48.883777 dnadb-0.6.3/src/dnadb/integration/tf/
--rw-r--r--   0 dwl2x     (1000) users      (100)       18 2023-05-23 06:20:23.000000 dnadb-0.6.3/src/dnadb/integration/tf/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     3200 2023-05-23 06:56:03.000000 dnadb-0.6.3/src/dnadb/integration/tf/dna.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    11231 2023-05-23 05:23:36.000000 dnadb-0.6.3/src/dnadb/sample.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    20094 2023-05-21 14:21:18.000000 dnadb-0.6.3/src/dnadb/taxonomy.py
--rw-r--r--   0 dwl2x     (1000) users      (100)       84 2023-05-21 14:17:53.000000 dnadb-0.6.3/src/dnadb/types.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.6.3/src/dnadb/utils.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 07:19:48.879777 dnadb-0.6.3/src/dnadb.egg-info/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-23 07:19:48.000000 dnadb-0.6.3/src/dnadb.egg-info/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)      644 2023-05-23 07:19:48.000000 dnadb-0.6.3/src/dnadb.egg-info/SOURCES.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-05-23 07:19:48.000000 dnadb-0.6.3/src/dnadb.egg-info/dependency_links.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)       64 2023-05-23 07:19:48.000000 dnadb-0.6.3/src/dnadb.egg-info/requires.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-05-23 07:19:48.000000 dnadb-0.6.3/src/dnadb.egg-info/top_level.txt
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-03 17:04:12.466433 dnadb-0.6.4/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.6.4/LICENSE
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-06-03 17:04:12.466433 dnadb-0.6.4/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.6.4/README.md
+-rw-r--r--   0 dwl2x     (1000) users      (100)      742 2023-06-03 17:02:06.000000 dnadb-0.6.4/pyproject.toml
+-rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-06-03 17:04:12.466433 dnadb-0.6.4/setup.cfg
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-03 17:04:12.466433 dnadb-0.6.4/src/
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-03 17:04:12.466433 dnadb-0.6.4/src/dnadb/
+-rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-06-03 17:02:15.000000 dnadb-0.6.4/src/dnadb/__init__.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-03 17:04:12.466433 dnadb-0.6.4/src/dnadb/datasets/
+-rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.6.4/src/dnadb/datasets/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-05-14 15:51:22.000000 dnadb-0.6.4/src/dnadb/datasets/dataset.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.6.4/src/dnadb/datasets/greengenes.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-03 17:04:12.466433 dnadb-0.6.4/src/dnadb/datasets/silva/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5538 2023-05-14 21:04:53.000000 dnadb-0.6.4/src/dnadb/datasets/silva/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-05-15 03:13:49.000000 dnadb-0.6.4/src/dnadb/datasets/silva/taxonomy_map.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     2252 2023-05-21 14:19:04.000000 dnadb-0.6.4/src/dnadb/db.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     4958 2023-05-23 07:14:31.000000 dnadb-0.6.4/src/dnadb/dna.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     8047 2023-05-23 07:16:22.000000 dnadb-0.6.4/src/dnadb/fasta.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6218 2023-05-31 17:48:30.000000 dnadb-0.6.4/src/dnadb/fastq.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-03 17:04:12.466433 dnadb-0.6.4/src/dnadb/integration/
+-rw-r--r--   0 dwl2x     (1000) users      (100)        0 2023-05-23 06:13:30.000000 dnadb-0.6.4/src/dnadb/integration/__init__.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-03 17:04:12.466433 dnadb-0.6.4/src/dnadb/integration/tf/
+-rw-r--r--   0 dwl2x     (1000) users      (100)       18 2023-05-23 06:20:23.000000 dnadb-0.6.4/src/dnadb/integration/tf/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     3266 2023-05-24 04:25:25.000000 dnadb-0.6.4/src/dnadb/integration/tf/dna.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    11296 2023-06-03 16:57:18.000000 dnadb-0.6.4/src/dnadb/sample.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    20938 2023-06-03 16:59:30.000000 dnadb-0.6.4/src/dnadb/taxonomy.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)       84 2023-05-21 14:17:53.000000 dnadb-0.6.4/src/dnadb/types.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.6.4/src/dnadb/utils.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-06-03 17:04:12.466433 dnadb-0.6.4/src/dnadb.egg-info/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-06-03 17:04:12.000000 dnadb-0.6.4/src/dnadb.egg-info/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)      644 2023-06-03 17:04:12.000000 dnadb-0.6.4/src/dnadb.egg-info/SOURCES.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-06-03 17:04:12.000000 dnadb-0.6.4/src/dnadb.egg-info/dependency_links.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)       64 2023-06-03 17:04:12.000000 dnadb-0.6.4/src/dnadb.egg-info/requires.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-06-03 17:04:12.000000 dnadb-0.6.4/src/dnadb.egg-info/top_level.txt
```

### Comparing `dnadb-0.6.3/LICENSE` & `dnadb-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.3/PKG-INFO` & `dnadb-0.6.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.6.3
+Version: 0.6.4
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.6.3/pyproject.toml` & `dnadb-0.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dnadb"
-version = "0.6.3"
+version = "0.6.4"
 authors = [
   { name="David Ludwig", email="davidludwigii@gmail.com" },
 ]
 description = "A library for handling DNA files."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `dnadb-0.6.3/src/dnadb/datasets/dataset.py` & `dnadb-0.6.4/src/dnadb/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.3/src/dnadb/datasets/greengenes.py` & `dnadb-0.6.4/src/dnadb/datasets/greengenes.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.3/src/dnadb/datasets/silva/__init__.py` & `dnadb-0.6.4/src/dnadb/datasets/silva/__init__.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.3/src/dnadb/datasets/silva/taxonomy_map.py` & `dnadb-0.6.4/src/dnadb/datasets/silva/taxonomy_map.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.3/src/dnadb/db.py` & `dnadb-0.6.4/src/dnadb/db.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.3/src/dnadb/dna.py` & `dnadb-0.6.4/src/dnadb/dna.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.3/src/dnadb/fasta.py` & `dnadb-0.6.4/src/dnadb/fasta.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.3/src/dnadb/fastq.py` & `dnadb-0.6.4/src/dnadb/fastq.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,15 +184,14 @@
     if isinstance(sequences, (str, Path)):
         with open_file(sequences, 'r') as buffer:
             yield from read(buffer)
     elif isinstance(sequences, io.TextIOBase):
         yield from read(sequences)
     else:
         yield from sequences
-    raise TypeError(f"Unsupported type: {type(sequences)}")
 
 
 def read(buffer: io.TextIOBase) -> Generator[FastqEntry, None, None]:
     """
     Read entries from a FASTQ file buffer.
     """
     line = buffer.readline()
```

### Comparing `dnadb-0.6.3/src/dnadb/integration/tf/dna.py` & `dnadb-0.6.4/src/dnadb/integration/tf/dna.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,69 @@
 import numpy as np
 import numpy.typing as npt
 import tensorflow as tf
 
 from ... import dna
 
-BASE_LOOKUP_TABLE = tf.constant(dna.BASE_LOOKUP_TABLE)
-BASE_REVERSE_LOOKUP_TABLE = dna.BASE_REVERSE_LOOKUP_TABLE
-IUPAC_AUGMENT_LOOKUP_TABLE = dna.IUPAC_AUGMENT_LOOKUP_TABLE
+BASE_LOOKUP_TABLE = tf.constant(dna.BASE_LOOKUP_TABLE, dtype=tf.int32)
+BASE_REVERSE_LOOKUP_TABLE = tf.constant(dna.BASE_REVERSE_LOOKUP_TABLE, dtype=tf.int32)
+IUPAC_AUGMENT_LOOKUP_TABLE = tf.constant(dna.IUPAC_AUGMENT_LOOKUP_TABLE, dtype=tf.int32)
 
 # DNA Sequence Encoding/Decoding -------------------------------------------------------------------
 
-def encode(sequences: str|npt.NDArray[np.str_]) -> npt.NDArray[np.uint8]:
+def encode(sequences: str|npt.NDArray[np.str_]|tf.Tensor) -> tf.Tensor:
     """
     Encode a DNA sequence into an integer vector representation.
     """
-    ascii = tf.strings.unicode_decode(sequences, output_encoding="UTF-8")
+    ascii = tf.cast(tf.io.decode_raw(sequences, tf.uint8), tf.int32)
     return tf.gather(BASE_LOOKUP_TABLE, ascii - 65)
 
 
 def decode(sequences: tf.Tensor) -> str:
     """
     Decode a DNA sequence integer vector representation into a string of bases.
     """
     ascii = tf.gather(BASE_REVERSE_LOOKUP_TABLE, sequences)
     return tf.strings.unicode_encode(ascii, output_encoding="UTF-8")
 
 
-# def encode_kmers(
-#     sequences: npt.NDArray[np.uint8],
-#     kmer: int,
-#     ambiguous_bases: bool = False
-# ) -> npt.NDArray[np.int64]:
-#     """
-#     Convert DNA sequences into sequences of k-mers.
-#     """
-#     slices = [slice(0, s) for s in sequences.shape[:-1]]
-#     edge_slices = slice((kmer - 1) // 2, (kmer - 1) // -2)
-#     num_bases = len(BASES + (AMBIGUOUS_BASES if ambiguous_bases else ""))
-#     powers = np.arange(kmer).reshape((1,)*len(slices) + (-1,))
-#     kernel = num_bases**powers
-#     return sp.ndimage.convolve(sequences, kernel)[(*slices, edge_slices)]
-
-
-# def decode_kmers(
-#     sequences: np.ndarray,
-#     kmer: int,
-#     ambiguous_bases: bool = False
-# ) -> npt.NDArray[np.uint8]:
-#     """
-#     Decode sequence of k-mers into 1-mer DNA sequences.
-#     """
-#     slices = [slice(0, s) for s in sequences.shape[:-1]]
-#     edge_slice = slice(-1, sequences.shape[-1])
-#     num_bases = len(BASES + (AMBIGUOUS_BASES if ambiguous_bases else ""))
-#     powers = np.arange(kmer - 1, -1, -1)
-#     kernel = num_bases**powers
-#     edge = (sequences[(*slices, edge_slice)] % kernel[:-1]) // kernel[1:]
-#     return np.concatenate([sequences // kernel[0], edge], axis=-1).astype(np.uint8)
+def encode_kmers(
+    sequences: tf.Tensor,
+    kmer: int|tf.Tensor,
+    ambiguous_bases: bool = False
+) -> tf.Tensor:
+    """
+    Convert DNA sequences into sequences of k-mers.
+    """
+    original_shape = tf.shape(sequences)
+    sequence_length = tf.shape(sequences)[-1]
+    sequences = tf.reshape(sequences, (-1, sequence_length, 1))
+    num_bases = len(dna.BASES + (dna.AMBIGUOUS_BASES if ambiguous_bases else ""))
+    kernel = tf.reshape(tf.pow(num_bases, tf.range(kmer-1, -1, -1, dtype=tf.int32)), (kmer, 1, 1))
+    result = tf.nn.convolution(sequences, kernel, padding="VALID")
+    return tf.reshape(
+        result,
+        tf.concat((original_shape[:-1], (sequence_length - kmer + 1,)), axis=0))
+
+
+def decode_kmers(
+    kmer_sequences: tf.Tensor,
+    kmer: int|tf.Tensor,
+    ambiguous_bases: bool = False
+) -> tf.Tensor:
+    """
+    Decode sequence of k-mers into 1-mer DNA sequences.
+    """
+    num_bases = len(dna.BASES + (dna.AMBIGUOUS_BASES if ambiguous_bases else ""))
+    powers = tf.range(kmer - 1, -1, -1)
+    kernel = num_bases**powers
+    return tf.concat([
+        kmer_sequences // kernel[0],
+        tf.repeat(kmer_sequences[:,-1:], kmer - 1, axis=-1) % kernel[:-1] // kernel[1:]
+    ], axis=-1)
 
 
 # def augment_ambiguous_bases(
 #     sequence: str,
 #     rng: np.random.Generator = np.random.default_rng()
 # ) -> str:
 #     """
```

### Comparing `dnadb-0.6.3/src/dnadb/sample.py` & `dnadb-0.6.4/src/dnadb/sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,18 @@
     def __init__(self, path: Union[str, Path], fasta_index_db: FastaIndexDb):
         super().__init__(path)
         self.fasta_index_db = fasta_index_db
         self.length = np.frombuffer(self.db["length"], dtype=np.int32, count=1)[0]
 
     def __getitem__(self, index_or_name: Union[int, str]) -> SampleMappingEntry:
         if isinstance(index_or_name, str):
-            index_or_name = np.frombuffer(self.db[f"name_{index_or_name}"], dtype=np.int32, count=1)[0]
+            index_or_name = np.frombuffer(
+                self.db[f"name_{index_or_name}"],
+                dtype=np.int32,
+                count=1)[0]
         return SampleMappingEntry.deserialize(self.db[str(index_or_name)], self.fasta_index_db)
 
     def __len__(self):
         return self.length
 
     def __iter__(self) -> Generator[SampleMappingEntry, None, None]:
         for i in range(len(self)):
@@ -156,24 +159,25 @@
 
 class FastaSample(SampleInterface):
     def __init__(self, fasta_db: FastaDb, name: Optional[str] = None):
         super().__init__(name or fasta_db.path.name)
         self.fasta_db = fasta_db
 
     def sample(
-        self, n: int_t,
+        self,
+        n: int_t,
         replace: bool = True,
         rng: np.random.Generator = np.random.default_rng()
     ) -> Generator[FastaEntry, None, None]:
         indices = rng.choice(len(self.fasta_db), size=n, replace=replace)
         indices, counts = np.unique(indices, return_counts=True)
         for index, count in zip(indices, counts):
-            fastq_entry = self.fasta_db[index]
+            fasta_entry = self.fasta_db[index]
             for _ in range(count):
-                yield fastq_entry
+                yield fasta_entry
 
     def __contains__(self, index_or_id: Union[int, str]) -> bool:
         return index_or_id in self.fasta_db
 
     def __len__(self) -> int:
         return len(self.fasta_db)
 
@@ -186,15 +190,16 @@
 
 class FastqSample(SampleInterface):
     def __init__(self, fastq_db: FastqDb, name: Optional[str] = None):
         super().__init__(name or fastq_db.path.name)
         self.fastq_db = fastq_db
 
     def sample(
-        self, n: int_t,
+        self,
+        n: int_t,
         replace: bool = True,
         rng: np.random.Generator = np.random.default_rng()
     ) -> Generator[FastqEntry, None, None]:
         indices = rng.choice(len(self.fastq_db), size=n, replace=replace)
         indices, counts = np.unique(indices, return_counts=True)
         for index, count in zip(indices, counts):
             fastq_entry = self.fastq_db[index]
```

### Comparing `dnadb-0.6.3/src/dnadb/taxonomy.py` & `dnadb-0.6.4/src/dnadb/taxonomy.py`

 * *Files 5% similar despite different names*

```diff
@@ -430,78 +430,100 @@
 
         Args:
             taxons (Tuple[str, ...]): The taxonomy tuple to reduce.
 
         Returns:
             Tuple[str, ...]: The reduced taxonomy tuple.
         """
-        result = tuple()
+        result: Tuple[str, ...] = tuple()
         head = self.taxon_tree_head
         for taxon in taxons[:self.depth]:
             if taxon not in head:
                 break
             result += (taxon,)
             head = head[taxon]
         return result
 
-    def tokenize(self, taxonomy: str, pad: bool = False) -> npt.NDArray[np.int32]:
+    def tokenize(
+        self,
+        taxonomy: str,
+        pad: bool = False,
+        include_missing: bool = False
+    ) -> npt.NDArray[np.int32]:
         """
         Tokenize the taxonomy label into a a tuple of taxon integer IDs
 
         Args:
             taxonomy (str): The taxonomy label to tokenize (e.g. "k__Bacteria; ...").
             pad (bool): Pad the taxonomy with -1s to the depth of the hierarchy. Defaults to False.
+            include_missing (bool): Assign missing taxons in the tokenized taxonomy to 0. Defaults to False.
 
         Returns:
             np.ndarray[np.int32]: The tokenized taxonomy.
         """
-        return self.tokenize_taxons(split_taxonomy(taxonomy), pad)
+        return self.tokenize_taxons(split_taxonomy(taxonomy), pad, include_missing)
 
-    def tokenize_taxons(self, taxons: Tuple[str, ...], pad: bool = False) -> npt.NDArray[np.int32]:
+    def tokenize_taxons(
+        self,
+        taxons: Tuple[str, ...],
+        pad: bool = False,
+        include_missing: bool = False
+    ) -> npt.NDArray[np.int32]:
         """
         Tokenize the taxonomy tuple into a a tuple of taxon integer IDs
 
         Args:
             taxons (Tuple[str, ...]): The taxonomy tuple to tokenize.
             pad (bool): Pad the taxonomy with -1s to the depth of the hierarchy. Defaults to False.
+            include_missing (bool): Assign missing taxons in the tokenized taxonomy to 0. Defaults to False.
 
         Returns:
             np.ndarray[np.int32]: The tokenized taxonomy.
         """
         taxons = taxons[:self.depth] # todo should we trim silently or throw error?
         result = np.empty(len(taxons), np.int32) if not pad else np.full(self.depth, -1, np.int32)
         head = self.taxon_tree_head
         for taxon in taxons:
             head = head[taxon]
             result[head.rank] = self.taxon_to_id_map[head.rank][head]
+        if include_missing:
+            result += 1
         return result
 
-    def detokenize(self, taxon_tokens: npt.NDArray[np.int32]) -> str:
+    def detokenize(self, taxon_tokens: npt.NDArray[np.int32], include_missing: bool = False) -> str:
         """
         Detokenize the taxonomy tokens into a taxonomy label.
 
         Args:
             taxon_tokens (npt.NDArray[np.int64]): The taxonomy tokens.
+            include_missing (bool): Assign missing taxons in the tokenized taxonomy to 0. Defaults to False.
 
         Returns:
             str: The detokenized taxonomy label.
         """
-        return join_taxonomy(self.detokenize_taxons(taxon_tokens))
+        return join_taxonomy(self.detokenize_taxons(taxon_tokens, include_missing))
 
-    def detokenize_taxons(self, taxon_tokens: npt.NDArray[np.int32]) -> Tuple[str, ...]:
+    def detokenize_taxons(
+        self,
+        taxon_tokens: npt.NDArray[np.int32],
+        include_missing: bool = False
+    ) -> Tuple[str, ...]:
         """
         Detokenize the taxonomy tokens into a taxonomy tuple.
 
         Args:
             taxon_tokens (npt.NDArray[np.int64]): The taxonomy tokens.
+            include_missing (bool): Assign missing taxons in the tokenized taxonomy to 0. Defaults to False.
 
         Returns:
             Tuple[str, ...]: The detokenized taxonomy tuple.
         """
-        result = tuple()
+        if include_missing:
+            taxon_tokens -= 1
+        result: Tuple[str, ...] = tuple()
         token: np.int32
         for rank, token in enumerate(taxon_tokens):
             if token < 0:
                 break
             result += (self.id_to_taxon_map[rank][token].name,)
         return result
```

### Comparing `dnadb-0.6.3/src/dnadb/utils.py` & `dnadb-0.6.4/src/dnadb/utils.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.3/src/dnadb.egg-info/PKG-INFO` & `dnadb-0.6.4/src/dnadb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.6.3
+Version: 0.6.4
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.6.3/src/dnadb.egg-info/SOURCES.txt` & `dnadb-0.6.4/src/dnadb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

