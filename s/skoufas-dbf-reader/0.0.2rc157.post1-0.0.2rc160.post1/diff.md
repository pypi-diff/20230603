# Comparing `tmp/skoufas_dbf_reader-0.0.2rc157.post1.tar.gz` & `tmp/skoufas_dbf_reader-0.0.2rc160.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skoufas_dbf_reader-0.0.2rc157.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "skoufas_dbf_reader-0.0.2rc160.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `skoufas_dbf_reader-0.0.2rc157.post1.tar` & `skoufas_dbf_reader-0.0.2rc160.post1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      358 2023-06-01 16:38:20.062433 skoufas_dbf_reader-0.0.2rc157.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     2310 2023-06-01 16:38:20.062433 skoufas_dbf_reader-0.0.2rc157.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0       93 2023-06-01 16:38:20.062433 skoufas_dbf_reader-0.0.2rc157.post1/.flake8
--rw-r--r--   0        0        0      239 2023-06-01 16:38:20.062433 skoufas_dbf_reader-0.0.2rc157.post1/.github/dependabot.yml
--rw-r--r--   0        0        0     1552 2023-06-01 16:38:20.062433 skoufas_dbf_reader-0.0.2rc157.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0     1521 2023-06-01 16:38:20.062433 skoufas_dbf_reader-0.0.2rc157.post1/.github/workflows/jekyll-gh-pages.yml
--rw-r--r--   0        0        0      263 2023-06-01 16:38:20.062433 skoufas_dbf_reader-0.0.2rc157.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1824 2023-06-01 16:38:20.062433 skoufas_dbf_reader-0.0.2rc157.post1/.gitignore
--rw-r--r--   0        0        0     1540 2023-06-01 16:38:20.062433 skoufas_dbf_reader-0.0.2rc157.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2023-06-01 16:38:20.062433 skoufas_dbf_reader-0.0.2rc157.post1/.pypirc
--rw-r--r--   0        0        0      129 2023-06-01 16:38:20.062433 skoufas_dbf_reader-0.0.2rc157.post1/.vscode/extensions.json
--rw-r--r--   0        0        0      127 2023-06-01 16:38:20.062433 skoufas_dbf_reader-0.0.2rc157.post1/.vscode/settings.json
--rw-r--r--   0        0        0    34523 2023-06-01 16:38:20.066433 skoufas_dbf_reader-0.0.2rc157.post1/LICENSE
--rw-r--r--   0        0        0     6247 2023-06-01 16:38:20.066433 skoufas_dbf_reader-0.0.2rc157.post1/README.md
--rw-r--r--   0        0        0     5747 2023-06-01 16:38:20.066433 skoufas_dbf_reader-0.0.2rc157.post1/pyproject.toml
--rw-r--r--   0        0        0       95 2023-06-01 16:38:23.466436 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/__init__.py
--rw-r--r--   0        0        0     4563 2023-06-01 16:38:20.066433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/correction_data.py
--rw-r--r--   0        0        0   678429 2023-06-01 16:38:20.066433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/author_corrections.yml
--rw-r--r--   0        0        0 17966037 2023-06-01 16:38:20.130433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/converted_entries.yml
--rw-r--r--   0        0        0   261526 2023-06-01 16:38:20.130433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/editor_corrections.yml
--rw-r--r--   0        0        0  6059317 2023-06-01 16:38:20.154433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/entries.yml
--rw-r--r--   0        0        0     2236 2023-06-01 16:38:20.154433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field04_corrections.yml
--rw-r--r--   0        0        0     1492 2023-06-01 16:38:20.154433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field05_corrections.yml
--rw-r--r--   0        0        0     1662 2023-06-01 16:38:20.154433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field06_corrections.yml
--rw-r--r--   0        0        0     2149 2023-06-01 16:38:20.154433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field07_corrections.yml
--rw-r--r--   0        0        0   133171 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field08_corrections.yml
--rw-r--r--   0        0        0    12404 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field09_corrections.yml
--rw-r--r--   0        0        0      493 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field10_corrections.yml
--rw-r--r--   0        0        0      440 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field11_corrections.yml
--rw-r--r--   0        0        0     1816 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field16_corrections.yml
--rw-r--r--   0        0        0    45765 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field17_corrections.yml
--rw-r--r--   0        0        0     1081 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field18_corrections.yml
--rw-r--r--   0        0        0    38584 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field19_corrections.yml
--rw-r--r--   0        0        0      247 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field20_corrections.yml
--rw-r--r--   0        0        0    24214 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field30_corrections.yml
--rw-r--r--   0        0        0     6773 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/first_names.yml
--rw-r--r--   0        0        0       50 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/language_codes.yml
--rw-r--r--   0        0        0    65691 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/topic_replacements.yml
--rw-r--r--   0        0        0   109074 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/translator_corrections.yml
--rw-r--r--   0        0        0     1192 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/dbf_to_yaml.py
--rw-r--r--   0        0        0    21896 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/field_extractors.py
--rw-r--r--   0        0        0    26558 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/generate_reports.py
--rw-r--r--   0        0        0     6286 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/utilities.py
--rw-r--r--   0        0        0    18619 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/tests/test_field_extractors.py
--rw-r--r--   0        0        0    17733 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/tests/test_reports.py
--rw-r--r--   0        0        0     1173 2023-06-01 16:38:20.158433 skoufas_dbf_reader-0.0.2rc157.post1/tests/test_utilities.py
--rw-r--r--   0        0        0     7952 1970-01-01 00:00:00.000000 skoufas_dbf_reader-0.0.2rc157.post1/PKG-INFO
+-rw-r--r--   0        0        0      358 2023-06-03 09:18:18.407166 skoufas_dbf_reader-0.0.2rc160.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     2310 2023-06-03 09:18:18.407166 skoufas_dbf_reader-0.0.2rc160.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0       93 2023-06-03 09:18:18.407166 skoufas_dbf_reader-0.0.2rc160.post1/.flake8
+-rw-r--r--   0        0        0      239 2023-06-03 09:18:18.407166 skoufas_dbf_reader-0.0.2rc160.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1552 2023-06-03 09:18:18.407166 skoufas_dbf_reader-0.0.2rc160.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0     1521 2023-06-03 09:18:18.407166 skoufas_dbf_reader-0.0.2rc160.post1/.github/workflows/jekyll-gh-pages.yml
+-rw-r--r--   0        0        0      263 2023-06-03 09:18:18.407166 skoufas_dbf_reader-0.0.2rc160.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1824 2023-06-03 09:18:18.407166 skoufas_dbf_reader-0.0.2rc160.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2023-06-03 09:18:18.407166 skoufas_dbf_reader-0.0.2rc160.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2023-06-03 09:18:18.407166 skoufas_dbf_reader-0.0.2rc160.post1/.pypirc
+-rw-r--r--   0        0        0      129 2023-06-03 09:18:18.407166 skoufas_dbf_reader-0.0.2rc160.post1/.vscode/extensions.json
+-rw-r--r--   0        0        0      127 2023-06-03 09:18:18.407166 skoufas_dbf_reader-0.0.2rc160.post1/.vscode/settings.json
+-rw-r--r--   0        0        0    34523 2023-06-03 09:18:18.407166 skoufas_dbf_reader-0.0.2rc160.post1/LICENSE
+-rw-r--r--   0        0        0     6247 2023-06-03 09:18:18.407166 skoufas_dbf_reader-0.0.2rc160.post1/README.md
+-rw-r--r--   0        0        0     5747 2023-06-03 09:18:18.407166 skoufas_dbf_reader-0.0.2rc160.post1/pyproject.toml
+-rw-r--r--   0        0        0       95 2023-06-03 09:18:21.339206 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/__init__.py
+-rw-r--r--   0        0        0     4563 2023-06-03 09:18:18.407166 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/correction_data.py
+-rw-r--r--   0        0        0   678429 2023-06-03 09:18:18.411166 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/author_corrections.yml
+-rw-r--r--   0        0        0 17966037 2023-06-03 09:18:18.471167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/converted_entries.yml
+-rw-r--r--   0        0        0   261526 2023-06-03 09:18:18.471167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/editor_corrections.yml
+-rw-r--r--   0        0        0  6059317 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/entries.yml
+-rw-r--r--   0        0        0     2236 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field04_corrections.yml
+-rw-r--r--   0        0        0     1492 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field05_corrections.yml
+-rw-r--r--   0        0        0     1662 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field06_corrections.yml
+-rw-r--r--   0        0        0     2149 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field07_corrections.yml
+-rw-r--r--   0        0        0   133171 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field08_corrections.yml
+-rw-r--r--   0        0        0    12404 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field09_corrections.yml
+-rw-r--r--   0        0        0      493 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field10_corrections.yml
+-rw-r--r--   0        0        0      440 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field11_corrections.yml
+-rw-r--r--   0        0        0     1816 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field16_corrections.yml
+-rw-r--r--   0        0        0    45765 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field17_corrections.yml
+-rw-r--r--   0        0        0     1081 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field18_corrections.yml
+-rw-r--r--   0        0        0    38584 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field19_corrections.yml
+-rw-r--r--   0        0        0      247 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field20_corrections.yml
+-rw-r--r--   0        0        0    24214 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field30_corrections.yml
+-rw-r--r--   0        0        0     6773 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/first_names.yml
+-rw-r--r--   0        0        0       50 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/language_codes.yml
+-rw-r--r--   0        0        0    65691 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/topic_replacements.yml
+-rw-r--r--   0        0        0   109074 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/translator_corrections.yml
+-rw-r--r--   0        0        0     1192 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/dbf_to_yaml.py
+-rw-r--r--   0        0        0    21896 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/field_extractors.py
+-rw-r--r--   0        0        0    28026 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/generate_reports.py
+-rw-r--r--   0        0        0     6286 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/utilities.py
+-rw-r--r--   0        0        0    18619 2023-06-03 09:18:18.499167 skoufas_dbf_reader-0.0.2rc160.post1/tests/test_field_extractors.py
+-rw-r--r--   0        0        0    18702 2023-06-03 09:18:18.503167 skoufas_dbf_reader-0.0.2rc160.post1/tests/test_reports.py
+-rw-r--r--   0        0        0     1173 2023-06-03 09:18:18.503167 skoufas_dbf_reader-0.0.2rc160.post1/tests/test_utilities.py
+-rw-r--r--   0        0        0     7952 1970-01-01 00:00:00.000000 skoufas_dbf_reader-0.0.2rc160.post1/PKG-INFO
```

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/.devcontainer/devcontainer.json` & `skoufas_dbf_reader-0.0.2rc160.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/.github/workflows/CI.yml` & `skoufas_dbf_reader-0.0.2rc160.post1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/.github/workflows/jekyll-gh-pages.yml` & `skoufas_dbf_reader-0.0.2rc160.post1/.github/workflows/jekyll-gh-pages.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/.gitignore` & `skoufas_dbf_reader-0.0.2rc160.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/.pre-commit-config.yaml` & `skoufas_dbf_reader-0.0.2rc160.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/LICENSE` & `skoufas_dbf_reader-0.0.2rc160.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/README.md` & `skoufas_dbf_reader-0.0.2rc160.post1/README.md`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/pyproject.toml` & `skoufas_dbf_reader-0.0.2rc160.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/correction_data.py` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/correction_data.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/author_corrections.yml` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/author_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/converted_entries.yml` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/converted_entries.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/editor_corrections.yml` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/editor_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/entries.yml` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/entries.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field04_corrections.yml` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field04_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field05_corrections.yml` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field05_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field06_corrections.yml` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field06_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field07_corrections.yml` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field07_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field08_corrections.yml` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field08_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field09_corrections.yml` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field09_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field16_corrections.yml` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field16_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field17_corrections.yml` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field17_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field18_corrections.yml` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field18_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field19_corrections.yml` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field19_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/field30_corrections.yml` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/field30_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/first_names.yml` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/first_names.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/topic_replacements.yml` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/topic_replacements.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/data/translator_corrections.yml` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/data/translator_corrections.yml`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/dbf_to_yaml.py` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/dbf_to_yaml.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/field_extractors.py` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/field_extractors.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/generate_reports.py` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/generate_reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,30 +217,56 @@
         doc.add_heading("Dewey στην είσοδο που δεν βγαίνουν στην έξοδο")
         for k, v in sorted(no_output_dewey.items()):
             doc.add_heading(k, level=2)
             doc.add_unordered_list([str(Inline(entry, link=f"../entries/entry_{entry:05}.html")) for entry in v])
         outfile.write(str(doc))
 
 
-def report_translators(reports_directory: str):
+def report_weird_names(reports_directory: str):
     os.makedirs(os.path.join(reports_directory, "checks"), exist_ok=True)
     weird_translators: list[str] = []
-    valid_translator_re = re.compile(r"[Α-Ω\-]+,[Α-Ω\.]*\.?")
+    weird_authors: list[str] = []
+    weird_curators: list[str] = []
+    weird_donors: list[str] = []
+    valid_name_re = re.compile(r"[A-ZΑ-Ω\-]+,[A-ZΑ-Ω\.]*\.?")
     for entry in all_entries():
         translator = translator_from_a06(entry[6])
         if translator:
             translators = translator.split("!!")
             for translator in translators:
-                if not valid_translator_re.fullmatch(translator):
+                if not valid_name_re.fullmatch(translator):
                     weird_translators.append(translator)
-    with open(os.path.join(reports_directory, "checks", "invalid_translators.md"), "w", encoding="utf-8") as outfile:
-        doc = Document()
-        doc.add_heading("Μεταφραστές με παράξενα ονόματα")
-        doc.add_unordered_list(sorted(weird_translators))
-        outfile.write(str(doc))
+        authors = authors_from_a01(entry[1])
+        for author in authors:
+            if not valid_name_re.fullmatch(author):
+                weird_authors.append(author)
+        curator = curator_from_a16(entry[16])
+        if curator:
+            curators = curator.split("!!")
+            for curator in curators:
+                if not valid_name_re.fullmatch(curator):
+                    weird_curators.append(curator)
+        donor = donation_from_a17_a30(entry[17], entry[30])
+        if donor:
+            donors = donor.split("!!")
+            for donor in donors:
+                if not valid_name_re.fullmatch(donor):
+                    weird_donors.append(donor)
+
+    for field, greek_name, thelist in [
+        ("translators", "Μεταφραστές", weird_translators),
+        ("authors", "Συγγραφείς", weird_authors),
+        ("curators", "Επιμελητές", weird_curators),
+        ("donors", "Δωρητές", weird_donors),
+    ]:
+        with open(os.path.join(reports_directory, "checks", f"invalid_{field}.md"), "w", encoding="utf-8") as outfile:
+            doc = Document()
+            doc.add_heading(f"{greek_name} με παράξενα ονόματα")
+            doc.add_unordered_list(sorted(set(thelist)))
+            outfile.write(str(doc))
 
 
 def report_donors(reports_directory: str):
     os.makedirs(os.path.join(reports_directory, "checks"), exist_ok=True)
     count_map: defaultdict[str, int] = defaultdict(int)
     for entry in all_entries():
         donors = donation_from_a17_a30(entry[17], entry[30])
@@ -587,15 +613,20 @@
         )
     )
     doc.add_paragraph(str(Inline("Καρτέλες χωρίς αριθμό εισαγωγής", link="./checks/no_entry_numbers.html")))
     doc.add_paragraph(
         str(Inline("Καρτέλες με μή αριθμητικό αριθμό εισαγωγής", link="./checks/non_numeric_entry_numbers.html"))
     )
     doc.add_paragraph(str(Inline("Dewey με προβληματικές τιμές", link="./checks/invalid_dewey.html")))
+
     doc.add_paragraph(str(Inline("Μεταφραστές με παράξενα ονόματα", link="./checks/invalid_translators.html")))
+    doc.add_paragraph(str(Inline("Συγγραφείς με παράξενα ονόματα", link="./checks/invalid_authors.html")))
+    doc.add_paragraph(str(Inline("Επιμελητές με παράξενα ονόματα", link="./checks/invalid_curators.html")))
+    doc.add_paragraph(str(Inline("Δωρητές με παράξενα ονόματα", link="./checks/invalid_donors.html")))
+
     doc.add_paragraph(str(Inline("Προβληματικά ISBN", link="./checks/invalid_isbn.html")))
 
     doc.add_paragraph(str(Inline("Δωρητές", link="./checks/donors.html")))
 
     with open(os.path.join(reports_directory, "index.md"), "w", encoding="utf-8") as outfile:
         outfile.write(str(doc))
 
@@ -605,15 +636,15 @@
     if len(sys.argv) > 0:
         md_report_dir = os.path.abspath(sys.argv[1])
     else:
         md_report_dir = os.path.join(os.path.dirname(os.path.abspath(__file__)), os.pardir, os.pardir, "md_reports")
     print(f"Creating reports in {md_report_dir}")
     shutil.rmtree(md_report_dir, ignore_errors=True)
     add_index(md_report_dir)
-    report_translators(md_report_dir)
+    report_weird_names(md_report_dir)
     report_donors(md_report_dir)
     report_isbns(md_report_dir)
     report_entry_numbers(md_report_dir)
     report_entries(md_report_dir)
     report_single_fields(md_report_dir)
     report_single_extracted_fields(md_report_dir)
     report_invalid_dewey(md_report_dir)
```

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/src/skoufas_dbf_reader/utilities.py` & `skoufas_dbf_reader-0.0.2rc160.post1/src/skoufas_dbf_reader/utilities.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/tests/test_field_extractors.py` & `skoufas_dbf_reader-0.0.2rc160.post1/tests/test_field_extractors.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/tests/test_reports.py` & `skoufas_dbf_reader-0.0.2rc160.post1/tests/test_reports.py`

 * *Files 6% similar despite different names*

```diff
@@ -202,26 +202,51 @@
         yaml.dump(no_entry_numbers, outfile, default_flow_style=False, allow_unicode=True)
     with open(os.path.join(reports_directory, f"entry_numbers_non_numeric.yml"), "w", encoding="utf-8") as outfile:
         yaml.dump(dict(non_numeric), outfile, default_flow_style=False, allow_unicode=True)
     with open(os.path.join(reports_directory, f"entry_numbers_duplicate.yml"), "w", encoding="utf-8") as outfile:
         yaml.dump(dict(duplicate_entry_numbers), outfile, default_flow_style=False, allow_unicode=True)
 
 
-def test_report_translators(reports_directory: str):
+def test_report_weird_names(reports_directory: str):
     weird_translators: list[str] = []
-    valid_translator_re = re.compile(r"[Α-Ω\-]+,[Α-Ω\.]*\.?")
+    weird_authors: list[str] = []
+    weird_curators: list[str] = []
+    weird_donors: list[str] = []
+    valid_name_re = re.compile(r"[A-ZΑ-Ω\-]+,[A-ZΑ-Ω\.]*\.?")
     for entry in all_entries():
         translator = translator_from_a06(entry[6])
         if translator:
             translators = translator.split("!!")
             for translator in translators:
-                if not valid_translator_re.fullmatch(translator):
+                if not valid_name_re.fullmatch(translator):
                     weird_translators.append(translator)
-    with open(os.path.join(reports_directory, f"weird_translators.yml"), "w", encoding="utf-8") as outfile:
-        yaml.dump(weird_translators, outfile, default_flow_style=False, allow_unicode=True)
+        authors = authors_from_a01(entry[1])
+        for author in authors:
+            if not valid_name_re.fullmatch(author):
+                weird_authors.append(author)
+        curator = curator_from_a16(entry[16])
+        if curator:
+            curators = curator.split("!!")
+            for curator in curators:
+                if not valid_name_re.fullmatch(curator):
+                    weird_curators.append(curator)
+        donor = donation_from_a17_a30(entry[17], entry[30])
+        if donor:
+            donors = donor.split("!!")
+            for donor in donors:
+                if not valid_name_re.fullmatch(donor):
+                    weird_donors.append(donor)
+    for field, thelist in [
+        ("translators", weird_translators),
+        ("authors", weird_authors),
+        ("curators", weird_curators),
+        ("donors", weird_donors),
+    ]:
+        with open(os.path.join(reports_directory, f"weird_{field}.yml"), "w", encoding="utf-8") as outfile:
+            yaml.dump(sorted(set(thelist)), outfile, default_flow_style=False, allow_unicode=True)
 
 
 def test_report_bools(reports_directory: str):
     entries_with_cd: list[dict[int, str]] = list()
     entries_with_dvd: list[dict[int, str]] = list()
     entries_with_offprint: list[dict[int, str]] = list()
     for entry in all_entries():
```

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/tests/test_utilities.py` & `skoufas_dbf_reader-0.0.2rc160.post1/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `skoufas_dbf_reader-0.0.2rc157.post1/PKG-INFO` & `skoufas_dbf_reader-0.0.2rc160.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skoufas-dbf-reader
-Version: 0.0.2rc157.post1
+Version: 0.0.2rc160.post1
 Summary: Library for reading legacy DBF file with library data
 Author-email: Claudio Bantaloukas <rockreamer@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

