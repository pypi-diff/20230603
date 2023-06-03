# Comparing `tmp/stocktracer-0.3.0.tar.gz` & `tmp/stocktracer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "stocktracer-0.4.0.tar", max compression
```

## Comparing `stocktracer-0.3.0.tar` & `stocktracer-0.4.0.tar`

### file list

```diff
@@ -1,73 +1,18 @@
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 stocktracer-0.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 stocktracer-0.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 stocktracer-0.3.0/Makefile
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 stocktracer-0.3.0/Pipfile
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 stocktracer-0.3.0/SECURITY.md
--rwxr-xr-x   0        0        0      617 2020-02-02 00:00:00.000000 stocktracer-0.3.0/auto-format.sh
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 stocktracer-0.3.0/conftest.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 stocktracer-0.3.0/mkdocs.yml
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 stocktracer-0.3.0/pydocktest.json
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 stocktracer-0.3.0/requirements.txt
--rwxr-xr-x   0        0        0      757 2020-02-02 00:00:00.000000 stocktracer-0.3.0/smoke-test.sh
--rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 stocktracer-0.3.0/verify-packaging.sh
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/pull_request_template.md
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/release.yml
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/workflows/cleanup.yml
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/workflows/python.yml
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/workflows/release-test.yml
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/getting-started.md
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/index.md
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/design/analysis.md
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/design/caching.md
--rw-r--r--   0        0        0    20504 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/design/data-retrieval.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/design/index.md
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/design/reference.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/design/report.md
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/javascripts/mathjax.js
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/javascripts/tablesort.js
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 stocktracer-0.3.0/docs/stylesheets/extra.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/__init__.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/__main__.py
--rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/cli.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/filter.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/interface.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/analysis/__init__.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/analysis/annual_reports.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/analysis/diluted_eps.py
--rw-r--r--   0        0        0     7289 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/analysis/f_score.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/analysis/stub.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/data/__init__.py
--rw-r--r--   0        0        0    31671 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/stocktracer/data/sec.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/__init__.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/test_cli.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/test_filter.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/analysis/__init__.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/analysis/test_annual_reports.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/analysis/test_diluted_eps.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/analysis/test_f_score.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/analysis/test_stub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/fixtures/network.py
--rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/fixtures/unit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/sec/__init__.py
--rw-r--r--   0        0        0     6507 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/sec/test_DataSelector.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/sec/test_DataSetReader.py
--rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/sec/test_filter.py
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/sec/test_network.py
--rw-r--r--   0        0        0     8600 2020-02-02 00:00:00.000000 stocktracer-0.3.0/src/tests/sec/test_sec.py
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 stocktracer-0.3.0/.gitignore
--rw-r--r--   0        0        0    14197 2020-02-02 00:00:00.000000 stocktracer-0.3.0/LICENSE
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 stocktracer-0.3.0/README.md
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 stocktracer-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    22066 2020-02-02 00:00:00.000000 stocktracer-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    14197 2023-06-03 15:54:43.958300 stocktracer-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2703 2023-06-03 15:54:43.958300 stocktracer-0.4.0/README.md
+-rw-r--r--   0        0        0     4618 2023-06-03 15:54:43.958300 stocktracer-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-03 15:54:43.958300 stocktracer-0.4.0/src/stocktracer/__init__.py
+-rw-r--r--   0        0        0      929 2023-06-03 15:54:43.958300 stocktracer-0.4.0/src/stocktracer/__main__.py
+-rw-r--r--   0        0        0       51 2023-06-03 15:54:43.958300 stocktracer-0.4.0/src/stocktracer/analysis/__init__.py
+-rw-r--r--   0        0        0     1850 2023-06-03 15:54:43.958300 stocktracer-0.4.0/src/stocktracer/analysis/annual_reports.py
+-rw-r--r--   0        0        0     1094 2023-06-03 15:54:43.958300 stocktracer-0.4.0/src/stocktracer/analysis/diluted_eps.py
+-rw-r--r--   0        0        0     7287 2023-06-03 15:54:43.962300 stocktracer-0.4.0/src/stocktracer/analysis/f_score.py
+-rw-r--r--   0        0        0      678 2023-06-03 15:54:43.962300 stocktracer-0.4.0/src/stocktracer/analysis/stub.py
+-rw-r--r--   0        0        0     3410 2023-06-03 15:54:43.962300 stocktracer-0.4.0/src/stocktracer/analysis/tensorflow.py
+-rw-r--r--   0        0        0     2007 2023-06-03 15:54:43.962300 stocktracer-0.4.0/src/stocktracer/cache.py
+-rw-r--r--   0        0        0     5157 2023-06-03 15:54:43.962300 stocktracer-0.4.0/src/stocktracer/cli.py
+-rw-r--r--   0        0        0       70 2023-06-03 15:54:43.962300 stocktracer-0.4.0/src/stocktracer/collector/__init__.py
+-rw-r--r--   0        0        0    29758 2023-06-03 15:54:43.962300 stocktracer-0.4.0/src/stocktracer/collector/sec.py
+-rw-r--r--   0        0        0      719 2023-06-03 15:54:43.962300 stocktracer-0.4.0/src/stocktracer/filter.py
+-rw-r--r--   0        0        0      890 2023-06-03 15:54:43.962300 stocktracer-0.4.0/src/stocktracer/interface.py
+-rw-r--r--   0        0        0     4443 1970-01-01 00:00:00.000000 stocktracer-0.4.0/PKG-INFO
```

### Comparing `stocktracer-0.3.0/src/stocktracer/__main__.py` & `stocktracer-0.4.0/src/stocktracer/__main__.py`

 * *Files identical despite different names*

### Comparing `stocktracer-0.3.0/src/stocktracer/cli.py` & `stocktracer-0.4.0/src/stocktracer/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """This is the CLI class for stocktracer."""
 import importlib
 import io
 import logging
-import os
 import warnings
 from pathlib import Path
 from typing import Literal, Optional, Union
 
 import pandas as pd
 from beartype import beartype
 from beartype.typing import Sequence, Tuple
-from diskcache import Cache
 
+from stocktracer import cache
 from stocktracer.interface import Analysis as AnalysisInterface
 from stocktracer.interface import Options as CliOptions
+from stocktracer.interface import ReportDate
 
 logger = logging.getLogger(__name__)
 
 
 @beartype
 def get_analysis_instance(module_name: str, options: CliOptions) -> AnalysisInterface:
     """Dynamically import and load the Analysis class from a module.
@@ -32,99 +32,66 @@
     module = importlib.import_module(module_name)
     class_ = getattr(module, "Analysis")
     instance = class_(options)
     assert isinstance(instance, AnalysisInterface)
     return instance
 
 
-@beartype
-def get_default_cache_path() -> Path:
-    """Get the default path for caching data.
-
-    Returns:
-        Path: path to cache data
-    """
-    return Path(os.getcwd()) / ".ticker-cache"
-
-
 ReportFormat = Literal["csv", "md", "json", "txt"]
 
 
 @beartype
 class Cli:
     """Tools for gathering resources, analyzing data, and publishing the results."""
 
     return_results: bool = True
 
     def analyze(  # pylint: disable=too-many-arguments
         self,
         tickers: Union[Sequence[str], str],
-        cache_path: Path | str = get_default_cache_path(),
-        refresh: bool = False,
         analysis_plugin: str = "stocktracer.analysis.annual_reports",
-        final_year: Optional[int] = None,
-        final_quarter: Optional[int] = None,
+        final_year: int = ReportDate().year,
+        final_quarter: int = ReportDate().quarter,
         report_format: ReportFormat = "txt",
         report_file: Optional[Path | str] = None,
     ) -> Optional[pd.DataFrame]:
         """Perform stock analysis.
 
         Args:
             tickers (Union[Sequence[str], str]): tickers to include in the analysis
-            cache_path (Path | str): path where to cache data
-            refresh (bool): Whether to refresh the calculation or use the results from a prior one
             analysis_plugin (str): module to load for analysis
-            final_year (Optional[int]): last year to consider for report collection
-            final_quarter (Optional[int]): last quarter to consider for report collection
+            final_year (int): last year to consider for report collection
+            final_quarter (int): last quarter to consider for report collection
             report_format (ReportFormat): Format of the report. Options include: csv, json, md (markdown)
             report_file (Optional[Path | str]): Where to store the report. Required if report_format is specified.
 
-        Raises:
-            LookupError: no analysis results found
-
         Returns:
             Optional[pd.DataFrame]: results of analysis
         """
-        cache_path = Path(cache_path)
         if report_file:
             report_file = Path(report_file)
+        tickers_set = set()
         if isinstance(tickers, str):
-            tickers = frozenset([tickers])
+            tickers_set.add(tickers)
         else:
-            tickers = frozenset(tickers)
-
-        analysis_module: AnalysisInterface = get_analysis_instance(
-            analysis_plugin,
-            CliOptions(
-                tickers=tickers,
-                cache_path=cache_path,
-                final_year=final_year,
-                final_quarter=final_quarter,
-            ),
-        )
-
-        cache, results_key, results = self._get_cached_results(
-            tickers, cache_path, analysis_plugin
+            tickers_set = set()
+            for t in tickers:
+                tickers_set.add(t)
+
+        # prep for caching
+        tickers_list = list(tickers_set)
+        tickers_list.sort()
+
+        results, analysis_module = self._get_result(
+            tickers=tickers_list,
+            analysis_plugin=analysis_plugin,
+            final_year=final_year,
+            final_quarter=final_quarter,
         )
 
-        if (
-            refresh
-            or results is None
-            or not isinstance(results, pd.DataFrame)
-            or results.empty
-        ):
-            # Call analysis plugin
-            results = None
-            results = analysis_module.analyze()
-            if results is None or results.empty:
-                raise LookupError("No analysis results available!")
-
-            # Save one week expiry
-            cache.set(key=results_key, value=results, expire=3600 * 24 * 7)
-
         self._generate_report(report_format, report_file, results)
         if analysis_module.under_development:
             warnings.warn(
                 "This analysis module is under development and may be incorrect, incomplete, or may change."
             )
         if self.return_results:
             return results
@@ -148,35 +115,43 @@
             case "json":
                 results.to_json(report_file)
             case "txt":
                 results.to_string(report_file)
         if isinstance(report_file, io.StringIO):
             print(report_file.getvalue())
 
-    def _get_cached_results(
-        self, tickers, cache_path, analysis_plugin
-    ) -> Tuple[Cache, str, Optional[pd.DataFrame]]:
-        assert isinstance(tickers, frozenset)
-        cache = Cache(directory=cache_path / "results")
-        results_key = get_cached_results_key(tickers, analysis_plugin)
-        results = cache.get(key=results_key, default=None)
-        return cache, results_key, results
-
+    @cache.results.memoize(typed=True, expire=60 * 60 * 24 * 7, tag="results")
+    def _get_result(
+        self,
+        tickers: list[str],
+        analysis_plugin: str,
+        final_year: int,
+        final_quarter: int,
+    ) -> Tuple[Optional[pd.DataFrame], AnalysisInterface]:
+        """Gets the results.
 
-@beartype
-def get_cached_results_key(tickers: frozenset[str], analysis_module: str) -> str:
-    """Get the key used for caching results from analyzed data.
+        Args:
+            tickers (list[str]): _description_
+            analysis_plugin (str): _description_
+            final_year (int): _description_
+            final_quarter (int): _description_
 
-    >>> get_cached_results_key(frozenset({"aapl","msft"}),"my.analysis")
-    'my.analysis-aapl-msft'
+        Raises:
+            LookupError: no analysis results found
 
-    Args:
-        tickers (frozenset[str]): tickers to check
-        analysis_module (str): name of analysis module
+        Returns:
+            Tuple[Optional[pd.DataFrame], AnalysisInterface]: _description_
+        """
+        analysis_module: AnalysisInterface = get_analysis_instance(
+            analysis_plugin,
+            CliOptions(
+                tickers=tickers,
+                final_report=ReportDate(year=final_year, quarter=final_quarter),
+            ),
+        )
 
-    Returns:
-        str: string with the cached key
-    """
-    sorted_tickers = list(tickers)
-    sorted_tickers.sort()
-    results_key = "-".join(sorted_tickers)
-    return "-".join((analysis_module, results_key))
+        # Call analysis plugin
+        results = None
+        results = analysis_module.analyze()
+        if results is None:
+            raise LookupError("No analysis results available!")
+        return results, analysis_module
```

### Comparing `stocktracer-0.3.0/src/stocktracer/filter.py` & `stocktracer-0.4.0/src/stocktracer/filter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 """Filter Interface.
 
 This may be removed or deprecated in the future. TBD.
 """
+from dataclasses import dataclass
+
 from beartype import beartype
 
-from stocktracer.data.sec import Filter as SecFilter
+from stocktracer.collector.sec import Filter as SecFilter
 
 
 @beartype
+@dataclass(frozen=True)
 class Selectors:
     """Selectors provide an aggregation point for a number of built-in filter mechanics.
 
     The original intent for this was to provide a bag to throw a bunch of filters in. However,
     analysis modules somewhat replace this concept by giving finer grained control over what
     filters get applied. This may go away in the future pending a determination whether or not
     the class is needed.
     """
 
-    def __init__(
-        self, ticker_filter: set[str] | list[str], sec_filter: SecFilter
-    ) -> None:
-        """Entry for data to search for in various sources.
-
-        Args:
-            ticker_filter (set[str] | list[str]): list of stock tickers to get information about
-            sec_filter (SecFilter): filter for SEC reports
-        """
-        self.ticker_filter = frozenset(ticker_filter)
-        self.sec_filter = sec_filter
+    ticker_filter: list[str]
+    sec_filter: SecFilter
```

### Comparing `stocktracer-0.3.0/src/stocktracer/interface.py` & `stocktracer-0.4.0/src/stocktracer/interface.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,37 @@
 """Interfaces for the StockTracer Module."""
 import abc
-from pathlib import Path
+from dataclasses import dataclass
 from typing import Optional
 
 from beartype import beartype
 from pandas import DataFrame
 
-from stocktracer.data.sec import ReportDate
+from stocktracer.collector.sec import ReportDate
 
 
 @beartype
+@dataclass(frozen=True)
 class Options:
     """Command Line Options."""
 
-    def __init__(
-        self,
-        tickers: frozenset[str],
-        cache_path: Path,
-        final_year: int | None,
-        final_quarter: int | None,
-    ):
-        """Options.
-
-        Args:
-            tickers (frozenset[str]): tickers to scrape from data sets
-            cache_path (Path): path to cache processed or downloaded information
-            final_year (int | None): last year to consider for report collection
-            final_quarter (int | None): last quarter to consider for report collection
-        """
-        self.tickers = tickers
-        self.cache_path = cache_path
-        self.last_report = ReportDate(year=final_year, quarter=final_quarter)
+    tickers: list[str]
+    final_report: ReportDate = ReportDate()
+
+    def __post_init__(self):
+        self.tickers.sort()
 
 
 @beartype
 class Analysis(metaclass=abc.ABCMeta):
     """Base class for all analysis techniques."""
 
     def __init__(self, options: Options) -> None:
         self.options = options
         assert self.options is not None
-        assert self.options.cache_path is not None
 
     @abc.abstractmethod
     def analyze(self) -> Optional[DataFrame]:
         """Perform financial analysis.
 
         Returns:
             Optional[DataFrame]: results of analysis
```

### Comparing `stocktracer-0.3.0/src/stocktracer/analysis/annual_reports.py` & `stocktracer-0.4.0/src/stocktracer/analysis/annual_reports.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 """Download and retrieves annual reports for the specified stock tickers."""
 import logging
 from typing import Optional
 
 import pandas as pd
 from beartype import beartype
 
-from stocktracer.data.sec import Filter as SecFilter
-from stocktracer.data.sec import Sec as SecDataSource
+import stocktracer.collector.sec as Sec
 from stocktracer.interface import Analysis as AnalysisInterface
-from stocktracer.interface import Options
 
 logger = logging.getLogger(__name__)
 
 
 def create_normalized_sec_table(
-    sec_filter: SecFilter, options: Options, normalize: bool = True
-) -> SecFilter.Results:
+    sec_filter: Sec.Filter, tickers: list[str], normalize: bool = True
+) -> Sec.Results.Table:
     """Create a normalized SEC table with all NA values removed.
 
     Args:
-        sec_filter (SecFilter): filter to use for grabbing results
-        options (Options): user provided CLI options
+        sec_filter (Sec.Filter): filter to use for grabbing results
+        tickers (list[str]): tickers to retrieve
         normalize (bool): Remove all columns that contain at least one NA value
 
     Returns:
-        SecFilter.Results: An SEC table with normalized results
+        Sec.Results.Table: An SEC table with normalized results
     """
-    sec = SecDataSource(storage_path=options.cache_path)
-    sec.filter_data(tickers=options.tickers, sec_filter=sec_filter)
+    # prep for caching
+    tickers.sort()
+    results = Sec.filter_data(tickers=tickers, sec_filter=sec_filter)
 
-    table = sec_filter.select()
+    table = results.select()
     # If you prefer to see columns that are not universal across all stocks, comment this out
     if normalize:
         table.normalize()
     return table
 
 
 @beartype
 class Analysis(AnalysisInterface):
     """Class for collecting and processing annual report data."""
 
     under_development = True
 
     def analyze(self) -> Optional[pd.DataFrame]:
         # By omitting the tags, we'll collect all tags for securities
-        sec_filter = SecFilter(
+        sec_filter = Sec.Filter(
             # tags=["EarningsPerShareDiluted"],
             years=1,  # Over the past 1 years
-            last_report=self.options.last_report,
+            last_report=self.options.final_report,
             only_annual=True,  # We only want the 10-K
         )
 
         # Create an SEC Data Source
-        table = create_normalized_sec_table(sec_filter, self.options, False)
+        table = create_normalized_sec_table(sec_filter, self.options.tickers, False)
 
         return table.data
 
     # Reuse documentation from parent
     analyze.__doc__ = AnalysisInterface.analyze.__doc__
```

### Comparing `stocktracer-0.3.0/src/stocktracer/analysis/diluted_eps.py` & `stocktracer-0.4.0/src/stocktracer/analysis/diluted_eps.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 """This analysis module determines the trend of EPS over the course of the past 5 years."""
 import logging
 from typing import Optional
 
 import pandas as pd
 from beartype import beartype
 
-from stocktracer.data.sec import Filter as SecFilter
-from stocktracer.data.sec import Sec as SecDataSource
+import stocktracer.collector.sec as Sec
 from stocktracer.interface import Analysis as AnalysisInterface
 
 logger = logging.getLogger(__name__)
 
 
 @beartype
 class Analysis(AnalysisInterface):
     """Class that calculates the EPS slope."""
 
     under_development = True
     years_of_analysis = 5
 
     def analyze(self) -> Optional[pd.DataFrame]:
         # Create the filter we'll use to scrape the results
-        sec_filter = SecFilter(
+        sec_filter = Sec.Filter(
             tags=["EarningsPerShareDiluted"],
             years=self.years_of_analysis,
-            last_report=self.options.last_report,
+            last_report=self.options.final_report,
             only_annual=True,  # We only want the 10-K
         )
 
-        # Create an SEC Data Source
-        sec = SecDataSource(storage_path=self.options.cache_path)
-
         # This is an expensive operation
-        sec.filter_data(tickers=self.options.tickers, sec_filter=sec_filter)
-        return sec_filter.select("slope").data
+        results = Sec.filter_data(tickers=self.options.tickers, sec_filter=sec_filter)
+        return results.select("slope").data
 
     # Reuse documentation from parent
     analyze.__doc__ = AnalysisInterface.analyze.__doc__
```

### Comparing `stocktracer-0.3.0/src/stocktracer/analysis/f_score.py` & `stocktracer-0.4.0/src/stocktracer/analysis/f_score.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Piotroski F-score is a number between 0 and 9 which is used to assess strength of company's financial position."""
 import logging
 from typing import Optional
 
 import pandas as pd
 from beartype import beartype
 
+import stocktracer.collector.sec as Sec
 from stocktracer.analysis.annual_reports import create_normalized_sec_table
-from stocktracer.data.sec import Filter as SecFilter
 from stocktracer.interface import Analysis as AnalysisInterface
 
 logger = logging.getLogger(__name__)
 
 
 @beartype
 class Analysis(AnalysisInterface):
@@ -43,34 +43,34 @@
     """
 
     under_development = True
     years_of_analysis = 2
 
     def analyze(self) -> Optional[pd.DataFrame]:
         # Create the filter to scrape the data we need for processing
-        sec_filter = SecFilter(
+        sec_filter = Sec.Filter(
             tags=[
                 "EarningsPerShareDiluted",
                 "CommonStockSharesIssued",
                 "AssetsCurrent",
                 "LiabilitiesCurrent",
                 "Assets",
                 "OperatingIncomeLoss",
                 "NetCashProvidedByUsedInOperatingActivities",
             ],
             years=self.years_of_analysis,
-            last_report=self.options.last_report,
+            last_report=self.options.final_report,
             only_annual=True,  # We only want the 10-K
         )
 
-        table = create_normalized_sec_table(sec_filter, self.options, False)
+        table = create_normalized_sec_table(sec_filter, self.options.tickers, False)
         table.data.fillna(0, inplace=True)
 
         assert (
-            self.options.last_report.year + 1
+            self.options.final_report.year + 1
             not in table.data.index.get_level_values(1)
         )
 
         logger.debug(f"filtered_data:\n{table.data}")
         max_year = int(table.data.index.get_level_values("fy").max())
 
         # Do calculations
```

### Comparing `stocktracer-0.3.0/src/stocktracer/analysis/stub.py` & `stocktracer-0.4.0/src/stocktracer/analysis/stub.py`

 * *Files identical despite different names*

### Comparing `stocktracer-0.3.0/src/stocktracer/data/sec.py` & `stocktracer-0.4.0/src/stocktracer/collector/sec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,52 @@
 """This data source grabs information from quarterly SEC data archives."""
 import copy
 import logging
 import sys
-from datetime import date, timedelta
+from dataclasses import dataclass, field
+from datetime import date
 from io import BytesIO
-from pathlib import Path
 from typing import Literal, Optional
 from zipfile import ZipFile
 
 import numpy as np
 import pandas as pd
 from alive_progress import alive_bar
 from beartype import beartype
 from beartype.typing import Callable, Sequence
-from numpy.linalg import LinAlgError
-from requests_cache import CachedSession, SQLiteCache
+
+from stocktracer import cache
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_CHUNK_SIZE = 1000000
 pd.set_option("mode.chained_assignment", "raise")
 
 
 @beartype
+@dataclass(frozen=True)
 class ReportDate:
     """ReportDate is used to select and identify archives created by the SEC."""
 
-    def __init__(
-        self,
-        year: int | None = None,
-        quarter: int | None = None,
-    ):
-        """
-
-        Args:
-            year (int, optional): Year of the archive. Defaults to date.today().year.
-            quarter (int, optional): Quarter the archive was created. Defaults to ((date.today().month - 1) // 3)+1.
-
-        Raises:
-            ValueError: If the value for quarter or year is invalid
-        """
-        self.year = date.today().year if year is None else year
-        self.quarter = (
-            ((date.today().month - 1) // 3) + 1 if quarter is None else quarter
-        )
+    year: int = date.today().year
+    quarter: int = ((date.today().month - 1) // 3) + 1
 
+    def __post_init__(self):
         if self.year > date.today().year:
             raise ValueError(
                 "you cannot request reports in the future...that would be illegal :)"
             )
         if self.quarter not in range(1, 5):
             raise ValueError(
-                f"the quarter must be a value between 1 and 4 - given: {quarter}"
+                f"the quarter must be a value between 1 and 4 - given: {self.quarter}"
             )
 
     def __str__(self) -> str:
         return f"{self.year}-q{self.quarter}"
 
-    def __repr__(self) -> str:
-        return f"ReportDate({self.year},{self.quarter})"
-
-    def __eq__(self, other: "ReportDate") -> bool:
-        return self.quarter == other.quarter and self.year == other.year
-
 
 @beartype
 class TickerReader:
     """This class provides translation services for CIK and Ticker values.
 
     The SEC has a `json` file that provides mappings from CIK values to Tickers.
     The data providing this conversion is injected into this class and then
@@ -129,14 +109,33 @@
             bool: if all the tickers are found
         """
         for ticker in tickers:
             self.convert_to_cik(ticker)
 
         return True
 
+    def get_ciks(self, tickers: frozenset[str]) -> frozenset[int]:
+        """Populates the filter's CIK list to be used for filtering.
+
+        The Filter doesn't need the ticker symbols. If we expand to other data sources,
+        we would have to repeat ticker symbols. For now, the only info we need in the
+        report is the CIK values to find the corresponding stocks.
+
+        Args:
+            tickers (frozenset[str]): ticker symbols to search for
+
+        Returns:
+            frozenset[int]: CIKs values translated from the tickers specified
+        """
+        cik_list: set[int] = set()
+        for ticker in tickers:
+            cik = self.convert_to_cik(ticker)
+            cik_list.add(int(cik))
+        return frozenset(cik_list)
+
 
 @beartype
 def slope(data: pd.Series, order: int = 1) -> float:
     """Calculate the trend of a series.
 
     >>> import math
     >>> math.isclose(slope(pd.Series((1,2,3))), 1)
@@ -152,25 +151,104 @@
     Returns:
         float: slope of the trend line
     """
     x_axis = range(len(data.keys()))
     y_axis = data.values
 
     try:
+        # An exception can be thrown if there's only one element of it's a nan
         coeffs = np.polyfit(x_axis, y_axis, order)
-    except LinAlgError:
+    except np.linalg.LinAlgError:
+        return float(0)
+    except Exception as e:
+        logger.warning(f"slope exception: {e}")
         return float(0)
     return coeffs[0]
 
 
 @beartype
+@dataclass(frozen=True)
 class Filter:
     """Filter for SEC tools to scrape relevant information when processing records."""
 
-    class Results:
+    years: int = field(hash=True)
+    tags: Optional[list[str]] = field(default=None, hash=True)
+    last_report: ReportDate = field(default=ReportDate(), hash=True)
+    only_annual: bool = field(default=True, hash=True)
+
+    @property
+    def focus_period(self) -> frozenset[str]:
+        """Get the focus period for the report.
+
+        Companies file quarterly reports. The annual report replaces the quarterly
+        report depending on when that is reported. Typically Q4 is replaced with FY
+        for the annual reports.
+
+        Returns:
+            frozenset[str]: list of focus periods to use for the filter
+        """
+        if self.only_annual:
+            return frozenset({"FY"})
+        return frozenset({"FY", "Q1", "Q2", "Q3", "Q4"})
+
+    @property
+    def required_reports(self) -> list[ReportDate]:
+        """Get a list of required reports to download for all the quarters.
+
+        The list generated will include an extra quarter so that you will always be
+        able to do analysis from the current quarter to the previous quarter.
+
+        Also note that it doesn't matter if you specify only_annual=True. Because
+        companies don't have the same fiscal year, we have to check every quarterly
+        report just to see if their annual report is in there.
+
+        Returns:
+            list[ReportDate]: list of report dates to retrieve
+        """
+        dl_list: list[ReportDate] = []
+        next_report = copy.deepcopy(self.last_report)
+        final_report = ReportDate(
+            self.last_report.year - self.years, self.last_report.quarter
+        )
+        while 1:
+            dl_list.append(
+                ReportDate(year=next_report.year, quarter=next_report.quarter)
+            )
+            if next_report == final_report:
+                break
+            if 1 == next_report.quarter:
+                next_report = ReportDate(year=next_report.year - 1, quarter=4)
+            else:
+                next_report = ReportDate(
+                    year=next_report.year, quarter=next_report.quarter - 1
+                )
+        return dl_list
+
+
+@beartype
+@dataclass
+class Results:
+    """Filtered data looks like this(in csv format):
+
+    Note that fp has the "Q" removed from the front so it can be stored as a simple number.
+
+    .. code-block:: text
+
+        ticker,tag,fy,fp,ddate,uom,value,period,title
+        AAPL,EntityCommonStockSharesOutstanding,2022,Q1,2023-01-31,shares,2000.0,2022-12-31,Apple Inc.
+        AAPL,FakeAttributeTag,2022,Q1,2023-01-31,shares,200.0,2022-12-31,Apple Inc.
+    """
+
+    filtered_data: pd.DataFrame
+
+    _cik_list: Optional[set[np.int64]] = None
+
+    @beartype
+    @dataclass
+    class Table:
         """This is the results from a `Filter.select()` call.
 
         The results table looks like the following:
 
         ```
         tag            AccountsPayableCurrent  ...  WeightedAverageNumberOfSharesOutstandingBasic
         ticker fy                              ...
@@ -185,35 +263,33 @@
         From here, you can call functions on this class like `get_value()` or `normalize()`.
 
         !!! note
             To get a list of all the tags, run the `annual_reports` analysis module and search through the output for meaningful tags.
 
         """
 
-        def __init__(self, results: pd.DataFrame) -> None:
-            logger.debug(f"results:\n{results}")
-            self.data = results
+        data: pd.DataFrame
 
         def __str__(self) -> str:
             return str(self.data)
 
         @property
         def tags(self) -> np.ndarray:
             """List of tags that can be used on this data set.
 
             Returns:
                 np.ndarray: array with results
             """
             return self.data.columns.values
 
-        def get_value(self, ticker: str | int, tag: str, year: int) -> int | float:
+        def get_value(self, ticker: str, tag: str, year: int) -> int | float:
             """Retrieve the exact value of a table cell.
 
             Args:
-                ticker (str | int): ticker identifying the equity of interest.
+                ticker (str): ticker identifying the equity of interest.
                 tag (str): attribute indicating the type of data to look at.
                 year (int): The year this data applies to.
 
             Returns:
                 int | float: value of result
             """
             # Lookup convert ticker to cik
@@ -222,30 +298,34 @@
 
         def normalize(self):
             """Remove all values that are NaN."""
             self.data = self.data.dropna(axis=1, how="any")
 
         def slice(
             self,
-            ticker: Optional[str | int] = None,
+            ticker: Optional[str | list[str]] = None,
             year: Optional[int] = None,
             tags: Optional[list[str]] = None,
         ) -> pd.DataFrame:
             """Slice the results by the specified values
 
             Args:
-                ticker (Optional[str  |  int]): _description_. Defaults to None.
+                ticker (Optional[str | list[str]]): _description_. Defaults to None.
                 tags (Optional[str]): _description_. Defaults to None.
                 year (Optional[int]): _description_. Defaults to None.
 
             Returns:
                 pd.DataFrame: _description_
             """
             result = self.data
             if ticker:
+                if isinstance(ticker, str):
+                    ticker = ticker.upper()
+                else:
+                    ticker = [t.upper() for t in ticker]
                 result = result.loc(axis=0)[ticker, :]
             if year:
                 result = result.loc(axis=0)[:, year, :]
             if tags:
                 result = pd.DataFrame(result.loc[:, tags], columns=tags)
             return result
 
@@ -307,90 +387,31 @@
 
             Args:
                 column_name (str): name to give the calculated column
                 delta_of (str): column name to calculate the delta of, such as ROI
             """
             self.data[column_name] = self.data.groupby(by=["ticker"]).diff()[delta_of]
 
-    def __init__(
-        self,
-        tags: Optional[list[str]] = None,
-        years: int = 1,
-        last_report: ReportDate = ReportDate(),
-        only_annual: bool = True,
-    ) -> None:
-        """
-
-        This is an important concept to dealing with large data sets. It allows us to chunk processing
-        into batches and find/locate only records of interest. Without these filters, the tool would
-        require absurd amounts of memory and storage to process.
-
-        Args:
-            tags (Optional[list[str]]): list of tags found in the SEC report, such as 'EntityCommonStockSharesOutstanding'
-            years (int): years of reports desired. Defaults to 1.
-            last_report (ReportDate): most recent SEC data dump identified by the year an quarter. Defaults to ReportDate().
-            only_annual (bool): If true, only scrape the annual reports. Defaults to True.
-        """
-        self.tags = tags
-        self.years = years
-        self.last_report = last_report
-        self.only_annual = only_annual
-        self._cik_list: set[int] = None
-        self._filtered_data: pd.DataFrame = None
-
-    @property
-    def filtered_data(self) -> pd.DataFrame:
-        """Filtered data looks like this(in csv format):
-
-        Note that fp has the "Q" removed from the front so it can be stored as a simple number.
-
-        .. code-block:: text
-
-            ticker,tag,fy,fp,ddate,uom,value,period,title
-            AAPL,EntityCommonStockSharesOutstanding,2022,Q1,2023-01-31,shares,2000.0,2022-12-31,Apple Inc.
-            AAPL,FakeAttributeTag,2022,Q1,2023-01-31,shares,200.0,2022-12-31,Apple Inc.
-
-        Returns:
-            pd.DataFrame: _description_
-        """
-        return self._filtered_data
-
-    @filtered_data.setter
-    def filtered_data(self, filtered_data: pd.DataFrame):
-        self._filtered_data = filtered_data
-
-    def __str__(self) -> str:
-        """
-        >>> print(Filter(["Income","Debt"],5,ReportDate(2023,1)))
-        Filter on 2023-q1 and the previous 5 years
-        Annual Only: True
-        CIK(s): None
-        Tags: Income,Debt
-        """
-        return f"""Filter on {self.last_report} and the previous {self.years} years
-Annual Only: {self.only_annual}
-CIK(s): {','.join([str(i) for i in self._cik_list]) if self._cik_list else 'None'}
-Tags: {','.join(self.tags) if self.tags else 'None'}"""
-
     def select(
         self,
         aggregate_func: Optional[
             Callable | Literal["mean", "std", "var", "sum", "min", "max", "slope"]
         ] = "mean",
         tickers: Optional[Sequence[str]] = None,
-    ) -> Results:
+    ) -> Table:
         """Select only a subset of the data matching the specified criteria.
 
         Args:
             aggregate_func (Optional[Callable | Literal['mean', 'std', 'var', 'sum', 'min','max','slope']]): Numpy function to use for aggregating the results. This should be a function like `numpy.average` or `numpy.sum`.
             tickers (Optional[Sequence[str]]): ticker symbol for the company
 
         Returns:
-            Filter.Results: Object that represents a pivot table with the data requested
+            Results.Table: Object that represents a pivot table with the data requested
         """
+        assert self.filtered_data is not None
         if tickers is not None:
             tickers = [t.upper() for t in tickers]
             logger.debug(f"ticker filter: {tickers}")
 
         data = (
             self.filtered_data
             if tickers is None
@@ -407,18 +428,18 @@
             data,
             values="value",
             columns="tag",
             index=["ticker", "fy"],
             aggfunc=aggregate_func,
         )
 
-        return Filter.Results(table)
+        return Results.Table(table)
 
     @property
-    def ciks(self) -> set[int]:
+    def ciks(self) -> set[np.int64]:
         """Retrieves a list of CIK values corresponding to the tickers being looked up.
 
         The SEC object will call populateCikList to generate this information. This helps
         with dependency injection by avoiding the Filter having to maintain references to
         these helper objects for temporary processing. It also lets us stub out the information
         provided without having to involve heavier utilities or network access.
 
@@ -430,108 +451,46 @@
         """
         if self._cik_list is None:
             raise LookupError(
                 "Filter was not provided a mapping of cik's based on the tickers."
             )
         return self._cik_list
 
-    def populate_ciks(
-        self, tickers: frozenset[str], ticker_reader: TickerReader
-    ) -> None:
-        """Populates the filter's CIK list to be used for filtering.
-
-        The Filter doesn't need the ticker symbols. If we expand to other data sources,
-        we would have to repeat ticker symbols. For now, the only info we need in the
-        report is the CIK values to find the corresponding stocks.
-
-        Args:
-            tickers (frozenset[str]): ticker symbols to search for
-            ticker_reader (TickerReader): reader to convert ticker symbols to CIK values
-        """
-        self._cik_list = set()
-        for ticker in tickers:
-            cik = ticker_reader.convert_to_cik(ticker)
-            self._cik_list.add(cik)
-
-    @property
-    def focus_period(self) -> list[str]:
-        """Get the focus period for the report.
-
-        Companies file quarterly reports. The annual report replaces the quarterly
-        report depending on when that is reported. Typically Q4 is replaced with FY
-        for the annual reports.
-
-        Returns:
-            list[str]: list of focus periods to use for the filter
-        """
-        if self.only_annual:
-            return ["FY"]
-        return ["FY", "Q1", "Q2", "Q3", "Q4"]
-
-    @property
-    def required_reports(self) -> list[ReportDate]:
-        """Get a list of required reports to download for all the quarters.
-
-        The list generated will include an extra quarter so that you will always be
-        able to do analysis from the current quarter to the previous quarter.
-
-        Also note that it doesn't matter if you specify only_annual=True. Because
-        companies don't have the same fiscal year, we have to check every quarterly
-        report just to see if their annual report is in there.
-
-        Returns:
-            list[ReportDate]: list of report dates to retrieve
-        """
-        dl_list: list[ReportDate] = []
-        next_report = copy.deepcopy(self.last_report)
-        final_report = ReportDate(
-            self.last_report.year - self.years, self.last_report.quarter
-        )
-        while 1:
-            dl_list.append(
-                ReportDate(year=next_report.year, quarter=next_report.quarter)
-            )
-            if next_report == final_report:
-                break
-            if 1 == next_report.quarter:
-                next_report.quarter = 4
-                next_report.year -= 1
-            else:
-                next_report.quarter -= 1
-        return dl_list
-
 
 @beartype
 class DataSetReader:
     """Reads the data from a zip file retrieved from the SEC website."""
 
     def __init__(self, zip_data: bytes) -> None:
         self.zip_data = BytesIO(zip_data)
 
-    def process_zip(self, sec_filter: Filter) -> Optional[pd.DataFrame]:
+    def process_zip(
+        self, sec_filter: Filter, ciks: frozenset[int]
+    ) -> Optional[pd.DataFrame]:
         """Process a zip archive with the provided filter.
 
         Args:
             sec_filter (Filter): results to filter out of the zip archive
-
-        Raises:
-            ImportError: the filter doesn't match anything
+            ciks (frozenset[int]): CIKs to filter data on
 
         Returns:
             Optional[pd.DataFrame]: filtered data
         """
         with ZipFile(self.zip_data) as myzip:
             # Process the mapping first
             logger.debug("opening sub.txt")
             with myzip.open("sub.txt") as myfile:
                 # Get reports that are 10-K or 10-Q
-                sub_dataframe = DataSetReader._process_sub_text(myfile, sec_filter)
+                sub_dataframe = DataSetReader._process_sub_text(
+                    myfile, sec_filter, ciks
+                )
 
                 if sub_dataframe is None or sub_dataframe.empty:
-                    raise ImportError("nothing found in sub.txt matching the filter")
+                    logger.debug("nothing found in sub.txt matching the filter")
+                    return None
 
                 with myzip.open("num.txt") as myfile:
                     return DataSetReader._process_num_text(
                         myfile, sec_filter, sub_dataframe
                     )
 
     @classmethod
@@ -549,15 +508,15 @@
             delimiter="\t",
             usecols=["adsh", "tag", "ddate", "uom", "value"],
             index_col=["adsh", "tag"],
             chunksize=DEFAULT_CHUNK_SIZE,
             parse_dates=["ddate"],
         )
 
-        filtered_data: pd.DataFrame = None
+        filtered_data: Optional[pd.DataFrame] = None
         chunk: pd.DataFrame
         for chunk in reader:
             # We want only the tables in left if they join on the key, so inner it is
             data = chunk.join(sub_dataframe, how="inner")
 
             # Additional Filtering if needed
             if sec_filter.tags is not None:
@@ -621,40 +580,42 @@
             filtered_data = data
         else:
             filtered_data = pd.concat([filtered_data, data])
         return filtered_data
 
     @classmethod
     def _process_sub_text(
-        cls, filepath_or_buffer, sec_filter: Filter
+        cls,
+        filepath_or_buffer,
+        sec_filter: Filter,
+        ciks: frozenset[int],  # pylint: disable=unused-argument
     ) -> Optional[pd.DataFrame]:
         """Contains the submissions.
 
         adsh	cik	name	sic	countryba	stprba	cityba	zipba	bas1	bas2	baph	countryma
         stprma	cityma	zipma	mas1	mas2	countryinc	stprinc	ein	former	changed	afs	wksi
         fye	form	period	fy	fp	filed	accepted	prevrpt	detail	instance	nciks	aciks
         """
         logger.debug("processing sub.txt")
         focus_periods = sec_filter.focus_period
-        cik_list = sec_filter.ciks  # pylint: disable=unused-variable
 
         oldest_fy = sec_filter.last_report.year - sec_filter.years
-        query_str = f"cik in @cik_list and fp in @focus_periods and fy >= {oldest_fy}"
+        query_str = f"cik in @ciks and fp in @focus_periods and fy >= {oldest_fy}"
         # logger.debug(f"Query string: {query_str}")
         reader = pd.read_csv(
             filepath_or_buffer,
             delimiter="\t",
             usecols=["adsh", "cik", "period", "fy", "fp"],
             index_col=["adsh", "cik"],
             chunksize=DEFAULT_CHUNK_SIZE,
             parse_dates=["period"],
             dtype={"cik": np.int32},
         )
         logger.info(f"keeping only these focus periods: {focus_periods}")
-        filtered_data: pd.DataFrame = None
+        filtered_data: Optional[pd.DataFrame] = None
         chunk: pd.DataFrame
         for chunk in reader:
             data = chunk.query(query_str)
             if data.empty:
                 continue
             filtered_data = cls.append(filtered_data, data)
         return filtered_data
@@ -665,20 +626,14 @@
     """This class is responsible for downloading and caching downloaded data sets from the SEC."""
 
     # Format of zip example: 2023q1.zip
     _base_url = "https://www.sec.gov/files/dera/data/financial-statement-data-sets"
 
     _company_tickers_url = "https://www.sec.gov/files/company_tickers.json"
 
-    def __init__(
-        self, ticker_session: CachedSession, data_session: CachedSession
-    ) -> None:
-        self._ticker_session = ticker_session
-        self._data_session = data_session
-
     @property
     def ticker_reader(self) -> TickerReader:
         """Get the CIK ticker mappings. This must be done before processing reports.
 
         The SEC stores the mappings of the CIK values to tickers in a JSON file.
         We can download and cache this information essentially for a year. We're
         not interested in companies that recently listed because they don't have a
@@ -691,20 +646,20 @@
         {"0":{"cik_str":320193,"ticker":"AAPL","title":"Apple Inc."},
          "1":{"cik_str":789019,"ticker":"MSFT","title":"MICROSOFT CORP"},
 
         Returns:
             TickerReader: maps cik to stock ticker
 
         """
-        response = self._ticker_session.get(self._company_tickers_url)
+        response = cache.sec_tickers.get(self._company_tickers_url)
         if response.from_cache:  # pragma: no cover
             logger.info("Retrieved tickers->cik mapping from cache")
         if response.status_code == 200:  # pragma: no cover
             return TickerReader(response.content.decode())
-        return TickerReader(pd.DataFrame())  # pragma: no cover
+        raise LookupError("unable to retrieve tickers")  # pragma: no cover
 
     def _create_download_uri(self, report_date: ReportDate) -> str:
         file = f"{report_date.year}q{report_date.quarter}.zip"
         return "/".join([self._base_url, file])
 
     def get_quarterly_report(self, report_date: ReportDate) -> Optional[DataSetReader]:
         """Retrieve from a cache or make a request archived quarterly data.
@@ -715,15 +670,15 @@
         Args:
             report_date (ReportDate): information specifying the quarterly dump to retrieve
 
         Returns:
             Optional[DataSetReader]: this object helps process the data received more granularly
         """
         request = self._create_download_uri(report_date)
-        response = self._data_session.get(request)
+        response = cache.sec_data.get(request)
         if response.from_cache:
             logger.info(f"Retrieved {request} from cache")
 
         if response.status_code == 200:
             return DataSetReader(response.content)
         return None  # pragma: no cover
 
@@ -731,22 +686,27 @@
 @beartype
 class DataSetCollector:
     """Take care of downloading all the data sets and aggregate them into a single structure."""
 
     def __init__(self, download_manager: DownloadManager):
         self.download_manager = download_manager
 
-    def get_data(self, sec_filter: Filter) -> None:
+    def get_data(self, sec_filter: Filter, ciks: frozenset[int]) -> Results:
         """Collect data based on the provided filter.
 
         Args:
             sec_filter (Filter): SEC specific filter of how to filter the results
+            ciks (frozenset[int]): CIK values to filter the datasets on
 
         Raises:
-            LookupError: when there are no results matching the filter
+            ImportError: when a download for a quarterly report fails
+            LookupError: when the filter returned no matches
+
+        Returns:
+            Results: filtered data results
 
         """
         data_frame = None
         report_dates = sec_filter.required_reports
         logger.info(f"Creating Unified Data record for these reports: {report_dates}")
         with alive_bar(
             # total=len(report_dates) * 2,
@@ -756,36 +716,38 @@
             file=sys.stderr,
             calibrate=5_000,
             dual_line=True,
         ) as status_bar:
             for report_date in report_dates:
                 status_bar.text(f"Downloading report {report_date}...")
                 reader = self.download_manager.get_quarterly_report(report_date)
-                if isinstance(reader, DataSetReader):
-                    try:
-                        status_bar.text(f"Processing report {report_date}...")
-                        data = reader.process_zip(sec_filter)
-                        if data_frame is not None:
-                            logger.debug(f"record count: {len(data_frame)}")
-                        if data is not None:
-                            logger.debug(f"new record count: {len(data)}")
-                            data_frame = DataSetReader.append(data_frame, data)
-                            record_count = len(data_frame)
-                            status_bar(record_count)  # pylint: disable=not-callable
-                            logger.info(
-                                f"There are now {record_count} filtered records"
-                            )
-
-                    except ImportError:
-                        # Note, when searching for annual reports, this will generally occur 1/4 times
-                        # if we're only searching for one stock's tags
-                        logger.debug(
-                            f"{report_date} did not have any matches for the provided filter"
-                        )
-                        logger.debug(f"{sec_filter}")
+
+                if reader is None:
+                    raise ImportError(f"missing quarterly report for {report_date}")
+
+                status_bar.text(f"Processing report {report_date}...")
+                data = reader.process_zip(sec_filter, ciks)
+
+                if data is None:
+                    # Note, when searching for annual reports, this will generally occur 1/4 times
+                    # if we're only searching for one stock's tags
+                    logger.debug(
+                        f"{report_date} did not have any matches for the provided filter"
+                    )
+                    logger.debug(f"{sec_filter}")
+                    continue
+
+                if data_frame is not None:
+                    logger.debug(f"record count: {len(data_frame)}")
+
+                logger.debug(f"new record count: {len(data)}")
+                data_frame = DataSetReader.append(data_frame, data)
+                record_count = len(data_frame)
+                status_bar(record_count)  # pylint: disable=not-callable
+                logger.info(f"There are now {record_count} filtered records")
 
         logger.info(f"Created Unified Data record for these reports: {report_dates}")
         if data_frame is None:
             raise LookupError("No data matching the filter was retrieved")
 
         # Now add an index for ticker values to pair with the cik
         # logger.debug(f"filtered_df_before_merge:\n{data_frame.to_csv()}")
@@ -798,67 +760,71 @@
 
         # Columns at this point look like this
         #  ,adsh,tag,cik,ddate,uom,value,period,fy,fp,cik_str,ticker,title
         # 0,0000097745-23-000008,EarningsPerShareDiluted,97745,2022-12-31,USD,17.63,2022-12-31,2022.0,FY,97745,TMO,THERMO FISHER SCIENTIFIC INC.
         # 1,0000097745-23-000008,EarningsPerShareDiluted,97745,2020-12-31,USD,15.96,2022-12-31,2022.0,FY,97745,TMO,THERMO FISHER SCIENTIFIC INC.
         # 2,0000097745-23-000008,EarningsPerShareDiluted,97745,2021-12-31,USD,19.46,2022-12-31,2022.0,FY,97745,TMO,THERMO FISHER SCIENTIFIC INC..
 
-        sec_filter.filtered_data = data_frame.drop(
-            columns=["cik_str", "adsh", "cik"]
-        ).set_index(["ticker", "tag", "fy", "fp"])
+        return Results(
+            data_frame.drop(columns=["cik_str", "adsh", "cik"]).set_index(
+                ["ticker", "tag", "fy", "fp"]
+            )
+        )
 
         # # Convert fp to number so we can sort easily
         # data_frame['fp'].mask(data_frame['fp'] == "Q1", 1, inplace=True)
         # data_frame['fp'].mask(data_frame['fp'] == "Q2", 2, inplace=True)
         # data_frame['fp'].mask(data_frame['fp'] == "Q3", 3, inplace=True)
         # data_frame['fp'].mask(data_frame['fp'] == "Q4", 4, inplace=True)
         # data_frame = data_frame.set_index("fp", append=True)
 
         # logger.debug(f"filtered_df:\n{data_frame}")
         # filter.filtered_data = data_frame
 
 
 @beartype
-class Sec:
-    """Object for handling requests for information relating to SEC data dumps."""
+@cache.results.memoize(tag="sec", ignore=("download_manager"))
+def filter_data(
+    tickers: list[str],
+    sec_filter: Filter,
+    download_manager: DownloadManager = DownloadManager(),
+) -> Results:
+    """Initiate the retrieval of ticker information based on the provided filters.
 
-    def __init__(self, storage_path: Path):
-        """
+    Filtered data is stored with the filter
 
-        Args:
-            storage_path (Path): Where to store the results.
-        """
-        storage_path.mkdir(parents=True, exist_ok=True)
-        data_session = CachedSession(
-            "data",
-            backend=SQLiteCache(db_path=storage_path / "data"),
-            serializer="pickle",
-            expire_after=timedelta(days=365 * 5),
-            stale_if_error=True,
-        )
-        ticker_session = CachedSession(
-            "tickers",
-            backend=SQLiteCache(db_path=storage_path / "tickers"),
-            expire_after=timedelta(days=365),
-            stale_if_error=True,
-        )
-        self.download_manager = DownloadManager(ticker_session, data_session)
+    Args:
+        tickers (list[str]): ticker symbols you want information about
+        sec_filter (Filter): SEC specific data to scrape from the reports
+        download_manager (DownloadManager): download manager to use
 
-    def filter_data(self, tickers: frozenset[str], sec_filter: Filter) -> Filter:
-        """Initiate the retrieval of ticker information based on the provided filters.
+    Returns:
+        Results: results with filtered data
+    """
+    logger.debug(f"tickers:\n{repr(tickers)}")
+    logger.debug(f"sec_filter:\n{repr(sec_filter)}")
+    return filter_data_nocache(frozenset(tickers), sec_filter, download_manager)
 
-        Filtered data is stored with the filter
 
-        Args:
-            tickers (frozenset[str]): ticker symbols you want information about
-            sec_filter (Filter): SEC specific data to scrape from the reports
+def filter_data_nocache(
+    tickers: frozenset[str],
+    sec_filter: Filter,
+    download_manager: DownloadManager = DownloadManager(),
+) -> Results:
+    """Same as filter_data but no caching is applied.
 
-        Returns:
-            Filter: filter with filtered data
-        """
-        collector = DataSetCollector(self.download_manager)
-        ticker_reader = self.download_manager.ticker_reader
-        if ticker_reader.contains(tickers):
-            sec_filter.populate_ciks(tickers=tickers, ticker_reader=ticker_reader)
-            collector.get_data(sec_filter)
+    Args:
+        tickers (frozenset[str]): ticker symbols you want information about
+        sec_filter (Filter): SEC specific data to scrape from the reports
+        download_manager (DownloadManager): download manager to use
+
+    Returns:
+        Results: results with filtered data
+    """
+    collector = DataSetCollector(download_manager)
+    ticker_reader = download_manager.ticker_reader
+
+    # Returns true or throws
+    ticker_reader.contains(tickers)
 
-        return sec_filter
+    ciks = ticker_reader.get_ciks(tickers=tickers)
+    return collector.get_data(sec_filter, ciks)
```

### Comparing `stocktracer-0.3.0/LICENSE` & `stocktracer-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stocktracer-0.3.0/README.md` & `stocktracer-0.4.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -26,45 +26,29 @@
 - `python 3.10+`
 
 ## Getting Started
 
 ### Users
 
 ```sh
+# basic install
 pip install stocktracer
 
+# with tensorflow dependencies for analysis modules
+pip install stocktracer[tensorflow]
+
 # Perform analysis
 stocktracer analyze --tickers aapl,msft > report.txt
 
 # Help
 stocktracer
 
 ```
 
-### Developers
-
-Make sure you have `pipenv` installed through a package manager or through pip.
-
-```sh
-pipenv install --dev
-
-# Perform analysis
-PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers aapl,msft
-PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers aapl,msft -a stocktracer.analysis.diluted_eps
-PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers aapl,msft -a stocktracer.analysis.diluted_eps --report-format csv
-PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers aapl,msft -a stocktracer.analysis.diluted_eps --report-format json --report-file my_results.json
-
-# Help
-PYTHONPATH=src pipenv run python -m stocktracer
-
-# Run Unit Tests
-pipenv run pytest
-```
-
-More information can be found in our [documentation](https://gyund.github.io/fundamental-analysis/)
+For development guides, see our [documentation](https://gyund.github.io/fundamental-analysis/getting-started)
 
 ## Disclaimer
 
 This project seeks to use publicly available information to perform security analysis and
 help perform long term risk analysis. Results provided from this project are generally for 
 academic use only and are not considered advice or recommendations. This project makes no
 performance claims or guarantees. Please read the [license](LICENSE)
```

#### html2text {}

```diff
@@ -4,26 +4,18 @@
 aggregate a variety of ways to consume information about a particular equity
 traded on the US stock market and provide a modular mechanism to process it.
 Core tenants of this project include: - **Heavy data caching** - don't download
 static data more than once - **Efficient use of storage** - leave data
 compressed while not in use - **Batch Processing** - We can't store all
 information in memory, so break problems up - **Speed** - Find and avoid
 bottlenecks of big data processing ## Requirements - `python 3.10+` ## Getting
-Started ### Users ```sh pip install stocktracer # Perform analysis stocktracer
-analyze --tickers aapl,msft > report.txt # Help stocktracer ``` ### Developers
-Make sure you have `pipenv` installed through a package manager or through pip.
-```sh pipenv install --dev # Perform analysis PYTHONPATH=src pipenv run python
--m stocktracer analyze --tickers aapl,msft PYTHONPATH=src pipenv run python -
-m stocktracer analyze --tickers aapl,msft -a stocktracer.analysis.diluted_eps
-PYTHONPATH=src pipenv run python -m stocktracer analyze --tickers aapl,msft -
-a stocktracer.analysis.diluted_eps --report-format csv PYTHONPATH=src pipenv
-run python -m stocktracer analyze --tickers aapl,msft -
-a stocktracer.analysis.diluted_eps --report-format json --report-file
-my_results.json # Help PYTHONPATH=src pipenv run python -m stocktracer # Run
-Unit Tests pipenv run pytest ``` More information can be found in our
-[documentation](https://gyund.github.io/fundamental-analysis/) ## Disclaimer
-This project seeks to use publicly available information to perform security
-analysis and help perform long term risk analysis. Results provided from this
-project are generally for academic use only and are not considered advice or
-recommendations. This project makes no performance claims or guarantees. Please
-read the [license](LICENSE) for this project. Usage of any data is at your own
-risk.
+Started ### Users ```sh # basic install pip install stocktracer # with
+tensorflow dependencies for analysis modules pip install stocktracer
+[tensorflow] # Perform analysis stocktracer analyze --tickers aapl,msft >
+report.txt # Help stocktracer ``` For development guides, see our
+[documentation](https://gyund.github.io/fundamental-analysis/getting-started)
+## Disclaimer This project seeks to use publicly available information to
+perform security analysis and help perform long term risk analysis. Results
+provided from this project are generally for academic use only and are not
+considered advice or recommendations. This project makes no performance claims
+or guarantees. Please read the [license](LICENSE) for this project. Usage of
+any data is at your own risk.
```

### Comparing `stocktracer-0.3.0/pyproject.toml` & `stocktracer-0.4.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,14 @@
-[build-system]
-requires = ["hatchling", "hatch-requirements-txt"]
-build-backend = "hatchling.build"
-
-[tool.hatch.build.targets.wheel]
-only-include = ["src/stocktracer"]
-sources = ["src"]
-
-[project]
-name = "stocktracer"
-version = "0.3.0"
-authors = [
-  { name="Gary Yund", email="gary.yund@gmail.com" },
-]
-description = "Tools for aggregating efficient ways to consume and process publically traded equities on the US stock market. Includes support for SEC quarterly data processing."
-readme = "README.md"
-requires-python = ">=3.10"
-license = {file = "LICENSE"}
-keywords = [ "sec-tools", "fundamental analysis", "stocks" ]
-classifiers = [
-    "License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)",
-    "Operating System :: OS Independent",
-    "Topic :: Scientific/Engineering :: Information Analysis",
-    "Topic :: Office/Business :: Financial :: Investment",
-    "Intended Audience :: Science/Research",
-    "Development Status :: 2 - Pre-Alpha",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11"
-]
-
-dynamic = ["dependencies"]
-
-[tool.hatch.metadata.hooks.requirements_txt]
-files = ["requirements.txt"]
-
-[project.urls]
-"Homepage" = "https://gyund.github.io/fundamental-analysis/"
-"Bug Tracker" = "https://github.com/gyund/fundamental-analysis/issues"
-
-[project.scripts]
-stocktracer = "stocktracer.__main__:main_cli"
-
 [tool.pytest.ini_options]
 # log_cli = true
 log_cli_level = "INFO"
 log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(pathname)s:%(lineno)s)"
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
 testpaths = [
-    "src/",
+    "src/tests",
 ]
 # addopts = [
 #     "--import-mode=importlib",
 # ]
 
 markers =[
     "webtest: mark a test as a webtest. These kinds of tests can trigger downloads or other network interactions.",
@@ -125,8 +82,89 @@
 # disable=["W1203"]
 # disable=["all"]
 
 [tool.pylint.format]
 max-line-length = "88"
 
 [tool.pylint.reports]
-output-format = ["colorized"]
+output-format = ["colorized"]
+
+
+[tool.poetry]
+name = "stocktracer"
+version = "0.4.0"
+description = "Tools for aggregating efficient ways to consume and process publically traded equities on the US stock market. Includes support for SEC quarterly data processing."
+authors = ["Gary Yund <gyund@users.noreply.github.com>"]
+# Per https://github.com/python-poetry/poetry/issues/7786
+# license = "License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)"
+readme = "README.md"
+# homepage = "https://gyund.github.io/fundamental-analysis/"
+repository = "https://github.com/gyund/fundamental-analysis/"
+documentation = "https://gyund.github.io/fundamental-analysis/"
+keywords = [ "sec-tools", "fundamental analysis", "stocks" ]
+classifiers = [
+    "License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)",
+    "Operating System :: OS Independent",
+    "Topic :: Scientific/Engineering :: Information Analysis",
+    "Topic :: Office/Business :: Financial :: Investment",
+    "Intended Audience :: Science/Research",
+    "Development Status :: 2 - Pre-Alpha"
+]
+
+packages = [
+    { include = "stocktracer", from = "src" },
+]
+
+[tool.poetry.urls]
+"Bug Tracker" = "https://github.com/gyund/fundamental-analysis/issues"
+
+[tool.poetry.scripts]
+stocktracer = "stocktracer.__main__:main_cli"
+
+[tool.poetry.dependencies]
+python = ">=3.10, <3.12"
+alive-progress = "~3.1.3"
+beartype = "~0.14.0"
+diskcache = "~5.6.1"
+fire = "~0.5.0"
+pandas = "~2.0.1"
+platformdirs = "~3.5.1"
+python-dateutil = "~2.8.2"
+requests = "~2.31.0"
+requests-cache = "~1.0.1"
+tabulate = "~0.9.0"
+tensorflow-decision-forests = { version = "^1.3.0", optional = true }
+
+[tool.poetry.group.dev.dependencies]
+coverage = "*"
+coveralls = "^3.3.1"
+black = "^23.3.0"
+build = "^0.10.0"
+isort = "^5.12.0"
+mock = "~5.0.2"
+pydocstyle = {extras = ["toml"], version = "~6.3.0"}
+pydoctest = "~0.1.22"
+pylint = "~2.17.4"
+pytest = "~7.3.1"
+pytest-benchmark = "~4.0.0"
+pytest-cov = "~4.1.0"
+ruff = "~0.0.270"
+
+[tool.poetry.extras]
+
+tensorflow = ["tensorflow-decision-forests"]
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+mkdocs-gen-files = "~0.5.0"
+mkdocs-git-revision-date-localized-plugin = "~1.2.0"
+mkdocs-literate-nav = "~0.6.0"
+mkdocs-material = "~9.1.14"
+mkdocs-material-extensions = "~1.1.1"
+mkdocs-section-index = "~0.3.5"
+mkdocstrings-python = "~1.1.0"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

