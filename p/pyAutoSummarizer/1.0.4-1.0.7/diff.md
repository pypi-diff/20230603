# Comparing `tmp/pyAutoSummarizer-1.0.4.tar.gz` & `tmp/pyAutoSummarizer-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyAutoSummarizer-1.0.4.tar", last modified: Wed May 31 14:07:59 2023, max compression
+gzip compressed data, was "dist\pyAutoSummarizer-1.0.7.tar", last modified: Fri Jun  2 22:33:37 2023, max compression
```

## Comparing `pyAutoSummarizer-1.0.4.tar` & `pyAutoSummarizer-1.0.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 14:07:59.000000 pyAutoSummarizer-1.0.4/
--rw-rw-rw-   0        0        0      674 2023-05-18 23:07:37.000000 pyAutoSummarizer-1.0.4/LICENSE
--rw-rw-rw-   0        0        0       50 2023-05-18 23:07:52.000000 pyAutoSummarizer-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4761 2023-05-31 14:07:59.000000 pyAutoSummarizer-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4361 2023-05-31 14:05:55.000000 pyAutoSummarizer-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 14:07:59.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:07:59.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/
--rw-rw-rw-   0        0        0       31 2023-05-13 15:40:37.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/__init__.py
--rw-rw-rw-   0        0        0    31949 2023-05-31 13:56:47.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/psr.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:07:59.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/
--rw-rw-rw-   0        0        0     6482 2023-05-31 13:32:50.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Arabic.txt
--rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Bengali.txt
--rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Bulgarian.txt
--rw-rw-rw-   0        0        0     3295 2023-05-28 21:46:34.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Chinese.txt
--rw-rw-rw-   0        0        0     1934 2023-05-31 13:36:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Czech.txt
--rw-rw-rw-   0        0        0     4284 2023-05-31 13:37:00.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-English.txt
--rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Finnish.txt
--rw-rw-rw-   0        0        0     3484 2023-05-31 13:37:46.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-French.txt
--rw-rw-rw-   0        0        0     4302 2023-05-31 13:39:46.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-German.txt
--rw-rw-rw-   0        0        0     7901 2023-05-28 21:47:27.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Greek.txt
--rw-rw-rw-   0        0        0     1656 2023-05-28 21:47:36.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Hebrew.txt
--rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Hindi.txt
--rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Hungarian.txt
--rw-rw-rw-   0        0        0     4074 2023-05-31 13:48:26.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Italian.txt
--rw-rw-rw-   0        0        0     2202 2023-05-28 21:48:04.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Japanese.txt
--rw-rw-rw-   0        0        0     7417 2023-05-28 21:48:29.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Korean.txt
--rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Marathi.txt
--rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Persian.txt
--rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Polish.txt
--rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Portuguese-br.txt
--rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Romanian.txt
--rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Russian.txt
--rw-rw-rw-   0        0        0      883 2023-05-28 21:48:40.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Slovak.txt
--rw-rw-rw-   0        0        0     3128 2023-05-31 13:53:58.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Spanish.txt
--rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Swedish.txt
--rw-rw-rw-   0        0        0     1521 2023-05-28 21:58:26.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Thai.txt
--rw-rw-rw-   0        0        0      627 2023-05-28 21:49:00.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Ukrainian.txt
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 14:07:59.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer.egg-info/
--rw-rw-rw-   0        0        0     4761 2023-05-31 14:07:57.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1724 2023-05-31 14:07:58.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 14:07:57.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-05-31 14:07:57.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-31 14:07:57.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-31 14:07:57.000000 pyAutoSummarizer-1.0.4/pyAutoSummarizer.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-05-31 14:07:59.000000 pyAutoSummarizer-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      820 2023-05-31 01:42:33.000000 pyAutoSummarizer-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 22:33:37.000000 pyAutoSummarizer-1.0.7/
+-rw-rw-rw-   0        0        0      674 2023-05-18 23:07:37.000000 pyAutoSummarizer-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-05-18 23:07:52.000000 pyAutoSummarizer-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4761 2023-06-02 22:33:37.000000 pyAutoSummarizer-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4361 2023-05-31 14:12:43.000000 pyAutoSummarizer-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 22:33:37.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 22:33:37.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/
+-rw-rw-rw-   0        0        0       31 2023-05-13 15:40:37.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/__init__.py
+-rw-rw-rw-   0        0        0    30831 2023-06-02 22:33:13.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/psr.py
+drwxrwxrwx   0        0        0        0 2023-06-02 22:33:37.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/
+-rw-rw-rw-   0        0        0     6482 2023-05-31 13:32:50.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Arabic.txt
+-rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Bengali.txt
+-rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Bulgarian.txt
+-rw-rw-rw-   0        0        0     3295 2023-05-28 21:46:34.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Chinese.txt
+-rw-rw-rw-   0        0        0     1934 2023-05-31 13:36:06.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Czech.txt
+-rw-rw-rw-   0        0        0     4284 2023-05-31 13:37:00.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-English.txt
+-rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Finnish.txt
+-rw-rw-rw-   0        0        0     3484 2023-05-31 13:37:46.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-French.txt
+-rw-rw-rw-   0        0        0     4302 2023-05-31 13:39:46.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-German.txt
+-rw-rw-rw-   0        0        0     7901 2023-05-28 21:47:27.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Greek.txt
+-rw-rw-rw-   0        0        0     1656 2023-05-28 21:47:36.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Hebrew.txt
+-rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Hindi.txt
+-rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Hungarian.txt
+-rw-rw-rw-   0        0        0     4074 2023-05-31 13:48:26.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Italian.txt
+-rw-rw-rw-   0        0        0     2202 2023-05-28 21:48:04.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Japanese.txt
+-rw-rw-rw-   0        0        0     7417 2023-05-28 21:48:29.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Korean.txt
+-rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Marathi.txt
+-rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Persian.txt
+-rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Polish.txt
+-rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Portuguese-br.txt
+-rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Romanian.txt
+-rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Russian.txt
+-rw-rw-rw-   0        0        0      883 2023-05-28 21:48:40.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Slovak.txt
+-rw-rw-rw-   0        0        0     3128 2023-05-31 13:53:58.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Spanish.txt
+-rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Swedish.txt
+-rw-rw-rw-   0        0        0     1521 2023-05-28 21:58:26.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Thai.txt
+-rw-rw-rw-   0        0        0      627 2023-05-28 21:49:00.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Ukrainian.txt
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 22:33:37.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer.egg-info/
+-rw-rw-rw-   0        0        0     4761 2023-06-02 22:33:37.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1724 2023-06-02 22:33:37.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 22:33:37.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-06-02 22:33:37.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-02 22:33:37.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-02 22:33:37.000000 pyAutoSummarizer-1.0.7/pyAutoSummarizer.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-06-02 22:33:37.000000 pyAutoSummarizer-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-06-02 22:33:28.000000 pyAutoSummarizer-1.0.7/setup.py
```

### Comparing `pyAutoSummarizer-1.0.4/LICENSE` & `pyAutoSummarizer-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/PKG-INFO` & `pyAutoSummarizer-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAutoSummarizer
-Version: 1.0.4
+Version: 1.0.7
 Summary: An Extractive and Abstractive Summarization Library Powered with Artificial Intelligence
 Home-page: https://github.com/Valdecy/pyAutoSummarizer
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -35,12 +35,12 @@
 - Example 02: LexRank            ([ Colab Demo ](https://colab.research.google.com/drive/1gT9fV7hAE4mvwAHbfzolF6TN3TjGgJOF?usp=sharing#scrollTo=npuyBY596tJ5))
 - Example 03: LSA                ([ Colab Demo ](https://colab.research.google.com/drive/19fUslzp43_Owib9YDCb0Xfe9XZm1OKmB?usp=sharing#scrollTo=npuyBY596tJ5))
 - Example 04: KL-Sum             ([ Colab Demo ](https://colab.research.google.com/drive/19zHjE0nR1GcAWi4NQmaJh1gjpqm4sqjP?usp=sharing#scrollTo=npuyBY596tJ5))
 - Example 05: T5 (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1tyWu-19xA9QMrwl_kPcGJH0ZSS3r_rDZ?usp=sharing#scrollTo=npuyBY596tJ5))
 
 Abstractive Summarization. 
 - Example 01: chatGPT (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1ipl6ZnyumJeuxsYelcmZEdsXDMIuM5WG?usp=sharing#scrollTo=npuyBY596tJ5)) Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
-- Example 02: Pegasus (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1RWIEm9WoZBPYA_p4A1LqKnFPaXhNsQcM?usp=sharing))
+- Example 02: PEGASUS (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1RWIEm9WoZBPYA_p4A1LqKnFPaXhNsQcM?usp=sharing))
 
 ## Others
 
 - [pyBibX](https://github.com/Valdecy/pyBibX) - A Bibliometric and Scientometric Python Library Powered with Artificial Intelligence Tools
```

### Comparing `pyAutoSummarizer-1.0.4/README.md` & `pyAutoSummarizer-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,12 +24,12 @@
 - Example 02: LexRank            ([ Colab Demo ](https://colab.research.google.com/drive/1gT9fV7hAE4mvwAHbfzolF6TN3TjGgJOF?usp=sharing#scrollTo=npuyBY596tJ5))
 - Example 03: LSA                ([ Colab Demo ](https://colab.research.google.com/drive/19fUslzp43_Owib9YDCb0Xfe9XZm1OKmB?usp=sharing#scrollTo=npuyBY596tJ5))
 - Example 04: KL-Sum             ([ Colab Demo ](https://colab.research.google.com/drive/19zHjE0nR1GcAWi4NQmaJh1gjpqm4sqjP?usp=sharing#scrollTo=npuyBY596tJ5))
 - Example 05: T5 (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1tyWu-19xA9QMrwl_kPcGJH0ZSS3r_rDZ?usp=sharing#scrollTo=npuyBY596tJ5))
 
 Abstractive Summarization. 
 - Example 01: chatGPT (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1ipl6ZnyumJeuxsYelcmZEdsXDMIuM5WG?usp=sharing#scrollTo=npuyBY596tJ5)) Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
-- Example 02: Pegasus (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1RWIEm9WoZBPYA_p4A1LqKnFPaXhNsQcM?usp=sharing))
+- Example 02: PEGASUS (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1RWIEm9WoZBPYA_p4A1LqKnFPaXhNsQcM?usp=sharing))
 
 ## Others
 
 - [pyBibX](https://github.com/Valdecy/pyBibX) - A Bibliometric and Scientometric Python Library Powered with Artificial Intelligence Tools
```

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/psr.py` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/psr.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 # Citation: 
 # PEREIRA, V. (2023). Project: pyAutoSummarizer, GitHub repository: <https://github.com/Valdecy/pyAutoSummarizer>
 
 ############################################################################
 
 # Required Libraries
+import chardet
 import numpy as np
 import openai 
 import re 
 import regex
 import unicodedata 
 
 try:
@@ -41,35 +42,37 @@
         self.p_rc     = rmv_special_chars 
         self.p_rn     = rmv_numbers
         self.p_rw     = rmv_custom_words
         self.p_vb     = verbose
         self.limit_w  = n_words
         self.limit_c  = n_chars
         self.full_txt = text
+        self.sw_full  = []
         pattern       = r'(?<!\b(?:Mr|Mrs|Ms|Dr|Prof|St|Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec|[A-Z]|[A-Z][a-z]|[a-z]))[.!?]\s+' # r'(?<=[.!?])\s+'
         if (self.limit_w <= 0 and self.limit_c <= 0):
             self.sentences = regex.split(pattern, text.strip()) 
             self.original  = regex.split(pattern, text.strip()) 
         else:
             self.sentences = self.split_sentences(words_per_sentence = self.limit_w, chars_per_sentence = self.limit_c)
             self.original  = self.split_sentences(words_per_sentence = self.limit_w, chars_per_sentence = self.limit_c)
-        self.corpus = self.clear_text(self.sentences, stop_words = self.p_sw, lowercase = self.p_lc, rmv_accents = self.p_ra, rmv_special_chars = self.p_rc, rmv_numbers = self.p_rn, rmv_custom_words = self.p_rw)
+        self.corpus    = self.clear_text(self.sentences, stop_words = self.p_sw, lowercase = self.p_lc, rmv_accents = self.p_ra, rmv_special_chars = self.p_rc, rmv_numbers = self.p_rn, rmv_custom_words = self.p_rw)
         self.txt       = '. '.join(self.corpus)
         self.sentences = regex.split(pattern, self.txt)
-        for i in range(len(self.sentences)-1, -1, -1):
-            self.sentences[i] = self.sentences[i].replace('.', '')
-            if (self.sentences[i] == ''):
+        for i in range(len(self.corpus)-1, -1, -1):
+            self.corpus[i] = self.corpus[i].replace('.', '')
+            if (self.corpus[i] == ''):
+                del self.corpus[i]
                 del self.sentences[i]
                 del self.original[i]
         self.tokens        = []
         self.w_freq        = {}
         self.w_dist        = {}
         self.loaded_models = {}
-        for i in range(0, len(self.sentences)):
-            self.tokens.append(re.findall(r'\b\w+\b', self.sentences[i].lower()))
+        for i in range(0, len(self.corpus)):
+            self.tokens.append(re.findall(r'\b\w+\b', self.corpus[i].lower()))
         self.vocabulary = set([token for s in self.tokens for token in s])
         self.all_tokens = [item for sublist in self.tokens for item in sublist]
         for token in self.vocabulary:
             self.w_freq[token] = self.all_tokens.count(token)
         total_w        = sum(self.w_freq.values()) 
         for token in self.vocabulary:
             self.w_dist[token] = self.w_freq[token]/total_w
@@ -114,15 +117,15 @@
             print(sentence)
             self.summ.append(sentence)
         self.summ = ' '.join(self.summ)
         return self.summ
     
     # Function: Text Pre-Processing
     def clear_text(self, corpus, stop_words = ['en'], lowercase = True, rmv_accents = True, rmv_special_chars = True, rmv_numbers = True, rmv_custom_words = [], verbose = False):
-        sw_full = []
+        self.sw_full = []
         # Lower Case
         if (lowercase == True):
             if (verbose == True):
                 print('Lower Case: Working...')
             corpus = [str(x).lower().replace("’","'") for x in  corpus]
             if (verbose == True):
                 print('Lower Case: Done!')
@@ -133,76 +136,81 @@
             corpus = [re.sub(r"[^a-zA-Z0-9']+", ' ', i) for i in corpus]
             if (verbose == True):
                 print('Removing Special Characters: Done!')
         # Remove Stopwords
         if (len(stop_words) > 0):
             for sw_ in stop_words: 
                 if   (sw_ == 'ar' or sw_ == 'ara' or 'arabic'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Arabic.txt', encoding = 'utf8')
+                    name = 'Stopwords-Arabic.txt'
                 elif (sw_ == 'bn' or sw_ == 'ben' or 'bengali'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Bengali.txt', encoding = 'utf8')
+                    name = 'Stopwords-Bengali.txt'
                 elif (sw_ == 'bg' or sw_ == 'bul' or 'bulgarian'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Bulgarian.txt', encoding = 'utf8')
+                    name = 'Stopwords-Bulgarian.txt'
                 elif (sw_ == 'zh' or sw_ == 'chi' or 'chinese'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Chinese.txt', encoding = 'utf8')
+                    name = 'Stopwords-Chinese.txt'
                 elif (sw_ == 'cs' or sw_ == 'cze' or sw_ == 'ces' or 'czech'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Czech.txt', encoding = 'utf8')
+                    name = 'Stopwords-Czech.txt'
                 elif (sw_ == 'en' or sw_ == 'eng' or 'english'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-English.txt', encoding = 'utf8')
+                    name = 'Stopwords-English.txt'
                 elif (sw_ == 'fi' or sw_ == 'fin' or 'finnish'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Finnish.txt', encoding = 'utf8')
+                    name = 'Stopwords-Finnish.txt'
                 elif (sw_ == 'fr' or sw_ == 'fre' or sw_ == 'fra' or 'french'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-French.txt', encoding = 'utf8')
+                    name = 'Stopwords-French.txt'
                 elif (sw_ == 'de' or sw_ == 'ger' or sw_ == 'deu' or 'german'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-German.txt', encoding = 'utf8')
+                    name = 'Stopwords-German.txt'
                 elif (sw_ == 'el' or sw_ == 'gre' or 'greek'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Greek.txt', encoding = 'utf8')
+                    name = 'Stopwords-Greek.txt'
                 elif (sw_ == 'he' or sw_ == 'heb' or 'hebrew'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Hebrew.txt', encoding = 'utf8')
+                    name = 'Stopwords-Hebrew.txt'
                 elif (sw_ == 'hi' or sw_ == 'hin' or 'hind'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Hind.txt', encoding = 'utf8')
+                    name = 'Stopwords-Hind.txt'
                 elif (sw_ == 'hu' or sw_ == 'hun' or 'hungarian'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Hungarian.txt', encoding = 'utf8')
+                    name = 'Stopwords-Hungarian.txt'
                 elif (sw_ == 'it' or sw_ == 'ita' or 'italian'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Italian.txt', encoding = 'utf8')
+                    name = 'Stopwords-Italian.txt'
                 elif (sw_ == 'ja' or sw_ == 'jpn' or 'japanese'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Japanese.txt', encoding = 'utf8')
+                    name = 'Stopwords-Japanese.txt'
                 elif (sw_ == 'ko' or sw_ == 'kor' or 'korean'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Korean.txt', encoding = 'utf8')
+                    name = 'Stopwords-Korean.txt'
                 elif (sw_ == 'mr' or sw_ == 'mar' or 'marathi'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Marathi.txt', encoding = 'utf8')
+                    name = 'Stopwords-Marathi.txt'
                 elif (sw_ == 'fa' or sw_ == 'per' or sw_ == 'fas' or 'persian'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Persian.txt', encoding = 'utf8')
+                    name = 'Stopwords-Persian.txt'
                 elif (sw_ == 'pl' or sw_ == 'pol' or 'polish'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Polish.txt', encoding = 'utf8')
+                    name = 'Stopwords-Polish.txt'
                 elif (sw_ == 'pt-br' or sw_ == 'por-br' or 'portuguese-br'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Portuguese-br.txt', encoding = 'utf8')
+                    name = 'Stopwords-Portuguese-br.txt'
                 elif (sw_ == 'ro' or sw_ == 'rum' or sw_ == 'ron' or 'romanian'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Romanian.txt', encoding = 'utf8')
+                    name = 'Stopwords-Romanian.txt'
                 elif (sw_ == 'ru' or sw_ == 'rus' or 'russian'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Russian.txt', encoding = 'utf8')
+                    name = 'Stopwords-Russian.txt'
                 elif (sw_ == 'sk' or sw_ == 'slo' or 'slovak'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Slovak.txt', encoding = 'utf8')
+                    name = 'Stopwords-Slovak.txt'
                 elif (sw_ == 'es' or sw_ == 'spa' or 'spanish'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Spanish.txt', encoding = 'utf8')
+                    name = 'Stopwords-Spanish.txt'
                 elif (sw_ == 'sv' or sw_ == 'swe' or 'swedish'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Swedish.txt', encoding = 'utf8')
+                    name = 'Stopwords-Swedish.txt'
                 elif (sw_ == 'th' or sw_ == 'tha' or 'thai'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Thai.txt', encoding = 'utf8')
+                    name = 'Stopwords-Thai.txt'
                 elif (sw_ == 'uk' or sw_ == 'ukr' or 'ukrainian'):
-                    f_file = pkg_resources.open_text(stws, 'Stopwords-Ukrainian.txt', encoding = 'utf8')
-                f_lines = f_file.read()
-                sw      = f_lines.split('\n')
-                sw      = list(filter(None, sw))
-                sw_full.extend(sw)
+                    name = 'Stopwords-Ukrainian.txt'
+                with pkg_resources.open_binary(stws, name) as file:
+                    raw_data = file.read()
+                result   = chardet.detect(raw_data)
+                encoding = result['encoding']
+                with pkg_resources.open_text(stws, name, encoding = encoding) as file:
+                    content = file.read()
+                content = [line.rstrip('\r') for line in content]
+                sw      = list(filter(None, content))
+                self.sw_full.extend(sw)
             if (verbose == True):
                 print('Removing Stopwords: Working...')
             for i in range(0, len(corpus)):
                text      = corpus[i].split()
-               text      = [x.replace(' ', '') for x in text if x.replace(' ', '') not in sw_full]
+               text      = [x.replace(' ', '') for x in text if x.replace(' ', '') not in self.sw_full]
                corpus[i] = ' '.join(text) 
                if (verbose == True):
                    print('Removing Stopwords: ' + str(i + 1) +  ' of ' + str(len(corpus)) )
             if (verbose == True):
                 print('Removing Stopwords: Done!')
         # Remove Custom Words
         if (len(rmv_custom_words) > 0):
@@ -267,36 +275,36 @@
         return V_
     
     ##############################################################################
     
     # Function: TF
     def tf_matrix(self):
         vectorizer = CountVectorizer()
-        vectorizer.fit(self.sentences)
-        tf_matrix  = vectorizer.transform(self.sentences)
+        vectorizer.fit(self.corpus)
+        tf_matrix  = vectorizer.transform(self.corpus)
         tf_m       = tf_matrix.toarray()
         tf_m       = tf_m/np.sum(tf_m, axis = 1).reshape(-1, 1)
         #vectorizer.vocabulary_
         #vectorizer.get_feature_names()
         return tf_m
     
     # Function: IDF
     def idf_matrix(self):
         vectorizer = TfidfVectorizer(use_idf = True)
-        vectorizer.fit(self.sentences)
-        idf_m      = vectorizer.transform(self.sentences)
+        vectorizer.fit(self.corpus)
+        idf_m      = vectorizer.transform(self.corpus)
         idf_m      = vectorizer.idf_
         #vectorizer.vocabulary_
         return idf_m
     
     # Function: TF-IDF
     def tf_idf_matrix(self):
         vectorizer    = TfidfVectorizer()
-        vectorizer.fit(self.sentences)
-        tf_idf_matrix = vectorizer.transform(self.sentences)
+        vectorizer.fit(self.corpus)
+        tf_idf_matrix = vectorizer.transform(self.corpus)
         tf_idf_m      = tf_idf_matrix.toarray()
         #vectorizer.vocabulary_
         #vectorizer.get_feature_names()
         return tf_idf_m
 
     ##############################################################################
     
@@ -479,17 +487,15 @@
     
     # TextRank
     
     # Function: Sentence Embeddings
     def create_embeddings(self, model = 'all-MiniLM-L6-v2'):
         if (model not in self.loaded_models):
             self.loaded_models[model] = SentenceTransformer(model)
-        #model_ = SentenceTransformer(model)
-        #embds  = model_.encode(self.sentences)
-        embds = self.loaded_models[model].encode(self.sentences)
+        embds = self.loaded_models[model].encode(self.corpus)
         return embds
     
     # Function: TextRank
     def summ_text_rank(self, iteration = 1000, D = 0.85, model = 'all-MiniLM-L6-v2'):
         embeddings = self.create_embeddings(model = model)
         sim_matrix = cosine_similarity(embeddings)
         rank       = self.page_rank(sim_matrix, iteration = iteration, D = D)
@@ -524,15 +530,15 @@
     
     # KL Divergence  
     
     # Function: Candidate Summary Distribution
     def cs_distribution(self, idx, vocab):
         tokens = []
         for i in idx:
-            tokens.append(self.sentences[i].split())
+            tokens.append(self.corpus[i].split())
         tokens = [word for sentence in tokens for word in sentence]
         q      = [tokens.count(word)/len(tokens) if word in tokens else 0 for word in vocab]
         return q 
 
     # Function: KL Divergence
     def KL_divergence(self, p, q):
         pq = [(p_i, q_i) for p_i, q_i in zip(p, q) if p_i > 0 and q_i > 0]
@@ -542,22 +548,22 @@
     
     # Function: KL
     def summ_ext_KL(self, n = 3):  
         best_summary = None
         min_KL       = float('inf')
         vocab        = sorted(self.vocabulary)
         p            = [self.w_dist[word] for word in vocab]
-        for candidate_summaries in combinations(range(0, len(self.sentences)), n):
+        for candidate_summaries in combinations(range(0, len(self.corpus)), n):
             idx = [i for i in candidate_summaries]
             q   = self.cs_distribution(idx, vocab)
             KL  = self.KL_divergence(p, q)
             if (KL < min_KL):
                 min_KL       = KL
                 best_summary = [item for item in idx]
-        rank     = [1 if x in best_summary else 0 for x in range(0, len(self.sentences))]
+        rank     = [1 if x in best_summary else 0 for x in range(0, len(self.corpus))]
         rank_sum = sum(rank)
         for i in range(0, len(rank)):
             if (rank[i] == 1):
                 rank[i]  = rank_sum
                 rank_sum = rank_sum - 1
         rank = np.array(rank)
         return rank
@@ -593,18 +599,18 @@
         prompt         = query + ':\n\n' + f'{self.full_txt}\n'
         summary        = query_chatgpt(prompt)
         self.summ      = summary 
         print(summary)
         return summary 
     
     # Function: PEGASUS
-    def summ_abst_pegasus(self, text, model_name = 'google/pegasus-xsum', min_L = 100, max_L = 150):
+    def summ_abst_pegasus(self, model_name = 'google/pegasus-xsum', min_L = 100, max_L = 150):
         tokenizer = PegasusTokenizer.from_pretrained(model_name)
         pegasus   = PegasusForConditionalGeneration.from_pretrained(model_name)
-        tokens    = tokenizer.encode('summarize: ' + text, return_tensors = 'pt', max_length = 1024, truncation = True)
+        tokens    = tokenizer.encode('summarize: ' + self.full_txt, return_tensors = 'pt', max_length = 1024, truncation = True)
         summary   = pegasus.generate(tokens, min_length = min_L, max_length = max_L, length_penalty = 2.0, num_beams = 4, early_stopping = True)
         summary   = tokenizer.decode(summary[0], skip_special_tokens = True)
         self.summ = summary 
         print(summary)
         return summary
 
     ##############################################################################
```

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Arabic.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Arabic.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Bengali.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Bengali.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Bulgarian.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Bulgarian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Chinese.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Chinese.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Czech.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Czech.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-English.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-English.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Finnish.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Finnish.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-French.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-French.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-German.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-German.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Greek.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Greek.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Hebrew.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Hebrew.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Hindi.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Hindi.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Hungarian.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Hungarian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Italian.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Italian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Japanese.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Japanese.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Korean.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Korean.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Marathi.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Marathi.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Persian.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Persian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Polish.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Polish.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Portuguese-br.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Portuguese-br.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Romanian.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Romanian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Russian.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Russian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Slovak.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Slovak.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Spanish.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Spanish.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Swedish.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Swedish.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Thai.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Thai.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer/base/stws/Stopwords-Ukrainian.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer/base/stws/Stopwords-Ukrainian.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer.egg-info/PKG-INFO` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAutoSummarizer
-Version: 1.0.4
+Version: 1.0.7
 Summary: An Extractive and Abstractive Summarization Library Powered with Artificial Intelligence
 Home-page: https://github.com/Valdecy/pyAutoSummarizer
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -35,12 +35,12 @@
 - Example 02: LexRank            ([ Colab Demo ](https://colab.research.google.com/drive/1gT9fV7hAE4mvwAHbfzolF6TN3TjGgJOF?usp=sharing#scrollTo=npuyBY596tJ5))
 - Example 03: LSA                ([ Colab Demo ](https://colab.research.google.com/drive/19fUslzp43_Owib9YDCb0Xfe9XZm1OKmB?usp=sharing#scrollTo=npuyBY596tJ5))
 - Example 04: KL-Sum             ([ Colab Demo ](https://colab.research.google.com/drive/19zHjE0nR1GcAWi4NQmaJh1gjpqm4sqjP?usp=sharing#scrollTo=npuyBY596tJ5))
 - Example 05: T5 (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1tyWu-19xA9QMrwl_kPcGJH0ZSS3r_rDZ?usp=sharing#scrollTo=npuyBY596tJ5))
 
 Abstractive Summarization. 
 - Example 01: chatGPT (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1ipl6ZnyumJeuxsYelcmZEdsXDMIuM5WG?usp=sharing#scrollTo=npuyBY596tJ5)) Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
-- Example 02: Pegasus (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1RWIEm9WoZBPYA_p4A1LqKnFPaXhNsQcM?usp=sharing))
+- Example 02: PEGASUS (Deep Learning) ([ Colab Demo ](https://colab.research.google.com/drive/1RWIEm9WoZBPYA_p4A1LqKnFPaXhNsQcM?usp=sharing))
 
 ## Others
 
 - [pyBibX](https://github.com/Valdecy/pyBibX) - A Bibliometric and Scientometric Python Library Powered with Artificial Intelligence Tools
```

### Comparing `pyAutoSummarizer-1.0.4/pyAutoSummarizer.egg-info/SOURCES.txt` & `pyAutoSummarizer-1.0.7/pyAutoSummarizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyAutoSummarizer-1.0.4/setup.py` & `pyAutoSummarizer-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyAutoSummarizer',
-    version='1.0.4',
+    version='1.0.7',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyAutoSummarizer',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
+        'chardet',
         'numpy',
         'regex',
         'scikit-learn',
         'sentence_transformers',
         'openai',
         'transformers'
     ],
```

