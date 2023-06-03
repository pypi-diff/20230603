# Comparing `tmp/NlpToolkit-InformationRetrieval-1.0.5.tar.gz` & `tmp/NlpToolkit-InformationRetrieval-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NlpToolkit-InformationRetrieval-1.0.5.tar", last modified: Wed Dec  7 12:13:23 2022, max compression
+gzip compressed data, was "dist/NlpToolkit-InformationRetrieval-1.0.6.tar", last modified: Sat Jun  3 12:04:20 2023, max compression
```

## Comparing `NlpToolkit-InformationRetrieval-1.0.5.tar` & `NlpToolkit-InformationRetrieval-1.0.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2022-12-07 12:13:23.000000 NlpToolkit-InformationRetrieval-1.0.5/
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2022-12-07 12:13:23.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2022-12-07 12:13:23.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/
--rw-r--r--   0 olcay      (501) staff       (20)     3646 2022-12-06 17:10:00.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/AbstractCollection.py
--rw-r--r--   0 olcay      (501) staff       (20)     4467 2022-12-05 19:31:23.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/DiskCollection.py
--rw-r--r--   0 olcay      (501) staff       (20)     2510 2022-11-02 12:42:15.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/Document.py
--rw-r--r--   0 olcay      (501) staff       (20)     1811 2022-10-19 18:20:46.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/DocumentText.py
--rw-r--r--   0 olcay      (501) staff       (20)      102 2022-10-19 18:17:50.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/DocumentType.py
--rw-r--r--   0 olcay      (501) staff       (20)      131 2022-07-31 12:59:34.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/DocumentWeighting.py
--rw-r--r--   0 olcay      (501) staff       (20)      111 2022-07-31 13:00:26.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/IndexType.py
--rw-r--r--   0 olcay      (501) staff       (20)    10147 2022-12-06 17:10:00.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/LargeCollection.py
--rw-r--r--   0 olcay      (501) staff       (20)     4405 2022-12-06 17:10:00.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/MediumCollection.py
--rw-r--r--   0 olcay      (501) staff       (20)     9651 2022-12-07 11:22:42.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/MemoryCollection.py
--rw-r--r--   0 olcay      (501) staff       (20)     3759 2022-12-06 16:56:11.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/Parameter.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2022-07-31 12:57:07.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/__init__.py
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2022-12-07 12:13:23.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/
--rw-r--r--   0 olcay      (501) staff       (20)     3457 2022-12-06 06:01:47.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/CategoryNode.py
--rw-r--r--   0 olcay      (501) staff       (20)     1506 2022-12-06 06:01:47.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/CategoryTree.py
--rw-r--r--   0 olcay      (501) staff       (20)     1879 2022-10-01 07:21:17.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/IncidenceMatrix.py
--rw-r--r--   0 olcay      (501) staff       (20)     3945 2022-10-01 07:21:17.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/InvertedIndex.py
--rw-r--r--   0 olcay      (501) staff       (20)      353 2022-08-04 16:41:54.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/NGramIndex.py
--rw-r--r--   0 olcay      (501) staff       (20)     8035 2022-11-02 12:44:26.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/PositionalIndex.py
--rw-r--r--   0 olcay      (501) staff       (20)      748 2022-10-01 07:21:18.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/PositionalPosting.py
--rw-r--r--   0 olcay      (501) staff       (20)     4205 2022-10-01 07:21:18.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/PositionalPostingList.py
--rw-r--r--   0 olcay      (501) staff       (20)      141 2022-10-01 07:21:17.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/Posting.py
--rw-r--r--   0 olcay      (501) staff       (20)     2246 2022-10-01 07:32:08.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/PostingList.py
--rw-r--r--   0 olcay      (501) staff       (20)      659 2022-10-01 07:32:08.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/PostingSkip.py
--rw-r--r--   0 olcay      (501) staff       (20)     2212 2022-10-01 07:32:08.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/PostingSkipList.py
--rw-r--r--   0 olcay      (501) staff       (20)      248 2022-10-01 07:32:08.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/Term.py
--rw-r--r--   0 olcay      (501) staff       (20)     4068 2022-10-01 07:32:08.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/TermDictionary.py
--rw-r--r--   0 olcay      (501) staff       (20)     2754 2022-10-01 07:32:08.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/TermOccurrence.py
--rw-r--r--   0 olcay      (501) staff       (20)       92 2022-07-31 13:01:19.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/TermType.py
--rw-r--r--   0 olcay      (501) staff       (20)      120 2022-07-31 13:02:23.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/TermWeighting.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2022-07-31 12:57:13.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/__init__.py
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2022-12-07 12:13:23.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Query/
--rw-r--r--   0 olcay      (501) staff       (20)      110 2022-12-06 05:59:11.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Query/CategoryDeterminationType.py
--rw-r--r--   0 olcay      (501) staff       (20)       96 2022-12-06 06:05:02.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Query/FocusType.py
--rw-r--r--   0 olcay      (501) staff       (20)     1113 2022-12-06 16:30:44.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Query/Query.py
--rw-r--r--   0 olcay      (501) staff       (20)     1574 2022-12-06 06:23:20.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Query/QueryResult.py
--rw-r--r--   0 olcay      (501) staff       (20)      368 2022-10-08 17:38:15.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Query/QueryResultItem.py
--rw-r--r--   0 olcay      (501) staff       (20)      145 2022-12-06 16:35:51.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Query/RetrievalType.py
--rw-r--r--   0 olcay      (501) staff       (20)     2265 2022-12-06 06:09:12.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Query/SearchParameter.py
--rw-r--r--   0 olcay      (501) staff       (20)     2616 2022-08-02 07:28:16.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Query/VectorSpaceModel.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2022-07-31 12:57:19.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Query/__init__.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2022-07-31 11:42:27.000000 NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/__init__.py
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2022-12-07 12:13:23.000000 NlpToolkit-InformationRetrieval-1.0.5/NlpToolkit_InformationRetrieval.egg-info/
--rw-r--r--   0 olcay      (501) staff       (20)     2524 2022-12-07 12:13:23.000000 NlpToolkit-InformationRetrieval-1.0.5/NlpToolkit_InformationRetrieval.egg-info/PKG-INFO
--rw-r--r--   0 olcay      (501) staff       (20)     2061 2022-12-07 12:13:23.000000 NlpToolkit-InformationRetrieval-1.0.5/NlpToolkit_InformationRetrieval.egg-info/SOURCES.txt
--rw-r--r--   0 olcay      (501) staff       (20)        1 2022-12-07 12:13:23.000000 NlpToolkit-InformationRetrieval-1.0.5/NlpToolkit_InformationRetrieval.egg-info/dependency_links.txt
--rw-r--r--   0 olcay      (501) staff       (20)       39 2022-12-07 12:13:23.000000 NlpToolkit-InformationRetrieval-1.0.5/NlpToolkit_InformationRetrieval.egg-info/requires.txt
--rw-r--r--   0 olcay      (501) staff       (20)       21 2022-12-07 12:13:23.000000 NlpToolkit-InformationRetrieval-1.0.5/NlpToolkit_InformationRetrieval.egg-info/top_level.txt
--rw-r--r--   0 olcay      (501) staff       (20)     2524 2022-12-07 12:13:23.000000 NlpToolkit-InformationRetrieval-1.0.5/PKG-INFO
--rw-r--r--   0 olcay      (501) staff       (20)     2212 2022-10-11 12:23:03.000000 NlpToolkit-InformationRetrieval-1.0.5/README.md
--rw-r--r--   0 olcay      (501) staff       (20)       38 2022-12-07 12:13:23.000000 NlpToolkit-InformationRetrieval-1.0.5/setup.cfg
--rw-r--r--   0 olcay      (501) staff       (20)      785 2022-12-07 12:13:19.000000 NlpToolkit-InformationRetrieval-1.0.5/setup.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2023-06-03 12:04:20.000000 NlpToolkit-InformationRetrieval-1.0.6/
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2023-06-03 12:04:20.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2023-06-03 12:04:20.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/
+-rw-r--r--   0 olcay      (501) staff       (20)     3724 2023-04-04 08:50:51.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/AbstractCollection.py
+-rw-r--r--   0 olcay      (501) staff       (20)     4467 2022-12-05 19:31:23.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/DiskCollection.py
+-rw-r--r--   0 olcay      (501) staff       (20)     2510 2022-11-02 12:42:15.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/Document.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1811 2022-10-19 18:20:46.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/DocumentText.py
+-rw-r--r--   0 olcay      (501) staff       (20)      102 2022-10-19 18:17:50.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/DocumentType.py
+-rw-r--r--   0 olcay      (501) staff       (20)      131 2022-07-31 12:59:34.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/DocumentWeighting.py
+-rw-r--r--   0 olcay      (501) staff       (20)      111 2022-07-31 13:00:26.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/IndexType.py
+-rw-r--r--   0 olcay      (501) staff       (20)    10147 2022-12-06 17:10:00.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/LargeCollection.py
+-rw-r--r--   0 olcay      (501) staff       (20)     4405 2022-12-06 17:10:00.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/MediumCollection.py
+-rw-r--r--   0 olcay      (501) staff       (20)    10987 2023-06-03 11:14:03.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/MemoryCollection.py
+-rw-r--r--   0 olcay      (501) staff       (20)     3759 2022-12-06 16:56:11.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/Parameter.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2022-07-31 12:57:07.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/__init__.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2023-06-03 12:04:20.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/
+-rw-r--r--   0 olcay      (501) staff       (20)     3457 2022-12-06 06:01:47.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/CategoryNode.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1506 2022-12-06 06:01:47.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/CategoryTree.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1879 2022-10-01 07:21:17.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/IncidenceMatrix.py
+-rw-r--r--   0 olcay      (501) staff       (20)     4472 2022-12-17 18:13:18.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/InvertedIndex.py
+-rw-r--r--   0 olcay      (501) staff       (20)      353 2022-08-04 16:41:54.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/NGramIndex.py
+-rw-r--r--   0 olcay      (501) staff       (20)     8035 2022-11-02 12:44:26.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/PositionalIndex.py
+-rw-r--r--   0 olcay      (501) staff       (20)      748 2022-10-01 07:21:18.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/PositionalPosting.py
+-rw-r--r--   0 olcay      (501) staff       (20)     4205 2022-10-01 07:21:18.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/PositionalPostingList.py
+-rw-r--r--   0 olcay      (501) staff       (20)      141 2022-10-01 07:21:17.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/Posting.py
+-rw-r--r--   0 olcay      (501) staff       (20)     2246 2022-10-01 07:32:08.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/PostingList.py
+-rw-r--r--   0 olcay      (501) staff       (20)      659 2022-10-01 07:32:08.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/PostingSkip.py
+-rw-r--r--   0 olcay      (501) staff       (20)     2212 2022-10-01 07:32:08.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/PostingSkipList.py
+-rw-r--r--   0 olcay      (501) staff       (20)      248 2022-10-01 07:32:08.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/Term.py
+-rw-r--r--   0 olcay      (501) staff       (20)     4068 2022-10-01 07:32:08.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/TermDictionary.py
+-rw-r--r--   0 olcay      (501) staff       (20)     2754 2022-10-01 07:32:08.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/TermOccurrence.py
+-rw-r--r--   0 olcay      (501) staff       (20)       92 2022-07-31 13:01:19.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/TermType.py
+-rw-r--r--   0 olcay      (501) staff       (20)      120 2022-07-31 13:02:23.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/TermWeighting.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2022-07-31 12:57:13.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/__init__.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2023-06-03 12:04:20.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Query/
+-rw-r--r--   0 olcay      (501) staff       (20)      110 2022-12-06 05:59:11.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Query/CategoryDeterminationType.py
+-rw-r--r--   0 olcay      (501) staff       (20)       96 2022-12-06 06:05:02.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Query/FocusType.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1266 2023-06-03 11:04:11.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Query/Query.py
+-rw-r--r--   0 olcay      (501) staff       (20)     3105 2023-06-03 11:03:43.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Query/QueryResult.py
+-rw-r--r--   0 olcay      (501) staff       (20)      368 2022-10-08 17:38:15.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Query/QueryResultItem.py
+-rw-r--r--   0 olcay      (501) staff       (20)      122 2023-06-03 10:59:28.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Query/RetrievalType.py
+-rw-r--r--   0 olcay      (501) staff       (20)     2532 2023-06-03 10:58:58.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Query/SearchParameter.py
+-rw-r--r--   0 olcay      (501) staff       (20)     2616 2022-08-02 07:28:16.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Query/VectorSpaceModel.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2022-07-31 12:57:19.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Query/__init__.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2022-07-31 11:42:27.000000 NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/__init__.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2023-06-03 12:04:20.000000 NlpToolkit-InformationRetrieval-1.0.6/NlpToolkit_InformationRetrieval.egg-info/
+-rw-r--r--   0 olcay      (501) staff       (20)     2524 2023-06-03 12:04:20.000000 NlpToolkit-InformationRetrieval-1.0.6/NlpToolkit_InformationRetrieval.egg-info/PKG-INFO
+-rw-r--r--   0 olcay      (501) staff       (20)     2061 2023-06-03 12:04:20.000000 NlpToolkit-InformationRetrieval-1.0.6/NlpToolkit_InformationRetrieval.egg-info/SOURCES.txt
+-rw-r--r--   0 olcay      (501) staff       (20)        1 2023-06-03 12:04:20.000000 NlpToolkit-InformationRetrieval-1.0.6/NlpToolkit_InformationRetrieval.egg-info/dependency_links.txt
+-rw-r--r--   0 olcay      (501) staff       (20)       39 2023-06-03 12:04:20.000000 NlpToolkit-InformationRetrieval-1.0.6/NlpToolkit_InformationRetrieval.egg-info/requires.txt
+-rw-r--r--   0 olcay      (501) staff       (20)       21 2023-06-03 12:04:20.000000 NlpToolkit-InformationRetrieval-1.0.6/NlpToolkit_InformationRetrieval.egg-info/top_level.txt
+-rw-r--r--   0 olcay      (501) staff       (20)     2524 2023-06-03 12:04:20.000000 NlpToolkit-InformationRetrieval-1.0.6/PKG-INFO
+-rw-r--r--   0 olcay      (501) staff       (20)     2212 2022-10-11 12:23:03.000000 NlpToolkit-InformationRetrieval-1.0.6/README.md
+-rw-r--r--   0 olcay      (501) staff       (20)       38 2023-06-03 12:04:20.000000 NlpToolkit-InformationRetrieval-1.0.6/setup.cfg
+-rw-r--r--   0 olcay      (501) staff       (20)      785 2023-06-03 12:04:12.000000 NlpToolkit-InformationRetrieval-1.0.6/setup.py
```

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/AbstractCollection.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/AbstractCollection.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,16 +59,18 @@
 
     def loadCategories(self):
         self.category_tree = CategoryTree(self.name)
         input_file = open(self.name + "-categories.txt", mode="r", encoding="utf-8")
         line = input_file.readline().strip()
         while line != "":
             items = line.split("\t")
-            doc_id = int(items[0])
-            self.documents[doc_id].setCategory(self.category_tree, items[1])
+            if len(items) > 0:
+                doc_id = int(items[0])
+                if len(items) > 1:
+                    self.documents[doc_id].setCategory(self.category_tree, items[1])
             line = input_file.readline().strip()
         input_file.close()
 
     def loadAttributeList(self):
         self.attribute_list = set()
         input_file = open(self.name + "-attributelist.txt", mode="r", encoding="utf-8")
         line = input_file.readline().strip()
```

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/DiskCollection.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/DiskCollection.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/Document.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/Document.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/DocumentText.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/DocumentText.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/LargeCollection.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/LargeCollection.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/MediumCollection.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/MediumCollection.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/MemoryCollection.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/MemoryCollection.py`

 * *Files 17% similar despite different names*

```diff
@@ -107,39 +107,48 @@
         for doc in self.documents:
             document_text = doc.loadDocument()
             doc_terms = document_text.constructTermList(doc.getDocId(), termType)
             terms.extend(doc_terms)
         terms.sort(key=cmp_to_key(TermOccurrence.termOccurrenceComparator))
         return terms
 
-    def attributeSearch(self, query: Query) -> QueryResult:
+    def attributeSearch(self, query: Query, parameter: SearchParameter) -> QueryResult:
         term_attributes = Query()
         phrase_attributes = Query()
         term_result = QueryResult()
         phrase_result = QueryResult()
-        query.filterAttributes(self.attribute_list, term_attributes, phrase_attributes)
+        filtered_query = query.filterAttributes(self.attribute_list, term_attributes, phrase_attributes)
         if term_attributes.size() > 0:
             term_result = self.inverted_index.search(term_attributes, self.dictionary)
         if phrase_attributes.size() > 0:
             phrase_result = self.phrase_index.search(phrase_attributes, self.phrase_dictionary)
         if term_attributes.size() == 0:
-            return phrase_result
-        if phrase_attributes.size() == 0:
-            return term_result
-        return term_result.intersection(phrase_result)
+            attribute_result = phrase_result
+        elif phrase_attributes.size() == 0:
+            attribute_result = term_result
+        else:
+            attribute_result = term_result.intersectionFastSearch(phrase_result)
+        if filtered_query.size() == 0:
+            return attribute_result
+        else:
+            filtered_result = self.searchWithInvertedIndex(filtered_query, parameter)
+            if parameter.getRetrievalType() != RetrievalType.RANKED:
+                return filtered_result.intersectionFastSearch(attribute_result)
+            elif attribute_result.size() < 10:
+                return filtered_result.intersectionLinearSearch(attribute_result)
+            else:
+                return filtered_result.intersectionBinarySearch(attribute_result)
 
     def searchWithInvertedIndex(self,
                                 query: Query,
                                 searchParameter: SearchParameter) -> QueryResult:
         if searchParameter.getRetrievalType() == RetrievalType.BOOLEAN:
             return self.inverted_index.search(query, self.dictionary)
         elif searchParameter.getRetrievalType() == RetrievalType.POSITIONAL:
             return self.positional_index.positionalSearch(query, self.dictionary)
-        elif searchParameter.getRetrievalType() == RetrievalType.ATTRIBUTE:
-            return self.attributeSearch(query)
         elif searchParameter.getRetrievalType() == RetrievalType.RANKED:
             return self.positional_index.rankedSearch(query,
                                                         self.dictionary,
                                                         self.documents,
                                                         searchParameter.getTermWeighting(),
                                                         searchParameter.getDocumentWeighting(),
                                                         searchParameter.getDocumentsRetrieved())
@@ -155,23 +164,41 @@
             category_node = self.documents[query_result_item.getDocId()].getCategoryNode()
             for possible_ancestor in categories:
                 if category_node.isDescendant(possible_ancestor):
                     filtered_result.add(query_result_item.getDocId(), query_result_item.getScore())
                     break
         return filtered_result
 
+    def autoCompleteWord(self, prefix: str) -> [str]:
+        result = []
+        i = self.dictionary.getWordStartingWith(prefix)
+        while i < self.dictionary.size():
+            if self.dictionary.getWordWithIndex(i).getName().startswith(prefix):
+                result.append(self.dictionary.getWordWithIndex(i).getName())
+            else:
+                break
+            i = i + 1
+        self.inverted_index.autoCompleteWord(result, self.dictionary)
+        return result
+
     def searchCollection(self,
                          query: Query,
                          searchParameter: SearchParameter):
         if searchParameter.getFocusType() == FocusType.CATEGORY:
-            current_result = self.searchWithInvertedIndex(query, searchParameter)
+            if searchParameter.getSearchAttributes():
+                current_result = self.attributeSearch(query, searchParameter)
+            else:
+                current_result = self.searchWithInvertedIndex(query, searchParameter)
             categories = self.category_tree.getCategories(query,
                                                             self.dictionary,
                                                             searchParameter.getCategoryDeterminationType())
             return self.filterAccordingToCategories(current_result, categories)
         else:
             if self.__index_type == IndexType.INCIDENCE_MATRIX:
                 return self.incidence_matrix.search(query, self.dictionary)
             elif self.__index_type == IndexType.INVERTED_INDEX:
-                return self.searchWithInvertedIndex(query, searchParameter)
+                if searchParameter.getSearchAttributes():
+                    return self.attributeSearch(query, searchParameter)
+                else:
+                    return self.searchWithInvertedIndex(query, searchParameter)
             else:
                 return QueryResult()
```

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Document/Parameter.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Document/Parameter.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/CategoryNode.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/CategoryNode.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/CategoryTree.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/CategoryTree.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/IncidenceMatrix.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/IncidenceMatrix.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/InvertedIndex.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/InvertedIndex.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,26 @@
         if termId in self.__index:
             posting_list = self.__index[termId]
         else:
             posting_list = PostingList()
         posting_list.add(docId)
         self.__index[termId] = posting_list
 
+    def autoCompleteWord(self,
+                         wordList: [str],
+                         dictionary: TermDictionary):
+        counts = []
+        for word in wordList:
+            counts.append(self.__index[dictionary.getWordIndex(word)].size())
+        for i in range(len(wordList) - 1):
+            for j in range(i + 1, len(wordList)):
+                if counts[i] < counts[j]:
+                    counts[i], counts[j] = counts[j], counts[i]
+                    wordList[i], wordList[j] = wordList[j], wordList[i]
+
     def search(self,
                query: Query,
                dictionary: TermDictionary) -> QueryResult:
         query_terms = []
         for i in range(query.size()):
             term_index = dictionary.getWordIndex(query.getTerm(i).getName())
             if term_index != -1:
```

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/PositionalIndex.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/PositionalIndex.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/PositionalPosting.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/PositionalPosting.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/PositionalPostingList.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/PositionalPostingList.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/PostingList.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/PostingList.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/PostingSkip.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/PostingSkip.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/PostingSkipList.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/PostingSkipList.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/TermDictionary.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/TermDictionary.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Index/TermOccurrence.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Index/TermOccurrence.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Query/Query.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Query/Query.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,19 +18,23 @@
 
     def size(self) -> int:
         return len(self.__terms)
 
     def filterAttributes(self,
                          attributeList: set,
                          termAttributes: Query,
-                         phraseAttributes: Query):
+                         phraseAttributes: Query) -> Query:
         i = 0
+        filtered_query = Query()
         while i < self.size():
             if i < self.size() - 1:
                 pair = self.__terms[i].getName() + " " + self.__terms[i + 1].getName()
                 if pair in attributeList:
                     phraseAttributes.__terms.append(Word(pair))
                     i = i + 2
                     continue
             if self.__terms[i].getName() in attributeList:
                 termAttributes.__terms.append(self.__terms[i])
+            else:
+                filtered_query.__terms.append(self.__terms[i])
             i = i + 1
+        return filtered_query
```

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Query/QueryResult.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Query/QueryResult.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     def size(self) -> int:
         return len(self.__items)
 
     def getItems(self) -> [QueryResultItem]:
         return self.__items
 
-    def intersection(self, queryResult: QueryResult) -> QueryResult:
+    def intersectionFastSearch(self, queryResult: QueryResult) -> QueryResult:
         result = QueryResult()
         i = 0
         j = 0
         while i < self.size() and j < queryResult.size():
             item1 = self.__items[i]
             item2 = queryResult.__items[j]
             if item1.getDocId() == item2.getDocId():
@@ -34,19 +34,55 @@
             else:
                 if item1.getDocId() < item2.getDocId():
                     i = i + 1
                 else:
                     j = j + 1
         return result
 
+    def intersectionBinarySearch(self, queryResult: QueryResult) -> QueryResult:
+        result = QueryResult()
+        for searched_item in self.__items:
+            low = 0
+            high = queryResult.size() - 1
+            middle = (low + high) // 2
+            found = False
+            while low <= high:
+                if searched_item.getDocId() > queryResult.__items[middle].getDocId():
+                    low = middle + 1
+                elif searched_item.getDocId() < queryResult.__items[middle].getDocId():
+                    high = middle - 1
+                else:
+                    found = True
+                    break
+                middle = (low + high) // 2
+            if found:
+                result.add(searched_item.getDocId(), searched_item.getScore())
+        return result
+
+    def intersectionLinearSearch(self, queryResult: QueryResult) -> QueryResult:
+        result = QueryResult()
+        for searched_item in self.__items:
+            for item in queryResult.__items:
+                if searched_item.getDocId() == item.getDocId():
+                    result.add(searched_item.getDocId(), searched_item.getScore())
+        return result
+
     def getBest(self, K: int):
-        minHeap = MinHeap(2 * K, lambda x1, x2: -1 if x1.getScore() > x2.getScore() else (0 if x1.getScore() == x2.getScore() else 1))
-        for queryResultItem in self.__items:
-            minHeap.insert(queryResultItem)
+        minHeap = MinHeap(K, lambda x1, x2: 1 if x1.getScore() > x2.getScore() else (0 if x1.getScore() == x2.getScore() else -1))
+        i = 0
+        while i < K and i < len(self.__items):
+            minHeap.insert(self.__items[i])
+            i = i + 1
+        for i in range(K + 1, len(self.__items)):
+            top_item = minHeap.delete()
+            if isinstance(top_item, QueryResultItem) and top_item.getScore() > self.__items[i].getScore():
+                minHeap.insert(top_item)
+            else:
+                minHeap.insert(self.__items[i])
         self.__items.clear()
         i = 0
         while i < K and not minHeap.isEmpty():
-            self.__items.append(minHeap.delete())
+            self.__items.insert(0, minHeap.delete())
             i = i + 1
 
     def __repr__(self):
         return f"{self.__items}"
```

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Query/SearchParameter.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Query/SearchParameter.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 
     __category_determination_type: CategoryDeterminationType
     __focus_type: FocusType
     __retrieval_type: RetrievalType
     __document_weighting: DocumentWeighting
     __term_weighting: TermWeighting
     __documents_retrieved: int
+    __search_attributes: bool
 
     def __init__(self):
         self.__retrieval_type = RetrievalType.RANKED
         self.__document_weighting = DocumentWeighting.NO_IDF
         self.__term_weighting = TermWeighting.NATURAL
         self.__documents_retrieved = 1
         self.__category_determination_type = CategoryDeterminationType.KEYWORD
         self.__focus_type = FocusType.OVERALL
+        self.__search_attributes = False
 
     def getRetrievalType(self) -> RetrievalType:
         return self.__retrieval_type
 
     def getDocumentWeighting(self) -> DocumentWeighting:
         return self.__document_weighting
 
@@ -36,14 +38,17 @@
 
     def getCategoryDeterminationType(self) -> CategoryDeterminationType:
         return self.__category_determination_type
 
     def getFocusType(self) -> FocusType:
         return self.__focus_type
 
+    def getSearchAttributes(self) -> bool:
+        return self.__search_attributes
+
     def setRetrievalType(self, retrievalType: RetrievalType):
         self.__retrieval_type = retrievalType
 
     def setDocumentWeighting(self, documentWeighting: DocumentWeighting):
         self.__document_weighting = documentWeighting
 
     def setTermWeighting(self, termWeighting: TermWeighting):
@@ -53,7 +58,10 @@
         self.__documents_retrieved = documentsRetrieved
 
     def setCategoryDeterminationType(self, categoryDeterminationType: CategoryDeterminationType):
         self.__category_determination_type = categoryDeterminationType
 
     def setFocusType(self, focusType: FocusType):
         self.__focus_type = focusType
+
+    def setSearchAttributes(self, searchAttributes: bool):
+        self.__search_attributes = searchAttributes
```

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/InformationRetrieval/Query/VectorSpaceModel.py` & `NlpToolkit-InformationRetrieval-1.0.6/InformationRetrieval/Query/VectorSpaceModel.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/NlpToolkit_InformationRetrieval.egg-info/PKG-INFO` & `NlpToolkit-InformationRetrieval-1.0.6/NlpToolkit_InformationRetrieval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NlpToolkit-InformationRetrieval
-Version: 1.0.5
+Version: 1.0.6
 Summary: Information Retrieval Library
 Home-page: https://github.com/StarlangSoftware/InformationRetrieval-Py
 Author: olcaytaner
 Author-email: olcay.yildiz@ozyegin.edu.tr
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/NlpToolkit_InformationRetrieval.egg-info/SOURCES.txt` & `NlpToolkit-InformationRetrieval-1.0.6/NlpToolkit_InformationRetrieval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/PKG-INFO` & `NlpToolkit-InformationRetrieval-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NlpToolkit-InformationRetrieval
-Version: 1.0.5
+Version: 1.0.6
 Summary: Information Retrieval Library
 Home-page: https://github.com/StarlangSoftware/InformationRetrieval-Py
 Author: olcaytaner
 Author-email: olcay.yildiz@ozyegin.edu.tr
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/README.md` & `NlpToolkit-InformationRetrieval-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `NlpToolkit-InformationRetrieval-1.0.5/setup.py` & `NlpToolkit-InformationRetrieval-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 setup(
     name='NlpToolkit-InformationRetrieval',
-    version='1.0.5',
+    version='1.0.6',
     packages=['InformationRetrieval',
               'InformationRetrieval.Document',
               'InformationRetrieval.Index',
               'InformationRetrieval.Query'],
     url='https://github.com/StarlangSoftware/InformationRetrieval-Py',
     license='',
     author='olcaytaner',
```

