# Comparing `tmp/pyvariant-2.2.0.tar.gz` & `tmp/pyvariant-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvariant-2.2.0.tar", last modified: Thu Jun  1 21:03:59 2023, max compression
+gzip compressed data, was "pyvariant-2.2.1.tar", last modified: Fri Jun  2 22:10:17 2023, max compression
```

## Comparing `pyvariant-2.2.0.tar` & `pyvariant-2.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-06-01 21:03:59.238783 pyvariant-2.2.0/
--rw-r--r--   0 mdouglas  (2185) users      (100)     1072 2023-05-16 21:59:33.000000 pyvariant-2.2.0/LICENSE
--rw-r--r--   0 mdouglas  (2185) users      (100)     8087 2023-06-01 21:03:59.241349 pyvariant-2.2.0/PKG-INFO
--rw-r--r--   0 mdouglas  (2185) users      (100)     6903 2023-05-16 21:59:33.000000 pyvariant-2.2.0/README.md
--rw-r--r--   0 mdouglas  (2185) users      (100)      342 2023-05-16 21:59:33.000000 pyvariant-2.2.0/pyproject.toml
-drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-06-01 21:03:59.071277 pyvariant-2.2.0/pyvariant/
--rw-r--r--   0 mdouglas  (2185) users      (100)      829 2023-06-01 20:06:52.000000 pyvariant-2.2.0/pyvariant/__init__.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     1995 2023-05-16 21:59:33.000000 pyvariant-2.2.0/pyvariant/cli.py
--rw-r--r--   0 mdouglas  (2185) users      (100)      956 2023-05-26 20:27:04.000000 pyvariant-2.2.0/pyvariant/constants.py
--rw-r--r--   0 mdouglas  (2185) users      (100)   143931 2023-06-01 20:06:42.000000 pyvariant-2.2.0/pyvariant/core.py
-drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-06-01 21:03:59.148769 pyvariant-2.2.0/pyvariant/data/
--rw-r--r--   0 mdouglas  (2185) users      (100)        4 2023-05-16 21:59:33.000000 pyvariant-2.2.0/pyvariant/data/empty.fa
--rw-r--r--   0 mdouglas  (2185) users      (100)       10 2023-05-16 21:59:33.000000 pyvariant-2.2.0/pyvariant/data/empty.fa.fai
--rw-r--r--   0 mdouglas  (2185) users      (100)    25066 2023-05-26 20:27:04.000000 pyvariant-2.2.0/pyvariant/ensembl_cache.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     7149 2023-05-30 19:30:43.000000 pyvariant-2.2.0/pyvariant/ensembl_release.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     4877 2023-05-16 21:59:33.000000 pyvariant-2.2.0/pyvariant/files.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     4728 2023-05-29 20:48:35.000000 pyvariant-2.2.0/pyvariant/parser.py
--rw-r--r--   0 mdouglas  (2185) users      (100)    14837 2023-05-29 20:48:35.000000 pyvariant-2.2.0/pyvariant/regex.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     8450 2023-05-26 20:27:04.000000 pyvariant-2.2.0/pyvariant/sequence.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     1623 2023-05-16 21:59:33.000000 pyvariant-2.2.0/pyvariant/tables.py
--rw-r--r--   0 mdouglas  (2185) users      (100)    14143 2023-05-16 21:59:33.000000 pyvariant-2.2.0/pyvariant/utils.py
--rw-r--r--   0 mdouglas  (2185) users      (100)    45586 2023-05-30 18:49:03.000000 pyvariant-2.2.0/pyvariant/variants.py
-drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-06-01 21:03:59.130250 pyvariant-2.2.0/pyvariant.egg-info/
--rw-r--r--   0 mdouglas  (2185) users      (100)     8087 2023-06-01 21:03:58.000000 pyvariant-2.2.0/pyvariant.egg-info/PKG-INFO
--rw-r--r--   0 mdouglas  (2185) users      (100)      802 2023-06-01 21:03:58.000000 pyvariant-2.2.0/pyvariant.egg-info/SOURCES.txt
--rw-r--r--   0 mdouglas  (2185) users      (100)        1 2023-06-01 21:03:58.000000 pyvariant-2.2.0/pyvariant.egg-info/dependency_links.txt
--rw-r--r--   0 mdouglas  (2185) users      (100)       49 2023-06-01 21:03:58.000000 pyvariant-2.2.0/pyvariant.egg-info/entry_points.txt
--rw-r--r--   0 mdouglas  (2185) users      (100)      166 2023-06-01 21:03:58.000000 pyvariant-2.2.0/pyvariant.egg-info/requires.txt
--rw-r--r--   0 mdouglas  (2185) users      (100)       10 2023-06-01 21:03:58.000000 pyvariant-2.2.0/pyvariant.egg-info/top_level.txt
--rw-r--r--   0 mdouglas  (2185) users      (100)        1 2023-06-01 21:03:58.000000 pyvariant-2.2.0/pyvariant.egg-info/zip-safe
--rw-r--r--   0 mdouglas  (2185) users      (100)     1624 2023-06-01 21:03:59.247901 pyvariant-2.2.0/setup.cfg
-drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-06-01 21:03:59.231228 pyvariant-2.2.0/tests/
--rw-r--r--   0 mdouglas  (2185) users      (100)    72420 2023-06-01 20:06:40.000000 pyvariant-2.2.0/tests/test_core.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     9802 2023-05-26 20:27:05.000000 pyvariant-2.2.0/tests/test_core_map.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     6158 2023-05-26 20:27:05.000000 pyvariant-2.2.0/tests/test_ensembl_cache.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     1487 2023-05-26 20:27:05.000000 pyvariant-2.2.0/tests/test_ensembl_release.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     2025 2023-05-26 20:27:05.000000 pyvariant-2.2.0/tests/test_files.py
--rw-r--r--   0 mdouglas  (2185) users      (100)       88 2023-05-16 21:59:34.000000 pyvariant-2.2.0/tests/test_init.py
--rw-r--r--   0 mdouglas  (2185) users      (100)    39897 2023-05-29 20:48:35.000000 pyvariant-2.2.0/tests/test_parser.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     3400 2023-05-26 20:27:05.000000 pyvariant-2.2.0/tests/test_sequence.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     7262 2023-05-16 21:59:34.000000 pyvariant-2.2.0/tests/test_utils.py
+drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-06-02 22:10:17.899139 pyvariant-2.2.1/
+-rw-r--r--   0 mdouglas  (2185) users      (100)     1072 2023-05-16 21:59:33.000000 pyvariant-2.2.1/LICENSE
+-rw-r--r--   0 mdouglas  (2185) users      (100)     8087 2023-06-02 22:10:17.901548 pyvariant-2.2.1/PKG-INFO
+-rw-r--r--   0 mdouglas  (2185) users      (100)     6903 2023-05-16 21:59:33.000000 pyvariant-2.2.1/README.md
+-rw-r--r--   0 mdouglas  (2185) users      (100)      342 2023-05-16 21:59:33.000000 pyvariant-2.2.1/pyproject.toml
+drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-06-02 22:10:17.733713 pyvariant-2.2.1/pyvariant/
+-rw-r--r--   0 mdouglas  (2185) users      (100)      829 2023-06-01 20:06:52.000000 pyvariant-2.2.1/pyvariant/__init__.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     1995 2023-05-16 21:59:33.000000 pyvariant-2.2.1/pyvariant/cli.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)      956 2023-05-26 20:27:04.000000 pyvariant-2.2.1/pyvariant/constants.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)   147434 2023-06-02 21:03:59.000000 pyvariant-2.2.1/pyvariant/core.py
+drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-06-02 22:10:17.809888 pyvariant-2.2.1/pyvariant/data/
+-rw-r--r--   0 mdouglas  (2185) users      (100)        4 2023-05-16 21:59:33.000000 pyvariant-2.2.1/pyvariant/data/empty.fa
+-rw-r--r--   0 mdouglas  (2185) users      (100)       10 2023-05-16 21:59:33.000000 pyvariant-2.2.1/pyvariant/data/empty.fa.fai
+-rw-r--r--   0 mdouglas  (2185) users      (100)    25066 2023-05-26 20:27:04.000000 pyvariant-2.2.1/pyvariant/ensembl_cache.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     7149 2023-05-30 19:30:43.000000 pyvariant-2.2.1/pyvariant/ensembl_release.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     4877 2023-05-16 21:59:33.000000 pyvariant-2.2.1/pyvariant/files.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     4728 2023-05-29 20:48:35.000000 pyvariant-2.2.1/pyvariant/parser.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)    14837 2023-05-29 20:48:35.000000 pyvariant-2.2.1/pyvariant/regex.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     8450 2023-05-26 20:27:04.000000 pyvariant-2.2.1/pyvariant/sequence.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     1623 2023-05-16 21:59:33.000000 pyvariant-2.2.1/pyvariant/tables.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)    14130 2023-06-02 21:03:59.000000 pyvariant-2.2.1/pyvariant/utils.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)    45586 2023-05-30 18:49:03.000000 pyvariant-2.2.1/pyvariant/variants.py
+drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-06-02 22:10:17.790980 pyvariant-2.2.1/pyvariant.egg-info/
+-rw-r--r--   0 mdouglas  (2185) users      (100)     8087 2023-06-02 22:10:17.000000 pyvariant-2.2.1/pyvariant.egg-info/PKG-INFO
+-rw-r--r--   0 mdouglas  (2185) users      (100)      802 2023-06-02 22:10:17.000000 pyvariant-2.2.1/pyvariant.egg-info/SOURCES.txt
+-rw-r--r--   0 mdouglas  (2185) users      (100)        1 2023-06-02 22:10:17.000000 pyvariant-2.2.1/pyvariant.egg-info/dependency_links.txt
+-rw-r--r--   0 mdouglas  (2185) users      (100)       49 2023-06-02 22:10:17.000000 pyvariant-2.2.1/pyvariant.egg-info/entry_points.txt
+-rw-r--r--   0 mdouglas  (2185) users      (100)      166 2023-06-02 22:10:17.000000 pyvariant-2.2.1/pyvariant.egg-info/requires.txt
+-rw-r--r--   0 mdouglas  (2185) users      (100)       10 2023-06-02 22:10:17.000000 pyvariant-2.2.1/pyvariant.egg-info/top_level.txt
+-rw-r--r--   0 mdouglas  (2185) users      (100)        1 2023-06-02 22:10:16.000000 pyvariant-2.2.1/pyvariant.egg-info/zip-safe
+-rw-r--r--   0 mdouglas  (2185) users      (100)     1624 2023-06-02 22:10:17.908025 pyvariant-2.2.1/setup.cfg
+drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-06-02 22:10:17.891656 pyvariant-2.2.1/tests/
+-rw-r--r--   0 mdouglas  (2185) users      (100)    72420 2023-06-01 20:06:40.000000 pyvariant-2.2.1/tests/test_core.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)    10396 2023-06-02 21:03:59.000000 pyvariant-2.2.1/tests/test_core_map.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     6158 2023-05-26 20:27:05.000000 pyvariant-2.2.1/tests/test_ensembl_cache.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     1487 2023-05-26 20:27:05.000000 pyvariant-2.2.1/tests/test_ensembl_release.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     2025 2023-05-26 20:27:05.000000 pyvariant-2.2.1/tests/test_files.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)       88 2023-05-16 21:59:34.000000 pyvariant-2.2.1/tests/test_init.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)    39897 2023-05-29 20:48:35.000000 pyvariant-2.2.1/tests/test_parser.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     3400 2023-05-26 20:27:05.000000 pyvariant-2.2.1/tests/test_sequence.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     7341 2023-06-02 21:03:59.000000 pyvariant-2.2.1/tests/test_utils.py
```

### Comparing `pyvariant-2.2.0/LICENSE` & `pyvariant-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvariant-2.2.0/PKG-INFO` & `pyvariant-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvariant
-Version: 2.2.0
+Version: 2.2.1
 Summary: Map biological sequence variants (mutations) to their equivalent chromosome, cDNA, gene, exon, protein, and RNA positions.
 Home-page: https://github.com/mattdoug604/pyvariant.git
 Author: Matthew Douglas
 Author-email: mattdoug604@gmail.com
 Maintainer: Matthew Douglas
 Maintainer-email: mattdoug604@gmail.com
 License: MIT
```

### Comparing `pyvariant-2.2.0/README.md` & `pyvariant-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyvariant-2.2.0/pyvariant/__init__.py` & `pyvariant-2.2.1/pyvariant/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.2.0/pyvariant/cli.py` & `pyvariant-2.2.1/pyvariant/cli.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.2.0/pyvariant/constants.py` & `pyvariant-2.2.1/pyvariant/constants.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.2.0/pyvariant/core.py` & `pyvariant-2.2.1/pyvariant/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -305,23 +305,28 @@
         if variant_type.lower() == "indel":
             variant_type = DELINS
 
         def get_refseq_altseq(position) -> Tuple[str, str]:
             refseq_ = refseq or self.sequence(position)
             if altseq:
                 altseq_ = altseq
+                if variant_type == INSERTION:
+                    if not altseq.startswith(refseq_[0]):
+                        altseq_ = refseq_[0] + altseq_
+                    if len(refseq_) > 1 and not altseq.endswith(refseq_[1]):
+                        altseq_ = altseq_ + refseq_[1]
             else:
                 if variant_type == DELETION:
                     altseq_ = ""
                 elif variant_type == DELINS:
                     raise ValueError(f"altseq required for {DELINS}")
                 elif variant_type == DUPLICATION:
                     altseq_ = refseq_ * 2
                 elif variant_type == FRAMESHIFT:
-                    raise ValueError(f"altseq required for {FRAMESHIFT}")
+                    altseq_ = ""
                 elif variant_type == INSERTION:
                     raise ValueError(f"altseq required for {INSERTION}")
                 elif variant_type == SUBSTITUTION:
                     raise ValueError(f"altseq required for {SUBSTITUTION}")
                 else:
                     raise ValueError(f"Unsupported variant type '{variant_type}'")
 
@@ -424,15 +429,19 @@
             raise ValueError(f"Unrecognized position type '{position_type}'")
 
         # Optional, convert each position and the given ref and alt sequences to variants
         if variant_type:
             result_ = []
             for position in result:
                 refseq_, altseq_ = get_refseq_altseq(position)
-                result_.extend(self._position_to_small_variant(position, refseq_, altseq_))
+                result_.extend(
+                    self._position_to_small_variant(
+                        position, refseq_, altseq_, is_frameshift=variant_type == FRAMESHIFT
+                    )
+                )
 
             result = result_
 
         # TODO: Should this always raise an error?
         if not result:
             raise ValueError("Unable to convert inputs to a variant")
 
@@ -1122,66 +1131,71 @@
                     position.start_offset,
                     position.end,
                     position.end_offset,
                     [position.strand],
                     position.refseq,
                     position.altseq,
                     canonical,
+                    position.is_frameshift,
                 )
             elif position.is_dna:
                 position = cast(_DnaSmallVariant, position)
                 return dnavf(
                     [position.contig_id],
                     position.start,
                     position.start_offset,
                     position.end,
                     position.end_offset,
                     [position.strand],
                     position.refseq,
                     position.altseq,
                     canonical,
+                    position.is_frameshift,
                 )
             elif position.is_exon:
                 position = cast(_ExonSmallVariant, position)
                 return exonvf(
                     [position.transcript_id],
                     position.start,
                     position.start_offset,
                     position.end,
                     position.end_offset,
                     [position.strand],
                     position.refseq,
                     position.altseq,
                     canonical,
+                    position.is_frameshift,
                 )
             elif position.is_protein:
                 position = cast(_ProteinSmallVariant, position)
                 return proteinvf(
                     [position.transcript_id],
                     position.start,
                     position.start_offset,
                     position.end,
                     position.end_offset,
                     [position.strand],
                     position.refseq,
                     position.altseq,
                     canonical,
+                    position.is_frameshift,
                 )
             elif position.is_rna:
                 position = cast(_RnaSmallVariant, position)
                 return rnavf(
                     [position.transcript_id],
                     position.start,
                     position.start_offset,
                     position.end,
                     position.end_offset,
                     [position.strand],
                     position.refseq,
                     position.altseq,
                     canonical,
+                    position.is_frameshift,
                 )
         else:
             if position.is_cdna:
                 position = cast(CdnaPosition, position)
                 return cdnaf(
                     [position.transcript_id],
                     position.start,
@@ -1306,29 +1320,32 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
         include_stop: bool = True,
     ) -> List[_CdnaSmallVariant]:
         result = []
 
         for cdna in self._cdna_to_cdna(
             transcript_id,
             start,
             start_offset,
             end,
             end_offset,
             strand,
             canonical=canonical,
             include_stop=include_stop,
         ):
-            result.extend(self._position_to_small_variant(cdna, refseq, altseq))
+            result.extend(
+                self._position_to_small_variant(cdna, refseq, altseq, is_frameshift=is_frameshift)
+            )
 
         return result
 
     def _cdna_to_dna(
         self,
         transcript_id: List[str],
         start: int,
@@ -1392,29 +1409,32 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
         include_stop: bool = True,
     ) -> List[_DnaSmallVariant]:
         result = []
 
         for dna in self._cdna_to_dna(
             transcript_id,
             start,
             start_offset,
             end,
             end_offset,
             strand,
             canonical=canonical,
             include_stop=include_stop,
         ):
-            result.extend(self._position_to_small_variant(dna, refseq, altseq))
+            result.extend(
+                self._position_to_small_variant(dna, refseq, altseq, is_frameshift=is_frameshift)
+            )
 
         return result
 
     def _cdna_to_exon(
         self,
         transcript_id: List[str],
         start: int,
@@ -1490,29 +1510,32 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
         include_stop: bool = True,
     ) -> List[_ExonSmallVariant]:
         result = []
 
         for exon in self._cdna_to_exon(
             transcript_id,
             start,
             start_offset,
             end,
             end_offset,
             strand,
             canonical=canonical,
             include_stop=include_stop,
         ):
-            result.extend(self._position_to_small_variant(exon, refseq, altseq))
+            result.extend(
+                self._position_to_small_variant(exon, refseq, altseq, is_frameshift=is_frameshift)
+            )
 
         return result
 
     def _cdna_to_protein(
         self,
         transcript_id: List[str],
         start: int,
@@ -1560,14 +1583,15 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
     ) -> List[_ProteinSmallVariant]:
         result = []
 
         for cdna in self._cdna_to_cdna(
             transcript_id,
             start,
             start_offset,
@@ -1599,15 +1623,14 @@
         protein_start = calc_cdna_to_protein(cdna.start)
         protein_end = calc_cdna_to_protein(cdna.end)
         protein = ProteinPosition.copy_from(
             cdna, start=protein_start, start_offset=0, end=protein_end, end_offset=0
         )
         refaa = self.sequence(protein)
         for altaa, is_frameshift in self.translate_cdna_variant(cdna, altseq):
-            # TODO: Support frameshift variants
             result.extend(
                 self._position_to_small_variant(protein, refaa, altaa, is_frameshift=is_frameshift)
             )
 
         return result
 
     def _cdna_to_rna(
@@ -1678,29 +1701,32 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
         include_stop: bool = True,
     ) -> List[_RnaSmallVariant]:
         result = []
 
         for rna in self._cdna_to_rna(
             transcript_id,
             start,
             start_offset,
             end,
             end_offset,
             strand,
             canonical=canonical,
             include_stop=include_stop,
         ):
-            result.extend(self._position_to_small_variant(rna, refseq, altseq))
+            result.extend(
+                self._position_to_small_variant(rna, refseq, altseq, is_frameshift=is_frameshift)
+            )
 
         return result
 
     def _dna_to_cdna(
         self,
         contig_id: List[str],
         start: int,
@@ -1771,29 +1797,32 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
         include_stop: bool = True,
     ) -> List[_CdnaSmallVariant]:
         result = []
 
         for cdna in self._dna_to_cdna(
             contig_id,
             start,
             start_offset,
             end,
             end_offset,
             strand,
             canonical=canonical,
             include_stop=include_stop,
         ):
-            result.extend(self._position_to_small_variant(cdna, refseq, altseq))
+            result.extend(
+                self._position_to_small_variant(cdna, refseq, altseq, is_frameshift=is_frameshift)
+            )
 
         return result
 
     def _dna_to_dna(
         self,
         contig_id: List[str],
         start: int,
@@ -1841,21 +1870,24 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
     ) -> List[_DnaSmallVariant]:
         result = []
 
         for dna in self._dna_to_dna(
             contig_id, start, start_offset, end, end_offset, strand, canonical=canonical
         ):
-            result.extend(self._position_to_small_variant(dna, refseq, altseq))
+            result.extend(
+                self._position_to_small_variant(dna, refseq, altseq, is_frameshift=is_frameshift)
+            )
 
         return result
 
     def _dna_to_exon(
         self,
         contig_id: List[str],
         start: int,
@@ -1918,21 +1950,24 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
     ) -> List[_ExonSmallVariant]:
         result = []
 
         for exon in self._dna_to_exon(
             contig_id, start, start_offset, end, end_offset, strand, canonical=canonical
         ):
-            result.extend(self._position_to_small_variant(exon, refseq, altseq))
+            result.extend(
+                self._position_to_small_variant(exon, refseq, altseq, is_frameshift=is_frameshift)
+            )
 
         return result
 
     def _dna_to_protein(
         self,
         contig_id: List[str],
         start: int,
@@ -1965,14 +2000,15 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
     ) -> List[_ProteinSmallVariant]:
         result = []
 
         for cdna in self._dna_to_cdna(
             contig_id,
             start,
             start_offset,
@@ -2053,21 +2089,24 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
     ) -> List[_RnaSmallVariant]:
         result = []
 
         for rna in self._dna_to_rna(
             contig_id, start, start_offset, end, end_offset, strand, canonical=canonical
         ):
-            result.extend(self._position_to_small_variant(rna, refseq, altseq))
+            result.extend(
+                self._position_to_small_variant(rna, refseq, altseq, is_frameshift=is_frameshift)
+            )
 
         return result
 
     def _exon_to_cdna(
         self,
         transcript_id: List[str],
         start: int,
@@ -2130,14 +2169,15 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
     ) -> List[_ExonSmallVariant]:
         return []
 
     def _exon_to_dna(
         self,
         transcript_id: List[str],
         start: int,
@@ -2192,14 +2232,15 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
     ) -> List[_ExonSmallVariant]:
         return []
 
     def _exon_to_exon(
         self,
         transcript_id: List[str],
         start: int,
@@ -2259,14 +2300,15 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
     ) -> List[_ExonSmallVariant]:
         return []
 
     def _exon_to_protein(
         self,
         transcript_id: List[str],
         start: int,
@@ -2309,14 +2351,15 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
     ) -> List[_ExonSmallVariant]:
         return []
 
     def _exon_to_rna(
         self,
         transcript_id: List[str],
         start: int,
@@ -2375,14 +2418,15 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
     ) -> List[_ExonSmallVariant]:
         return []
 
     def _protein_to_cdna(
         self,
         transcript_id: List[str],
         start: int,
@@ -2419,26 +2463,31 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
     ) -> List[_CdnaSmallVariant]:
         result = []
 
         for cdna in self._protein_to_cdna(
             transcript_id, start, start_offset, end, end_offset, strand, canonical=canonical
         ):
             for ref, alt in product(reverse_translate(refseq), reverse_translate(altseq)):
                 # For insertions, check that the sequence flanking the inserted sequence matches the ref
                 if is_insertion(refseq, altseq) and not is_insertion(ref, alt):
                     continue
 
-                result.extend(self._position_to_small_variant(cdna, ref, alt, validate=True))
+                result.extend(
+                    self._position_to_small_variant(
+                        cdna, ref, alt, is_frameshift=is_frameshift, validate=True
+                    )
+                )
 
         return result
 
     def _protein_to_dna(
         self,
         transcript_id: List[str],
         start: int,
@@ -2474,39 +2523,42 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
     ) -> List[_DnaSmallVariant]:
         result = []
 
         for cdna in self._protein_to_cdna_variant(
             transcript_id,
             start,
             start_offset,
             end,
             end_offset,
             strand,
             refseq,
             altseq,
             canonical=canonical,
+            is_frameshift=is_frameshift,
         ):
             result.extend(
                 self._cdna_to_dna_variant(
                     [cdna.transcript_id],
                     cdna.start,
                     cdna.start_offset,
                     cdna.end,
                     cdna.end_offset,
                     [cdna.strand],
                     cdna.refseq,
                     cdna.altseq,
                     canonical=canonical,
+                    is_frameshift=is_frameshift,
                     include_stop=True,
                 )
             )
 
         return sorted(set(result))
 
     def _protein_to_exon(
@@ -2545,39 +2597,42 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
     ) -> List[_ExonSmallVariant]:
         result = []
 
         for cdna in self._protein_to_cdna_variant(
             transcript_id,
             start,
             start_offset,
             end,
             end_offset,
             strand,
             refseq,
             altseq,
             canonical=canonical,
+            is_frameshift=is_frameshift,
         ):
             result.extend(
                 self._cdna_to_exon_variant(
                     [cdna.transcript_id],
                     cdna.start,
                     cdna.start_offset,
                     cdna.end,
                     cdna.end_offset,
                     [cdna.strand],
                     cdna.refseq,
                     cdna.altseq,
                     canonical=canonical,
+                    is_frameshift=is_frameshift,
                     include_stop=True,
                 )
             )
 
         return sorted(set(result))
 
     def _protein_to_protein(
@@ -2616,41 +2671,54 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
     ) -> List[_ProteinSmallVariant]:
         result = []
 
-        for cdna in self._protein_to_cdna_variant(
-            transcript_id,
-            start,
-            start_offset,
-            end,
-            end_offset,
-            strand,
-            refseq,
-            altseq,
-            canonical=canonical,
-        ):
-            result.extend(
-                self._cdna_to_protein_variant(
-                    [cdna.transcript_id],
-                    cdna.start,
-                    cdna.start_offset,
-                    cdna.end,
-                    cdna.end_offset,
-                    [cdna.strand],
-                    cdna.refseq,
-                    cdna.altseq,
-                    canonical=canonical,
+        if is_frameshift:
+            for protein in self._protein_to_protein(
+                transcript_id, start, start_offset, end, end_offset, strand, canonical
+            ):
+                result.extend(
+                    self._position_to_small_variant(
+                        protein, refseq, altseq, is_frameshift=is_frameshift
+                    )
+                )
+        else:
+            for cdna in self._protein_to_cdna_variant(
+                transcript_id,
+                start,
+                start_offset,
+                end,
+                end_offset,
+                strand,
+                refseq,
+                altseq,
+                canonical=canonical,
+                is_frameshift=is_frameshift,
+            ):
+                result.extend(
+                    self._cdna_to_protein_variant(
+                        [cdna.transcript_id],
+                        cdna.start,
+                        cdna.start_offset,
+                        cdna.end,
+                        cdna.end_offset,
+                        [cdna.strand],
+                        cdna.refseq,
+                        cdna.altseq,
+                        canonical=canonical,
+                        is_frameshift=is_frameshift,
+                    )
                 )
-            )
 
         return sorted(set(result))
 
     def _protein_to_rna(
         self,
         transcript_id: List[str],
         start: int,
@@ -2686,39 +2754,42 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
     ) -> List[_RnaSmallVariant]:
         result = []
 
         for cdna in self._protein_to_cdna_variant(
             transcript_id,
             start,
             start_offset,
             end,
             end_offset,
             strand,
             refseq,
             altseq,
             canonical=canonical,
+            is_frameshift=is_frameshift,
         ):
             result.extend(
                 self._cdna_to_rna_variant(
                     [cdna.transcript_id],
                     cdna.start,
                     cdna.start_offset,
                     cdna.end,
                     cdna.end_offset,
                     [cdna.strand],
                     cdna.refseq,
                     cdna.altseq,
                     canonical=canonical,
+                    is_frameshift=is_frameshift,
                 )
             )
 
         return sorted(set(result))
 
     def _rna_to_cdna(
         self,
@@ -2789,29 +2860,32 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
         include_stop: bool = True,
     ) -> List[_CdnaSmallVariant]:
         result = []
 
         for cdna in self._rna_to_cdna(
             transcript_id,
             start,
             start_offset,
             end,
             end_offset,
             strand,
             canonical=canonical,
             include_stop=include_stop,
         ):
-            result.extend(self._position_to_small_variant(cdna, refseq, altseq))
+            result.extend(
+                self._position_to_small_variant(cdna, refseq, altseq, is_frameshift=is_frameshift)
+            )
 
         return result
 
     def _rna_to_dna(
         self,
         transcript_id: List[str],
         start: int,
@@ -2873,21 +2947,24 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
     ) -> List[_DnaSmallVariant]:
         result = []
 
         for dna in self._rna_to_dna(
             transcript_id, start, start_offset, end, end_offset, strand, canonical=canonical
         ):
-            result.extend(self._position_to_small_variant(dna, refseq, altseq))
+            result.extend(
+                self._position_to_small_variant(dna, refseq, altseq, is_frameshift=is_frameshift)
+            )
 
         return result
 
     def _rna_to_exon(
         self,
         transcript_id: List[str],
         start: int,
@@ -2954,21 +3031,24 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
     ) -> List[_ExonSmallVariant]:
         result = []
 
         for exon in self._rna_to_exon(
             transcript_id, start, start_offset, end, end_offset, strand, canonical=canonical
         ):
-            result.extend(self._position_to_small_variant(exon, refseq, altseq))
+            result.extend(
+                self._position_to_small_variant(exon, refseq, altseq, is_frameshift=is_frameshift)
+            )
 
         return result
 
     def _rna_to_protein(
         self,
         transcript_id: List[str],
         start: int,
@@ -3011,27 +3091,29 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
     ) -> List[_ProteinSmallVariant]:
         result = []
 
         for cdna in self._rna_to_cdna_variant(
             transcript_id,
             start,
             start_offset,
             end,
             end_offset,
             strand,
             refseq,
             altseq,
             canonical=canonical,
+            is_frameshift=is_frameshift,
             include_stop=False,
         ):
             result.extend(
                 self._cdna_to_protein_variant(
                     [cdna.transcript_id],
                     cdna.start,
                     cdna.start_offset,
@@ -3110,21 +3192,24 @@
         start_offset: int,
         end: int,
         end_offset: int,
         strand: List[str],
         refseq: str,
         altseq: str,
         canonical: bool = False,
+        is_frameshift: bool = False,
     ) -> List[_RnaSmallVariant]:
         result = []
 
         for rna in self._rna_to_rna(
             transcript_id, start, start_offset, end, end_offset, strand, canonical=canonical
         ):
-            result.extend(self._position_to_small_variant(rna, refseq, altseq))
+            result.extend(
+                self._position_to_small_variant(rna, refseq, altseq, is_frameshift=is_frameshift)
+            )
 
         return result
 
     def _position_to_small_variant(
         self,
         position: _Position,
         refseq: str,
@@ -3248,14 +3333,18 @@
             if position.position_type == PROTEIN and is_frameshift:
                 # NOTE: Only the first amino acid change is preserved.
                 # See https://varnomen.hgvs.org/recommendations/protein/variant/frameshift/
                 variant_class = ProteinFrameshift
                 end = start
                 new_ref = new_ref[0] if new_ref else new_ref
                 new_alt = new_alt[0] if new_alt else new_alt
+            elif position.position_type != PROTEIN and is_frameshift and not new_alt:
+                # NOTE: If we're mapping from a frameshift and we don't know what the sequence
+                # change is, return an empty list because otherwise there's too many possible results
+                continue
             else:
                 variant_class = variant_class_map.get((position.position_type, variant_type))
 
             # Initialize a new variant object from the given position object
             if variant_class:
                 variant = variant_class.copy_from(
                     position,
```

### Comparing `pyvariant-2.2.0/pyvariant/ensembl_cache.py` & `pyvariant-2.2.1/pyvariant/ensembl_cache.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.2.0/pyvariant/ensembl_release.py` & `pyvariant-2.2.1/pyvariant/ensembl_release.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.2.0/pyvariant/files.py` & `pyvariant-2.2.1/pyvariant/files.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.2.0/pyvariant/parser.py` & `pyvariant-2.2.1/pyvariant/parser.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.2.0/pyvariant/regex.py` & `pyvariant-2.2.1/pyvariant/regex.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.2.0/pyvariant/sequence.py` & `pyvariant-2.2.1/pyvariant/sequence.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.2.0/pyvariant/tables.py` & `pyvariant-2.2.1/pyvariant/tables.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.2.0/pyvariant/utils.py` & `pyvariant-2.2.1/pyvariant/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         return ref, alt, 0, 0
 
     # Trim bases from each end that are identical between the ref and alt
     ref_collapse, alt_collapse, same_5_prime, same_3_prime = split_common_sequence(ref, alt)
     start_offset = len(same_5_prime)
     end_offset = len(same_3_prime)
 
-    # If the event is an insertion or deletion, preserve the 5' and 3' ref bases
+    # If the event is an insertion preserve the 5' and 3' ref bases
     if same_5_prime and same_3_prime:
         if len(ref_collapse) < len(alt_collapse):
             ref_collapse = same_5_prime[-1] + ref_collapse + same_3_prime[0]
             alt_collapse = same_5_prime[-1] + alt_collapse + same_3_prime[0]
             start_offset -= 1
             end_offset -= 1
```

### Comparing `pyvariant-2.2.0/pyvariant/variants.py` & `pyvariant-2.2.1/pyvariant/variants.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.2.0/pyvariant.egg-info/PKG-INFO` & `pyvariant-2.2.1/pyvariant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvariant
-Version: 2.2.0
+Version: 2.2.1
 Summary: Map biological sequence variants (mutations) to their equivalent chromosome, cDNA, gene, exon, protein, and RNA positions.
 Home-page: https://github.com/mattdoug604/pyvariant.git
 Author: Matthew Douglas
 Author-email: mattdoug604@gmail.com
 Maintainer: Matthew Douglas
 Maintainer-email: mattdoug604@gmail.com
 License: MIT
```

### Comparing `pyvariant-2.2.0/pyvariant.egg-info/SOURCES.txt` & `pyvariant-2.2.1/pyvariant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvariant-2.2.0/setup.cfg` & `pyvariant-2.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyvariant
-version = 2.2.0
+version = 2.2.1
 description = Map biological sequence variants (mutations) to their equivalent chromosome, cDNA, gene, exon, protein, and RNA positions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mattdoug604/pyvariant.git
 author = Matthew Douglas
 author_email = mattdoug604@gmail.com
 maintainer = Matthew Douglas
```

### Comparing `pyvariant-2.2.0/tests/test_core.py` & `pyvariant-2.2.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.2.0/tests/test_core_map.py` & `pyvariant-2.2.1/tests/test_core_map.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 
 def assert_and_select_expected(output: List, expected: str):
     """Select the expected variant from a list (if it exists) for further testing."""
     # If there is no expected variant output, assert the function returned an empty list
     if not expected:
         assert not output, f"Expected no output, got: {output}"
+        return
 
     # Assert that the expected variant is in the list of variants returned by the function
     str_to_variant = {str(i): i for i in output}
     assert expected in str_to_variant, f"Expected {expected}, got: {list(str_to_variant)}"
 
     return str_to_variant[expected]
 
@@ -142,40 +143,58 @@
     if select := assert_and_select_expected(output, params["rna_str"]):
         assert_rna_has_attributes(select, params)
 
 
 @pytest.mark.parametrize("params", select_params(["protein_str"]), ids=lambda x: x["protein_str"])
 def test_protein_to_cdna_from_str(ensembl100: EnsemblRelease, params: Dict):
     """Test that a protein variant can be parsed from a string and mapped to the expected cDNA variant."""
+    if "fs" in params["protein_str"]:
+        print("Not expecting to be able to map protein frame shift to a non-protein variant")
+        expected = ""
+    else:
+        expected = params["cdna_str"]
+
     output = ensembl100.to_cdna(params["protein_str"])
-    if select := assert_and_select_expected(output, params["cdna_str"]):
+    if select := assert_and_select_expected(output, expected):
         assert_cdna_has_attributes(select, params)
 
 
 @pytest.mark.parametrize("params", select_params(["protein_str"]), ids=lambda x: x["protein_str"])
 def test_protein_to_dna_from_str(ensembl100: EnsemblRelease, params: Dict):
     """Test that a protein variant can be parsed from a string and mapped to the expected DNA variant."""
+    if "fs" in params["protein_str"]:
+        print("Not expecting to be able to map protein frame shift to a non-protein variant")
+        expected = ""
+    else:
+        expected = params["dna_str"]
+
     output = ensembl100.to_dna(params["protein_str"])
-    if select := assert_and_select_expected(output, params["dna_str"]):
+    if select := assert_and_select_expected(output, expected):
         assert_dna_has_attributes(select, params)
 
 
 @pytest.mark.parametrize("params", select_params(["protein_str"]), ids=lambda x: x["protein_str"])
 def test_protein_to_protein_from_str(ensembl100: EnsemblRelease, params: Dict):
     """Test that a protein variant can be parsed from a string and mapped to the expected protein variant."""
     output = ensembl100.to_protein(params["protein_str"])
     if select := assert_and_select_expected(output, params["protein_str"]):
         assert_protein_has_attributes(select, params)
 
 
 @pytest.mark.parametrize("params", select_params(["protein_str"]), ids=lambda x: x["protein_str"])
 def test_protein_to_rna_from_str(ensembl100: EnsemblRelease, params: Dict):
     """Test that a protein variant can be parsed from a string and mapped to the expected RNA variant."""
+    if "fs" in params["protein_str"]:
+        print("Not expecting to be able to map protein frame shift to a non-protein variant")
+        expected = ""
+    else:
+        expected = params["rna_str"]
+
     output = ensembl100.to_rna(params["protein_str"])
-    if select := assert_and_select_expected(output, params["rna_str"]):
+    if select := assert_and_select_expected(output, expected):
         assert_rna_has_attributes(select, params)
 
 
 @pytest.mark.parametrize("params", select_params(["rna_str"]), ids=lambda x: x["rna_str"])
 def test_rna_to_cdna_from_str(ensembl100: EnsemblRelease, params: Dict):
     """Test that a RNA variant can be parsed from a string and mapped to the expected cDNA variant."""
     output = ensembl100.to_cdna(params["rna_str"])
```

### Comparing `pyvariant-2.2.0/tests/test_ensembl_cache.py` & `pyvariant-2.2.1/tests/test_ensembl_cache.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.2.0/tests/test_ensembl_release.py` & `pyvariant-2.2.1/tests/test_ensembl_release.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.2.0/tests/test_files.py` & `pyvariant-2.2.1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.2.0/tests/test_parser.py` & `pyvariant-2.2.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.2.0/tests/test_sequence.py` & `pyvariant-2.2.1/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.2.0/tests/test_utils.py` & `pyvariant-2.2.1/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,20 +66,22 @@
     assert split_common_sequence("GCTGGT", "GCTACTGGT") == ("", "ACT", "GCT", "GGT")
 
 
 def test_expand_nt():
     assert list(expand_nt("A")) == ["A"]
     assert list(expand_nt("R")) == ["A", "G"]
     assert list(expand_nt("N")) == ["A", "C", "G", "T"]
+    assert list(expand_nt("")) == [""]
 
 
 def test_expand_pep():
     assert list(expand_pep("A")) == ["A"]
     assert list(expand_pep("Z")) == ["E", "Q"]
     assert len(list(expand_pep("X"))) == 20  # all amino acids except '*'
+    assert list(expand_pep("")) == [""]
 
 
 def test_format_hgvs_position():
     assert format_hgvs_position(5, 0) == "5"
     assert format_hgvs_position(5, 1) == "5+1"
     assert format_hgvs_position(5, -1) == "5-1"
     assert format_hgvs_position(1, 1) == "+1"
```

