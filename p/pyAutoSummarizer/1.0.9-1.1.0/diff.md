# Comparing `tmp/pyAutoSummarizer-1.0.9.tar.gz` & `tmp/pyAutoSummarizer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyAutoSummarizer-1.0.9.tar", last modified: Fri Jun  2 23:15:11 2023, max compression
+gzip compressed data, was "dist\pyAutoSummarizer-1.1.0.tar", last modified: Sat Jun  3 02:14:36 2023, max compression
```

## Comparing `pyAutoSummarizer-1.0.9.tar` & `pyAutoSummarizer-1.1.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 23:15:11.000000 pyAutoSummarizer-1.0.9/
--rw-rw-rw-   0        0        0      674 2023-05-18 23:07:37.000000 pyAutoSummarizer-1.0.9/LICENSE
--rw-rw-rw-   0        0        0       50 2023-05-18 23:07:52.000000 pyAutoSummarizer-1.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     4761 2023-06-02 23:15:11.000000 pyAutoSummarizer-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     4361 2023-05-31 14:12:43.000000 pyAutoSummarizer-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 23:15:11.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 23:15:11.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/
--rw-rw-rw-   0        0        0       31 2023-05-13 15:40:37.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/__init__.py
--rw-rw-rw-   0        0        0    31047 2023-06-02 23:10:55.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/psr.py
-drwxrwxrwx   0        0        0        0 2023-06-02 23:15:11.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/
--rw-rw-rw-   0        0        0     6482 2023-05-31 13:32:50.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Arabic.txt
--rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Bengali.txt
--rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Bulgarian.txt
--rw-rw-rw-   0        0        0     3295 2023-05-28 21:46:34.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Chinese.txt
--rw-rw-rw-   0        0        0     1934 2023-05-31 13:36:06.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Czech.txt
--rw-rw-rw-   0        0        0     4284 2023-05-31 13:37:00.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-English.txt
--rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Finnish.txt
--rw-rw-rw-   0        0        0     3484 2023-05-31 13:37:46.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-French.txt
--rw-rw-rw-   0        0        0     4302 2023-05-31 13:39:46.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-German.txt
--rw-rw-rw-   0        0        0     7901 2023-05-28 21:47:27.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Greek.txt
--rw-rw-rw-   0        0        0     1656 2023-05-28 21:47:36.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Hebrew.txt
--rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Hindi.txt
--rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Hungarian.txt
--rw-rw-rw-   0        0        0     4074 2023-05-31 13:48:26.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Italian.txt
--rw-rw-rw-   0        0        0     2202 2023-05-28 21:48:04.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Japanese.txt
--rw-rw-rw-   0        0        0     7417 2023-05-28 21:48:29.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Korean.txt
--rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Marathi.txt
--rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Persian.txt
--rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Polish.txt
--rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Portuguese-br.txt
--rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Romanian.txt
--rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Russian.txt
--rw-rw-rw-   0        0        0      883 2023-05-28 21:48:40.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Slovak.txt
--rw-rw-rw-   0        0        0     3128 2023-05-31 13:53:58.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Spanish.txt
--rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Swedish.txt
--rw-rw-rw-   0        0        0     1521 2023-05-28 21:58:26.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Thai.txt
--rw-rw-rw-   0        0        0      627 2023-05-28 21:49:00.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Ukrainian.txt
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 23:15:11.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer.egg-info/
--rw-rw-rw-   0        0        0     4761 2023-06-02 23:15:11.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1724 2023-06-02 23:15:11.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 23:15:11.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-06-02 23:15:11.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-02 23:15:11.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-02 23:15:11.000000 pyAutoSummarizer-1.0.9/pyAutoSummarizer.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-06-02 23:15:11.000000 pyAutoSummarizer-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-06-02 23:11:32.000000 pyAutoSummarizer-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 02:14:36.000000 pyAutoSummarizer-1.1.0/
+-rw-rw-rw-   0        0        0      674 2023-05-18 23:07:37.000000 pyAutoSummarizer-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-05-18 23:07:52.000000 pyAutoSummarizer-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4973 2023-06-03 02:14:36.000000 pyAutoSummarizer-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4572 2023-06-03 02:09:56.000000 pyAutoSummarizer-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 02:14:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 02:14:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/
+-rw-rw-rw-   0        0        0       31 2023-05-13 15:40:37.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/__init__.py
+-rw-rw-rw-   0        0        0    32162 2023-06-03 02:11:24.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/psr.py
+drwxrwxrwx   0        0        0        0 2023-06-03 02:14:36.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/
+-rw-rw-rw-   0        0        0     6482 2023-05-31 13:32:50.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Arabic.txt
+-rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Bengali.txt
+-rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Bulgarian.txt
+-rw-rw-rw-   0        0        0     3295 2023-05-28 21:46:34.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Chinese.txt
+-rw-rw-rw-   0        0        0     1934 2023-05-31 13:36:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Czech.txt
+-rw-rw-rw-   0        0        0     4284 2023-05-31 13:37:00.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-English.txt
+-rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Finnish.txt
+-rw-rw-rw-   0        0        0     3484 2023-05-31 13:37:46.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-French.txt
+-rw-rw-rw-   0        0        0     4302 2023-05-31 13:39:46.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-German.txt
+-rw-rw-rw-   0        0        0     7901 2023-05-28 21:47:27.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Greek.txt
+-rw-rw-rw-   0        0        0     1656 2023-05-28 21:47:36.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Hebrew.txt
+-rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Hindi.txt
+-rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Hungarian.txt
+-rw-rw-rw-   0        0        0     4074 2023-05-31 13:48:26.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Italian.txt
+-rw-rw-rw-   0        0        0     2202 2023-05-28 21:48:04.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Japanese.txt
+-rw-rw-rw-   0        0        0     7417 2023-05-28 21:48:29.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Korean.txt
+-rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Marathi.txt
+-rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Persian.txt
+-rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Polish.txt
+-rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Portuguese-br.txt
+-rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Romanian.txt
+-rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Russian.txt
+-rw-rw-rw-   0        0        0      883 2023-05-28 21:48:40.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Slovak.txt
+-rw-rw-rw-   0        0        0     3128 2023-05-31 13:53:58.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Spanish.txt
+-rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Swedish.txt
+-rw-rw-rw-   0        0        0     1521 2023-05-28 21:58:26.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Thai.txt
+-rw-rw-rw-   0        0        0      627 2023-05-28 21:49:00.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Ukrainian.txt
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 02:14:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer.egg-info/
+-rw-rw-rw-   0        0        0     4973 2023-06-03 02:14:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1724 2023-06-03 02:14:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 02:14:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-06-03 02:14:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-03 02:14:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-03 02:14:35.000000 pyAutoSummarizer-1.1.0/pyAutoSummarizer.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-06-03 02:14:36.000000 pyAutoSummarizer-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-06-03 01:21:36.000000 pyAutoSummarizer-1.1.0/setup.py
```

### Comparing `pyAutoSummarizer-1.0.9/LICENSE` & `pyAutoSummarizer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/PKG-INFO` & `pyAutoSummarizer-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyAutoSummarizer
-Version: 1.0.9
+Version: 1.1.0
 Summary: An Extractive and Abstractive Summarization Library Powered with Artificial Intelligence
 Home-page: https://github.com/Valdecy/pyAutoSummarizer
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyAutoSummarizer
 
 pyAutoSummarizer - An Extractive and Abstractive Summarization Library Powered with Artificial Intelligence. 
 
 ## Introduction
 
-pyAutoSummarizer is a sophisticated Python library developed to handle the complex task of text summarization, an essential component of NLP (Natural Language Processing). The library implements several advanced summarization algorithms, both extractive and abstractive. Extractive summarization algorithms focus on identifying and extracting key sentences or phrases from the original text to form the summary. Among the techniques utilized by pyAutoSummarizer are **TextRank**, **LexRank**, **LSA** (Latent Semantic Analysis), and **KL-Sum**. In the domain of deep learning, pyAutoSummarizer incorporates the use of **T5** (Text-to-Text Transfer Transformer) model, which is known for its versatility in handling a range of language tasks including summarization. Furthermore, pyAutoSummarizer also utilizes **PEGASUS** (Pre-training with Extracted Gap-sentences for Abstractive Summarization) and the OpenAI's GPT (Generative Pretrained Transformer), specifically the **chatGPT** model for abstractive summarization. Unlike extractive techniques, abstractive summarization involves generating new sentences, offering a summary that maintains the essence of the original text but may not use the exact wording.
+pyAutoSummarizer is a sophisticated Python library developed to handle the complex task of text summarization, an essential component of NLP (Natural Language Processing). The library implements several advanced summarization algorithms, both extractive and abstractive. Extractive summarization algorithms focus on identifying and extracting key sentences or phrases from the original text to form the summary. Among the techniques utilized by pyAutoSummarizer are **TextRank**, **LexRank**, **LSA** (Latent Semantic Analysis), and **KL-Sum**. In the domain of deep learning, pyAutoSummarizer incorporates **BART** (Bidirectional and Auto-Regressive Transformers) and the use of **T5** (Text-to-Text Transfer Transformer) model, which is known for its versatility in handling a range of language tasks including summarization. Furthermore, pyAutoSummarizer also utilizes **PEGASUS** (Pre-training with Extracted Gap-sentences for Abstractive Summarization) and the OpenAI's GPT (Generative Pretrained Transformer), specifically the **chatGPT** model for abstractive summarization. Unlike extractive techniques, abstractive summarization involves generating new sentences, offering a summary that maintains the essence of the original text but may not use the exact wording.
 
 pyAutoSummarizer stands out for its proficient preprocessing capabilities that pave the way for high-quality text summarization. Recognizing the importance of text normalization, the library offers a range of text cleansing and standardization features. It can convert text to **lowercase**, ensuring uniformity across the data. Additionally, it can **remove accents**, **remove special characters**, and **remove numbers**, which helps mitigate the text's noise. It also offers the functionality to **remove custom words**, enabling users to tailor their preprocessing needs. Notably, pyAutoSummarizer supports **stopwords** removal across various languages, including Arabic, Bengali, Bulgarian, Chinese, Czech, English, Finnish, French, German, Greek, Hebrew, Hind, Hungarian, Italian, Japanese, Korean, Marathi, Persia, Polish, Portuguese-br, Romanian, Russian, Slovak, Spanish, Swedish, Thai, and Ukrainian. The library provides flexibility in sentence segmentation, allowing sentences to be split based on **punctuation**, **character count**, or **word count**. 
 
 To evaluate the quality of the summaries generated, pyAutoSummarizer integrates various metrics such as **Rouge-N**, **Rouge-L**, and **Rouge-S**, which compare the overlap of n-grams, longest common subsequence, and skip-bigram between the generated summary and the reference summary respectively. Additionally, it employs **BLEU** (Bilingual Evaluation Understudy), and **METEOR** (Metric for Evaluation of Translation with Explicit ORdering).
 
 ## Usage
 
@@ -27,19 +27,20 @@
 ```bash
 pip install pyAutoSummarizer
 ```
 
 2. Try it in **Colab**:
 
 Extractive Summarization
-- Example 01: TextRank           ([ Colab Demo ](https://colab.research.google.com/drive/1m7mF4R7s6hakuVhrwymrgqNNJpTySUM4?usp=sharing#scrollTo=npuyBY596tJ5))
-- Example 02: LexRank            ([ Colab Demo ](https://colab.research.google.com/drive/1gT9fV7hAE4mvwAHbfzolF6TN3TjGgJOF?usp=sharing#scrollTo=npuyBY596tJ5))
-- Example 03: LSA                ([ Colab Demo ](https://colab.research.google.com/drive/19fUslzp43_Owib9YDCb0Xfe9XZm1OKmB?usp=sharing#scrollTo=npuyBY596tJ5))
-- Example 04: KL-Sum             ([ Colab Demo ](https://colab.research.google.com/drive/19zHjE0nR1GcAWi4NQmaJh1gjpqm4sqjP?usp=sharing#scrollTo=npuyBY596tJ5))
-- Example 05: T5 (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1tyWu-19xA9QMrwl_kPcGJH0ZSS3r_rDZ?usp=sharing#scrollTo=npuyBY596tJ5))
+- Example 01: TextRank             ([ Colab Demo ](https://colab.research.google.com/drive/1m7mF4R7s6hakuVhrwymrgqNNJpTySUM4?usp=sharing#scrollTo=npuyBY596tJ5))
+- Example 02: LexRank              ([ Colab Demo ](https://colab.research.google.com/drive/1gT9fV7hAE4mvwAHbfzolF6TN3TjGgJOF?usp=sharing#scrollTo=npuyBY596tJ5))
+- Example 03: LSA                  ([ Colab Demo ](https://colab.research.google.com/drive/19fUslzp43_Owib9YDCb0Xfe9XZm1OKmB?usp=sharing#scrollTo=npuyBY596tJ5))
+- Example 04: KL-Sum               ([ Colab Demo ](https://colab.research.google.com/drive/19zHjE0nR1GcAWi4NQmaJh1gjpqm4sqjP?usp=sharing#scrollTo=npuyBY596tJ5))
+- Example 05: BART (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1sAYBDQFxwlA16nBUozgE28_xZlNzUCg-?usp=sharing))
+- Example 06: T5 (Deep Learning)   ([ Colab Demo ](https://colab.research.google.com/drive/1tyWu-19xA9QMrwl_kPcGJH0ZSS3r_rDZ?usp=sharing#scrollTo=npuyBY596tJ5))
 
 Abstractive Summarization. 
 - Example 01: chatGPT (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1ipl6ZnyumJeuxsYelcmZEdsXDMIuM5WG?usp=sharing#scrollTo=npuyBY596tJ5)) Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
 - Example 02: PEGASUS (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1RWIEm9WoZBPYA_p4A1LqKnFPaXhNsQcM?usp=sharing))
 
 ## Others
```

### Comparing `pyAutoSummarizer-1.0.9/README.md` & `pyAutoSummarizer-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pyAutoSummarizer
 
 pyAutoSummarizer - An Extractive and Abstractive Summarization Library Powered with Artificial Intelligence. 
 
 ## Introduction
 
-pyAutoSummarizer is a sophisticated Python library developed to handle the complex task of text summarization, an essential component of NLP (Natural Language Processing). The library implements several advanced summarization algorithms, both extractive and abstractive. Extractive summarization algorithms focus on identifying and extracting key sentences or phrases from the original text to form the summary. Among the techniques utilized by pyAutoSummarizer are **TextRank**, **LexRank**, **LSA** (Latent Semantic Analysis), and **KL-Sum**. In the domain of deep learning, pyAutoSummarizer incorporates the use of **T5** (Text-to-Text Transfer Transformer) model, which is known for its versatility in handling a range of language tasks including summarization. Furthermore, pyAutoSummarizer also utilizes **PEGASUS** (Pre-training with Extracted Gap-sentences for Abstractive Summarization) and the OpenAI's GPT (Generative Pretrained Transformer), specifically the **chatGPT** model for abstractive summarization. Unlike extractive techniques, abstractive summarization involves generating new sentences, offering a summary that maintains the essence of the original text but may not use the exact wording.
+pyAutoSummarizer is a sophisticated Python library developed to handle the complex task of text summarization, an essential component of NLP (Natural Language Processing). The library implements several advanced summarization algorithms, both extractive and abstractive. Extractive summarization algorithms focus on identifying and extracting key sentences or phrases from the original text to form the summary. Among the techniques utilized by pyAutoSummarizer are **TextRank**, **LexRank**, **LSA** (Latent Semantic Analysis), and **KL-Sum**. In the domain of deep learning, pyAutoSummarizer incorporates **BART** (Bidirectional and Auto-Regressive Transformers) and the use of **T5** (Text-to-Text Transfer Transformer) model, which is known for its versatility in handling a range of language tasks including summarization. Furthermore, pyAutoSummarizer also utilizes **PEGASUS** (Pre-training with Extracted Gap-sentences for Abstractive Summarization) and the OpenAI's GPT (Generative Pretrained Transformer), specifically the **chatGPT** model for abstractive summarization. Unlike extractive techniques, abstractive summarization involves generating new sentences, offering a summary that maintains the essence of the original text but may not use the exact wording.
 
 pyAutoSummarizer stands out for its proficient preprocessing capabilities that pave the way for high-quality text summarization. Recognizing the importance of text normalization, the library offers a range of text cleansing and standardization features. It can convert text to **lowercase**, ensuring uniformity across the data. Additionally, it can **remove accents**, **remove special characters**, and **remove numbers**, which helps mitigate the text's noise. It also offers the functionality to **remove custom words**, enabling users to tailor their preprocessing needs. Notably, pyAutoSummarizer supports **stopwords** removal across various languages, including Arabic, Bengali, Bulgarian, Chinese, Czech, English, Finnish, French, German, Greek, Hebrew, Hind, Hungarian, Italian, Japanese, Korean, Marathi, Persia, Polish, Portuguese-br, Romanian, Russian, Slovak, Spanish, Swedish, Thai, and Ukrainian. The library provides flexibility in sentence segmentation, allowing sentences to be split based on **punctuation**, **character count**, or **word count**. 
 
 To evaluate the quality of the summaries generated, pyAutoSummarizer integrates various metrics such as **Rouge-N**, **Rouge-L**, and **Rouge-S**, which compare the overlap of n-grams, longest common subsequence, and skip-bigram between the generated summary and the reference summary respectively. Additionally, it employs **BLEU** (Bilingual Evaluation Understudy), and **METEOR** (Metric for Evaluation of Translation with Explicit ORdering).
 
 ## Usage
 
@@ -16,19 +16,20 @@
 ```bash
 pip install pyAutoSummarizer
 ```
 
 2. Try it in **Colab**:
 
 Extractive Summarization
-- Example 01: TextRank           ([ Colab Demo ](https://colab.research.google.com/drive/1m7mF4R7s6hakuVhrwymrgqNNJpTySUM4?usp=sharing#scrollTo=npuyBY596tJ5))
-- Example 02: LexRank            ([ Colab Demo ](https://colab.research.google.com/drive/1gT9fV7hAE4mvwAHbfzolF6TN3TjGgJOF?usp=sharing#scrollTo=npuyBY596tJ5))
-- Example 03: LSA                ([ Colab Demo ](https://colab.research.google.com/drive/19fUslzp43_Owib9YDCb0Xfe9XZm1OKmB?usp=sharing#scrollTo=npuyBY596tJ5))
-- Example 04: KL-Sum             ([ Colab Demo ](https://colab.research.google.com/drive/19zHjE0nR1GcAWi4NQmaJh1gjpqm4sqjP?usp=sharing#scrollTo=npuyBY596tJ5))
-- Example 05: T5 (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1tyWu-19xA9QMrwl_kPcGJH0ZSS3r_rDZ?usp=sharing#scrollTo=npuyBY596tJ5))
+- Example 01: TextRank             ([ Colab Demo ](https://colab.research.google.com/drive/1m7mF4R7s6hakuVhrwymrgqNNJpTySUM4?usp=sharing#scrollTo=npuyBY596tJ5))
+- Example 02: LexRank              ([ Colab Demo ](https://colab.research.google.com/drive/1gT9fV7hAE4mvwAHbfzolF6TN3TjGgJOF?usp=sharing#scrollTo=npuyBY596tJ5))
+- Example 03: LSA                  ([ Colab Demo ](https://colab.research.google.com/drive/19fUslzp43_Owib9YDCb0Xfe9XZm1OKmB?usp=sharing#scrollTo=npuyBY596tJ5))
+- Example 04: KL-Sum               ([ Colab Demo ](https://colab.research.google.com/drive/19zHjE0nR1GcAWi4NQmaJh1gjpqm4sqjP?usp=sharing#scrollTo=npuyBY596tJ5))
+- Example 05: BART (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1sAYBDQFxwlA16nBUozgE28_xZlNzUCg-?usp=sharing))
+- Example 06: T5 (Deep Learning)   ([ Colab Demo ](https://colab.research.google.com/drive/1tyWu-19xA9QMrwl_kPcGJH0ZSS3r_rDZ?usp=sharing#scrollTo=npuyBY596tJ5))
 
 Abstractive Summarization. 
 - Example 01: chatGPT (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1ipl6ZnyumJeuxsYelcmZEdsXDMIuM5WG?usp=sharing#scrollTo=npuyBY596tJ5)) Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
 - Example 02: PEGASUS (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1RWIEm9WoZBPYA_p4A1LqKnFPaXhNsQcM?usp=sharing))
 
 ## Others
```

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/psr.py` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/psr.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from . import stws
 
 from itertools import combinations
 from sentence_transformers import SentenceTransformer 
 from sklearn.feature_extraction.text import CountVectorizer
 from sklearn.feature_extraction.text import TfidfVectorizer
 from sklearn.metrics.pairwise import cosine_similarity
+from transformers import BartTokenizer, BartForConditionalGeneration
 from transformers import T5ForConditionalGeneration, T5Tokenizer
 from transformers import PegasusForConditionalGeneration, PegasusTokenizer
 
 ############################################################################
 
 class summarization():
     def __init__(self, text, stop_words = ['en'], n_words = 0, n_chars = 0, lowercase = True, rmv_accents = True, rmv_special_chars = True, rmv_numbers = True, rmv_custom_words = [], verbose = False):
@@ -103,22 +104,23 @@
                     sentence_parts.append(part)
                 sentences.extend(sentence_parts)
             else:
                 sentences.append(sentence)
         return sentences
 
     # Function: Show Summary
-    def show_summary(self, rank, n = 3):
+    def show_summary(self, rank, n = 3, verbose = False):
         idx       = np.argsort(rank)[::-1]
         self.summ = []
         if (n > len(rank)):
             n = len(rank)
         for i in range(0, n):
             sentence =  self.original[idx[i]]
-            print(sentence)
+            if (verbose == True):
+                print(sentence)
             self.summ.append(sentence)
         self.summ = ' '.join(self.summ)
         return self.summ
     
     # Function: Text Pre-Processing
     def clear_text(self, corpus, stop_words = ['en'], lowercase = True, rmv_accents = True, rmv_special_chars = True, rmv_numbers = True, rmv_custom_words = [], verbose = False):
         self.sw_full = []
@@ -565,52 +567,75 @@
             if (rank[i] == 1):
                 rank[i]  = rank_sum
                 rank_sum = rank_sum - 1
         rank = np.array(rank)
         return rank
 
     ##############################################################################   
-
-    # Function: T5
-    def summ_ext_t5(self, model = 't5-base', min_len = 30, max_len = 250):
-        tokenizer = T5Tokenizer.from_pretrained(model)
+    
+    # BART
+    
+    # Function: BART
+    def summ_ext_bart(self, model = 'facebook/bart-large-cnn', max_len = 250, verbose = False):
+        tokenizer = BartTokenizer.from_pretrained(model)
+        bart      = BartForConditionalGeneration.from_pretrained(model)
+        inputs    = tokenizer([self.full_txt], max_length = 1024, truncation = True, padding = 'longest', return_tensors = 'pt')
+        outputs   = bart.generate(inputs['input_ids'], num_beams = 4, max_length = max_len, early_stopping = True)
+        summary   = tokenizer.decode(outputs[0], skip_special_tokens = True)
+        self.summ = summary
+        if (verbose == True):
+            print(summary)
+        return summary
+        
+    # T5
+    
+    # Function: T5       
+    def summ_ext_t5(self, model = 't5-base', min_len = 30, max_len = 250, model_max_length = 512, verbose = False):
+        tokenizer = T5Tokenizer.from_pretrained(model, model_max_length = model_max_length)
         t5_model  = T5ForConditionalGeneration.from_pretrained(model)
-        inputs    = tokenizer.encode('summarize: ' + self.full_txt, return_tensors = 'pt', max_length = 512, truncation = True)
+        inputs    = tokenizer.encode('summarize: ' + self.full_txt, return_tensors = 'pt', truncation = True)
         outputs   = t5_model.generate(inputs, min_length = min_len, max_length = max_len, num_beams = 4, no_repeat_ngram_size = 2)
         summary   = tokenizer.decode(outputs[0], skip_special_tokens = True)
-        self.summ = summary 
-        print(summary)
+        self.summ = summary
+        if (verbose == True):
+            print(summary)
         return summary
-
+        
     ##############################################################################
     
+    # PEGASUS
+    
+    # Function: PEGASUS
+    def summ_abst_pegasus(self, model_name = 'google/pegasus-xsum', min_L = 100, max_L = 150, verbose = False):
+        tokenizer = PegasusTokenizer.from_pretrained(model_name)
+        pegasus   = PegasusForConditionalGeneration.from_pretrained(model_name)
+        tokens    = tokenizer.encode('summarize: ' + self.full_txt, return_tensors = 'pt', max_length = 1024, truncation = True)
+        summary   = pegasus.generate(tokens, min_length = min_L, max_length = max_L, length_penalty = 2.0, num_beams = 4, early_stopping = True)
+        summary   = tokenizer.decode(summary[0], skip_special_tokens = True)
+        self.summ = summary 
+        if (verbose == True):
+            print(summary)
+        return summary
+    
+    # chatGPT
+    
     # Function: chatGPT
-    def summ_abst_chatgpt(self, api_key = 'your_api_key_here', query = 'make an abstratctive summarization', model = 'text-davinci-003', max_tokens = 250, n = 1, temperature = 0.8):
+    def summ_abst_chatgpt(self, api_key = 'your_api_key_here', query = 'make an abstratctive summarization', model = 'text-davinci-003', max_tokens = 250, n = 1, temperature = 0.8, verbose = False):
         def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
             response = openai.Completion.create(
                                                 engine      = model,
                                                 prompt      = prompt,
                                                 max_tokens  = max_tokens,
                                                 n           = n,
                                                 stop        = None,
                                                 temperature = temperature
                                                 )
             return response.choices[0].text.strip()
         openai.api_key = api_key   
         prompt         = query + ':\n\n' + f'{self.full_txt}\n'
         summary        = query_chatgpt(prompt)
         self.summ      = summary 
-        print(summary)
+        if (verbose == True):
+            print(summary)
         return summary 
-    
-    # Function: PEGASUS
-    def summ_abst_pegasus(self, model_name = 'google/pegasus-xsum', min_L = 100, max_L = 150):
-        tokenizer = PegasusTokenizer.from_pretrained(model_name)
-        pegasus   = PegasusForConditionalGeneration.from_pretrained(model_name)
-        tokens    = tokenizer.encode('summarize: ' + self.full_txt, return_tensors = 'pt', max_length = 1024, truncation = True)
-        summary   = pegasus.generate(tokens, min_length = min_L, max_length = max_L, length_penalty = 2.0, num_beams = 4, early_stopping = True)
-        summary   = tokenizer.decode(summary[0], skip_special_tokens = True)
-        self.summ = summary 
-        print(summary)
-        return summary
 
     ##############################################################################
```

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Arabic.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Arabic.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Bengali.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Bengali.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Bulgarian.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Bulgarian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Chinese.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Chinese.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Czech.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Czech.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-English.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-English.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Finnish.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Finnish.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-French.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-French.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-German.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-German.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Greek.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Greek.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Hebrew.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Hebrew.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Hindi.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Hindi.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Hungarian.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Hungarian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Italian.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Italian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Japanese.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Japanese.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Korean.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Korean.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Marathi.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Marathi.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Persian.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Persian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Polish.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Polish.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Portuguese-br.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Portuguese-br.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Romanian.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Romanian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Russian.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Russian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Slovak.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Slovak.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Spanish.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Spanish.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Swedish.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Swedish.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Thai.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Thai.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer/base/stws/Stopwords-Ukrainian.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer/base/stws/Stopwords-Ukrainian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer.egg-info/PKG-INFO` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyAutoSummarizer
-Version: 1.0.9
+Version: 1.1.0
 Summary: An Extractive and Abstractive Summarization Library Powered with Artificial Intelligence
 Home-page: https://github.com/Valdecy/pyAutoSummarizer
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyAutoSummarizer
 
 pyAutoSummarizer - An Extractive and Abstractive Summarization Library Powered with Artificial Intelligence. 
 
 ## Introduction
 
-pyAutoSummarizer is a sophisticated Python library developed to handle the complex task of text summarization, an essential component of NLP (Natural Language Processing). The library implements several advanced summarization algorithms, both extractive and abstractive. Extractive summarization algorithms focus on identifying and extracting key sentences or phrases from the original text to form the summary. Among the techniques utilized by pyAutoSummarizer are **TextRank**, **LexRank**, **LSA** (Latent Semantic Analysis), and **KL-Sum**. In the domain of deep learning, pyAutoSummarizer incorporates the use of **T5** (Text-to-Text Transfer Transformer) model, which is known for its versatility in handling a range of language tasks including summarization. Furthermore, pyAutoSummarizer also utilizes **PEGASUS** (Pre-training with Extracted Gap-sentences for Abstractive Summarization) and the OpenAI's GPT (Generative Pretrained Transformer), specifically the **chatGPT** model for abstractive summarization. Unlike extractive techniques, abstractive summarization involves generating new sentences, offering a summary that maintains the essence of the original text but may not use the exact wording.
+pyAutoSummarizer is a sophisticated Python library developed to handle the complex task of text summarization, an essential component of NLP (Natural Language Processing). The library implements several advanced summarization algorithms, both extractive and abstractive. Extractive summarization algorithms focus on identifying and extracting key sentences or phrases from the original text to form the summary. Among the techniques utilized by pyAutoSummarizer are **TextRank**, **LexRank**, **LSA** (Latent Semantic Analysis), and **KL-Sum**. In the domain of deep learning, pyAutoSummarizer incorporates **BART** (Bidirectional and Auto-Regressive Transformers) and the use of **T5** (Text-to-Text Transfer Transformer) model, which is known for its versatility in handling a range of language tasks including summarization. Furthermore, pyAutoSummarizer also utilizes **PEGASUS** (Pre-training with Extracted Gap-sentences for Abstractive Summarization) and the OpenAI's GPT (Generative Pretrained Transformer), specifically the **chatGPT** model for abstractive summarization. Unlike extractive techniques, abstractive summarization involves generating new sentences, offering a summary that maintains the essence of the original text but may not use the exact wording.
 
 pyAutoSummarizer stands out for its proficient preprocessing capabilities that pave the way for high-quality text summarization. Recognizing the importance of text normalization, the library offers a range of text cleansing and standardization features. It can convert text to **lowercase**, ensuring uniformity across the data. Additionally, it can **remove accents**, **remove special characters**, and **remove numbers**, which helps mitigate the text's noise. It also offers the functionality to **remove custom words**, enabling users to tailor their preprocessing needs. Notably, pyAutoSummarizer supports **stopwords** removal across various languages, including Arabic, Bengali, Bulgarian, Chinese, Czech, English, Finnish, French, German, Greek, Hebrew, Hind, Hungarian, Italian, Japanese, Korean, Marathi, Persia, Polish, Portuguese-br, Romanian, Russian, Slovak, Spanish, Swedish, Thai, and Ukrainian. The library provides flexibility in sentence segmentation, allowing sentences to be split based on **punctuation**, **character count**, or **word count**. 
 
 To evaluate the quality of the summaries generated, pyAutoSummarizer integrates various metrics such as **Rouge-N**, **Rouge-L**, and **Rouge-S**, which compare the overlap of n-grams, longest common subsequence, and skip-bigram between the generated summary and the reference summary respectively. Additionally, it employs **BLEU** (Bilingual Evaluation Understudy), and **METEOR** (Metric for Evaluation of Translation with Explicit ORdering).
 
 ## Usage
 
@@ -27,19 +27,20 @@
 ```bash
 pip install pyAutoSummarizer
 ```
 
 2. Try it in **Colab**:
 
 Extractive Summarization
-- Example 01: TextRank           ([ Colab Demo ](https://colab.research.google.com/drive/1m7mF4R7s6hakuVhrwymrgqNNJpTySUM4?usp=sharing#scrollTo=npuyBY596tJ5))
-- Example 02: LexRank            ([ Colab Demo ](https://colab.research.google.com/drive/1gT9fV7hAE4mvwAHbfzolF6TN3TjGgJOF?usp=sharing#scrollTo=npuyBY596tJ5))
-- Example 03: LSA                ([ Colab Demo ](https://colab.research.google.com/drive/19fUslzp43_Owib9YDCb0Xfe9XZm1OKmB?usp=sharing#scrollTo=npuyBY596tJ5))
-- Example 04: KL-Sum             ([ Colab Demo ](https://colab.research.google.com/drive/19zHjE0nR1GcAWi4NQmaJh1gjpqm4sqjP?usp=sharing#scrollTo=npuyBY596tJ5))
-- Example 05: T5 (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1tyWu-19xA9QMrwl_kPcGJH0ZSS3r_rDZ?usp=sharing#scrollTo=npuyBY596tJ5))
+- Example 01: TextRank             ([ Colab Demo ](https://colab.research.google.com/drive/1m7mF4R7s6hakuVhrwymrgqNNJpTySUM4?usp=sharing#scrollTo=npuyBY596tJ5))
+- Example 02: LexRank              ([ Colab Demo ](https://colab.research.google.com/drive/1gT9fV7hAE4mvwAHbfzolF6TN3TjGgJOF?usp=sharing#scrollTo=npuyBY596tJ5))
+- Example 03: LSA                  ([ Colab Demo ](https://colab.research.google.com/drive/19fUslzp43_Owib9YDCb0Xfe9XZm1OKmB?usp=sharing#scrollTo=npuyBY596tJ5))
+- Example 04: KL-Sum               ([ Colab Demo ](https://colab.research.google.com/drive/19zHjE0nR1GcAWi4NQmaJh1gjpqm4sqjP?usp=sharing#scrollTo=npuyBY596tJ5))
+- Example 05: BART (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1sAYBDQFxwlA16nBUozgE28_xZlNzUCg-?usp=sharing))
+- Example 06: T5 (Deep Learning)   ([ Colab Demo ](https://colab.research.google.com/drive/1tyWu-19xA9QMrwl_kPcGJH0ZSS3r_rDZ?usp=sharing#scrollTo=npuyBY596tJ5))
 
 Abstractive Summarization. 
 - Example 01: chatGPT (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1ipl6ZnyumJeuxsYelcmZEdsXDMIuM5WG?usp=sharing#scrollTo=npuyBY596tJ5)) Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
 - Example 02: PEGASUS (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1RWIEm9WoZBPYA_p4A1LqKnFPaXhNsQcM?usp=sharing))
 
 ## Others
```

### Comparing `pyAutoSummarizer-1.0.9/pyAutoSummarizer.egg-info/SOURCES.txt` & `pyAutoSummarizer-1.1.0/pyAutoSummarizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.9/setup.py` & `pyAutoSummarizer-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyAutoSummarizer',
-    version='1.0.9',
+    version='1.1.0',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyAutoSummarizer',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

