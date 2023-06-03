# Comparing `tmp/django-bootstrap5-23.2.dev0.tar.gz` & `tmp/django_bootstrap5-23.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bootstrap5-23.2.dev0.tar", last modified: Fri Apr 28 13:44:45 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `django-bootstrap5-23.2.dev0.tar` & `django_bootstrap5-23.3.tar`

### file list

```diff
@@ -1,95 +1,398 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.030165 django-bootstrap5-23.2.dev0/
--rw-r--r--   0 dylan      (501) staff       (20)      757 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/AUTHORS
--rw-r--r--   0 dylan      (501) staff       (20)     1533 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/LICENSE
--rw-r--r--   0 dylan      (501) staff       (20)      281 2023-04-23 08:55:44.000000 django-bootstrap5-23.2.dev0/MANIFEST.in
--rw-r--r--   0 dylan      (501) staff       (20)     3593 2023-04-28 13:44:45.030238 django-bootstrap5-23.2.dev0/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)     2483 2023-04-28 11:37:05.000000 django-bootstrap5-23.2.dev0/README.md
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.019418 django-bootstrap5-23.2.dev0/docs/
--rw-r--r--   0 dylan      (501) staff       (20)       30 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/docs/changelog.rst
--rw-r--r--   0 dylan      (501) staff       (20)     1023 2023-04-28 13:17:05.000000 django-bootstrap5-23.2.dev0/docs/conf.py
--rw-r--r--   0 dylan      (501) staff       (20)      577 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/docs/example_template.rst
--rw-r--r--   0 dylan      (501) staff       (20)     3276 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/docs/forms.rst
--rw-r--r--   0 dylan      (501) staff       (20)      249 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/docs/index.rst
--rw-r--r--   0 dylan      (501) staff       (20)      585 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/docs/installation.rst
--rw-r--r--   0 dylan      (501) staff       (20)       28 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/docs/migrate.rst
--rw-r--r--   0 dylan      (501) staff       (20)      665 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/docs/quickstart.rst
--rw-r--r--   0 dylan      (501) staff       (20)       62 2023-04-28 13:18:42.000000 django-bootstrap5-23.2.dev0/docs/requirements.txt
--rw-r--r--   0 dylan      (501) staff       (20)     3275 2022-10-14 14:58:03.000000 django-bootstrap5-23.2.dev0/docs/settings.rst
--rw-r--r--   0 dylan      (501) staff       (20)     1364 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/docs/templates.rst
--rw-r--r--   0 dylan      (501) staff       (20)     2217 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/docs/templatetags.rst
--rw-r--r--   0 dylan      (501) staff       (20)      799 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/docs/widgets.rst
--rwxr-xr-x   0 dylan      (501) staff       (20)      252 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/manage.py
--rw-r--r--   0 dylan      (501) staff       (20)     1376 2023-04-28 13:17:05.000000 django-bootstrap5-23.2.dev0/pyproject.toml
--rw-r--r--   0 dylan      (501) staff       (20)     1129 2023-04-28 13:44:45.030502 django-bootstrap5-23.2.dev0/setup.cfg
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.015115 django-bootstrap5-23.2.dev0/src/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.021272 django-bootstrap5-23.2.dev0/src/django_bootstrap5/
--rw-r--r--   0 dylan      (501) staff       (20)       55 2023-04-28 13:44:39.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     2351 2022-08-05 14:34:59.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/components.py
--rw-r--r--   0 dylan      (501) staff       (20)     2692 2023-04-23 08:55:44.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/core.py
--rw-r--r--   0 dylan      (501) staff       (20)      621 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/css.py
--rw-r--r--   0 dylan      (501) staff       (20)     1482 2022-10-15 06:32:49.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/forms.py
--rw-r--r--   0 dylan      (501) staff       (20)      870 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/html.py
--rw-r--r--   0 dylan      (501) staff       (20)    21153 2022-11-22 12:41:26.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/renderers.py
--rw-r--r--   0 dylan      (501) staff       (20)      901 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/size.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.015227 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.023075 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/
--rw-r--r--   0 dylan      (501) staff       (20)     1079 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/bootstrap5.html
--rw-r--r--   0 dylan      (501) staff       (20)       95 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/field_errors.html
--rw-r--r--   0 dylan      (501) staff       (20)       79 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/field_help_text.html
--rw-r--r--   0 dylan      (501) staff       (20)      122 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/form_errors.html
--rw-r--r--   0 dylan      (501) staff       (20)      206 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/messages.html
--rw-r--r--   0 dylan      (501) staff       (20)     1762 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/pagination.html
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.023568 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/widgets/
--rw-r--r--   0 dylan      (501) staff       (20)      895 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/widgets/clearable_file_input.html
--rw-r--r--   0 dylan      (501) staff       (20)     1052 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select.html
--rw-r--r--   0 dylan      (501) staff       (20)      670 2022-10-15 06:09:49.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select_button_group.html
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.024008 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templatetags/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templatetags/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)    19229 2023-04-02 08:04:04.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/templatetags/django_bootstrap5.py
--rw-r--r--   0 dylan      (501) staff       (20)      467 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/text.py
--rw-r--r--   0 dylan      (501) staff       (20)     1497 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/utils.py
--rw-r--r--   0 dylan      (501) staff       (20)      745 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5/widgets.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.022189 django-bootstrap5-23.2.dev0/src/django_bootstrap5.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)     3593 2023-04-28 13:44:45.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)     2693 2023-04-28 13:44:45.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2023-04-28 13:44:45.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2021-12-12 13:27:59.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5.egg-info/not-zip-safe
--rw-r--r--   0 dylan      (501) staff       (20)       12 2023-04-28 13:44:45.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5.egg-info/requires.txt
--rw-r--r--   0 dylan      (501) staff       (20)       18 2023-04-28 13:44:45.000000 django-bootstrap5-23.2.dev0/src/django_bootstrap5.egg-info/top_level.txt
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.029483 django-bootstrap5-23.2.dev0/tests/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/__init__.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-04-28 13:44:45.029925 django-bootstrap5-23.2.dev0/tests/app/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/app/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     1703 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/app/settings.py
--rw-r--r--   0 dylan      (501) staff       (20)       17 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/app/urls.py
--rw-r--r--   0 dylan      (501) staff       (20)      836 2021-12-27 05:56:30.000000 django-bootstrap5-23.2.dev0/tests/base.py
--rw-r--r--   0 dylan      (501) staff       (20)     3439 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/image.py
--rw-r--r--   0 dylan      (501) staff       (20)     1595 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_alert.py
--rw-r--r--   0 dylan      (501) staff       (20)     2698 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_button.py
--rw-r--r--   0 dylan      (501) staff       (20)     2024 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_css_and_js_tags.py
--rw-r--r--   0 dylan      (501) staff       (20)     3065 2022-10-15 06:31:02.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field.py
--rw-r--r--   0 dylan      (501) staff       (20)     3343 2021-12-27 05:56:30.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_datetime.py
--rw-r--r--   0 dylan      (501) staff       (20)     3521 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_input_checkbox.py
--rw-r--r--   0 dylan      (501) staff       (20)     2120 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_input_color.py
--rw-r--r--   0 dylan      (501) staff       (20)     3150 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_input_file.py
--rw-r--r--   0 dylan      (501) staff       (20)     2003 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_input_range.py
--rw-r--r--   0 dylan      (501) staff       (20)    12018 2023-04-23 08:55:44.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_input_text.py
--rw-r--r--   0 dylan      (501) staff       (20)     3657 2023-04-23 08:55:44.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_parameters.py
--rw-r--r--   0 dylan      (501) staff       (20)     4590 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_radio_select.py
--rw-r--r--   0 dylan      (501) staff       (20)     2240 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_select.py
--rw-r--r--   0 dylan      (501) staff       (20)     1340 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_textarea.py
--rw-r--r--   0 dylan      (501) staff       (20)     6094 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_form.py
--rw-r--r--   0 dylan      (501) staff       (20)     1634 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_formset.py
--rw-r--r--   0 dylan      (501) staff       (20)      869 2022-10-15 06:31:02.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_label.py
--rw-r--r--   0 dylan      (501) staff       (20)     2934 2022-08-05 14:34:59.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_messages.py
--rw-r--r--   0 dylan      (501) staff       (20)     6807 2023-04-25 10:31:45.000000 django-bootstrap5-23.2.dev0/tests/test_bootstrap_pagination.py
--rw-r--r--   0 dylan      (501) staff       (20)     2600 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_components.py
--rw-r--r--   0 dylan      (501) staff       (20)      839 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_css.py
--rw-r--r--   0 dylan      (501) staff       (20)      511 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_html.py
--rw-r--r--   0 dylan      (501) staff       (20)      515 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_settings.py
--rw-r--r--   0 dylan      (501) staff       (20)     1149 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_size.py
--rw-r--r--   0 dylan      (501) staff       (20)      852 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_templates.py
--rw-r--r--   0 dylan      (501) staff       (20)      556 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_text.py
--rw-r--r--   0 dylan      (501) staff       (20)     1257 2023-04-23 08:55:44.000000 django-bootstrap5-23.2.dev0/tests/test_urls.py
--rw-r--r--   0 dylan      (501) staff       (20)      315 2021-12-12 13:22:34.000000 django-bootstrap5-23.2.dev0/tests/test_version.py
--rw-r--r--   0 dylan      (501) staff       (20)     2033 2023-04-28 13:20:24.000000 django-bootstrap5-23.2.dev0/tox.ini
+-rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.DS_Store
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.readthedocs.yml
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/CHANGELOG.md
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/MIGRATE.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/Makefile
+-rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/manage.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.github/workflows/dependabot-auto-approve-and-merge.yml
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/10863d782de422d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/10fe5d770f046ee9
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/11cd065b380d3eac
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/1225164498a1e2c3
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/122b715713289559
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/12b0dbba75cf026b
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/12fa33ec33f3d42e
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/1311838226113b93
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/1507bd100a6bb616
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/1583d5542ac253fc
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/15e6cefade6acae3
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/1681d9d6a7b9147d
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/16b86702d3379319
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/181138f8bc11db61
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/182218b58fd14a79
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/1b46db97a0bd510
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/1bc7d510d7f56cb
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/1c85a26be60f6bd7
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/1c8eb5b5a4b904e6
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/1d5996c7bd14c775
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/1f87ca16c7719913
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/1fe859b78181088
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/2134f48316380e2d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/21ff11a6f6330667
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/2205b664579ec9a9
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/227526d97d1e267c
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/22beb1518113df6d
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/23382b94347e37a9
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/25baefbb672db3b0
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/25e11b72bfa62337
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/2616c4995a93f199
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/2656e03f2206207e
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/269b6640bd377364
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/271cea175d8c1ade
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/27ad4920bfacb7be
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/29b0da840df8787b
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/29b94ea3486967c0
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/29c092abdbe01e8c
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/2a019f67e2b807f7
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/2a04dafe0e3a1a94
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/2b21c87dbb42790
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/2cd5cc0b11b41b78
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/2edea93924426899
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/2f4fe2a730b6fa76
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/2f5a807bc6470ef3
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/2fe47b8a651667f
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/2fe8bd6968889123
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/30499e19b1fd41dd
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/308923df94205e1f
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/372e68420f47f1bc
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/3773d62dc579d159
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/37ad7ac989bb6e71
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/37c564f4cbefae67
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/3959f0e94715778
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/39b1698b680bbd42
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/3acc3efdae26213b
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/3b4a2adfceb8db37
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/3bffe0eb3c4e13ba
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/3c9258c9050817f7
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/3dccf8bb532b8229
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/4201fd4b8eb9ac32
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/43022e1e5fa18012
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/4386fb965b556be9
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/4473df1761979a4c
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/4480e020ec341dd7
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/4862c5f14d916b14
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/4a5c213d86d5809
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/4ad3b7dd45b7fc2e
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/4b0b966f6aff7339
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/4cdc3470137f3eca
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/4da90a9b5a7dd6e
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/4e957a2da03a29ba
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/4eef699e296a65b4
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/4f70301cdf41f67d
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/4fdb5e8ba1a2cf54
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/5047573e22b2be19
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/50cd38caedfc5fb5
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/50f2b5d95d50b293
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/53b93ef46ee774aa
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/54715ef113526e72
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/5569ae43929d6a88
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/579153fbc6cbc57f
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/57e7b65c6c28effd
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/58168cb2404f008c
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/58bdbb8ab6ef4450
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/58cba685f49a59c7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/58e1a39955556d9c
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/59385c5680eb5c43
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/59a22c43cc02f19
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/5a0b5e93af8590a6
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/5beadff814ec202f
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/5cb315ea10adba7e
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/5cdc386661335b78
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/5da51997fd1e5514
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/5e36e26a8b066a26
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/5f922ecc11bfbb06
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/5fb3aab0bf1805a3
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/5fe4f030cdea2ea2
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/60fe30696a3a500
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/61637fab9e3e0bab
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/6189745aba226d0
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/6276024ba5ef74c7
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/633096650392ef
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/63e955e6f0553afd
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/6421b7ddd2f221c8
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/643d500fbbfccadd
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/64584219ab387d55
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/64c6c10281630a60
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/651de1bf692fe176
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/6585ab889c9feed7
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/6603a052252ba004
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/668520781b664ff3
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/67c58915a7da85b3
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/67de119a9f48cd6c
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/68503b379935d42e
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/6852d6c354a69264
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/6883e8f4dd570dfe
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/68968d095dab9247
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/6b4c70527b27c66a
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/6f9b61264218d443
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/7058662657ff6fa6
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/70bae877097fd633
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/70c7e3bfbd447243
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/72037b0959509207
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/72087aee6a7d69fd
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/744f461c107389be
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/758272a9fbdef326
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/75e0f48a6790aa72
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/75fd89ab0fe0cea3
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/761de2a40b4b0548
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/7627b09ea8d63eaa
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/7734d95a087c7673
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/775db88c2533d589
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/780573dba6012d32
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/78295c737610b448
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/78cf9ea64d455135
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/7dcc08eb43742433
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/7ea28688efeed69a
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/7ea32022c4113cb0
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/7eec2bd3c1b3bc13
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/8031649caa3cc1ae
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/82050e68d42880df
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/82804d86f34cad91
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/82a24234febfaacb
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/835ab18683012e94
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/843c4264852a62e4
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/859780852307959a
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/861f43af3b6d214c
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/86961cb0bf57c203
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/870158f3b3bbb978
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/87976675f1a0d7b8
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/88452bba47e05883
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/8853623ebd69e0d6
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/891b7b828127ec96
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/893ab48047938aee
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/897c6e06883bf8af
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/8b5c2c8714a5959e
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/8d3ce2b5f8b599e8
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/8d55e216ce3ee63b
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/8d5cb4e9681936e9
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/8e0fadbc747b2373
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/8e94baa9e216bb77
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/8f038b2a113d9184
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/903be52ff672b9c2
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/909ffc9b194248cf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/90f566459dac02ab
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/916b685aa5f9af8e
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/91edf1b7664c94c2
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/935449a3a8ab7de
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/943243eee30d3aa0
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/9496bf0fb42ff51a
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/94f507678591b0db
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/95448205af9c61ad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/9591cf005e3cf70c
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/96dfed638f910d43
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/9787bc52b60a4972
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/987425672cfd5c16
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/9b070a70d30fae98
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/9e22dc2323847ab1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/9f55f35e72ec01af
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/a00e9ebe1fe3ea27
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/a11c073601164ae7
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/a212cb71be4375c0
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/a3410894b1759c13
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/a387f8ad3262b284
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/a3ae861257a87f9b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/a44b0a25ee9c11a4
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/a47f795d12c16795
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/a66f4c880154f7fc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/a67137df72ca5dd9
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/a7503c49f4eae8a
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/a81b31e5977fe54c
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/aa8a7e4606951d3f
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/aa8b9f84a9212fc0
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/aad1fe125b50060d
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/ab1aee3d0bac6582
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/ac76b25ad36a910f
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/aedfb61e71d36077
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/af4e883866e0934b
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/b03ac96f0c13f2b0
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/b145e5cfee68a416
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/b22c8ded186f4d1d
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/b333daf4e267d445
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/b3977f07f36a998e
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/b43783a04eb0a6b1
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/b6fd9f8c20f33945
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/b74a6c0623698d6b
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/b913173c7f36dfd
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/b9fcdc19c381c65c
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/bb9365b683ad614
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/bba335b16a7cb12e
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/bbf4ec57c6a097be
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/bdc7ec67adc405a9
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/c0507a0c61052764
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/c0a70c805615e78f
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/c0df89a8265adfe4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/c1a6096f8934dc40
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/c1b1946958ea5205
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/c3444f65b8b64531
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/c49b2760a18c6d8d
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/c5cd6a57d7c29b83
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/c62ff5d6bf6d39ce
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/c644ae3db145c9ae
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/c652b00a6ac9c07
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/c65705662f405136
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/c78b0108312514a4
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/c7bf43c2e2db9f5d
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/c847d8a230c8fa85
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/c94d9b8d1c2d981
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/ca1d0c1e53a57ffc
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/cabab8833b54cbba
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/cad5488342025ab1
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/cb291a0b8598439a
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/cd298fcdcbc99b63
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/ce3593fc5c2d7768
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/ceddd901d914dd16
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/cf3d9e1d14c318c3
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/d14f17b1a6ddc84f
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/d1612c2701601799
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/d1b21806897163ef
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/d3604dc5e67dae63
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/d366e25fa8f0c1cf
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/d40ab6e17b6d7c8
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/d6e95bbb6742cfab
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/d87c59ac694a46b1
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/d8cfe052cd41eff2
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/d9a10fba1eb779f8
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/da8291dabeebe6bc
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/da9eebf70447e329
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/dc0c321b58900bb7
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/dd5aecccc36ea6a1
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/dda40bf0ac46c84f
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/ddf2cec008af26b4
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/de35ba519c356b8b
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/de7705f960697eb2
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/de8cf62f04d065b3
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/dfedab7158f6a69c
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/e0575ac948aab754
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/e0b8d37020c090ab
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/e1f95e877e6b1283
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/e29b50a18f410762
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/e2bcfb886083a2
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/e356e382d398c4b0
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/e504c49fbc5ed36c
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/e50fbd80950509dc
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/e66c888491f05f00
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/e7ba2648572feb2d
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/e82d41b8bd902207
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/e954ca260f6431aa
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/ed57c525feb0ce13
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/f1891d473579419d
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/f1c41e98b28af43f
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/f20ffb512ad3eaa3
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/f25781a1aac7a97
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/f2ae430687564b18
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/f3321fe8e95a52d4
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/f3469c9c7375f9e8
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/f503987a27669a67
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/f526732c6003bfda
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/f5e00122a327efda
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/f5f1271a1c02e968
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/f684f73621b4276
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/f7abb2d9c7da8bb3
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/f7b9ce59577fcb89
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/f7eadae27513fee8
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/f88143d444f7c9e6
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/f8c762b669482db7
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/fa715b7faedc73cc
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/fadb3013794231a4
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/fb3669f2427ea155
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.ruff_cache/content/fbc329e3a5865c9f
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.vscode/settings.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/docs/changelog.rst
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/docs/conf.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/docs/contributing.rst
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/docs/example_template.rst
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/docs/forms.rst
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/docs/index.rst
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/docs/installation.rst
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/docs/migrate.rst
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/docs/quickstart.rst
+-rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/docs/settings.rst
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/docs/templates.rst
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/docs/templatetags.rst
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/docs/widgets.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/example/__init__.py
+-rwxr-xr-x   0        0        0      242 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/example/manage.py
+-rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/example/settings.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/example/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/example/app/__init__.py
+-rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/example/app/forms.py
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/example/app/views.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/example/templates/app/base.html
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/example/templates/app/bootstrap.html
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/example/templates/app/form.html
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/example/templates/app/form_by_field.html
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/example/templates/app/form_horizontal.html
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/example/templates/app/form_inline.html
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/example/templates/app/form_with_files.html
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/example/templates/app/formset.html
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/example/templates/app/home.html
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/example/templates/app/misc.html
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/example/templates/app/pagination.html
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/__about__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/__init__.py
+-rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/components.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/core.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/css.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/forms.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/html.py
+-rw-r--r--   0        0        0    21153 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/renderers.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/size.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/text.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/utils.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/widgets.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/templates/django_bootstrap5/bootstrap5.html
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/templates/django_bootstrap5/field_errors.html
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/templates/django_bootstrap5/field_help_text.html
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/templates/django_bootstrap5/form_errors.html
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/templates/django_bootstrap5/messages.html
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/templates/django_bootstrap5/pagination.html
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/templates/django_bootstrap5/widgets/clearable_file_input.html
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select.html
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select_button_group.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/templatetags/__init__.py
+-rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/src/django_bootstrap5/templatetags/django_bootstrap5.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/__init__.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/base.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/image.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_bootstrap_alert.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_bootstrap_button.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_bootstrap_css_and_js_tags.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_bootstrap_field.py
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_bootstrap_field_datetime.py
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_bootstrap_field_input_checkbox.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_bootstrap_field_input_color.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_bootstrap_field_input_file.py
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_bootstrap_field_input_range.py
+-rw-r--r--   0        0        0    12018 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_bootstrap_field_input_text.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_bootstrap_field_parameters.py
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_bootstrap_field_radio_select.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_bootstrap_field_select.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_bootstrap_field_textarea.py
+-rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_bootstrap_form.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_bootstrap_formset.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_bootstrap_label.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_bootstrap_messages.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_bootstrap_pagination.py
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_components.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_css.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_html.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_settings.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_size.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_templates.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_text.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_urls.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/app/__init__.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/app/settings.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/tests/app/urls.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/.gitignore
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/AUTHORS
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/LICENSE
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/README.md
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/pyproject.toml
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 django_bootstrap5-23.3/PKG-INFO
```

### Comparing `django-bootstrap5-23.2.dev0/AUTHORS` & `django_bootstrap5-23.3/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/LICENSE` & `django_bootstrap5-23.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/PKG-INFO` & `django_bootstrap5-23.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 Metadata-Version: 2.1
 Name: django-bootstrap5
-Version: 23.2.dev0
+Version: 23.3
 Summary: Bootstrap 5 for Django
-Home-page: https://github.com/zostera/django-bootstrap5
-Author: Dylan Verheul
-Author-email: dylan@dyve.net
-License: BSD-3-Clause
+Project-URL: Changelog, https://github.com/zostera/django-bootstrap5/blob/main/CHANGELOG.md
+Project-URL: Documentation, https://django-bootstrap5.readthedocs.io/
+Project-URL: Homepage, https://github.com/zostera/django-bootstrap5
+Project-URL: Issues, https://github.com/zostera/django-bootstrap5/issues
+Project-URL: Source, https://github.com/zostera/django-bootstrap5
+Author-email: Dylan Verheul <dylan@dyve.net>
+License-Expression: BSD-3-Clause
+License-File: AUTHORS
+License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
@@ -20,17 +25,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
+Requires-Dist: django>=3.2
 Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
 
 # django-bootstrap5
 
 [![CI](https://github.com/zostera/django-bootstrap5/workflows/CI/badge.svg?branch=main)](https://github.com/zostera/django-bootstrap5/actions?workflow=CI)
 [![Coverage Status](https://coveralls.io/repos/github/zostera/django-bootstrap5/badge.svg?branch=main)](https://coveralls.io/github/zostera/django-bootstrap5?branch=main)
 [![Latest PyPI version](https://img.shields.io/pypi/v/django-bootstrap5.svg)](https://pypi.python.org/pypi/django-bootstrap5)
 [![Any color you like](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
@@ -55,15 +59,15 @@
 
 The full documentation is at https://django-bootstrap5.readthedocs.io/
 
 ## Installation
 
 1. Install using pip:
 
-    ```bash
+    ```console
     pip install django-bootstrap5
     ```
 
 2. Add to `INSTALLED_APPS` in your `settings.py`:
 
    ```python
    INSTALLED_APPS = (
@@ -88,19 +92,18 @@
     {% bootstrap_button button_type="submit" content="OK" %}
     {% bootstrap_button button_type="reset" content="Cancel" %}
 </form>
 ```
 
 ## Example app
 
-An example app is provided in the folder `example`. You can run it with `python manage.py runserver`.
+An example app is provided in the folder `example`. You can run the example app with this command:
 
-```bash
-cd example
-python manage.py runserver
+```console
+make example
 ```
 
 ## Bugs and suggestions
 
 If you have found a bug or if you have a request for additional functionality, please use the issue tracker on GitHub.
 
 https://github.com/zostera/django-bootstrap5/issues
```

### Comparing `django-bootstrap5-23.2.dev0/README.md` & `django_bootstrap5-23.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 The full documentation is at https://django-bootstrap5.readthedocs.io/
 
 ## Installation
 
 1. Install using pip:
 
-    ```bash
+    ```console
     pip install django-bootstrap5
     ```
 
 2. Add to `INSTALLED_APPS` in your `settings.py`:
 
    ```python
    INSTALLED_APPS = (
@@ -58,19 +58,18 @@
     {% bootstrap_button button_type="submit" content="OK" %}
     {% bootstrap_button button_type="reset" content="Cancel" %}
 </form>
 ```
 
 ## Example app
 
-An example app is provided in the folder `example`. You can run it with `python manage.py runserver`.
+An example app is provided in the folder `example`. You can run the example app with this command:
 
-```bash
-cd example
-python manage.py runserver
+```console
+make example
 ```
 
 ## Bugs and suggestions
 
 If you have found a bug or if you have a request for additional functionality, please use the issue tracker on GitHub.
 
 https://github.com/zostera/django-bootstrap5/issues
```

### Comparing `django-bootstrap5-23.2.dev0/docs/example_template.rst` & `django_bootstrap5-23.3/docs/example_template.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/docs/forms.rst` & `django_bootstrap5-23.3/docs/forms.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/docs/installation.rst` & `django_bootstrap5-23.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/docs/quickstart.rst` & `django_bootstrap5-23.3/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/docs/settings.rst` & `django_bootstrap5-23.3/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/docs/templates.rst` & `django_bootstrap5-23.3/docs/templates.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/docs/templatetags.rst` & `django_bootstrap5-23.3/docs/templatetags.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/docs/widgets.rst` & `django_bootstrap5-23.3/docs/widgets.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/src/django_bootstrap5/components.py` & `django_bootstrap5-23.3/src/django_bootstrap5/components.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/src/django_bootstrap5/core.py` & `django_bootstrap5-23.3/src/django_bootstrap5/core.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/src/django_bootstrap5/css.py` & `django_bootstrap5-23.3/src/django_bootstrap5/css.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/src/django_bootstrap5/forms.py` & `django_bootstrap5-23.3/src/django_bootstrap5/forms.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/src/django_bootstrap5/html.py` & `django_bootstrap5-23.3/src/django_bootstrap5/html.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/src/django_bootstrap5/renderers.py` & `django_bootstrap5-23.3/src/django_bootstrap5/renderers.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/src/django_bootstrap5/size.py` & `django_bootstrap5-23.3/src/django_bootstrap5/size.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/bootstrap5.html` & `django_bootstrap5-23.3/src/django_bootstrap5/templates/django_bootstrap5/bootstrap5.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/pagination.html` & `django_bootstrap5-23.3/src/django_bootstrap5/templates/django_bootstrap5/pagination.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/widgets/clearable_file_input.html` & `django_bootstrap5-23.3/src/django_bootstrap5/templates/django_bootstrap5/widgets/clearable_file_input.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select.html` & `django_bootstrap5-23.3/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select_button_group.html` & `django_bootstrap5-23.3/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select_button_group.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/src/django_bootstrap5/templatetags/django_bootstrap5.py` & `django_bootstrap5-23.3/src/django_bootstrap5/templatetags/django_bootstrap5.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/src/django_bootstrap5/utils.py` & `django_bootstrap5-23.3/src/django_bootstrap5/utils.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/src/django_bootstrap5/widgets.py` & `django_bootstrap5-23.3/src/django_bootstrap5/widgets.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/app/settings.py` & `django_bootstrap5-23.3/tests/app/settings.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/base.py` & `django_bootstrap5-23.3/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/image.py` & `django_bootstrap5-23.3/tests/image.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_bootstrap_alert.py` & `django_bootstrap5-23.3/tests/test_bootstrap_alert.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_bootstrap_button.py` & `django_bootstrap5-23.3/tests/test_bootstrap_button.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_bootstrap_css_and_js_tags.py` & `django_bootstrap5-23.3/tests/test_bootstrap_css_and_js_tags.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field.py` & `django_bootstrap5-23.3/tests/test_bootstrap_field.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_datetime.py` & `django_bootstrap5-23.3/tests/test_bootstrap_field_datetime.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_input_checkbox.py` & `django_bootstrap5-23.3/tests/test_bootstrap_field_input_checkbox.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_input_color.py` & `django_bootstrap5-23.3/tests/test_bootstrap_field_input_color.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_input_file.py` & `django_bootstrap5-23.3/tests/test_bootstrap_field_input_file.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_input_range.py` & `django_bootstrap5-23.3/tests/test_bootstrap_field_input_range.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_input_text.py` & `django_bootstrap5-23.3/tests/test_bootstrap_field_input_text.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_parameters.py` & `django_bootstrap5-23.3/tests/test_bootstrap_field_parameters.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_radio_select.py` & `django_bootstrap5-23.3/tests/test_bootstrap_field_radio_select.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_select.py` & `django_bootstrap5-23.3/tests/test_bootstrap_field_select.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_bootstrap_field_textarea.py` & `django_bootstrap5-23.3/tests/test_bootstrap_field_textarea.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_bootstrap_form.py` & `django_bootstrap5-23.3/tests/test_bootstrap_form.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_bootstrap_formset.py` & `django_bootstrap5-23.3/tests/test_bootstrap_formset.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_bootstrap_label.py` & `django_bootstrap5-23.3/tests/test_bootstrap_label.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_bootstrap_messages.py` & `django_bootstrap5-23.3/tests/test_bootstrap_messages.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_bootstrap_pagination.py` & `django_bootstrap5-23.3/tests/test_bootstrap_pagination.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_components.py` & `django_bootstrap5-23.3/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_css.py` & `django_bootstrap5-23.3/tests/test_css.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_settings.py` & `django_bootstrap5-23.3/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_size.py` & `django_bootstrap5-23.3/tests/test_size.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_templates.py` & `django_bootstrap5-23.3/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_text.py` & `django_bootstrap5-23.3/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.2.dev0/tests/test_urls.py` & `django_bootstrap5-23.3/tests/test_urls.py`

 * *Files identical despite different names*

