# Comparing `tmp/roboduck-0.4.0.tar.gz` & `tmp/roboduck-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboduck-0.4.0.tar", last modified: Fri Jun  2 06:26:35 2023, max compression
+gzip compressed data, was "roboduck-0.4.1.tar", last modified: Sat Jun  3 04:23:19 2023, max compression
```

## Comparing `roboduck-0.4.0.tar` & `roboduck-0.4.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-02 06:26:35.524701 roboduck-0.4.0/
--rw-r--r--   0 hmamin     (501) staff       (20)      110 2023-03-29 04:32:37.000000 roboduck-0.4.0/MANIFEST.in
--rw-r--r--   0 hmamin     (501) staff       (20)    11529 2023-06-02 06:26:35.524312 roboduck-0.4.0/PKG-INFO
--rw-r--r--   0 hmamin     (501) staff       (20)    11300 2023-05-29 21:50:53.000000 roboduck-0.4.0/README.md
--rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-04-30 05:54:13.000000 roboduck-0.4.0/requirements.txt
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-02 06:26:35.517135 roboduck-0.4.0/roboduck/
--rw-r--r--   0 hmamin     (501) staff       (20)      548 2023-06-02 06:25:16.000000 roboduck-0.4.0/roboduck/__init__.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-02 06:26:35.519882 roboduck-0.4.0/roboduck/cli/
--rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-17 05:19:25.000000 roboduck-0.4.0/roboduck/cli/__init__.py
--rw-r--r--   0 hmamin     (501) staff       (20)     3412 2023-05-28 04:07:25.000000 roboduck-0.4.0/roboduck/cli/cli.py
--rw-r--r--   0 hmamin     (501) staff       (20)     7410 2023-05-24 05:02:54.000000 roboduck-0.4.0/roboduck/config.py
--rw-r--r--   0 hmamin     (501) staff       (20)    22975 2023-05-31 07:15:56.000000 roboduck-0.4.0/roboduck/debug.py
--rw-r--r--   0 hmamin     (501) staff       (20)    10858 2023-05-29 22:16:38.000000 roboduck-0.4.0/roboduck/decorators.py
--rw-r--r--   0 hmamin     (501) staff       (20)    11439 2023-05-29 23:13:09.000000 roboduck-0.4.0/roboduck/errors.py
--rw-r--r--   0 hmamin     (501) staff       (20)     5700 2023-05-25 04:02:32.000000 roboduck-0.4.0/roboduck/ipy_utils.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-02 06:26:35.521304 roboduck-0.4.0/roboduck/langchain/
--rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-13 04:59:30.000000 roboduck-0.4.0/roboduck/langchain/__init__.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1512 2023-05-15 05:01:22.000000 roboduck-0.4.0/roboduck/langchain/callbacks.py
--rw-r--r--   0 hmamin     (501) staff       (20)    14589 2023-05-23 05:07:18.000000 roboduck-0.4.0/roboduck/langchain/chat.py
--rw-r--r--   0 hmamin     (501) staff       (20)     1136 2023-05-15 05:02:58.000000 roboduck-0.4.0/roboduck/langchain/utils.py
--rw-r--r--   0 hmamin     (501) staff       (20)     6333 2023-05-29 23:12:35.000000 roboduck-0.4.0/roboduck/logging.py
--rw-r--r--   0 hmamin     (501) staff       (20)     5183 2023-05-31 05:27:53.000000 roboduck-0.4.0/roboduck/magic.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-02 06:26:35.521893 roboduck-0.4.0/roboduck/prompts/
--rw-r--r--   0 hmamin     (501) staff       (20)       36 2023-03-29 04:32:37.000000 roboduck-0.4.0/roboduck/prompts/__init__.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-02 06:26:35.523867 roboduck-0.4.0/roboduck/prompts/chat/
--rw-r--r--   0 hmamin     (501) staff       (20)      650 2023-04-20 04:16:32.000000 roboduck-0.4.0/roboduck/prompts/chat/__template__.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2123 2023-05-25 03:31:37.000000 roboduck-0.4.0/roboduck/prompts/chat/debug.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2170 2023-05-25 03:31:43.000000 roboduck-0.4.0/roboduck/prompts/chat/debug_full.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2098 2023-05-25 03:31:49.000000 roboduck-0.4.0/roboduck/prompts/chat/debug_full_stack_trace.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     2067 2023-05-25 03:31:54.000000 roboduck-0.4.0/roboduck/prompts/chat/debug_stack_trace.yaml
--rw-r--r--   0 hmamin     (501) staff       (20)     3887 2023-05-28 03:58:55.000000 roboduck-0.4.0/roboduck/prompts/utils.py
--rw-r--r--   0 hmamin     (501) staff       (20)    15138 2023-05-28 04:07:13.000000 roboduck-0.4.0/roboduck/utils.py
-drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-02 06:26:35.519401 roboduck-0.4.0/roboduck.egg-info/
--rw-r--r--   0 hmamin     (501) staff       (20)    11529 2023-06-02 06:26:34.000000 roboduck-0.4.0/roboduck.egg-info/PKG-INFO
--rw-r--r--   0 hmamin     (501) staff       (20)      843 2023-06-02 06:26:35.000000 roboduck-0.4.0/roboduck.egg-info/SOURCES.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        1 2023-06-02 06:26:34.000000 roboduck-0.4.0/roboduck.egg-info/dependency_links.txt
--rw-r--r--   0 hmamin     (501) staff       (20)       46 2023-06-02 06:26:35.000000 roboduck-0.4.0/roboduck.egg-info/entry_points.txt
--rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-06-02 06:26:35.000000 roboduck-0.4.0/roboduck.egg-info/requires.txt
--rw-r--r--   0 hmamin     (501) staff       (20)        9 2023-06-02 06:26:35.000000 roboduck-0.4.0/roboduck.egg-info/top_level.txt
--rw-r--r--   0 hmamin     (501) staff       (20)       38 2023-06-02 06:26:35.524871 roboduck-0.4.0/setup.cfg
--rw-r--r--   0 hmamin     (501) staff       (20)     1181 2023-05-27 04:33:17.000000 roboduck-0.4.0/setup.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-03 04:23:19.641137 roboduck-0.4.1/
+-rw-r--r--   0 hmamin     (501) staff       (20)      110 2023-03-29 04:32:37.000000 roboduck-0.4.1/MANIFEST.in
+-rw-r--r--   0 hmamin     (501) staff       (20)    11724 2023-06-03 04:23:19.640699 roboduck-0.4.1/PKG-INFO
+-rw-r--r--   0 hmamin     (501) staff       (20)    11300 2023-06-03 04:08:08.000000 roboduck-0.4.1/README.md
+-rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-04-30 05:54:13.000000 roboduck-0.4.1/requirements.txt
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-03 04:23:19.629419 roboduck-0.4.1/roboduck/
+-rw-r--r--   0 hmamin     (501) staff       (20)      548 2023-06-03 04:23:07.000000 roboduck-0.4.1/roboduck/__init__.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-03 04:23:19.633474 roboduck-0.4.1/roboduck/cli/
+-rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-17 05:19:25.000000 roboduck-0.4.1/roboduck/cli/__init__.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     3412 2023-05-28 04:07:25.000000 roboduck-0.4.1/roboduck/cli/cli.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     7410 2023-05-24 05:02:54.000000 roboduck-0.4.1/roboduck/config.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    22975 2023-05-31 07:15:56.000000 roboduck-0.4.1/roboduck/debug.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    10858 2023-05-29 22:16:38.000000 roboduck-0.4.1/roboduck/decorators.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    11439 2023-05-29 23:13:09.000000 roboduck-0.4.1/roboduck/errors.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     5700 2023-05-25 04:02:32.000000 roboduck-0.4.1/roboduck/ipy_utils.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-03 04:23:19.634853 roboduck-0.4.1/roboduck/langchain/
+-rw-r--r--   0 hmamin     (501) staff       (20)        0 2023-05-13 04:59:30.000000 roboduck-0.4.1/roboduck/langchain/__init__.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1512 2023-05-15 05:01:22.000000 roboduck-0.4.1/roboduck/langchain/callbacks.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    14589 2023-05-23 05:07:18.000000 roboduck-0.4.1/roboduck/langchain/chat.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     1136 2023-05-15 05:02:58.000000 roboduck-0.4.1/roboduck/langchain/utils.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     6333 2023-05-29 23:12:35.000000 roboduck-0.4.1/roboduck/logging.py
+-rw-r--r--   0 hmamin     (501) staff       (20)     5183 2023-05-31 05:27:53.000000 roboduck-0.4.1/roboduck/magic.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-03 04:23:19.635511 roboduck-0.4.1/roboduck/prompts/
+-rw-r--r--   0 hmamin     (501) staff       (20)       36 2023-03-29 04:32:37.000000 roboduck-0.4.1/roboduck/prompts/__init__.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-03 04:23:19.640007 roboduck-0.4.1/roboduck/prompts/chat/
+-rw-r--r--   0 hmamin     (501) staff       (20)      650 2023-04-20 04:16:32.000000 roboduck-0.4.1/roboduck/prompts/chat/__template__.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2123 2023-05-25 03:31:37.000000 roboduck-0.4.1/roboduck/prompts/chat/debug.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2170 2023-05-25 03:31:43.000000 roboduck-0.4.1/roboduck/prompts/chat/debug_full.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2098 2023-05-25 03:31:49.000000 roboduck-0.4.1/roboduck/prompts/chat/debug_full_stack_trace.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     2067 2023-05-25 03:31:54.000000 roboduck-0.4.1/roboduck/prompts/chat/debug_stack_trace.yaml
+-rw-r--r--   0 hmamin     (501) staff       (20)     3887 2023-05-28 03:58:55.000000 roboduck-0.4.1/roboduck/prompts/utils.py
+-rw-r--r--   0 hmamin     (501) staff       (20)    15138 2023-05-28 04:07:13.000000 roboduck-0.4.1/roboduck/utils.py
+drwxr-xr-x   0 hmamin     (501) staff       (20)        0 2023-06-03 04:23:19.632880 roboduck-0.4.1/roboduck.egg-info/
+-rw-r--r--   0 hmamin     (501) staff       (20)    11724 2023-06-03 04:23:19.000000 roboduck-0.4.1/roboduck.egg-info/PKG-INFO
+-rw-r--r--   0 hmamin     (501) staff       (20)      843 2023-06-03 04:23:19.000000 roboduck-0.4.1/roboduck.egg-info/SOURCES.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        1 2023-06-03 04:23:19.000000 roboduck-0.4.1/roboduck.egg-info/dependency_links.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       46 2023-06-03 04:23:19.000000 roboduck-0.4.1/roboduck.egg-info/entry_points.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)      100 2023-06-03 04:23:19.000000 roboduck-0.4.1/roboduck.egg-info/requires.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)        9 2023-06-03 04:23:19.000000 roboduck-0.4.1/roboduck.egg-info/top_level.txt
+-rw-r--r--   0 hmamin     (501) staff       (20)       38 2023-06-03 04:23:19.641273 roboduck-0.4.1/setup.cfg
+-rw-r--r--   0 hmamin     (501) staff       (20)     1408 2023-06-03 04:21:44.000000 roboduck-0.4.1/setup.py
```

### Comparing `roboduck-0.4.0/PKG-INFO` & `roboduck-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: roboduck
-Version: 0.4.0
+Version: 0.4.1
 Summary: A natural language debugger.
 Author: Harrison Mamin
 Author-email: harrisonmamin@gmail.com
 License: UNKNOWN
+Project-URL: Documentation, https://hdmamin.github.io/roboduck/
+Project-URL: Repository, https://github.com/hdmamin/roboduck
+Keywords: debugging,llm,language model,dev tools,errors,jupyter magic
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/hdmamin/roboduck/main/data/images/roboduck_blue_banner.png" alt="roboduck logo">
 <p></p>
 <a href="https://hdmamin.github.io/roboduck/"><img src="https://img.shields.io/badge/Documentation-Online-blue.svg" alt="Documentation"></a>
@@ -143,15 +146,15 @@
 
 To rebuild the docs locally:
 ```
 make docs
 ```
 
 ---
-Start of auto-generated file data.<br/>Last updated: 2023-05-29 14:50:53
+Start of auto-generated file data.<br/>Last updated: 2023-06-02 21:08:08
 
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th>File</th>
       <th>Summary</th>
       <th>Line Count</th>
@@ -160,65 +163,65 @@
     </tr>
   </thead>
   <tbody>
     <tr>
       <td>__init__.py</td>
       <td>_</td>
       <td>17</td>
-      <td>2023-05-26 21:33:35</td>
+      <td>2023-06-01 23:26:46</td>
       <td>548.00 b</td>
     </tr>
     <tr>
       <td>config.py</td>
       <td>Allow us to easily read from and write to roboduck's config file.<br/><br/>Roboduck creates a config file at `~/.roboduck/config.yaml`. This currently<br/>supports only two fields:<br/><br/>- `openai_api_key`: See the [Quickstart](https://hdmamin.github.io/roboduck/)<br/>for setup help.<br/><br/>- `model_name` (optional): Roboduck is configured to use gpt-3.5-turbo by<br/>default. This field lets you change that (e.g. to gpt-4). If present in the<br/>config file, this will take priority over any model_name field specified in a<br/>chat template<br/>(e.g. our [default debug prompt template](https://github.com/hdmamin/roboduck/blob/7ff904972921fd3f82b8b9fd862c4ffc7b61aee4/lib/roboduck/prompts/chat/debug.yaml#L2)).<br/>You can view valid options with `roboduck.available_models()`.<br/>You can still override the config default by manually passing a value into a<br/>function, e.g. `duck(model_name='gpt-4-32k')`.<br/><br/>You can manually edit your config file or use a command like<br/>`roboduck.update_config(model_name='gpt-4')`. Passing in a value of None<br/>(e.g. `roboduck.update_config(model_name=None)`) will delete that field from<br/>your config file.</td>
       <td>181</td>
       <td>2023-05-23 22:09:40</td>
       <td>7.41 kb</td>
     </tr>
     <tr>
       <td>debug.py</td>
       <td>A conversational debugger and drop-in replacement for pdb. Python's default<br/>interactive debugging session is already a crude conversation with your<br/>program or interpreter, in a sense - this just lets your program communicate to<br/>you more effectively.<br/><br/>Quickstart<br/>----------<br/>Here's a broken version of bubble sort that places a `duck()` call on the<br/>second to last line where you might normally call `breakpoint()`.<br/><br/>```<br/>from roboduck import duck<br/><br/>def bubble_sort(nums):<br/>    for i in range(len(nums)):<br/>        for j in range(len(nums) - 1):<br/>            if nums[j] &gt; nums[j + 1]:<br/>                nums[j + 1] = nums[j]<br/>                nums[j] = nums[j + 1]<br/>                duck()   # &lt;--------------------------- instead of breakpoint()<br/>    return nums<br/><br/>nums = [3, 1, 9, 2, 1]<br/>bubble_sort(nums)<br/>```</td>
-      <td>486</td>
-      <td>2023-05-25 22:14:45</td>
-      <td>20.18 kb</td>
+      <td>571</td>
+      <td>2023-05-31 00:16:13</td>
+      <td>22.98 kb</td>
     </tr>
     <tr>
       <td>decorators.py</td>
       <td>Miscellaneous decorators used throughout the library.</td>
-      <td>287</td>
-      <td>2023-05-21 22:59:59</td>
-      <td>10.26 kb</td>
+      <td>305</td>
+      <td>2023-05-29 15:21:23</td>
+      <td>10.86 kb</td>
     </tr>
     <tr>
       <td>errors.py</td>
       <td>Errors that explain themselves! Or more precisely, errors that are explained<br/>to you by a gpt-esque model. Simply importing this module will change python's<br/>default behavior when it encounters an error.<br/><br/>Quickstart<br/>----------<br/>Importing the errors module automatically enables optional error explanations.<br/>`disable()` reverts to python's regular behavior on errors. `enable()` can be<br/>used to re-enable error explanations or to change settings. For example,<br/>setting auto=True automatically explains all errors rather than asking the user<br/>if they want an explanation (y/n) when an error occurs.<br/>```<br/>from roboduck import errors<br/><br/>data = {'x': 0}<br/>y = data.x<br/><br/>errors.disable()<br/>y = data.x<br/><br/>errors.enable(auto=True)<br/>y = data.x<br/>```</td>
-      <td>276</td>
-      <td>2023-05-28 21:41:30</td>
-      <td>11.35 kb</td>
+      <td>279</td>
+      <td>2023-05-29 16:15:02</td>
+      <td>11.44 kb</td>
     </tr>
     <tr>
       <td>ipy_utils.py</td>
       <td>Functions related to loading, saving, or otherwise working with ipython<br/>sessions or jupyter notebooks.</td>
       <td>186</td>
       <td>2023-05-24 21:37:48</td>
       <td>5.70 kb</td>
     </tr>
     <tr>
       <td>logging.py</td>
       <td>Logger that attempts to diagnose and propose a solution for any errors it<br/>is asked to log. Unlike our debugger and errors modules, explanations are<br/>not streamed because the intended use case is not focused on live development.<br/><br/>Quickstart<br/>----------<br/>```<br/>from roboduck import logging<br/><br/>logger = logging.getLogger(path='/tmp/log.txt')<br/>data = {'x': 0}<br/>try:<br/>    x = data.x<br/>except Exception as e:<br/>    logger.error(e)<br/>```</td>
-      <td>157</td>
-      <td>2023-05-18 22:25:48</td>
-      <td>6.28 kb</td>
+      <td>158</td>
+      <td>2023-05-29 16:15:02</td>
+      <td>6.33 kb</td>
     </tr>
     <tr>
       <td>magic.py</td>
       <td>GPT-powered rough equivalent of the `%debug` Jupyter magic. After an error<br/>occurs, just run %duck in the next cell to get an explanation. This is very<br/>similar to using the errors module, but is less intrusive - you only call it<br/>when you want an explanation, rather than having to type y/n after each error.<br/>We also provide `paste` mode, which attempts to paste a solution into a new<br/>code cell below, and `interactive` mode, which throws you into a conversational<br/>debugging session (technically closer to the original `%debug` magic<br/>functionality.<br/><br/>Quickstart<br/>----------<br/>```<br/># cell 1<br/>from roboduck import magic<br/><br/>nums = [1, 2, 3]<br/>nums.add(4)<br/>```<br/><br/>```<br/># cell 2<br/>%duck<br/>```</td>
-      <td>126</td>
-      <td>2023-05-28 21:41:30</td>
-      <td>5.11 kb</td>
+      <td>127</td>
+      <td>2023-05-30 22:28:43</td>
+      <td>5.18 kb</td>
     </tr>
     <tr>
       <td>utils.py</td>
       <td>Utility functions used by other roboduck modules.</td>
       <td>420</td>
       <td>2023-05-27 21:32:29</td>
       <td>15.14 kb</td>
```

### Comparing `roboduck-0.4.0/README.md` & `roboduck-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
 To rebuild the docs locally:
 ```
 make docs
 ```
 
 ---
-Start of auto-generated file data.<br/>Last updated: 2023-05-29 14:50:53
+Start of auto-generated file data.<br/>Last updated: 2023-06-02 21:08:08
 
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th>File</th>
       <th>Summary</th>
       <th>Line Count</th>
@@ -150,65 +150,65 @@
     </tr>
   </thead>
   <tbody>
     <tr>
       <td>__init__.py</td>
       <td>_</td>
       <td>17</td>
-      <td>2023-05-26 21:33:35</td>
+      <td>2023-06-01 23:26:46</td>
       <td>548.00 b</td>
     </tr>
     <tr>
       <td>config.py</td>
       <td>Allow us to easily read from and write to roboduck's config file.<br/><br/>Roboduck creates a config file at `~/.roboduck/config.yaml`. This currently<br/>supports only two fields:<br/><br/>- `openai_api_key`: See the [Quickstart](https://hdmamin.github.io/roboduck/)<br/>for setup help.<br/><br/>- `model_name` (optional): Roboduck is configured to use gpt-3.5-turbo by<br/>default. This field lets you change that (e.g. to gpt-4). If present in the<br/>config file, this will take priority over any model_name field specified in a<br/>chat template<br/>(e.g. our [default debug prompt template](https://github.com/hdmamin/roboduck/blob/7ff904972921fd3f82b8b9fd862c4ffc7b61aee4/lib/roboduck/prompts/chat/debug.yaml#L2)).<br/>You can view valid options with `roboduck.available_models()`.<br/>You can still override the config default by manually passing a value into a<br/>function, e.g. `duck(model_name='gpt-4-32k')`.<br/><br/>You can manually edit your config file or use a command like<br/>`roboduck.update_config(model_name='gpt-4')`. Passing in a value of None<br/>(e.g. `roboduck.update_config(model_name=None)`) will delete that field from<br/>your config file.</td>
       <td>181</td>
       <td>2023-05-23 22:09:40</td>
       <td>7.41 kb</td>
     </tr>
     <tr>
       <td>debug.py</td>
       <td>A conversational debugger and drop-in replacement for pdb. Python's default<br/>interactive debugging session is already a crude conversation with your<br/>program or interpreter, in a sense - this just lets your program communicate to<br/>you more effectively.<br/><br/>Quickstart<br/>----------<br/>Here's a broken version of bubble sort that places a `duck()` call on the<br/>second to last line where you might normally call `breakpoint()`.<br/><br/>```<br/>from roboduck import duck<br/><br/>def bubble_sort(nums):<br/>    for i in range(len(nums)):<br/>        for j in range(len(nums) - 1):<br/>            if nums[j] &gt; nums[j + 1]:<br/>                nums[j + 1] = nums[j]<br/>                nums[j] = nums[j + 1]<br/>                duck()   # &lt;--------------------------- instead of breakpoint()<br/>    return nums<br/><br/>nums = [3, 1, 9, 2, 1]<br/>bubble_sort(nums)<br/>```</td>
-      <td>486</td>
-      <td>2023-05-25 22:14:45</td>
-      <td>20.18 kb</td>
+      <td>571</td>
+      <td>2023-05-31 00:16:13</td>
+      <td>22.98 kb</td>
     </tr>
     <tr>
       <td>decorators.py</td>
       <td>Miscellaneous decorators used throughout the library.</td>
-      <td>287</td>
-      <td>2023-05-21 22:59:59</td>
-      <td>10.26 kb</td>
+      <td>305</td>
+      <td>2023-05-29 15:21:23</td>
+      <td>10.86 kb</td>
     </tr>
     <tr>
       <td>errors.py</td>
       <td>Errors that explain themselves! Or more precisely, errors that are explained<br/>to you by a gpt-esque model. Simply importing this module will change python's<br/>default behavior when it encounters an error.<br/><br/>Quickstart<br/>----------<br/>Importing the errors module automatically enables optional error explanations.<br/>`disable()` reverts to python's regular behavior on errors. `enable()` can be<br/>used to re-enable error explanations or to change settings. For example,<br/>setting auto=True automatically explains all errors rather than asking the user<br/>if they want an explanation (y/n) when an error occurs.<br/>```<br/>from roboduck import errors<br/><br/>data = {'x': 0}<br/>y = data.x<br/><br/>errors.disable()<br/>y = data.x<br/><br/>errors.enable(auto=True)<br/>y = data.x<br/>```</td>
-      <td>276</td>
-      <td>2023-05-28 21:41:30</td>
-      <td>11.35 kb</td>
+      <td>279</td>
+      <td>2023-05-29 16:15:02</td>
+      <td>11.44 kb</td>
     </tr>
     <tr>
       <td>ipy_utils.py</td>
       <td>Functions related to loading, saving, or otherwise working with ipython<br/>sessions or jupyter notebooks.</td>
       <td>186</td>
       <td>2023-05-24 21:37:48</td>
       <td>5.70 kb</td>
     </tr>
     <tr>
       <td>logging.py</td>
       <td>Logger that attempts to diagnose and propose a solution for any errors it<br/>is asked to log. Unlike our debugger and errors modules, explanations are<br/>not streamed because the intended use case is not focused on live development.<br/><br/>Quickstart<br/>----------<br/>```<br/>from roboduck import logging<br/><br/>logger = logging.getLogger(path='/tmp/log.txt')<br/>data = {'x': 0}<br/>try:<br/>    x = data.x<br/>except Exception as e:<br/>    logger.error(e)<br/>```</td>
-      <td>157</td>
-      <td>2023-05-18 22:25:48</td>
-      <td>6.28 kb</td>
+      <td>158</td>
+      <td>2023-05-29 16:15:02</td>
+      <td>6.33 kb</td>
     </tr>
     <tr>
       <td>magic.py</td>
       <td>GPT-powered rough equivalent of the `%debug` Jupyter magic. After an error<br/>occurs, just run %duck in the next cell to get an explanation. This is very<br/>similar to using the errors module, but is less intrusive - you only call it<br/>when you want an explanation, rather than having to type y/n after each error.<br/>We also provide `paste` mode, which attempts to paste a solution into a new<br/>code cell below, and `interactive` mode, which throws you into a conversational<br/>debugging session (technically closer to the original `%debug` magic<br/>functionality.<br/><br/>Quickstart<br/>----------<br/>```<br/># cell 1<br/>from roboduck import magic<br/><br/>nums = [1, 2, 3]<br/>nums.add(4)<br/>```<br/><br/>```<br/># cell 2<br/>%duck<br/>```</td>
-      <td>126</td>
-      <td>2023-05-28 21:41:30</td>
-      <td>5.11 kb</td>
+      <td>127</td>
+      <td>2023-05-30 22:28:43</td>
+      <td>5.18 kb</td>
     </tr>
     <tr>
       <td>utils.py</td>
       <td>Utility functions used by other roboduck modules.</td>
       <td>420</td>
       <td>2023-05-27 21:32:29</td>
       <td>15.14 kb</td>
```

### Comparing `roboduck-0.4.0/roboduck/__init__.py` & `roboduck-0.4.1/roboduck/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from roboduck.debug import duck, DuckDB, CodeCompletionCache
 from roboduck.langchain.chat import Chat, DummyChatModel
 from roboduck.config import update_config, load_config, set_openai_api_key
 from roboduck.ipy_utils import is_colab
 from roboduck.utils import available_models
 
 
-__version__ = '0.4.0'
+__version__ = '0.4.1'
 set_openai_api_key()
 if is_colab():
     warnings.warn(
         'It looks like you\'re using Google Colab, which may make your '
         'roboduck experience slightly sub-optimal (e.g. typing can be a bit '
         'laggy).'
     )
```

### Comparing `roboduck-0.4.0/roboduck/cli/cli.py` & `roboduck-0.4.1/roboduck/cli/cli.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.0/roboduck/config.py` & `roboduck-0.4.1/roboduck/config.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.0/roboduck/debug.py` & `roboduck-0.4.1/roboduck/debug.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.0/roboduck/decorators.py` & `roboduck-0.4.1/roboduck/decorators.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.0/roboduck/errors.py` & `roboduck-0.4.1/roboduck/errors.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.0/roboduck/ipy_utils.py` & `roboduck-0.4.1/roboduck/ipy_utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.0/roboduck/langchain/callbacks.py` & `roboduck-0.4.1/roboduck/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.0/roboduck/langchain/chat.py` & `roboduck-0.4.1/roboduck/langchain/chat.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.0/roboduck/langchain/utils.py` & `roboduck-0.4.1/roboduck/langchain/utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.0/roboduck/logging.py` & `roboduck-0.4.1/roboduck/logging.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.0/roboduck/magic.py` & `roboduck-0.4.1/roboduck/magic.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.0/roboduck/prompts/chat/__template__.yaml` & `roboduck-0.4.1/roboduck/prompts/chat/__template__.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.0/roboduck/prompts/chat/debug.yaml` & `roboduck-0.4.1/roboduck/prompts/chat/debug.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.0/roboduck/prompts/chat/debug_full.yaml` & `roboduck-0.4.1/roboduck/prompts/chat/debug_full.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.0/roboduck/prompts/chat/debug_full_stack_trace.yaml` & `roboduck-0.4.1/roboduck/prompts/chat/debug_full_stack_trace.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.0/roboduck/prompts/chat/debug_stack_trace.yaml` & `roboduck-0.4.1/roboduck/prompts/chat/debug_stack_trace.yaml`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.0/roboduck/prompts/utils.py` & `roboduck-0.4.1/roboduck/prompts/utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.0/roboduck/utils.py` & `roboduck-0.4.1/roboduck/utils.py`

 * *Files identical despite different names*

### Comparing `roboduck-0.4.0/roboduck.egg-info/PKG-INFO` & `roboduck-0.4.1/roboduck.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: roboduck
-Version: 0.4.0
+Version: 0.4.1
 Summary: A natural language debugger.
 Author: Harrison Mamin
 Author-email: harrisonmamin@gmail.com
 License: UNKNOWN
+Project-URL: Documentation, https://hdmamin.github.io/roboduck/
+Project-URL: Repository, https://github.com/hdmamin/roboduck
+Keywords: debugging,llm,language model,dev tools,errors,jupyter magic
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/hdmamin/roboduck/main/data/images/roboduck_blue_banner.png" alt="roboduck logo">
 <p></p>
 <a href="https://hdmamin.github.io/roboduck/"><img src="https://img.shields.io/badge/Documentation-Online-blue.svg" alt="Documentation"></a>
@@ -143,15 +146,15 @@
 
 To rebuild the docs locally:
 ```
 make docs
 ```
 
 ---
-Start of auto-generated file data.<br/>Last updated: 2023-05-29 14:50:53
+Start of auto-generated file data.<br/>Last updated: 2023-06-02 21:08:08
 
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th>File</th>
       <th>Summary</th>
       <th>Line Count</th>
@@ -160,65 +163,65 @@
     </tr>
   </thead>
   <tbody>
     <tr>
       <td>__init__.py</td>
       <td>_</td>
       <td>17</td>
-      <td>2023-05-26 21:33:35</td>
+      <td>2023-06-01 23:26:46</td>
       <td>548.00 b</td>
     </tr>
     <tr>
       <td>config.py</td>
       <td>Allow us to easily read from and write to roboduck's config file.<br/><br/>Roboduck creates a config file at `~/.roboduck/config.yaml`. This currently<br/>supports only two fields:<br/><br/>- `openai_api_key`: See the [Quickstart](https://hdmamin.github.io/roboduck/)<br/>for setup help.<br/><br/>- `model_name` (optional): Roboduck is configured to use gpt-3.5-turbo by<br/>default. This field lets you change that (e.g. to gpt-4). If present in the<br/>config file, this will take priority over any model_name field specified in a<br/>chat template<br/>(e.g. our [default debug prompt template](https://github.com/hdmamin/roboduck/blob/7ff904972921fd3f82b8b9fd862c4ffc7b61aee4/lib/roboduck/prompts/chat/debug.yaml#L2)).<br/>You can view valid options with `roboduck.available_models()`.<br/>You can still override the config default by manually passing a value into a<br/>function, e.g. `duck(model_name='gpt-4-32k')`.<br/><br/>You can manually edit your config file or use a command like<br/>`roboduck.update_config(model_name='gpt-4')`. Passing in a value of None<br/>(e.g. `roboduck.update_config(model_name=None)`) will delete that field from<br/>your config file.</td>
       <td>181</td>
       <td>2023-05-23 22:09:40</td>
       <td>7.41 kb</td>
     </tr>
     <tr>
       <td>debug.py</td>
       <td>A conversational debugger and drop-in replacement for pdb. Python's default<br/>interactive debugging session is already a crude conversation with your<br/>program or interpreter, in a sense - this just lets your program communicate to<br/>you more effectively.<br/><br/>Quickstart<br/>----------<br/>Here's a broken version of bubble sort that places a `duck()` call on the<br/>second to last line where you might normally call `breakpoint()`.<br/><br/>```<br/>from roboduck import duck<br/><br/>def bubble_sort(nums):<br/>    for i in range(len(nums)):<br/>        for j in range(len(nums) - 1):<br/>            if nums[j] &gt; nums[j + 1]:<br/>                nums[j + 1] = nums[j]<br/>                nums[j] = nums[j + 1]<br/>                duck()   # &lt;--------------------------- instead of breakpoint()<br/>    return nums<br/><br/>nums = [3, 1, 9, 2, 1]<br/>bubble_sort(nums)<br/>```</td>
-      <td>486</td>
-      <td>2023-05-25 22:14:45</td>
-      <td>20.18 kb</td>
+      <td>571</td>
+      <td>2023-05-31 00:16:13</td>
+      <td>22.98 kb</td>
     </tr>
     <tr>
       <td>decorators.py</td>
       <td>Miscellaneous decorators used throughout the library.</td>
-      <td>287</td>
-      <td>2023-05-21 22:59:59</td>
-      <td>10.26 kb</td>
+      <td>305</td>
+      <td>2023-05-29 15:21:23</td>
+      <td>10.86 kb</td>
     </tr>
     <tr>
       <td>errors.py</td>
       <td>Errors that explain themselves! Or more precisely, errors that are explained<br/>to you by a gpt-esque model. Simply importing this module will change python's<br/>default behavior when it encounters an error.<br/><br/>Quickstart<br/>----------<br/>Importing the errors module automatically enables optional error explanations.<br/>`disable()` reverts to python's regular behavior on errors. `enable()` can be<br/>used to re-enable error explanations or to change settings. For example,<br/>setting auto=True automatically explains all errors rather than asking the user<br/>if they want an explanation (y/n) when an error occurs.<br/>```<br/>from roboduck import errors<br/><br/>data = {'x': 0}<br/>y = data.x<br/><br/>errors.disable()<br/>y = data.x<br/><br/>errors.enable(auto=True)<br/>y = data.x<br/>```</td>
-      <td>276</td>
-      <td>2023-05-28 21:41:30</td>
-      <td>11.35 kb</td>
+      <td>279</td>
+      <td>2023-05-29 16:15:02</td>
+      <td>11.44 kb</td>
     </tr>
     <tr>
       <td>ipy_utils.py</td>
       <td>Functions related to loading, saving, or otherwise working with ipython<br/>sessions or jupyter notebooks.</td>
       <td>186</td>
       <td>2023-05-24 21:37:48</td>
       <td>5.70 kb</td>
     </tr>
     <tr>
       <td>logging.py</td>
       <td>Logger that attempts to diagnose and propose a solution for any errors it<br/>is asked to log. Unlike our debugger and errors modules, explanations are<br/>not streamed because the intended use case is not focused on live development.<br/><br/>Quickstart<br/>----------<br/>```<br/>from roboduck import logging<br/><br/>logger = logging.getLogger(path='/tmp/log.txt')<br/>data = {'x': 0}<br/>try:<br/>    x = data.x<br/>except Exception as e:<br/>    logger.error(e)<br/>```</td>
-      <td>157</td>
-      <td>2023-05-18 22:25:48</td>
-      <td>6.28 kb</td>
+      <td>158</td>
+      <td>2023-05-29 16:15:02</td>
+      <td>6.33 kb</td>
     </tr>
     <tr>
       <td>magic.py</td>
       <td>GPT-powered rough equivalent of the `%debug` Jupyter magic. After an error<br/>occurs, just run %duck in the next cell to get an explanation. This is very<br/>similar to using the errors module, but is less intrusive - you only call it<br/>when you want an explanation, rather than having to type y/n after each error.<br/>We also provide `paste` mode, which attempts to paste a solution into a new<br/>code cell below, and `interactive` mode, which throws you into a conversational<br/>debugging session (technically closer to the original `%debug` magic<br/>functionality.<br/><br/>Quickstart<br/>----------<br/>```<br/># cell 1<br/>from roboduck import magic<br/><br/>nums = [1, 2, 3]<br/>nums.add(4)<br/>```<br/><br/>```<br/># cell 2<br/>%duck<br/>```</td>
-      <td>126</td>
-      <td>2023-05-28 21:41:30</td>
-      <td>5.11 kb</td>
+      <td>127</td>
+      <td>2023-05-30 22:28:43</td>
+      <td>5.18 kb</td>
     </tr>
     <tr>
       <td>utils.py</td>
       <td>Utility functions used by other roboduck modules.</td>
       <td>420</td>
       <td>2023-05-27 21:32:29</td>
       <td>15.14 kb</td>
```

### Comparing `roboduck-0.4.0/roboduck.egg-info/SOURCES.txt` & `roboduck-0.4.1/roboduck.egg-info/SOURCES.txt`

 * *Files identical despite different names*

