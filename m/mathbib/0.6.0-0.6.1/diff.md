# Comparing `tmp/mathbib-0.6.0.tar.gz` & `tmp/mathbib-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathbib-0.6.0.tar", max compression
+gzip compressed data, was "mathbib-0.6.1.tar", max compression
```

## Comparing `mathbib-0.6.0.tar` & `mathbib-0.6.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.6.0/LICENSE
--rw-r--r--   0        0        0     5351 2023-05-29 16:41:55.640378 mathbib-0.6.0/README.md
--rw-r--r--   0        0        0      143 2023-05-29 16:27:47.709639 mathbib-0.6.0/mathbib/__init__.py
--rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.6.0/mathbib/__main__.py
--rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.6.0/mathbib/bibtex.py
--rw-r--r--   0        0        0     2831 2023-05-28 15:54:03.882001 mathbib-0.6.0/mathbib/citegen.py
--rw-r--r--   0        0        0    10051 2023-05-30 19:06:35.770568 mathbib-0.6.0/mathbib/command.py
--rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.6.0/mathbib/partition.py
--rw-r--r--   0        0        0     9459 2023-05-28 15:11:22.084659 mathbib-0.6.0/mathbib/record.py
--rw-r--r--   0        0        0     5481 2023-05-28 13:40:33.677396 mathbib-0.6.0/mathbib/remote/__init__.py
--rw-r--r--   0        0        0     3088 2023-05-28 12:38:27.635690 mathbib-0.6.0/mathbib/remote/arxiv.py
--rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.6.0/mathbib/remote/doi.py
--rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.6.0/mathbib/remote/error.py
--rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.6.0/mathbib/remote/isbn.py
--rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.6.0/mathbib/remote/ol.py
--rw-r--r--   0        0        0     4257 2023-05-28 15:10:12.248626 mathbib-0.6.0/mathbib/remote/utils.py
--rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.6.0/mathbib/remote/zbl.py
--rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.6.0/mathbib/remote/zbmath.py
--rw-r--r--   0        0        0     5512 2023-05-29 16:27:20.815594 mathbib-0.6.0/mathbib/request.py
--rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.6.0/mathbib/resources/__init__.py
--rw-r--r--   0        0        0   270234 2023-05-30 19:21:30.067741 mathbib-0.6.0/mathbib/resources/journal_abbrevs.json
--rw-r--r--   0        0        0     2785 2023-05-30 19:29:22.770722 mathbib-0.6.0/mathbib/session.py
--rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.6.0/mathbib/term.py
--rw-r--r--   0        0        0      917 2023-05-30 19:28:57.582115 mathbib-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     6240 1970-01-01 00:00:00.000000 mathbib-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.6.1/LICENSE
+-rw-r--r--   0        0        0     5351 2023-05-29 16:41:55.640378 mathbib-0.6.1/README.md
+-rw-r--r--   0        0        0      143 2023-05-29 16:27:47.709639 mathbib-0.6.1/mathbib/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.6.1/mathbib/__main__.py
+-rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.6.1/mathbib/bibtex.py
+-rw-r--r--   0        0        0     2831 2023-05-28 15:54:03.882001 mathbib-0.6.1/mathbib/citegen.py
+-rw-r--r--   0        0        0    10051 2023-05-30 19:06:35.770568 mathbib-0.6.1/mathbib/command.py
+-rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.6.1/mathbib/partition.py
+-rw-r--r--   0        0        0     9518 2023-06-03 19:53:05.633854 mathbib-0.6.1/mathbib/record.py
+-rw-r--r--   0        0        0     5481 2023-05-28 13:40:33.677396 mathbib-0.6.1/mathbib/remote/__init__.py
+-rw-r--r--   0        0        0     3088 2023-05-28 12:38:27.635690 mathbib-0.6.1/mathbib/remote/arxiv.py
+-rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.6.1/mathbib/remote/doi.py
+-rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.6.1/mathbib/remote/error.py
+-rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.6.1/mathbib/remote/isbn.py
+-rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.6.1/mathbib/remote/ol.py
+-rw-r--r--   0        0        0     4257 2023-05-28 15:10:12.248626 mathbib-0.6.1/mathbib/remote/utils.py
+-rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.6.1/mathbib/remote/zbl.py
+-rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.6.1/mathbib/remote/zbmath.py
+-rw-r--r--   0        0        0     5604 2023-06-03 19:50:07.002465 mathbib-0.6.1/mathbib/request.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.6.1/mathbib/resources/__init__.py
+-rw-r--r--   0        0        0   270281 2023-05-30 19:36:41.814752 mathbib-0.6.1/mathbib/resources/journal_abbrevs.json
+-rw-r--r--   0        0        0     2785 2023-05-30 19:29:22.770722 mathbib-0.6.1/mathbib/session.py
+-rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.6.1/mathbib/term.py
+-rw-r--r--   0        0        0      917 2023-06-03 19:54:27.525920 mathbib-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6240 1970-01-01 00:00:00.000000 mathbib-0.6.1/PKG-INFO
```

### Comparing `mathbib-0.6.0/LICENSE` & `mathbib-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.0/README.md` & `mathbib-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.0/mathbib/bibtex.py` & `mathbib-0.6.1/mathbib/bibtex.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.0/mathbib/citegen.py` & `mathbib-0.6.1/mathbib/citegen.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.0/mathbib/command.py` & `mathbib-0.6.1/mathbib/command.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.0/mathbib/partition.py` & `mathbib-0.6.1/mathbib/partition.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.0/mathbib/record.py` & `mathbib-0.6.1/mathbib/record.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,14 +270,15 @@
                 return keyid.file_path()
         return None
 
     def download_file(self) -> Optional[Path]:
         for keyid in self.related_keys():
             download_url = get_remote_record(keyid).download_url
             path = keyid.file_path()
+            path.parent.mkdir(exist_ok=True, parents=True)
             if (
                 download_url is not None
                 and self.cli_session.remote_session.make_raw_streaming_request(
                     download_url(keyid.identifier), path
                 )
             ):
                 return path
```

### Comparing `mathbib-0.6.0/mathbib/remote/__init__.py` & `mathbib-0.6.1/mathbib/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.0/mathbib/remote/arxiv.py` & `mathbib-0.6.1/mathbib/remote/arxiv.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.0/mathbib/remote/doi.py` & `mathbib-0.6.1/mathbib/remote/doi.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.0/mathbib/remote/error.py` & `mathbib-0.6.1/mathbib/remote/error.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.0/mathbib/remote/isbn.py` & `mathbib-0.6.1/mathbib/remote/isbn.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.0/mathbib/remote/ol.py` & `mathbib-0.6.1/mathbib/remote/ol.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.0/mathbib/remote/utils.py` & `mathbib-0.6.1/mathbib/remote/utils.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.0/mathbib/remote/zbl.py` & `mathbib-0.6.1/mathbib/remote/zbl.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.0/mathbib/remote/zbmath.py` & `mathbib-0.6.1/mathbib/remote/zbmath.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.0/mathbib/request.py` & `mathbib-0.6.1/mathbib/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,20 @@
         timeout: float = 30,
         info: bool = True,
         cache: bool = True,
         remote: bool = True,
     ):
         self.session = requests.Session()
 
-        contact_email = tomllib.loads(
-            (xdg_config_home() / "mathbib" / "config.toml").read_text()
-        ).get("email")
+        try:
+            contact_email = tomllib.loads(
+                (xdg_config_home() / "mathbib" / "config.toml").read_text()
+            ).get("email")
+        except FileNotFoundError:
+            contact_email = None
         if contact_email is not None:
             self.session.headers.update(
                 {"User-Agent": f"MathBib (mailto:{contact_email})"}
             )
 
         self.timeout = timeout
         self.print_info = info
```

### Comparing `mathbib-0.6.0/mathbib/resources/journal_abbrevs.json` & `mathbib-0.6.1/mathbib/resources/journal_abbrevs.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992959729653619%*

 * *Differences: {"'indagationes_mathematicae_new_series'": "'Indag. Math.'",*

 * * "'koninklijke_nederlandse_akademie_van_wetenschappen_indagationes_mathematicae_new_series'": "'Indag. "*

 * *                                                                                              "Math.'",*

 * * "'markov_processes_and_related_fields'": "'Markov Process. Relat. Fields'",*

 * * "'probability_theory_and_related_fields'": "'Probab. Theory Relat. Fields'"}*

```diff
@@ -1302,14 +1302,15 @@
     "ima_journal_of_numerical_analysis": "IMA J. Numer. Anal.",
     "image_analysis_&_stereology_quantitative_methods_and_applications": "Image Anal. Stereol.",
     "imhotep_journal_africain_de_mathematiques_pures_et_appliquees_african_journal_of_pure_and_applied_mathematics": "IMHOTEP J. Afr. Math. Pures Appl.",
     "imhotep_mathematical_proceedings": "Imhotep Math. Proc.",
     "impa_monographs": "IMPA Monogr.",
     "impan_lecture_notes": "IMPAN Lect. Notes",
     "imsc_lecture_notes_in_mathematics": "IMSc Lect. Notes Math.",
+    "indagationes_mathematicae_new_series": "Indag. Math.",
     "indian_academy_of_sciences_proceedings_mathematical_sciences": "Proc. Indian Acad. Sci. Math. Sci.",
     "indian_journal_of_discrete_mathematics": "Indian J. Discrete Math.",
     "indian_journal_of_history_of_science": "Indian J. Hist. Sci.",
     "indian_journal_of_mathematics": "Indian J. Math.",
     "indian_journal_of_pure_and_applied_mathematics": "Indian J. Pure Appl. Math.",
     "indian_statistical_institute_series": "Indian Stat. Inst. Ser.",
     "indiana_university_mathematics_journal": "Indiana Univ. Math. J.",
@@ -1881,15 +1882,15 @@
     "kinetic_and_related_models": "Kinet. Relat. Models",
     "kinki_university_series_on_quantum_computing": "Kinki Univ. Ser. Quantum Comput.",
     "klagenfurter_beitrage_zur_didaktik_der_mathematik": "Klagenf. Beitr. Didakt. Math.",
     "klassische_texte_der_wissenschaft": "Klass. Texte Wiss.",
     "kobe_journal_of_mathematics": "Kobe J. Math.",
     "kodai_mathematical_journal": "Kodai Math. J.",
     "kolleg_philosophie": "Kolleg Philos.",
-    "koninklijke_nederlandse_akademie_van_wetenschappen_indagationes_mathematicae_new_series": "Indag. Math. (N.S.)",
+    "koninklijke_nederlandse_akademie_van_wetenschappen_indagationes_mathematicae_new_series": "Indag. Math.",
     "konuralp_journal_of_mathematics": "Konuralp J. Math.",
     "korean_annals_of_mathematics": "Korean Ann. Math.",
     "korean_mathematical_society_communications": "Commun. Korean Math. Soc.",
     "kragujevac_journal_of_mathematics": "Kragujevac J. Math.",
     "kumamoto_journal_of_mathematics": "Kumamoto J. Math.",
     "kuwait_journal_of_science": "Kuwait J. Sci.",
     "kybernetes_the_international_journal_of_cybernetics,_systems_and_management_sciences": "Kybernetes",
@@ -2014,15 +2015,15 @@
     "male_monografie_pwn_technika": "Male Monogr. PWN Tech.",
     "management_and_industrial_engineering": "Manag. Ind. Eng",
     "management_and_information_systems": "Management and Inform. Systems",
     "management_for_professionals": "Manag. Prof.",
     "manufacturing_engineering_and_materials_processing": "Manuf. Eng. Mater. Process.",
     "manuscripta_mathematica": "Manuscripta Math.",
     "mario_boella_series_on_electromagnetism_in_information_and_communication": "Mario Boella Ser. Electromagn. Inf. Commun.",
-    "markov_processes_and_related_fields": "Markov Process. Related Fields",
+    "markov_processes_and_related_fields": "Markov Process. Relat. Fields",
     "martin_gardner's_mathematical_games": "Martin Gardner's Math. Games",
     "mastering_mathematical_finance": "Mastering Math. Finance",
     "mat_serie_a:_conferencias,_seminarios_y_trabajos_de_matematica": "MAT Ser. A Conf. Semin. Trab. Mat.",
     "match_communications_in_mathematical_and_in_computer_chemistry": "MATCH Commun. Math. Comput. Chem.",
     "matematica,_cultura_e_societa_rivista_dell'unione_matematica_italiana_serie_i": "Mat. Cult. Soc. Riv. Unione Mat. Ital. (I)",
     "matematica_contemporanea": "Mat. Contemp.",
     "matematiche_complementari": "Mat. Complement.",
@@ -2554,15 +2555,15 @@
     "probability,_uncertainty_and_quantitative_risk": "Probab. Uncertain. Quant. Risk",
     "probability_and_its_applications": "Probab. Appl.",
     "probability_and_its_applications_(new_york)": "Probab. Appl. (N. Y.)",
     "probability_and_mathematical_physics": "Probab. Math. Phys.",
     "probability_and_mathematical_statistics": "Probab. Math. Statist.",
     "probability_in_the_engineering_and_informational_sciences": "Probab. Engrg. Inform. Sci.",
     "probability_surveys": "Probab. Surv.",
-    "probability_theory_and_related_fields": "Probab. Theory Related Fields",
+    "probability_theory_and_related_fields": "Probab. Theory Relat. Fields",
     "probability_theory_and_stochastic_modelling": "Probab. Theory Stoch. Model.",
     "problem_books_in_mathematics": "Probl. Books in Math.",
     "problem_solving_in_mathematics_and_beyond": "Probl. Solving Math. Beyond",
     "probleme_de_matematica_si_fizica:_serie_pentru_liceu": "Probl. Mat. Fiz. Ser. Pentru Liceu",
     "probleme_globale_ale_omenirii": "Probl. Globale Omen.",
     "problems_of_information_transmission": "Probl. Inf. Transm.",
     "problemy_analiza_issues_of_analysis": "Probl. Anal. Issues Anal.",
```

### Comparing `mathbib-0.6.0/mathbib/session.py` & `mathbib-0.6.1/mathbib/session.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.0/mathbib/term.py` & `mathbib-0.6.1/mathbib/term.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.0/pyproject.toml` & `mathbib-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mathbib"
-version = "0.6.0"
+version = "0.6.1"
 description = "A mathematics BibLaTeX bibliography manager."
 authors = ["Alex Rutar <alex@rutar.org>"]
 readme = "README.md"
 packages = [{include = "mathbib"}]
 license = "MIT"
 repository = "https://github.com/alexrutar/mathbib-py"
 include = ["mathbib/resources/journal_abbrevs.json"]
```

### Comparing `mathbib-0.6.0/PKG-INFO` & `mathbib-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathbib
-Version: 0.6.0
+Version: 0.6.1
 Summary: A mathematics BibLaTeX bibliography manager.
 Home-page: https://github.com/alexrutar/mathbib-py
 License: MIT
 Author: Alex Rutar
 Author-email: alex@rutar.org
 Requires-Python: >=3.11.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

