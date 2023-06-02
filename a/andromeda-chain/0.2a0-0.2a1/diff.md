# Comparing `tmp/andromeda-chain-0.2a0.tar.gz` & `tmp/andromeda-chain-0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "andromeda-chain-0.2a0.tar", last modified: Fri Jun  2 22:24:40 2023, max compression
+gzip compressed data, was "andromeda-chain-0.2a1.tar", last modified: Fri Jun  2 22:33:19 2023, max compression
```

## Comparing `andromeda-chain-0.2a0.tar` & `andromeda-chain-0.2a1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 paolo     (1000) paolo     (1000)        0 2023-06-02 22:24:40.667373 andromeda-chain-0.2a0/
--rw-rw-r--   0 paolo     (1000) paolo     (1000)     1064 2023-06-02 20:56:27.000000 andromeda-chain-0.2a0/LICENSE
--rw-rw-r--   0 paolo     (1000) paolo     (1000)      900 2023-06-02 22:24:40.667373 andromeda-chain-0.2a0/PKG-INFO
--rw-rw-r--   0 paolo     (1000) paolo     (1000)     1680 2023-06-02 21:57:21.000000 andromeda-chain-0.2a0/README.md
--rw-rw-r--   0 paolo     (1000) paolo     (1000)       38 2023-06-02 22:24:40.667373 andromeda-chain-0.2a0/setup.cfg
--rw-rw-r--   0 paolo     (1000) paolo     (1000)     1513 2023-06-02 22:08:00.000000 andromeda-chain-0.2a0/setup.py
-drwxrwxr-x   0 paolo     (1000) paolo     (1000)        0 2023-06-02 22:24:40.667373 andromeda-chain-0.2a0/src/
-drwxrwxr-x   0 paolo     (1000) paolo     (1000)        0 2023-06-02 22:24:40.667373 andromeda-chain-0.2a0/src/andromeda_chain/
--rw-rw-r--   0 paolo     (1000) paolo     (1000)      165 2023-06-02 22:23:30.000000 andromeda-chain-0.2a0/src/andromeda_chain/__init__.py
--rw-rw-r--   0 paolo     (1000) paolo     (1000)     3345 2023-06-02 22:23:30.000000 andromeda-chain-0.2a0/src/andromeda_chain/andromeda_chain.py
--rw-rw-r--   0 paolo     (1000) paolo     (1000)      353 2023-06-02 22:23:29.000000 andromeda-chain-0.2a0/src/andromeda_chain/prompt.py
--rw-rw-r--   0 paolo     (1000) paolo     (1000)      157 2023-06-02 22:23:30.000000 andromeda-chain-0.2a0/src/andromeda_chain/response.py
--rw-rw-r--   0 paolo     (1000) paolo     (1000)       21 2023-06-02 22:23:30.000000 andromeda-chain-0.2a0/src/andromeda_chain/version.py
-drwxrwxr-x   0 paolo     (1000) paolo     (1000)        0 2023-06-02 22:24:40.667373 andromeda-chain-0.2a0/src/andromeda_chain.egg-info/
--rw-rw-r--   0 paolo     (1000) paolo     (1000)      900 2023-06-02 22:24:40.000000 andromeda-chain-0.2a0/src/andromeda_chain.egg-info/PKG-INFO
--rw-rw-r--   0 paolo     (1000) paolo     (1000)      428 2023-06-02 22:24:40.000000 andromeda-chain-0.2a0/src/andromeda_chain.egg-info/SOURCES.txt
--rw-rw-r--   0 paolo     (1000) paolo     (1000)        1 2023-06-02 22:24:40.000000 andromeda-chain-0.2a0/src/andromeda_chain.egg-info/dependency_links.txt
--rw-rw-r--   0 paolo     (1000) paolo     (1000)        9 2023-06-02 22:24:40.000000 andromeda-chain-0.2a0/src/andromeda_chain.egg-info/requires.txt
--rw-rw-r--   0 paolo     (1000) paolo     (1000)       16 2023-06-02 22:24:40.000000 andromeda-chain-0.2a0/src/andromeda_chain.egg-info/top_level.txt
-drwxrwxr-x   0 paolo     (1000) paolo     (1000)        0 2023-06-02 22:24:40.667373 andromeda-chain-0.2a0/tests/
--rw-rw-r--   0 paolo     (1000) paolo     (1000)      166 2023-06-02 22:19:36.000000 andromeda-chain-0.2a0/tests/test_andromeda.py
+drwxrwxr-x   0 paolo     (1000) paolo     (1000)        0 2023-06-02 22:33:19.270066 andromeda-chain-0.2a1/
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)     1064 2023-06-02 20:56:27.000000 andromeda-chain-0.2a1/LICENSE
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)      900 2023-06-02 22:33:19.270066 andromeda-chain-0.2a1/PKG-INFO
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)     1680 2023-06-02 21:57:21.000000 andromeda-chain-0.2a1/README.md
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)       38 2023-06-02 22:33:19.270066 andromeda-chain-0.2a1/setup.cfg
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)     1513 2023-06-02 22:08:00.000000 andromeda-chain-0.2a1/setup.py
+drwxrwxr-x   0 paolo     (1000) paolo     (1000)        0 2023-06-02 22:33:19.270066 andromeda-chain-0.2a1/src/
+drwxrwxr-x   0 paolo     (1000) paolo     (1000)        0 2023-06-02 22:33:19.270066 andromeda-chain-0.2a1/src/andromeda_chain/
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)      165 2023-06-02 22:23:30.000000 andromeda-chain-0.2a1/src/andromeda_chain/__init__.py
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)     3464 2023-06-02 22:32:45.000000 andromeda-chain-0.2a1/src/andromeda_chain/andromeda_chain.py
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)      353 2023-06-02 22:23:29.000000 andromeda-chain-0.2a1/src/andromeda_chain/prompt.py
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)      157 2023-06-02 22:23:30.000000 andromeda-chain-0.2a1/src/andromeda_chain/response.py
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)       22 2023-06-02 22:33:12.000000 andromeda-chain-0.2a1/src/andromeda_chain/version.py
+drwxrwxr-x   0 paolo     (1000) paolo     (1000)        0 2023-06-02 22:33:19.270066 andromeda-chain-0.2a1/src/andromeda_chain.egg-info/
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)      900 2023-06-02 22:33:19.000000 andromeda-chain-0.2a1/src/andromeda_chain.egg-info/PKG-INFO
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)      428 2023-06-02 22:33:19.000000 andromeda-chain-0.2a1/src/andromeda_chain.egg-info/SOURCES.txt
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)        1 2023-06-02 22:33:19.000000 andromeda-chain-0.2a1/src/andromeda_chain.egg-info/dependency_links.txt
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)        9 2023-06-02 22:33:19.000000 andromeda-chain-0.2a1/src/andromeda_chain.egg-info/requires.txt
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)       16 2023-06-02 22:33:19.000000 andromeda-chain-0.2a1/src/andromeda_chain.egg-info/top_level.txt
+drwxrwxr-x   0 paolo     (1000) paolo     (1000)        0 2023-06-02 22:33:19.270066 andromeda-chain-0.2a1/tests/
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)      779 2023-06-02 22:31:33.000000 andromeda-chain-0.2a1/tests/test_andromeda.py
```

### Comparing `andromeda-chain-0.2a0/LICENSE` & `andromeda-chain-0.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `andromeda-chain-0.2a0/PKG-INFO` & `andromeda-chain-0.2a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andromeda-chain
-Version: 0.2a0
+Version: 0.2a1
 Summary: A client to query a HTTP Guidance server
 Home-page: https://github.com/ChuloAI/andromeda-chain
 Author: Paolo Rechia
 Author-email: paolorechia@gmail.com
 Maintainer: Paolo Rechia
 Maintainer-email: paolorechia@gmail.com
 License: MIT
```

### Comparing `andromeda-chain-0.2a0/README.md` & `andromeda-chain-0.2a1/README.md`

 * *Files identical despite different names*

### Comparing `andromeda-chain-0.2a0/setup.py` & `andromeda-chain-0.2a1/setup.py`

 * *Files identical despite different names*

### Comparing `andromeda-chain-0.2a0/src/andromeda_chain/andromeda_chain.py` & `andromeda-chain-0.2a1/src/andromeda_chain/andromeda_chain.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 class AndromedaChain:
     def __init__(self, guidance_url: str = "http://0.0.0.0:9000") -> None:
         self._guidance_url = guidance_url
 
     def run_guidance_prompt(
         self,
         guidance_prompt: AndromedaPrompt,
-        input_vars: Dict[str, str],
+        input_vars: Optional[Dict[str, str]] = None,
         macro_values: Optional[dict] = None,
     ) -> AndromedaResponse:
         """Interprets the guidance prompt using a guidance server
 
         Also expands macro calls.
 
         Parameters:
             guidance_prompt (GuidancePrompt): The prompt template to use for the guidance.
-            input_vars (Dict[str, str]): The input variables to use for the guidance.
+            input_vars (Optional[Dict[str, str]]): The input variables to use for the guidance.
             macro_values (Optional[dict]): Macro values to be expanded. Not all prompts need this.
 
         Returns:
             GuidanceResponse: The response from the guidance server
 
         """
         # Macro variables are generaly currently not necessary
@@ -43,14 +43,18 @@
                 prompt_str = prompt_str.replace(macro_identifier, str(value))
 
         if macro_vars:
             raise TypeError(
                 "Unexpanded macro variables in prompt! Fix your prompt or pass the macro variable"
             )
 
+        # Avoid passing null to API
+        if not input_vars:
+            input_vars = {}
+
         result = self._call_guidance(
             prompt_template=prompt_str,
             input_vars=input_vars,
             output_vars=guidance_prompt.output_vars,
             guidance_kwargs=guidance_prompt.guidance_kwargs,
         )
         expanded_generation = result.pop("__main__")
```

### Comparing `andromeda-chain-0.2a0/src/andromeda_chain.egg-info/PKG-INFO` & `andromeda-chain-0.2a1/src/andromeda_chain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andromeda-chain
-Version: 0.2a0
+Version: 0.2a1
 Summary: A client to query a HTTP Guidance server
 Home-page: https://github.com/ChuloAI/andromeda-chain
 Author: Paolo Rechia
 Author-email: paolorechia@gmail.com
 Maintainer: Paolo Rechia
 Maintainer-email: paolorechia@gmail.com
 License: MIT
```

