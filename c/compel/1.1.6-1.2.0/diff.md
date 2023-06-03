# Comparing `tmp/compel-1.1.6.tar.gz` & `tmp/compel-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-u_y8cts3/compel-1.1.6.tar", last modified: Sat Jun  3 06:59:16 2023, max compression
+gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-t4pc895k/compel-1.2.0.tar", last modified: Sat Jun  3 18:39:27 2023, max compression
```

## Comparing `compel-1.1.6.tar` & `compel-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-03 06:59:16.000000 compel-1.1.6/
--rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-1.1.6/LICENSE
--rw-r--r--   0 damian     (501) staff       (20)     8547 2023-06-03 06:59:16.000000 compel-1.1.6/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)     7969 2023-06-03 06:58:01.000000 compel-1.1.6/README.md
--rw-r--r--   0 damian     (501) staff       (20)      761 2023-06-03 06:58:48.000000 compel-1.1.6/pyproject.toml
--rw-r--r--   0 damian     (501) staff       (20)       38 2023-06-03 06:59:16.000000 compel-1.1.6/setup.cfg
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-03 06:59:16.000000 compel-1.1.6/src/
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-03 06:59:16.000000 compel-1.1.6/src/compel/
--rw-r--r--   0 damian     (501) staff       (20)      175 2023-06-03 06:15:19.000000 compel-1.1.6/src/compel/__init__.py
--rw-r--r--   0 damian     (501) staff       (20)    14772 2023-06-03 06:27:49.000000 compel-1.1.6/src/compel/compel.py
--rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-1.1.6/src/compel/conditioning_scheduler.py
--rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-1.1.6/src/compel/cross_attention_control.py
--rw-r--r--   0 damian     (501) staff       (20)      653 2023-06-03 06:15:19.000000 compel-1.1.6/src/compel/diffusers_textual_inversion_manager.py
--rw-r--r--   0 damian     (501) staff       (20)    25187 2023-06-03 06:15:11.000000 compel-1.1.6/src/compel/embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    29912 2023-06-03 06:55:13.000000 compel-1.1.6/src/compel/prompt_parser.py
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-03 06:59:16.000000 compel-1.1.6/src/compel.egg-info/
--rw-r--r--   0 damian     (501) staff       (20)     8547 2023-06-03 06:59:16.000000 compel-1.1.6/src/compel.egg-info/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)      512 2023-06-03 06:59:16.000000 compel-1.1.6/src/compel.egg-info/SOURCES.txt
--rw-r--r--   0 damian     (501) staff       (20)        1 2023-06-03 06:59:16.000000 compel-1.1.6/src/compel.egg-info/dependency_links.txt
--rw-r--r--   0 damian     (501) staff       (20)       56 2023-06-03 06:59:16.000000 compel-1.1.6/src/compel.egg-info/requires.txt
--rw-r--r--   0 damian     (501) staff       (20)        7 2023-06-03 06:59:16.000000 compel-1.1.6/src/compel.egg-info/top_level.txt
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-03 06:59:16.000000 compel-1.1.6/test/
--rw-r--r--   0 damian     (501) staff       (20)    14425 2023-06-03 06:37:18.000000 compel-1.1.6/test/test_compel.py
--rw-r--r--   0 damian     (501) staff       (20)    21072 2023-06-03 06:15:11.000000 compel-1.1.6/test/test_embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    47562 2023-06-03 06:55:54.000000 compel-1.1.6/test/test_prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-03 18:39:27.000000 compel-1.2.0/
+-rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-1.2.0/LICENSE
+-rw-r--r--   0 damian     (501) staff       (20)    10987 2023-06-03 18:39:27.000000 compel-1.2.0/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)    10409 2023-06-03 18:38:59.000000 compel-1.2.0/README.md
+-rw-r--r--   0 damian     (501) staff       (20)      761 2023-06-03 18:15:52.000000 compel-1.2.0/pyproject.toml
+-rw-r--r--   0 damian     (501) staff       (20)       38 2023-06-03 18:39:27.000000 compel-1.2.0/setup.cfg
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-03 18:39:27.000000 compel-1.2.0/src/
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-03 18:39:27.000000 compel-1.2.0/src/compel/
+-rw-r--r--   0 damian     (501) staff       (20)      175 2023-06-03 06:15:19.000000 compel-1.2.0/src/compel/__init__.py
+-rw-r--r--   0 damian     (501) staff       (20)    14940 2023-06-03 18:09:49.000000 compel-1.2.0/src/compel/compel.py
+-rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-1.2.0/src/compel/conditioning_scheduler.py
+-rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-1.2.0/src/compel/cross_attention_control.py
+-rw-r--r--   0 damian     (501) staff       (20)      653 2023-06-03 06:15:19.000000 compel-1.2.0/src/compel/diffusers_textual_inversion_manager.py
+-rw-r--r--   0 damian     (501) staff       (20)    25187 2023-06-03 06:15:11.000000 compel-1.2.0/src/compel/embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    29912 2023-06-03 06:55:13.000000 compel-1.2.0/src/compel/prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-03 18:39:27.000000 compel-1.2.0/src/compel.egg-info/
+-rw-r--r--   0 damian     (501) staff       (20)    10987 2023-06-03 18:39:27.000000 compel-1.2.0/src/compel.egg-info/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)      512 2023-06-03 18:39:27.000000 compel-1.2.0/src/compel.egg-info/SOURCES.txt
+-rw-r--r--   0 damian     (501) staff       (20)        1 2023-06-03 18:39:27.000000 compel-1.2.0/src/compel.egg-info/dependency_links.txt
+-rw-r--r--   0 damian     (501) staff       (20)       56 2023-06-03 18:39:27.000000 compel-1.2.0/src/compel.egg-info/requires.txt
+-rw-r--r--   0 damian     (501) staff       (20)        7 2023-06-03 18:39:27.000000 compel-1.2.0/src/compel.egg-info/top_level.txt
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-06-03 18:39:27.000000 compel-1.2.0/test/
+-rw-r--r--   0 damian     (501) staff       (20)    15682 2023-06-03 18:14:58.000000 compel-1.2.0/test/test_compel.py
+-rw-r--r--   0 damian     (501) staff       (20)    21072 2023-06-03 06:15:11.000000 compel-1.2.0/test/test_embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    47562 2023-06-03 06:55:54.000000 compel-1.2.0/test/test_prompt_parser.py
```

### Comparing `compel-1.1.6/LICENSE` & `compel-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `compel-1.1.6/PKG-INFO` & `compel-1.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,11 @@
-Metadata-Version: 2.1
-Name: compel
-Version: 1.1.6
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
 
-With a flexible and intuitive syntax, you can re-weight different parts of a prompt string and thus re-weight the different parts of the embeddning tensor produced from the string.
+With a flexible and intuitive syntax, you can re-weight different parts of a prompt string and thus re-weight the different parts of the embedding tensor produced from the string.
 
 Tested and developed against Hugging Face's `StableDiffusionPipeline` but it should work with any diffusers-based system that uses an `Tokenizer` and a `Text Encoder` of some kind.  
 
 Adapted from the [InvokeAI](https://github.com/invoke-ai) prompting code (also by [@damian0815](https://github.com/damian0815)). For now, the syntax is fully documented [here](Reference.md).
 
 Note that cross-attention control `.swap()` is currently ignored by Compel, but you can use it by calling `build_conditioning_tensor_for_prompt_object()` yourself, and implementing cross-attention control in your diffusion loop.
 
@@ -37,15 +23,15 @@
 
 ### Quickstart
 
 with Hugging Face diffusers >=0.12:
 
 ```python
 from diffusers import StableDiffusionPipeline
-from compel import Compel, DiffusersTextualInversionManager
+from compel import Compel
 
 pipeline = StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
 compel = Compel(tokenizer=pipeline.tokenizer, text_encoder=pipeline.text_encoder)
 
 # upweight "ball"
 prompt = "a cat playing with a ball++ in the forest"
 conditioning = compel.build_conditioning_tensor(prompt)
@@ -55,18 +41,16 @@
 images = pipeline(prompt_embeds=conditioning, num_inference_steps=20).images
 images[0].save("image.jpg")
 ```
 
 For batched input, use the __call__ interface to compel:
 
 ```python
-import torch
-
 from diffusers import StableDiffusionPipeline
-from compel import Compel, DiffusersTextualInversionManager
+from compel import Compel
 
 pipeline = StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
 compel = Compel(tokenizer=pipeline.tokenizer, text_encoder=pipeline.text_encoder)
 
 prompts = ["a cat playing with a ball++ in the forest", "a dog playing with a ball in the forest"]
 prompt_embeds = compel(prompts)
 images = pipeline(prompt_embeds=prompt_embeds).images
@@ -76,29 +60,86 @@
 ```
 
 ### Textual Inversion support
 
 If you want to have access to 🤗diffusers textual inversions, instantiate a `DiffusersTextualInversionManager` and pass it on Compel init:
 
 ```
-textual_inversion_manager = DiffusersTextualInversionManager(pipeline)
 pipeline = StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
+textual_inversion_manager = DiffusersTextualInversionManager(pipeline)
 compel = Compel(tokenizer=pipeline.tokenizer, text_encoder=pipeline.text_encoder, 
     textual_inversion_manager=textual_inversion_manager)
 ```
 
 ## Memory usage/VRAM leaks
 
 If you are using Compel heavily and repeatedly, you may run into PyTorch memory issues. To alleviate this, according to @kshieh1: 
 > After image generation, you should explictly de-reference the tensor object (i.e., prompt_embeds = None) and call gc.collect()
 
 See https://github.com/damian0815/compel/issues/24 for more details. Thanks @kshieh1 !
 
 ## Changelog
 
+### 1.2.0 - Concatenate embeddings using `.and()`
+
+For Stable Diffusion 2.1 I've been experimenting with a new feature: concatenated embeddings. What I noticed, for example, is that for more complex prompts image generation quality becomes wildly better when the prompt is broken into multiple parts and fed to OpenCLIP separately.
+
+TL;DR: you can now experiment with breaking up your prompts into segments, which for SD2.1 appears to improve the generated image. The syntax is `("prompt part 1", "prompt part 2").and()`. You can have more than one part, and you can also weight them, eg `("a man eating an apple", "sitting on the roof of a car", "high quality, trending on artstation, 8K UHD").and(1, 0.5, 0.5)` which will assign weight `1` to `man eating an apple` and `0.5` to `sitting on the roof of a car` and `high quality, trending on artstation, 8K UHD`. 
+
+Here's a nonsense example from the InvokeAI discord #garbage-bin channel, created by gogurt enjoyer's incredible [nightmare prompt generator](https://huggingface.co/cactusfriend/nightmare-invokeai-prompts):
+
+```
+a moist sloppy pindlesackboy sloppy hamblin' bogomadong, Clem Fandango is pissed-off, Wario's Woods in background, making a noise like ga-woink-a
+```
+
+Plugging this straight into SD2.1 we get this, which is really not a good image:
+![](images/000075.6dfd7adf.466129594.png)
+
+However, if the prompt is broken up into chunks and fed into OpenCLIP separately as four separate prompts, and then concatenated:
+
+```
+a moist sloppy pindlesackboy sloppy hamblin' bogomadong
+
+Clem Fandango is pissed-off
+
+Wario's Woods in background
+
+making a noise like ga-woink-a
+```
+
+then output image with the same seed is *so much* better:
+![](images/000076.68b1c320.466129594.png)
+
+In the new `.and()` syntax you would prompt this as follows:
+```
+("a moist sloppy pindlesackboy sloppy hamblin' bogomadong", "Clem Fandango is pissed-off", "Wario's Woods in background", "making a noise like ga-woink-a").and()
+```
+
+The effect can be more or less subtle. Here for example is 
+```
+A dream of a distant galaxy, by Caspar David Friedrich, matte painting, trending on artstation, HQ
+```
+![](images/000129.1b33b559.2793529321.png)
+
+And the same split into two parts:
+```
+A dream of a distant galaxy, by Caspar David Friedrich, matte painting
+
+trending on artstation, HQ
+```
+![](images/000128.b5d5cd62.2793529321.png)
+
+The Compel prompt for this is: 
+```
+("A dream of a distant galaxy, by Caspar David Friedrich, matte painting", "trending on artstation, HQ").and()
+```
+
+
+
+
 #### 1.1.6 - misc small fixes
 - add `DiffusersTextualInversionManager` (thanks @pdoane)
 - fix batch embedding generation with truncated/non-truncated prompt lengths (#18, thanks @abassino)
 - add note about memory leakage (ref #24, thanks @kshieh1) 
 - fix incorrect parsing when commas are not followed by whitespace (#34, thanks @moono)
 
 #### 1.1.5 - fix for compel turning numbers into floats for text inside parentheses
```

### Comparing `compel-1.1.6/pyproject.toml` & `compel-1.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "compel"
-version = "1.1.6"
+version = "1.2.0"
 authors = [
   { name="Damian Stewart", email="null@damianstewart.com" },
 ]
 description = "A prompting enhancement library for transformers-type text embedding systems."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `compel-1.1.6/src/compel/compel.py` & `compel-1.2.0/src/compel/compel.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,19 +72,23 @@
             [positive_conditioning, negative_conditioning]
         )
         return StaticConditioningScheduler(positive_conditioning=positive_conditioning,
                                            negative_conditioning=negative_conditioning)
 
     def build_conditioning_tensor(self, text: str) -> torch.Tensor:
         conjunction = self.parse_prompt_string(text)
-        if len(conjunction.prompts)>1:
-            raise ValueError("Conjunctions of >1 prompt are currently not supported by build_conditioning_tensor()")
-        prompt_object = conjunction.prompts[0]
-        conditioning, _ = self.build_conditioning_tensor_for_prompt_object(prompt_object)
-        return conditioning
+        if len(conjunction.prompts) > 1 and conjunction.type != 'AND':
+            raise ValueError("Only AND conjunctions are supported by build_conditioning_tensor()")
+        # concatenate each prompt in the conjunction (typically there will only be 1)
+        to_concat = []
+        for p in conjunction.prompts:
+            conditioning, _ = self.build_conditioning_tensor_for_prompt_object(p)
+            to_concat.append(conditioning)
+        return torch.concat(to_concat, dim=1)
+
 
     @torch.no_grad()
     def __call__(self, text: Union[str, List[str]]) -> torch.FloatTensor:
         if not isinstance(text, list):
             text = [text]
 
         cond_tensor = []
```

### Comparing `compel-1.1.6/src/compel/conditioning_scheduler.py` & `compel-1.2.0/src/compel/conditioning_scheduler.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.6/src/compel/cross_attention_control.py` & `compel-1.2.0/src/compel/cross_attention_control.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.6/src/compel/diffusers_textual_inversion_manager.py` & `compel-1.2.0/src/compel/diffusers_textual_inversion_manager.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.6/src/compel/embeddings_provider.py` & `compel-1.2.0/src/compel/embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.6/src/compel/prompt_parser.py` & `compel-1.2.0/src/compel/prompt_parser.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.6/src/compel.egg-info/PKG-INFO` & `compel-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 1.1.6
+Version: 1.2.0
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Compel
 A text prompt weighting and blending library for transformers-type text embedding systems, by [@damian0815](https://github.com/damian0815).
 
-With a flexible and intuitive syntax, you can re-weight different parts of a prompt string and thus re-weight the different parts of the embeddning tensor produced from the string.
+With a flexible and intuitive syntax, you can re-weight different parts of a prompt string and thus re-weight the different parts of the embedding tensor produced from the string.
 
 Tested and developed against Hugging Face's `StableDiffusionPipeline` but it should work with any diffusers-based system that uses an `Tokenizer` and a `Text Encoder` of some kind.  
 
 Adapted from the [InvokeAI](https://github.com/invoke-ai) prompting code (also by [@damian0815](https://github.com/damian0815)). For now, the syntax is fully documented [here](Reference.md).
 
 Note that cross-attention control `.swap()` is currently ignored by Compel, but you can use it by calling `build_conditioning_tensor_for_prompt_object()` yourself, and implementing cross-attention control in your diffusion loop.
 
@@ -37,15 +37,15 @@
 
 ### Quickstart
 
 with Hugging Face diffusers >=0.12:
 
 ```python
 from diffusers import StableDiffusionPipeline
-from compel import Compel, DiffusersTextualInversionManager
+from compel import Compel
 
 pipeline = StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
 compel = Compel(tokenizer=pipeline.tokenizer, text_encoder=pipeline.text_encoder)
 
 # upweight "ball"
 prompt = "a cat playing with a ball++ in the forest"
 conditioning = compel.build_conditioning_tensor(prompt)
@@ -55,18 +55,16 @@
 images = pipeline(prompt_embeds=conditioning, num_inference_steps=20).images
 images[0].save("image.jpg")
 ```
 
 For batched input, use the __call__ interface to compel:
 
 ```python
-import torch
-
 from diffusers import StableDiffusionPipeline
-from compel import Compel, DiffusersTextualInversionManager
+from compel import Compel
 
 pipeline = StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
 compel = Compel(tokenizer=pipeline.tokenizer, text_encoder=pipeline.text_encoder)
 
 prompts = ["a cat playing with a ball++ in the forest", "a dog playing with a ball in the forest"]
 prompt_embeds = compel(prompts)
 images = pipeline(prompt_embeds=prompt_embeds).images
@@ -76,29 +74,86 @@
 ```
 
 ### Textual Inversion support
 
 If you want to have access to 🤗diffusers textual inversions, instantiate a `DiffusersTextualInversionManager` and pass it on Compel init:
 
 ```
-textual_inversion_manager = DiffusersTextualInversionManager(pipeline)
 pipeline = StableDiffusionPipeline.from_pretrained("runwayml/stable-diffusion-v1-5")
+textual_inversion_manager = DiffusersTextualInversionManager(pipeline)
 compel = Compel(tokenizer=pipeline.tokenizer, text_encoder=pipeline.text_encoder, 
     textual_inversion_manager=textual_inversion_manager)
 ```
 
 ## Memory usage/VRAM leaks
 
 If you are using Compel heavily and repeatedly, you may run into PyTorch memory issues. To alleviate this, according to @kshieh1: 
 > After image generation, you should explictly de-reference the tensor object (i.e., prompt_embeds = None) and call gc.collect()
 
 See https://github.com/damian0815/compel/issues/24 for more details. Thanks @kshieh1 !
 
 ## Changelog
 
+### 1.2.0 - Concatenate embeddings using `.and()`
+
+For Stable Diffusion 2.1 I've been experimenting with a new feature: concatenated embeddings. What I noticed, for example, is that for more complex prompts image generation quality becomes wildly better when the prompt is broken into multiple parts and fed to OpenCLIP separately.
+
+TL;DR: you can now experiment with breaking up your prompts into segments, which for SD2.1 appears to improve the generated image. The syntax is `("prompt part 1", "prompt part 2").and()`. You can have more than one part, and you can also weight them, eg `("a man eating an apple", "sitting on the roof of a car", "high quality, trending on artstation, 8K UHD").and(1, 0.5, 0.5)` which will assign weight `1` to `man eating an apple` and `0.5` to `sitting on the roof of a car` and `high quality, trending on artstation, 8K UHD`. 
+
+Here's a nonsense example from the InvokeAI discord #garbage-bin channel, created by gogurt enjoyer's incredible [nightmare prompt generator](https://huggingface.co/cactusfriend/nightmare-invokeai-prompts):
+
+```
+a moist sloppy pindlesackboy sloppy hamblin' bogomadong, Clem Fandango is pissed-off, Wario's Woods in background, making a noise like ga-woink-a
+```
+
+Plugging this straight into SD2.1 we get this, which is really not a good image:
+![](images/000075.6dfd7adf.466129594.png)
+
+However, if the prompt is broken up into chunks and fed into OpenCLIP separately as four separate prompts, and then concatenated:
+
+```
+a moist sloppy pindlesackboy sloppy hamblin' bogomadong
+
+Clem Fandango is pissed-off
+
+Wario's Woods in background
+
+making a noise like ga-woink-a
+```
+
+then output image with the same seed is *so much* better:
+![](images/000076.68b1c320.466129594.png)
+
+In the new `.and()` syntax you would prompt this as follows:
+```
+("a moist sloppy pindlesackboy sloppy hamblin' bogomadong", "Clem Fandango is pissed-off", "Wario's Woods in background", "making a noise like ga-woink-a").and()
+```
+
+The effect can be more or less subtle. Here for example is 
+```
+A dream of a distant galaxy, by Caspar David Friedrich, matte painting, trending on artstation, HQ
+```
+![](images/000129.1b33b559.2793529321.png)
+
+And the same split into two parts:
+```
+A dream of a distant galaxy, by Caspar David Friedrich, matte painting
+
+trending on artstation, HQ
+```
+![](images/000128.b5d5cd62.2793529321.png)
+
+The Compel prompt for this is: 
+```
+("A dream of a distant galaxy, by Caspar David Friedrich, matte painting", "trending on artstation, HQ").and()
+```
+
+
+
+
 #### 1.1.6 - misc small fixes
 - add `DiffusersTextualInversionManager` (thanks @pdoane)
 - fix batch embedding generation with truncated/non-truncated prompt lengths (#18, thanks @abassino)
 - add note about memory leakage (ref #24, thanks @kshieh1) 
 - fix incorrect parsing when commas are not followed by whitespace (#34, thanks @moono)
 
 #### 1.1.5 - fix for compel turning numbers into floats for text inside parentheses
```

### Comparing `compel-1.1.6/src/compel.egg-info/SOURCES.txt` & `compel-1.2.0/src/compel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compel-1.1.6/test/test_compel.py` & `compel-1.2.0/test/test_compel.py`

 * *Files 4% similar despite different names*

```diff
@@ -251,10 +251,36 @@
         compel = Compel(tokenizer=tokenizer, text_encoder=text_encoder, truncate_long_prompts=False)
 
         prompts = ["a b c", "a b c a b c a b"]
         embeds = compel(prompts)
         # 3*max_length is caused by the need to have eos/bos markers at start and end of each encoded part
         self.assertTrue(embeds.shape == (2, 3*max_length, 768))
 
+    def test_concat_for_and(self):
+        max_length = 5
+        tokenizer = DummyTokenizer(model_max_length=max_length)
+        text_encoder = DummyTransformer()
+        compel = Compel(tokenizer=tokenizer, text_encoder=text_encoder, truncate_long_prompts=False)
+
+        embeds_separate = compel(['a b c', 'b a'])
+        embeds_concat = compel('("a b c", "b a").and()')
+        self.assertTrue(torch.allclose(embeds_concat, torch.reshape(embeds_separate, [1, 10, 768])))
+
+        embeds_separate = torch.concat([compel('a b c a b c a b c'), compel('b a')], dim=1)
+        embeds_concat = compel('("a b c a b c a b c", "b a").and()')
+        self.assertTrue(torch.allclose(embeds_concat, embeds_separate))
+
+
+        compel = Compel(tokenizer=tokenizer, text_encoder=text_encoder, truncate_long_prompts=True)
+
+        embeds_separate = compel(['a b c', 'b a'])
+        embeds_concat = compel('("a b c", "b a").and()')
+        self.assertTrue(torch.allclose(embeds_concat, torch.reshape(embeds_separate, [1, 10, 768])))
+
+        embeds_separate = torch.concat([compel('a b c a b c a b c'), compel('b a')], dim=1)
+        embeds_concat = compel('("a b c a b c a b c", "b a").and()')
+        self.assertTrue(torch.allclose(embeds_concat, embeds_separate))
+
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `compel-1.1.6/test/test_embeddings_provider.py` & `compel-1.2.0/test/test_embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-1.1.6/test/test_prompt_parser.py` & `compel-1.2.0/test/test_prompt_parser.py`

 * *Files identical despite different names*

