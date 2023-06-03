# Comparing `tmp/mleko-0.3.1.tar.gz` & `tmp/mleko-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mleko-0.3.1.tar", max compression
+gzip compressed data, was "mleko-0.4.0.tar", max compression
```

## Comparing `mleko-0.3.1.tar` & `mleko-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,49 @@
--rw-r--r--   0        0        0     1073 2023-05-21 14:49:50.169455 mleko-0.3.1/LICENSE
--rw-r--r--   0        0        0     2561 2023-05-21 14:49:50.169455 mleko-0.3.1/README.md
--rw-r--r--   0        0        0     2753 2023-05-21 14:50:31.169551 mleko-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1286 2023-05-21 14:50:31.101550 mleko-0.3.1/src/mleko/__init__.py
--rw-r--r--   0        0        0     1372 2023-05-21 14:49:50.169455 mleko-0.3.1/src/mleko/cache/__init__.py
--rw-r--r--   0        0        0    15230 2023-05-21 14:49:50.169455 mleko-0.3.1/src/mleko/cache/cache.py
--rw-r--r--   0        0        0     3573 2023-05-21 14:49:50.169455 mleko-0.3.1/src/mleko/cache/fingerprinters.py
--rw-r--r--   0        0        0      502 2023-05-21 14:49:50.169455 mleko-0.3.1/src/mleko/data/__init__.py
--rw-r--r--   0        0        0    11680 2023-05-21 14:49:50.169455 mleko-0.3.1/src/mleko/data/converters.py
--rw-r--r--   0        0        0      676 2023-05-21 14:49:50.169455 mleko-0.3.1/src/mleko/data/sources/__init__.py
--rw-r--r--   0        0        0     2760 2023-05-21 14:49:50.169455 mleko-0.3.1/src/mleko/data/sources/base_data_source.py
--rw-r--r--   0        0        0    17518 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/data/sources/kaggle_data_source.py
--rw-r--r--   0        0        0     8531 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/data/sources/s3_data_source.py
--rw-r--r--   0        0        0    10930 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/data/splitters.py
--rw-r--r--   0        0        0      608 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/pipeline/__init__.py
--rw-r--r--   0        0        0     1095 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/pipeline/data_container.py
--rw-r--r--   0        0        0     4205 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/pipeline/pipeline.py
--rw-r--r--   0        0        0     3425 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/pipeline/pipeline_step.py
--rw-r--r--   0        0        0      515 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/pipeline/steps/__init__.py
--rw-r--r--   0        0        0     2220 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/pipeline/steps/convert.py
--rw-r--r--   0        0        0     2080 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/pipeline/steps/ingest.py
--rw-r--r--   0        0        0     2110 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/pipeline/steps/split.py
--rw-r--r--   0        0        0        0 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/py.typed
--rw-r--r--   0        0        0      731 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/utils/__init__.py
--rw-r--r--   0        0        0     4497 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/utils/custom_logger.py
--rw-r--r--   0        0        0     2698 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/utils/decorators.py
--rw-r--r--   0        0        0      742 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/utils/file_helpers.py
--rw-r--r--   0        0        0     1176 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/utils/tqdm.py
--rw-r--r--   0        0        0     1600 2023-05-21 14:49:50.173455 mleko-0.3.1/src/mleko/utils/vaex.py
--rw-r--r--   0        0        0     3527 1970-01-01 00:00:00.000000 mleko-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-03 21:07:46.476830 mleko-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2561 2023-06-03 21:07:46.476830 mleko-0.4.0/README.md
+-rw-r--r--   0        0        0     1323 2023-06-03 21:08:25.148945 mleko-0.4.0/mleko/__init__.py
+-rw-r--r--   0        0        0      584 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/cache/__init__.py
+-rw-r--r--   0        0        0    11493 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/cache/cache_mixin.py
+-rw-r--r--   0        0        0      805 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/cache/fingerprinters/__init__.py
+-rw-r--r--   0        0        0     1167 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/cache/fingerprinters/base_fingerprinter.py
+-rw-r--r--   0        0        0     2843 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/cache/fingerprinters/csv_fingerprinter.py
+-rw-r--r--   0        0        0     1233 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/cache/fingerprinters/vaex_fingerprinter.py
+-rw-r--r--   0        0        0      398 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/cache/format/__init__.py
+-rw-r--r--   0        0        0     1933 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/cache/format/vaex_cache_format_mixin.py
+-rw-r--r--   0        0        0     5974 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/cache/lru_cache_mixin.py
+-rw-r--r--   0        0        0      740 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/__init__.py
+-rw-r--r--   0        0        0      491 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/convert/__init__.py
+-rw-r--r--   0        0        0     1435 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/convert/base_converter.py
+-rw-r--r--   0        0        0    11536 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/convert/csv_to_vaex_converter.py
+-rw-r--r--   0        0        0     1613 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/feature_select/__init__.py
+-rw-r--r--   0        0        0     5922 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/feature_select/base_feature_selector.py
+-rw-r--r--   0        0        0     5268 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/feature_select/composite_feature_selector.py
+-rw-r--r--   0        0        0     4988 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/feature_select/invariance_feature_selector.py
+-rw-r--r--   0        0        0     5253 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/feature_select/missing_rate_feature_selector.py
+-rw-r--r--   0        0        0     7083 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
+-rw-r--r--   0        0        0     5506 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/feature_select/variance_feature_selector.py
+-rw-r--r--   0        0        0      877 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/ingest/__init__.py
+-rw-r--r--   0        0        0     2211 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/ingest/base_ingester.py
+-rw-r--r--   0        0        0    18015 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/ingest/kaggle_ingester.py
+-rw-r--r--   0        0        0     9632 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/ingest/s3_ingester.py
+-rw-r--r--   0        0        0      679 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/split/__init__.py
+-rw-r--r--   0        0        0     1394 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/split/base_splitter.py
+-rw-r--r--   0        0        0     3815 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/split/expression_splitter.py
+-rw-r--r--   0        0        0     5934 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/split/random_splitter.py
+-rw-r--r--   0        0        0      644 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/pipeline/__init__.py
+-rw-r--r--   0        0        0     1420 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/pipeline/data_container.py
+-rw-r--r--   0        0        0     4496 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/pipeline/pipeline.py
+-rw-r--r--   0        0        0     3595 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/pipeline/pipeline_step.py
+-rw-r--r--   0        0        0      638 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/pipeline/steps/__init__.py
+-rw-r--r--   0        0        0     2359 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/pipeline/steps/convert_step.py
+-rw-r--r--   0        0        0     2179 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/pipeline/steps/feature_select_step.py
+-rw-r--r--   0        0        0     2141 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/pipeline/steps/ingest_step.py
+-rw-r--r--   0        0        0     2248 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/pipeline/steps/split_step.py
+-rw-r--r--   0        0        0        0 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/py.typed
+-rw-r--r--   0        0        0      765 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/utils/__init__.py
+-rw-r--r--   0        0        0     4497 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/utils/custom_logger.py
+-rw-r--r--   0        0        0     3430 2023-06-03 21:07:46.484830 mleko-0.4.0/mleko/utils/decorators.py
+-rw-r--r--   0        0        0      742 2023-06-03 21:07:46.484830 mleko-0.4.0/mleko/utils/file_helpers.py
+-rw-r--r--   0        0        0     1403 2023-06-03 21:07:46.484830 mleko-0.4.0/mleko/utils/tqdm_helpers.py
+-rw-r--r--   0        0        0     2836 2023-06-03 21:07:46.484830 mleko-0.4.0/mleko/utils/vaex_helpers.py
+-rw-r--r--   0        0        0     2752 2023-06-03 21:08:25.212945 mleko-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3580 1970-01-01 00:00:00.000000 mleko-0.4.0/PKG-INFO
```

### Comparing `mleko-0.3.1/LICENSE` & `mleko-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mleko-0.3.1/README.md` & `mleko-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mleko-0.3.1/pyproject.toml` & `mleko-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tool.poetry]
 name = "mleko"
-version = "0.3.1"
+version = "0.4.0"
 description = "ML-Ekosystem"
 authors = ["Erik Båvenstrand <erik@bavenstrand.se>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ErikBavenstrand/mleko"
 repository = "https://github.com/ErikBavenstrand/mleko"
 documentation = "https://mleko.readthedocs.io"
 classifiers = [
     "Development Status :: 3 - Alpha",
 ]
 
 [tool.poetry.urls]
-Changelog = "https://github.com/ErikBavenstrand/mleko/releases"
+Changelog = "https://github.com/ErikBavenstrand/mleko/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "3.10.* || 3.9.* || 3.8.*"
 boto3 = "^1.26.91"
 botocore = "^1.29.91"
 tqdm = "^4.65.0"
 vaex = "^4.16.0"
 scikit-learn = "^1.2.2"
+pandas = "^2.0.2"
 
 [tool.poetry.group.dev.dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 boto3-stubs = {extras = ["s3"], version = "^1.26.91"}
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
@@ -54,25 +55,25 @@
 nox = "^2023.4.22"
 nox-poetry = "^1.0.2"
 sphinx-autodoc-typehints = "^1.23.0"
 sphinx-autoapi = "^2.1.0"
 python-semantic-release = "^7.33.3"
 
 [tool.coverage.paths]
-source = ["src", "*/site-packages"]
+source = ["mleko", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
 branch = false
 source = ["mleko"]
 
 [tool.coverage.report]
 show_missing = true
 fail_under = 100
-exclude_lines = ["pragma: no cover", "raise NotImplementedError", '"""']
+exclude_lines = ["pragma: no cover", "raise NotImplementedError", '"""', "self._cached_execute"]
 
 [tool.isort]
 profile = "black"
 lines_after_imports = 2
 line_length = 120
 use_parentheses = true
 include_trailing_comma = true
@@ -87,33 +88,31 @@
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
 
 
 [[tool.mypy.overrides]]
 module = [
-    "vaex",
-    "tqdm",
-    "boto3",
-    "boto3.s3.transfer",
-    "botocore.config",
-    "pyarrow",
-    "requests",
-    "requests.auth",
-    "sklearn.model_selection",
+    "vaex.*",
+    "tqdm.*",
+    "boto3.*",
+    "botocore.*",
+    "pyarrow.*",
+    "requests.*",
+    "sklearn.*",
 ]
 ignore_missing_imports = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 branch = "main"
-version_variable = "src/mleko/__init__.py:__version__"
+version_variable = "mleko/__init__.py:__version__"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_source = "tag"
 commit_version_number = true
 tag_commit = true
 upload_to_pypi = false
 upload_to_release = false
 hvcs = "github"
```

### Comparing `mleko-0.3.1/src/mleko/__init__.py` & `mleko-0.4.0/mleko/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,8 +16,11 @@
    caching of method call results and tracking changes in data.
 
 * Utilities: A collection of utility functions for logging, decorating, file management, and TQDM wrappers.
 
 Each subpackage is designed to be modular and extensible, making it easy to customize and adapt the library to a wide
 range of model building processes and requirements.
 """
-__version__ = "0.3.1"
+from __future__ import annotations
+
+
+__version__ = "0.4.0"
```

### Comparing `mleko-0.3.1/src/mleko/cache/cache.py` & `mleko-0.4.0/mleko/cache/cache_mixin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,142 +1,121 @@
-"""A mixin module that provides a flexible and configurable caching mechanism for method call results.
+"""This module contains the basic `CacheMixin` class for caching the results of method calls.
 
-This module contains mixin classes designed to cache method call results efficiently, reducing
-the overhead of repetitive calculations or data fetching. The CacheMixin class stores the results
-of method calls on a per-instance basis, based on user-defined cache keys and fingerprints. The
-LRUCacheMixin class extends the CacheMixin to implement a Least Recently Used (LRU) cache eviction
-mechanism that helps manage the cache size by evicting the least recently used cache entries when
-the specified maximum number of cache entries is exceeded.
-
-Usage:
-    CacheMixin should be subclassed by other classes that require caching capabilities for their method calls.
-    The subclass should implement the method logic inside a lambda function and pass it to the `_cached_execute`
-    method, along with any cache keys needed to identify unique results. For more advanced use cases,
-    the LRUCacheMixin can be employed to enable automatic cache eviction based on an LRU strategy.
+This class can be used as a mixin to add caching functionality to a class. It provides the basic
+functionality for caching the results of method calls based on user-defined cache keys and fingerprints.
+
+The class can be extended to provide additional functionality by inheriting from it and overriding
+the `_read_cache_file()` and `_write_cache_file()` methods to customize the cache loading and saving
+processes, respectively.
+
+Combining this class with the format mixins can be used to add support for caching different data
+formats, such as Vaex DataFrames in Arrow format.
 """
 from __future__ import annotations
 
 import hashlib
 import inspect
 import pickle
 import re
-from collections import OrderedDict
 from pathlib import Path
 from typing import Any, Callable, Hashable, Sequence
 
-import vaex
-from tqdm import tqdm
-
-from mleko.cache.fingerprinters import Fingerprinter
+from mleko.cache.fingerprinters.base_fingerprinter import BaseFingerprinter
 from mleko.utils.custom_logger import CustomLogger
-from mleko.utils.tqdm import set_tqdm_percent_wrapper
 
 
 logger = CustomLogger()
-"""A CustomLogger instance that's used throughout the module for logging."""
+"""A module-level logger instance."""
 
 
 def get_frame_qualname(frame: inspect.FrameInfo) -> str:
     """Gets the fully qualified name of the function or method associated with the provided frame.
 
     Args:
-        frame: A FrameInfo object containing the information of the function or method call.
+        frame: A `FrameInfo` object containing the information of the function or method call.
 
     Returns:
         A string representing the fully qualified name, in the format "module.class.method" for class methods or
         "module.function" for functions.
     """
     caller_function = frame.function
     caller_obj = inspect.getmodule(frame[0])
     module_name = caller_obj.__name__ if caller_obj is not None else "__main__"
     if "self" in frame.frame.f_locals:
         class_name = frame.frame.f_locals["self"].__class__.__name__
         return f"{module_name}.{class_name}.{caller_function}"
     return f"{module_name}.{caller_function}"
 
 
-class VaexArrowCacheFormatMixin:
-    """A mixin class for Vaex DataFrames to provide Arrow format caching capabilities.
-
-    This mixin class adds methods for reading and writing arrow cache files for Vaex DataFrames.
-    """
-
-    cache_file_suffix = "arrow"
-    """The file extension to use for cache files."""
-
-    def _read_cache_file(self, cache_file_path: Path) -> vaex.DataFrame:
-        """Reads a cache file containing a Vaex DataFrame.
-
-        Args:
-            cache_file_path: The path of the cache file to be read.
-
-        Returns:
-            The contents of the cache file as a DataFrame.
-        """
-        return vaex.open(cache_file_path)
-
-    def _write_cache_file(self, cache_file_path: Path, output: vaex.DataFrame) -> None:
-        """Writes the results of the DataFrame conversion to Arrow format in a cache file with arrow suffix.
-
-        Args:
-            cache_file_path: The path of the cache file to be written.
-            output: The Vaex DataFrame to be saved in the cache file.
-        """
-        with tqdm(total=100, desc="Writing DataFrame to Arrow file") as pbar:
-            output.export_arrow(
-                cache_file_path,
-                progress=set_tqdm_percent_wrapper(pbar),
-                parallel=True,
-                reduce_large=True,
-            )
-        output.close()
-
-
 class CacheMixin:
     """A mixin class for caching the results of method calls based on user-defined cache keys and fingerprints.
 
+    The basic functionality of this class is to cache the results of method calls based on user-defined cache keys and
+    fingerprints. The cache keys can be a mix of hashable values and tuples containing a value and a BaseFingerprinter
+    instance for generating fingerprints. The `CacheMixin` class will save cache files in the specified cache directory
+    using the cache key as the filename and the cache file suffix as the file extension. The cache files will be saved
+    in the cache directory as pickle files.
+
     Warning:
         This class maintains an ever-growing cache, which means that the cache size may increase indefinitely
         with new method calls, possibly consuming a large amount of disk space. It does not implement any
         cache eviction strategy. It is recommended to either clear the cache manually when needed or
         use the LRUCacheMixin class, which extends this class to provide an LRU cache mechanism with
         eviction of least recently used cache entries based on a specified maximum number of cache entries.
     """
 
     def __init__(self, cache_directory: str | Path, cache_file_suffix: str) -> None:
-        """Initializes the CacheMixin with the provided cache directory.
+        """Initializes the `CacheMixin` with the provided cache directory.
+
+        Note:
+            The cache directory will be created if it does not exist.
 
         Args:
             cache_directory: The directory where cache files will be stored.
             cache_file_suffix: The suffix/file ending of the cache files.
+
+        Examples:
+            >>> from mleko.cache.cache_mixin import CacheMixin
+            >>> class MyClass(CacheMixin):
+            ...     def __init__(self):
+            ...         super().__init__(".cache", "pkl")
+            ...
+            ...     def my_method(self, x):
+            ...         return self._cached_execute(lambda: x ** 2, [x])
+            ...
+            >>> my_class = MyClass()
+            >>> my_class.my_method(2)
+            4 # This will be computed and cached
+            >>> my_class.my_method(2)
+            4 # This will be loaded from the cache
+            >>> my_class.my_method(3)
+            9 # This will be recomputed and cached
         """
         self._cache_directory = Path(cache_directory)
         self._cache_directory.mkdir(parents=True, exist_ok=True)
         self._cache_file_suffix = cache_file_suffix
-        self._cache_type_name = [
-            base.__name__ for base in self.__class__.__bases__ if CacheMixin.__name__ in base.__name__
-        ][0].replace("Mixin", "")
+        self._cache_type_name = self._find_cache_type_name(self.__class__)
 
     def _cached_execute(
         self,
         lambda_func: Callable[[], Any],
-        cache_keys: list[Hashable | tuple[Any, Fingerprinter]],
+        cache_keys: list[Hashable | tuple[Any, BaseFingerprinter]],
         force_recompute: bool = False,
     ) -> Any:
         """Executes the given function, caching the results based on the provided cache keys and fingerprints.
 
         Args:
             lambda_func: A lambda function to execute.
             cache_keys: A list of cache keys that can be a mix of hashable values and tuples containing a value and a
-                Fingerprinter instance for generating fingerprints.
+                BaseFingerprinter instance for generating fingerprints.
             force_recompute: A boolean indicating whether to force recompute the result and update the cache, even if a
                 cached result is available.
 
         Returns:
-            The result of executing the given function. If a cached result is available and force_recompute is False,
+            The result of executing the given function. If a cached result is available and `force_recompute` is False,
             the cached result will be returned instead of recomputing the result.
         """
         frame_qualname = get_frame_qualname(inspect.stack()[1])
         class_method_name = ".".join(frame_qualname.split(".")[-2:])
         cache_key = self._compute_cache_key(cache_keys, frame_qualname)
 
         if not force_recompute:
@@ -155,30 +134,32 @@
                 f"\033[33mForce Cache Refresh\033[0m ({self._cache_type_name}) {class_method_name}: Executing method."
             )
 
         output = lambda_func()
         self._save_to_cache(cache_key, output)
         return self._load_from_cache(cache_key)
 
-    def _compute_cache_key(self, cache_keys: list[Hashable | tuple[Any, Fingerprinter]], frame_qualname: str) -> str:
+    def _compute_cache_key(
+        self, cache_keys: list[Hashable | tuple[Any, BaseFingerprinter]], frame_qualname: str
+    ) -> str:
         """Computes the cache key based on the provided cache keys and the calling function's fully qualified name.
 
         Args:
             cache_keys: A list of cache keys that can be a mix of hashable values and tuples containing a value and a
-                Fingerprinter instance for generating fingerprints.
+                BaseFingerprinter instance for generating fingerprints.
             frame_qualname: The fully qualified name of the cached function stack frame.
 
         Returns:
             A string representing the computed cache key, which is the MD5 hash of the fully qualified name of the
             calling function or method, along with the fingerprints of the provided cache keys.
         """
         values_to_hash: list[Hashable] = []
 
         for key in cache_keys:
-            if isinstance(key, tuple) and len(key) == 2 and isinstance(key[1], Fingerprinter):
+            if isinstance(key, tuple) and len(key) == 2 and isinstance(key[1], BaseFingerprinter):
                 value, fingerprinter = key
                 values_to_hash.append(fingerprinter.fingerprint(value))
             else:
                 values_to_hash.append(key)
 
         data = pickle.dumps((frame_qualname, values_to_hash))
 
@@ -252,85 +233,24 @@
             for i in range(len(output)):
                 cache_file_path = self._cache_directory / f"{cache_key}_{i}.{self._cache_file_suffix}"
                 self._write_cache_file(cache_file_path, output[i])
         else:
             cache_file_path = self._cache_directory / f"{cache_key}.{self._cache_file_suffix}"
             self._write_cache_file(cache_file_path, output)
 
-
-class LRUCacheMixin(CacheMixin):
-    """Least Recently Used Cache Mixin.
-
-    This mixin class extends the CacheMixin to provide a Least Recently Used (LRU) cache mechanism.
-    It evicts the least recently used cache entries when the maximum number of cache entries is exceeded.
-    The LRU cache mechanism ensures that the most frequently accessed cache entries are retained,
-    while entries that are rarely accessed and have not been accessed recently are evicted first as the cache fills up.
-    """
-
-    def __init__(self, cache_directory: str | Path, cache_file_suffix: str, max_entries: int) -> None:
-        """Initializes the LRUCacheMixin with the provided cache directory and maximum number of cache entries.
-
-        Args:
-            cache_directory: The directory where cache files will be stored.
-            cache_file_suffix: The file extension to use for cache files.
-            max_entries: The maximum number of cache entries allowed before eviction.
-        """
-        super().__init__(cache_directory, cache_file_suffix)
-        self._max_entries = max_entries
-        self._cache: OrderedDict[str, bool] = OrderedDict()
-        self._load_cache_from_disk()
-
-    def _load_cache_from_disk(self) -> None:
-        """Loads the cache entries from the cache directory and initializes the LRU cache.
-
-        Cache entries are ordered by their modification time, and the cache is trimmed if needed.
-        """
-        frame_qualname = get_frame_qualname(inspect.stack()[2])
-        class_name = frame_qualname.split(".")[-2]
-        cache_files = [
-            f
-            for f in self._cache_directory.glob(f"*.{self._cache_file_suffix}")
-            if re.search(rf"{class_name}\.[a-zA-Z]+\.[a-fA-F\d]{{32}}", str(f.stem))
-        ]
-        ordered_cache_files = sorted(cache_files, key=lambda x: x.stat().st_mtime)
-        for cache_file in ordered_cache_files:
-            cache_key = cache_file.stem.split("_")[0]
-            if cache_key not in self._cache:
-                if len(self._cache) >= self._max_entries:
-                    oldest_key = next(iter(self._cache))
-                    del self._cache[oldest_key]
-                    for file in self._cache_directory.glob(f"{oldest_key}*.{self._cache_file_suffix}"):
-                        file.unlink()
-                self._cache[cache_key] = True
-
-    def _load_from_cache(self, cache_key: str) -> Any | None:
-        """Loads data from the cache based on the provided cache key and updates the LRU cache.
+    def _find_cache_type_name(self, cls: type) -> str | None:
+        """Recursively searches the class hierarchy for the name of the class that inherits from `CacheMixin`.
 
         Args:
-            cache_key: A string representing the cache key.
+            cls: The class to search.
 
         Returns:
-            The cached data if it exists, or None if there is no data for the given cache key.
+            The name of the class that inherits from `CacheMixin`, or None if no such class exists.
         """
-        if cache_key in self._cache:
-            self._cache.move_to_end(cache_key)
-        return super()._load_from_cache(cache_key)
+        if CacheMixin.__name__ in cls.__name__:
+            return cls.__name__.replace("Mixin", "")
 
-    def _save_to_cache(self, cache_key: str, output: Any) -> None:
-        """Saves the given data to the cache using the provided cache key, updating the LRU cache accordingly.
-
-        If the cache reaches its maximum size, the least recently used entry will be evicted.
-
-        Args:
-            cache_key: A string representing the cache key.
-            output: The data to be saved to the cache.
-        """
-        if cache_key not in self._cache:
-            if len(self._cache) >= self._max_entries:
-                oldest_key = next(iter(self._cache))
-                del self._cache[oldest_key]
-                for file in self._cache_directory.glob(f"{oldest_key}*.{self._cache_file_suffix}"):
-                    file.unlink()
-            self._cache[cache_key] = True
-        else:
-            self._cache.move_to_end(cache_key)
-        super()._save_to_cache(cache_key, output)
+        for base in cls.__bases__:
+            found_class_name = self._find_cache_type_name(base)
+            if found_class_name:
+                return found_class_name
+        return None
```

### Comparing `mleko-0.3.1/src/mleko/cache/fingerprinters.py` & `mleko-0.4.0/mleko/cache/fingerprinters/csv_fingerprinter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,37 @@
-"""This module provides Fingerprinter classes for generating unique fingerprints.
-
-Fingerprinters are used for generating unique fingerprints of various data and file types,
-such as Vaex DataFrames or CSV files. These fingerprints can be used to track changes in data and support
-caching mechanisms.
-"""
+"""The module contains a fingerprinter for CSV files supporting Gzipped and raw CSV files."""
 from __future__ import annotations
 
 import gzip
 import hashlib
-from abc import ABC, abstractmethod
 from concurrent import futures
 from itertools import islice
 from pathlib import Path
-from typing import Any
-
-import vaex
-
-
-class Fingerprinter(ABC):
-    """Abstract base class for creating specialized fingerprinters."""
-
-    @abstractmethod
-    def fingerprint(self, data: Any) -> str:
-        """Generate a fingerprint for the given data.
-
-        Args:
-            data: Data that should be fingerprinted.
-
-        Raises:
-            NotImplementedError: The method has to be implemented by the subclass.
 
-        Returns:
-            str: The fingerprint as a hexadecimal string.
-        """
-        raise NotImplementedError
+from .base_fingerprinter import BaseFingerprinter
 
 
-class CSVFingerprinter(Fingerprinter):
+class CSVFingerprinter(BaseFingerprinter):
     """A fingerprinter for CSV files supporting Gzipped and raw CSV files."""
 
     def __init__(self, n_rows: int = 1000):
         """Initialize the CSVFingerprinter.
 
+        Warning:
+            The fingerprint is generated by reading the first `n_rows` of each CSV file. If the
+            CSV file is larger than `n_rows`, only the first `n_rows` are read. This means that
+            the fingerprint is not unique for the entire CSV file, but only for the first `n_rows`.
+
         Args:
             n_rows: The number of rows to sample from each CSV file for fingerprinting.
+
+        Examples:
+            >>> fingerprinter = CSVFingerprinter(n_rows=1000)
+            >>> fingerprinter.fingerprint(["data.csv", "data2.csv"])
+            "fingerprint"
         """
         self._n_rows = n_rows
 
     def fingerprint(self, file_paths: list[str] | list[Path]) -> str:
         """Generate a fingerprint for the given list of CSV files.
 
         The currently supported file types are `.csv`, `.gz`, and `.csv.gz`.
@@ -85,23 +69,7 @@
             with gzip.open(file_path, "rb") as f:
                 sample = b"".join(islice((f.readline() for _ in range(self._n_rows)), self._n_rows))
         else:
             with open(file_path, "rb") as f:
                 sample = b"".join(islice((f.readline() for _ in range(self._n_rows)), self._n_rows))
         fingerprint = hashlib.md5(str(sample).encode()).hexdigest()
         return fingerprint
-
-
-class VaexFingerprinter(Fingerprinter):
-    """A fingerprinter for Vaex DataFrames."""
-
-    def fingerprint(self, dataframe: vaex.DataFrame) -> str:
-        """Generate a fingerprint for a Vaex DataFrame.
-
-        Args:
-            dataframe: The Vaex DataFrame to be fingerprinted.
-
-        Returns:
-            The fingerprint as a hexadecimal string.
-        """
-        fingerprint = hashlib.md5(str(dataframe.fingerprint()).encode()).hexdigest()
-        return fingerprint
```

### Comparing `mleko-0.3.1/src/mleko/data/converters.py` & `mleko-0.4.0/mleko/dataset/convert/csv_to_vaex_converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,36 @@
-"""The module provides functionality for converting data between different file formats.
-
-It includes a base class for data converters to support various file format conversions and caching mechanisms.
-While it primarily focuses on handling CSV files, the infrastructure allows for extending its
-capabilities to other formats as needed.
-"""
+"""The module contains the `CSVToVaexConverter`, which converts CSV to a random-access `vaex` compatible format."""
 from __future__ import annotations
 
 import multiprocessing
-from abc import ABC, abstractmethod
 from concurrent import futures
 from itertools import repeat
 from pathlib import Path
 
 import vaex
 from pyarrow import csv as arrow_csv
 from tqdm import tqdm
 
-from mleko.cache.cache import LRUCacheMixin, VaexArrowCacheFormatMixin
 from mleko.cache.fingerprinters import CSVFingerprinter
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
+from mleko.utils.file_helpers import clear_directory
+
+from .base_converter import BaseConverter
 
 
 logger = CustomLogger()
-"""A CustomLogger instance that's used throughout the module for logging."""
+"""A module-level logger instance."""
 
 V_CPU_COUNT = multiprocessing.cpu_count()
 """A module-level constant representing the total number of CPUs available on the current system."""
 
 
-class BaseDataConverter(ABC):
-    """A base class for data converter classes, providing an interface for converting file formats."""
-
-    def __init__(self, output_directory: str | Path):
-        """Initialize the BaseDataConverter with the output directory for the converted files.
-
-        Args:
-            output_directory: The directory where the converted files will be saved.
-        """
-        self._output_directory = Path(output_directory)
-        self._output_directory.mkdir(parents=True, exist_ok=True)
-
-    @abstractmethod
-    def convert(self, file_paths: list[Path] | list[str]) -> vaex.DataFrame:
-        """Abstract method to convert the input file paths to the desired output format.
-
-        Args:
-            file_paths: A list of input file paths to be converted.
-
-        Returns:
-            vaex.DataFrame: The resulting DataFrame after conversion.
-        """
-        raise NotImplementedError
-
-
-class CsvToArrowConverter(BaseDataConverter, VaexArrowCacheFormatMixin, LRUCacheMixin):
-    """A class that converts CSV files to Arrow format using the vaex library and caches the resulting dataframes."""
+class CSVToVaexConverter(BaseConverter):
+    """A class that converts CSV to a random-access `vaex` compatible format."""
 
     @auto_repr
     def __init__(
         self,
         output_directory: str | Path,
         forced_numerical_columns: list[str] | tuple[str, ...] | tuple[()] = (),
         forced_categorical_columns: list[str] | tuple[str, ...] | tuple[()] = (),
@@ -87,59 +58,87 @@
             "missing",
         ),
         true_values: list[str] | tuple[str, ...] | tuple[()] = ("t", "True", "true", "1"),
         false_values: list[str] | tuple[str, ...] | tuple[()] = ("f", "False", "false", "0"),
         downcast_float: bool = False,
         random_state: int | None = None,
         num_workers: int = V_CPU_COUNT,
-        max_cache_entries: int = 1,
+        cache_size: int = 1,
     ) -> None:
-        """Initializes the CsvToArrowConverter with the necessary configurations and parameters.
+        """Initializes the `CSVToArrowConverter` with the necessary configurations and parameters.
 
         Args:
             output_directory: The directory where the converted files will be saved.
             forced_numerical_columns: A sequence of column names to force as numerical type.
             forced_categorical_columns: A sequence of column names to force as categorical type.
             forced_boolean_columns: A sequence of column names to force as boolean type.
             drop_columns: A sequence of column names to drop during conversion.
             na_values: A sequence of strings to consider as NaN or missing values.
             true_values: A sequence of strings to consider as True values.
             false_values: A sequence of strings to consider as False values.
             downcast_float: If True, downcast float64 to float32 during conversion.
             random_state: A seed for the random number generator.
             num_workers: Number of workers to use for parallel processing.
-            max_cache_entries: Maximum number of cache entries for the LRUCacheMixin.
+            cache_size: Maximum number of cache entries for the LRUCacheMixin.
+
+        Warning:
+            The `forced_numerical_columns`, `forced_categorical_columns`, `forced_boolean_columns`, and `drop_columns`
+            parameters are mutually exclusive. Meaning, a column cannot be specified in more than one of these
+            parameters. If a column is specified in more than one of these parameters, the last parameter will be used
+            and the previous ones will be ignored.
+
+        Example:
+            >>> import vaex
+            >>> from mleko.dataset.convert import CSVToArrowConverter
+            >>> converter = CSVToArrowConverter(
+            ...     output_directory="cache",
+            ...     forced_numerical_columns=["x"],
+            ...     forced_categorical_columns=["y"],
+            ...     forced_boolean_columns=["z"],
+            ...     drop_columns=["a"],
+            ...     na_values=["-9999"],
+            ...     true_values=["t"],
+            ...     false_values=["f"],
+            ...     downcast_float=True,
+            ...     random_state=42,
+            ...     num_workers=4,
+            ...     cache_size=1,
+            ... )
+            >>> df = converter.convert(["data.csv"])
         """
-        BaseDataConverter.__init__(self, output_directory)
-        VaexArrowCacheFormatMixin.__init__(self)
-        LRUCacheMixin.__init__(self, output_directory, VaexArrowCacheFormatMixin.cache_file_suffix, max_cache_entries)
+        super().__init__(output_directory, cache_size)
         self._forced_numerical_columns = tuple(forced_numerical_columns)
         self._forced_categorical_columns = tuple(forced_categorical_columns)
         self._forced_boolean_columns = tuple(forced_boolean_columns)
         self._drop_columns = tuple(drop_columns)
         self._na_values = tuple(na_values)
         self._true_values = tuple(true_values)
         self._false_values = tuple(false_values)
         self._downcast_float = downcast_float
         self._num_workers = num_workers
         self._random_state = random_state
 
     def convert(self, file_paths: list[Path] | list[str], force_recompute: bool = False) -> vaex.DataFrame:
-        """Converts a list of CSV files to Arrow format and returns a vaex dataframe joined from the converted data.
+        """Converts a list of CSV files to Arrow format and returns a `vaex` dataframe joined from the converted data.
 
-        The method takes care of caching, and results will be reused accordingly unless force_recompute is set to True.
-        The resulting dataframe is a vaex DataFrame joined from the converted data. The conversion is done in chunks
-        to optimize parallel processing.
+        The method takes care of caching, and results will be reused accordingly unless `force_recompute`
+        is set to True. The resulting dataframe is a `vaex` DataFrame joined from the converted data.
+        The conversion is done in chunks to optimize parallel processing.
+
+        Note:
+            Will read the first `100,000/len(file_paths)` rows of each file to determine if the file is the same as the
+            one in the cache. If the file is the same, the cache will be used. Otherwise, the file will be converted
+            and the cache will be updated.
 
         Args:
             file_paths: A list of file paths to be converted.
             force_recompute: If set to True, forces recomputation and ignores the cache.
 
         Returns:
-            vaex.DataFrame: The resulting dataframe with the combined converted data.
+            The resulting dataframe with the combined converted data.
         """
         return self._cached_execute(
             lambda_func=lambda: self._convert(file_paths),
             cache_keys=[
                 self._forced_numerical_columns,
                 self._forced_categorical_columns,
                 self._forced_boolean_columns,
@@ -216,15 +215,15 @@
                     "%Y-%m-%dT%H:%M:%S",
                     "%Y-%m-%dT%H:%M:%S.%f",
                 ],
             ),
         ).drop(drop_columns)
 
         output_path = output_directory / f"df_chunk_{file_path.stem}.{dataframe_suffix}"
-        df_chunk.export_arrow(output_path)
+        df_chunk.export(output_path)
         df_chunk.close()
 
     def _convert(self, file_paths: list[Path] | list[str]) -> vaex.DataFrame:
         """Converts a list of CSV files to Arrow format using parallel processing.
 
         Chunks of files are processed in parallel and saved in the output directory.
 
@@ -233,35 +232,33 @@
 
         Returns:
             A DataFrame containing the merged chunks.
         """
         with tqdm(total=len(file_paths), desc="Converting CSV files") as pbar:
             with futures.ProcessPoolExecutor(max_workers=min(self._num_workers, len(file_paths))) as executor:
                 for _ in executor.map(
-                    CsvToArrowConverter._convert_csv_file_to_arrow,
+                    CSVToVaexConverter._convert_csv_file_to_arrow,
                     file_paths,
-                    repeat(self._output_directory),
-                    repeat(VaexArrowCacheFormatMixin.cache_file_suffix),
+                    repeat(self._cache_directory),
+                    repeat(self._cache_file_suffix),
                     repeat(self._forced_numerical_columns),
                     repeat(self._forced_categorical_columns),
                     repeat(self._forced_boolean_columns),
                     repeat(self._drop_columns),
                     repeat(self._na_values),
                     repeat(self._true_values),
                     repeat(self._false_values),
                     repeat(self._downcast_float),
                 ):
                     pbar.update(1)
 
-        return vaex.open(self._output_directory / f"df_chunk_*.{VaexArrowCacheFormatMixin.cache_file_suffix}")
+        return vaex.open(self._cache_directory / f"df_chunk_*.{self._cache_file_suffix}")
 
     def _write_cache_file(self, cache_file_path: Path, output: vaex.DataFrame) -> None:
         """Writes the results of the DataFrame conversion to Arrow format in a cache file with arrow suffix.
 
         Args:
             cache_file_path: The path of the cache file to be written.
             output: The Vaex DataFrame to be saved in the cache file.
         """
         super()._write_cache_file(cache_file_path, output)
-        df_chunks = cache_file_path.parent.glob(f"df_chunk_*.{VaexArrowCacheFormatMixin.cache_file_suffix}")
-        for df_chunk in df_chunks:
-            df_chunk.unlink()
+        clear_directory(cache_file_path.parent, pattern=f"df_chunk_*.{self._cache_file_suffix}")
```

### Comparing `mleko-0.3.1/src/mleko/data/sources/kaggle_data_source.py` & `mleko-0.4.0/mleko/dataset/ingest/kaggle_ingester.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 """A module for downloading and managing Kaggle datasets using the Kaggle API.
 
-This module focuses on the KaggleDataSource class, which provides a convenient way to download and update Kaggle
-datasets by handling credentials, fetching file metadata, downloading files, and keeping the local cache up to date.
-
 In order to use this module, the user must have valid Kaggle API credentials.
 """
 from __future__ import annotations
 
 import json
 import os
 import shutil
@@ -21,19 +18,19 @@
 from requests.auth import HTTPBasicAuth
 from tqdm import tqdm
 
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 from mleko.utils.file_helpers import clear_directory
 
-from .base_data_source import BaseDataSource
+from .base_ingester import BaseIngester
 
 
 logger = CustomLogger()
-"""A CustomLogger instance that's used throughout the module for logging."""
+"""A module-level custom logger."""
 
 
 class KaggleCredentials(NamedTuple):
     """Represents a set of Kaggle API credentials, including a username and API key."""
 
     username: str
     """Username for the Kaggle API."""
@@ -169,38 +166,20 @@
     creation_timestamp: float
     """Timestamp of the file creation."""
 
     total_bytes: int
     """Total size of the file in bytes."""
 
 
-class KaggleDataSource(BaseDataSource):
+class KaggleIngester(BaseIngester):
     """Handles dataset retrieval from Kaggle, downloading and updating files as necessary.
 
-    The KaggleDataSource class downloads files from the specified Kaggle dataset and saves them to the destination
+    The `KaggleIngester` class downloads files from the specified Kaggle dataset and saves them to the destination
     directory. It also checks if the local files are up to date and skips downloading if everything is already in
     place.
-
-    In order to use KaggleDataSource, valid Kaggle API credentials are required. These credentials can be obtained by
-    creating an API token on the Kaggle account settings page. The token should be saved in a JSON file named
-    `kaggle.json` containing the "username" and "key" fields.
-
-    There are three possible locations where Kaggle API credentials can be provided:
-
-    1. Custom file location: Pass the file path to `kaggle_api_credentials_file` in the constructor.
-    2. Environment variables: Set the KAGGLE_USERNAME and KAGGLE_KEY environment variables.
-    3. Default .kaggle folder: Place the `kaggle.json` file into the "~/.kaggle/" directory.
-
-    Note:
-        The Kaggle API is not perfect and sometimes returns incorrect metadata for files, where one or more of the
-        files are missing from the dataset. This can lead to the wrong files being downloaded or the download failing
-        altogether. If you encounter this issue, please report it to Kaggle.
-
-        The issue is observed when the dataset contains a large number of files (e.g. 1000+) or if the dataset contains
-        nested folders.
     """
 
     _KAGGLE_API_VERSION = "v1"
     """The Kaggle API version to use."""
 
     _KAGGLE_DATASET_URL = f"https://www.kaggle.com/api/{_KAGGLE_API_VERSION}/datasets"
     """The base URL for Kaggle dataset API requests."""
@@ -212,49 +191,73 @@
         owner_slug: str,
         dataset_slug: str,
         file_names: list[str] | None = None,
         dataset_version: str | int | None = None,
         kaggle_api_credentials_file: str | Path | None = None,
         num_workers: int = 64,
     ) -> None:
-        """Initializes a KaggleDataSource instance to fetch data from a specific Kaggle dataset.
+        """Initializes a `KaggleIngester` instance to fetch data from a specific Kaggle dataset.
+
+        In order to use `KaggleIngester`, valid Kaggle API credentials are required. These credentials can be obtained
+        by creating an API token on the Kaggle account settings page. The token should be saved in a JSON file named
+        `kaggle.json` containing the "username" and "key" fields.
+
+        There are three possible locations where Kaggle API credentials can be provided:
+
+        1. Custom file location: Pass the file path to `kaggle_api_credentials_file` in the constructor.
+        2. Environment variables: Set the KAGGLE_USERNAME and KAGGLE_KEY environment variables.
+        3. Default .kaggle folder: Place the `kaggle.json` file into the "~/.kaggle/" directory.
+
+        Note:
+            The Kaggle API is not perfect and sometimes returns incorrect metadata for files, where one or more of the
+            files are missing from the dataset. This can lead to the wrong files being downloaded or the download
+            failing altogether. If you encounter this issue, please report it to Kaggle.
+
+            The issue is observed when the dataset contains a large number of files (e.g. 1000+) or if the dataset
+            contains nested folders.
 
         Args:
             destination_directory: The directory where the downloaded files will be stored.
             owner_slug: The owner's Kaggle username or organization name.
             dataset_slug: The dataset's unique Kaggle identifier (slug).
             file_names: A list of file names to download. If not provided or empty, all files in
                 the dataset will be downloaded.
             dataset_version: The specific dataset version number to download. If not provided,
                 the latest version will be fetched.
             kaggle_api_credentials_file: Path to a Kaggle API credentials JSON file. If not
                 provided, environment variables or the default file location will be used.
             num_workers: Number of concurrent threads to use when downloading files.
 
-        Note:
-            The Kaggle API is not perfect and sometimes returns incorrect metadata for files, where one or more of the
-            files are missing from the dataset. This can lead to the wrong files being downloaded or the download
-            failing altogether. If you encounter this issue, please report it to Kaggle.
+        Examples:
+            >>> from mleko.dataset.sources import KaggleIngester
+            >>> kaggle_ingester = KaggleIngester(
+            ...     destination_directory="~/data",
+            ...     owner_slug="allen-institute-for-ai",
+            ...     dataset_slug="covid-19-masks-dataset",
+            ...     file_names=["images.zip", "annotations.json"],
+            ...     dataset_version=1,
+            ... )
+            >>> kaggle_ingester.fetch_data()
+            [PosixPath('~/data/images.zip'), PosixPath('~/data/annotations.json')]
         """
         super().__init__(destination_directory)
-
         self._owner_slug, self._dataset_slug, self._dataset_version = owner_slug, dataset_slug, dataset_version
         self._file_names: set[str] = set(file_names) if file_names is not None else set()
         self._kaggle_config = KaggleCredentialsManager.get_kaggle_credentials(kaggle_api_credentials_file)
         self._num_workers = num_workers
 
-    def fetch_data(self, use_cache: bool = True) -> list[Path]:
+    def fetch_data(self, force_recompute: bool = False) -> list[Path]:
         """Fetches data from the specified Kaggle dataset.
 
         This method downloads files from the Kaggle dataset and returns the local file paths of the downloaded files.
         The method checks if local files are up-to-date and skips downloading if everything is already in place and
-        `use_cache` is set to True.
+        `force_recompute` is set to False.
 
         Args:
-            use_cache: If set to True, the method will check if the local files are up-to-date and
+            force_recompute: If set to False, the method will check if the local files are up-to-date and
                 skip downloading if everything is already in place.
 
         Returns:
             A list of local file paths pointing to the downloaded files.
 
         Raises:
             ValueError: If Kaggle returns 0 files for the given dataset. This could occur if the API is broken.
@@ -268,26 +271,40 @@
         files_metadata = self._kaggle_fetch_files_metadata(params)
 
         if len(files_metadata) == 0:
             error_msg = f"Kaggle returned 0 files for the given dataset {dataset_path}."
             logger.error(error_msg)
             raise ValueError(error_msg)
 
-        if use_cache and self._is_local_dataset_fresh(files_metadata):
-            logger.info("Local dataset is up to date with Kaggle, skipping download.")
+        if not force_recompute and self._is_local_dataset_fresh(files_metadata):
+            logger.info("\033[32mCache Hit\033[0m: Local dataset is up to date with Kaggle, skipping download.")
             return self._get_local_filenames(["gz", "csv", "zip"])
 
         file_names = "*"
         if self._file_names:
             file_names = f"{list(self._file_names)!r}"
-        logger.info(f"Downloading {dataset_path}/{file_names} to {self._destination_directory} from Kaggle.")
+
+        if force_recompute:
+            logger.info(
+                f"\033[33mForce Cache Refresh\033[0m: Downloading {dataset_path}/{file_names} to "
+                f"{self._destination_directory} from Kaggle."
+            )
+        else:
+            logger.info(
+                f"\033[31mCache Miss\033[0m: Downloading {dataset_path}/{file_names} to "
+                f"{self._destination_directory} from Kaggle."
+            )
+
         clear_directory(self._destination_directory)
 
         kaggle_file_paths = [f"{dataset_path}/{file_metadata.name}" for file_metadata in files_metadata]
-        self._kaggle_fetch_files(kaggle_file_paths, params)
+
+        if kaggle_file_paths:
+            self._kaggle_fetch_files(kaggle_file_paths, params)
+            logger.info(f"Finished downloading {len(kaggle_file_paths)} files from Kaggle.")
 
         return self._get_local_filenames(["gz", "csv", "zip"])
 
     def _kaggle_fetch_files_metadata(self, params: dict[str, str]) -> list[KaggleFileMetadata]:
         """Fetch the metadata of the files in the dataset.
 
         When fetching the metadata, the API returns a list of files in the dataset. The list contains the name of the
```

### Comparing `mleko-0.3.1/src/mleko/data/sources/s3_data_source.py` & `mleko-0.4.0/mleko/dataset/ingest/s3_ingester.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,8 @@
-"""Module for fetching data from AWS S3 and storing it locally using the S3DataSource class.
-
-The S3DataSource class provides an interface for downloading specified data from an AWS S3 bucket.
-It allows users to specify the attributes related to the S3 system and configure concurrent downloads.
-This module uses boto3 library for interacting with the AWS API.
-"""
+"""Module for fetching data from AWS S3 and storing it locally using the `S3Ingester` class."""
 from __future__ import annotations
 
 import json
 import os
 from concurrent import futures
 from pathlib import Path
 from typing import Any
@@ -17,25 +12,25 @@
 from botocore.config import Config as BotoConfig
 from tqdm import tqdm
 
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 from mleko.utils.file_helpers import clear_directory
 
-from .base_data_source import BaseDataSource
+from .base_ingester import BaseIngester
 
 
 logger = CustomLogger()
-"""A CustomLogger instance that's used throughout the module for logging."""
+"""A module-level custom logger."""
 
 
-class S3DataSource(BaseDataSource):
-    """S3DataSource provides a convenient interface for fetching data from AWS S3 buckets and storing it locally.
+class S3Ingester(BaseIngester):
+    """`S3Ingester` provides a convenient interface for fetching data from AWS S3 buckets and storing it locally.
 
-    This class extends interacts with AWS S3, allowing users to download specified data from an S3 bucket.
+    This class interacts with AWS S3 to download specified data from an S3 bucket.
     It supports manifest-based caching, enabling more efficient data fetching by verifying if the
     local dataset is up-to-date before downloading.
     """
 
     @auto_repr
     def __init__(
         self,
@@ -46,43 +41,61 @@
         aws_region_name: str = "eu-west-1",
         num_workers: int = 64,
         manifest_file_name: str = "manifest",
         check_s3_timestamps: bool = True,
     ) -> None:
         """Initializes the S3 bucket client, configures the destination directory, and sets client-related parameters.
 
+        Note:
+            The S3 bucket client is initialized using the provided AWS profile and region. If no profile is provided,
+            the default profile will be used. If no region is provided, the default region will be used.
+
+            The profile and region is read from the AWS credentials file located at '~/.aws/credentials'.
+
         Args:
             destination_directory: Directory to store the fetched data locally.
             s3_bucket_name: Name of the S3 bucket containing the data.
             s3_key_prefix: Prefix of the S3 keys for the files to download.
             aws_profile_name: AWS profile name to use.
             aws_region_name: AWS region name where the S3 bucket is located.
             num_workers: Number of workers to use for concurrent downloads.
             manifest_file_name: Name of the manifest file.
             check_s3_timestamps: Whether to check if all S3 files have the same timestamp.
+
+        Examples:
+            >>> from mleko.dataset.sources import S3Ingester
+            >>> s3_ingester = S3Ingester(
+            ...     destination_directory="data",
+            ...     s3_bucket_name="mleko-datasets",
+            ...     s3_key_prefix="kaggle/ashishpatel26/indian-food-101",
+            ...     aws_profile_name="mleko",
+            ...     aws_region_name="eu-west-1",
+            ...     num_workers=64,
+            ...     manifest_file_name="manifest",
+            ...     check_s3_timestamps=True,
+            ... )
+            >>> s3_ingester.fetch_data()
+            [PosixPath('data/indian_food.csv')]
         """
         super().__init__(destination_directory)
-
         self._s3_bucket_name = s3_bucket_name
         self._s3_key_prefix = s3_key_prefix
         self._s3_client = self._get_s3_client(aws_profile_name, aws_region_name)
-
         self._num_workers = num_workers
-
         self._manifest_file_name = manifest_file_name
         self._check_s3_timestamps = check_s3_timestamps
 
-    def fetch_data(self, use_cache: bool = True) -> list[Path]:
+    def fetch_data(self, force_recompute: bool = False) -> list[Path]:
         """Downloads the data from the S3 bucket and stores it in the 'destination_directory'.
 
-        If 'use_cache' is True, verifies whether the data in the local 'destination_directory' is current with the
-        S3 bucket contents based on the manifest file, and skips downloading if it is up to date.
+        If 'force_recompute' is False, verifies whether the data in the local 'destination_directory' is current
+        with the S3 bucket contents based on the manifest file, and skips downloading if it is up to date.
 
         Args:
-            use_cache: Whether to skip downloading if the local data is up to date.
+            force_recompute: Whether to force the data source to recompute its output, even if it already exists.
 
         Raises:
             Exception: If files in the S3 bucket have different last modified dates, indicating potential corruption
                        or duplication.
 
         Returns:
             A list of Path objects pointing to the downloaded data files.
@@ -101,29 +114,40 @@
 
         manifest_file_key = next(
             entry["Key"]
             for entry in resp["Contents"]
             if "Key" in entry and entry["Key"].endswith(self._manifest_file_name)
         )
 
-        if use_cache and manifest_file_key:
+        if not force_recompute and manifest_file_key:
             self._s3_client.download_file(
                 Bucket=self._s3_bucket_name,
                 Key=manifest_file_key,
                 Filename=str(self._destination_directory / self._manifest_file_name),
             )
             with open(self._destination_directory / self._manifest_file_name) as f:
                 manifest: dict[str, Any] = json.load(f)
                 if self._is_local_dataset_fresh(manifest):
-                    logger.info("Local dataset is up to date with S3 bucket contents, skipping download.")
+                    logger.info(
+                        "\033[32mCache Hit\033[0m: Local dataset is up to date with S3 bucket contents, "
+                        "skipping download."
+                    )
                     return self._get_local_filenames(["gz", "csv", "zip"])
 
-        logger.info(
-            f"Downloading {self._s3_bucket_name}/{self._s3_key_prefix} to {self._destination_directory} from S3."
-        )
+        if force_recompute:
+            logger.info(
+                f"\033[33mForce Cache Refresh\033[0m: Downloading {self._s3_bucket_name}/{self._s3_key_prefix} to "
+                f"{self._destination_directory} from S3."
+            )
+        else:
+            logger.info(
+                f"\033[31mCache Miss\033[0m: Downloading {self._s3_bucket_name}/{self._s3_key_prefix} to "
+                f"{self._destination_directory} from S3."
+            )
+
         clear_directory(self._destination_directory)
         keys_to_download = [
             entry["Key"]
             for entry in resp["Contents"]
             if "Key" in entry and (entry["Key"].endswith(".csv") or entry["Key"].endswith(".gz"))
         ]
```

### Comparing `mleko-0.3.1/src/mleko/pipeline/__init__.py` & `mleko-0.4.0/mleko/pipeline/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Pipeline subpackage for managing and executing data processing steps.
 
 This subpackage provides the necessary components to create a customizable data processing pipeline. It includes
 abstract base classes for pipeline steps, a flexible and customizable Pipeline class for managing and executing a
 series of data processing steps, and a subpackage named `steps` that contains concrete implementations of the
 `PipelineStep` class.
 """
+from __future__ import annotations
+
 from .data_container import DataContainer
 from .pipeline import Pipeline
 from .pipeline_step import PipelineStep
 
 
 __all__ = ["Pipeline", "PipelineStep", "DataContainer"]
```

### Comparing `mleko-0.3.1/src/mleko/pipeline/data_container.py` & `mleko-0.4.0/mleko/pipeline/data_container.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,18 +13,27 @@
 
 @dataclass
 class DataContainer:
     """Class for holding data used in the pipeline.
 
     This class serves as a common interface and can be extended to enforce
     a shared structure or behavior across different types of data.
+
+    Examples:
+        >>> data_container = DataContainer()
+        >>> data_container.data["my_data"] = [Path("path/to/data")]
+        >>> data_container.data["my_data"]
+        [Path("path/to/data")]
     """
 
     data: dict[str, list[Path] | vaex.DataFrame] = field(default_factory=dict)
-    """The data stored in the DataContainer."""
+    """The data stored in the DataContainer.
+
+    The data is stored in a dictionary, where the keys are the names of the data and the values are the data itself.
+    """
 
     def __repr__(self) -> str:
         """Get string representation of DataContainer.
 
         Returns:
             String representation of the DataContainer, including data type and stored data.
         """
```

### Comparing `mleko-0.3.1/src/mleko/pipeline/pipeline.py` & `mleko-0.4.0/mleko/pipeline/pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,64 +19,66 @@
 
 class Pipeline:
     """Encapsulates a pipeline that manages and executes a series of data processing steps in a defined order."""
 
     def __init__(self, steps: list[PipelineStep] | None = None) -> None:
         """Creates a new Pipeline instance, initializing it with a list of steps or an empty list.
 
-        Args:
-            steps: An optional list of `PipelineStep` instances that define the data processing steps in the
-                   pipeline. If not provided, the pipeline will be initialized with an empty list of steps,
-                   allowing steps to be added later using the `add_step` method.
-
         Note:
             The steps list can be provided as an argument to the constructor, or the pipeline can be initialized
             with an empty list of steps and have them added later using the `add_step` method. This allows for
             more flexibility in the creation of the pipeline, as steps can be added dynamically.
+
+        Args:
+            steps: An optional list of `PipelineStep` instances that define the data processing steps in the
+                   pipeline. If not provided, the pipeline will be initialized with an empty list of steps,
+                   allowing steps to be added later using the `add_step` method.
         """
-        self.steps = steps if steps is not None else []
+        self._steps = steps if steps is not None else []
 
     def __repr__(self) -> str:
         """Returns a string representation of the Pipeline, including the ordered list of steps.
 
         Returns:
             String representaition of Pipeline that includes the class name and each step in the order they appear
             in the pipeline, numbered for easier identification.
         """
         cls_name = type(self).__name__
-        steps_str = "\n".join([f"  {index + 1}. {step!r}" for index, step in enumerate(self.steps)])
+        steps_str = "\n".join([f"  {index + 1}. {step!r}" for index, step in enumerate(self._steps)])
         return f"{cls_name}:\n{steps_str}"
 
     def add_step(self, step: PipelineStep) -> None:
         """Appends a new PipelineStep to the end of the pipeline, extending the processing sequence.
 
         Adding a step to the pipeline implies that it will be executed after all the steps previously
         appended to the pipeline when calling the `run` method.
 
         Args:
             step: The PipelineStep instance to be added at the end of the pipeline's steps list.
         """
-        self.steps.append(step)
+        self._steps.append(step)
 
-    def run(self, data_container: DataContainer | None = None) -> DataContainer:
+    def run(self, data_container: DataContainer | None = None, force_recompute: bool = False) -> DataContainer:
         """Executes the pipeline steps in the order they were added, passing output from one to the next.
 
         Processes the initial given data or an empty data container through each step in the pipeline.
         The output of each step is passed as input to the next step, allowing the given input to be transformed
         through the whole sequence of steps.
 
         Args:
             data_container: An optional DataContainer instance carrying the input data to be processed by the
                             first step in the pipeline. If not provided, an empty DataContainer instance will be
                             created automatically, and the first step's execute method must handle it.
+            force_recompute: Whether to force the pipeline to recompute its output, even if it already exists.
 
         Returns:
             The output as a DataContainer instance from the last step in the pipeline after processing the data.
         """
         if data_container is None:
+            logger.info("No data container provided. Creating an empty one.")
             data_container = DataContainer()
 
-        for i, step in enumerate(self.steps):
-            logger.info(f"Executing step {i+1}: {step.__class__.__name__}")
-            data_container = step.execute(data_container)
-            logger.info(f"Finished step {i+1}")
+        for i, step in enumerate(self._steps):
+            logger.info(f"Executing step {i+1}/{len(self._steps)}: {step.__class__.__name__}.")
+            data_container = step.execute(data_container, force_recompute)
+            logger.info(f"Finished step {i+1}/{len(self._steps)} execution.")
         return data_container
```

### Comparing `mleko-0.3.1/src/mleko/pipeline/pipeline_step.py` & `mleko-0.4.0/mleko/pipeline/pipeline_step.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,23 +43,24 @@
         self.inputs = tuple(inputs)
         self.outputs = tuple(outputs)
 
         self._validate_inputs()
         self._validate_outputs()
 
     @abstractmethod
-    def execute(self, data_container: DataContainer) -> DataContainer:
+    def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
         """Execute the data processing operation associated with this pipeline step.
 
-        The input data to be processed is passed via `data_container`, and the structure depends on the specific
-        implementation. After the operation, the method returns the processed data in the form of a `DataContainer`,
-        which includes the data and an enum determining the data type.
+        The `execute` method is the main entry point for the data processing operation associated with this step.
+        It receives a `DataContainer` instance as input, containing the data to be processed by this step.
+        The method should perform the processing operation and return the processed data as a `DataContainer` instance.
 
         Args:
             data_container: Input data for this step's processing operation.
+            force_recompute: Whether to force the step to recompute its output, even if it already exists.
 
         Raises:
             NotImplementedError: Must be implemented by subclass.
 
         Returns:
             Processed data as a `DataContainer`.
         """
```

### Comparing `mleko-0.3.1/src/mleko/pipeline/steps/__init__.py` & `mleko-0.4.0/mleko/pipeline/steps/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """Subpackage containing specialized pipeline steps for various data processing tasks.
 
 This subpackage offers a collection of pipeline steps, each designed for a specific purpose: data ingestion,
 data conversion, and other data manipulation tasks. By using these unique steps sequentially, you can create a
 complete data processing workflow within the pipeline.
 """
-from .convert import ConvertStep
-from .ingest import IngestStep
-from .split import SplitStep
+from __future__ import annotations
 
+from .convert_step import ConvertStep
+from .feature_select_step import FeatureSelectStep
+from .ingest_step import IngestStep
+from .split_step import SplitStep
 
-__all__ = ["IngestStep", "ConvertStep", "SplitStep"]
+
+__all__ = ["IngestStep", "ConvertStep", "SplitStep", "FeatureSelectStep"]
```

### Comparing `mleko-0.3.1/src/mleko/pipeline/steps/convert.py` & `mleko-0.4.0/mleko/pipeline/steps/convert_step.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This module contains the `ConvertStep` class which is a specialized pipeline step for handling data format
 conversion. It uses the provided `BaseDataConverter` for converting the data into the desired format.
 """
 from __future__ import annotations
 
 from pathlib import Path
 
-from mleko.data.converters import BaseDataConverter
+from mleko.dataset.convert import BaseConverter
 from mleko.pipeline.data_container import DataContainer
 from mleko.pipeline.pipeline_step import PipelineStep
 from mleko.utils.decorators import auto_repr
 
 
 class ConvertStep(PipelineStep):
     """Pipeline step that manages data conversion from one format to another."""
@@ -21,40 +21,41 @@
 
     _num_outputs = 1
     """Number of outputs expected by the ConvertStep."""
 
     @auto_repr
     def __init__(
         self,
-        converter: BaseDataConverter,
+        converter: BaseConverter,
         inputs: list[str] | tuple[str, ...] | tuple[()] = (),
         outputs: list[str] | tuple[str, ...] | tuple[()] = (),
     ) -> None:
         """Initialize the ConvertStep with the specified data converter.
 
         Args:
             converter: The DataConverter responsible for handling data format conversion.
             inputs: List or tuple of input keys expected by this step.
             outputs: List or tuple of output keys produced by this step.
         """
         super().__init__(inputs, outputs)
         self._converter = converter
 
-    def execute(self, data_container: DataContainer) -> DataContainer:
+    def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
         """Perform data format conversion using the configured converter.
 
         Args:
             data_container: Contains a list of file Paths to be converted.
+            force_recompute: Whether to force the step to recompute its output, even if it already exists.
 
         Raises:
             ValueError: If data container contains invalid data - not a list of Paths.
 
         Returns:
             A DataContainer containing the converted data as a vaex dataframe.
         """
         file_paths = data_container.data[self.inputs[0]]
         if not isinstance(file_paths, list) or not all(isinstance(e, Path) for e in file_paths):
             raise ValueError
 
-        df = self._converter.convert(file_paths)
+        df = self._converter.convert(file_paths, force_recompute)
         data_container.data[self.outputs[0]] = df
         return data_container
```

### Comparing `mleko-0.3.1/src/mleko/pipeline/steps/ingest.py` & `mleko-0.4.0/mleko/pipeline/steps/ingest_step.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Module handling data ingestion from a data source in the pipeline process.
 
 This module contains the `IngestStep` class which is a specialized pipeline step designed for handling data
-fetching from a specified `BaseDataSource`. It's responsible for retrieving data from the data source, and
+fetching from a specified `BaseIngester`. It's responsible for retrieving data from the data source, and
 returning a `DataContainer` object containing the list of fetched files.
 """
 from __future__ import annotations
 
-from mleko.data.sources import BaseDataSource
+from mleko.dataset.ingest import BaseIngester
 from mleko.pipeline.data_container import DataContainer
 from mleko.pipeline.pipeline_step import PipelineStep
 from mleko.utils import auto_repr
 
 
 class IngestStep(PipelineStep):
     """Pipeline step that manages data ingestion from a configured data source."""
@@ -20,33 +20,34 @@
 
     _num_outputs = 1
     """Number of outputs expected by the IngestStep."""
 
     @auto_repr
     def __init__(
         self,
-        data_source: BaseDataSource,
+        ingester: BaseIngester,
         inputs: list[str] | tuple[str, ...] | tuple[()] = (),
         outputs: list[str] | tuple[str, ...] | tuple[()] = (),
     ) -> None:
         """Initialize the IngestStep with the specified data source.
 
         Args:
-            data_source: The data source from which to fetch the data, a BaseDataSource instance.
+            ingester: The data source from which to fetch the data, a BaseIngester instance.
             inputs: List or tuple of input keys expected by this step.
             outputs: List or tuple of output keys produced by this step.
         """
         super().__init__(inputs, outputs)
-        self._data_source = data_source
+        self._ingester = ingester
 
-    def execute(self, _data_container: DataContainer) -> DataContainer:
+    def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
         """Fetch data from the configured data source and return a DataContainer with fetched files.
 
-        The `_data_container` parameter is unused in this step as this operation only deals with data ingestion
-        and no input data is required.
+        Args:
+            data_container: Input data for this step's processing operation.
+            force_recompute: Whether to force the step to recompute its output, even if it already exists.
 
         Returns:
             DataContainer: A DataContainer containing a list of fetched files.
         """
-        files = self._data_source.fetch_data()
-        _data_container.data[self.outputs[0]] = files
-        return _data_container
+        files = self._ingester.fetch_data(force_recompute)
+        data_container.data[self.outputs[0]] = files
+        return data_container
```

### Comparing `mleko-0.3.1/src/mleko/pipeline/steps/split.py` & `mleko-0.4.0/mleko/pipeline/steps/split_step.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,59 +3,60 @@
 This module contains the SplitStep class, which is responsible for splitting a DataFrame into two parts.
 It uses a BaseDataSplitter to perform the actual splitting.
 """
 from __future__ import annotations
 
 from vaex import DataFrame
 
-from mleko.data.splitters import BaseDataSplitter
+from mleko.dataset.split.base_splitter import BaseSplitter
 from mleko.pipeline.data_container import DataContainer
 from mleko.pipeline.pipeline_step import PipelineStep
 from mleko.utils.decorators import auto_repr
 
 
 class SplitStep(PipelineStep):
-    """Pipeline step that splits a DataFrame in two."""
+    """Pipeline step that splits a DataFrame into two parts."""
 
     _num_inputs = 1
     """Number of inputs expected by the SplitStep."""
 
     _num_outputs = 2
     """Number of outputs expected by the SplitStep."""
 
     @auto_repr
     def __init__(
         self,
-        splitter: BaseDataSplitter,
+        splitter: BaseSplitter,
         inputs: list[str] | tuple[str, ...] | tuple[()] = (),
         outputs: list[str] | tuple[str, ...] | tuple[()] = (),
     ) -> None:
         """Initialize the SplitStep with the specified data splitter.
 
         Args:
             splitter: The DataSplitter responsible for handling data splitting.
             inputs: List or tuple of input keys expected by this step.
             outputs: List or tuple of output keys produced by this step.
         """
         super().__init__(inputs, outputs)
         self._splitter = splitter
 
-    def execute(self, data_container: DataContainer) -> DataContainer:
+    def execute(self, data_container: DataContainer, force_recompute: bool) -> DataContainer:
         """Perform data splitting using the configured splitter.
 
         Args:
             data_container: Contains the DataFrame to be split.
+            force_recompute: Whether to force the step to recompute its output, even if it already exists.
 
         Raises:
             ValueError: If data container contains invalid data - not a vaex DataFrame.
 
         Returns:
             A DataContainer containing the split data as two vaex DataFrames.
         """
         dataframe = data_container.data[self.inputs[0]]
         if not isinstance(dataframe, DataFrame):
             raise ValueError
 
-        df_first, df_second = self._splitter.split(dataframe)
-        data_container.data[self.outputs[0]] = df_first
-        data_container.data[self.outputs[1]] = df_second
+        df1, df2 = self._splitter.split(dataframe, force_recompute)
+        data_container.data[self.outputs[0]] = df1
+        data_container.data[self.outputs[1]] = df2
         return data_container
```

### Comparing `mleko-0.3.1/src/mleko/utils/custom_logger.py` & `mleko-0.4.0/mleko/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.1/src/mleko/utils/decorators.py` & `mleko-0.4.0/mleko/utils/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,28 +17,39 @@
 
 This TypeVar is designed for type hinting in decorators in the module. It essentially states that F can be
 a function with any number of arguments and any return type.
 """
 
 
 def auto_repr(init_method: F) -> F:
-    """Decorator for generating a __repr__ method for a class automatically based on the __init__ method signature.
+    """Decorator for generating a `__repr__` method for a class automatically based on the `__init__` method signature.
 
-    The decorator inspects the __init__ method's signature and uses parameter names and values to create a __repr__
+    The decorator inspects the `__init__` method's signature and uses parameter names and values to create a `__repr__`
     method that represents the class instance.
 
     Args:
-        init_method: The __init__ method of the class to be decorated.
+        init_method: The `__init__` method of the class to be decorated.
 
     Returns:
-        The wrapped __init__ method with an automatically generated __repr__ method.
+        The wrapped `__init__` method with an automatically generated `__repr__` method.
+
+    Examples:
+        >>> from mleko.utils import auto_repr
+        >>> class TestClass:
+        ...     @auto_repr
+        ...     def __init__(self, param1: int, param2: str = "default"):
+        ...         self.param1 = param1
+        ...         self.param2 = param2
+        >>> test_instance = TestClass(1, "test")
+        >>> test_instance
+        TestClass(param1=1, param2='test')
     """
 
     @wraps(init_method)
-    def wrapped_init(self: Any, *args: Any, **kwargs: dict[str, Any]) -> None:
+    def wrapped_init(self: Any, *args: Any, **kwargs: Any) -> None:
         init_method(self, *args, **kwargs)
 
         signature = inspect.signature(init_method)
         parameter_names = list(signature.parameters.keys())[1:]
         parameter_values = dict(zip(parameter_names, args))
 
         for key, param in signature.parameters.items():
@@ -57,23 +68,35 @@
 
     return cast(F, wrapped_init)
 
 
 def timing(func: F) -> F:
     """A decorator that logs the execution time of the decorated function using a CustomLogger instance.
 
+    Warning:
+        On certain platforms, the timing may be inaccurate due to OS scheduling. This is a known issue with some
+        MacOS versions.
+
     Args:
         func: The function to be decorated.
 
     Returns:
         The wrapped function that logs its execution time.
+
+    Example:
+        >>> from mleko.utils import timing
+        >>> @timing
+        ... def test_func():
+        ...     pass
+        >>> test_func()
+        Function: test_func    Timing: 0.0000s
     """
 
     @wraps(func)
-    def wrap(*args: Any, **kwargs: dict[str, Any]) -> Any:
+    def wrap(*args: Any, **kwargs: Any) -> Any:
         ts = perf_counter()
         result = func(*args, **kwargs)
         te = perf_counter()
         elapsed_time = te - ts
         logger.debug(f"Function: {func.__qualname__}    Timing: {elapsed_time:.4f}s")
         return result
```

### Comparing `mleko-0.3.1/src/mleko/utils/file_helpers.py` & `mleko-0.4.0/mleko/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.3.1/src/mleko/utils/vaex.py` & `mleko-0.4.0/mleko/utils/vaex_helpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-"""Utility functions for working with Vaex DataFrames.
-
-This module provides utility functions that help with extracting specific columns
-and rows from Vaex DataFrames.
-"""
+"""This module contains helper functions for working with `vaex` DataFrames."""
 from __future__ import annotations
 
 import vaex
 
 
 def get_column(df: vaex.DataFrame, column: str) -> vaex.Expression:
     """Get specified column from a DataFrame as an Expression.
@@ -17,38 +13,77 @@
 
     Returns:
         The specified column as an Expression.
     """
     return df[column]
 
 
-def get_columns(df: vaex.DataFrame, columns: list[str] | vaex.Expression) -> vaex.DataFrame:
+def get_columns(df: vaex.DataFrame, columns: list[str]) -> vaex.DataFrame:
     """Get specified columns from a DataFrame.
 
     Args:
         df: The input DataFrame.
         columns: A list of the names of the desired columns or an Expression.
-            If an Expression is provided, it is assumed to be a boolean mask
-            that can be used to filter the DataFrame.
 
     Returns:
         A DataFrame containing only the specified columns.
+
+    Examples:
+        >>> import vaex
+        >>> from mleko.utils import get_columns
+        >>> df = vaex.from_arrays(column1=[1, 2, 3], column2=[4, 5, 6], column3=[7, 8, 9])
+        >>> get_columns(df, ["column1", "column3"]).get_column_names()
+        ['column1', 'column3']
     """
     return df[columns]
 
 
+def get_filtered_df(df: vaex.DataFrame, filter: vaex.Expression) -> vaex.DataFrame:
+    """Get filtered DataFrame.
+
+    Will return a DataFrame containing only the rows that satisfy the filter. The filter is an Expression that
+    evaluates to a boolean value for each row.
+
+    Args:
+        df: The input DataFrame.
+        filter: A boolean Expression used to filter the DataFrame.
+
+    Returns:
+        A DataFrame containing only the rows that satisfy the filter.
+
+    Examples:
+        >>> import vaex
+        >>> from mleko.utils import get_filtered_df
+        >>> df = vaex.from_arrays(column1=[1, 2, 3], column2=[4, 5, 6], column3=[7, 8, 9])
+        >>> get_filtered_df(df, df.column1 > 1)
+        #    column1    column2    column3
+        0          2          5          8
+        1          3          6          9
+    """
+    return df[filter]
+
+
 def get_indices(df: vaex.DataFrame, indices: list[int]) -> vaex.DataFrame:
-    """Get specified row indices from a DataFrame.
+    """Get DataFrame containing only the specified indices.
 
     Args:
         df: The input DataFrame.
-        indices: A list of row indices to extract from the DataFrame.
+        indices: A list of the indices to be extracted.
 
     Returns:
-        A DataFrame containing rows for the specified indices.
+        A DataFrame containing only the specified indices.
+
+    Examples:
+        >>> import vaex
+        >>> from mleko.utils import get_indices
+        >>> df = vaex.from_arrays(column1=[1, 2, 3], column2=[4, 5, 6], column3=[7, 8, 9])
+        >>> get_indices(df, [0, 2])
+        #    column1    column2    column3
+        0          1          4          7
+        1          3          6          9
     """
     idx_name = "index"
     df[idx_name] = vaex.vrange(0, df.shape[0])
     index = get_column(df, idx_name)
-    selection = get_columns(df, index.isin(indices))
+    selection = get_filtered_df(df, index.isin(indices))
     selection.delete_virtual_column(idx_name)
     return selection.extract()
```

### Comparing `mleko-0.3.1/PKG-INFO` & `mleko-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: mleko
-Version: 0.3.1
+Version: 0.4.0
 Summary: ML-Ekosystem
 Home-page: https://github.com/ErikBavenstrand/mleko
 License: MIT
 Author: Erik Båvenstrand
 Author-email: erik@bavenstrand.se
 Requires-Python: >=3.8.0,<3.11.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: boto3 (>=1.26.91,<2.0.0)
 Requires-Dist: botocore (>=1.29.91,<2.0.0)
+Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: vaex (>=4.16.0,<5.0.0)
-Project-URL: Changelog, https://github.com/ErikBavenstrand/mleko/releases
+Project-URL: Changelog, https://github.com/ErikBavenstrand/mleko/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://mleko.readthedocs.io
 Project-URL: Repository, https://github.com/ErikBavenstrand/mleko
 Description-Content-Type: text/markdown
 
 # ML-Ekosystem
 
 [![PyPI](https://img.shields.io/pypi/v/mleko.svg)][pypi_]
```

