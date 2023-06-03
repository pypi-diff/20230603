# Comparing `tmp/EdgeGPT-0.7.2.tar.gz` & `tmp/EdgeGPT-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.7.2.tar", last modified: Fri Jun  2 15:13:08 2023, max compression
+gzip compressed data, was "EdgeGPT-0.8.0.tar", last modified: Sat Jun  3 13:20:13 2023, max compression
```

## Comparing `EdgeGPT-0.7.2.tar` & `EdgeGPT-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:13:08.705255 EdgeGPT-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-02 15:12:29.000000 EdgeGPT-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-06-02 15:13:08.705255 EdgeGPT-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-06-02 15:13:08.000000 EdgeGPT-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-02 15:13:08.705255 EdgeGPT-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-02 15:12:29.000000 EdgeGPT-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:13:08.701255 EdgeGPT-0.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:13:08.705255 EdgeGPT-0.7.2/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-06-02 15:13:08.000000 EdgeGPT-0.7.2/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-02 15:13:08.000000 EdgeGPT-0.7.2/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 15:13:08.000000 EdgeGPT-0.7.2/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-02 15:13:08.000000 EdgeGPT-0.7.2/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-02 15:13:08.000000 EdgeGPT-0.7.2/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 15:13:08.000000 EdgeGPT-0.7.2/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    43363 2023-06-02 15:12:29.000000 EdgeGPT-0.7.2/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-02 15:12:29.000000 EdgeGPT-0.7.2/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:20:13.531043 EdgeGPT-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-03 13:19:42.000000 EdgeGPT-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-06-03 13:20:13.531043 EdgeGPT-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-06-03 13:20:13.000000 EdgeGPT-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-03 13:20:13.531043 EdgeGPT-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-03 13:19:42.000000 EdgeGPT-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:20:13.531043 EdgeGPT-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:20:13.531043 EdgeGPT-0.8.0/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-06-03 13:20:13.000000 EdgeGPT-0.8.0/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-03 13:20:13.000000 EdgeGPT-0.8.0/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 13:20:13.000000 EdgeGPT-0.8.0/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-03 13:20:13.000000 EdgeGPT-0.8.0/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-03 13:20:13.000000 EdgeGPT-0.8.0/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-03 13:20:13.000000 EdgeGPT-0.8.0/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34543 2023-06-03 13:19:42.000000 EdgeGPT-0.8.0/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-03 13:19:42.000000 EdgeGPT-0.8.0/src/ImageGen.py
```

### Comparing `EdgeGPT-0.7.2/LICENSE` & `EdgeGPT-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.7.2/PKG-INFO` & `EdgeGPT-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.7.2
+Version: 0.8.0
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -69,15 +69,15 @@
 # Chatbot
 
 </summary>
 
 ## Authentication
 
 !!! NOT REQUIRED ANYMORE !!!
-Microsoft has made the chat feature available to everyone, so you can skip this step.
+Microsoft has made the chat feature available to everyone, so you don't need to use cookies from a logged-in Microsoft account any more.  However, if you wish to cycle through multiple cookies/accounts, please look at the `EdgeUtils.Cookie` methods.
 
 1. Install the latest version of Microsoft Edge
 <details>
 
 2. Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
 
 </details>
@@ -155,18 +155,18 @@
 
 ### 2) The `Query` and `Cookie` helper classes
 
   </summary>
 
 Create a simple Bing Chat AI query (using the 'precise' conversation style by default) and see just the main text output rather than the whole API response:
 
-Remeber to store your cookies in a specific format: `bing_cookie_*.json`.
+Remeber to store your cookies in a specific format: `bing_cookies_*.json`.
 
 ```python
-from EdgeGPT import Query, Cookie
+from EdgeUtils import Query, Cookie
 
 q = Query("What are you? Give your answer as Python code")
 print(q)
 ```
 
 Or change the conversation style or cookie file to be used:
 
@@ -270,15 +270,15 @@
 ## Running in Python
 
 ### 1) The `ImageQuery` helper class
 
 Generate images based on a simple prompt and download to the current working directory:
 
 ```python
-from EdgeGPT import ImageQuery
+from EdgeUtils import ImageQuery
 
 q=ImageQuery("Meerkats at a garden party in Devon")
 ```
 
 Change the download directory for all future images in this session:
 
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.7.2 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.8.0 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -13,16 +13,18 @@
                [PyPI_version] [Python version] [Total downloads]
   # Setup  ### Install package ```bash python3 -m pip install EdgeGPT --upgrade
 ``` ### Requirements - python 3.8+ - A Microsoft Account with access to
 bing.com/chat> (Optional) - Required in a supported country or region with New
 Bing (Chinese mainland VPN required) - [Selenium](https://pypi.org/project/
 selenium/) (for automatic cookie setup)   # Chatbot  ## Authentication !!! NOT
 REQUIRED ANYMORE !!! Microsoft has made the chat feature available to everyone,
-so you can skip this step. 1. Install the latest version of Microsoft Edge  2.
-Alternatively, you can use any browser and set the user-agent to look like
+so you don't need to use cookies from a logged-in Microsoft account any more.
+However, if you wish to cycle through multiple cookies/accounts, please look at
+the `EdgeUtils.Cookie` methods. 1. Install the latest version of Microsoft Edge
+2. Alternatively, you can use any browser and set the user-agent to look like
 you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64)
 AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/
 111.0.1661.51`). You can do this easily with an extension like "User-Agent
 Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/
 user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox]
 (https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
 3. Open [bing.com/chat](https://bing.com/chat) 4. If you see a chat feature,
@@ -52,16 +54,16 @@
 import asyncio from EdgeGPT import Chatbot, ConversationStyle async def main():
 bot = await Chatbot.create() # Passing cookies is optional print(await bot.ask
 (prompt="Hello world", conversation_style=ConversationStyle.creative)) await
 bot.close() if __name__ == "__main__": asyncio.run(main()) ```   ### 2) The
 `Query` and `Cookie` helper classes  Create a simple Bing Chat AI query (using
 the 'precise' conversation style by default) and see just the main text output
 rather than the whole API response: Remeber to store your cookies in a specific
-format: `bing_cookie_*.json`. ```python from EdgeGPT import Query, Cookie q =
-Query("What are you? Give your answer as Python code") print(q) ``` Or change
+format: `bing_cookies_*.json`. ```python from EdgeUtils import Query, Cookie q
+= Query("What are you? Give your answer as Python code") print(q) ``` Or change
 the conversation style or cookie file to be used: ```python q = Query( "What
 are you? Give your answer as Python code", style="creative", # or 'balanced'
 cookies="./bing_cookies_alternative.json" ) ``` Quickly extract the text
 output, code snippets, list of sources/references, or suggested follow-on
 questions using the following attributes: ```python q.output q.code
 q.suggestions q.sources # for the full json output q.sources_dict # for a
 dictionary of titles and urls ``` Get the orginal prompt and the conversation
@@ -87,15 +89,15 @@
 prompt PROMPT [--output-dir OUTPUT_DIR] [--quiet] [--asyncio] optional
 arguments: -h, --help show this help message and exit -U U Auth cookie from
 browser --cookie-file COOKIE_FILE File containing auth cookie --prompt PROMPT
 Prompt to generate images for --output-dir OUTPUT_DIR Output directory --quiet
 Disable pipeline messages --asyncio Run ImageGen using asyncio ``` ## Running
 in Python ### 1) The `ImageQuery` helper class Generate images based on a
 simple prompt and download to the current working directory: ```python from
-EdgeGPT import ImageQuery q=ImageQuery("Meerkats at a garden party in Devon")
+EdgeUtils import ImageQuery q=ImageQuery("Meerkats at a garden party in Devon")
 ``` Change the download directory for all future images in this session: ```
 Query.image_dirpath = Path("./to_another_folder") ``` ### 2) The `ImageGen`
 class and `asyncio` for more granular control ```python from ImageGen import
 ImageGen import argparse import json async def async_image_gen(args) -> None:
 async with ImageGenAsync(args.U, args.quiet) as image_generator: images = await
 image_generator.get_images(args.prompt) await image_generator.save_images
 (images, output_dir=args.output_dir) if __name__ == "__main__": parser =
```

### Comparing `EdgeGPT-0.7.2/README.md` & `EdgeGPT-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 # Chatbot
 
 </summary>
 
 ## Authentication
 
 !!! NOT REQUIRED ANYMORE !!!
-Microsoft has made the chat feature available to everyone, so you can skip this step.
+Microsoft has made the chat feature available to everyone, so you don't need to use cookies from a logged-in Microsoft account any more.  However, if you wish to cycle through multiple cookies/accounts, please look at the `EdgeUtils.Cookie` methods.
 
 1. Install the latest version of Microsoft Edge
 <details>
 
 2. Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
 
 </details>
@@ -136,18 +136,18 @@
 
 ### 2) The `Query` and `Cookie` helper classes
 
   </summary>
 
 Create a simple Bing Chat AI query (using the 'precise' conversation style by default) and see just the main text output rather than the whole API response:
 
-Remeber to store your cookies in a specific format: `bing_cookie_*.json`.
+Remeber to store your cookies in a specific format: `bing_cookies_*.json`.
 
 ```python
-from EdgeGPT import Query, Cookie
+from EdgeUtils import Query, Cookie
 
 q = Query("What are you? Give your answer as Python code")
 print(q)
 ```
 
 Or change the conversation style or cookie file to be used:
 
@@ -251,15 +251,15 @@
 ## Running in Python
 
 ### 1) The `ImageQuery` helper class
 
 Generate images based on a simple prompt and download to the current working directory:
 
 ```python
-from EdgeGPT import ImageQuery
+from EdgeUtils import ImageQuery
 
 q=ImageQuery("Meerkats at a garden party in Devon")
 ```
 
 Change the download directory for all future images in this session:
 
 ```
```

#### html2text {}

```diff
@@ -3,16 +3,18 @@
                [PyPI_version] [Python version] [Total downloads]
   # Setup  ### Install package ```bash python3 -m pip install EdgeGPT --upgrade
 ``` ### Requirements - python 3.8+ - A Microsoft Account with access to
 bing.com/chat> (Optional) - Required in a supported country or region with New
 Bing (Chinese mainland VPN required) - [Selenium](https://pypi.org/project/
 selenium/) (for automatic cookie setup)   # Chatbot  ## Authentication !!! NOT
 REQUIRED ANYMORE !!! Microsoft has made the chat feature available to everyone,
-so you can skip this step. 1. Install the latest version of Microsoft Edge  2.
-Alternatively, you can use any browser and set the user-agent to look like
+so you don't need to use cookies from a logged-in Microsoft account any more.
+However, if you wish to cycle through multiple cookies/accounts, please look at
+the `EdgeUtils.Cookie` methods. 1. Install the latest version of Microsoft Edge
+2. Alternatively, you can use any browser and set the user-agent to look like
 you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64)
 AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/
 111.0.1661.51`). You can do this easily with an extension like "User-Agent
 Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/
 user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox]
 (https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
 3. Open [bing.com/chat](https://bing.com/chat) 4. If you see a chat feature,
@@ -42,16 +44,16 @@
 import asyncio from EdgeGPT import Chatbot, ConversationStyle async def main():
 bot = await Chatbot.create() # Passing cookies is optional print(await bot.ask
 (prompt="Hello world", conversation_style=ConversationStyle.creative)) await
 bot.close() if __name__ == "__main__": asyncio.run(main()) ```   ### 2) The
 `Query` and `Cookie` helper classes  Create a simple Bing Chat AI query (using
 the 'precise' conversation style by default) and see just the main text output
 rather than the whole API response: Remeber to store your cookies in a specific
-format: `bing_cookie_*.json`. ```python from EdgeGPT import Query, Cookie q =
-Query("What are you? Give your answer as Python code") print(q) ``` Or change
+format: `bing_cookies_*.json`. ```python from EdgeUtils import Query, Cookie q
+= Query("What are you? Give your answer as Python code") print(q) ``` Or change
 the conversation style or cookie file to be used: ```python q = Query( "What
 are you? Give your answer as Python code", style="creative", # or 'balanced'
 cookies="./bing_cookies_alternative.json" ) ``` Quickly extract the text
 output, code snippets, list of sources/references, or suggested follow-on
 questions using the following attributes: ```python q.output q.code
 q.suggestions q.sources # for the full json output q.sources_dict # for a
 dictionary of titles and urls ``` Get the orginal prompt and the conversation
@@ -77,15 +79,15 @@
 prompt PROMPT [--output-dir OUTPUT_DIR] [--quiet] [--asyncio] optional
 arguments: -h, --help show this help message and exit -U U Auth cookie from
 browser --cookie-file COOKIE_FILE File containing auth cookie --prompt PROMPT
 Prompt to generate images for --output-dir OUTPUT_DIR Output directory --quiet
 Disable pipeline messages --asyncio Run ImageGen using asyncio ``` ## Running
 in Python ### 1) The `ImageQuery` helper class Generate images based on a
 simple prompt and download to the current working directory: ```python from
-EdgeGPT import ImageQuery q=ImageQuery("Meerkats at a garden party in Devon")
+EdgeUtils import ImageQuery q=ImageQuery("Meerkats at a garden party in Devon")
 ``` Change the download directory for all future images in this session: ```
 Query.image_dirpath = Path("./to_another_folder") ``` ### 2) The `ImageGen`
 class and `asyncio` for more granular control ```python from ImageGen import
 ImageGen import argparse import json async def async_image_gen(args) -> None:
 async with ImageGenAsync(args.U, args.quiet) as image_generator: images = await
 image_generator.get_images(args.prompt) await image_generator.save_images
 (images, output_dir=args.output_dir) if __name__ == "__main__": parser =
```

### Comparing `EdgeGPT-0.7.2/setup.py` & `EdgeGPT-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.7.2",
+    version="0.8.0",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.7.2/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.8.0/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.7.2
+Version: 0.8.0
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -69,15 +69,15 @@
 # Chatbot
 
 </summary>
 
 ## Authentication
 
 !!! NOT REQUIRED ANYMORE !!!
-Microsoft has made the chat feature available to everyone, so you can skip this step.
+Microsoft has made the chat feature available to everyone, so you don't need to use cookies from a logged-in Microsoft account any more.  However, if you wish to cycle through multiple cookies/accounts, please look at the `EdgeUtils.Cookie` methods.
 
 1. Install the latest version of Microsoft Edge
 <details>
 
 2. Alternatively, you can use any browser and set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
 
 </details>
@@ -155,18 +155,18 @@
 
 ### 2) The `Query` and `Cookie` helper classes
 
   </summary>
 
 Create a simple Bing Chat AI query (using the 'precise' conversation style by default) and see just the main text output rather than the whole API response:
 
-Remeber to store your cookies in a specific format: `bing_cookie_*.json`.
+Remeber to store your cookies in a specific format: `bing_cookies_*.json`.
 
 ```python
-from EdgeGPT import Query, Cookie
+from EdgeUtils import Query, Cookie
 
 q = Query("What are you? Give your answer as Python code")
 print(q)
 ```
 
 Or change the conversation style or cookie file to be used:
 
@@ -270,15 +270,15 @@
 ## Running in Python
 
 ### 1) The `ImageQuery` helper class
 
 Generate images based on a simple prompt and download to the current working directory:
 
 ```python
-from EdgeGPT import ImageQuery
+from EdgeUtils import ImageQuery
 
 q=ImageQuery("Meerkats at a garden party in Devon")
 ```
 
 Change the download directory for all future images in this session:
 
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.7.2 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.8.0 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -13,16 +13,18 @@
                [PyPI_version] [Python version] [Total downloads]
   # Setup  ### Install package ```bash python3 -m pip install EdgeGPT --upgrade
 ``` ### Requirements - python 3.8+ - A Microsoft Account with access to
 bing.com/chat> (Optional) - Required in a supported country or region with New
 Bing (Chinese mainland VPN required) - [Selenium](https://pypi.org/project/
 selenium/) (for automatic cookie setup)   # Chatbot  ## Authentication !!! NOT
 REQUIRED ANYMORE !!! Microsoft has made the chat feature available to everyone,
-so you can skip this step. 1. Install the latest version of Microsoft Edge  2.
-Alternatively, you can use any browser and set the user-agent to look like
+so you don't need to use cookies from a logged-in Microsoft account any more.
+However, if you wish to cycle through multiple cookies/accounts, please look at
+the `EdgeUtils.Cookie` methods. 1. Install the latest version of Microsoft Edge
+2. Alternatively, you can use any browser and set the user-agent to look like
 you're using Edge (e.g., `Mozilla/5.0 (Windows NT 10.0; Win64; x64)
 AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/
 111.0.1661.51`). You can do this easily with an extension like "User-Agent
 Switcher and Manager" for [Chrome](https://chrome.google.com/webstore/detail/
 user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and [Firefox]
 (https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/).
 3. Open [bing.com/chat](https://bing.com/chat) 4. If you see a chat feature,
@@ -52,16 +54,16 @@
 import asyncio from EdgeGPT import Chatbot, ConversationStyle async def main():
 bot = await Chatbot.create() # Passing cookies is optional print(await bot.ask
 (prompt="Hello world", conversation_style=ConversationStyle.creative)) await
 bot.close() if __name__ == "__main__": asyncio.run(main()) ```   ### 2) The
 `Query` and `Cookie` helper classes  Create a simple Bing Chat AI query (using
 the 'precise' conversation style by default) and see just the main text output
 rather than the whole API response: Remeber to store your cookies in a specific
-format: `bing_cookie_*.json`. ```python from EdgeGPT import Query, Cookie q =
-Query("What are you? Give your answer as Python code") print(q) ``` Or change
+format: `bing_cookies_*.json`. ```python from EdgeUtils import Query, Cookie q
+= Query("What are you? Give your answer as Python code") print(q) ``` Or change
 the conversation style or cookie file to be used: ```python q = Query( "What
 are you? Give your answer as Python code", style="creative", # or 'balanced'
 cookies="./bing_cookies_alternative.json" ) ``` Quickly extract the text
 output, code snippets, list of sources/references, or suggested follow-on
 questions using the following attributes: ```python q.output q.code
 q.suggestions q.sources # for the full json output q.sources_dict # for a
 dictionary of titles and urls ``` Get the orginal prompt and the conversation
@@ -87,15 +89,15 @@
 prompt PROMPT [--output-dir OUTPUT_DIR] [--quiet] [--asyncio] optional
 arguments: -h, --help show this help message and exit -U U Auth cookie from
 browser --cookie-file COOKIE_FILE File containing auth cookie --prompt PROMPT
 Prompt to generate images for --output-dir OUTPUT_DIR Output directory --quiet
 Disable pipeline messages --asyncio Run ImageGen using asyncio ``` ## Running
 in Python ### 1) The `ImageQuery` helper class Generate images based on a
 simple prompt and download to the current working directory: ```python from
-EdgeGPT import ImageQuery q=ImageQuery("Meerkats at a garden party in Devon")
+EdgeUtils import ImageQuery q=ImageQuery("Meerkats at a garden party in Devon")
 ``` Change the download directory for all future images in this session: ```
 Query.image_dirpath = Path("./to_another_folder") ``` ### 2) The `ImageGen`
 class and `asyncio` for more granular control ```python from ImageGen import
 ImageGen import argparse import json async def async_image_gen(args) -> None:
 async with ImageGenAsync(args.U, args.quiet) as image_generator: images = await
 image_generator.get_images(args.prompt) await image_generator.save_images
 (images, output_dir=args.output_dir) if __name__ == "__main__": parser =
```

### Comparing `EdgeGPT-0.7.2/src/EdgeGPT.py` & `EdgeGPT-0.8.0/src/EdgeGPT.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 import ssl
 import sys
 import time
 import uuid
 from enum import Enum
 from pathlib import Path
 from typing import Generator
+from typing import Union
 
 import aiofiles
 
 try:
-    from typing import Literal
+    from typing import Literal, Union
 except ImportError:
     from typing_extensions import Literal
 from typing import Optional
 
 import aiohttp
 import certifi
 import httpx
@@ -172,15 +173,15 @@
                 "RegionType": 2,
                 "SourceType": 1,
             },
         ],
     }
 
 
-LOCATION_HINT_TYPES = Optional[LocationHint | Literal["USA", "CHINA", "EU", "UK"]]
+LOCATION_HINT_TYPES = Optional[Union[LocationHint, Literal["USA", "CHINA", "EU", "UK"]]]
 
 
 def get_location_hint_from_locale(locale: str) -> dict | None:
     locale = locale.lower()
     if locale == "en-us":
         hint = LocationHint.USA.value
     if locale == "zh-cn":
@@ -246,15 +247,15 @@
         "clgalileo",
         "gencontentv3",
         "nojbfedge",
     ]
 
 
 CONVERSATION_STYLE_TYPE = Optional[
-    ConversationStyle | Literal["creative", "balanced", "precise"]
+    Union[ConversationStyle, Literal["creative", "balanced", "precise"]]
 ]
 
 
 def _append_identifier(msg: dict) -> str:
     # Convert dict to json string
     return json.dumps(msg, ensure_ascii=False) + DELIMITER
 
@@ -1020,249 +1021,9 @@
         default="en-US",
         required=False,
         help="your locale",
     )
     args = parser.parse_args()
     asyncio.run(async_main(args))
 
-
-class Cookie:
-    """
-    Convenience class for Bing Cookie files, data, and configuration. This Class
-    is updated dynamically by the Query class to allow cycling through >1
-    cookie/credentials file e.g. when daily request limits (current 200 per
-    account per day) are exceeded.
-    """
-
-    current_file_index = 0
-    dirpath = Path("./").resolve()
-    search_pattern = "bing_cookies_*.json"
-    ignore_files = set()
-    current_filepath: dict | None = None
-
-    @classmethod
-    def fetch_default(cls, path: Path | None = None) -> None:
-        from selenium import webdriver
-        from selenium.webdriver.common.by import By
-
-        driver = webdriver.Edge()
-        driver.get("https://bing.com/chat")
-        time.sleep(5)
-        xpath = '//button[@id="bnp_btn_accept"]'
-        driver.find_element(By.XPATH, xpath).click()
-        time.sleep(2)
-        xpath = '//a[@id="codexPrimaryButton"]'
-        driver.find_element(By.XPATH, xpath).click()
-        if path is None:
-            path = Path("./bing_cookies__default.json")
-            # Double underscore ensures this file is first when sorted
-        cookies = driver.get_cookies()
-        Path(path).write_text(json.dumps(cookies, indent=4), encoding="utf-8")
-        # Path again in case supplied path is: str
-        print(f"Cookies saved to: {path}")
-        driver.quit()
-
-    @classmethod
-    def files(cls) -> list[Path]:
-        """Return a sorted list of all cookie files matching .search_pattern"""
-        all_files = set(cls.dirpath.glob(cls.search_pattern))
-        return sorted(all_files - cls.ignore_files)
-
-    @classmethod
-    def import_data(cls) -> None:
-        """
-        Read the active cookie file and populate the following attributes:
-
-          .current_filepath
-          .current_data
-          .image_token
-        """
-        try:
-            cls.current_filepath = cls.files()[cls.current_file_index]
-        except IndexError as exc:
-            print(
-                "> Please set Cookie.current_filepath to a valid cookie file, then run Cookie.import_data()",
-            )
-            raise "No valid cookie file found." from exc
-        print(f"> Importing cookies from: {cls.current_filepath.name}")
-        with Path.open(cls.current_filepath, encoding="utf-8") as file:
-            cls.current_data = json.load(file)
-        cls.image_token = [x for x in cls.current_data if x.get("name") == "_U"]
-        cls.image_token = cls.image_token[0].get("value")
-
-    @classmethod
-    def import_next(cls) -> None:
-        """
-        Cycle through to the next cookies file.  Import it.  Mark the previous
-        file to be ignored for the remainder of the current session.
-        """
-        cls.ignore_files.add(cls.current_filepath)
-        if Cookie.current_file_index >= len(cls.files()):
-            Cookie.current_file_index = 0
-        Cookie.import_data()
-
-
-class Query:
-    """
-    A convenience class that wraps around EdgeGPT.Chatbot to encapsulate input,
-    config, and output all together.  Relies on Cookie class for authentication
-    """
-
-    def __init__(
-        self,
-        prompt: str,
-        style: str = "precise",
-        content_type: str = "text",
-        cookie_file: int = 0,
-        echo: bool = True,
-        echo_prompt: bool = False,
-        proxy: str | None = None,
-    ) -> None:
-        """
-        Arguments:
-
-        prompt: Text to enter into Bing Chat
-        style: creative, balanced, or precise
-        content_type: "text" for Bing Chat; "image" for Dall-e
-        cookie_file: Path, filepath string, or index (int) to list of cookie paths
-        echo: Print something to confirm request made
-        echo_prompt: Print confirmation of the evaluated prompt
-        """
-        self.proxy = proxy
-        self.index = []
-        self.request_count = {}
-        self.image_dirpath = Path("./").resolve()
-        Cookie.import_data()
-        self.index += [self]
-        self.prompt = prompt
-        files = Cookie.files()
-        if isinstance(cookie_file, int):
-            index = cookie_file if cookie_file < len(files) else 0
-        else:
-            if not isinstance(cookie_file, str | Path):
-                message = "'cookie_file' must be an int, str, or Path object"
-                raise TypeError(message)
-            cookie_file = Path(cookie_file)
-            if cookie_file in files:  # Supplied filepath IS in Cookie.dirpath
-                index = files.index(cookie_file)
-            else:  # Supplied filepath is NOT in Cookie.dirpath
-                if cookie_file.is_file():
-                    Cookie.dirpath = cookie_file.parent.resolve()
-                if cookie_file.is_dir():
-                    Cookie.dirpath = cookie_file.resolve()
-                index = 0
-        Cookie.current_file_index = index
-        if content_type == "text":
-            self.style = style
-            self.log_and_send_query(echo, echo_prompt)
-        if content_type == "image":
-            self.create_image()
-
-    def log_and_send_query(self, echo: bool, echo_prompt: bool) -> None:
-        self.response = asyncio.run(self.send_to_bing(echo, echo_prompt))
-        name = str(Cookie.current_filepath.name)
-        if not self.request_count.get(name):
-            self.request_count[name] = 1
-        else:
-            self.request_count[name] += 1
-
-    def create_image(self) -> None:
-        image_generator = ImageGen(Cookie.image_token)
-        image_generator.save_images(
-            image_generator.get_images(self.prompt),
-            output_dir=self.image_dirpath,
-        )
-
-    async def send_to_bing(self, echo: bool = True, echo_prompt: bool = False) -> str:
-        """Creat, submit, then close a Chatbot instance.  Return the response"""
-        retries = len(Cookie.files())
-        while retries:
-            try:
-                # Read the cookies file
-                bot = await Chatbot.create(
-                    proxy=self.proxy,
-                    cookies=Cookie.current_data,
-                )
-                if echo_prompt:
-                    print(f"> {self.prompt}=")
-                if echo:
-                    print("> Waiting for response...")
-                if self.style.lower() not in "creative balanced precise".split():
-                    self.style = "precise"
-                return await bot.ask(
-                    prompt=self.prompt,
-                    conversation_style=getattr(ConversationStyle, self.style),
-                    # wss_link="wss://sydney.bing.com/sydney/ChatHub"
-                    # What other values can this parameter take? It seems to be optional
-                )
-            except KeyError:
-                print(
-                    f"> KeyError [{Cookie.current_filepath.name} may have exceeded the daily limit]",
-                )
-                Cookie.import_next()
-                retries -= 1
-            finally:
-                await bot.close()
-        return None
-
-    @property
-    def output(self) -> str:
-        """The response from a completed Chatbot request"""
-        return self.response["item"]["messages"][1]["text"]
-
-    @property
-    def sources(self) -> str:
-        """The source names and details parsed from a completed Chatbot request"""
-        return self.response["item"]["messages"][1]["sourceAttributions"]
-
-    @property
-    def sources_dict(self) -> dict[str, str]:
-        """The source names and details as a dictionary"""
-        sources_dict = {}
-        name = "providerDisplayName"
-        url = "seeMoreUrl"
-        for source in self.sources:
-            if name in source and url in source:
-                sources_dict[source[name]] = source[url]
-            else:
-                continue
-        return sources_dict
-
-    @property
-    def code(self) -> str:
-        """Extract and join any snippets of Python code in the response"""
-        code_blocks = self.output.split("```")[1:-1:2]
-        code_blocks = ["\n".join(x.splitlines()[1:]) for x in code_blocks]
-        return "\n\n".join(code_blocks)
-
-    @property
-    def languages(self) -> set[str]:
-        """Extract all programming languages given in code blocks"""
-        code_blocks = self.output.split("```")[1:-1:2]
-        return {x.splitlines()[0] for x in code_blocks}
-
-    @property
-    def suggestions(self) -> list[str]:
-        """Follow-on questions suggested by the Chatbot"""
-        return [
-            x["text"]
-            for x in self.response["item"]["messages"][1]["suggestedResponses"]
-        ]
-
-    def __repr__(self) -> str:
-        return f"<EdgeGPT.Query: {self.prompt}>"
-
-    def __str__(self) -> str:
-        return self.output
-
-
-class ImageQuery(Query):
-    def __init__(self, prompt: str, **kwargs) -> None:
-        kwargs["content_type"] = "image"
-        super().__init__(prompt, **kwargs)
-
-    def __repr__(self) -> str:
-        return f"<EdgeGPT.ImageQuery: {self.prompt}>"
-
-
 if __name__ == "__main__":
     main()
```

