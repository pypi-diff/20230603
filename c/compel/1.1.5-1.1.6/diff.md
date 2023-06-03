# Comparing `tmp/compel-1.1.5.tar.gz` & `tmp/compel-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-orkrwdod/compel-1.1.5.tar", last modified: Sun May  7 18:32:13 2023, max compression
+gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-u_y8cts3/compel-1.1.6.tar", last modified: Sat Jun  3 06:59:16 2023, max compression
```

## Comparing `compel-1.1.5.tar` & `compel-1.1.6.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-07 18:32:13.000000 compel-1.1.5/
--rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-1.1.5/LICENSE
--rw-r--r--   0 damian     (501) staff       (20)     7286 2023-05-07 18:32:13.000000 compel-1.1.5/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)     6708 2023-05-07 18:31:45.000000 compel-1.1.5/README.md
--rw-r--r--   0 damian     (501) staff       (20)      761 2023-05-07 18:28:05.000000 compel-1.1.5/pyproject.toml
--rw-r--r--   0 damian     (501) staff       (20)       38 2023-05-07 18:32:13.000000 compel-1.1.5/setup.cfg
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-07 18:32:13.000000 compel-1.1.5/src/
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-07 18:32:13.000000 compel-1.1.5/src/compel/
--rw-r--r--   0 damian     (501) staff       (20)      124 2023-01-26 00:22:00.000000 compel-1.1.5/src/compel/__init__.py
--rw-r--r--   0 damian     (501) staff       (20)    14678 2023-05-07 07:42:07.000000 compel-1.1.5/src/compel/compel.py
--rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-1.1.5/src/compel/conditioning_scheduler.py
--rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-1.1.5/src/compel/cross_attention_control.py
--rw-r--r--   0 damian     (501) staff       (20)    25187 2023-05-07 07:42:07.000000 compel-1.1.5/src/compel/embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    29813 2023-05-07 18:26:04.000000 compel-1.1.5/src/compel/prompt_parser.py
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-07 18:32:13.000000 compel-1.1.5/src/compel.egg-info/
--rw-r--r--   0 damian     (501) staff       (20)     7286 2023-05-07 18:32:13.000000 compel-1.1.5/src/compel.egg-info/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)      462 2023-05-07 18:32:13.000000 compel-1.1.5/src/compel.egg-info/SOURCES.txt
--rw-r--r--   0 damian     (501) staff       (20)        1 2023-05-07 18:32:13.000000 compel-1.1.5/src/compel.egg-info/dependency_links.txt
--rw-r--r--   0 damian     (501) staff       (20)       56 2023-05-07 18:32:13.000000 compel-1.1.5/src/compel.egg-info/requires.txt
--rw-r--r--   0 damian     (501) staff       (20)        7 2023-05-07 18:32:13.000000 compel-1.1.5/src/compel.egg-info/top_level.txt
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-05-07 18:32:13.000000 compel-1.1.5/test/
--rw-r--r--   0 damian     (501) staff       (20)    14454 2023-05-07 07:40:27.000000 compel-1.1.5/test/test_compel.py
--rw-r--r--   0 damian     (501) staff       (20)    21072 2023-04-30 12:11:27.000000 compel-1.1.5/test/test_embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    47329 2023-05-07 18:27:10.000000 compel-1.1.5/test/test_prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-03 06:59:16.000000 compel-1.1.6/
+-rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-1.1.6/LICENSE
+-rw-r--r--   0 damian     (501) staff       (20)     8547 2023-06-03 06:59:16.000000 compel-1.1.6/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)     7969 2023-06-03 06:58:01.000000 compel-1.1.6/README.md
+-rw-r--r--   0 damian     (501) staff       (20)      761 2023-06-03 06:58:48.000000 compel-1.1.6/pyproject.toml
+-rw-r--r--   0 damian     (501) staff       (20)       38 2023-06-03 06:59:16.000000 compel-1.1.6/setup.cfg
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-03 06:59:16.000000 compel-1.1.6/src/
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-03 06:59:16.000000 compel-1.1.6/src/compel/
+-rw-r--r--   0 damian     (501) staff       (20)      175 2023-06-03 06:15:19.000000 compel-1.1.6/src/compel/__init__.py
+-rw-r--r--   0 damian     (501) staff       (20)    14772 2023-06-03 06:27:49.000000 compel-1.1.6/src/compel/compel.py
+-rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-1.1.6/src/compel/conditioning_scheduler.py
+-rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-1.1.6/src/compel/cross_attention_control.py
+-rw-r--r--   0 damian     (501) staff       (20)      653 2023-06-03 06:15:19.000000 compel-1.1.6/src/compel/diffusers_textual_inversion_manager.py
+-rw-r--r--   0 damian     (501) staff       (20)    25187 2023-06-03 06:15:11.000000 compel-1.1.6/src/compel/embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    29912 2023-06-03 06:55:13.000000 compel-1.1.6/src/compel/prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-03 06:59:16.000000 compel-1.1.6/src/compel.egg-info/
+-rw-r--r--   0 damian     (501) staff       (20)     8547 2023-06-03 06:59:16.000000 compel-1.1.6/src/compel.egg-info/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)      512 2023-06-03 06:59:16.000000 compel-1.1.6/src/compel.egg-info/SOURCES.txt
+-rw-r--r--   0 damian     (501) staff       (20)        1 2023-06-03 06:59:16.000000 compel-1.1.6/src/compel.egg-info/dependency_links.txt
+-rw-r--r--   0 damian     (501) staff       (20)       56 2023-06-03 06:59:16.000000 compel-1.1.6/src/compel.egg-info/requires.txt
+-rw-r--r--   0 damian     (501) staff       (20)        7 2023-06-03 06:59:16.000000 compel-1.1.6/src/compel.egg-info/top_level.txt
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-03 06:59:16.000000 compel-1.1.6/test/
+-rw-r--r--   0 damian     (501) staff       (20)    14425 2023-06-03 06:37:18.000000 compel-1.1.6/test/test_compel.py
+-rw-r--r--   0 damian     (501) staff       (20)    21072 2023-06-03 06:15:11.000000 compel-1.1.6/test/test_embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    47562 2023-06-03 06:55:54.000000 compel-1.1.6/test/test_prompt_parser.py
```

### Comparing `compel-1.1.5/LICENSE` & `compel-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `compel-1.1.5/PKG-INFO` & `compel-1.1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: compel
-Version: 1.1.5
-Summary: A prompting enhancement library for transformers-type text embedding systems.
-Author-email: Damian Stewart <null@damianstewart.com>
-Project-URL: Homepage, https://github.com/damian0815/compel
-Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Compel
 A text prompt weighting and blending library for transformers-type text embedding systems, by [@damian0815](https://github.com/damian0815).
 
 With a flexible and intuitive syntax, you can re-weight different parts of a prompt string and thus re-weight the different parts of the embeddning tensor produced from the string.
 
 Tested and developed against Hugging Face's `StableDiffusionPipeline` but it should work with any diffusers-based system that uses an `Tokenizer` and a `Text Encoder` of some kind.  
 
@@ -37,15 +23,15 @@
 
 ### Quickstart
 
 with Hugging Face diffusers >=0.12:
 
 ```python
 from diffusers import StableDiffusionPipeline
-from compel import Compel
+from compel import Compel, DiffusersTextualInversionManager
 
 pipeline = StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
 compel = Compel(tokenizer=pipeline.tokenizer, text_encoder=pipeline.text_encoder)
 
 # upweight "ball"
 prompt = "a cat playing with a ball++ in the forest"
 conditioning = compel.build_conditioning_tensor(prompt)
@@ -58,29 +44,53 @@
 
 For batched input, use the __call__ interface to compel:
 
 ```python
 import torch
 
 from diffusers import StableDiffusionPipeline
-from compel import Compel
+from compel import Compel, DiffusersTextualInversionManager
 
 pipeline = StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
 compel = Compel(tokenizer=pipeline.tokenizer, text_encoder=pipeline.text_encoder)
 
 prompts = ["a cat playing with a ball++ in the forest", "a dog playing with a ball in the forest"]
 prompt_embeds = compel(prompts)
 images = pipeline(prompt_embeds=prompt_embeds).images
 
 images[0].save("image0.jpg")
 images[1].save("image1.jpg")
 ```
 
+### Textual Inversion support
+
+If you want to have access to 🤗diffusers textual inversions, instantiate a `DiffusersTextualInversionManager` and pass it on Compel init:
+
+```
+textual_inversion_manager = DiffusersTextualInversionManager(pipeline)
+pipeline = StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
+compel = Compel(tokenizer=pipeline.tokenizer, text_encoder=pipeline.text_encoder, 
+    textual_inversion_manager=textual_inversion_manager)
+```
+
+## Memory usage/VRAM leaks
+
+If you are using Compel heavily and repeatedly, you may run into PyTorch memory issues. To alleviate this, according to @kshieh1: 
+> After image generation, you should explictly de-reference the tensor object (i.e., prompt_embeds = None) and call gc.collect()
+
+See https://github.com/damian0815/compel/issues/24 for more details. Thanks @kshieh1 !
+
 ## Changelog
 
+#### 1.1.6 - misc small fixes
+- add `DiffusersTextualInversionManager` (thanks @pdoane)
+- fix batch embedding generation with truncated/non-truncated prompt lengths (#18, thanks @abassino)
+- add note about memory leakage (ref #24, thanks @kshieh1) 
+- fix incorrect parsing when commas are not followed by whitespace (#34, thanks @moono)
+
 #### 1.1.5 - fix for compel turning numbers into floats for text inside parentheses
 
 #### 1.1.4 - fixes for #23 (sequential offload) and InvokeAI issue #3442 (allow hyphens in LoRA names) 
 
 #### 1.1.3 - enable fetching the penultimate CLIP hidden layer (aka "clip skip")
 
 To use, pass `use_penultimate_clip_layer=True` when initializing your `Compel` instance. Note that there's no need to pass this flag for SD2.0/SD2.1 because diffusers already throws away the last hidden layer when loading the SD2.0+ text encoder.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `compel-1.1.5/pyproject.toml` & `compel-1.1.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "compel"
-version = "1.1.5"
+version = "1.1.6"
 authors = [
   { name="Damian Stewart", email="null@damianstewart.com" },
 ]
 description = "A prompting enhancement library for transformers-type text embedding systems."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `compel-1.1.5/src/compel/compel.py` & `compel-1.1.6/src/compel/compel.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
         if not isinstance(text, list):
             text = [text]
 
         cond_tensor = []
         for text_input in text:
             cond_tensor.append(self.build_conditioning_tensor(text_input))
 
+        cond_tensor = self.pad_conditioning_tensors_to_same_length(conditionings=cond_tensor)
         cond_tensor = torch.cat(cond_tensor)
 
         return cond_tensor
 
     @classmethod
     def parse_prompt_string(cls, prompt_string: str) -> Conjunction:
         pp = PromptParser()
```

### Comparing `compel-1.1.5/src/compel/conditioning_scheduler.py` & `compel-1.1.6/src/compel/conditioning_scheduler.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.5/src/compel/cross_attention_control.py` & `compel-1.1.6/src/compel/cross_attention_control.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.5/src/compel/embeddings_provider.py` & `compel-1.1.6/src/compel/embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.5/src/compel/prompt_parser.py` & `compel-1.1.6/src/compel/prompt_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import string
 from dataclasses import dataclass
 from typing import Union, Optional, List, Tuple
 import pyparsing as pp
+import re
 
 __all__ = ["PromptParser"]
 
 '''
 This module parses prompt strings and produces tree-like structures that can be used generate and control the conditioning tensors.
 weighted subprompts.
 
@@ -303,14 +304,17 @@
     def parse_conjunction(self, prompt: str, verbose: bool=False) -> Conjunction:
         '''
         :param prompt: The prompt string to parse
         :return: a Conjunction representing the parsed results.
         '''
         verbose and print(f"parsing '{prompt}'")
 
+        # enforce whitespace after ,
+        prompt = re.sub(r',(\S)', r', \1', prompt)
+
         if len(prompt.strip()) == 0:
             return Conjunction(prompts=[FlattenedPrompt([('', 1.0)])], weights=[1.0])
 
         root = self.conjunction.parse_string(prompt)
         verbose and print(f"'{prompt}' parsed to root", root)
         #fused = fuse_fragments(parts)
         #print("fused to", fused)
```

### Comparing `compel-1.1.5/src/compel.egg-info/PKG-INFO` & `compel-1.1.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 1.1.5
+Version: 1.1.6
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -37,15 +37,15 @@
 
 ### Quickstart
 
 with Hugging Face diffusers >=0.12:
 
 ```python
 from diffusers import StableDiffusionPipeline
-from compel import Compel
+from compel import Compel, DiffusersTextualInversionManager
 
 pipeline = StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
 compel = Compel(tokenizer=pipeline.tokenizer, text_encoder=pipeline.text_encoder)
 
 # upweight "ball"
 prompt = "a cat playing with a ball++ in the forest"
 conditioning = compel.build_conditioning_tensor(prompt)
@@ -58,29 +58,53 @@
 
 For batched input, use the __call__ interface to compel:
 
 ```python
 import torch
 
 from diffusers import StableDiffusionPipeline
-from compel import Compel
+from compel import Compel, DiffusersTextualInversionManager
 
 pipeline = StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
 compel = Compel(tokenizer=pipeline.tokenizer, text_encoder=pipeline.text_encoder)
 
 prompts = ["a cat playing with a ball++ in the forest", "a dog playing with a ball in the forest"]
 prompt_embeds = compel(prompts)
 images = pipeline(prompt_embeds=prompt_embeds).images
 
 images[0].save("image0.jpg")
 images[1].save("image1.jpg")
 ```
 
+### Textual Inversion support
+
+If you want to have access to 🤗diffusers textual inversions, instantiate a `DiffusersTextualInversionManager` and pass it on Compel init:
+
+```
+textual_inversion_manager = DiffusersTextualInversionManager(pipeline)
+pipeline = StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
+compel = Compel(tokenizer=pipeline.tokenizer, text_encoder=pipeline.text_encoder, 
+    textual_inversion_manager=textual_inversion_manager)
+```
+
+## Memory usage/VRAM leaks
+
+If you are using Compel heavily and repeatedly, you may run into PyTorch memory issues. To alleviate this, according to @kshieh1: 
+> After image generation, you should explictly de-reference the tensor object (i.e., prompt_embeds = None) and call gc.collect()
+
+See https://github.com/damian0815/compel/issues/24 for more details. Thanks @kshieh1 !
+
 ## Changelog
 
+#### 1.1.6 - misc small fixes
+- add `DiffusersTextualInversionManager` (thanks @pdoane)
+- fix batch embedding generation with truncated/non-truncated prompt lengths (#18, thanks @abassino)
+- add note about memory leakage (ref #24, thanks @kshieh1) 
+- fix incorrect parsing when commas are not followed by whitespace (#34, thanks @moono)
+
 #### 1.1.5 - fix for compel turning numbers into floats for text inside parentheses
 
 #### 1.1.4 - fixes for #23 (sequential offload) and InvokeAI issue #3442 (allow hyphens in LoRA names) 
 
 #### 1.1.3 - enable fetching the penultimate CLIP hidden layer (aka "clip skip")
 
 To use, pass `use_penultimate_clip_layer=True` when initializing your `Compel` instance. Note that there's no need to pass this flag for SD2.0/SD2.1 because diffusers already throws away the last hidden layer when loading the SD2.0+ text encoder.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `compel-1.1.5/test/test_compel.py` & `compel-1.1.6/test/test_compel.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,26 +240,21 @@
         self.assertTrue(torch.allclose(expected_positive_conditioning,
                                        conditioning_at_end.positive_conditioning,
                                        atol=1e-6))
         self.assertTrue(torch.allclose(expected_negative_conditioning,
                                        conditioning_at_end.negative_conditioning,
                                        atol=1e-6))
 
-
-
-    def test_long_bad_prompt(self):
+    def test_long_and_short_call(self):
         max_length = 5
         tokenizer = DummyTokenizer(model_max_length=max_length)
         text_encoder = DummyTransformer()
         compel = Compel(tokenizer=tokenizer, text_encoder=text_encoder, truncate_long_prompts=False)
 
-        positive_prompt = "a b c withLora(something)"
-        negative_prompt = '("a b c a b c a b", "c").blend()'
-        positive_conditioning = compel.build_conditioning_tensor(positive_prompt)
-        negative_conditioning = compel.build_conditioning_tensor(negative_prompt)
-
-
-
+        prompts = ["a b c", "a b c a b c a b"]
+        embeds = compel(prompts)
+        # 3*max_length is caused by the need to have eos/bos markers at start and end of each encoded part
+        self.assertTrue(embeds.shape == (2, 3*max_length, 768))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `compel-1.1.5/test/test_embeddings_provider.py` & `compel-1.1.6/test/test_embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.5/test/test_prompt_parser.py` & `compel-1.1.6/test/test_prompt_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -615,9 +615,13 @@
                          parse_prompt("(happy camper:0.3)"))
 
     def test_numbers_to_floats(self):
         self.assertEqual(Conjunction([FlattenedPrompt([("test1 , 1test , test1test", 1.0)])]),
                         parse_prompt("(test1, 1test, test1test)"))
 
 
+    def test_commas_and_whitespace(self):
+        self.assertEqual(Conjunction([FlattenedPrompt([("middle age,", 1.0), ("fantasy", pow(1.1, 2)), ("style", 1)])]),
+                         parse_prompt("middle age,fantasy++ style"))
+
 if __name__ == '__main__':
     unittest.main()
```

