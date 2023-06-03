# Comparing `tmp/clown_sort-1.6.4.tar.gz` & `tmp/clown_sort-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clown_sort-1.6.4.tar", max compression
+gzip compressed data, was "clown_sort-1.7.0.tar", max compression
```

## Comparing `clown_sort-1.6.4.tar` & `clown_sort-1.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3134 2023-06-02 22:23:44.794224 clown_sort-1.6.4/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.6.4/LICENSE
--rw-r--r--   0        0        0     8659 2023-05-28 21:20:43.213283 clown_sort-1.6.4/README.md
--rw-r--r--   0        0        0     3369 2023-05-27 22:11:48.831591 clown_sort-1.6.4/clown_sort/__init__.py
--rw-r--r--   0        0        0     7864 2023-05-28 21:12:17.679551 clown_sort-1.6.4/clown_sort/config.py
--rw-r--r--   0        0        0     9021 2023-06-02 20:58:04.234216 clown_sort-1.6.4/clown_sort/filename_extractor.py
--rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.6.4/clown_sort/files/image_file.py
--rw-r--r--   0        0        0     2756 2023-06-02 21:34:09.379034 clown_sort-1.6.4/clown_sort/files/pdf_file.py
--rw-r--r--   0        0        0    11399 2023-06-02 21:49:12.145554 clown_sort-1.6.4/clown_sort/files/sortable_file.py
--rwxr-xr-x   0        0        0     3310 2023-06-02 21:07:10.228823 clown_sort-1.6.4/clown_sort/sort_selector.py
--rw-r--r--   0        0        0    10270 2023-06-02 22:21:00.287460 clown_sort-1.6.4/clown_sort/sorting_rules/crypto.csv
--rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.6.4/clown_sort/util/argument_parser.py
--rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.6.4/clown_sort/util/constants.py
--rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.6.4/clown_sort/util/dict_helper.py
--rw-r--r--   0        0        0     3690 2023-06-02 22:06:05.123239 clown_sort-1.6.4/clown_sort/util/filesystem_helper.py
--rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.6.4/clown_sort/util/logging.py
--rw-r--r--   0        0        0     3427 2023-05-27 22:16:38.822426 clown_sort-1.6.4/clown_sort/util/rich_helper.py
--rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.6.4/clown_sort/util/string_helper.py
--rw-r--r--   0        0        0     1619 2023-06-02 22:23:44.801788 clown_sort-1.6.4/pyproject.toml
--rw-r--r--   0        0        0    10081 1970-01-01 00:00:00.000000 clown_sort-1.6.4/PKG-INFO
+-rw-r--r--   0        0        0     3216 2023-06-03 00:37:57.393324 clown_sort-1.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.7.0/LICENSE
+-rw-r--r--   0        0        0     8766 2023-06-03 00:17:25.185210 clown_sort-1.7.0/README.md
+-rw-r--r--   0        0        0     3369 2023-05-27 22:11:48.831591 clown_sort-1.7.0/clown_sort/__init__.py
+-rw-r--r--   0        0        0     7987 2023-06-03 00:19:42.985646 clown_sort-1.7.0/clown_sort/config.py
+-rw-r--r--   0        0        0     9021 2023-06-02 20:58:04.234216 clown_sort-1.7.0/clown_sort/filename_extractor.py
+-rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.7.0/clown_sort/files/image_file.py
+-rw-r--r--   0        0        0     2756 2023-06-02 21:34:09.379034 clown_sort-1.7.0/clown_sort/files/pdf_file.py
+-rw-r--r--   0        0        0    11399 2023-06-02 21:49:12.145554 clown_sort-1.7.0/clown_sort/files/sortable_file.py
+-rwxr-xr-x   0        0        0     3310 2023-06-02 21:07:10.228823 clown_sort-1.7.0/clown_sort/sort_selector.py
+-rw-r--r--   0        0        0    10323 2023-06-03 00:36:44.463991 clown_sort-1.7.0/clown_sort/sorting_rules/crypto.csv
+-rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.7.0/clown_sort/util/argument_parser.py
+-rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.7.0/clown_sort/util/constants.py
+-rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.7.0/clown_sort/util/dict_helper.py
+-rw-r--r--   0        0        0     3690 2023-06-02 22:06:05.123239 clown_sort-1.7.0/clown_sort/util/filesystem_helper.py
+-rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.7.0/clown_sort/util/logging.py
+-rw-r--r--   0        0        0     3427 2023-05-27 22:16:38.822426 clown_sort-1.7.0/clown_sort/util/rich_helper.py
+-rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.7.0/clown_sort/util/string_helper.py
+-rw-r--r--   0        0        0     1619 2023-06-03 00:37:57.396990 clown_sort-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0    10188 1970-01-01 00:00:00.000000 clown_sort-1.7.0/PKG-INFO
```

### Comparing `clown_sort-1.6.4/CHANGELOG.md` & `clown_sort-1.7.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # NEXT RELEASE
 
+# 1.7.0
+* Skip comment rows starting with `#` in rules CSVs.
+* New default rules
+
 ### 1.6.4
 * Crop very long PDF pages when previewing in manual select window
 * Fix regexes for wallet addresses
 * Gracefully handle failures in file timestamp copying call
 
 ### 1.6.3
 * Fix bug with manual folder selection
```

### Comparing `clown_sort-1.6.4/LICENSE` & `clown_sort-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.4/README.md` & `clown_sort-1.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,20 @@
 
 ### Help Screen
 ![](doc/sort_screenshots_help.png)
 
 (In my personal usuage I tend to run the tool with the `--all` and `--manual-fallback` options.)
 
 ### Custom Sorting Rules
-The default is to sort cryptocurrency related content but you can define your own CSV of rules with two columns `folder` and `regex`. The value in `folder` specifies the subdirectory to sort into and `regex` is the pattern to match against. See [the default crypto related configuration](clown_sort/sorting_rules/crypto.csv) for an example. An explanation of regular expressions is beyond the scope of this README but many resources are available to help. If you're not good at regexes just remember that any alphanumeric string is a regex that will match that string. [pythex](http://pythex.org/) is a great website for testing your regexes.
+The default is to sort cryptocurrency related content but you can define your own CSV of rules with two columns `folder` and `regex`.
+
+* Lines whose first non-whitespace character is `#` will be considered to be comments and skipped as will empty lines
+* `folder` specifies the subdirectory to sort into
+* `regex` is the pattern to match against. See [the default crypto related configuration](clown_sort/sorting_rules/crypto.csv) for an example. An explanation of regular expressions is beyond the scope of this README but many resources are available to help. If you're not good at regexes just remember that any alphanumeric string is a regex that will match that string. [pythex](http://pythex.org/) is a great website for testing your regexes.
+
 
 ### Example Output (Automated Sorting)
 ![](doc/output_example.png)
 
 
 ## Manually Sorting (Experimental)
 **This is an experimental feature.** It's only been tested on macOS.
```

### Comparing `clown_sort-1.6.4/clown_sort/__init__.py` & `clown_sort-1.7.0/clown_sort/__init__.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.4/clown_sort/config.py` & `clown_sort-1.7.0/clown_sort/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,18 @@
         return sorted(subdirs_of_dir(cls.sorted_screenshots_dir), key=lambda d: d.lower())
 
     @classmethod
     def _load_rules_csv(cls, file_path: Union[Path, str]) -> List[SortRule]:
         with open(Path(file_path), mode='r') as csvfile:
             return [
                 SortRule(row['folder'], re.compile(row['regex'], re.IGNORECASE | re.MULTILINE))
-                for row in csv.DictReader(csvfile, delimiter=',')
+                for row in csv.DictReader(
+                    filter(lambda _row: len(_row) > 0 and _row.lstrip()[0] != '#', csvfile),
+                    delimiter=','
+                )
             ]
 
     @classmethod
     def _rules_table(cls) -> Table:
         """Generate a table of the sort rules in effect."""
         table = Table(
             'Folder', 'Regex',
@@ -209,10 +212,10 @@
             style='bright_white'
         )
 
     console = Console()
     console.line()
     console.print(msg)
     console.line()
-    console.print(f"     pipx install clown_sort\[{module_name}] --force", style='bright_cyan')
+    console.print(f"     pipx install clown_sort\\[{module_name}] --force", style='bright_cyan')
     console.line()
     console.print(f"'pip install' works if you're not using pipx. Use 'poetry install --all-extras' if you're in a development environment.")
```

### Comparing `clown_sort-1.6.4/clown_sort/filename_extractor.py` & `clown_sort-1.7.0/clown_sort/filename_extractor.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.4/clown_sort/files/image_file.py` & `clown_sort-1.7.0/clown_sort/files/image_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.4/clown_sort/files/pdf_file.py` & `clown_sort-1.7.0/clown_sort/files/pdf_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.4/clown_sort/files/sortable_file.py` & `clown_sort-1.7.0/clown_sort/files/sortable_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.4/clown_sort/sort_selector.py` & `clown_sort-1.7.0/clown_sort/sort_selector.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.4/clown_sort/sorting_rules/crypto.csv` & `clown_sort-1.7.0/clown_sort/sorting_rules/crypto.csv`

 * *Files 2% similar despite different names*

```diff
@@ -18,27 +18,27 @@
 Bitdeer,Bitdeer
 BitGet,Bitget
 Bithumb,\bbithumb
 Bitmain,Bitmain
 Bitstamp,Bitstamp
 Bittrex,Bittrex|Ritchie[-_\s.]*Lai|Kiran[-_\s.]*Raj|John[-_\s.]*Roth\b|\bAquila\b
 Bitzlato,Bitzlato
-Blockchain.com,\bblockchain\.com\b|@blockchain\b|@AskBlockchain\b
+Blockchain.com,\bblockchain\.com\b|@blockchain\b|@AskBlockchain\b|Patrick[-_\s.]*McHenry
 Blockchain8,Blockchain8|tom[-_\s.]*emmer|ritchie[-_\s.]*torres|repritchie|Warren[-_\s.]*Davidson|Byron[-_\s.]*Donalds|Ted[-_\s.]*Budd|Josh[-_\s.]*Gotheimer|Jake[-_\s.]*Auchincloss|Darren[-_\s.]*Soto|ro[-_\s.]*khanna|KMSmithDC|Kristin[-_\s.]*Smith\b|Warren[-_\s.]*Davidson
 Blockchain Capital,Blockchain[-_\s.]*Capital|\bbrock\b|brockpierce
 BlockFi,BlockFi|Zac[-_\s.]*Prince|Brian[-_\s.]*Oliver
 Blockstream,Blockstream
 Bored Ape Yacht Club,BAYC|Bored[-_\s.]*Ape|yuga[-_\s.]*labs
-Bros,cryptomanran|trillionUSD|nic[-_\s.]*carter|bitboy|ben[-_\s.]*armstrong|basedkarbon|thecryptolark|adam([-_\s.]*back|3us)|@DegenSp|APompliano|IIICapital|\bMeltem\b|algodtrading|whatbitcoindid|CryptoKaleo|Mike[-_\s.]*Alfred|natbrunell|natalie[-_\s.]*brunell|stackersatoshi|Max[-_\s.]*Keiser|Cowboy[-_\s.]*Crypto|minimalcsgo|greg16676935420|@Aridavidpaul|\bAri[-_\s.]*Paul\b|raoul(gmi|[-_\s.]*pal)|mccormack|andr3w|andrew[-_\s.]*wang|\b(JW)?[-_\s.]*Verret\b
+Bros,cryptomanran|trillionUSD|nic[-_\s.]*carter|bitboy|ben[-_\s.]*armstrong|basedkarbon|thecryptolark|adam([-_\s.]*back|3us)|@DegenSp|APompliano|IIICapital|\bMeltem\b|algodtrading|whatbitcoindid|CryptoKaleo|Mike[-_\s.]*Alfred|natbrunell|natalie[-_\s.]*brunell|stackersatoshi|Max[-_\s.]*Keiser|Cowboy[-_\s.]*Crypto|minimalcsgo|greg16676935420|@Aridavidpaul|\bAri[-_\s.]*Paul\b|raoul(gmi|[-_\s.]*pal)|mccormack|andr3w|andrew[-_\s.]*wang|\b(JW)?[-_\s.]*Verret\b|@FlurETH\b
 Broettes,Nicole[-_\s.]*Behnam|natbrunell
 Bybit,\bBybit\b|Ben[-_\s.]*Zhou|InvestByBit|TravelByBit
 Cardano,Cardano|[$\s]ADA[^\w]|Hoskinson|\bIOHK
 Cathie Wood,Cathie[-_\s.]*Wood|\bARK(F|G|K|[-_\s.]*Innovation|[-_\s.]*Invest)|\bIZRL
 Celsius,celsius|mashinsky|levity[-_\s.]*and[-_\s.]*love|\bcelsian|Artur[-_\s.]*Abreu|ronpaulbot|\bnuke[-_\s.]*gold(stein)?
-China,fentanyl|chin(a|ese)
+China,fentanyl|\bchin(a|ese)|Hong[-_\s.]*Kong
 Circle,[@#]circle|usdc|circle[-_\s.]*internet|disparte|\ballaire|jerallaire
 CMCC Global,CMCC[-_\s.]*Global
 Coinbase,Coinbase|\$COIN|brian[-_\s.]*armstrong|grewal\b|Asiff[-_\s.]*Hirji|\bbalaji|Fred[-_\s.]*Ehrsam|\bremitly\b|\$RELY\b
 Coinflex,Mark[-_\s.]*Lamb|Roger[-_\s.]*Ver|coinflex|Doug[-_\s.]*Polk|OPNX|flexusd|Leslie[-_\s.]*Lamb|dougpolkvids
 CoinLoan,coinloan|Faliushin\b
 CompoundFi,compoundfi|leshner|\bgonen\b
 ConsenSys,ConsenSys
```

### Comparing `clown_sort-1.6.4/clown_sort/util/argument_parser.py` & `clown_sort-1.7.0/clown_sort/util/argument_parser.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.4/clown_sort/util/constants.py` & `clown_sort-1.7.0/clown_sort/util/constants.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.4/clown_sort/util/filesystem_helper.py` & `clown_sort-1.7.0/clown_sort/util/filesystem_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.4/clown_sort/util/rich_helper.py` & `clown_sort-1.7.0/clown_sort/util/rich_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.4/clown_sort/util/string_helper.py` & `clown_sort-1.7.0/clown_sort/util/string_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.6.4/pyproject.toml` & `clown_sort-1.7.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clown_sort"
-version = "1.6.4"
+version = "1.7.0"
 description = "Sort screenshots based on rules or through individual review."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 readme = "README.md"
 packages = [{include = "clown_sort"}]
 homepage = "https://github.com/michelcrypt4d4mus/clown_sort"
 
 include = [
```

### Comparing `clown_sort-1.6.4/PKG-INFO` & `clown_sort-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clown-sort
-Version: 1.6.4
+Version: 1.7.0
 Summary: Sort screenshots based on rules or through individual review.
 Home-page: https://github.com/michelcrypt4d4mus/clown_sort
 Keywords: ocr,organization,organizer,screenshot,rename,sort
 Author: Michel de Cryptadamus
 Author-email: michel@cryptadamus.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -138,15 +138,20 @@
 
 ### Help Screen
 ![](doc/sort_screenshots_help.png)
 
 (In my personal usuage I tend to run the tool with the `--all` and `--manual-fallback` options.)
 
 ### Custom Sorting Rules
-The default is to sort cryptocurrency related content but you can define your own CSV of rules with two columns `folder` and `regex`. The value in `folder` specifies the subdirectory to sort into and `regex` is the pattern to match against. See [the default crypto related configuration](clown_sort/sorting_rules/crypto.csv) for an example. An explanation of regular expressions is beyond the scope of this README but many resources are available to help. If you're not good at regexes just remember that any alphanumeric string is a regex that will match that string. [pythex](http://pythex.org/) is a great website for testing your regexes.
+The default is to sort cryptocurrency related content but you can define your own CSV of rules with two columns `folder` and `regex`.
+
+* Lines whose first non-whitespace character is `#` will be considered to be comments and skipped as will empty lines
+* `folder` specifies the subdirectory to sort into
+* `regex` is the pattern to match against. See [the default crypto related configuration](clown_sort/sorting_rules/crypto.csv) for an example. An explanation of regular expressions is beyond the scope of this README but many resources are available to help. If you're not good at regexes just remember that any alphanumeric string is a regex that will match that string. [pythex](http://pythex.org/) is a great website for testing your regexes.
+
 
 ### Example Output (Automated Sorting)
 ![](doc/output_example.png)
 
 
 ## Manually Sorting (Experimental)
 **This is an experimental feature.** It's only been tested on macOS.
```

