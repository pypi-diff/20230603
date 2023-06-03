# Comparing `tmp/chatdocs-0.1.0.tar.gz` & `tmp/chatdocs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatdocs-0.1.0.tar", last modified: Fri Jun  2 21:28:18 2023, max compression
+gzip compressed data, was "chatdocs-0.1.1.tar", last modified: Sat Jun  3 12:54:50 2023, max compression
```

## Comparing `chatdocs-0.1.0.tar` & `chatdocs-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 21:28:18.487817 chatdocs-0.1.0/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3994 2023-06-02 21:28:18.487817 chatdocs-0.1.0/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2279 2023-06-02 20:59:47.000000 chatdocs-0.1.0/README.md
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 21:28:18.487817 chatdocs-0.1.0/chatdocs/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-06-01 18:46:12.000000 chatdocs-0.1.0/chatdocs/__init__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       29 2023-06-01 19:38:54.000000 chatdocs-0.1.0/chatdocs/__main__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     6201 2023-06-02 17:41:03.000000 chatdocs-0.1.0/chatdocs/add.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3061 2023-06-02 19:30:06.000000 chatdocs-0.1.0/chatdocs/chat.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      178 2023-06-02 17:43:46.000000 chatdocs-0.1.0/chatdocs/config.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      290 2023-06-02 20:37:18.000000 chatdocs-0.1.0/chatdocs/download.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2454 2023-06-02 11:45:11.000000 chatdocs-0.1.0/chatdocs/main.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-02 21:28:18.487817 chatdocs-0.1.0/chatdocs.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3994 2023-06-02 21:28:18.000000 chatdocs-0.1.0/chatdocs.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      375 2023-06-02 21:28:18.000000 chatdocs-0.1.0/chatdocs.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-02 21:28:18.000000 chatdocs-0.1.0/chatdocs.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       48 2023-06-02 21:28:18.000000 chatdocs-0.1.0/chatdocs.egg-info/entry_points.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-02 21:28:18.000000 chatdocs-0.1.0/chatdocs.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      313 2023-06-02 21:28:18.000000 chatdocs-0.1.0/chatdocs.egg-info/requires.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-06-02 21:28:18.000000 chatdocs-0.1.0/chatdocs.egg-info/top_level.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-06-02 21:28:18.487817 chatdocs-0.1.0/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1979 2023-06-02 21:27:10.000000 chatdocs-0.1.0/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-03 12:54:50.515591 chatdocs-0.1.1/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3994 2023-06-03 12:54:50.515591 chatdocs-0.1.1/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2279 2023-06-02 20:59:47.000000 chatdocs-0.1.1/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-03 12:54:50.515591 chatdocs-0.1.1/chatdocs/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-06-01 18:46:12.000000 chatdocs-0.1.1/chatdocs/__init__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       29 2023-06-01 19:38:54.000000 chatdocs-0.1.1/chatdocs/__main__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     6201 2023-06-02 17:41:03.000000 chatdocs-0.1.1/chatdocs/add.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3142 2023-06-03 11:09:24.000000 chatdocs-0.1.1/chatdocs/chat.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      178 2023-06-02 17:43:46.000000 chatdocs-0.1.1/chatdocs/config.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      290 2023-06-02 20:37:18.000000 chatdocs-0.1.1/chatdocs/download.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2454 2023-06-02 11:45:11.000000 chatdocs-0.1.1/chatdocs/main.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-03 12:54:50.515591 chatdocs-0.1.1/chatdocs.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3994 2023-06-03 12:54:50.000000 chatdocs-0.1.1/chatdocs.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      375 2023-06-03 12:54:50.000000 chatdocs-0.1.1/chatdocs.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-03 12:54:50.000000 chatdocs-0.1.1/chatdocs.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       48 2023-06-03 12:54:50.000000 chatdocs-0.1.1/chatdocs.egg-info/entry_points.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-03 12:54:50.000000 chatdocs-0.1.1/chatdocs.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      313 2023-06-03 12:54:50.000000 chatdocs-0.1.1/chatdocs.egg-info/requires.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-06-03 12:54:50.000000 chatdocs-0.1.1/chatdocs.egg-info/top_level.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-06-03 12:54:50.515591 chatdocs-0.1.1/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1979 2023-06-03 12:51:50.000000 chatdocs-0.1.1/setup.py
```

### Comparing `chatdocs-0.1.0/PKG-INFO` & `chatdocs-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatdocs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Chat with your documents offline using AI.
 Home-page: https://github.com/marella/chatdocs
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [ChatDocs](https://github.com/marella/chatdocs) [![PyPI](https://img.shields.io/pypi/v/chatdocs)](https://pypi.org/project/chatdocs/) [![tests](https://github.com/marella/chatdocs/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/chatdocs/actions/workflows/tests.yml)
```

### Comparing `chatdocs-0.1.0/README.md` & `chatdocs-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `chatdocs-0.1.0/chatdocs/add.py` & `chatdocs-0.1.1/chatdocs/add.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.1.0/chatdocs/chat.py` & `chatdocs-0.1.1/chatdocs/chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 from chromadb.config import Settings
 from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 from langchain.chains import RetrievalQA
 from langchain.embeddings import HuggingFaceInstructEmbeddings
 from langchain.llms import CTransformers, HuggingFacePipeline
 from langchain.vectorstores import Chroma
 from rich import print
+from rich.markup import escape
 from rich.panel import Panel
 
 from . import config
 
 
 def print_response(text: str) -> None:
-    print(f"[bright_cyan]{text}[/bright_cyan]", end="", flush=True)
+    print(f"[bright_cyan]{escape(text)}", end="", flush=True)
 
 
 class StreamingPrintCallbackHandler(StreamingStdOutCallbackHandler):
     def on_llm_new_token(self, token: str, **kwargs: Any) -> None:
         print_response(token)
 
 
@@ -72,33 +73,34 @@
 
     interactive = not query
     print()
     if interactive:
         print("Type your query below and press Enter.")
         print("Type 'exit' or 'quit' or 'q' to exit the application.\n")
     while True:
-        print("[bold]Q:[/bold] ", end="", flush=True)
+        print("[bold]Q: ", end="", flush=True)
         if interactive:
             query = input()
         else:
-            print(query)
+            print(escape(query))
         print()
         if query.strip() in ["exit", "quit", "q"]:
             print("Exiting...\n")
             break
-        print("[bold]A:[/bold]", end="", flush=True)
+        print("[bold]A:", end="", flush=True)
 
         res = qa(query)
         if hf:
             print_response(res["result"])
 
         print()
         for doc in res["source_documents"]:
+            source, content = doc.metadata["source"], doc.page_content
             print(
                 Panel(
-                    f"[bright_blue]{doc.metadata['source']}[/bright_blue]\n\n{doc.page_content}"
+                    f"[bright_blue]{escape(source)}[/bright_blue]\n\n{escape(content)}"
                 )
             )
         print()
 
         if not interactive:
             break
```

### Comparing `chatdocs-0.1.0/chatdocs/main.py` & `chatdocs-0.1.1/chatdocs/main.py`

 * *Files identical despite different names*

### Comparing `chatdocs-0.1.0/chatdocs.egg-info/PKG-INFO` & `chatdocs-0.1.1/chatdocs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatdocs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Chat with your documents offline using AI.
 Home-page: https://github.com/marella/chatdocs
 Author: Ravindra Marella
 Author-email: mv.ravindra007@gmail.com
 License: MIT
 Description: # [ChatDocs](https://github.com/marella/chatdocs) [![PyPI](https://img.shields.io/pypi/v/chatdocs)](https://pypi.org/project/chatdocs/) [![tests](https://github.com/marella/chatdocs/actions/workflows/tests.yml/badge.svg)](https://github.com/marella/chatdocs/actions/workflows/tests.yml)
```

### Comparing `chatdocs-0.1.0/setup.py` & `chatdocs-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md") as f:
     long_description = f.read()
 
 name = "chatdocs"
 
 setup(
     name=name,
-    version="0.1.0",
+    version="0.1.1",
     description="Chat with your documents offline using AI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Ravindra Marella",
     author_email="mv.ravindra007@gmail.com",
     url="https://github.com/marella/{}".format(name),
     license="MIT",
```

