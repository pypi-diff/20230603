# Comparing `tmp/pyverse-1.0.0.tar.gz` & `tmp/pyverse-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyverse-1.0.0.tar", last modified: Thu Jan  7 09:07:16 2021, max compression
+gzip compressed data, was "pyverse-1.1.0.tar", last modified: Sat Jun  3 16:13:46 2023, max compression
```

## Comparing `pyverse-1.0.0.tar` & `pyverse-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxrwxr-x   0 nebur     (1000) nebur     (1000)        0 2021-01-07 09:07:16.865830 pyverse-1.0.0/
--rw-rw-r--   0 nebur     (1000) nebur     (1000)     5663 2021-01-07 09:07:16.865830 pyverse-1.0.0/PKG-INFO
--rw-rw-r--   0 nebur     (1000) nebur     (1000)     4320 2021-01-07 00:56:02.000000 pyverse-1.0.0/README.md
-drwxrwxr-x   0 nebur     (1000) nebur     (1000)        0 2021-01-07 09:07:16.861830 pyverse-1.0.0/pyverse/
--rw-rw-r--   0 nebur     (1000) nebur     (1000)       32 2021-01-07 00:55:26.000000 pyverse-1.0.0/pyverse/__init__.py
--rw-rw-r--   0 nebur     (1000) nebur     (1000)     1032 2021-01-07 00:55:26.000000 pyverse-1.0.0/pyverse/__main__.py
--rw-rw-r--   0 nebur     (1000) nebur     (1000)    16656 2021-01-07 00:55:26.000000 pyverse-1.0.0/pyverse/silabeador.py
--rw-rw-r--   0 nebur     (1000) nebur     (1000)     1746 2021-01-06 23:09:18.000000 pyverse-1.0.0/pyverse/vars.py
-drwxrwxr-x   0 nebur     (1000) nebur     (1000)        0 2021-01-07 09:07:16.865830 pyverse-1.0.0/pyverse.egg-info/
--rw-rw-r--   0 nebur     (1000) nebur     (1000)     5663 2021-01-07 09:07:16.000000 pyverse-1.0.0/pyverse.egg-info/PKG-INFO
--rw-rw-r--   0 nebur     (1000) nebur     (1000)      284 2021-01-07 09:07:16.000000 pyverse-1.0.0/pyverse.egg-info/SOURCES.txt
--rw-rw-r--   0 nebur     (1000) nebur     (1000)        1 2021-01-07 09:07:16.000000 pyverse-1.0.0/pyverse.egg-info/dependency_links.txt
--rw-rw-r--   0 nebur     (1000) nebur     (1000)       55 2021-01-07 09:07:16.000000 pyverse-1.0.0/pyverse.egg-info/entry_points.txt
--rw-rw-r--   0 nebur     (1000) nebur     (1000)       20 2021-01-07 09:07:16.000000 pyverse-1.0.0/pyverse.egg-info/requires.txt
--rw-rw-r--   0 nebur     (1000) nebur     (1000)        8 2021-01-07 09:07:16.000000 pyverse-1.0.0/pyverse.egg-info/top_level.txt
--rw-rw-r--   0 nebur     (1000) nebur     (1000)       38 2021-01-07 09:07:16.865830 pyverse-1.0.0/setup.cfg
--rw-rw-r--   0 nebur     (1000) nebur     (1000)      878 2021-01-07 00:55:26.000000 pyverse-1.0.0/setup.py
+drwxr-xr-x   0 rubenkarlsson   (501) staff       (20)        0 2023-06-03 16:13:46.182005 pyverse-1.1.0/
+-rw-r--r--   0 rubenkarlsson   (501) staff       (20)     1071 2023-06-03 11:20:38.000000 pyverse-1.1.0/LICENSE
+-rw-r--r--   0 rubenkarlsson   (501) staff       (20)     4723 2023-06-03 16:13:46.181743 pyverse-1.1.0/PKG-INFO
+-rw-r--r--   0 rubenkarlsson   (501) staff       (20)     4253 2023-06-03 11:20:38.000000 pyverse-1.1.0/README.md
+drwxr-xr-x   0 rubenkarlsson   (501) staff       (20)        0 2023-06-03 16:13:46.177325 pyverse-1.1.0/pyverse/
+-rw-r--r--   0 rubenkarlsson   (501) staff       (20)       32 2023-06-03 14:24:50.000000 pyverse-1.1.0/pyverse/__init__.py
+-rw-r--r--   0 rubenkarlsson   (501) staff       (20)     1032 2023-06-03 11:20:38.000000 pyverse-1.1.0/pyverse/__main__.py
+-rw-r--r--   0 rubenkarlsson   (501) staff       (20)     3082 2023-06-03 14:16:15.000000 pyverse-1.1.0/pyverse/sentence.py
+-rw-r--r--   0 rubenkarlsson   (501) staff       (20)     3844 2023-06-03 16:02:26.000000 pyverse-1.1.0/pyverse/silabeador.py
+-rw-r--r--   0 rubenkarlsson   (501) staff       (20)     1746 2023-06-03 11:20:38.000000 pyverse-1.1.0/pyverse/vars.py
+-rw-r--r--   0 rubenkarlsson   (501) staff       (20)    11151 2023-06-03 16:02:17.000000 pyverse-1.1.0/pyverse/word.py
+drwxr-xr-x   0 rubenkarlsson   (501) staff       (20)        0 2023-06-03 16:13:46.180906 pyverse-1.1.0/pyverse.egg-info/
+-rw-r--r--   0 rubenkarlsson   (501) staff       (20)     4723 2023-06-03 16:13:45.000000 pyverse-1.1.0/pyverse.egg-info/PKG-INFO
+-rw-r--r--   0 rubenkarlsson   (501) staff       (20)      353 2023-06-03 16:13:45.000000 pyverse-1.1.0/pyverse.egg-info/SOURCES.txt
+-rw-r--r--   0 rubenkarlsson   (501) staff       (20)        1 2023-06-03 16:13:45.000000 pyverse-1.1.0/pyverse.egg-info/dependency_links.txt
+-rw-r--r--   0 rubenkarlsson   (501) staff       (20)       54 2023-06-03 16:13:45.000000 pyverse-1.1.0/pyverse.egg-info/entry_points.txt
+-rw-r--r--   0 rubenkarlsson   (501) staff       (20)       20 2023-06-03 16:13:45.000000 pyverse-1.1.0/pyverse.egg-info/requires.txt
+-rw-r--r--   0 rubenkarlsson   (501) staff       (20)        8 2023-06-03 16:13:45.000000 pyverse-1.1.0/pyverse.egg-info/top_level.txt
+-rw-r--r--   0 rubenkarlsson   (501) staff       (20)       38 2023-06-03 16:13:46.182083 pyverse-1.1.0/setup.cfg
+-rw-r--r--   0 rubenkarlsson   (501) staff       (20)      878 2023-06-03 16:06:19.000000 pyverse-1.1.0/setup.py
+drwxr-xr-x   0 rubenkarlsson   (501) staff       (20)        0 2023-06-03 16:13:46.181259 pyverse-1.1.0/tests/
+-rw-r--r--   0 rubenkarlsson   (501) staff       (20)    16316 2023-06-03 16:05:26.000000 pyverse-1.1.0/tests/test_silabeador.py
```

### Comparing `pyverse-1.0.0/PKG-INFO` & `pyverse-1.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,123 +1,122 @@
 Metadata-Version: 2.1
 Name: pyverse
-Version: 1.0.0
+Version: 1.1.0
 Summary: find syllables and rhymes of words/verses in spanish
 Home-page: https://github.com/neburnodrog/Pyverso
 Author: Ruben Karlsson
 Author-email: neburnodrog@gmail.com
 License: MIT
-Description: [![codecov](https://img.shields.io/codecov/c/github/neburnodrog/silabizador)](https://codecov.io/gh/neburnodrog/silabizador)
-        
-        # Pyverse
-        #### A automatic syllabification algorithm for Spanish verses written in Python
-        
-        <<<<<<< HEAD
-        Pyverse comes from Python & Verso.
-        Verso beeing verse in Spanish.
-        
-        =======
-        >>>>>>> b6c26b835e85222557c8cfc4777db1b55a37d8fb
-        - It separates every syllable of words and verses. It counts the syllables of verses as it's done in the spanish language poetry tradition.
-        
-        ### Description
-          **silabizador** syllabifies words and verses taking into account [synalephas](https://en.wikipedia.org/wiki/Synalepha) and the [accentuation](https://en.wikipedia.org/wiki/Metre_(poetry)#Spanish) of the final word in the verse. 
-        
-          - The [prosodic](https://en.wikipedia.org/wiki/Prosody_(linguistics)) metre of a verse in Spanish poetry differs from the rules of syllabification specified by the [RAE](https://en.wikipedia.org/wiki/Royal_Spanish_Academy) for the counting of syllables. Depending on the accentuation of the last word of the verse we encounter different cases:
-        
-            1. If the last word is [oxytone](https://en.wikipedia.org/wiki/Oxytone), the prosodic perception will impose the addition of an extra syllable to the syllable count of the verse.
-            2. If it's [paroxytone](https://en.wikipedia.org/wiki/Paroxytone) we leave as it is: we neither add nor substract a syllable to the counting.
-            3. If it's [proparoxytone](https://en.wikipedia.org/wiki/Proparoxytone) we substract one syllable.
-            4. If it's **superproparoxytone** we substract two.  
-        
-        ### Instalation
-        ```
-        pip install pyverse
-        ```
-        ### Use
-        You can either use Pyverse in the command line:
-        ```
-        pyverso "un velero bergantín;"
-        
-                Syllabified Text | -un -ve-le-ro -ber-ga-tín;
-                Count            | 8
-                Consonant Rhyme  | atin
-                Assonant Rhyme   | ai
-        ```
-        or as a python package
-        ```
-        >>> from pyverse import Pyverse
-        >>> verse = Pyverse("un velero bergantín;")
-        >>> print(verse.get_syllables())
-        '-un -ve-le-ro -ber-gan-tín;'
-        >>> print(verse.count)
-        8
-        ```
-        ---
-        
-        # Pyverse en Español
-        #### Un algoritmo silabeador de versos en español escrito en Python.
-        ```
-        [silabear](https://dle.rae.es/silabear)
-        1. Ir pronunciando separadamente cada sílaba.
-        ```
-        
-        ### Descripcion
-        Pyverse silabea palabras y versos en Español. Cuenta las sílabas a la manera de la tradición poética en lengua española. 
-        Es decir: tiene en cuenta sinalefas y finales de verso. 
-        
-        - Según la [acentuación fonética](https://es.wikipedia.org/wiki/Acentuaci%C3%B3n_del_idioma_espa%C3%B1ol#Reglas_generales_de_acentuaci%C3%B3n) de la última palabra del verso se dan varios casos:
-        
-          1. Si la última palabra tiene una acetuación **aguda** u **oxítona**, la perceptión prosódica del verso impone que se le sume una sílaba al número de sílabas ortográficas del verso.  
-          2. Si es **llana** o **paroxítona** se deja como está: ni se le resta ni se le suman sílabas al verso.
-          3. Si la última palabra del verso es **esdrújula** o *proparoxítona* se le resta una sílaba al verso.
-          4. Si es **superproparoxítona** o **sobresdrújula** se le restan dos sílabas al verso.
-          
-        - [Sinalefas](https://es.wikipedia.org/wiki/Sinalefa)
-        
-          - La sinalefa es un fenómeno prosódico mediante el cual se juntan en una sola sílaba fonética la última sílaba de una palabra y la primera de la siguiente en caso de ser las dos vocales.
-          
-            ```
-            -el -ar-ma_an-ti-gua
-            -el -vien-to_a-zul
-            ```
-          - No se produce sinalefa si la segunda palabra empieza con vocal acentuada:
-          
-            ```
-            -el -ar-la -á-ri-da
-            -el -vien-to -ár-ti-co
-            ```
-        - Rimas
-        
-          - El silabizador proporciona las rimas [asonante](https://es.wikipedia.org/wiki/Rima_asonante) y [consonantes](https://es.wikipedia.org/wiki/Rima_consonante) tanto de palabras como de versos
-        
-        ### Instalación
-        ```
-        pip install Pyverse
-        ```
-        
-        ### Uso
-        puedes usar Pyverse desde el terminal:
-        ```
-        pyverso "un velero bergantín;"
-        
-                Syllabified Text | -un -ve-le-ro -ber-ga-tín;
-                Count            | 8
-                Consonant Rhyme  | atin
-                Assonant Rhyme   | ai
-        ```
-        o como una librería de Python
-        ```
-        >>> from pyverse import Pyverse
-        >>> verse = Pyverse("un velero bergantín;")
-        >>> print(verse.get_syllables())
-        '-un -ve-le-ro -ber-gan-tín;'
-        >>> print(verse.count)
-        8
-        ```
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![codecov](https://img.shields.io/codecov/c/github/neburnodrog/silabizador)](https://codecov.io/gh/neburnodrog/silabizador)
+
+# Pyverse
+#### A automatic syllabification algorithm for Spanish verses written in Python
+
+Pyverse comes from Python & Verso.
+Verso beeing verse in Spanish.
+
+=======
+
+- It separates every syllable of words and verses. It counts the syllables of verses as it's done in the spanish language poetry tradition.
+
+### Description
+  **silabizador** syllabifies words and verses taking into account [synalephas](https://en.wikipedia.org/wiki/Synalepha) and the [accentuation](https://en.wikipedia.org/wiki/Metre_(poetry)#Spanish) of the final word in the verse. 
+
+  - The [prosodic](https://en.wikipedia.org/wiki/Prosody_(linguistics)) metre of a verse in Spanish poetry differs from the rules of syllabification specified by the [RAE](https://en.wikipedia.org/wiki/Royal_Spanish_Academy) for the counting of syllables. Depending on the accentuation of the last word of the verse we encounter different cases:
+
+    1. If the last word is [oxytone](https://en.wikipedia.org/wiki/Oxytone), the prosodic perception will impose the addition of an extra syllable to the syllable count of the verse.
+    2. If it's [paroxytone](https://en.wikipedia.org/wiki/Paroxytone) we leave as it is: we neither add nor substract a syllable to the counting.
+    3. If it's [proparoxytone](https://en.wikipedia.org/wiki/Proparoxytone) we substract one syllable.
+    4. If it's **superproparoxytone** we substract two.  
+
+### Instalation
+```
+pip install pyverse
+```
+### Use
+You can either use Pyverse in the command line:
+```
+pyverso "un velero bergantín;"
+
+        Syllabified Text | -un -ve-le-ro -ber-ga-tín;
+        Count            | 8
+        Consonant Rhyme  | atin
+        Assonant Rhyme   | ai
+```
+or as a python package
+```
+>>> from pyverse import Pyverse
+>>> verse = Pyverse("un velero bergantín;")
+>>> print(verse.get_syllables())
+'-un -ve-le-ro -ber-gan-tín;'
+>>> print(verse.count)
+8
+```
+---
+
+# Pyverse en Español
+#### Un algoritmo silabeador de versos en español escrito en Python.
+```
+[silabear](https://dle.rae.es/silabear)
+1. Ir pronunciando separadamente cada sílaba.
+```
+
+### Descripcion
+Pyverse silabea palabras y versos en Español. Cuenta las sílabas a la manera de la tradición poética en lengua española. 
+Es decir: tiene en cuenta sinalefas y finales de verso. 
+
+- Según la [acentuación fonética](https://es.wikipedia.org/wiki/Acentuaci%C3%B3n_del_idioma_espa%C3%B1ol#Reglas_generales_de_acentuaci%C3%B3n) de la última palabra del verso se dan varios casos:
+
+  1. Si la última palabra tiene una acetuación **aguda** u **oxítona**, la perceptión prosódica del verso impone que se le sume una sílaba al número de sílabas ortográficas del verso.  
+  2. Si es **llana** o **paroxítona** se deja como está: ni se le resta ni se le suman sílabas al verso.
+  3. Si la última palabra del verso es **esdrújula** o *proparoxítona* se le resta una sílaba al verso.
+  4. Si es **superproparoxítona** o **sobresdrújula** se le restan dos sílabas al verso.
+  
+- [Sinalefas](https://es.wikipedia.org/wiki/Sinalefa)
+
+  - La sinalefa es un fenómeno prosódico mediante el cual se juntan en una sola sílaba fonética la última sílaba de una palabra y la primera de la siguiente en caso de ser las dos vocales.
+  
+    ```
+    -el -ar-ma_an-ti-gua
+    -el -vien-to_a-zul
+    ```
+  - No se produce sinalefa si la segunda palabra empieza con vocal acentuada:
+  
+    ```
+    -el -ar-la -á-ri-da
+    -el -vien-to -ár-ti-co
+    ```
+- Rimas
+
+  - El silabizador proporciona las rimas [asonante](https://es.wikipedia.org/wiki/Rima_asonante) y [consonantes](https://es.wikipedia.org/wiki/Rima_consonante) tanto de palabras como de versos
+
+### Instalación
+```
+pip install Pyverse
+```
+
+### Uso
+puedes usar Pyverse desde el terminal:
+```
+$ pyverse "un velero bergantín;"
+
+        Syllabified Text | -un -ve-le-ro -ber-ga-tín;
+        Count            | 8
+        Consonant Rhyme  | atin
+        Assonant Rhyme   | ai
+```
+o como una librería de Python
+```
+from pyverse import Pyverse
+verse = Pyverse("un velero bergantín;")
+print(verse.get_syllables())
+>>> '-un -ve-le-ro -ber-gan-tín;'
+print(verse.count)
+>>> 8
+```
```

### Comparing `pyverse-1.0.0/README.md` & `pyverse-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [![codecov](https://img.shields.io/codecov/c/github/neburnodrog/silabizador)](https://codecov.io/gh/neburnodrog/silabizador)
 
 # Pyverse
 #### A automatic syllabification algorithm for Spanish verses written in Python
 
-<<<<<<< HEAD
 Pyverse comes from Python & Verso.
 Verso beeing verse in Spanish.
 
 =======
->>>>>>> b6c26b835e85222557c8cfc4777db1b55a37d8fb
+
 - It separates every syllable of words and verses. It counts the syllables of verses as it's done in the spanish language poetry tradition.
 
 ### Description
   **silabizador** syllabifies words and verses taking into account [synalephas](https://en.wikipedia.org/wiki/Synalepha) and the [accentuation](https://en.wikipedia.org/wiki/Metre_(poetry)#Spanish) of the final word in the verse. 
 
   - The [prosodic](https://en.wikipedia.org/wiki/Prosody_(linguistics)) metre of a verse in Spanish poetry differs from the rules of syllabification specified by the [RAE](https://en.wikipedia.org/wiki/Royal_Spanish_Academy) for the counting of syllables. Depending on the accentuation of the last word of the verse we encounter different cases:
 
@@ -86,23 +85,23 @@
 ```
 pip install Pyverse
 ```
 
 ### Uso
 puedes usar Pyverse desde el terminal:
 ```
-pyverso "un velero bergantín;"
+$ pyverse "un velero bergantín;"
 
         Syllabified Text | -un -ve-le-ro -ber-ga-tín;
         Count            | 8
         Consonant Rhyme  | atin
         Assonant Rhyme   | ai
 ```
 o como una librería de Python
 ```
->>> from pyverse import Pyverse
->>> verse = Pyverse("un velero bergantín;")
->>> print(verse.get_syllables())
-'-un -ve-le-ro -ber-gan-tín;'
->>> print(verse.count)
-8
+from pyverse import Pyverse
+verse = Pyverse("un velero bergantín;")
+print(verse.get_syllables())
+>>> '-un -ve-le-ro -ber-gan-tín;'
+print(verse.count)
+>>> 8
 ```
```

### Comparing `pyverse-1.0.0/pyverse/__main__.py` & `pyverse-1.1.0/pyverse/__main__.py`

 * *Files identical despite different names*

### Comparing `pyverse-1.0.0/pyverse/vars.py` & `pyverse-1.1.0/pyverse/vars.py`

 * *Files identical despite different names*

### Comparing `pyverse-1.0.0/pyverse.egg-info/PKG-INFO` & `pyverse-1.1.0/pyverse.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,123 +1,122 @@
 Metadata-Version: 2.1
 Name: pyverse
-Version: 1.0.0
+Version: 1.1.0
 Summary: find syllables and rhymes of words/verses in spanish
 Home-page: https://github.com/neburnodrog/Pyverso
 Author: Ruben Karlsson
 Author-email: neburnodrog@gmail.com
 License: MIT
-Description: [![codecov](https://img.shields.io/codecov/c/github/neburnodrog/silabizador)](https://codecov.io/gh/neburnodrog/silabizador)
-        
-        # Pyverse
-        #### A automatic syllabification algorithm for Spanish verses written in Python
-        
-        <<<<<<< HEAD
-        Pyverse comes from Python & Verso.
-        Verso beeing verse in Spanish.
-        
-        =======
-        >>>>>>> b6c26b835e85222557c8cfc4777db1b55a37d8fb
-        - It separates every syllable of words and verses. It counts the syllables of verses as it's done in the spanish language poetry tradition.
-        
-        ### Description
-          **silabizador** syllabifies words and verses taking into account [synalephas](https://en.wikipedia.org/wiki/Synalepha) and the [accentuation](https://en.wikipedia.org/wiki/Metre_(poetry)#Spanish) of the final word in the verse. 
-        
-          - The [prosodic](https://en.wikipedia.org/wiki/Prosody_(linguistics)) metre of a verse in Spanish poetry differs from the rules of syllabification specified by the [RAE](https://en.wikipedia.org/wiki/Royal_Spanish_Academy) for the counting of syllables. Depending on the accentuation of the last word of the verse we encounter different cases:
-        
-            1. If the last word is [oxytone](https://en.wikipedia.org/wiki/Oxytone), the prosodic perception will impose the addition of an extra syllable to the syllable count of the verse.
-            2. If it's [paroxytone](https://en.wikipedia.org/wiki/Paroxytone) we leave as it is: we neither add nor substract a syllable to the counting.
-            3. If it's [proparoxytone](https://en.wikipedia.org/wiki/Proparoxytone) we substract one syllable.
-            4. If it's **superproparoxytone** we substract two.  
-        
-        ### Instalation
-        ```
-        pip install pyverse
-        ```
-        ### Use
-        You can either use Pyverse in the command line:
-        ```
-        pyverso "un velero bergantín;"
-        
-                Syllabified Text | -un -ve-le-ro -ber-ga-tín;
-                Count            | 8
-                Consonant Rhyme  | atin
-                Assonant Rhyme   | ai
-        ```
-        or as a python package
-        ```
-        >>> from pyverse import Pyverse
-        >>> verse = Pyverse("un velero bergantín;")
-        >>> print(verse.get_syllables())
-        '-un -ve-le-ro -ber-gan-tín;'
-        >>> print(verse.count)
-        8
-        ```
-        ---
-        
-        # Pyverse en Español
-        #### Un algoritmo silabeador de versos en español escrito en Python.
-        ```
-        [silabear](https://dle.rae.es/silabear)
-        1. Ir pronunciando separadamente cada sílaba.
-        ```
-        
-        ### Descripcion
-        Pyverse silabea palabras y versos en Español. Cuenta las sílabas a la manera de la tradición poética en lengua española. 
-        Es decir: tiene en cuenta sinalefas y finales de verso. 
-        
-        - Según la [acentuación fonética](https://es.wikipedia.org/wiki/Acentuaci%C3%B3n_del_idioma_espa%C3%B1ol#Reglas_generales_de_acentuaci%C3%B3n) de la última palabra del verso se dan varios casos:
-        
-          1. Si la última palabra tiene una acetuación **aguda** u **oxítona**, la perceptión prosódica del verso impone que se le sume una sílaba al número de sílabas ortográficas del verso.  
-          2. Si es **llana** o **paroxítona** se deja como está: ni se le resta ni se le suman sílabas al verso.
-          3. Si la última palabra del verso es **esdrújula** o *proparoxítona* se le resta una sílaba al verso.
-          4. Si es **superproparoxítona** o **sobresdrújula** se le restan dos sílabas al verso.
-          
-        - [Sinalefas](https://es.wikipedia.org/wiki/Sinalefa)
-        
-          - La sinalefa es un fenómeno prosódico mediante el cual se juntan en una sola sílaba fonética la última sílaba de una palabra y la primera de la siguiente en caso de ser las dos vocales.
-          
-            ```
-            -el -ar-ma_an-ti-gua
-            -el -vien-to_a-zul
-            ```
-          - No se produce sinalefa si la segunda palabra empieza con vocal acentuada:
-          
-            ```
-            -el -ar-la -á-ri-da
-            -el -vien-to -ár-ti-co
-            ```
-        - Rimas
-        
-          - El silabizador proporciona las rimas [asonante](https://es.wikipedia.org/wiki/Rima_asonante) y [consonantes](https://es.wikipedia.org/wiki/Rima_consonante) tanto de palabras como de versos
-        
-        ### Instalación
-        ```
-        pip install Pyverse
-        ```
-        
-        ### Uso
-        puedes usar Pyverse desde el terminal:
-        ```
-        pyverso "un velero bergantín;"
-        
-                Syllabified Text | -un -ve-le-ro -ber-ga-tín;
-                Count            | 8
-                Consonant Rhyme  | atin
-                Assonant Rhyme   | ai
-        ```
-        o como una librería de Python
-        ```
-        >>> from pyverse import Pyverse
-        >>> verse = Pyverse("un velero bergantín;")
-        >>> print(verse.get_syllables())
-        '-un -ve-le-ro -ber-gan-tín;'
-        >>> print(verse.count)
-        8
-        ```
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![codecov](https://img.shields.io/codecov/c/github/neburnodrog/silabizador)](https://codecov.io/gh/neburnodrog/silabizador)
+
+# Pyverse
+#### A automatic syllabification algorithm for Spanish verses written in Python
+
+Pyverse comes from Python & Verso.
+Verso beeing verse in Spanish.
+
+=======
+
+- It separates every syllable of words and verses. It counts the syllables of verses as it's done in the spanish language poetry tradition.
+
+### Description
+  **silabizador** syllabifies words and verses taking into account [synalephas](https://en.wikipedia.org/wiki/Synalepha) and the [accentuation](https://en.wikipedia.org/wiki/Metre_(poetry)#Spanish) of the final word in the verse. 
+
+  - The [prosodic](https://en.wikipedia.org/wiki/Prosody_(linguistics)) metre of a verse in Spanish poetry differs from the rules of syllabification specified by the [RAE](https://en.wikipedia.org/wiki/Royal_Spanish_Academy) for the counting of syllables. Depending on the accentuation of the last word of the verse we encounter different cases:
+
+    1. If the last word is [oxytone](https://en.wikipedia.org/wiki/Oxytone), the prosodic perception will impose the addition of an extra syllable to the syllable count of the verse.
+    2. If it's [paroxytone](https://en.wikipedia.org/wiki/Paroxytone) we leave as it is: we neither add nor substract a syllable to the counting.
+    3. If it's [proparoxytone](https://en.wikipedia.org/wiki/Proparoxytone) we substract one syllable.
+    4. If it's **superproparoxytone** we substract two.  
+
+### Instalation
+```
+pip install pyverse
+```
+### Use
+You can either use Pyverse in the command line:
+```
+pyverso "un velero bergantín;"
+
+        Syllabified Text | -un -ve-le-ro -ber-ga-tín;
+        Count            | 8
+        Consonant Rhyme  | atin
+        Assonant Rhyme   | ai
+```
+or as a python package
+```
+>>> from pyverse import Pyverse
+>>> verse = Pyverse("un velero bergantín;")
+>>> print(verse.get_syllables())
+'-un -ve-le-ro -ber-gan-tín;'
+>>> print(verse.count)
+8
+```
+---
+
+# Pyverse en Español
+#### Un algoritmo silabeador de versos en español escrito en Python.
+```
+[silabear](https://dle.rae.es/silabear)
+1. Ir pronunciando separadamente cada sílaba.
+```
+
+### Descripcion
+Pyverse silabea palabras y versos en Español. Cuenta las sílabas a la manera de la tradición poética en lengua española. 
+Es decir: tiene en cuenta sinalefas y finales de verso. 
+
+- Según la [acentuación fonética](https://es.wikipedia.org/wiki/Acentuaci%C3%B3n_del_idioma_espa%C3%B1ol#Reglas_generales_de_acentuaci%C3%B3n) de la última palabra del verso se dan varios casos:
+
+  1. Si la última palabra tiene una acetuación **aguda** u **oxítona**, la perceptión prosódica del verso impone que se le sume una sílaba al número de sílabas ortográficas del verso.  
+  2. Si es **llana** o **paroxítona** se deja como está: ni se le resta ni se le suman sílabas al verso.
+  3. Si la última palabra del verso es **esdrújula** o *proparoxítona* se le resta una sílaba al verso.
+  4. Si es **superproparoxítona** o **sobresdrújula** se le restan dos sílabas al verso.
+  
+- [Sinalefas](https://es.wikipedia.org/wiki/Sinalefa)
+
+  - La sinalefa es un fenómeno prosódico mediante el cual se juntan en una sola sílaba fonética la última sílaba de una palabra y la primera de la siguiente en caso de ser las dos vocales.
+  
+    ```
+    -el -ar-ma_an-ti-gua
+    -el -vien-to_a-zul
+    ```
+  - No se produce sinalefa si la segunda palabra empieza con vocal acentuada:
+  
+    ```
+    -el -ar-la -á-ri-da
+    -el -vien-to -ár-ti-co
+    ```
+- Rimas
+
+  - El silabizador proporciona las rimas [asonante](https://es.wikipedia.org/wiki/Rima_asonante) y [consonantes](https://es.wikipedia.org/wiki/Rima_consonante) tanto de palabras como de versos
+
+### Instalación
+```
+pip install Pyverse
+```
+
+### Uso
+puedes usar Pyverse desde el terminal:
+```
+$ pyverse "un velero bergantín;"
+
+        Syllabified Text | -un -ve-le-ro -ber-ga-tín;
+        Count            | 8
+        Consonant Rhyme  | atin
+        Assonant Rhyme   | ai
+```
+o como una librería de Python
+```
+from pyverse import Pyverse
+verse = Pyverse("un velero bergantín;")
+print(verse.get_syllables())
+>>> '-un -ve-le-ro -ber-gan-tín;'
+print(verse.count)
+>>> 8
+```
```

### Comparing `pyverse-1.0.0/setup.py` & `pyverse-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 setup(
     name="pyverse",
-    version="1.0.0",
+    version="1.1.0",
     description="find syllables and rhymes of words/verses in spanish",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/neburnodrog/Pyverso",
     author="Ruben Karlsson",
     author_email="neburnodrog@gmail.com",
     license="MIT",
```

