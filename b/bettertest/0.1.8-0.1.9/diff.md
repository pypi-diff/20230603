# Comparing `tmp/bettertest-0.1.8.tar.gz` & `tmp/bettertest-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bettertest-0.1.8.tar", max compression
+gzip compressed data, was "bettertest-0.1.9.tar", max compression
```

## Comparing `bettertest-0.1.8.tar` & `bettertest-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,35 @@
--rw-r--r--   0        0        0        0 2023-06-02 20:04:06.755501 bettertest-0.1.8/README.md
--rw-r--r--   0        0        0     8147 2023-06-03 01:10:06.904519 bettertest-0.1.8/bettertest/__init__.py
--rw-r--r--   0        0        0     6049 2023-06-02 20:05:51.516351 bettertest-0.1.8/bettertest/promptTemplate.py
--rw-r--r--   0        0        0    25976 2023-06-02 23:51:45.524589 bettertest-0.1.8/bettertest/test.py
--rw-r--r--   0        0        0      335 2023-06-03 01:10:08.733344 bettertest-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 bettertest-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-02 20:04:06.755501 bettertest-0.1.9/README.md
+-rw-r--r--   0        0        0       15 2023-06-03 01:16:25.466591 bettertest-0.1.9/bettertest/.git/COMMIT_EDITMSG
+-rw-r--r--   0        0        0       23 2023-06-03 01:11:50.013485 bettertest-0.1.9/bettertest/.git/HEAD
+-rw-r--r--   0        0        0      313 2023-06-03 01:16:27.666266 bettertest-0.1.9/bettertest/.git/config
+-rw-r--r--   0        0        0       73 2023-06-03 01:11:50.007226 bettertest-0.1.9/bettertest/.git/description
+-rwxr-xr-x   0        0        0      478 2023-06-03 01:11:50.008783 bettertest-0.1.9/bettertest/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0        0        0      896 2023-06-03 01:11:50.007790 bettertest-0.1.9/bettertest/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0        0        0      189 2023-06-03 01:11:50.009625 bettertest-0.1.9/bettertest/.git/hooks/post-update.sample
+-rwxr-xr-x   0        0        0      424 2023-06-03 01:11:50.009944 bettertest-0.1.9/bettertest/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0        0        0     1642 2023-06-03 01:11:50.008509 bettertest-0.1.9/bettertest/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0        0        0     1348 2023-06-03 01:11:50.010228 bettertest-0.1.9/bettertest/.git/hooks/pre-push.sample
+-rwxr-xr-x   0        0        0     4898 2023-06-03 01:11:50.008243 bettertest-0.1.9/bettertest/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0        0        0      544 2023-06-03 01:11:50.009112 bettertest-0.1.9/bettertest/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0        0        0     1492 2023-06-03 01:11:50.009343 bettertest-0.1.9/bettertest/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0        0        0     3610 2023-06-03 01:11:50.010486 bettertest-0.1.9/bettertest/.git/hooks/update.sample
+-rw-r--r--   0        0        0      549 2023-06-03 01:16:25.463459 bettertest-0.1.9/bettertest/.git/index
+-rw-r--r--   0        0        0      250 2023-06-03 01:11:50.006697 bettertest-0.1.9/bettertest/.git/info/exclude
+-rw-r--r--   0        0        0      174 2023-06-03 01:16:25.471446 bettertest-0.1.9/bettertest/.git/logs/HEAD
+-rw-r--r--   0        0        0      174 2023-06-03 01:16:25.471954 bettertest-0.1.9/bettertest/.git/logs/refs/heads/master
+-rw-r--r--   0        0        0      156 2023-06-03 01:16:27.669146 bettertest-0.1.9/bettertest/.git/logs/refs/remotes/origin/master
+-rw-r--r--   0        0        0      110 2023-06-03 01:16:25.461572 bettertest-0.1.9/bettertest/.git/objects/25/c0b2152e5d1514c70c0bee2642099a75f89e85
+-rw-r--r--   0        0        0     2823 2023-06-03 01:16:06.621945 bettertest-0.1.9/bettertest/.git/objects/35/a42c73dbff08d473cb0754ef523b8dea0b4adf
+-rw-r--r--   0        0        0     7218 2023-06-03 01:16:06.630832 bettertest-0.1.9/bettertest/.git/objects/8b/2ee1f88d310a2dec1ae91818b9b10f1ffefbf2
+-rw-r--r--   0        0        0      162 2023-06-03 01:16:25.462817 bettertest-0.1.9/bettertest/.git/objects/a4/6567b6a06ad368dc9556d760c5c77cf40a14c8
+-rw-r--r--   0        0        0      126 2023-06-03 01:16:25.468332 bettertest-0.1.9/bettertest/.git/objects/b2/de9ae5cbb76b92ef68cf73751cc3524ae749e6
+-rw-r--r--   0        0        0     6398 2023-06-03 01:16:06.624873 bettertest-0.1.9/bettertest/.git/objects/d7/c683472260e7bbbec0605ded764cb8e795f111
+-rw-r--r--   0        0        0     2287 2023-06-03 01:16:06.628353 bettertest-0.1.9/bettertest/.git/objects/e5/e5ec46839842beac6ab62e61a0208dd7468749
+-rw-r--r--   0        0        0     2447 2023-06-03 01:16:06.626507 bettertest-0.1.9/bettertest/.git/objects/ee/2bfbbc12c07b69cf2eabc9ba8ceabcf84553f3
+-rw-r--r--   0        0        0       41 2023-06-03 01:16:25.471067 bettertest-0.1.9/bettertest/.git/refs/heads/master
+-rw-r--r--   0        0        0       41 2023-06-03 01:16:27.667879 bettertest-0.1.9/bettertest/.git/refs/remotes/origin/master
+-rw-r--r--   0        0        0     8147 2023-06-03 01:26:10.636843 bettertest-0.1.9/bettertest/__init__.py
+-rw-r--r--   0        0        0     6049 2023-06-02 20:05:51.516351 bettertest-0.1.9/bettertest/promptTemplate.py
+-rw-r--r--   0        0        0    25976 2023-06-02 23:51:45.524589 bettertest-0.1.9/bettertest/test.py
+-rw-r--r--   0        0        0      335 2023-06-03 01:26:14.627445 bettertest-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 bettertest-0.1.9/PKG-INFO
```

### Comparing `bettertest-0.1.8/bettertest/__init__.py` & `bettertest-0.1.9/bettertest/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 from supabase import create_client
 import traceback
 import csv 
 from tenacity import wait_random_exponential, retry, stop_after_attempt
 import asyncio 
 import time 
 import openai 
@@ -14,15 +14,15 @@
 import uuid
 import builtins
 import inspect
 
 
 supa_url = "https://gwfhoxolvmhoszkvddnv.supabase.co"
 supa_key = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6Imd3ZmhveG9sdm1ob3N6a3ZkZG52Iiwicm9sZSI6ImFub24iLCJpYXQiOjE2ODU3MzU0OTgsImV4cCI6MjAwMTMxMTQ5OH0.gFJSZGvGPx2Prr9bu4TxpkRT1Z7ezDZL-x6zVN1_SE0"
-openai.api_key = "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"
+openai.api_key = "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"
 
 import time
 
 supabase = create_client(supa_url, supa_key)
 
 class LogPrintCalls:
```

### Comparing `bettertest-0.1.8/bettertest/promptTemplate.py` & `bettertest-0.1.9/bettertest/promptTemplate.py`

 * *Files identical despite different names*

### Comparing `bettertest-0.1.8/bettertest/test.py` & `bettertest-0.1.9/bettertest/test.py`

 * *Files identical despite different names*

### Comparing `bettertest-0.1.8/PKG-INFO` & `bettertest-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bettertest
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: krrishdholakia
 Author-email: krrishdholakia@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

