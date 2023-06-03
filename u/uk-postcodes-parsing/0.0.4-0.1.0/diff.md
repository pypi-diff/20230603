# Comparing `tmp/uk_postcodes_parsing-0.0.4.tar.gz` & `tmp/uk_postcodes_parsing-0.1.0.tar.gz`

## Comparing `uk_postcodes_parsing-0.0.4.tar` & `uk_postcodes_parsing-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/src/uk_postcodes_parsing/__init__.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/src/uk_postcodes_parsing/fix.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/src/uk_postcodes_parsing/postcode_utils.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/src/uk_postcodes_parsing/ukpostcode.py
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/tests/test_all.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/tests/data/postcode_parse_test.csv
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/LICENSE
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/README.md
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/src/uk_postcodes_parsing/__init__.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/src/uk_postcodes_parsing/fix.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/src/uk_postcodes_parsing/postcode_utils.py
+-rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/src/uk_postcodes_parsing/ukpostcode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/tests/test_all.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/tests/data/postcode_parse_test.csv
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/README.md
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/PKG-INFO
```

### Comparing `uk_postcodes_parsing-0.0.4/.github/workflows/python-publish.yml` & `uk_postcodes_parsing-0.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.0.4/.github/workflows/test.yml` & `uk_postcodes_parsing-0.1.0/.github/workflows/test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -26,8 +26,8 @@
           pip install black pytest pandas
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
       - name: Lint check with black
         run: |
           black src/uk_postcodes_parsing/ --check 
       - name: Test with pytest
         run: |
-          pytest
+          pytest -v
```

### Comparing `uk_postcodes_parsing-0.0.4/src/uk_postcodes_parsing/fix.py` & `uk_postcodes_parsing-0.1.0/src/uk_postcodes_parsing/fix.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,52 +2,85 @@
 
 FIXABLE_REGEX = re.compile(
     r"^\s*[a-z01]{1,2}[0-9oi][a-z\d]?\s*[0-9oi][a-z01]{2}\s*$", re.I
 )
 
 
 def fix(s: str) -> str:
-    match = FIXABLE_REGEX.match(s)
-    if match is None:
+    """Attempts to fix a given postcode
+
+    Args:
+        s (str): The postcode to fix
+    Returns:
+        str: The fixed postcode
+    """
+    if not FIXABLE_REGEX.match(s):
         return s
     s = s.upper().strip().replace(r"\s+", "")
     inward = s[-3:].strip()
     outward = s[:-3].strip()
     return f"{coerce_outcode(outward)} {coerce_incode(inward)}"
 
 
-def to_letter(c: str) -> str:
+def to_letter(char: str) -> str:
+    """
+    Convert a number to a letter if possible. For example,
+        "0" => "O"
+        "1" => "I"
+
+    Args:
+        c (str): The number to convert
+    Returns:
+        str: The letter
+    """
     return {
         "0": "O",
         "1": "I",
-    }.get(c, c)
+    }.get(char, char)
 
 
-def to_number(c: str) -> str:
+def to_number(char: str) -> str:
+    """
+    Convert a letter to a number if possible. For example,
+        "O" => "0"
+        "I" => "1"
+
+    Args:
+        c (str): The letter to convert
+    Returns:
+        str: The number
+    """
     return {
         "O": "0",
         "I": "1",
-    }.get(c, c)
+    }.get(char, char)
 
 
-def coerce(pattern: str, input: str) -> str:
+def coerce(pattern: str, string: str) -> str:
     """
-    Coerce a given input into a pattern. For e.g.
-            pattern: "LN" => signifies a letter followed by a number
-            input: "01" => changes to "O1". Where the first 0 should be a letter so it
-                is coverted from 0 to O. The Second 1 is already correct so no change.
+    Coerce a given string into a pattern. For e.g.
+        pattern: "LN" => signifies a letter followed by a number
+        input: "01" => changes to "O1". Where the first 0 should be a letter so it
+            is coverted from 0 to O. The Second 1 is already correct so no change.
+
+    Args:
+        pattern (str): The pattern to coerce the string into
+        string (str): The string to coerce
+
+    Returns:
+        str: The coerced string (with the pattern applied to it)
     """
     return "".join(
         to_number(c) if target == "N" else to_letter(c) if target == "L" else c
-        for c, target in zip(input, pattern)
+        for c, target in zip(string, pattern)
     )
 
 
 def coerce_outcode(i: str) -> str:
-    """Coerce outcode based on length of outcode"""
+    """Coerce outcode"""
     if len(i) == 2:
         return coerce("LN", i)
     elif len(i) == 3:
         return coerce("L??", i)
     elif len(i) == 4:
         return coerce("LLN?", i)
     else:
```

### Comparing `uk_postcodes_parsing-0.0.4/tests/test_all.py` & `uk_postcodes_parsing-0.1.0/tests/test_all.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import pandas as pd
 
 from uk_postcodes_parsing.fix import fix
 from uk_postcodes_parsing import ukpostcode
-from uk_postcodes_parsing.ukpostcode import parse_from_corpus, Postcode
+from uk_postcodes_parsing.ukpostcode import (
+    parse_from_corpus,
+    Postcode,
+)
 
 
 def test_fix():
     # Trims postcode
     assert fix(" SW1A 2AA ") == "SW1A 2AA"
     # Upper case
     assert fix(" Sw1A 2aa ") == "SW1A 2AA"
@@ -73,15 +76,15 @@
             district="E3",
             sub_district=None,
             sector="E3 4",
             unit="SS",
         ),
     ]
 
-    corpus = "this is a check to see if we can get post codes liek thia ec1r 1ub , and that e34ss. But also eh16 50y and ei412"
+    corpus = "this is a check to see if we can get post codes liek thia ec1r 1ub , and that e34ss. But also eh16 50y and ei412. followed by ehi6 50y"
     lst = parse_from_corpus(corpus, attempt_fix=True)
     assert lst == [
         Postcode(
             original="ec1r 1ub",
             postcode="EC1R 1UB",
             incode="1UB",
             outcode="EC1R",
@@ -109,14 +112,25 @@
             outcode="EH16",
             area="EH",
             district="EH16",
             sub_district=None,
             sector="EH16 5",
             unit="OY",
         ),
+        Postcode(
+            original="ehi6 50y",
+            postcode="EH16 5OY",
+            incode="5OY",
+            outcode="EH16",
+            area="EH",
+            district="EH16",
+            sub_district=None,
+            sector="EH16 5",
+            unit="OY",
+        ),
     ]
 
 
 def test_parsing_detailed():
     df = pd.read_csv("tests/data/postcode_parse_test.csv")
     df = df.where(pd.notnull(df), None)
 
@@ -126,7 +140,58 @@
         assert parsed_postcode.outcode == df.iloc[i][".outcode"]
         assert parsed_postcode.incode == df.iloc[i][".incode"]
         assert parsed_postcode.area == df.iloc[i][".area"]
         assert parsed_postcode.district == df.iloc[i][".district"]
         assert parsed_postcode.sub_district == df.iloc[i][".subDistrict"]
         assert parsed_postcode.sector == df.iloc[i][".sector"]
         assert parsed_postcode.unit == df.iloc[i][".unit"]
+
+
+def test_sort_by_fix_distance():
+    corpus = "this EC1r 1ub followed by to one, ecir iub e0 i00"
+    lst = parse_from_corpus(corpus, attempt_fix=True)
+    assert sorted(lst, reverse=True) == [
+        Postcode(
+            original="ecir iub",
+            postcode="EC1R 1UB",
+            incode="1UB",
+            outcode="EC1R",
+            area="EC",
+            district="EC1",
+            sub_district="EC1R",
+            sector="EC1R 1",
+            unit="UB",
+        ),
+        Postcode(
+            original="ec1r 1ub",
+            postcode="EC1R 1UB",
+            incode="1UB",
+            outcode="EC1R",
+            area="EC",
+            district="EC1",
+            sub_district="EC1R",
+            sector="EC1R 1",
+            unit="UB",
+        ),
+        Postcode(
+            original="e0 i00",
+            postcode="E0 1OO",
+            incode="1OO",
+            outcode="E0",
+            area="E",
+            district="E0",
+            sub_district=None,
+            sector="E0 1",
+            unit="OO",
+        ),
+        Postcode(
+            original="to one",
+            postcode="T0 0NE",
+            incode="0NE",
+            outcode="T0",
+            area="T",
+            district="T0",
+            sub_district=None,
+            sector="T0 0",
+            unit="NE",
+        ),
+    ]
```

### Comparing `uk_postcodes_parsing-0.0.4/.gitignore` & `uk_postcodes_parsing-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.0.4/LICENSE` & `uk_postcodes_parsing-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.0.4/README.md` & `uk_postcodes_parsing-0.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -36,39 +36,41 @@
 
 ```python
 >>> from uk_postcodes_parsing import ukpostcode
 >>> corpus = "this is a check to see if we can get post codes liek thia ec1r 1ub , and that e3 4ss. But also eh16 50y and ei412"          
 >>> postcodes = ukpostcode.parse_from_corpus(corpus)
 INFO:uk-postcodes-parsing:Found 2 postcodes in corpus
 >>> print(postcodes)
-[Postcode(original='ec1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB'), Postcode(original='e34ss', postcode='E3 4SS', incode='4SS', outcode='E3', area='E', district='E3', sub_district=None, sector='E3 4', unit='SS')]
+[Postcode(verified_against_postcode_io=True, fix_distance=0, original='ec1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB'), Postcode(verified_against_postcode_io=True, fix_distance=0, original='e3 4ss', postcode='E3 4SS', incode='4SS', outcode='E3', area='E', district='E3', sub_district=None, sector='E3 4', unit='SS')]
 ```
 
 - Optional auto-correct: Attempt correcting common mistakes in postcodes such as reading "O" and "0" and vice-versa.
 
 ```python
 >>> from uk_postcodes_parsing import ukpostcode
 >>> corpus = "this is a check to see if we can get post codes liek thia ec1r 1ub , and that e3 4ss. But also eh16 50y and ei412"          
 >>> postcodes = ukpostcode.parse_from_corpus(corpus, attempt_fix=True)
-INFO:uk-postcodes-parsing:Postcode Fixed: 'eh16 50y' => 'EH16 5OY'
 INFO:uk-postcodes-parsing:Found 3 postcodes in corpus
+INFO:uk-postcodes-parsing:Postcode Fixed: 'eh16 50y' => 'EH16 5OY'
 ```
 
 - Parsing
 
 ```python
 >>> from uk_postcodes_parsing import ukpostcode
 >>> ukpostcode.parse("EC1r 1ub")
-Postcode(original='ec1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB')
+Postcode(verified_against_postcode_io=True, fix_distance=0, original='EC1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB')
 ```
+
 ```python
 >>> ukpostcode.parse("EH16 50Y")
-INFO:uk-postcodes-parsing:Postcode Fixed: 'eh16 50y' => 'EH16 5OY'
-Postcode(original='eh16 50y', postcode='EH16 5OY', incode='5OY', outcode='EH16', area='EH', district='EH16', sub_district=None, sector='EH16 5', unit='OY')
+INFO:uk-postcodes-parsing:Postcode Fixed: 'EH16 50Y' => 'EH16 5OY'
+Postcode(verified_against_postcode_io=False, fix_distance=1, original='EH16 50Y', postcode='EH16 5OY', incode='5OY', outcode='EH16', area='EH', district='EH16', sub_district=None, sector='EH16 5', unit='OY')
 ```
+
 ```python
 >>> ukpostcode.parse("EH16 50Y", attempt_fix=False) # Don't attempt fixes during parsing
 ERROR:uk-postcodes-parsing:Failed to parse postcode
 >>> ukpostcode.parse("0W1") 
 ERROR:uk-postcodes-parsing:Unable to fix postcode
 ERROR:uk-postcodes-parsing:Failed to parse postcode
 ```
@@ -87,14 +89,44 @@
 
 ```python
 >>> from uk_postcodes_parsing.fix import fix
 >>> fix("0W1 OAA") 
 'OW1 0AA'
 ```
 
+# Postcode class definition
+
+```python
+@dataclass(order=True)
+class Postcode:
+    # Calculate post initialization
+    verified_against_postcode_io: bool = field(init=False)
+    fix_distance: int = field(init=False)
+    # raw text
+    original: str 
+    # The rest of the fields are parsed from the postcode using regex
+    postcode: str
+    incode: str
+    outcode: str
+    area: str
+    district: str
+    sub_district: Union[str, None]
+    sector: str
+    unit: str
+
+```
+
+- 2 fileds calculated after init of class
+  - `verified_against_postcode_io`: Check against [`api.postcodes.io/postcodes/`](https://postcodes.io/) which uses the [ONS Postcode Directory](https://geoportal.statistics.gov.uk/datasets/489c152010a3425f80a71dc3663f73e1/about)
+  - `fix_distance`: A measure of number of characters changed from raw text via auto-fix to get a valid post code. 
+    - E.g. `SW1A OAA` => `SW1A 0AA` has fix_distance=1. Where as, `SWIA OAA` => `SW1A 0AA` has fix_distance=2.
+  - These fields are particularly helpful using `parse_from_corpus` with `attempt_fix=True` which might return many potential postcodes. These field can be used as proxy for confidence on which parsed postcodes are correct.
+- `raw_text`: To keep track of the original string without formatting changes and auto-fixes.
+- 8 fileds are parsed using regex
+
 # Testing
 
 ```bash
 pytest tests/
 ```
 
 ## Similar works
```

### Comparing `uk_postcodes_parsing-0.0.4/pyproject.toml` & `uk_postcodes_parsing-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "uk_postcodes_parsing"
-version = "0.0.4"
+version = "0.1.0"
 authors = [
   { name="Anirudh Gangwal", email="angangwa@amazon.com" },
 ]
+dependencies = ["requests"]
 description = "A Python package to parge UK postcodes from text. Useful in applications such as OCR and IDP."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -27,8 +28,8 @@
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
 testpaths = [
     "tests/",
-]
+]
```

### Comparing `uk_postcodes_parsing-0.0.4/PKG-INFO` & `uk_postcodes_parsing-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: uk_postcodes_parsing
-Version: 0.0.4
+Version: 0.1.0
 Summary: A Python package to parge UK postcodes from text. Useful in applications such as OCR and IDP.
 Project-URL: Homepage, https://github.com/anirudhgangwal/ukpostcodes
 Project-URL: Bug Tracker, https://github.com/anirudhgangwal/ukpostcodes/issues
 Author-email: Anirudh Gangwal <angangwa@amazon.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: requests
 Provides-Extra: lint
 Requires-Dist: black; extra == 'lint'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
@@ -55,39 +56,41 @@
 
 ```python
 >>> from uk_postcodes_parsing import ukpostcode
 >>> corpus = "this is a check to see if we can get post codes liek thia ec1r 1ub , and that e3 4ss. But also eh16 50y and ei412"          
 >>> postcodes = ukpostcode.parse_from_corpus(corpus)
 INFO:uk-postcodes-parsing:Found 2 postcodes in corpus
 >>> print(postcodes)
-[Postcode(original='ec1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB'), Postcode(original='e34ss', postcode='E3 4SS', incode='4SS', outcode='E3', area='E', district='E3', sub_district=None, sector='E3 4', unit='SS')]
+[Postcode(verified_against_postcode_io=True, fix_distance=0, original='ec1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB'), Postcode(verified_against_postcode_io=True, fix_distance=0, original='e3 4ss', postcode='E3 4SS', incode='4SS', outcode='E3', area='E', district='E3', sub_district=None, sector='E3 4', unit='SS')]
 ```
 
 - Optional auto-correct: Attempt correcting common mistakes in postcodes such as reading "O" and "0" and vice-versa.
 
 ```python
 >>> from uk_postcodes_parsing import ukpostcode
 >>> corpus = "this is a check to see if we can get post codes liek thia ec1r 1ub , and that e3 4ss. But also eh16 50y and ei412"          
 >>> postcodes = ukpostcode.parse_from_corpus(corpus, attempt_fix=True)
-INFO:uk-postcodes-parsing:Postcode Fixed: 'eh16 50y' => 'EH16 5OY'
 INFO:uk-postcodes-parsing:Found 3 postcodes in corpus
+INFO:uk-postcodes-parsing:Postcode Fixed: 'eh16 50y' => 'EH16 5OY'
 ```
 
 - Parsing
 
 ```python
 >>> from uk_postcodes_parsing import ukpostcode
 >>> ukpostcode.parse("EC1r 1ub")
-Postcode(original='ec1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB')
+Postcode(verified_against_postcode_io=True, fix_distance=0, original='EC1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB')
 ```
+
 ```python
 >>> ukpostcode.parse("EH16 50Y")
-INFO:uk-postcodes-parsing:Postcode Fixed: 'eh16 50y' => 'EH16 5OY'
-Postcode(original='eh16 50y', postcode='EH16 5OY', incode='5OY', outcode='EH16', area='EH', district='EH16', sub_district=None, sector='EH16 5', unit='OY')
+INFO:uk-postcodes-parsing:Postcode Fixed: 'EH16 50Y' => 'EH16 5OY'
+Postcode(verified_against_postcode_io=False, fix_distance=1, original='EH16 50Y', postcode='EH16 5OY', incode='5OY', outcode='EH16', area='EH', district='EH16', sub_district=None, sector='EH16 5', unit='OY')
 ```
+
 ```python
 >>> ukpostcode.parse("EH16 50Y", attempt_fix=False) # Don't attempt fixes during parsing
 ERROR:uk-postcodes-parsing:Failed to parse postcode
 >>> ukpostcode.parse("0W1") 
 ERROR:uk-postcodes-parsing:Unable to fix postcode
 ERROR:uk-postcodes-parsing:Failed to parse postcode
 ```
@@ -106,14 +109,44 @@
 
 ```python
 >>> from uk_postcodes_parsing.fix import fix
 >>> fix("0W1 OAA") 
 'OW1 0AA'
 ```
 
+# Postcode class definition
+
+```python
+@dataclass(order=True)
+class Postcode:
+    # Calculate post initialization
+    verified_against_postcode_io: bool = field(init=False)
+    fix_distance: int = field(init=False)
+    # raw text
+    original: str 
+    # The rest of the fields are parsed from the postcode using regex
+    postcode: str
+    incode: str
+    outcode: str
+    area: str
+    district: str
+    sub_district: Union[str, None]
+    sector: str
+    unit: str
+
+```
+
+- 2 fileds calculated after init of class
+  - `verified_against_postcode_io`: Check against [`api.postcodes.io/postcodes/`](https://postcodes.io/) which uses the [ONS Postcode Directory](https://geoportal.statistics.gov.uk/datasets/489c152010a3425f80a71dc3663f73e1/about)
+  - `fix_distance`: A measure of number of characters changed from raw text via auto-fix to get a valid post code. 
+    - E.g. `SW1A OAA` => `SW1A 0AA` has fix_distance=1. Where as, `SWIA OAA` => `SW1A 0AA` has fix_distance=2.
+  - These fields are particularly helpful using `parse_from_corpus` with `attempt_fix=True` which might return many potential postcodes. These field can be used as proxy for confidence on which parsed postcodes are correct.
+- `raw_text`: To keep track of the original string without formatting changes and auto-fixes.
+- 8 fileds are parsed using regex
+
 # Testing
 
 ```bash
 pytest tests/
 ```
 
 ## Similar works
```

