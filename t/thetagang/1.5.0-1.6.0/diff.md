# Comparing `tmp/thetagang-1.5.0.tar.gz` & `tmp/thetagang-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thetagang-1.5.0.tar", max compression
+gzip compressed data, was "thetagang-1.6.0.tar", max compression
```

## Comparing `thetagang-1.5.0.tar` & `thetagang-1.6.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0    34523 2023-04-11 11:55:13.557196 thetagang-1.5.0/LICENSE
--rw-r--r--   0        0        0    14673 2023-04-11 11:55:13.557196 thetagang-1.5.0/README.md
--rw-r--r--   0        0        0     1618 2023-04-11 11:55:13.557196 thetagang-1.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/__init__.py
--rw-r--r--   0        0        0     7734 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/config.py
--rw-r--r--   0        0        0      642 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/config_defaults.py
--rw-r--r--   0        0        0     1461 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/dict_merge.py
--rw-r--r--   0        0        0       59 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/entry.py
--rw-r--r--   0        0        0     1022 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/main.py
--rw-r--r--   0        0        0      376 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/options.py
--rw-r--r--   0        0        0    47953 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/portfolio_manager.py
--rw-r--r--   0        0        0     3951 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/test_util.py
--rwxr-xr-x   0        0        0     7753 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/thetagang.py
--rw-r--r--   0        0        0     5323 2023-04-11 11:55:13.561197 thetagang-1.5.0/thetagang/util.py
--rw-r--r--   0        0        0    15937 1970-01-01 00:00:00.000000 thetagang-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-03 13:21:31.628847 thetagang-1.6.0/LICENSE
+-rw-r--r--   0        0        0    14673 2023-06-03 13:21:31.628847 thetagang-1.6.0/README.md
+-rw-r--r--   0        0        0     1634 2023-06-03 13:21:31.632847 thetagang-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/__init__.py
+-rw-r--r--   0        0        0     8247 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/config.py
+-rw-r--r--   0        0        0     1068 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/config_defaults.py
+-rw-r--r--   0        0        0     1461 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/dict_merge.py
+-rw-r--r--   0        0        0       59 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/entry.py
+-rw-r--r--   0        0        0     1091 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/fmt.py
+-rw-r--r--   0        0        0     1022 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/main.py
+-rw-r--r--   0        0        0      376 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/options.py
+-rw-r--r--   0        0        0    67559 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/portfolio_manager.py
+-rw-r--r--   0        0        0     3951 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/test_util.py
+-rwxr-xr-x   0        0        0     8433 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/thetagang.py
+-rw-r--r--   0        0        0     5488 2023-06-03 13:21:31.636847 thetagang-1.6.0/thetagang/util.py
+-rw-r--r--   0        0        0    15885 1970-01-01 00:00:00.000000 thetagang-1.6.0/PKG-INFO
```

### Comparing `thetagang-1.5.0/LICENSE` & `thetagang-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thetagang-1.5.0/README.md` & `thetagang-1.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 starts back at the beginning. Please keep in mind this may have tax
 implications, but that is outside the scope of this README.
 
 In normal usage, you would run the script as a cronjob on a daily, weekly, or
 monthly basis according to your preferences. Running more frequently than
 daily is not recommended, but the choice is yours.
 
-![Paper account sample output](sample.gif)
+![Paper account sample output](sample.png)
 
 ## Project status
 
 This project is, in its current state, considered to be complete. I'm open
 to contributions, but I am unlikely to accept PRs or feature requests that
 involve significant changes to the underlying algorithm.
```

### Comparing `thetagang-1.5.0/pyproject.toml` & `thetagang-1.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 description = "ThetaGang is an IBKR bot for getting money"
 documentation = "https://github.com/brndnmtthws/thetagang/blob/master/README.md"
 homepage = "https://github.com/brndnmtthws/thetagang"
 license = "AGPL-3.0-only"
 name = "thetagang"
 readme = "README.md"
 repository = "https://github.com/brndnmtthws/thetagang.git"
-version = "1.5.0"
+version = "1.6.0"
 
 [tool.poetry.dependencies]
 click = "^8.1.3"
 click-log = "^0.4.0"
-colorama = "^0.4.6"
 ib_insync = "^0.9.81"
-python = ">=3.8,<4.0"
+python = ">=3.9,<4.0"
 python-dateutil = "^2.8.1"
 pytimeparse = "^1.1.8"
-schema = "^0.7.3"
+schema = "^0.7.5"
 toml = "^0.10.2"
+rich = "^13.3.5"
 
 [tool.poetry.group.dev.dependencies]
 autoflake = "^2.0"
-autohooks = "^23.1.0"
-autohooks-plugin-black = "^22.11.0"
-autohooks-plugin-isort = "^22.8.0"
-autohooks-plugin-pylint = "^22.8.1"
+autohooks = "^23.4.0"
+autohooks-plugin-black = ">=22.11,<24.0"
+autohooks-plugin-isort = ">=22.8,<24.0"
+autohooks-plugin-pylint = ">=22.8.1,<24.0.0"
 black = "^23.1.0"
 isort = "^5.12.0"
 pylint = "^2.16.2"
 pytest = "^7.2.1"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/brndnmtthws/thetagang/issues"
```

### Comparing `thetagang-1.5.0/thetagang/config.py` & `thetagang-1.6.0/thetagang/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import math
 
-import click
+from rich.console import Console
 from schema import And, Optional, Or, Schema
 
 import thetagang.config_defaults as config_defaults
 from thetagang.dict_merge import dict_merge
 
+error_console = Console(stderr=True, style="bold red")
+console = Console()
+
 
 def normalize_config(config):
     # Do any pre-processing necessary to the config here, such as handling
     # defaults, deprecated values, config changes, etc.
 
     if "twsVersion" in config["ibc"]:
-        click.secho(
+        error_console.print(
             "WARNING: config param ibc.twsVersion is deprecated, please remove it from your config.",
-            fg="yellow",
-            err=True,
         )
 
         # TWS version is pinned to latest stable, delete any existing config if it's present
         del config["ibc"]["twsVersion"]
 
     if "maximum_new_contracts" in config["target"]:
-        click.secho(
+        error_console.print(
             "WARNING: config param target.maximum_new_contracts is deprecated, please remove it from your config.",
-            fg="yellow",
-            err=True,
         )
 
         del config["target"]["maximum_new_contracts"]
 
     # xor: should have weight OR parts, but not both
     if any(["weight" in s for s in config["symbols"].values()]) == any(
         ["parts" in s for s in config["symbols"].values()]
@@ -179,14 +178,26 @@
                 Optional("probeContract"): {
                     Optional("currency"): And(str, len),
                     Optional("exchange"): And(str, len),
                     Optional("secType"): And(str, len),
                     Optional("symbol"): And(str, len),
                 },
             },
+            Optional("vix_call_hedge"): {
+                "enabled": bool,
+                Optional("delta"): And(float, lambda n: 0 <= n <= 1),
+                Optional("close_hedges_when_vix_exceeds"): float,
+                Optional("allocation"): [
+                    {
+                        Optional("lower_bound"): float,
+                        Optional("upper_bound"): float,
+                        Optional("weight"): float,
+                    },
+                ],
+            },
         }
     )
     schema.validate(config)
 
     assert len(config["symbols"]) > 0
 
     assert math.isclose(
```

### Comparing `thetagang-1.5.0/thetagang/dict_merge.py` & `thetagang-1.6.0/thetagang/dict_merge.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.5.0/thetagang/main.py` & `thetagang-1.6.0/thetagang/main.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.5.0/thetagang/test_util.py` & `thetagang-1.6.0/thetagang/test_util.py`

 * *Files identical despite different names*

### Comparing `thetagang-1.5.0/thetagang/util.py` & `thetagang-1.6.0/thetagang/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 import math
 from datetime import datetime
 
 from ib_insync import util
 from ib_insync.contract import Option
 
 
-def to_camel_case(snake_str):
-    components = snake_str.split("_")
-    # We capitalize the first letter of each component except the first one
-    # with the 'title' method and join them together.
-    return components[0] + "".join(x.title() for x in components[1:])
-
-
 def account_summary_to_dict(account_summary):
     d = dict()
     for s in account_summary:
         d[s.tag] = s
     return d
 
 
@@ -63,41 +56,57 @@
                 ]
             )
         )
 
     return 0
 
 
+def net_option_positions(symbol, portfolio_positions, right):
+    if symbol in portfolio_positions:
+        return math.floor(
+            sum(
+                [
+                    p.position
+                    for p in portfolio_positions[symbol]
+                    if isinstance(p.contract, Option)
+                    and p.contract.right.upper().startswith(right.upper())
+                ]
+            )
+        )
+
+    return 0
+
+
 def wait_n_seconds(pred, body, seconds_to_wait, started_at=None):
     if not started_at:
         started_at = datetime.now()
     diff = datetime.now() - started_at
     remaining = seconds_to_wait - diff.seconds
     if not remaining or remaining <= 0 or math.isclose(remaining, 0.0):
         raise RuntimeError(
             "Exhausted retries waiting on predicate. This shouldn't happen."
         )
     if pred():
         body(remaining)
         wait_n_seconds(pred, body, seconds_to_wait, started_at)
 
 
-def get_highest_price(ticker):
+def get_higher_price(ticker):
     # Returns the highest of either the option model price, the midpoint, or the
     # market price. The midpoint is usually a bit higher than the IB model's
     # pricing, but we want to avoid leaving money on the table in cases where
     # the spread might be messed up. This may in some cases make it harder for
     # orders to fill in a given day, but I think that's a reasonable tradeoff to
     # avoid leaving money on the table.
     if ticker.modelGreeks:
         return max([midpoint_or_market_price(ticker), ticker.modelGreeks.optPrice])
     return midpoint_or_market_price(ticker)
 
 
-def get_lowest_price(ticker):
+def get_lower_price(ticker):
     # Same as get_highest_price(), except get the lower price instead.
     if ticker.modelGreeks:
         return min([midpoint_or_market_price(ticker), ticker.modelGreeks.optPrice])
     return midpoint_or_market_price(ticker)
 
 
 def midpoint_or_market_price(ticker):
```

### Comparing `thetagang-1.5.0/PKG-INFO` & `thetagang-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: thetagang
-Version: 1.5.0
+Version: 1.6.0
 Summary: ThetaGang is an IBKR bot for getting money
 Home-page: https://github.com/brndnmtthws/thetagang
 License: AGPL-3.0-only
 Author: Brenden Matthews
 Author-email: brenden@brndn.io
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-log (>=0.4.0,<0.5.0)
-Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: ib_insync (>=0.9.81,<0.10.0)
 Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
 Requires-Dist: pytimeparse (>=1.1.8,<2.0.0)
-Requires-Dist: schema (>=0.7.3,<0.8.0)
+Requires-Dist: rich (>=13.3.5,<14.0.0)
+Requires-Dist: schema (>=0.7.5,<0.8.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Bug Tracker, https://github.com/brndnmtthws/thetagang/issues
 Project-URL: Documentation, https://github.com/brndnmtthws/thetagang/blob/master/README.md
 Project-URL: GitHub, https://github.com/brndnmtthws/thetagang
 Project-URL: Repository, https://github.com/brndnmtthws/thetagang.git
 Description-Content-Type: text/markdown
 
@@ -98,15 +97,15 @@
 starts back at the beginning. Please keep in mind this may have tax
 implications, but that is outside the scope of this README.
 
 In normal usage, you would run the script as a cronjob on a daily, weekly, or
 monthly basis according to your preferences. Running more frequently than
 daily is not recommended, but the choice is yours.
 
-![Paper account sample output](sample.gif)
+![Paper account sample output](sample.png)
 
 ## Project status
 
 This project is, in its current state, considered to be complete. I'm open
 to contributions, but I am unlikely to accept PRs or feature requests that
 involve significant changes to the underlying algorithm.
```

