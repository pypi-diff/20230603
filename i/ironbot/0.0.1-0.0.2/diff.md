# Comparing `tmp/ironbot-0.0.1.tar.gz` & `tmp/ironbot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ironbot-0.0.1.tar", max compression
+gzip compressed data, was "ironbot-0.0.2.tar", max compression
```

## Comparing `ironbot-0.0.1.tar` & `ironbot-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-06-01 22:19:22.270689 ironbot-0.0.1/LICENSE
--rw-r--r--   0        0        0     1801 2023-06-01 22:42:35.725271 ironbot-0.0.1/README.md
--rw-r--r--   0        0        0     2884 2023-06-01 22:19:22.271358 ironbot-0.0.1/ironbot/__init__.py
--rw-r--r--   0        0        0     1062 2023-06-01 22:42:28.225359 ironbot-0.0.1/ironbot/__main__.py
--rw-r--r--   0        0        0      628 2023-06-01 22:31:27.030384 ironbot-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2499 1970-01-01 00:00:00.000000 ironbot-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-01 22:19:22.270689 ironbot-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1823 2023-06-02 23:33:11.660579 ironbot-0.0.2/README.md
+-rw-r--r--   0        0        0     4016 2023-06-02 23:38:38.857517 ironbot-0.0.2/ironbot/__init__.py
+-rw-r--r--   0        0        0     1021 2023-06-02 23:30:58.279636 ironbot-0.0.2/ironbot/__main__.py
+-rw-r--r--   0        0        0     1131 2023-06-02 23:51:37.296030 ironbot-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3000 1970-01-01 00:00:00.000000 ironbot-0.0.2/PKG-INFO
```

### Comparing `ironbot-0.0.1/LICENSE` & `ironbot-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ironbot-0.0.1/README.md` & `ironbot-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # `ironbot`
 
 ## Requirements
 
- `ironbot` depends on Python 3.9 or newer, and on `pdftotext` which [requires `poppler`](https://github.com/jalan/pdftotext#os-dependencies).
+ `ironbot` depends on Python 3.9 or newer, and on [Camelot, which requires `ghostscript`](https://camelot-py.readthedocs.io/en/master/user/install-deps.html).
 
 ## Install
 
 ```console
 $ pip install ironbot
 ```
 
@@ -22,15 +22,15 @@
   --show-completion [bash|zsh|fish|powershell|pwsh]
                                   Show completion for the specified shell, to
                                   copy it or customize the installation.
   --help                          Show this message and exit.
 
 Commands:
   calendar     List the details of the upcoming Ironman professional races.
-  start-list   Gets the URL to the PDF containing the start list for an...
+  start-list   Gets the start list for an Ironman professional race (use...
   start-lists  List upcoming Ironman professional races with start list...
 ```
 
 ### Exemples
 
 #### Details of upcoming Ironman professional races
 
@@ -48,19 +48,22 @@
 $ ironbot start-lists
 Choose one of the followign events to use with `start-list` command:
  [1] 2023 IRONMAN European Championship Hamburg
  [2] 2023 IRONMAN 70.3 Boulder
  …
 ```
 
-#### Get the URL to the start list of an event
+#### Get the start list of an event
 
 ```console
 $ ironbot start-list 4
-https://files.constantcontact.com/a202847d001/81c60c53-85dd-45f9-b6aa-dd0fda086862.pdf
+1	Daniela Ryf	CHE (Switzerland)
+3	Ashleigh Gentle	AUS (Australia)
+4	Anne Reischmann	DEU (Germany)
+…
 ```
 
 ## Contributing
 
 Make sure that both checks pass:
 
 ```console
```

### Comparing `ironbot-0.0.1/PKG-INFO` & `ironbot-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 Metadata-Version: 2.1
 Name: ironbot
-Version: 0.0.1
+Version: 0.0.2
 Summary: CLI to get information about Ironman professional races
-License: GPL-3
+Home-page: https://github.com/cuducos/ironbot/
+License: GPLv3
+Keywords: triathlon,Ironamn,Professional triathletes,Professional triathlon races
 Author: Eduardo Cuducos
 Author-email: 4732915+cuducos@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Utilities
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
-Requires-Dist: httpx (>=0.24.1,<0.25.0)
-Requires-Dist: pdftotext (>=2.2.2,<3.0.0)
+Requires-Dist: camelot-py (>=0.11.0,<0.12.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
+Project-URL: Repository, https://github.com/cuducos/ironbot/
 Description-Content-Type: text/markdown
 
 # `ironbot`
 
 ## Requirements
 
- `ironbot` depends on Python 3.9 or newer, and on `pdftotext` which [requires `poppler`](https://github.com/jalan/pdftotext#os-dependencies).
+ `ironbot` depends on Python 3.9 or newer, and on [Camelot, which requires `ghostscript`](https://camelot-py.readthedocs.io/en/master/user/install-deps.html).
 
 ## Install
 
 ```console
 $ pip install ironbot
 ```
 
@@ -41,15 +50,15 @@
   --show-completion [bash|zsh|fish|powershell|pwsh]
                                   Show completion for the specified shell, to
                                   copy it or customize the installation.
   --help                          Show this message and exit.
 
 Commands:
   calendar     List the details of the upcoming Ironman professional races.
-  start-list   Gets the URL to the PDF containing the start list for an...
+  start-list   Gets the start list for an Ironman professional race (use...
   start-lists  List upcoming Ironman professional races with start list...
 ```
 
 ### Exemples
 
 #### Details of upcoming Ironman professional races
 
@@ -67,19 +76,22 @@
 $ ironbot start-lists
 Choose one of the followign events to use with `start-list` command:
  [1] 2023 IRONMAN European Championship Hamburg
  [2] 2023 IRONMAN 70.3 Boulder
  …
 ```
 
-#### Get the URL to the start list of an event
+#### Get the start list of an event
 
 ```console
 $ ironbot start-list 4
-https://files.constantcontact.com/a202847d001/81c60c53-85dd-45f9-b6aa-dd0fda086862.pdf
+1	Daniela Ryf	CHE (Switzerland)
+3	Ashleigh Gentle	AUS (Australia)
+4	Anne Reischmann	DEU (Germany)
+…
 ```
 
 ## Contributing
 
 Make sure that both checks pass:
 
 ```console
```

