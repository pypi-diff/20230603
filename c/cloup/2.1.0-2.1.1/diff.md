# Comparing `tmp/cloup-2.1.0.tar.gz` & `tmp/cloup-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cloup/cloup/dist/.tmp-hidybb66/cloup-2.1.0.tar", last modified: Mon May 15 01:54:24 2023, max compression
+gzip compressed data, was "/home/runner/work/cloup/cloup/dist/.tmp-gwe3sspa/cloup-2.1.1.tar", last modified: Sat Jun  3 14:20:39 2023, max compression
```

## Comparing `cloup-2.1.0.tar` & `cloup-2.1.1.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-15 01:54:09.000000 cloup-2.1.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-15 01:54:09.000000 cloup-2.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-15 01:54:09.000000 cloup-2.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-15 01:54:09.000000 cloup-2.1.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-15 01:54:09.000000 cloup-2.1.0/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-15 01:54:09.000000 cloup-2.1.0/.github/ISSUE_TEMPLATE/other.md
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-15 01:54:09.000000 cloup-2.1.0/.github/release.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-15 01:54:09.000000 cloup-2.1.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-15 01:54:09.000000 cloup-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-15 01:54:09.000000 cloup-2.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-05-15 01:54:09.000000 cloup-2.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-15 01:54:09.000000 cloup-2.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-15 01:54:09.000000 cloup-2.1.0/CREDITS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-15 01:54:09.000000 cloup-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-15 01:54:09.000000 cloup-2.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-05-15 01:54:24.000000 cloup-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-15 01:54:09.000000 cloup-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup/
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29113 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/_option_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/_params.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/_sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/constraints/_conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/constraints/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/constraints/_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/constraints/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/constraints/conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/constraints/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup/formatting/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/formatting/_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/formatting/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/formatting/sep.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/styling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-15 01:54:09.000000 cloup-2.1.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/docs/_autoapi_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/docs/_autoapi_templates/python/
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/_autoapi_templates/python/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    57493 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/_static/basic-example.png
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/_static/logo-dark-mode.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/_static/logo-on-white.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/docs/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/_static/styles/extensions-overrides.css
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/_static/styles/theme-overrides.css
--rw-r--r--   0 runner    (1001) docker     (123)    62855 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/_static/theme-elems.png
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/docs/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/aliases.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/arguments.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    20026 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/constraints.rst
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/credits.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13553 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/formatting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/misc.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/option-groups.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/sections.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-15 01:54:09.000000 cloup-2.1.0/examples/arguments_with_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-15 01:54:09.000000 cloup-2.1.0/examples/default_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-15 01:54:09.000000 cloup-2.1.0/examples/flat_option_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-15 01:54:09.000000 cloup-2.1.0/examples/git_sections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/examples/manim/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-15 01:54:09.000000 cloup-2.1.0/examples/manim/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-15 01:54:09.000000 cloup-2.1.0/examples/manim/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-15 01:54:09.000000 cloup-2.1.0/examples/manim/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-15 01:54:09.000000 cloup-2.1.0/examples/option_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-15 01:54:09.000000 cloup-2.1.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-05-15 01:54:09.000000 cloup-2.1.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-15 01:54:09.000000 cloup-2.1.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-15 01:54:09.000000 cloup-2.1.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 01:54:09.000000 cloup-2.1.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-15 01:54:09.000000 cloup-2.1.0/requirements/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-15 01:54:09.000000 cloup-2.1.0/scripts/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-15 01:54:09.000000 cloup-2.1.0/scripts/copytree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-15 01:54:09.000000 cloup-2.1.0/scripts/generate_git_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-15 01:54:09.000000 cloup-2.1.0/scripts/make-help.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-15 01:54:09.000000 cloup-2.1.0/scripts/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-15 01:54:24.000000 cloup-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-15 01:54:09.000000 cloup-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/tests/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/constraints/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/constraints/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/constraints/test_conditional_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    14505 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/constraints/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/constraints/test_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/example_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/example_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/test_aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/test_option_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/test_sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/test_sep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/test_styling.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-15 01:54:09.000000 cloup-2.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-03 14:20:28.000000 cloup-2.1.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 14:20:28.000000 cloup-2.1.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-03 14:20:28.000000 cloup-2.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-03 14:20:28.000000 cloup-2.1.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-03 14:20:28.000000 cloup-2.1.1/.github/ISSUE_TEMPLATE/enhancement.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-03 14:20:28.000000 cloup-2.1.1/.github/ISSUE_TEMPLATE/other.md
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-03 14:20:28.000000 cloup-2.1.1/.github/release.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-03 14:20:28.000000 cloup-2.1.1/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-03 14:20:28.000000 cloup-2.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-03 14:20:28.000000 cloup-2.1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-06-03 14:20:28.000000 cloup-2.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-03 14:20:28.000000 cloup-2.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-03 14:20:28.000000 cloup-2.1.1/CREDITS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-03 14:20:28.000000 cloup-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-03 14:20:28.000000 cloup-2.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-06-03 14:20:39.000000 cloup-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-06-03 14:20:28.000000 cloup-2.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup/
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29113 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/_option_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/_params.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/_sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/constraints/_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/constraints/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/constraints/_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/constraints/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/constraints/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/constraints/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup/formatting/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17385 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/formatting/_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/formatting/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/formatting/sep.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/styling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-03 14:20:28.000000 cloup-2.1.1/cloup/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-03 14:20:39.000000 cloup-2.1.1/cloup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-03 14:20:28.000000 cloup-2.1.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/docs/_autoapi_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/docs/_autoapi_templates/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/_autoapi_templates/python/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    57493 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/_static/basic-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/_static/logo-dark-mode.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/_static/logo-on-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/docs/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/_static/styles/extensions-overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/_static/styles/theme-overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)    62855 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/_static/theme-elems.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/docs/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/aliases.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/arguments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20026 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/constraints.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13553 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/formatting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/option-groups.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-06-03 14:20:28.000000 cloup-2.1.1/docs/pages/sections.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-03 14:20:28.000000 cloup-2.1.1/examples/arguments_with_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-03 14:20:28.000000 cloup-2.1.1/examples/default_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-03 14:20:28.000000 cloup-2.1.1/examples/flat_option_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-06-03 14:20:28.000000 cloup-2.1.1/examples/git_sections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/examples/manim/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-03 14:20:28.000000 cloup-2.1.1/examples/manim/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-03 14:20:28.000000 cloup-2.1.1/examples/manim/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-03 14:20:28.000000 cloup-2.1.1/examples/manim/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-03 14:20:28.000000 cloup-2.1.1/examples/option_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-03 14:20:28.000000 cloup-2.1.1/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-06-03 14:20:28.000000 cloup-2.1.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-03 14:20:28.000000 cloup-2.1.1/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-03 14:20:28.000000 cloup-2.1.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 14:20:28.000000 cloup-2.1.1/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-03 14:20:28.000000 cloup-2.1.1/requirements/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-03 14:20:28.000000 cloup-2.1.1/scripts/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-03 14:20:28.000000 cloup-2.1.1/scripts/copytree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-06-03 14:20:28.000000 cloup-2.1.1/scripts/generate_git_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-03 14:20:28.000000 cloup-2.1.1/scripts/make-help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-03 14:20:28.000000 cloup-2.1.1/scripts/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-03 14:20:39.000000 cloup-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-03 14:20:28.000000 cloup-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:39.000000 cloup-2.1.1/tests/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/constraints/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/constraints/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/constraints/test_conditional_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14505 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/constraints/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/constraints/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/example_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/example_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/test_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/test_option_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/test_sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/test_sep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/test_styling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-03 14:20:28.000000 cloup-2.1.1/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-03 14:20:28.000000 cloup-2.1.1/tox.ini
```

### Comparing `cloup-2.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `cloup-2.1.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/.github/workflows/tests.yaml` & `cloup-2.1.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/.gitignore` & `cloup-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/CHANGELOG.rst` & `cloup-2.1.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/CONTRIBUTING.rst` & `cloup-2.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/CREDITS.rst` & `cloup-2.1.1/CREDITS.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/LICENSE` & `cloup-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/Makefile` & `cloup-2.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/PKG-INFO` & `cloup-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloup
-Version: 2.1.0
+Version: 2.1.1
 Summary: Adds features to Click: option groups, constraints, subcommand sections and help themes.
 Home-page: https://github.com/janLuke/cloup
 Author: Gianluca Gippetto
 Author-email: gianluca.gippetto@gmail.com
 License: BSD 3-Clause
 Keywords: CLI,click,argument groups,option groups,constraints,help colors,help themes,help styles
 Classifier: Intended Audience :: Developers
```

### Comparing `cloup-2.1.0/README.rst` & `cloup-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup/__init__.py` & `cloup-2.1.1/cloup/__init__.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup/_commands.py` & `cloup-2.1.1/cloup/_commands.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup/_context.py` & `cloup-2.1.1/cloup/_context.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup/_option_groups.py` & `cloup-2.1.1/cloup/_option_groups.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup/_params.py` & `cloup-2.1.1/cloup/_params.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup/_params.pyi` & `cloup-2.1.1/cloup/_params.pyi`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup/_sections.py` & `cloup-2.1.1/cloup/_sections.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup/_util.py` & `cloup-2.1.1/cloup/_util.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup/constraints/__init__.py` & `cloup-2.1.1/cloup/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup/constraints/_conditional.py` & `cloup-2.1.1/cloup/constraints/_conditional.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup/constraints/_core.py` & `cloup-2.1.1/cloup/constraints/_core.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup/constraints/_support.py` & `cloup-2.1.1/cloup/constraints/_support.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup/constraints/common.py` & `cloup-2.1.1/cloup/constraints/common.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup/constraints/conditions.py` & `cloup-2.1.1/cloup/constraints/conditions.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup/constraints/exceptions.py` & `cloup-2.1.1/cloup/constraints/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup/formatting/_formatter.py` & `cloup-2.1.1/cloup/formatting/_formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,18 +164,18 @@
     def available_width(self) -> int:
         return self.width - self.current_indent
 
     def write(self, *strings: str) -> None:
         self.buffer += strings
 
     def write_usage(
-        self, prog: str, args: str = "", prefix: Optional[str] = 'Usage:'
+        self, prog: str, args: str = "", prefix: Optional[str] = None
     ) -> None:
-        if prefix:
-            prefix = self.theme.heading(prefix + ' ')
+        prefix = "Usage:" if prefix is None else prefix
+        prefix = self.theme.heading(prefix) + " "
         prog = self.theme.invoked_command(prog)
         super().write_usage(prog, args, prefix)
 
     def write_aliases(self, aliases: Sequence[str]) -> None:
         self.write_heading("Aliases", newline=False)
         alias_list = ", ".join(self.theme.col1(alias) for alias in aliases)
         self.write(f" {alias_list}\n")
```

### Comparing `cloup-2.1.0/cloup/formatting/_util.py` & `cloup-2.1.1/cloup/formatting/_util.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup/formatting/sep.py` & `cloup-2.1.1/cloup/formatting/sep.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup/styling.py` & `cloup-2.1.1/cloup/styling.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup/types.py` & `cloup-2.1.1/cloup/types.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup/typing.py` & `cloup-2.1.1/cloup/typing.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/cloup.egg-info/PKG-INFO` & `cloup-2.1.1/cloup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloup
-Version: 2.1.0
+Version: 2.1.1
 Summary: Adds features to Click: option groups, constraints, subcommand sections and help themes.
 Home-page: https://github.com/janLuke/cloup
 Author: Gianluca Gippetto
 Author-email: gianluca.gippetto@gmail.com
 License: BSD 3-Clause
 Keywords: CLI,click,argument groups,option groups,constraints,help colors,help themes,help styles
 Classifier: Intended Audience :: Developers
```

### Comparing `cloup-2.1.0/cloup.egg-info/SOURCES.txt` & `cloup-2.1.1/cloup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/docs/Makefile` & `cloup-2.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/docs/_autoapi_templates/python/module.rst` & `cloup-2.1.1/docs/_autoapi_templates/python/module.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/docs/_static/basic-example.png` & `cloup-2.1.1/docs/_static/basic-example.png`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/docs/_static/logo-dark-mode.svg` & `cloup-2.1.1/docs/_static/logo-dark-mode.svg`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/docs/_static/logo-on-white.svg` & `cloup-2.1.1/docs/_static/logo-on-white.svg`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/docs/_static/logo.svg` & `cloup-2.1.1/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/docs/_static/styles/extensions-overrides.css` & `cloup-2.1.1/docs/_static/styles/extensions-overrides.css`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/docs/_static/styles/theme-overrides.css` & `cloup-2.1.1/docs/_static/styles/theme-overrides.css`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/docs/_static/theme-elems.png` & `cloup-2.1.1/docs/_static/theme-elems.png`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/docs/conf.py` & `cloup-2.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/docs/index.rst` & `cloup-2.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/docs/make.bat` & `cloup-2.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/docs/pages/aliases.rst` & `cloup-2.1.1/docs/pages/aliases.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/docs/pages/arguments.rst` & `cloup-2.1.1/docs/pages/arguments.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/docs/pages/constraints.rst` & `cloup-2.1.1/docs/pages/constraints.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/docs/pages/formatting.rst` & `cloup-2.1.1/docs/pages/formatting.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/docs/pages/installation.rst` & `cloup-2.1.1/docs/pages/installation.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/docs/pages/option-groups.rst` & `cloup-2.1.1/docs/pages/option-groups.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/docs/pages/sections.rst` & `cloup-2.1.1/docs/pages/sections.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/examples/arguments_with_help.py` & `cloup-2.1.1/examples/arguments_with_help.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/examples/default_command.py` & `cloup-2.1.1/examples/default_command.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/examples/flat_option_groups.py` & `cloup-2.1.1/examples/flat_option_groups.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/examples/git_sections.py` & `cloup-2.1.1/examples/git_sections.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/examples/manim/config.py` & `cloup-2.1.1/examples/manim/config.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/examples/manim/main.py` & `cloup-2.1.1/examples/manim/main.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/examples/manim/render.py` & `cloup-2.1.1/examples/manim/render.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/examples/option_groups.py` & `cloup-2.1.1/examples/option_groups.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/requirements/dev.txt` & `cloup-2.1.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/requirements/docs.txt` & `cloup-2.1.1/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/requirements/test.txt` & `cloup-2.1.1/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/scripts/generate_git_example.py` & `cloup-2.1.1/scripts/generate_git_example.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/scripts/remove.py` & `cloup-2.1.1/scripts/remove.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/setup.py` & `cloup-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/tests/conftest.py` & `cloup-2.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/tests/constraints/conftest.py` & `cloup-2.1.1/tests/constraints/conftest.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/tests/constraints/test_common.py` & `cloup-2.1.1/tests/constraints/test_common.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/tests/constraints/test_conditional_constraints.py` & `cloup-2.1.1/tests/constraints/test_conditional_constraints.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/tests/constraints/test_constraints.py` & `cloup-2.1.1/tests/constraints/test_constraints.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/tests/constraints/test_support.py` & `cloup-2.1.1/tests/constraints/test_support.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/tests/example_command.py` & `cloup-2.1.1/tests/example_command.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/tests/example_group.py` & `cloup-2.1.1/tests/example_group.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/tests/test_aliases.py` & `cloup-2.1.1/tests/test_aliases.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/tests/test_commands.py` & `cloup-2.1.1/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/tests/test_context.py` & `cloup-2.1.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/tests/test_formatting.py` & `cloup-2.1.1/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/tests/test_option_groups.py` & `cloup-2.1.1/tests/test_option_groups.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/tests/test_sections.py` & `cloup-2.1.1/tests/test_sections.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/tests/test_sep.py` & `cloup-2.1.1/tests/test_sep.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/tests/test_styling.py` & `cloup-2.1.1/tests/test_styling.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/tests/test_util.py` & `cloup-2.1.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/tests/util.py` & `cloup-2.1.1/tests/util.py`

 * *Files identical despite different names*

### Comparing `cloup-2.1.0/tox.ini` & `cloup-2.1.1/tox.ini`

 * *Files identical despite different names*

