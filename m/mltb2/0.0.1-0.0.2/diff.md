# Comparing `tmp/mltb2-0.0.1.tar.gz` & `tmp/mltb2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltb2-0.0.1.tar", last modified: Sun May 28 18:20:57 2023, max compression
+gzip compressed data, was "mltb2-0.0.2.tar", last modified: Sat Jun  3 05:17:09 2023, max compression
```

## Comparing `mltb2-0.0.1.tar` & `mltb2-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:20:57.203389 mltb2-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-28 18:20:47.000000 mltb2-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-28 18:20:47.000000 mltb2-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-28 18:20:57.203389 mltb2-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-28 18:20:47.000000 mltb2-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:20:57.203389 mltb2-0.0.1/mltb2/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-28 18:20:47.000000 mltb2-0.0.1/mltb2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-28 18:20:47.000000 mltb2-0.0.1/mltb2/optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-28 18:20:47.000000 mltb2-0.0.1/mltb2/somajo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-28 18:20:47.000000 mltb2-0.0.1/mltb2/somajo_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-28 18:20:47.000000 mltb2-0.0.1/mltb2/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:20:57.203389 mltb2-0.0.1/mltb2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-28 18:20:57.000000 mltb2-0.0.1/mltb2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-28 18:20:57.000000 mltb2-0.0.1/mltb2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 18:20:57.000000 mltb2-0.0.1/mltb2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-28 18:20:57.000000 mltb2-0.0.1/mltb2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-28 18:20:57.000000 mltb2-0.0.1/mltb2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-28 18:20:47.000000 mltb2-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-28 18:20:57.203389 mltb2-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-28 18:20:47.000000 mltb2-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:20:57.203389 mltb2-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-28 18:20:47.000000 mltb2-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-28 18:20:47.000000 mltb2-0.0.1/tests/test__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-28 18:20:47.000000 mltb2-0.0.1/tests/test_optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-28 18:20:47.000000 mltb2-0.0.1/tests/test_somajo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-28 18:20:47.000000 mltb2-0.0.1/tests/test_somajo_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-28 18:20:47.000000 mltb2-0.0.1/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:17:09.056301 mltb2-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-03 05:16:55.000000 mltb2-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-03 05:16:55.000000 mltb2-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-03 05:17:09.056301 mltb2-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-03 05:16:55.000000 mltb2-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:17:09.056301 mltb2-0.0.2/mltb2/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-03 05:16:55.000000 mltb2-0.0.2/mltb2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-03 05:16:55.000000 mltb2-0.0.2/mltb2/optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-03 05:16:55.000000 mltb2-0.0.2/mltb2/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-03 05:16:55.000000 mltb2-0.0.2/mltb2/somajo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-03 05:16:55.000000 mltb2-0.0.2/mltb2/somajo_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-03 05:16:55.000000 mltb2-0.0.2/mltb2/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:17:09.056301 mltb2-0.0.2/mltb2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-03 05:17:09.000000 mltb2-0.0.2/mltb2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-03 05:17:09.000000 mltb2-0.0.2/mltb2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 05:17:09.000000 mltb2-0.0.2/mltb2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-03 05:17:09.000000 mltb2-0.0.2/mltb2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 05:17:09.000000 mltb2-0.0.2/mltb2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-03 05:16:55.000000 mltb2-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-03 05:17:09.056301 mltb2-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-03 05:16:55.000000 mltb2-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:17:09.056301 mltb2-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-03 05:16:55.000000 mltb2-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-03 05:16:55.000000 mltb2-0.0.2/tests/test__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-03 05:16:55.000000 mltb2-0.0.2/tests/test_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-03 05:16:55.000000 mltb2-0.0.2/tests/test_somajo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-03 05:16:55.000000 mltb2-0.0.2/tests/test_somajo_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-03 05:16:55.000000 mltb2-0.0.2/tests/test_transformers.py
```

### Comparing `mltb2-0.0.1/LICENSE` & `mltb2-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.1/mltb2/optuna.py` & `mltb2-0.0.2/mltb2/optuna.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,28 +18,27 @@
 
 class SignificanceRepeatedTrainingPruner(BasePruner):
     """Pruner which uses statistical significance as an heuristic for decision-making.
 
     Pruner to use statistical significance to prune repeated trainings like in a cross validation.
     As the test method a t-test is used. Our experiments have shown that an ``aplha`` value
     between 0.3 and 0.4 is reasonable.
+
+    Args:
+        alpha: The alpha level for the statistical significance test.
+            The larger this value is, the more aggressively this pruner works.
+            The smaller this value is, the stronger the statistical difference between the two
+            distributions must be for Optuna to prune.
+            ``alpha`` must be ``0 < alpha < 1``.
+            Our experiments have shown that an ``aplha`` value between 0.3 and 0.4 is reasonable.
+        n_warmup_steps: Pruning is disabled until the trial reaches or exceeds the given number
+            of steps.
     """
 
     def __init__(self, alpha: float = 0.1, n_warmup_steps: int = 4) -> None:
-        """Constructor.
-
-        Args:
-            alpha: The alpha level for the statistical significance test.
-                The larger this value is, the more aggressively this pruner works.
-                The smaller this value is, the stronger the statistical difference between the two
-                distributions must be for Optuna to prune.
-                ``alpha`` must be ``0 < alpha < 1``.
-            n_warmup_steps: Pruning is disabled until the trial reaches or exceeds the given number
-                of steps.
-        """
         # input value check
         if n_warmup_steps < 0:
             raise ValueError(
                 "'n_warmup_steps' must not be negative! n_warmup_steps: {}".format(n_warmup_steps)
             )
         if alpha >= 1:
             raise ValueError("'alpha' must be smaller than 1! {}".format(alpha))
```

### Comparing `mltb2-0.0.1/mltb2/somajo.py` & `mltb2-0.0.2/mltb2/somajo_transformers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,72 @@
 # Copyright (c) 2023 Philip May
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
-"""SoMaJo tools."""
+"""SoMaJo and Transformers tools."""
 
 
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from typing import List
 
-from somajo import SoMaJo
+from tqdm.auto import tqdm
+
+from mltb2.somajo import SoMaJoSentenceSplitter
+from mltb2.transformers import TransformersTokenCounter
 
 
 @dataclass
-class SoMaJoSentenceSplitter:
-    """Use SoMaJo to split text into sentences.
+class TextSplitter:
+    """Split the text into sections with a specified maximum token number.
+
+    Does not divide words, but always whole sentences.
 
     Args:
-        language: The language. ``de_CMC`` for German or ``en_PTB`` for English.
+        max_token: Maximum number of tokens per text section.
+        somajo_sentence_splitter: The sentence splitter to be used.
+        transformers_token_counter: The token counter to be used.
+        show_progress_bar: Show a progressbar during processing.
     """
 
-    language: str
-    somajo: SoMaJo = field(init=False, repr=False)
-
-    def __post_init__(self):
-        """Do post init."""
-        self.somajo = SoMaJo(self.language)
-
-    # see https://github.com/tsproisl/SoMaJo/issues/17
-    @staticmethod
-    def detokenize(tokens) -> str:
-        """Convert SoMaJo tokens to sentence (string)."""
-        result_list = []
-        for token in tokens:
-            if token.original_spelling is not None:
-                result_list.append(token.original_spelling)
-            else:
-                result_list.append(token.text)
-
-            if token.space_after:
-                result_list.append(" ")
-        result = "".join(result_list)
-        result = result.strip()
-        return result
+    max_token: int
+    somajo_sentence_splitter: SoMaJoSentenceSplitter
+    transformers_token_counter: TransformersTokenCounter
+    show_progress_bar: bool = True
 
     def __call__(self, text: str) -> List[str]:
-        """Split the test into a list of sentences."""
-        sentences = self.somajo.tokenize_text([text])
-
-        result = []
+        """Split the text into sections.
 
-        for sentence in sentences:
-            sentence_string = self.detokenize(sentence)
-            result.append(sentence_string)
+        Args:
+            text: The text to be split.
+        Returns:
+            The list of section splits.
+        """
+        sentences = self.somajo_sentence_splitter(text)
+        counts = self.transformers_token_counter(sentences)
+
+        assert len(sentences) == len(counts)  # type: ignore
+
+        result_splits: List[str] = []
+        current_sentences: List[str] = []
+        current_count: int = 0
+        for sentence, count in zip(
+            tqdm(sentences, disable=not self.show_progress_bar), counts  # type: ignore
+        ):
+            if count > self.max_token:
+                raise ValueError("No sentence may be longer than 'max_token'.")
+            if current_count + count <= self.max_token:
+                current_count += count
+                current_sentences.append(sentence)
+            else:
+                result_split = " ".join(current_sentences)
+                result_splits.append(result_split)
+                current_sentences = []
+                current_count = 0
+                current_count += count
+                current_sentences.append(sentence)
+
+        # add the rest
+        if len(current_sentences) > 0:
+            result_split = " ".join(current_sentences)
+            result_splits.append(result_split)
 
-        return result
+        return result_splits
```

### Comparing `mltb2-0.0.1/mltb2/transformers.py` & `mltb2-0.0.2/mltb2/transformers.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,37 +6,53 @@
 
 import os
 from dataclasses import dataclass, field
 from typing import Iterable, List, Union
 
 import sklearn
 import torch
+from tqdm.auto import tqdm
 from transformers import AutoTokenizer
 from transformers.tokenization_utils import PreTrainedTokenizerBase
 
 
 @dataclass
 class TransformersTokenCounter:
-    """Count Transformers tokenizer tokens."""
+    """Count Transformers tokenizer tokens.
+
+    Args:
+        pretrained_model_name_or_path:
+            The *model id* of a tokenizer hosted inside a model repo on huggingface.co or
+            a path to a *directory* containing a tokenizer.
+        show_progress_bar: Show a progressbar during processing.
+    """
 
     pretrained_model_name_or_path: Union[str, os.PathLike]
     tokenizer: PreTrainedTokenizerBase = field(init=False, repr=False)
+    show_progress_bar: bool = True
 
     def __post_init__(self):
         """Do post init."""
         self.tokenizer = AutoTokenizer.from_pretrained(self.pretrained_model_name_or_path)
 
     def __call__(self, text: Union[str, Iterable]) -> Union[int, List[int]]:
-        """Count tokens for text."""
+        """Count tokens for text.
+
+        Args:
+            text: The text for which the tokens are to be counted.
+        Returns:
+            The number of tokens if text was just a ``str``.
+            If text is an ``Iterable`` then a ``list`` of number of tokens.
+        """
         if isinstance(text, str):
             tokenized_text = self.tokenizer.tokenize(text)
             return len(tokenized_text)
         else:
             counts = []
-            for t in text:
+            for t in tqdm(text, disable=not self.show_progress_bar):
                 tokenized_text = self.tokenizer.tokenize(t)
                 counts.append(len(tokenized_text))
             return counts
 
 
 class LabeledDataset(torch.utils.data.Dataset):
     """Dataset with labes."""
```

### Comparing `mltb2-0.0.1/pyproject.toml` & `mltb2-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.black]
 line-length = 99
-target-version = ["py39"]
+target-version = ["py38"]
 
 [tool.isort]
 profile = "black"
 lines_after_imports = 2
 line_length = 99
 
 [tool.pylint."MASTER"]
```

### Comparing `mltb2-0.0.1/setup.py` & `mltb2-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 
 import setuptools
 
 
 project_name = "mltb2"
 source_code = "https://github.com/telekom/mltb2"
 keywords = "optuna deep-learning ml ai machine-learning hyperparameter-optimization"
-install_requires = ["numpy", "scipy"]
+install_requires = ["numpy", "scipy", "tqdm"]
 extras_require = {
     "checking": [
         "black",
         "flake8",
         "isort",
         "mdformat",
         "pydocstyle",
         "mypy",
         "pylint",
         "pylintfileheader",
     ],
-    "optional": ["optuna", "SoMaJo", "transformers", "torch", "scikit-learn"],
+    "optional": ["optuna", "SoMaJo", "transformers", "torch", "scikit-learn", "matplotlib"],
     "testing": ["pytest", "packaging"],
     "doc": ["sphinx", "sphinx_rtd_theme", "myst_parser", "sphinx_copybutton"],
 }
 
 # add "all"
 all_extra_packages = list(
     {package_name for value in extras_require.values() for package_name in value}
@@ -57,35 +57,35 @@
     author_email="philip@may.la",
     description="Machine Learning Toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=source_code,
     project_urls={
         "Bug Tracker": source_code + "/issues",
-        #        "Documentation": "https://telekom.github.io/mltb2/",
+        "Documentation": "https://telekom.github.io/mltb2/",
         "Source Code": source_code,
-        #        "Contributing": source_code + "/blob/main/CONTRIBUTING.md",
-        #        "Code of Conduct": source_code + "/blob/main/CODE_OF_CONDUCT.md",
+        # "Contributing": source_code + "/blob/main/CONTRIBUTING.md",
+        # "Code of Conduct": source_code + "/blob/main/CODE_OF_CONDUCT.md",
     },
     packages=setuptools.find_packages(),
-    python_requires=">=3.9",
+    python_requires=">=3.8",
     install_requires=install_requires,
     extras_require=extras_require,
     keywords=keywords,
     classifiers=[
         "Development Status :: 3 - Alpha",
         # "Development Status :: 4 - Beta",
         # "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Science/Research",
         # "Intended Audience :: Education",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         # "Programming Language :: Python :: 3.7",
-        # "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Mathematics",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development",
```

### Comparing `mltb2-0.0.1/tests/test_optuna.py` & `mltb2-0.0.2/tests/test_optuna.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.1/tests/test_somajo_transformers.py` & `mltb2-0.0.2/tests/test_somajo_transformers.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.0.1/tests/test_transformers.py` & `mltb2-0.0.2/tests/test_transformers.py`

 * *Files identical despite different names*

