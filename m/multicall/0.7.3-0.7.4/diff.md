# Comparing `tmp/multicall-0.7.3.tar.gz` & `tmp/multicall-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicall-0.7.3.tar", max compression
+gzip compressed data, was "multicall-0.7.4.tar", max compression
```

## Comparing `multicall-0.7.3.tar` & `multicall-0.7.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      116 2022-09-24 21:37:51.678438 multicall-0.7.3/multicall/__init__.py
--rw-r--r--   0        0        0     4884 2023-04-21 01:32:54.180157 multicall-0.7.3/multicall/call.py
--rw-r--r--   0        0        0    21026 2023-04-21 01:26:37.041976 multicall-0.7.3/multicall/constants.py
--rw-r--r--   0        0        0       54 2022-09-24 21:37:51.678438 multicall-0.7.3/multicall/exceptions.py
--rw-r--r--   0        0        0      267 2022-09-24 21:37:51.678438 multicall-0.7.3/multicall/loggers.py
--rw-r--r--   0        0        0     8331 2023-04-21 01:33:04.472591 multicall-0.7.3/multicall/multicall.py
--rw-r--r--   0        0        0     2490 2023-04-21 01:26:37.041976 multicall-0.7.3/multicall/signature.py
--rw-r--r--   0        0        0     3116 2023-02-03 17:57:14.581595 multicall-0.7.3/multicall/utils.py
--rw-r--r--   0        0        0      624 2023-04-21 01:33:56.926764 multicall-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 multicall-0.7.3/setup.py
--rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 multicall-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0      116 2022-09-24 21:37:51.678438 multicall-0.7.4/multicall/__init__.py
+-rw-r--r--   0        0        0     4884 2023-06-02 21:58:45.142203 multicall-0.7.4/multicall/call.py
+-rw-r--r--   0        0        0    21026 2023-06-02 21:58:45.142203 multicall-0.7.4/multicall/constants.py
+-rw-r--r--   0        0        0       54 2022-09-24 21:37:51.678438 multicall-0.7.4/multicall/exceptions.py
+-rw-r--r--   0        0        0      267 2022-09-24 21:37:51.678438 multicall-0.7.4/multicall/loggers.py
+-rw-r--r--   0        0        0     8331 2023-06-02 21:58:45.142203 multicall-0.7.4/multicall/multicall.py
+-rw-r--r--   0        0        0     2490 2023-06-02 21:58:45.142203 multicall-0.7.4/multicall/signature.py
+-rw-r--r--   0        0        0     3165 2023-06-02 21:58:45.142203 multicall-0.7.4/multicall/utils.py
+-rw-r--r--   0        0        0      624 2023-06-02 21:59:22.810828 multicall-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 multicall-0.7.4/setup.py
+-rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 multicall-0.7.4/PKG-INFO
```

### Comparing `multicall-0.7.3/multicall/call.py` & `multicall-0.7.4/multicall/call.py`

 * *Files identical despite different names*

### Comparing `multicall-0.7.3/multicall/constants.py` & `multicall-0.7.4/multicall/constants.py`

 * *Files identical despite different names*

### Comparing `multicall-0.7.3/multicall/multicall.py` & `multicall-0.7.4/multicall/multicall.py`

 * *Files identical despite different names*

### Comparing `multicall-0.7.3/multicall/signature.py` & `multicall-0.7.4/multicall/signature.py`

 * *Files identical despite different names*

### Comparing `multicall-0.7.3/multicall/utils.py` & `multicall-0.7.4/multicall/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,21 +55,23 @@
         # with incompatible synchronous middlewares by default.
         middlewares=[],
     )
     async_w3.eth = AsyncEth(async_w3)
     async_w3s[w3] = async_w3
     return async_w3
 
-def get_event_loop() -> asyncio.AbstractEventLoop:
+def get_event_loop() -> asyncio.BaseEventLoop:
     try:
-        return asyncio.get_event_loop()
+        loop = asyncio.get_event_loop()
     except RuntimeError as e: # Necessary for use with multi-threaded applications.
         if not str(e).startswith("There is no current event loop in thread"):
             raise e
-        return asyncio.new_event_loop()
+        loop = asyncio.new_event_loop()
+        asyncio.set_event_loop(loop)
+    return loop
 
 def await_awaitable(awaitable: Awaitable) -> Any:
     return get_event_loop().run_until_complete(awaitable)
 
 async def run_in_subprocess(callable: Callable, *args: Any, **kwargs) -> Any:
     if NUM_PROCESSES == 1:
         return callable(*args, **kwargs)
```

### Comparing `multicall-0.7.3/pyproject.toml` & `multicall-0.7.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multicall"
-version = "0.7.3"
+version = "0.7.4"
 description = "aggregate results from multiple ethereum contract calls"
 authors = ["banteg"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 # These web3.py versions have a busted async provider and cannot be used in any multithreaded applications
 web3 = "^5.27,!=5.29.*,!=5.30.*,!=5.31.0,!=5.31.1,!=5.31.2"
```

### Comparing `multicall-0.7.3/setup.py` & `multicall-0.7.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 install_requires = \
 ['eth_retry>=0.1.8,<0.2.0',
  'web3>=5.27,<6.0,!=5.29.*,!=5.30.*,!=5.31.0,!=5.31.1,!=5.31.2']
 
 setup_kwargs = {
     'name': 'multicall',
-    'version': '0.7.3',
+    'version': '0.7.4',
     'description': 'aggregate results from multiple ethereum contract calls',
     'long_description': 'None',
     'author': 'banteg',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

