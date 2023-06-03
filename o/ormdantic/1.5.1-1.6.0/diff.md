# Comparing `tmp/ormdantic-1.5.1.tar.gz` & `tmp/ormdantic-1.6.0.tar.gz`

## Comparing `ormdantic-1.5.1.tar` & `ormdantic-1.6.0.tar`

### file list

```diff
@@ -1,60 +1,54 @@
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 ormdantic-1.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ormdantic-1.5.1/codecov.yml
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 ormdantic-1.5.1/mkdocs.yml
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ormdantic-1.5.1/mypy.ini
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 ormdantic-1.5.1/pytest.ini
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ormdantic-1.5.1/setup.cfg
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 ormdantic-1.5.1/.github/CODEOWNERS
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ormdantic-1.5.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ormdantic-1.5.1/.github/dependabot.yml
--rw-r--r--   0        0        0    18349 2020-02-02 00:00:00.000000 ormdantic-1.5.1/.github/logo.png
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 ormdantic-1.5.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 ormdantic-1.5.1/.github/workflows/integration.yml
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 ormdantic-1.5.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 ormdantic-1.5.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 ormdantic-1.5.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 ormdantic-1.5.1/docs/code_of_conduct.md
--rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 ormdantic-1.5.1/docs/contributing.md
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 ormdantic-1.5.1/docs/faq.md
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 ormdantic-1.5.1/docs/favicon.png
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 ormdantic-1.5.1/docs/index.md
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 ormdantic-1.5.1/docs/installation.md
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 ormdantic-1.5.1/docs/license.md
--rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 ormdantic-1.5.1/docs/usage.md
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ormdantic-1.5.1/ormdantic/__init__.py
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 ormdantic-1.5.1/ormdantic/orm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ormdantic-1.5.1/ormdantic/py.typed
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 ormdantic-1.5.1/ormdantic/generator/__init__.py
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 ormdantic-1.5.1/ormdantic/generator/_crud.py
--rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 ormdantic-1.5.1/ormdantic/generator/_field.py
--rw-r--r--   0        0        0     6789 2020-02-02 00:00:00.000000 ormdantic-1.5.1/ormdantic/generator/_lazy.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 ormdantic-1.5.1/ormdantic/generator/_query.py
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 ormdantic-1.5.1/ormdantic/generator/_serializer.py
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 ormdantic-1.5.1/ormdantic/generator/_table.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ormdantic-1.5.1/ormdantic/handler/__init__.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 ormdantic-1.5.1/ormdantic/handler/errors.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ormdantic-1.5.1/ormdantic/handler/helper.py
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 ormdantic-1.5.1/ormdantic/handler/random.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 ormdantic-1.5.1/ormdantic/handler/snake.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ormdantic-1.5.1/ormdantic/models/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 ormdantic-1.5.1/ormdantic/models/models.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ormdantic-1.5.1/ormdantic/types/__init__.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 ormdantic-1.5.1/ormdantic/types/base.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 ormdantic-1.5.1/scripts/clean.sh
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ormdantic-1.5.1/scripts/format.sh
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ormdantic-1.5.1/scripts/integration.sh
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 ormdantic-1.5.1/scripts/lint.sh
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 ormdantic-1.5.1/scripts/test.sh
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ormdantic-1.5.1/scripts/test_html.sh
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 ormdantic-1.5.1/tests/test_errors.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 ormdantic-1.5.1/tests/test_generator.py
--rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 ormdantic-1.5.1/tests/test_orm.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 ormdantic-1.5.1/tests/test_otm_relations.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 ormdantic-1.5.1/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ormdantic-1.5.1/tests/integration/__init__.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 ormdantic-1.5.1/tests/integration/demo.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 ormdantic-1.5.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ormdantic-1.5.1/LICENSE
--rw-r--r--   0        0        0    10553 2020-02-02 00:00:00.000000 ormdantic-1.5.1/README.md
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 ormdantic-1.5.1/pyproject.toml
--rw-r--r--   0        0        0    12815 2020-02-02 00:00:00.000000 ormdantic-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 ormdantic-1.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 ormdantic-1.6.0/mkdocs.yml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ormdantic-1.6.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 ormdantic-1.6.0/.github/dependabot.yml
+-rw-r--r--   0        0        0    18349 2020-02-02 00:00:00.000000 ormdantic-1.6.0/.github/logo.png
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ormdantic-1.6.0/.github/workflows/cache.yml
+-rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 ormdantic-1.6.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 ormdantic-1.6.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 ormdantic-1.6.0/docs/code_of_conduct.md
+-rw-r--r--   0        0        0     6057 2020-02-02 00:00:00.000000 ormdantic-1.6.0/docs/contributing.md
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 ormdantic-1.6.0/docs/faq.md
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 ormdantic-1.6.0/docs/favicon.png
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 ormdantic-1.6.0/docs/index.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 ormdantic-1.6.0/docs/installation.md
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 ormdantic-1.6.0/docs/license.md
+-rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 ormdantic-1.6.0/docs/usage.md
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ormdantic-1.6.0/ormdantic/__init__.py
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 ormdantic-1.6.0/ormdantic/orm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ormdantic-1.6.0/ormdantic/py.typed
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 ormdantic-1.6.0/ormdantic/generator/__init__.py
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 ormdantic-1.6.0/ormdantic/generator/_crud.py
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 ormdantic-1.6.0/ormdantic/generator/_field.py
+-rw-r--r--   0        0        0     6789 2020-02-02 00:00:00.000000 ormdantic-1.6.0/ormdantic/generator/_lazy.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 ormdantic-1.6.0/ormdantic/generator/_query.py
+-rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 ormdantic-1.6.0/ormdantic/generator/_serializer.py
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 ormdantic-1.6.0/ormdantic/generator/_table.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 ormdantic-1.6.0/ormdantic/handler/__init__.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 ormdantic-1.6.0/ormdantic/handler/errors.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ormdantic-1.6.0/ormdantic/handler/helper.py
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 ormdantic-1.6.0/ormdantic/handler/random.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 ormdantic-1.6.0/ormdantic/handler/snake.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ormdantic-1.6.0/ormdantic/models/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 ormdantic-1.6.0/ormdantic/models/models.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ormdantic-1.6.0/ormdantic/types/__init__.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 ormdantic-1.6.0/ormdantic/types/base.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 ormdantic-1.6.0/scripts/clean.sh
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ormdantic-1.6.0/scripts/format.sh
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ormdantic-1.6.0/scripts/integration.sh
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 ormdantic-1.6.0/scripts/lint.sh
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 ormdantic-1.6.0/scripts/test.sh
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 ormdantic-1.6.0/scripts/test_html.sh
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 ormdantic-1.6.0/tests/test_errors.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 ormdantic-1.6.0/tests/test_generator.py
+-rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 ormdantic-1.6.0/tests/test_orm.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 ormdantic-1.6.0/tests/test_otm_relations.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 ormdantic-1.6.0/tests/test_snake.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 ormdantic-1.6.0/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ormdantic-1.6.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 ormdantic-1.6.0/tests/integration/demo.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 ormdantic-1.6.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ormdantic-1.6.0/LICENSE
+-rw-r--r--   0        0        0    10496 2020-02-02 00:00:00.000000 ormdantic-1.6.0/README.md
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 ormdantic-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0    12959 2020-02-02 00:00:00.000000 ormdantic-1.6.0/PKG-INFO
```

### Comparing `ormdantic-1.5.1/mkdocs.yml` & `ormdantic-1.6.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/.github/logo.png` & `ormdantic-1.6.0/.github/logo.png`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/.github/workflows/docs.yml` & `ormdantic-1.6.0/.github/workflows/release.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-name: Build Docs
+name: Publish
+
 on:
-  push:
-    branches:
-      - main
+  release:
+    types:
+      - created
 
 jobs:
-  build-docs:
-    runs-on: ubuntu-18.04
+  publish:
+    runs-on: ubuntu-latest
     steps:
       - name: Dump GitHub context
         env:
           GITHUB_CONTEXT: ${{ toJson(github) }}
         run: echo "$GITHUB_CONTEXT"
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.10"
       - uses: actions/cache@v3
         id: cache
         with:
           path: ${{ env.pythonLocation }}
-          key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-docs
-      - name: Install docs extras
+          key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-publish
+      - name: Install build dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install -e .[docs]
-      - name: Build docs
-        run: mkdocs build -d build
-
-      - name: Deploy docs
-        uses: jsmrcaga/action-netlify-deploy@v1.1.0
+        run: pip install build
+      - name: Build distribution
+        run: python -m build
+      - name: Publish
+        uses: pypa/gh-action-pypi-publish@v1.8.6
         with:
-          NETLIFY_AUTH_TOKEN: ${{ secrets.NETLIFY_TOKEN }}
-          NETLIFY_SITE_ID: ${{ secrets.NETLIFY_SITE_ID }}
-          NETLIFY_DEPLOY_TO_PROD: true
-          NETLIFY_DEPLOY_MESSAGE: "Prod deploy v${{ github.ref }}"
+          password: ${{ secrets.PYPI_API_TOKEN }}
+      - name: Dump GitHub context
+        env:
+          GITHUB_CONTEXT: ${{ toJson(github) }}
+        run: echo "$GITHUB_CONTEXT"
```

### Comparing `ormdantic-1.5.1/.github/workflows/integration.yml` & `ormdantic-1.6.0/.github/workflows/ci.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,74 @@
-name: Integration Suite
+name: Continuous Integration
 
 on:
   push:
     branches:
       - main
-  pull_request:
-    types: [opened, synchronize]
+  pull_request: {}
 
 jobs:
+  lint:
+    runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        python-version: ["3.11"]
+      fail-fast: false
+
+    steps:
+      - uses: actions/checkout@v3
+      - name: Set up Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python-version }}
+      - name: Install Dependencies
+        run: pip install -e .[lint]
+      - uses: pre-commit/action@v3.0.0
+        with:
+          extra_args: --all-files --verbose
+      - name: check Static Analysis
+        run: bash scripts/lint.sh
+
+  tests:
+    name: test on python ${{ matrix.python-version }}
+    runs-on: ubuntu-latest
+    timeout-minutes: 30
+    strategy:
+      matrix:
+        python-version: ["3.10", "3.11"]
+
+    steps:
+      - uses: actions/checkout@v3
+      - name: Set up Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python-version }}
+      - uses: actions/cache@v3
+        id: cache
+        with:
+          path: ${{ env.pythonLocation }}
+          key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-test-v02
+      - name: Install SQLAlchemy version 1.4.42
+        run: |
+          python -m pip install --upgrade pip
+          pip install SQLAlchemy==1.4.42
+      - name: Install Dependencies
+        if: steps.cache.outputs.cache-hit != 'true'
+        run: pip install -e .[sqlite,test]
+      - name: Test with pytest
+        run: bash scripts/test.sh
+        env:
+          DATABASE_URL: sqlite+aiosqlite:///db.sqlite3
+      - name: Upload coverage
+        env:
+          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
+        uses: codecov/codecov-action@v3
+
   postgres:
+    name: test on python ${{ matrix.python-version }} with postgres ${{ matrix.postgres-version }}
     runs-on: ubuntu-latest
     timeout-minutes: 30
     strategy:
       matrix:
         python-version: ["3.10", "3.11"]
         postgres-version: [14]
 
@@ -46,14 +102,15 @@
         run: pip install -e .[postgresql,test]
       - name: Integration Tests, Postgres
         run: bash scripts/integration.sh
         env:
           DATABASE_URL: postgresql+asyncpg://postgres:postgres@localhost:5432/postgres
 
   sqlite:
+    name: test on python ${{ matrix.python-version }} with sqlite
     runs-on: ubuntu-latest
     timeout-minutes: 30
     strategy:
       matrix:
         python-version: ["3.10", "3.11"]
 
     steps:
@@ -70,7 +127,18 @@
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
         run: pip install -e .[sqlite,test]
       - name: Integration Tests, SQLite
         run: bash scripts/integration.sh
         env:
           DATABASE_URL: sqlite+aiosqlite:///db.sqlite3
+
+  # https://github.com/marketplace/actions/alls-green#why used for branch protection checks
+  check:
+    if: always()
+    needs: [lint, tests, postgres, sqlite]
+    runs-on: ubuntu-latest
+    steps:
+      - name: Decide whether the needed jobs succeeded or failed
+        uses: re-actors/alls-green@release/v1
+        with:
+          jobs: ${{ toJSON(needs) }}
```

### Comparing `ormdantic-1.5.1/docs/code_of_conduct.md` & `ormdantic-1.6.0/docs/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/docs/contributing.md` & `ormdantic-1.6.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/docs/faq.md` & `ormdantic-1.6.0/docs/faq.md`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/docs/favicon.png` & `ormdantic-1.6.0/docs/favicon.png`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/docs/index.md` & `ormdantic-1.6.0/docs/index.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 ![Logo](https://raw.githubusercontent.com/yezz123/ormdantic/main/.github/logo.png)
 
 <p align="center">
     <em>Asynchronous ORM that uses pydantic models to represent database tables ✨</em>
 </p>
 
 <p align="center">
-<a href="https://github.com/yezz123/ormdantic/actions/workflows/lint.yml" target="_blank">
-    <img src="https://github.com/yezz123/ormdantic/actions/workflows/lint.yml/badge.svg" alt="lint">
-</a>
-<a href="https://github.com/yezz123/ormdantic/actions/workflows/test.yml" target="_blank">
-    <img src="https://github.com/yezz123/ormdantic/actions/workflows/test.yml/badge.svg" alt="Test">
+<a href="https://github.com/yezz123/ormdantic/actions/workflows/ci.yml" target="_blank">
+    <img src="https://github.com/yezz123/ormdantic/actions/workflows/ci.yml/badge.svg" alt="Test">
 </a>
 <a href="https://codecov.io/gh/yezz123/ormdantic">
     <img src="https://codecov.io/gh/yezz123/ormdantic/branch/main/graph/badge.svg"/>
 </a>
 <a href="https://pypi.org/project/ormdantic" target="_blank">
     <img src="https://img.shields.io/pypi/v/ormdantic?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 ![Logo](https://raw.githubusercontent.com/yezz123/ormdantic/main/.github/
 logo.png)
   Asynchronous ORM that uses pydantic models to represent database tables â¨
-   [lint] [Test] [https://codecov.io/gh/yezz123/ormdantic/branch/main/graph/
-                    badge.svg] [Package_version] [Sponsor]
+ [Test] [https://codecov.io/gh/yezz123/ormdantic/branch/main/graph/badge.svg]
+                          [Package_version] [Sponsor]
 Ormdantic is a library for interacting with Asynchronous SQL databases from
 Python code, with Python objects. It is designed to be intuitive, easy to use,
 compatible, and robust. **Ormdantic** is based on [Pypika](https://github.com/
 kayak/pypika), and powered by Pydantic and SQLAlchemy, and Highly inspired by
 Sqlmodel, Created by [@tiangolo](https://github.com/tiangolo). > What is
 [Pypika](https://github.com/kayak/pypika)? > > PyPika is a Python API for
 building SQL queries. The motivation behind PyPika is to provide a simple
```

### Comparing `ormdantic-1.5.1/docs/installation.md` & `ormdantic-1.6.0/docs/installation.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,20 +14,14 @@
 ---> 100%
 
 Successfully installed Ormdantic
 ```
 
 * Install The specific Asynchronous ORM library for your database.
 
-### MySQL
-
-```shell
-$ pip install ormdantic[mysql]
-```
-
 ### SQLite
 
 ```shell
 $ pip install ormdantic[sqlite]
 ```
 
 ### PostgreSQL
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 ## Requirements A recent and currently supported version of Python (right now,
 Python_supports_versions_3.10_and_above). As **Ormdantic** is based on
 **Pydantic** and **SQLAlchemy** and **Pypika**, it requires them. They will be
 automatically installed when you install Ormdantic. ## Installation You can add
 Ormdantic in a few easy steps. First of all, install the dependency: ```shell $
 pip install ormdantic ---> 100% Successfully installed Ormdantic ``` * Install
-The specific Asynchronous ORM library for your database. ### MySQL ```shell $
-pip install ormdantic[mysql] ``` ### SQLite ```shell $ pip install ormdantic
-[sqlite] ``` ### PostgreSQL ```shell $ pip install ormdantic[postgresql] ```
+The specific Asynchronous ORM library for your database. ### SQLite ```shell $
+pip install ormdantic[sqlite] ``` ### PostgreSQL ```shell $ pip install
+ormdantic[postgresql] ```
```

### Comparing `ormdantic-1.5.1/docs/license.md` & `ormdantic-1.6.0/docs/license.md`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/docs/usage.md` & `ormdantic-1.6.0/docs/usage.md`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/ormdantic/orm.py` & `ormdantic-1.6.0/ormdantic/orm.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/ormdantic/generator/_crud.py` & `ormdantic-1.6.0/ormdantic/generator/_crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
     def __init__(
         self,
         table_data: OrmTable,  # type: ignore
         table_map: Map,
         engine: AsyncEngine,
     ) -> None:
-
         self._engine = engine
         self._table_map = table_map
         self._table_data = table_data
         self.tablename = table_data.tablename
         self.columns = table_data.columns
 
     async def find_one(self, pk: Any, depth: int = 0) -> ModelType | None:
```

### Comparing `ormdantic-1.5.1/ormdantic/generator/_field.py` & `ormdantic-1.6.0/ormdantic/generator/_field.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/ormdantic/generator/_lazy.py` & `ormdantic-1.6.0/ormdantic/generator/_lazy.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/ormdantic/generator/_query.py` & `ormdantic-1.6.0/ormdantic/generator/_query.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/ormdantic/generator/_serializer.py` & `ormdantic-1.6.0/ormdantic/generator/_serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 class OrmSerializer(Generic[SerializedType]):
     """Generate Python models from a table map and result set."""
 
     def __init__(
         self,
         table_data: OrmTable,  # type: ignore
         table_map: Map,
+        # TODO: Missing type parameters for generic type "CursorResult".
         result_set: CursorResult,
         is_array: bool,
         depth: int,
     ) -> None:
         """Generate Python models from a table map and result set.
 
         :param table_data: Table data for the returned model type.
```

### Comparing `ormdantic-1.5.1/ormdantic/generator/_table.py` & `ormdantic-1.6.0/ormdantic/generator/_table.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/ormdantic/handler/__init__.py` & `ormdantic-1.6.0/ormdantic/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/ormdantic/handler/errors.py` & `ormdantic-1.6.0/ormdantic/handler/errors.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/ormdantic/handler/helper.py` & `ormdantic-1.6.0/ormdantic/handler/helper.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/ormdantic/handler/random.py` & `ormdantic-1.6.0/ormdantic/handler/random.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/ormdantic/handler/snake.py` & `ormdantic-1.6.0/ormdantic/handler/snake.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/ormdantic/models/models.py` & `ormdantic-1.6.0/ormdantic/models/models.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/ormdantic/types/base.py` & `ormdantic-1.6.0/ormdantic/types/base.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/scripts/clean.sh` & `ormdantic-1.6.0/scripts/clean.sh`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/tests/test_errors.py` & `ormdantic-1.6.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/tests/test_generator.py` & `ormdantic-1.6.0/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/tests/test_orm.py` & `ormdantic-1.6.0/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/tests/test_otm_relations.py` & `ormdantic-1.6.0/tests/test_otm_relations.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/tests/integration/demo.py` & `ormdantic-1.6.0/tests/integration/demo.py`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/.gitignore` & `ormdantic-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/LICENSE` & `ormdantic-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ormdantic-1.5.1/README.md` & `ormdantic-1.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 ![Logo](https://raw.githubusercontent.com/yezz123/ormdantic/main/.github/logo.png)
 
 <p align="center">
     <em>Asynchronous ORM that uses pydantic models to represent database tables ✨</em>
 </p>
 
 <p align="center">
-<a href="https://github.com/yezz123/ormdantic/actions/workflows/lint.yml" target="_blank">
-    <img src="https://github.com/yezz123/ormdantic/actions/workflows/lint.yml/badge.svg" alt="lint">
-</a>
-<a href="https://github.com/yezz123/ormdantic/actions/workflows/test.yml" target="_blank">
-    <img src="https://github.com/yezz123/ormdantic/actions/workflows/test.yml/badge.svg" alt="Test">
+<a href="https://github.com/yezz123/ormdantic/actions/workflows/ci.yml" target="_blank">
+    <img src="https://github.com/yezz123/ormdantic/actions/workflows/ci.yml/badge.svg" alt="Test">
 </a>
 <a href="https://codecov.io/gh/yezz123/ormdantic">
     <img src="https://codecov.io/gh/yezz123/ormdantic/branch/main/graph/badge.svg"/>
 </a>
 <a href="https://pypi.org/project/ormdantic" target="_blank">
     <img src="https://img.shields.io/pypi/v/ormdantic?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
+<a href="https://pypi.org/project/ormdantic" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/ormdantic.svg?color=%2334D058" alt="Supported Python versions">
+</a>
 </p>
 
 Ormdantic is a library for interacting with Asynchronous <abbr title='Also called "Relational databases"'>SQL databases</abbr> from Python code, with Python objects. It is designed to be intuitive, easy to use, compatible, and robust.
 
 **Ormdantic** is based on [Pypika](https://github.com/kayak/pypika), and powered by <a href="https://pydantic-docs.helpmanual.io/" class="external-link" target="_blank">Pydantic</a> and <a href="https://sqlalchemy.org/" class="external-link" target="_blank">SQLAlchemy</a>, and Highly inspired by <a href="https://github.com/tiangolo/Sqlmodel" class="external-link" target="_blank">Sqlmodel</a>, Created by [@tiangolo](https://github.com/tiangolo).
 
 > What is [Pypika](https://github.com/kayak/pypika)?
@@ -51,17 +51,14 @@
 
 Successfully installed Ormdantic
 ```
 
 * Install The specific Asynchronous ORM library for your database.
 
 ```shell
-# MySQL
-$ pip install ormdantic[mysql]
-
 # PostgreSQL
 $ pip install ormdantic[postgres]
 
 # SQLite
 $ pip install ormdantic[sqlite]
 ```
```

### Comparing `ormdantic-1.5.1/pyproject.toml` & `ormdantic-1.6.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -7,72 +7,83 @@
 description = "asynchronous ORM that uses pydantic models to represent database tables"
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MIT"
 authors = [
     { name = "Yasser Tahiri", email = "hello@yezz.me" },
 ]
+keywords = [
+    "orm",
+    "sqlalchemy",
+    "pydantic",
+    "asyncio",
+]
 
 classifiers = [
+    "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
+    "Intended Audience :: Information Technology",
     "Framework :: AsyncIO",
+    "Framework :: Pydantic",
+    "Framework :: Pydantic :: 1",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Internet :: WWW/HTTP :: Session",
+    "Topic :: Database",
     "Typing :: Typed",
 ]
 
 dependencies = [
-    "typing-extensions >=3.7.4,<4.5.0",
+    "typing-extensions >=3.7.4,<4.7.0",
     "pydantic >=1.6.2,!=1.7,!=1.7.1,!=1.7.2,!=1.7.3,!=1.8,!=1.8.1,<2.0.0",
-    "sqlalchemy[asyncio] >=1.3.18,<1.5.0",
+    "sqlalchemy[asyncio]>=1.3.18,<2.0.0",
     "PyPika ==0.48.9"
 ]
 
 dynamic = ["version"]
 
+[tool.hatch.metadata]
+allow-direct-references = true
+
 [project.urls]
 Homepage = "https://github.com/yezz123/ormdantic"
 Documentation = "https://ormdantic.yezz.me/"
 Funding = 'https://github.com/sponsors/yezz123'
 
 [project.optional-dependencies]
 sqlite = [
     "aiosqlite",
 ]
 postgresql = [
     "psycopg2-binary",
     "asyncpg"
 ]
-mysql = [
-    "aiomysql",
-]
 lint = [
-    "pre-commit==2.21.0",
-    "mypy==0.991",
+    "pre-commit==3.3.2",
+    "mypy==1.3.0",
 ]
 test = [
-    "pytest==7.2.0",
-    "pytest-asyncio == 0.20.3",
-    "codecov==2.1.12",
-    "pytest-cov==4.0.0",
+    "pytest==7.3.1",
+    "pytest-asyncio == 0.21.0",
+    "pytest-cov==4.1.0",
     "python-decouple",
+    "pytest-pretty==1.2.0"
 ]
 docs = [
     "mkdocs >=1.1.2,<2.0.0",
-    "mkdocs-material >=8.1.4,<9.0.0",
+    "mkdocs-material >=8.1.4,<10.0.0",
     "mdx-include >=1.4.1,<2.0.0",
     "mkdocs-markdownextradata-plugin >=0.1.7,<0.3.0",
     "mkdocs-mermaid2-plugin==0.6.0",
-    "markdown-include==0.8.0",
-    "pymdown-extensions==9.9",
+    "markdown-include==0.8.1",
+    "pymdown-extensions==10.0.1",
     "jinja2==3.1.2"
 ]
 
 [tool.hatch.version]
 path = "ormdantic/__init__.py"
 
 [tool.isort]
@@ -95,7 +106,53 @@
 ]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.ruff.isort]
 known-third-party = ["pydantic", "sqlalchemy", "typing_extensions"]
+
+[tool.coverage.run]
+source = ["ormdantic"]
+branch = true
+context = '${CONTEXT}'
+
+[tool.coverage.paths]
+source = [
+    "ormdantic",
+]
+
+[tool.mypy]
+plugins = "pydantic.mypy"
+follow_imports = "silent"
+strict_optional = true
+warn_redundant_casts = true
+warn_unused_ignores = true
+disallow_any_generics = true
+check_untyped_defs = true
+ignore_missing_imports = true
+disallow_untyped_defs = true
+
+[[tool.mypy.overrides]]
+module = [
+    'dotenv.*',
+]
+ignore_missing_imports = true
+
+[tool.coverage.report]
+precision = 2
+exclude_lines = [
+    "pragma: no cover",
+    "raise NotImplementedError",
+    "raise NotImplemented",
+    "@overload",
+    "if TYPE_CHECKING:",
+    "if __name__ == .__main__.:",
+]
+
+[tool.pytest.ini_options]
+testpaths = 'tests'
+log_cli = "1"
+log_cli_level = "INFO"
+log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
+log_cli_date_format= "%Y-%m-%d %H:%M:%S"
+asyncio_mode= "auto"
```

### Comparing `ormdantic-1.5.1/PKG-INFO` & `ormdantic-1.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,78 +1,82 @@
 Metadata-Version: 2.1
 Name: ormdantic
-Version: 1.5.1
+Version: 1.6.0
 Summary: asynchronous ORM that uses pydantic models to represent database tables
 Project-URL: Homepage, https://github.com/yezz123/ormdantic
 Project-URL: Documentation, https://ormdantic.yezz.me/
 Project-URL: Funding, https://github.com/sponsors/yezz123
 Author-email: Yasser Tahiri <hello@yezz.me>
 License-Expression: MIT
 License-File: LICENSE
+Keywords: asyncio,orm,pydantic,sqlalchemy
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
+Classifier: Framework :: Pydantic
+Classifier: Framework :: Pydantic :: 1
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Database
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Requires-Dist: pydantic!=1.7,!=1.7.1,!=1.7.2,!=1.7.3,!=1.8,!=1.8.1,<2.0.0,>=1.6.2
 Requires-Dist: pypika==0.48.9
-Requires-Dist: sqlalchemy[asyncio]<1.5.0,>=1.3.18
-Requires-Dist: typing-extensions<4.5.0,>=3.7.4
+Requires-Dist: sqlalchemy[asyncio]<2.0.0,>=1.3.18
+Requires-Dist: typing-extensions<4.7.0,>=3.7.4
 Provides-Extra: docs
 Requires-Dist: jinja2==3.1.2; extra == 'docs'
-Requires-Dist: markdown-include==0.8.0; extra == 'docs'
+Requires-Dist: markdown-include==0.8.1; extra == 'docs'
 Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'docs'
 Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'docs'
-Requires-Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'docs'
+Requires-Dist: mkdocs-material<10.0.0,>=8.1.4; extra == 'docs'
 Requires-Dist: mkdocs-mermaid2-plugin==0.6.0; extra == 'docs'
 Requires-Dist: mkdocs<2.0.0,>=1.1.2; extra == 'docs'
-Requires-Dist: pymdown-extensions==9.9; extra == 'docs'
+Requires-Dist: pymdown-extensions==10.0.1; extra == 'docs'
 Provides-Extra: lint
-Requires-Dist: mypy==0.991; extra == 'lint'
-Requires-Dist: pre-commit==2.21.0; extra == 'lint'
-Provides-Extra: mysql
-Requires-Dist: aiomysql; extra == 'mysql'
+Requires-Dist: mypy==1.3.0; extra == 'lint'
+Requires-Dist: pre-commit==3.3.2; extra == 'lint'
 Provides-Extra: postgresql
 Requires-Dist: asyncpg; extra == 'postgresql'
 Requires-Dist: psycopg2-binary; extra == 'postgresql'
 Provides-Extra: sqlite
 Requires-Dist: aiosqlite; extra == 'sqlite'
 Provides-Extra: test
-Requires-Dist: codecov==2.1.12; extra == 'test'
-Requires-Dist: pytest-asyncio==0.20.3; extra == 'test'
-Requires-Dist: pytest-cov==4.0.0; extra == 'test'
-Requires-Dist: pytest==7.2.0; extra == 'test'
+Requires-Dist: pytest-asyncio==0.21.0; extra == 'test'
+Requires-Dist: pytest-cov==4.1.0; extra == 'test'
+Requires-Dist: pytest-pretty==1.2.0; extra == 'test'
+Requires-Dist: pytest==7.3.1; extra == 'test'
 Requires-Dist: python-decouple; extra == 'test'
 Description-Content-Type: text/markdown
 
 ![Logo](https://raw.githubusercontent.com/yezz123/ormdantic/main/.github/logo.png)
 
 <p align="center">
     <em>Asynchronous ORM that uses pydantic models to represent database tables ✨</em>
 </p>
 
 <p align="center">
-<a href="https://github.com/yezz123/ormdantic/actions/workflows/lint.yml" target="_blank">
-    <img src="https://github.com/yezz123/ormdantic/actions/workflows/lint.yml/badge.svg" alt="lint">
-</a>
-<a href="https://github.com/yezz123/ormdantic/actions/workflows/test.yml" target="_blank">
-    <img src="https://github.com/yezz123/ormdantic/actions/workflows/test.yml/badge.svg" alt="Test">
+<a href="https://github.com/yezz123/ormdantic/actions/workflows/ci.yml" target="_blank">
+    <img src="https://github.com/yezz123/ormdantic/actions/workflows/ci.yml/badge.svg" alt="Test">
 </a>
 <a href="https://codecov.io/gh/yezz123/ormdantic">
     <img src="https://codecov.io/gh/yezz123/ormdantic/branch/main/graph/badge.svg"/>
 </a>
 <a href="https://pypi.org/project/ormdantic" target="_blank">
     <img src="https://img.shields.io/pypi/v/ormdantic?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
+<a href="https://pypi.org/project/ormdantic" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/ormdantic.svg?color=%2334D058" alt="Supported Python versions">
+</a>
 </p>
 
 Ormdantic is a library for interacting with Asynchronous <abbr title='Also called "Relational databases"'>SQL databases</abbr> from Python code, with Python objects. It is designed to be intuitive, easy to use, compatible, and robust.
 
 **Ormdantic** is based on [Pypika](https://github.com/kayak/pypika), and powered by <a href="https://pydantic-docs.helpmanual.io/" class="external-link" target="_blank">Pydantic</a> and <a href="https://sqlalchemy.org/" class="external-link" target="_blank">SQLAlchemy</a>, and Highly inspired by <a href="https://github.com/tiangolo/Sqlmodel" class="external-link" target="_blank">Sqlmodel</a>, Created by [@tiangolo](https://github.com/tiangolo).
 
 > What is [Pypika](https://github.com/kayak/pypika)?
@@ -103,17 +107,14 @@
 
 Successfully installed Ormdantic
 ```
 
 * Install The specific Asynchronous ORM library for your database.
 
 ```shell
-# MySQL
-$ pip install ormdantic[mysql]
-
 # PostgreSQL
 $ pip install ormdantic[postgres]
 
 # SQLite
 $ pip install ormdantic[sqlite]
 ```
```

