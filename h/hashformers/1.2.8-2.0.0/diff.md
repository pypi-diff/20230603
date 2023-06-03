# Comparing `tmp/hashformers-1.2.8.tar.gz` & `tmp/hashformers-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashformers-1.2.8.tar", last modified: Fri Apr  8 12:02:25 2022, max compression
+gzip compressed data, was "hashformers-2.0.0.tar", last modified: Sat Jun  3 15:56:03 2023, max compression
```

## Comparing `hashformers-1.2.8.tar` & `hashformers-2.0.0.tar`

### file list

```diff
@@ -1,53 +1,43 @@
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2022-04-08 12:02:25.818687 hashformers-1.2.8/
--rwxrwxrwx   0 user      (1000) user      (1000)     2035 2022-02-04 01:58:05.000000 hashformers-1.2.8/.gitignore
--rwxrwxrwx   0 user      (1000) user      (1000)     1068 2022-02-04 01:58:05.000000 hashformers-1.2.8/LICENSE
--rwxrwxrwx   0 user      (1000) user      (1000)       81 2022-04-08 11:40:55.000000 hashformers-1.2.8/MANIFEST.in
--rwxrwxrwx   0 user      (1000) user      (1000)      233 2022-04-08 12:02:25.819937 hashformers-1.2.8/PKG-INFO
--rwxrwxrwx   0 user      (1000) user      (1000)     3923 2022-03-16 21:34:30.000000 hashformers-1.2.8/README.md
--rwxrwxrwx   0 user      (1000) user      (1000)    20755 2022-02-04 12:53:35.000000 hashformers-1.2.8/barplot_evaluation.png
--rwxrwxrwx   0 user      (1000) user      (1000)    63066 2022-03-16 22:05:53.000000 hashformers-1.2.8/hashformers.ipynb
--rwxrwxrwx   0 user      (1000) user      (1000)    24845 2022-02-04 01:58:05.000000 hashformers-1.2.8/hashformers.png
--rwxrwxrwx   0 user      (1000) user      (1000)      116 2022-02-07 09:02:24.000000 hashformers-1.2.8/requirements.txt
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2022-04-08 12:02:23.875057 hashformers-1.2.8/scripts/
--rwxrwxrwx   0 user      (1000) user      (1000)     4270 2022-02-04 13:41:00.000000 hashformers-1.2.8/scripts/evaluate_ekphrasis.py
--rwxrwxrwx   0 user      (1000) user      (1000)       79 2022-04-08 12:02:25.827674 hashformers-1.2.8/setup.cfg
--rwxrwxrwx   0 user      (1000) user      (1000)      437 2022-04-08 12:02:08.000000 hashformers-1.2.8/setup.py
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2022-04-08 12:02:23.580917 hashformers-1.2.8/src/
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2022-04-08 12:02:23.958521 hashformers-1.2.8/src/hashformers/
--rwxrwxrwx   0 user      (1000) user      (1000)       77 2022-02-12 04:55:28.000000 hashformers-1.2.8/src/hashformers/__init__.py
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2022-04-08 12:02:24.933058 hashformers-1.2.8/src/hashformers/beamsearch/
--rwxrwxrwx   0 user      (1000) user      (1000)        0 2022-02-04 01:58:05.000000 hashformers-1.2.8/src/hashformers/beamsearch/__init__.py
--rwxrwxrwx   0 user      (1000) user      (1000)     2868 2022-02-12 04:55:28.000000 hashformers-1.2.8/src/hashformers/beamsearch/algorithm.py
--rwxrwxrwx   0 user      (1000) user      (1000)     1047 2022-02-04 04:48:33.000000 hashformers-1.2.8/src/hashformers/beamsearch/bert_lm.py
--rwxrwxrwx   0 user      (1000) user      (1000)     4799 2022-02-04 01:58:05.000000 hashformers-1.2.8/src/hashformers/beamsearch/data_structures.py
--rwxrwxrwx   0 user      (1000) user      (1000)     3705 2022-02-06 23:28:31.000000 hashformers-1.2.8/src/hashformers/beamsearch/gpt2_lm.py
--rwxrwxrwx   0 user      (1000) user      (1000)      575 2022-02-10 15:31:17.000000 hashformers-1.2.8/src/hashformers/beamsearch/model_lm.py
--rwxrwxrwx   0 user      (1000) user      (1000)      927 2022-02-12 04:55:28.000000 hashformers-1.2.8/src/hashformers/beamsearch/reranker.py
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2022-04-08 12:02:24.985926 hashformers-1.2.8/src/hashformers/ensemble/
--rwxrwxrwx   0 user      (1000) user      (1000)        0 2022-02-04 01:58:05.000000 hashformers-1.2.8/src/hashformers/ensemble/__init__.py
--rwxrwxrwx   0 user      (1000) user      (1000)     1594 2022-02-12 04:55:28.000000 hashformers-1.2.8/src/hashformers/ensemble/top2_fusion.py
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2022-04-08 12:02:25.095815 hashformers-1.2.8/src/hashformers/evaluation/
--rwxrwxrwx   0 user      (1000) user      (1000)       22 2022-02-04 01:58:05.000000 hashformers-1.2.8/src/hashformers/evaluation/__init__.py
--rwxrwxrwx   0 user      (1000) user      (1000)     3328 2022-02-04 01:58:05.000000 hashformers-1.2.8/src/hashformers/evaluation/modeler.py
--rwxrwxrwx   0 user      (1000) user      (1000)     1688 2022-02-04 05:32:34.000000 hashformers-1.2.8/src/hashformers/evaluation/utils.py
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2022-04-08 12:02:25.256611 hashformers-1.2.8/src/hashformers/experiments/
--rwxrwxrwx   0 user      (1000) user      (1000)        0 2022-02-04 01:58:05.000000 hashformers-1.2.8/src/hashformers/experiments/__init__.py
--rwxrwxrwx   0 user      (1000) user      (1000)     2029 2022-02-04 05:32:44.000000 hashformers-1.2.8/src/hashformers/experiments/evaluation.py
--rwxrwxrwx   0 user      (1000) user      (1000)     2220 2022-02-04 05:32:51.000000 hashformers-1.2.8/src/hashformers/experiments/utils.py
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2022-04-08 12:02:25.768522 hashformers-1.2.8/src/hashformers/segmenter/
--rwxrwxrwx   0 user      (1000) user      (1000)       24 2022-02-10 15:28:36.000000 hashformers-1.2.8/src/hashformers/segmenter/__init__.py
--rwxrwxrwx   0 user      (1000) user      (1000)     4555 2022-03-05 09:38:49.000000 hashformers-1.2.8/src/hashformers/segmenter/auto.py
--rwxrwxrwx   0 user      (1000) user      (1000)     1730 2022-02-12 04:55:28.000000 hashformers-1.2.8/src/hashformers/segmenter/base_segmenter.py
--rwxrwxrwx   0 user      (1000) user      (1000)      632 2022-02-12 04:55:28.000000 hashformers-1.2.8/src/hashformers/segmenter/data_structures.py
--rwxrwxrwx   0 user      (1000) user      (1000)      797 2022-02-12 04:55:28.000000 hashformers-1.2.8/src/hashformers/segmenter/regex_segmenter.py
--rwxrwxrwx   0 user      (1000) user      (1000)     8595 2022-03-05 10:44:14.000000 hashformers-1.2.8/src/hashformers/segmenter/segmenter.py
--rwxrwxrwx   0 user      (1000) user      (1000)     5091 2022-03-05 10:05:25.000000 hashformers-1.2.8/src/hashformers/segmenter/unigram_segmenter.py
--rwxrwxrwx   0 user      (1000) user      (1000)      565 2022-02-12 04:55:28.000000 hashformers-1.2.8/src/hashformers/segmenter/utils.py
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2022-04-08 12:02:24.320285 hashformers-1.2.8/src/hashformers.egg-info/
--rwxrwxrwx   0 user      (1000) user      (1000)      233 2022-04-08 12:02:16.000000 hashformers-1.2.8/src/hashformers.egg-info/PKG-INFO
--rwxrwxrwx   0 user      (1000) user      (1000)     1324 2022-04-08 12:02:23.000000 hashformers-1.2.8/src/hashformers.egg-info/SOURCES.txt
--rwxrwxrwx   0 user      (1000) user      (1000)        1 2022-04-08 12:02:16.000000 hashformers-1.2.8/src/hashformers.egg-info/dependency_links.txt
--rwxrwxrwx   0 user      (1000) user      (1000)       74 2022-04-08 12:02:17.000000 hashformers-1.2.8/src/hashformers.egg-info/requires.txt
--rwxrwxrwx   0 user      (1000) user      (1000)       12 2022-04-08 12:02:17.000000 hashformers-1.2.8/src/hashformers.egg-info/top_level.txt
-drwxrwxrwx   0 user      (1000) user      (1000)        0 2022-04-08 12:02:25.791623 hashformers-1.2.8/tutorials/
--rwxrwxrwx   0 user      (1000) user      (1000)     4769 2022-02-07 11:33:07.000000 hashformers-1.2.8/tutorials/EVALUATION.md
+drwxrwxrwx   0 ruan      (1000) ruan      (1000)        0 2023-06-03 15:56:03.720008 hashformers-2.0.0/
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)     1068 2023-05-23 13:53:27.000000 hashformers-2.0.0/LICENSE
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)       81 2023-05-23 13:53:27.000000 hashformers-2.0.0/MANIFEST.in
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)      188 2023-06-03 15:56:03.720189 hashformers-2.0.0/PKG-INFO
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)     5627 2023-06-03 14:15:05.000000 hashformers-2.0.0/README.md
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)       79 2023-06-03 15:56:03.720869 hashformers-2.0.0/setup.cfg
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)      385 2023-05-25 20:11:44.000000 hashformers-2.0.0/setup.py
+drwxrwxrwx   0 ruan      (1000) ruan      (1000)        0 2023-06-03 15:56:00.861566 hashformers-2.0.0/src/
+drwxrwxrwx   0 ruan      (1000) ruan      (1000)        0 2023-06-03 15:56:03.621155 hashformers-2.0.0/src/hashformers/
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)       77 2023-05-23 13:53:27.000000 hashformers-2.0.0/src/hashformers/__init__.py
+drwxrwxrwx   0 ruan      (1000) ruan      (1000)        0 2023-06-03 15:56:03.640413 hashformers-2.0.0/src/hashformers/beamsearch/
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)        0 2023-05-23 13:53:27.000000 hashformers-2.0.0/src/hashformers/beamsearch/__init__.py
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)     5243 2023-05-23 13:53:27.000000 hashformers-2.0.0/src/hashformers/beamsearch/algorithm.py
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)      948 2023-05-24 20:04:15.000000 hashformers-2.0.0/src/hashformers/beamsearch/bert_lm.py
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)     8512 2023-05-23 13:53:27.000000 hashformers-2.0.0/src/hashformers/beamsearch/data_structures.py
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)      745 2023-05-24 20:03:17.000000 hashformers-2.0.0/src/hashformers/beamsearch/gpt2_lm.py
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)     1714 2023-06-03 10:59:37.000000 hashformers-2.0.0/src/hashformers/beamsearch/minicons_lm.py
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)     2314 2023-05-24 20:25:26.000000 hashformers-2.0.0/src/hashformers/beamsearch/model_lm.py
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)     2541 2023-05-23 13:53:27.000000 hashformers-2.0.0/src/hashformers/beamsearch/reranker.py
+drwxrwxrwx   0 ruan      (1000) ruan      (1000)        0 2023-06-03 15:56:03.642789 hashformers-2.0.0/src/hashformers/ensemble/
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)        0 2023-05-23 13:53:27.000000 hashformers-2.0.0/src/hashformers/ensemble/__init__.py
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)     3504 2023-05-23 13:53:27.000000 hashformers-2.0.0/src/hashformers/ensemble/top2_fusion.py
+drwxrwxrwx   0 ruan      (1000) ruan      (1000)        0 2023-06-03 15:56:03.681671 hashformers-2.0.0/src/hashformers/evaluation/
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)       22 2023-05-23 13:53:27.000000 hashformers-2.0.0/src/hashformers/evaluation/__init__.py
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)     3328 2023-05-23 13:53:27.000000 hashformers-2.0.0/src/hashformers/evaluation/modeler.py
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)     2294 2023-05-23 13:53:27.000000 hashformers-2.0.0/src/hashformers/evaluation/utils.py
+drwxrwxrwx   0 ruan      (1000) ruan      (1000)        0 2023-06-03 15:56:03.699523 hashformers-2.0.0/src/hashformers/experiments/
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)        0 2023-05-23 13:53:27.000000 hashformers-2.0.0/src/hashformers/experiments/__init__.py
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)     4557 2023-05-23 13:53:27.000000 hashformers-2.0.0/src/hashformers/experiments/evaluation.py
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)     4881 2023-05-23 13:53:27.000000 hashformers-2.0.0/src/hashformers/experiments/utils.py
+drwxrwxrwx   0 ruan      (1000) ruan      (1000)        0 2023-06-03 15:56:03.718934 hashformers-2.0.0/src/hashformers/segmenter/
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)       24 2023-05-23 13:53:27.000000 hashformers-2.0.0/src/hashformers/segmenter/__init__.py
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)     3454 2023-05-25 16:30:29.000000 hashformers-2.0.0/src/hashformers/segmenter/auto.py
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)     4120 2023-05-23 13:53:27.000000 hashformers-2.0.0/src/hashformers/segmenter/base_segmenter.py
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)      540 2023-05-23 13:53:27.000000 hashformers-2.0.0/src/hashformers/segmenter/data_structures.py
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)     2330 2023-05-23 13:53:27.000000 hashformers-2.0.0/src/hashformers/segmenter/regex_segmenter.py
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)    13995 2023-05-25 17:29:03.000000 hashformers-2.0.0/src/hashformers/segmenter/segmenter.py
+drwxrwxrwx   0 ruan      (1000) ruan      (1000)        0 2023-06-03 15:56:03.626697 hashformers-2.0.0/src/hashformers.egg-info/
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)      188 2023-06-03 15:56:00.000000 hashformers-2.0.0/src/hashformers.egg-info/PKG-INFO
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)     1145 2023-06-03 15:56:00.000000 hashformers-2.0.0/src/hashformers.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)        1 2023-06-03 15:56:00.000000 hashformers-2.0.0/src/hashformers.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)       36 2023-06-03 15:56:00.000000 hashformers-2.0.0/src/hashformers.egg-info/requires.txt
+-rwxrwxrwx   0 ruan      (1000) ruan      (1000)       12 2023-06-03 15:56:00.000000 hashformers-2.0.0/src/hashformers.egg-info/top_level.txt
```

### Comparing `hashformers-1.2.8/LICENSE` & `hashformers-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hashformers-1.2.8/src/hashformers/evaluation/modeler.py` & `hashformers-2.0.0/src/hashformers/evaluation/modeler.py`

 * *Files identical despite different names*

### Comparing `hashformers-1.2.8/src/hashformers/segmenter/auto.py` & `hashformers-2.0.0/src/hashformers/segmenter/auto.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,62 +2,26 @@
 from hashformers.segmenter import (
     BaseWordSegmenter
 )
 
 from hashformers.beamsearch.algorithm import Beamsearch
 from hashformers.beamsearch.reranker import Reranker
 from hashformers.ensemble.top2_fusion import Top2_Ensembler
-from hashformers.segmenter.unigram_segmenter import UnigramWordSegmenter
-
-class FastWordSegmenter(BaseWordSegmenter):
-    def __init__(
-        self,
-        unigram_lang = "en",
-        unigram_wordlist = "best",
-        unigram_match_cutoff = None,
-        max_split_length=20,
-        reranker_gpu_batch_size = 1000,
-        reranker_model_name_or_path = "distilgpt2",
-        reranker_model_type = "gpt2"      
-    ):
-
-        segmenter_model = UnigramWordSegmenter(
-            max_split_length=max_split_length,
-            lang=unigram_lang,
-            wordlist=unigram_wordlist,
-            match_cutoff=unigram_match_cutoff
-        )
-
-        if reranker_model_name_or_path:
-            reranker_model = Reranker(
-                model_name_or_path=reranker_model_name_or_path,
-                model_type=reranker_model_type,
-                gpu_batch_size=reranker_gpu_batch_size
-            )
-        else:
-            reranker_model = None
-
-        ensembler = Top2_Ensembler()
-
-        super().__init__(
-            segmenter=segmenter_model,
-            reranker=reranker_model,
-            ensembler=ensembler
-        )    
 
 class TransformerWordSegmenter(BaseWordSegmenter):
     def __init__(
         self,
         segmenter_model_name_or_path = "gpt2",
         segmenter_model_type = "gpt2",
         segmenter_device = "cuda",
         segmenter_gpu_batch_size = 1000,
         reranker_gpu_batch_size = 1000,
         reranker_model_name_or_path = None,
-        reranker_model_type = "bert"
+        reranker_model_type = "bert",
+        reranker_device = "cuda"
     ):
         """Word segmentation API initialization. 
            A GPT-2 model must be passed to `segmenter_model_name_or_path`, and optionally a BERT model to `reranker_model_name_or_path`.
            If `reranker_model_name_or_path` is set to `False` or `None`, the word segmenter object will work without a reranker.
 
 
         Args:
@@ -76,15 +40,16 @@
         gpu_batch_size=segmenter_gpu_batch_size
     )
 
         if reranker_model_name_or_path:
             reranker_model = Reranker(
                 model_name_or_path=reranker_model_name_or_path,
                 model_type=reranker_model_type,
-                gpu_batch_size=reranker_gpu_batch_size
+                gpu_batch_size=reranker_gpu_batch_size,
+                device=reranker_device
             )
         else:
             reranker_model = None
 
         ensembler = Top2_Ensembler()
 
         super().__init__(
```

### Comparing `hashformers-1.2.8/src/hashformers/segmenter/data_structures.py` & `hashformers-2.0.0/src/hashformers/segmenter/data_structures.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,13 +14,8 @@
     hashtags: List[List[str]]
     hashtag_set: List[str]
     replacement_dict: dict
 
 @dataclass
 class TweetSegmenterOutput:
     output: List[str]
-    word_segmenter_output: Any
-
-@dataclass
-class CascadeNode:
-    word_segmenter: Any
-    word_segmenter_kwargs: dict
+    word_segmenter_output: Any
```

### Comparing `hashformers-1.2.8/src/hashformers/segmenter/unigram_segmenter.py` & `hashformers-2.0.0/src/hashformers/beamsearch/algorithm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,148 +1,146 @@
-from math import log10
-from math import inf
-from hashformers.segmenter.base_segmenter import BaseSegmenter
-from wordfreq import get_frequency_list
-from functools import reduce
-from hashformers.beamsearch.data_structures import ProbabilityDictionary
-
-def corrected_log10(x):
-    return log10(x) if x != 0 else -inf
-
-class Pdist(dict):
-    """
-    A probability distribution estimated from word counts
-    Notice: if pw = Pdist(unigrams, n_tokens:
-        * pw[w] is the raw count of the word w
-        * pw(w) is the probability of the word w
-    """
-
-    @staticmethod
-    def default_unk_func(key, total):
-        return 1. / total
-
-    def __init__(self, data=None, total=None, unk_func=None, **kwargs):
-        super().__init__(**kwargs)
-
-        # insert the word counts
-        data = data or {}
-        for key, count in data.items():
-            self[key] = self.get(key, 0) + int(count)
-
-        self.total = float(total or sum(self.values()))
-        self.unk_prob = unk_func or self.default_unk_func
-
-    def __call__(self, key):
-        if key in self:
-            return self[key] / self.total
-        else:
-            return self.unk_prob(key, self.total)
-
-
-class UnigramWordSegmenter(BaseSegmenter):
-    """
-    The Segmenter Class implements the Viterbi algorithm for word segmentation.
-    Based on CH14 from the book Beautiful Data (Segaran and Hammerbacher, 2009)
-    """
-    def __init__(self, max_split_length=20, **kwargs):
-        """
-        Args:
-            corpus (str): the statistics from which corpus to use for
-                the spell correction.
-            max_split_length (int): the maximum length of that a word can have
-                for looking for splits
-        """
-        self.unigrams = self.read_stats(**kwargs)
-        self.N = sum(self.unigrams.values())
-        self.L = max_split_length
-
-        self.Pw = Pdist(self.unigrams, self.N, self.unk_probability)
-
-    @staticmethod
-    def read_stats(lang='en', wordlist='best', match_cutoff=None):
-        """
-        Read key,value pairs from file.
-        """
-        output = {}
-        frequency_list = get_frequency_list.__wrapped__(lang, wordlist=wordlist, match_cutoff=match_cutoff)
-        for index in range(len(frequency_list)):
-            j = ~index
-            for word in frequency_list[j]:
-                output[word] = index
-        return output
-
-    def condProbWord(self, word, prev, ngram_sep='_'):
+import itertools
+import re
+from hashformers.beamsearch.data_structures import (
+    Node,
+    ProbabilityDictionary
+)
+
+from hashformers.beamsearch.model_lm import ModelLM
+
+class Beamsearch(ModelLM):
+
+    def __init__(
+            self,
+            model_name_or_path="gpt2", 
+            model_type="gpt2", 
+            device='cuda', 
+            gpu_batch_size=1000):
         """
-        Conditional probability of word, given previous word
-        if bigram is not in our list, then fall back to unigrams
+        Initializes the Beamsearch class.
+
         Args:
-            word (): candidate word
-            prev (): previous observed word
+            model_name_or_path (str): Name of the model or path to the model to be loaded. Default is "gpt2".
+            model_type (str): Type of the model. Default is "gpt2".
+            device (str): Device to be used for computation. Default is 'cuda'.
+            gpu_batch_size (int): Size of the batch to be processed on the GPU. Default is 1000.
+        """
+        super().__init__(
+            model_name_or_path=model_name_or_path, 
+            model_type=model_type, 
+            device=device, 
+            gpu_batch_size=gpu_batch_size)
 
+    def next_step(self, list_of_candidates):
+        """
+        Generates the next possible candidates.
+
+        Args:
+            list_of_candidates (List[str]): List of current candidate strings.
+        
         Returns:
+            List[str]: List of possible next candidates.
+        """
+        output = []
+        for candidate_string in list_of_candidates:
+            candidates = [ 
+                candidate_string[:pos] + ' ' + candidate_string[pos:] \
+                    if pos else candidate_string for pos in range(len(candidate_string)) 
+                ]
+            candidates = list(filter(lambda x: not re.findall(".*?(?=\s{2})", x), candidates))
+            output.extend(candidates)
+        return output
 
+    def update_probabilities(self, tree, prob_dict):
         """
-        return self.Pw(word)
+        Updates the probabilities in the given probability dictionary.
 
-    @staticmethod
-    def unk_probability(key, total):
+        Args:
+            tree (List[str]): List of candidate strings.
+            prob_dict (dict): Dictionary of probabilities of the candidates.
+        
+        Returns:
+            dict: Updated probability dictionary.
         """
-        Estimate the probability of an unknown word, penalizing its length
-        :param key: the word
-        :param total: the count of all tokens
-        :return:
+        for item in tree:
+            current_batch = []
+            for word in item:
+                if word in prob_dict:
+                    continue
+                else:
+                    current_batch.append(word)
+            if current_batch:
+                current_batch_probs = self.model.get_probs(current_batch)
+            for idx, word in enumerate(current_batch):
+                prob_dict[word] = current_batch_probs[idx]
+        return prob_dict
+
+    def reshape_tree(self, tree, measure):
         """
-        return 10. / (total * 10 ** len(key))
+        Reshapes the tree according to the provided measure.
 
-    @staticmethod
-    def combine(first, rem):
+        Args:
+            tree (List[str]): List of candidate strings.
+            measure (int): Measure to reshape the tree.
+        
+        Returns:
+            List[List[str]]: Reshaped tree.
         """
-        Combine first and rem results into one (probability, words) pair
-        :param first: a tuple in the form: probability, word
-        :param rem: a tuple in the form: probability, list_of_words
-        :return:
+        return [ tree[x:x+measure] for x in range(0, len(tree), measure) ]
+
+    def flatten_list(self, list_):
         """
-        (first_prob, first_word) = first
-        (rem_prob, rem_words) = rem
-        return first_prob + rem_prob, [first_word] + rem_words
+        Flattens a nested list.
 
-    def splits(self, text):
+        Args:
+            list_ (List[List[Any]]): Nested list to be flattened.
+        
+        Returns:
+            List[Any]: Flattened list.
         """
-        Return a list of all possible (first, rem) pairs with max length of first <=L
-        :param text:
-        :return:
+        return [ item for sublist in list_ for item in sublist ]
+
+    def trim_tree(self, tree, prob_dict, topk):
         """
-        return [(text[:i + 1], text[i + 1:])
-                for i in range(min(len(text), self.L))]
+        Trims the tree to the top k candidates.
 
-    def find_candidates(self, text, prev='<S>'):
+        Args:
+            tree (List[str]): List of candidate strings.
+            prob_dict (dict): Dictionary of probabilities of the candidates.
+            topk (int): Number of top candidates to be retained.
+        
+        Returns:
+            List[str]: List of top k candidates.
+        """
+        output = []
+        probs = [ prob_dict[x] for x in tree ]
         candidates = [
-            self.combine(
-                (corrected_log10(self.condProbWord(first, prev)), first), 
-                self.find_segment(rem, first))
-                      for first, rem in self.splits(text)]
-        return candidates
-
-    def find_segment(self, text, prev='<S>'):
-        """
-        Return (log P(words), words), where words is the best estimated segmentation
-        :param text: the text to be segmented
-        :param prev:
-        :return:
-        """
-        if not text:
-            return 0.0, []
-        return max(self.find_candidates(text, prev=prev))
-
-    def segment_word(self, word):
-        return " ".join(self.find_segment(word)[1])
-
-    def segment(self, inputs, **kwargs):
-        inputs = super().preprocess(**kwargs)
-        return [ self.segment_word(word) for word in inputs ]
-
-    def run(self, inputs, **kwargs):
-        candidates = [ self.find_candidates(word) for word in inputs ]
-        candidates = reduce(lambda x,y: x+y, candidates)
-        candidates = list(map(lambda x: (" ".join(x[1]),abs(x[0])), candidates))
-        candidates = dict(candidates)
-        return ProbabilityDictionary(dictionary=candidates)
+            Node(item, item.replace(" ", ""), probs[idx]) for idx, item in enumerate(tree)
+        ]
+        for key, group in itertools.groupby(candidates, key=lambda x: x.characters):
+            sorted_group = sorted(list(group), key=lambda x: x.score)
+            trimmed_group = sorted_group[0:topk]
+            trimmed_group = [x.hypothesis for x in trimmed_group]
+            output.extend(trimmed_group)
+        return output
+
+    def run(self, dataset, topk=20, steps=13):
+        """
+        Runs the beamsearch algorithm on the provided dataset.
+
+        Args:
+            dataset (List[str]): List of initial candidate strings.
+            topk (int): Number of top candidates to be retained in each step. Default is 20.
+            steps (int): Number of steps to run the algorithm. Default is 13.
+        
+        Returns:
+            ProbabilityDictionary: Dictionary of final probabilities of the candidates.
+        """
+        tree = dataset
+        prob_dict = {}
+        for i in range(steps):
+            tree = self.next_step(tree)
+            tree = self.reshape_tree(tree, self.gpu_batch_size)
+            prob_dict = self.update_probabilities(tree, prob_dict)
+            tree = self.flatten_list(tree)
+            tree = self.trim_tree(tree, prob_dict, topk)
+        return ProbabilityDictionary(prob_dict)
```

